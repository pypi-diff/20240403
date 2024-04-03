# Comparing `tmp/galaxy-tool-util-23.2.dev0.tar.gz` & `tmp/galaxy-tool-util-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-tool-util-23.2.dev0.tar", last modified: Fri Dec  8 17:38:41 2023, max compression
+gzip compressed data, was "galaxy-tool-util-24.0.0.tar", last modified: Wed Apr  3 02:45:02 2024, max compression
```

## Comparing `galaxy-tool-util-23.2.dev0.tar` & `galaxy-tool-util-24.0.0.tar`

### file list

```diff
@@ -1,183 +1,184 @@
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.572075 galaxy-tool-util-23.2.dev0/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12583 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12875 2023-12-08 17:18:17.000000 galaxy-tool-util-23.2.dev0/LICENSE
--rw-r--r--   0 mvandenb   (501) wheel        (0)      331 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) wheel        (0)    14501 2023-12-08 17:38:41.571976 galaxy-tool-util-23.2.dev0/PKG-INFO
--rw-r--r--   0 mvandenb   (501) wheel        (0)      278 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/README.rst
--rw-r--r--   0 mvandenb   (501) wheel        (0)       89 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.543689 galaxy-tool-util-23.2.dev0/galaxy/
--rw-r--r--   0 mvandenb   (501) wheel        (0)       91 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/py.typed
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.545716 galaxy-tool-util-23.2.dev0/galaxy/tool_util/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/__init__.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.546311 galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      307 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1699 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/interface.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3570 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/source.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.546582 galaxy-tool-util-23.2.dev0/galaxy/tool_util/client/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/client/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    14527 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/client/staging.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.548441 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      515 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4109 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/cwltool_deps.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    45995 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/parser.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    18637 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/representation.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      939 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/runnable.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     9400 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/runtime_actions.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4075 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/schema.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    25744 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/util.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.548829 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    58982 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3009 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/_schema.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.549083 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/bundles/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/bundles/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     9761 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/bundles/models.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.552242 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    20484 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/__init__.py
--rwxr-xr-x   0 mvandenb   (501) wheel        (0)    19566 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/brew_exts.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1119 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/brew_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      396 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/commands.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2931 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/conda_compat.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    27435 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/conda_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    22826 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_classes.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.552963 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2687 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    10889 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/explicit.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    29672 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/mulled.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      587 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/test.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2461 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_volumes.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    18185 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/containers.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6766 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/dependencies.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     8104 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/docker_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2673 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/dockerfiles.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2466 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/installable.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.555141 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      422 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/_cli.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    11859 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/get_tests.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4029 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/invfile.lua
--rw-r--r--   0 mvandenb   (501) wheel        (0)    22233 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4090 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_channel.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3797 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_files.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1759 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_tool.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      887 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_hash.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5062 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_list.py
--rwxr-xr-x   0 mvandenb   (501) wheel        (0)    15814 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_search.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    10081 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    17250 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    13059 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/requirements.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.557118 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    11209 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5378 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    20607 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/conda.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      702 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5389 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/galaxy_packages.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2033 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/homebrew.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     7971 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/lmod.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     8887 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/modules.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2748 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/resolver_mixins.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3571 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     7542 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3855 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/singularity_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    18441 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/views.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2585 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/edam_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1098 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/fetcher.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12138 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/lint.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.559029 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/
--rw-r--r--   0 mvandenb   (501) wheel        (0)       64 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      333 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1565 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/citations.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1941 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/command.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1777 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/cwl.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3566 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/general.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1696 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/help.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    26292 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/inputs.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5769 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/outputs.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2604 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/stdio.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    10898 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/tests.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1751 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/xml_order.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      391 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/loader.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     9920 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/loader_directory.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.559722 galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      669 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2393 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/dockstore.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      250 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/file.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      483 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/http.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.560740 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    53080 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/biotools_mappings.tsv
--rw-r--r--   0 mvandenb   (501) wheel        (0)       52 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
--rw-r--r--   0 mvandenb   (501) wheel        (0)       27 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3651 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/ontology_data.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     8618 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/output_checker.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.563198 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      480 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5857 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/cwl.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4558 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/factory.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    19369 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/interface.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    25328 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_actions.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5865 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_collection_def.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    16163 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_objects.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4171 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/stdio.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      645 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    54564 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/xml.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    12882 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/yaml.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     9462 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/provided_metadata.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.564739 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      366 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    65008 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/base.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.565090 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/filters/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4454 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/filters/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4726 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/filters/examples.py.sample
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6939 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/integrated_panel.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.565764 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      108 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2522 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/factory.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2767 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/interface.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    10207 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/panel.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4812 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/parser.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.567022 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/
--rw-r--r--   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3778 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/definitions.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6819 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/edam.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2546 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/interface.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1685 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/sources.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     9250 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/static.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6880 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/watcher.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.567576 galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/
--rw-r--r--   0 mvandenb   (501) wheel        (0)      775 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1911 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/interactor.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      417 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/sample_data.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.568549 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    18679 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/__init__.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.569887 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4335 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/__init__.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3184 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/_util.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     3749 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/archive.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1416 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/hdf5.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1429 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/json.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      757 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/size.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1325 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/tabular.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5350 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/text.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     5298 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/xml.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    74237 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/interactor.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)    22843 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/script.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)      850 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/test_config.sample.yml
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4113 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/test_data.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1430 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/wait.py
--rw-r--r--   0 mvandenb   (501) wheel        (0)     4877 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/version.py
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.570482 galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1131 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/LICENSE
--rw-r--r--   0 mvandenb   (501) wheel        (0)     1079 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/README.md
--rw-r--r--   0 mvandenb   (501) wheel        (0)      694 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/galaxy.jxb
--rw-r--r--   0 mvandenb   (501) wheel        (0)   332235 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/galaxy.xsd
-drwxr-xr-x   0 mvandenb   (501) wheel        (0)        0 2023-12-08 17:38:41.571528 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/
--rw-r--r--   0 mvandenb   (501) wheel        (0)    14501 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) wheel        (0)     6004 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)        1 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)      653 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)      211 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)        7 2023-12-08 17:38:41.000000 galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) wheel        (0)       81 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/pyproject.toml
--rw-r--r--   0 mvandenb   (501) wheel        (0)     2111 2023-12-08 17:38:41.572348 galaxy-tool-util-23.2.dev0/setup.cfg
--rw-r--r--   0 mvandenb   (501) wheel        (0)       26 2023-12-08 17:18:18.000000 galaxy-tool-util-23.2.dev0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    22206 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.407017 galaxy-tool-util-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/client/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/cwltool_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45945 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runtime_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25745 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    59526 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.415017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19566 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_exts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27451 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.415017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/mulled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18185 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dockerfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/installable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.419017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/get_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/invfile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15814 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.419017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/galaxy_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/homebrew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/resolver_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/singularity_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/edam_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52233 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22415 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xml_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/loader_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/dockstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53080 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/biotools_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/ontology_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/output_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_collection_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54802 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/provided_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65232 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/examples.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/integrated_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/edam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)    21654 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75994 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22843 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_config.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.jxb
+-rw-r--r--   0 runner    (1001) docker     (127)   343351 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/test-requirements.txt
```

### Comparing `galaxy-tool-util-23.2.dev0/HISTORY.rst` & `galaxy-tool-util-24.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,180 @@
+Metadata-Version: 2.1
+Name: galaxy-tool-util
+Version: 24.0.0
+Summary: Galaxy tool and tool dependency utilities
+Home-page: https://github.com/galaxyproject/galaxy
+Author: Galaxy Project and Community
+Author-email: galaxy-committers@lists.galaxyproject.org
+License: AFL
+Keywords: Galaxy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Academic Free License (AFL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: galaxy-util>=22.1
+Requires-Dist: conda-package-streaming
+Requires-Dist: lxml!=4.2.2
+Requires-Dist: MarkupSafe
+Requires-Dist: packaging
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: sortedcontainers
+Requires-Dist: typing-extensions
+Provides-Extra: cwl
+Requires-Dist: cwltool>=3.1.20230624081518; extra == "cwl"
+Provides-Extra: mulled
+Requires-Dist: jinja2; extra == "mulled"
+Requires-Dist: Whoosh; extra == "mulled"
+Provides-Extra: edam
+Requires-Dist: edam-ontology; extra == "edam"
+Provides-Extra: extended-assertions
+Requires-Dist: numpy; extra == "extended-assertions"
+Requires-Dist: pysam; extra == "extended-assertions"
+Requires-Dist: pillow; extra == "extended-assertions"
+
+
+.. image:: https://badge.fury.io/py/galaxy-tool-util.svg
+   :target: https://pypi.org/project/galaxy-tool-util/
+
+
+Overview
+--------
+
+The Galaxy_ tool utilities.
+
+* Code: https://github.com/galaxyproject/galaxy/tree/dev/packages/tool_util
+
+.. _Galaxy: http://galaxyproject.org/
+
 History
 -------
 
 .. to_doc
 
--------
-23.2rc1
--------
+-------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* xsd: reorder choices for permissive boolean by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17187 <https://github.com/galaxyproject/galaxy/pull/17187>`_
+* Allow for upper case container tags by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17254 <https://github.com/galaxyproject/galaxy/pull/17254>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Escape pipe character in tool XSD docs by `@neoformit <https://github.com/neoformit>`_ in `#17359 <https://github.com/galaxyproject/galaxy/pull/17359>`_
+* XSD schema doc building: quote pipe characters in attribute tables by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17364 <https://github.com/galaxyproject/galaxy/pull/17364>`_
+* Fix IUC best practices links, mention data_source_async in XSD by `@wm75 <https://github.com/wm75>`_ in `#17409 <https://github.com/galaxyproject/galaxy/pull/17409>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* Add tool XML schema documention for outputs - collection - data by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17465 <https://github.com/galaxyproject/galaxy/pull/17465>`_
+* has_size assertion: implement size (as synonym for value) by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17490 <https://github.com/galaxyproject/galaxy/pull/17490>`_
+* Yaml nested assertions: fix parsing by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17641 <https://github.com/galaxyproject/galaxy/pull/17641>`_
+
+============
+Enhancements
+============
+
+* build_mulled: also use namespace for building singularity images by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15657 <https://github.com/galaxyproject/galaxy/pull/15657>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Extend regex groups in stdio regex matches by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17016 <https://github.com/galaxyproject/galaxy/pull/17016>`_
+* Split linters in separate classes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17081 <https://github.com/galaxyproject/galaxy/pull/17081>`_
+* Add select parameter with options from remote resources by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17087 <https://github.com/galaxyproject/galaxy/pull/17087>`_
+* Replace discouraged Mambaforge with Miniforge3 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17177 <https://github.com/galaxyproject/galaxy/pull/17177>`_
+* Clarify the meaning of lexical sorting of discovered datasets by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17190 <https://github.com/galaxyproject/galaxy/pull/17190>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Add element_identifier and ext to inputs config file export by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17357 <https://github.com/galaxyproject/galaxy/pull/17357>`_
+* Enable ``warn_unreachable`` mypy option by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17365 <https://github.com/galaxyproject/galaxy/pull/17365>`_
+* Fix type annotation of code using XML etree by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17367 <https://github.com/galaxyproject/galaxy/pull/17367>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Some additional typing for test interactor stuff. by `@jmchilton <https://github.com/jmchilton>`_ in `#17398 <https://github.com/galaxyproject/galaxy/pull/17398>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* `data_column` parameter: use `column_names` metadata if present by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17478 <https://github.com/galaxyproject/galaxy/pull/17478>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Add `image_diff` comparison method for test output verification using images by `@kostrykin <https://github.com/kostrykin>`_ in `#17556 <https://github.com/galaxyproject/galaxy/pull/17556>`_
+* add shm_size based on ShmSize  by `@richard-burhans <https://github.com/richard-burhans>`_ in `#17565 <https://github.com/galaxyproject/galaxy/pull/17565>`_
+* Record missing outputs as test errors by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17874 <https://github.com/galaxyproject/galaxy/pull/17874>`_
+
+=============
+Other changes
+=============
+
+* consistently compare profile versions by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16492 <https://github.com/galaxyproject/galaxy/pull/16492>`_
 
+-------------------
+23.2.1 (2024-02-21)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Never consider `_galaxy_` conda env as unused by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16460 <https://github.com/galaxyproject/galaxy/pull/16460>`_
+* chore: fix typos by `@afuetterer <https://github.com/afuetterer>`_ in `#16851 <https://github.com/galaxyproject/galaxy/pull/16851>`_
+* Ruff and flake8 fixes by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16884 <https://github.com/galaxyproject/galaxy/pull/16884>`_
+* Quote singularity env parameters by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17055 <https://github.com/galaxyproject/galaxy/pull/17055>`_
+* Remove duplicates when copying sections for tool panel view by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#17117 <https://github.com/galaxyproject/galaxy/pull/17117>`_
+* Display application fixes and tests by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17233 <https://github.com/galaxyproject/galaxy/pull/17233>`_
+
+============
+Enhancements
+============
+
+* Implement default locations for data and collection parameters. by `@jmchilton <https://github.com/jmchilton>`_ in `#14955 <https://github.com/galaxyproject/galaxy/pull/14955>`_
+* Add framework test for profile behavior of `format="input"` by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15482 <https://github.com/galaxyproject/galaxy/pull/15482>`_
+* Tool Shed 2.0 by `@jmchilton <https://github.com/jmchilton>`_ in `#15639 <https://github.com/galaxyproject/galaxy/pull/15639>`_
+* Add ability to assert metadata properties on input dataset parameters by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15825 <https://github.com/galaxyproject/galaxy/pull/15825>`_
+* Migrate a part of the users API to Fast API by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#16341 <https://github.com/galaxyproject/galaxy/pull/16341>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#16436 <https://github.com/galaxyproject/galaxy/pull/16436>`_
+* Tweak tool memory use and optimize shared memory when using preload by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16536 <https://github.com/galaxyproject/galaxy/pull/16536>`_
+* Document that required text parameters need a validator by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16538 <https://github.com/galaxyproject/galaxy/pull/16538>`_
+* Include `regex` when linting validators by `@davelopez <https://github.com/davelopez>`_ in `#16684 <https://github.com/galaxyproject/galaxy/pull/16684>`_
+* Refactor Tool Panel views structures and combine ToolBox and ToolBoxWorkflow into one component by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16739 <https://github.com/galaxyproject/galaxy/pull/16739>`_
+* Replace file_name property with get_file_name function by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#16783 <https://github.com/galaxyproject/galaxy/pull/16783>`_
+* Updated path-based interactive tools with entry point path injection, support for ITs with relative links, shortened URLs, doc and config updates including Podman job_conf by `@sveinugu <https://github.com/sveinugu>`_ in `#16795 <https://github.com/galaxyproject/galaxy/pull/16795>`_
+* Remove remaining legacy backbone form input elements by `@guerler <https://github.com/guerler>`_ in `#16834 <https://github.com/galaxyproject/galaxy/pull/16834>`_
+* Change `api/tool_panel` to `api/tool_panels/...` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#16928 <https://github.com/galaxyproject/galaxy/pull/16928>`_
+* optimize object store cache operations by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#17025 <https://github.com/galaxyproject/galaxy/pull/17025>`_
+* Enhance xsd schema and allow simpler assertion lists by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17134 <https://github.com/galaxyproject/galaxy/pull/17134>`_
+
+=============
+Other changes
+=============
+
+* Merge 23.1 into dev by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16534 <https://github.com/galaxyproject/galaxy/pull/16534>`_
+* Explicitly document default of multiple by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16625 <https://github.com/galaxyproject/galaxy/pull/16625>`_
+
+-------------------
+23.1.4 (2024-01-04)
+-------------------
+
+
+=========
+Bug fixes
+=========
 
+* Separate collection and non-collection data element by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17236 <https://github.com/galaxyproject/galaxy/pull/17236>`_
 
 -------------------
 23.1.3 (2023-12-01)
 -------------------
 
 No recorded changes since last release
 
@@ -39,15 +202,14 @@
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
 * Fixes for two framework test tools by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15483 <https://github.com/galaxyproject/galaxy/pull/15483>`_
 * add missing f for f-string by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15584 <https://github.com/galaxyproject/galaxy/pull/15584>`_
 * Fix call to `docker_cached_container_description` by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15598 <https://github.com/galaxyproject/galaxy/pull/15598>`_
 * Fix log message by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15838 <https://github.com/galaxyproject/galaxy/pull/15838>`_
 * add required_files to the tag list for linting by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16129 <https://github.com/galaxyproject/galaxy/pull/16129>`_
 * Handle appending to a results file that does not exists. by `@ksuderman <https://github.com/ksuderman>`_ in `#16233 <https://github.com/galaxyproject/galaxy/pull/16233>`_
 * Improve container resolver documentation by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16280 <https://github.com/galaxyproject/galaxy/pull/16280>`_
@@ -61,15 +223,14 @@
 * Fix short ids in tool panel views.  by `@jmchilton <https://github.com/jmchilton>`_ in `#16800 <https://github.com/galaxyproject/galaxy/pull/16800>`_
 * Fix tool panel views for versionless tool ids by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16809 <https://github.com/galaxyproject/galaxy/pull/16809>`_
 
 ============
 Enhancements
 ============
 
-* 
 * Decompress history data for testing assertions by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15085 <https://github.com/galaxyproject/galaxy/pull/15085>`_
 * OIDC tokens by `@SergeyYakubov <https://github.com/SergeyYakubov>`_ in `#15300 <https://github.com/galaxyproject/galaxy/pull/15300>`_
 * Fix for new style conda packages by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15446 <https://github.com/galaxyproject/galaxy/pull/15446>`_
 * Move database access code out of tool_util by `@jdavcs <https://github.com/jdavcs>`_ in `#15467 <https://github.com/galaxyproject/galaxy/pull/15467>`_
 * Protection against problematic boolean parameters. by `@jmchilton <https://github.com/jmchilton>`_ in `#15493 <https://github.com/galaxyproject/galaxy/pull/15493>`_
 * Implement initial tool/wf test assertions module for JSON data. by `@jmchilton <https://github.com/jmchilton>`_ in `#15494 <https://github.com/galaxyproject/galaxy/pull/15494>`_
 * Explore tool remote test data by `@davelopez <https://github.com/davelopez>`_ in `#15510 <https://github.com/galaxyproject/galaxy/pull/15510>`_
@@ -98,31 +259,26 @@
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
 * Fixes for extra files handling and cached object stores  by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16595 <https://github.com/galaxyproject/galaxy/pull/16595>`_
 * Fix create/install commands for conda 23.9.0 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16831 <https://github.com/galaxyproject/galaxy/pull/16831>`_
 
 -------------------
 23.0.5 (2023-07-29)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
-* 
 * Allow duplicate labels in linter if outputs contain filters  by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15933 <https://github.com/galaxyproject/galaxy/pull/15933>`_
 * Fix parsing tool metadata from bio.tools by `@kysrpex <https://github.com/kysrpex>`_ in `#16449 <https://github.com/galaxyproject/galaxy/pull/16449>`_
 * Linter: fix regex for profile version by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16480 <https://github.com/galaxyproject/galaxy/pull/16480>`_
 * Adjust test_data_download method in GalaxyInteractorApi so an admin user is not required by `@simonbray <https://github.com/simonbray>`_ in `#16482 <https://github.com/galaxyproject/galaxy/pull/16482>`_
 
 -------------------
 23.0.4 (2023-06-30)
@@ -135,77 +291,52 @@
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
-* 
-* 
 * xsd: add missing `sep` attribute for `has_n_columns` by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16262 <https://github.com/galaxyproject/galaxy/pull/16262>`_
 * Missing init prevents models.py being bundled into tool_util by `@nuwang <https://github.com/nuwang>`_ in `#16308 <https://github.com/galaxyproject/galaxy/pull/16308>`_
 
 ============
 Enhancements
 ============
 
-* 
-* 
 * When importing tool data bundles, use the first loc file for the matching table by `@natefoo <https://github.com/natefoo>`_ in `#16247 <https://github.com/galaxyproject/galaxy/pull/16247>`_
 
 -------------------
 23.0.2 (2023-06-13)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
-* 
-* 
-* 
-* 
 * Don't fail CWL tool parsing when Cheetah not installed by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16219 <https://github.com/galaxyproject/galaxy/pull/16219>`_
 * Allow skipping ``expect_num_outputs`` when ``expect_failure`` is set in tool test by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#16237 <https://github.com/galaxyproject/galaxy/pull/16237>`_
 
 -------------------
 23.0.1 (2023-06-08)
 -------------------
 
 
 =========
 Bug fixes
 =========
 
-* 
-* 
-* 
-* 
-* 
-* 
-* 
 * Fix assertion linting to not fail on byte suffixes by `@bernt-matthias <https://github.com/bernt-matthias>`_ in `#15873 <https://github.com/galaxyproject/galaxy/pull/15873>`_
 * Fix ``get_test_from_anaconda()`` and ``base_image_for_targets()`` functions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#16125 <https://github.com/galaxyproject/galaxy/pull/16125>`_
 * Fix test search for mulled container hashes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16170 <https://github.com/galaxyproject/galaxy/pull/16170>`_
 
 ============
 Enhancements
 ============
 
-* 
-* 
-* 
-* 
-* 
-* 
 * Allow setting auto_decompress property in staging interface by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16014 <https://github.com/galaxyproject/galaxy/pull/16014>`_
 
 -------------------
 22.1.5 (2022-11-14)
 -------------------
 
 * Set test status to success on expected failure
```

### Comparing `galaxy-tool-util-23.2.dev0/LICENSE` & `galaxy-tool-util-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/interface.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/biotools/source.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/source.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/client/staging.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/client/staging.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Client for staging inputs for Galaxy Tools and Workflows.
 
 Implement as a connector to serve a bridge between galactic_job_json
 utility and a Galaxy API library.
 """
+
 import abc
 import json
 import logging
 import os
 from typing import (
     Any,
     BinaryIO,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/cwltool_deps.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/cwltool_deps.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Logic for dealing with cwltool as an optional dependency.
 
 Use this as the import interface for cwltool and just call
 :func:`ensure_cwltool_available` before using any of the imported
 functionality at runtime.
 """
+
 import re
 import warnings
 
 warnings.filterwarnings("ignore", message=r"[\n.]DEPRECATION: Python 2", module="cwltool")
 
 import requests
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/parser.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,15 @@
 
 class ExpressionToolProxy(CommandLineToolProxy):
     _class = "ExpressionTool"
 
 
 class JobProxy:
     def __init__(self, tool_proxy, input_dict, output_dict, job_directory):
+        assert RuntimeContext is not None, "cwltool is not installed, cannot run CWL jobs"
         self._tool_proxy = tool_proxy
         self._input_dict = input_dict
         self._output_dict = output_dict
         self._job_directory = job_directory
 
         self._final_output = None
         self._ok = True
@@ -323,20 +324,16 @@
                 outdir=os.path.join(self._job_directory, "working"),
                 tmpdir=os.path.join(self._job_directory, "cwltmp"),
                 stagedir=os.path.join(self._job_directory, "cwlstagedir"),
                 use_container=False,
                 beta_relaxed_fmt_check=beta_relaxed_fmt_check,
             )
 
-            args = []
+            args = [RuntimeContext(job_args)]
             kwargs: Dict[str, str] = {}
-            if RuntimeContext is not None:
-                args.append(RuntimeContext(job_args))
-            else:
-                kwargs = job_args
             self._cwl_job = next(self._tool_proxy._tool.job(self._input_dict, self._output_callback, *args, **kwargs))
             self._is_command_line_job = hasattr(self._cwl_job, "command_line")
 
     def _normalize_job(self):
         # Somehow reuse whatever causes validate in cwltool... maybe?
         def pathToLoc(p):
             if "location" not in p and "path" in p:
@@ -1227,20 +1224,18 @@
         self.label = label
         self.description = description
         self.required = True
         self.array = array
         self.area = area
 
     @overload
-    def to_dict(self, itemwise: Literal[False]) -> InputInstanceDict:
-        ...
+    def to_dict(self, itemwise: Literal[False]) -> InputInstanceDict: ...
 
     @overload
-    def to_dict(self, itemwise: Literal[True]) -> Union[InputInstanceDict, InputInstanceArrayDict]:
-        ...
+    def to_dict(self, itemwise: Literal[True]) -> Union[InputInstanceDict, InputInstanceArrayDict]: ...
 
     def to_dict(self, itemwise: bool = True) -> Union[InputInstanceDict, InputInstanceArrayDict]:
         if itemwise and self.array:
             return InputInstanceArrayDict(
                 type="repeat", name=f"{self.name}_repeat", title=f"{self.name}", blocks=[self.to_dict(itemwise=False)]
             )
         else:
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/representation.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/representation.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/runnable.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runnable.py`

 * *Files identical despite different names*

```diff
@@ -1,8 +1,9 @@
 """Lighter-weight variant of Planemo runnable outputs."""
+
 from galaxy.tool_util.parser import get_tool_source
 from .parser import workflow_proxy
 from .util import guess_artifact_type
 
 
 def get_outputs(path):
     tool_or_workflow = guess_artifact_type(path)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/runtime_actions.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runtime_actions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/schema.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Abstraction around cwltool and related libraries for loading a CWL artifact."""
+
 import os
 import tempfile
 from typing import NamedTuple
 
 from .cwltool_deps import (
     CommentedMap,
     default_loader,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/cwl/util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Client-centric CWL-related utilities.
 
 Used to share code between the Galaxy test framework
 and other Galaxy CWL clients (e.g. Planemo)."""
+
 import abc
 import hashlib
 import io
 import json
 import os
 import tarfile
 import tempfile
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     Any,
     BinaryIO,
     Callable,
     cast,
     Dict,
     List,
     Optional,
+    overload,
     Set,
     Tuple,
     Type,
     TYPE_CHECKING,
     Union,
 )
 
@@ -77,16 +78,15 @@
 
 # Internally just the first two - but tool shed code (data_manager_manual) will still
 # pass DataManager in.
 EntrySource = Optional[Union[dict, RepoInfo, "DataManager"]]
 
 
 class StoresConfigFilePaths(Protocol):
-    def get(self, key: Any, default: Optional[Any]) -> Optional[Any]:
-        ...
+    def get(self, key: Any, default: Optional[Any]) -> Optional[Any]: ...
 
 
 class ToolDataPathFiles:
     update_time: float
 
     def __init__(self, tool_data_path):
         self.tool_data_path = os.path.abspath(tool_data_path)
@@ -165,25 +165,26 @@
         config_element: Element,
         tool_data_path: Optional[StrPath],
         tool_data_path_files: ToolDataPathFiles,
         from_shed_config: bool = False,
         filename: Optional[StrPath] = None,
         other_config_dict: Optional[StoresConfigFilePaths] = None,
     ) -> None:
-        self.name = config_element.get("name")
-        self.comment_char = config_element.get("comment_char")
+        name = config_element.get("name")
+        assert name
+        self.name = name
         self.empty_field_value = config_element.get("empty_field_value", "")
         self.empty_field_values: Dict[str, str] = {}
         self.allow_duplicate_entries = util.asbool(config_element.get("allow_duplicate_entries", True))
         self.here = os.path.dirname(filename) if filename else None
         self.filenames: Dict[str, FileNameInfoT] = {}
         self.tool_data_path = tool_data_path
         self.tool_data_path_files = tool_data_path_files
         self.other_config_dict = other_config_dict or {}
-        self.missing_index_file = None
+        self.missing_index_file: Optional[str] = None
         # increment this variable any time a new entry is added, or when the table is totally reloaded
         # This value has no external meaning, and does not represent an abstract version of the underlying data
         self._loaded_content_version = 1
         self._load_info = (
             (config_element, tool_data_path),
             {
                 "from_shed_config": from_shed_config,
@@ -344,19 +345,27 @@
         self.comment_char = config_element.get("comment_char", "#")
         # Configure columns
         self.parse_column_spec(config_element)
 
         # store repo info if available:
         repo_elem = config_element.find("tool_shed_repository")
         if repo_elem is not None:
+            tool_shed_elem = repo_elem.find("tool_shed")
+            assert tool_shed_elem is not None
+            repository_name_elem = repo_elem.find("repository_name")
+            assert repository_name_elem is not None
+            repository_owner_elem = repo_elem.find("repository_owner")
+            assert repository_owner_elem is not None
+            installed_changeset_revision_elem = repo_elem.find("installed_changeset_revision")
+            assert installed_changeset_revision_elem is not None
             repo_info = dict(
-                tool_shed=repo_elem.find("tool_shed").text,
-                name=repo_elem.find("repository_name").text,
-                owner=repo_elem.find("repository_owner").text,
-                installed_changeset_revision=repo_elem.find("installed_changeset_revision").text,
+                tool_shed=tool_shed_elem.text,
+                name=repository_name_elem.text,
+                owner=repository_owner_elem.text,
+                installed_changeset_revision=installed_changeset_revision_elem.text,
             )
         else:
             repo_info = None
         # Read every file
         for file_element in config_element.findall("file"):
             tmp_file = None
             filename = file_element.get("path", None)
@@ -371,20 +380,21 @@
                         log.error('Error loading Data Table URL "%s": %s', filename, e)
                         continue
                     log.debug('Loading Data Table URL "%s" as filename "%s".', filename, tmp_file.name)
                     filename = tmp_file.name
                     tmp_file.flush()
                 else:
                     # Pull the filename from a global config
-                    filename = file_element.get("from_config", None) or None
+                    filename = file_element.get("from_config")
                     if filename:
                         filename = self.other_config_dict.get(filename, None)
-            filename = file_path = _expand_here_template(filename, here=self.here)
+            if filename:
+                filename = _expand_here_template(filename, here=self.here)
             found = False
-            if file_path is None:
+            if filename is None:
                 log.debug(
                     "Encountered a file element (%s) that does not contain a path value when loading tool data table '%s'.",
                     util.xml_to_string(file_element),
                     self.name,
                 )
                 continue
 
@@ -395,15 +405,15 @@
             # tool_data_tables_conf.xml file, containing correct <file path=> attributes. Allowing a
             # path.join with a different root should be allowed, but splitting should not be necessary.
             if tool_data_path and from_shed_config:
                 # Must identify with from_shed_config as well, because the
                 # regular galaxy app has and uses tool_data_path.
                 # We're loading a tool in the tool shed, so we cannot use the Galaxy tool-data
                 # directory which is hard-coded into the tool_data_table_conf.xml entries.
-                filename = os.path.split(file_path)[1]
+                filename = os.path.split(filename)[1]
                 filename = os.path.join(tool_data_path, filename)
             if self.tool_data_path_files.exists(filename):
                 found = True
             elif not os.path.isabs(filename):
                 # Since the path attribute can include a hard-coded path to a specific directory
                 # (e.g., <file path="tool-data/cg_crr_files.loc" />) which may not be the same value
                 # as self.tool_data_path, we'll parse the path to get the filename and see if it is
@@ -475,15 +485,15 @@
 
     def handle_found_index_file(self, filename):
         self.missing_index_file = None
         self.extend_data_with(filename)
 
     # This method is used in tools, so need to keep its API stable
     def get_fields(self) -> List[List[str]]:
-        return self.data
+        return self.data.copy()
 
     def get_field(self, value):
         rval = None
         for i in self.get_named_fields_list():
             if i["value"] == value:
                 rval = TabularToolDataField(i)
         return rval
@@ -522,19 +532,19 @@
             column_names = [n.strip() for n in column_names.split(",")]
             for index, name in enumerate(column_names):
                 self.columns[name] = index
                 self.largest_index = index
         else:
             self.largest_index = 0
             for column_elem in config_element.findall("column"):
-                name = column_elem.get("name", None)
+                name = column_elem.get("name")
                 assert name is not None, "Required 'name' attribute missing from column def"
-                index = column_elem.get("index", None)
-                assert index is not None, "Required 'index' attribute missing from column def"
-                index = int(index)
+                index_attr = column_elem.get("index")
+                assert index_attr is not None, "Required 'index' attribute missing from column def"
+                index = int(index_attr)
                 self.columns[name] = index
                 if index > self.largest_index:
                     self.largest_index = index
                 empty_field_value = column_elem.get("empty_field_value", None)
                 if empty_field_value is not None:
                     self.empty_field_values[name] = empty_field_value
         assert "value" in self.columns, "Required 'value' column missing from column def"
@@ -643,15 +653,15 @@
                 source_repo_info_model: Optional[RepoInfo]
                 if source is None or isinstance(source, RepoInfo):
                     source_repo_info_model = source
                 else:
                     # we have a data manager, use its repo_info method
                     source_data_manager = cast("DataManager", source)
                     source_repo_info_model = source_data_manager.repo_info
-                source_repo_info = source_repo_info_model.dict() if source_repo_info_model else None
+                source_repo_info = source_repo_info_model.model_dump() if source_repo_info_model else None
         filename = default
         for name, value in self.filenames.items():
             repo_info = value.get("tool_shed_repository")
             if (not source_repo_info and not repo_info) or (
                 source_repo_info and repo_info and source_repo_info == repo_info
             ):
                 filename = name
@@ -865,44 +875,50 @@
         rval["fields"] = self.data
         rval["base_dir"] = (self.get_base_dir(),)
         rval["files"] = self.get_filesize_map(True)
         rval["fingerprint"] = self.get_fingerprint()
         return rval
 
 
-def _expand_here_template(content: str, here: Optional[str]) -> str:
+@overload
+def _expand_here_template(content: str, here: Optional[str]) -> str: ...
+
+
+@overload
+def _expand_here_template(content: None, here: Optional[str]) -> None: ...
+
+
+def _expand_here_template(content: Optional[str], here: Optional[str]) -> Optional[str]:
     if here and content:
         content = string.Template(content).safe_substitute({"__HERE__": here})
     return content
 
 
 # Registry of tool data types by type_key
 tool_data_table_types_list: List[Type[ToolDataTable]] = [TabularToolDataTable]
 
 
 class HasExtraFiles(Protocol):
     extra_files_path: str
 
-    def extra_files_path_exists(self) -> bool:
-        ...
+    def extra_files_path_exists(self) -> bool: ...
 
 
 class DirectoryAsExtraFiles(HasExtraFiles):
     def __init__(self, directory):
         self.extra_files_path = directory
 
     def extra_files_path_exists(self) -> bool:
         return True
 
 
 class OutputDataset(HasExtraFiles, Protocol):
     ext: str
 
-    def get_file_name(self, sync_cache=True) -> str:
-        ...
+    def get_file_name(self, sync_cache=True) -> str: ...
 
 
 class ToolDataTableManager(Dictifiable):
     """Manages a collection of tool data tables"""
 
     data_tables: Dict[str, ToolDataTable]
     tool_data_table_types = {cls.type_key: cls for cls in tool_data_table_types_list}
@@ -924,15 +940,15 @@
         for single_config_filename in util.listify(config_filename):
             if not single_config_filename:
                 continue
             self.load_from_config_file(single_config_filename, self.tool_data_path, from_shed_config=False)
 
     def index(self) -> ToolDataEntryList:
         data_tables = [ToolDataEntry(**table.to_dict()) for table in self.data_tables.values()]
-        return ToolDataEntryList.construct(__root__=data_tables)
+        return ToolDataEntryList.model_construct(root=data_tables)
 
     def __getitem__(self, key: str) -> ToolDataTable:
         return self.data_tables.__getitem__(key)
 
     def __setitem__(self, key: str, value) -> None:
         return self.data_tables.__setitem__(key, value)
 
@@ -1097,18 +1113,15 @@
                 else:
                     raise
             root = tree.getroot()
             out_elems = [elem for elem in root]
         except Exception as e:
             out_elems = []
             log.debug("Could not parse existing tool data table config, assume no existing elements: %s", e)
-        for elem in remove_elems:
-            # handle multiple occurrences of remove elem in existing elems
-            while elem in out_elems:
-                remove_elems.remove(elem)
+        out_elems = [elem for elem in out_elems if elem not in remove_elems]
         # add new elems
         out_elems.extend(new_elems)
         out_path_is_new = not os.path.exists(full_path)
 
         root = util.parse_xml_string('<?xml version="1.0"?>\n<tables></tables>')
         for elem in out_elems:
             root.append(elem)
@@ -1195,15 +1208,15 @@
                 output_name=output_name,
                 processor_description=bundle_description,
                 repo_info=repo_info,
             )
             extra_files_path = dataset.extra_files_path
             bundle_path = os.path.join(extra_files_path, BUNDLE_INDEX_FILE_NAME)
             with open(bundle_path, "w") as fw:
-                json.dump(bundle.dict(), fw)
+                fw.write(bundle.model_dump_json())
             bundle_datasets[bundle_path] = dataset
         return bundle_datasets
 
 
 SUPPORTED_DATA_TABLE_TYPES = TabularToolDataTable
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/_schema.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/data/_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,73 +2,79 @@
     Dict,
     List,
     Optional,
 )
 
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
+    RootModel,
 )
 
 
-class ToolDataEntry(BaseModel):
+class Model(BaseModel):
+    model_config = ConfigDict(protected_namespaces=())
+
+
+class ToolDataEntry(Model):
     name: str = Field(
         ...,  # Mark this field as required
         title="Name",
         description="The name of this tool data entry",
-        example="all_fasta",
+        examples=["all_fasta"],
     )
     model_class: str = Field(
         ...,  # Mark this field as required
         title="Model class",
         description="The name of class modelling this tool data",
-        example="TabularToolDataTable",
+        examples=["TabularToolDataTable"],
     )
 
 
-class ToolDataEntryList(BaseModel):
-    __root__: List[ToolDataEntry] = Field(
+class ToolDataEntryList(RootModel):
+    root: List[ToolDataEntry] = Field(
         title="A list with details on individual data tables.",
     )
 
     def find_entry(self, name: str) -> Optional[ToolDataEntry]:
-        for entry in self.__root__:
+        for entry in self.root:
             if entry.name == name:
                 return entry
         return None
 
 
 class ToolDataDetails(ToolDataEntry):
     columns: List[str] = Field(
         ...,  # Mark this field as required
         title="Columns",
         description="A list of column names",
-        example=["value", "dbkey", "name", "path"],
+        examples=["value", "dbkey", "name", "path"],
     )
     # We must use an alias since the name 'fields'
     # shadows a Model attribute
     fields_value: List[List[str]] = Field(
         alias="fields",
         default=[],
         title="Fields",
         description="",  # TODO add documentation
     )
 
 
-class ToolDataField(BaseModel):
+class ToolDataField(Model):
     name: str = Field(
         ...,  # Mark this field as required
         title="Name",
         description="The name of the field",
     )
     model_class: str = Field(
         ...,  # Mark this field as required
         title="Model class",
         description="The name of class modelling this tool data field",
-        example="TabularToolDataField",
+        examples=["TabularToolDataField"],
     )
     # We must use an alias since the name 'fields'
     # shadows a Model attribute
     fields_value: Dict[str, str] = Field(
         ...,  # Mark this field as required
         alias="fields",
         title="Fields",
@@ -79,27 +85,27 @@
         title="Base directories",
         description="A list of directories where the data files are stored",
     )
     files: Dict[str, int] = Field(
         ...,  # Mark this field as required
         title="Files",
         description="A dictionary of file names and their size in bytes",
-        example={"file.txt": 136},
+        examples=[{"file.txt": 136}],
     )
     fingerprint: str = Field(
         ...,  # Mark this field as required
         title="Fingerprint",
         description="SHA1 Hash",
-        example="22b45237a85c2b3f474bf66888c534387ffe0ced",
+        examples=["22b45237a85c2b3f474bf66888c534387ffe0ced"],
     )
 
 
-class ToolDataItem(BaseModel):
+class ToolDataItem(Model):
     values: str = Field(
         ...,  # Mark this field as required
         title="Values",
         description=(
             "A `\\t` (TAB) separated list of column __contents__."
             " You must specify a value for each of the columns of the data table."
         ),
-        example="value\tdbkey\tname\tpath",
+        examples=["value\tdbkey\tname\tpath"],
     )
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/data/bundles/models.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     Optional,
     Tuple,
     Union,
 )
 
 from pydantic import (
     BaseModel,
-    Extra,
-    root_validator,
+    ConfigDict,
+    model_validator,
 )
 
 from galaxy.util import (
     asbool,
     Element,
 )
 
@@ -24,70 +24,59 @@
 VALUE_TRANSLATION_FUNCTIONS: Dict[str, Callable] = dict(abspath=os.path.abspath)
 DEFAULT_VALUE_TRANSLATION_TYPE = "template"
 
 
 class DataTableBundleProcessorDataTableOutputColumnTranslation(BaseModel):
     type: str
     value: str
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class DataTableBundleProcessorDataTableOutputColumnMove(BaseModel):
     type: str
     source_base: Optional[str] = None
     source_value: str = ""
     target_base: Optional[str] = None
     target_value: Optional[str] = None
     relativize_symlinks: bool
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class DataTableBundleProcessorDataTableOutputColumn(BaseModel):
     name: str
     data_table_name: str
     output_ref: Optional[str] = None
     value_translations: List[DataTableBundleProcessorDataTableOutputColumnTranslation] = []
     moves: List[DataTableBundleProcessorDataTableOutputColumnMove] = []
+    model_config = ConfigDict(extra="forbid")
 
-    class Config:
-        extra = Extra.forbid
-
-    @root_validator(pre=True)
+    @model_validator(mode="before")
+    @classmethod
     def fill_in_default_data_table_name(cls, values):
         data_table_name = values.get("data_table_name")
         if data_table_name is None:
             values["data_table_name"] = values["name"]
         return values
 
 
 class DataTableBundleProcessorDataTableOutput(BaseModel):
     columns: List[DataTableBundleProcessorDataTableOutputColumn]
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class DataTableBundleProcessorDataTable(BaseModel):
     name: str
-    output: Optional[DataTableBundleProcessorDataTableOutput]
-
-    class Config:
-        extra = Extra.forbid
+    output: Optional[DataTableBundleProcessorDataTableOutput] = None
+    model_config = ConfigDict(extra="forbid")
 
 
 class DataTableBundleProcessorDescription(BaseModel):
     undeclared_tables: bool = False
     data_tables: List[DataTableBundleProcessorDataTable]
-
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     @property
     def data_table_names(self) -> List[str]:
         names = []
         for data_table in self.data_tables:
             data_table_name = data_table.name
             names.append(data_table_name)
@@ -153,18 +142,15 @@
 
 
 class RepoInfo(BaseModel):
     tool_shed: str
     name: str
     owner: str
     installed_changeset_revision: str
-
-    class Config:
-        # we use dictionary equality (yuk) so definitely make sure this is okay.
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class DataTableBundle(BaseModel):
     processor_description: DataTableBundleProcessorDescription
     data_tables: dict
     output_name: Optional[str] = None
     repo_info: Optional[RepoInfo] = None
@@ -177,19 +163,19 @@
     )  # TODO: should we instead always relativize links?
     source_elem = move_elem.find("source")
     if source_elem is None:
         source_base = None
         source_value = ""
     else:
         source_base = source_elem.get("base", None)
-        source_value = source_elem.text
+        source_value = source_elem.text or ""
     target_elem = move_elem.find("target")
     if target_elem is None:
         target_base = None
-        target_value = ""
+        target_value: Optional[str] = ""
     else:
         target_base = target_elem.get("base", None)
         target_value = target_elem.text
     return DataTableBundleProcessorDataTableOutputColumnMove(
         type=move_type,
         source_base=source_base,
         source_value=source_value,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/brew_exts.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_exts.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/brew_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ brew_exts defines generic extensions to Homebrew this file
 builds on those abstraction and provides Galaxy specific functionality
 not useful to the brew external commands.
 """
+
 from . import brew_exts
 
 DEFAULT_TAP = "homebrew/science"
 
 
 class HomebrewRecipe:
     def __init__(self, recipe, version, tap):
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/conda_compat.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Compat. layer with conda_build/verify if Galaxy/galaxy-lib not installed through conda.
 
 In general there are utilities available for Conda building and parsing that are high-quality
 and should be utilized when available but that are only available in conda channels and not in
 PyPI. This module serves as a PyPI capable interface to these utilities.
 """
+
 import os
-from collections.abc import Hashable
 
 import yaml
 
 try:
     from conda_build.metadata import MetaData
 except ImportError:
     MetaData = None
@@ -26,18 +26,14 @@
 
 class _Memoized:
     def __init__(self, func):
         self.func = func
         self.cache = {}
 
     def __call__(self, *args):
-        if not isinstance(args, Hashable):
-            # uncacheable. a list, for instance.
-            # better to not cache than blow up.
-            return self.func(*args)
         if args in self.cache:
             return self.cache[args]
         else:
             value = self.func(*args)
             self.cache[args] = value
             return value
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/conda_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,23 +52,23 @@
 CONDA_BUILD_SPECS = ("conda-build>=3.22.0",)
 USE_LOCAL_DEFAULT = False
 
 
 def conda_link() -> str:
     if IS_OS_X:
         if "arm64" in platform.platform():
-            url = "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-MacOSX-arm64.sh"
+            url = "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-arm64.sh"
         else:
-            url = "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-MacOSX-x86_64.sh"
+            url = "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-MacOSX-x86_64.sh"
     else:
         if sys.maxsize > 2**32:
             if "arm64" in platform.platform():
-                url = "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Linux-aarch64.sh"
+                url = "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-aarch64.sh"
             else:
-                url = "https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Linux-x86_64.sh"
+                url = "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-Linux-x86_64.sh"
         else:
             url = "https://repo.anaconda.com/miniconda/Miniconda3-4.5.12-Linux-x86.sh"
     return url
 
 
 def find_conda_prefix() -> str:
     """If supplied conda_prefix is not set, default to the default location
@@ -250,15 +250,15 @@
         if self.debug:
             cmd.append("--debug")
         cmd.extend(args)
         env = {}
         if self.condarc_override:
             env["CONDARC"] = self.condarc_override
         cmd_string = shlex_join(cmd)
-        kwds = dict()
+        kwds: Dict[str, Any] = dict()
         try:
             if stdout_path:
                 kwds["stdout"] = open(stdout_path, "w")
                 cmd_string += f" > '{stdout_path}'"
             conda_exec_home = env["HOME"] = tempfile.mkdtemp(
                 prefix="conda_exec_home_"
             )  # We don't want to pollute ~/.conda, which may not even be writable
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_classes.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_classes.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Optional,
     Tuple,
     Type,
     TYPE_CHECKING,
 )
 from uuid import uuid4
 
+from packaging.version import Version
 from typing_extensions import Protocol
 
 from galaxy.util import (
     asbool,
     in_directory,
 )
 from . import (
@@ -92,24 +93,21 @@
 
 class ContainerProtocol(Protocol):
     """
     Helper class to allow typing for the HasDockerLikeVolumes mixin
     """
 
     @property
-    def app_info(self) -> "AppInfo":
-        ...
+    def app_info(self) -> "AppInfo": ...
 
     @property
-    def tool_info(self) -> "ToolInfo":
-        ...
+    def tool_info(self) -> "ToolInfo": ...
 
     @property
-    def job_info(self) -> Optional["JobInfo"]:
-        ...
+    def job_info(self) -> Optional["JobInfo"]: ...
 
 
 class Container(metaclass=ABCMeta):
     """
     TODO The container resolvers currently initialize job_info as None,
     ContainerFinder.find_container fixes this by constructing a new container
     with job_info (see __destination_container)
@@ -359,15 +357,15 @@
             else:
                 defaults = "$_GALAXY_JOB_TMP_DIR:rw,$TMPDIR:rw,$TMP:rw,$TEMP:rw"
             defaults += ",$galaxy_root:default_ro"
             if self.job_info.tool_directory:
                 defaults += ",$tool_directory:default_ro"
             if self.job_info.job_directory:
                 defaults += ",$job_directory:default_ro,$job_directory/outputs:rw"
-                if self.tool_info.profile <= 19.09:
+                if Version(str(self.tool_info.profile)) <= Version("19.09"):
                     defaults += ",$job_directory/configs:rw"
             if self.job_info.home_directory is not None:
                 defaults += ",$home_directory:rw"
             if self.app_info.outputs_to_working_directory:
                 # Should need default_file_path (which is of course an estimate given
                 # object stores anyway).
                 defaults += ",$working_directory:rw,$default_file_path:default_ro"
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module defines the abstract interface for resolving container images for tool execution."""
+
 from abc import (
     ABCMeta,
     abstractmethod,
     abstractproperty,
 )
 from typing import (
     Any,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/explicit.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/explicit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module describes the :class:`ExplicitContainerResolver` ContainerResolver plugin."""
+
 import copy
 import logging
 import os
 from typing import (
     cast,
     Container,
     Optional,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/mulled.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/mulled.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,14 +782,15 @@
         super().__init__(app_info=app_info, hash_func=hash_func, **kwds)
         self._involucro_context_kwds = {"involucro_bin": self._get_config_option("involucro_path", None)}
         self.auto_install = string_as_bool(auto_install)
         self._mulled_kwds = {
             "channels": self._get_config_option("mulled_channels", DEFAULT_CHANNELS),
             "hash_func": self.hash_func,
             "command": "build-and-test",
+            "namespace": "local",
             "singularity": True,
             "singularity_image_dir": self.cache_directory.path,
             "use_mamba": True,
         }
         self.involucro_context = InvolucroContext(**self._involucro_context_kwds)
         auto_init = self._get_config_option("involucro_auto_init", True)
         self.enabled = ensure_installed(self.involucro_context, auto_init)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_resolvers/test.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/test.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/container_volumes.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_volumes.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/containers.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/dependencies.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/docker_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/docker_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Utilities for building up Docker commands...
 
 ...using common defaults and configuration mechanisms.
 """
+
 import os
 import shlex
 import sys
 from typing import (
     List,
     Optional,
     TYPE_CHECKING,
@@ -105,15 +106,15 @@
     run_extra_arguments: Optional[str] = DEFAULT_RUN_EXTRA_ARGUMENTS,
     docker_cmd: str = DEFAULT_DOCKER_COMMAND,
     sudo: bool = DEFAULT_SUDO,
     sudo_cmd: str = DEFAULT_SUDO_COMMAND,
     auto_rm: bool = DEFAULT_AUTO_REMOVE,
     set_user: Optional[str] = DEFAULT_SET_USER,
     host: Optional[str] = DEFAULT_HOST,
-    guest_ports: Union[bool, List[str]] = False,
+    guest_ports: Union[bool, str, List[str]] = False,
     container_name: Optional[str] = None,
 ) -> str:
     env_directives = env_directives or []
     volumes = volumes or []
     command_parts = _docker_prefix(docker_cmd=docker_cmd, sudo=sudo, sudo_cmd=sudo_cmd, host=host)
     command_parts.append("run")
     if interactive:
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/dockerfiles.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dockerfiles.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/installable.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/installable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/get_tests.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/get_tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/invfile.lua` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/invfile.lua`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_channel.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_channel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_files.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_build_tool.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_hash.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_hash.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_list.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_search.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_search.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/mulled/util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/requirements.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,19 +185,25 @@
         identifier: str,
         type: str = DEFAULT_CONTAINER_TYPE,
         resolve_dependencies: bool = DEFAULT_CONTAINER_RESOLVE_DEPENDENCIES,
         shell: str = DEFAULT_CONTAINER_SHELL,
     ) -> None:
         # Force to lowercase because container image names must be lowercase.
         # Cached singularity images include the path on disk, so only lowercase
-        # the image identifier portion.
+        # the image identifier portion. Note, the tag can also contain upper case
+        # letters.
         self.identifier = identifier
         if identifier:
             parts = identifier.rsplit(os.sep, 1)
-            parts[-1] = parts[-1].lower()
+            if ":" in parts[-1]:
+                name, tag = parts[-1].rsplit(":", 1)
+                parts[-1] = f"{name.lower()}:{tag}"
+            else:
+                parts[-1] = parts[-1].lower()
+
             self.identifier = os.sep.join(parts)
         self.type = type
         self.resolve_dependencies = resolve_dependencies
         self.shell = shell
         self.explicit = False
 
     def to_dict(self, *args, **kwds) -> Dict[str, Any]:
@@ -233,14 +239,15 @@
     "tmpdir_min",
     "tmpdir_max",
     "cuda_version_min",
     "cuda_compute_capability",
     "gpu_memory_min",
     "cuda_device_count_min",
     "cuda_device_count_max",
+    "shm_size",
 ]
 VALID_RESOURCE_TYPES = get_args(ResourceType)
 
 
 class ResourceRequirement:
     def __init__(self, value_or_expression: Union[int, float, str], resource_type: ResourceType) -> None:
         self.value_or_expression = value_or_expression
@@ -277,14 +284,15 @@
         "tmpdirMin": "tmpdir_min",
         "tmpdirMax": "tmpdir_max",
         "cudaVersionMin": "cuda_version_min",
         "cudaComputeCapability": "cuda_compute_capability",
         "gpuMemoryMin": "gpu_memory_min",
         "cudaDeviceCountMin": "cuda_device_count_min",
         "cudaDeviceCountMax": "cuda_device_count_max",
+        "ShmSize": "shm_size",
     }
     rr = []
     for r in requirements:
         if r.get("class") == "ResourceRequirement":
             valid_key_set = set(cwl_to_galaxy.keys())
         elif r.get("type") == "resource":
             valid_key_set = set(cwl_to_galaxy.values())
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The module defines the abstract interface for dealing tool dependency resolution plugins."""
+
 import errno
 import os.path
 from abc import (
     ABCMeta,
     abstractmethod,
     abstractproperty,
 )
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This dependency resolver resolves tool shed dependencies (those defined
 tool_dependencies.xml) installed using Platform Homebrew and converted
 via shed2tap (e.g. https://github.com/jmchilton/homebrew-toolshed).
 """
+
 import logging
 import os
 
 from galaxy.util import parse_xml
 from . import (
     DependencyResolver,
     NullDependency,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/conda.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/conda.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/galaxy_packages.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/galaxy_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/homebrew.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/homebrew.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/lmod.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/lmod.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This is a prototype dependency resolver to be able to use the "LMOD environment modules system" from TACC to solve package requirements
 
 LMOD official website: https://www.tacc.utexas.edu/research-development/tacc-projects/lmod
 
 LMOD @ Github: https://github.com/TACC/Lmod
 
 """
+
 import logging
 from io import StringIO
 from os import getenv
 from os.path import exists
 from subprocess import (
     PIPE,
     Popen,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/modules.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This file contains the outline of an implementation to load environment modules
 (http://modules.sourceforge.net/).
 
 This is a community contributed feature and the core Galaxy team does utilize
 it, hence support for it will be minimal. The Galaxy team eagerly welcomes
 community contribution and maintenance however.
 """
+
 import logging
 from io import StringIO
 from os import (
     environ,
     pathsep,
 )
 from os.path import (
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/resolver_mixins.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/resolver_mixins.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 This tool is still under development so the default behaviour could change.
 It has been tested when placed in the same directory as galaxy_packages.py
 
 At the time of writing July 3 2015 this resolver has to be plugged in.
 See bottom for instructions on how to add this resolver.
 
 """
+
 import logging
 from os import listdir
 from os.path import (
     exists,
     getmtime,
     join,
 )
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/singularity_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/singularity_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/deps/views.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/views.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/edam_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/edam_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/fetcher.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/fetcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/lint.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/lint.py`

 * *Files 9% similar despite different names*

```diff
@@ -41,48 +41,87 @@
   ``lint_message_class=XMLLintMessageLine``
 - the additional parameter needs to be added as well to calls adding messages
   to the lint context, e.g. ``lint_ctx.error("some message", node=X)``. Note
   that the additional properties must be given as keyword arguments.
 """
 
 import inspect
+from abc import (
+    ABC,
+    abstractmethod,
+)
 from enum import IntEnum
 from typing import (
     Callable,
     List,
     Optional,
     Type,
+    TYPE_CHECKING,
     TypeVar,
     Union,
 )
 
+import galaxy.tool_util.linters
 from galaxy.tool_util.parser import get_tool_source
 from galaxy.util import (
-    etree,
+    Element,
     submodules,
 )
 
+if TYPE_CHECKING:
+    from galaxy.tool_util.parser.interface import ToolSource
+
 
 class LintLevel(IntEnum):
     SILENT = 5
     ERROR = 4
     WARN = 3
     INFO = 2
     VALID = 1
     ALL = 0
 
 
+class Linter(ABC):
+    """
+    a linter. needs to define a lint method and the code property.
+    optionally a fix method can be given
+    """
+
+    @classmethod
+    @abstractmethod
+    def lint(cls, tool_source: "ToolSource", lint_ctx: "LintContext"):
+        """
+        should add at most one message to the lint context
+        """
+        pass
+
+    @classmethod
+    def name(cls) -> str:
+        """
+        get the linter name
+        """
+        return cls.__name__
+
+    @classmethod
+    def list_listers(cls) -> List[str]:
+        """
+        list the names of all linter derived from Linter
+        """
+        return [s.__name__ for s in cls.__subclasses__()]
+
+
 class LintMessage:
     """
     a message from the linter
     """
 
-    def __init__(self, level: str, message: str, **kwargs):
+    def __init__(self, level: str, message: str, linter: Optional[str] = None, **kwargs):
         self.level = level
         self.message = message
+        self.linter = linter
 
     def __eq__(self, other) -> bool:
         """
         add equal operator to easy lookup of a message in a
         List[LintMessage] which is useful in tests.
 
         If the other object is a string, it is loosely checked if the
@@ -91,39 +130,43 @@
         if isinstance(other, str):
             return other in self.message
         if isinstance(other, LintMessage):
             return self.message == other.message
         return False
 
     def __str__(self) -> str:
-        return f".. {self.level.upper()}: {self.message}"
+        if self.linter:
+            linter = f" ({self.linter})"
+        else:
+            linter = ""
+        return f".. {self.level.upper()}{linter}: {self.message}"
 
     def __repr__(self) -> str:
         return f"LintMessage({self.message})"
 
 
 class XMLLintMessageLine(LintMessage):
-    def __init__(self, level: str, message: str, node: Optional[etree.Element] = None):
-        super().__init__(level, message)
+    def __init__(self, level: str, message: str, linter: Optional[str] = None, node: Optional[Element] = None):
+        super().__init__(level, message, linter)
         self.line = None
         if node is not None:
             self.line = node.sourceline
 
     def __str__(self) -> str:
         rval = super().__str__()
         if self.line is not None:
             rval += " ("
             rval += str(self.line)
             rval += ")"
         return rval
 
 
 class XMLLintMessageXPath(LintMessage):
-    def __init__(self, level: str, message: str, node: Optional[etree.Element] = None):
-        super().__init__(level, message)
+    def __init__(self, level: str, message: str, linter: Optional[str] = None, node: Optional[Element] = None):
+        super().__init__(level, message, linter)
         self.xpath = None
         if node is not None:
             tool_xml = node.getroottree()
             self.xpath = tool_xml.getpath(node)
 
     def __str__(self) -> str:
         rval = super().__str__()
@@ -166,15 +209,16 @@
         return len(self.error_messages) > 0
 
     @property
     def found_warns(self) -> bool:
         return len(self.warn_messages) > 0
 
     def lint(self, name: str, lint_func: Callable[[LintTargetType, "LintContext"], None], lint_target: LintTargetType):
-        name = name[len("lint_") :]
+        if name.startswith("lint_"):
+            name = name[len("lint_") :]
         if name in self.skip_types:
             return
 
         if self.level < LintLevel.SILENT:
             # this is a relict from the past where the lint context
             # was reset when called with a new lint_func, as workaround
             # we save the message list, apply the lint_func (which then
@@ -183,45 +227,26 @@
             tmp_message_list = list(self.message_list)
             self.message_list = []
 
         # call linter
         lint_func(lint_target, self)
 
         if self.level < LintLevel.SILENT:
-            # TODO: colorful emoji if in click CLI.
-            if self.error_messages:
-                status = "FAIL"
-            elif self.warn_messages:
-                status = "WARNING"
-            else:
-                status = "CHECK"
-
-            def print_linter_info(printed_linter_info):
-                if printed_linter_info:
-                    return True
-                print(f"Applying linter {name}... {status}")
-                return True
-
-            plf = False
             for message in self.error_messages:
-                plf = print_linter_info(plf)
                 print(f"{message}")
 
             if self.level <= LintLevel.WARN:
                 for message in self.warn_messages:
-                    plf = print_linter_info(plf)
                     print(f"{message}")
 
             if self.level <= LintLevel.INFO:
                 for message in self.info_messages:
-                    plf = print_linter_info(plf)
                     print(f"{message}")
             if self.level <= LintLevel.VALID:
                 for message in self.valid_messages:
-                    plf = print_linter_info(plf)
                     print(f"{message}")
             self.message_list = tmp_message_list + self.message_list
 
     @property
     def valid_messages(self) -> List[LintMessage]:
         return [x for x in self.message_list if x.level == "check"]
 
@@ -233,30 +258,30 @@
     def warn_messages(self) -> List[LintMessage]:
         return [x for x in self.message_list if x.level == "warning"]
 
     @property
     def error_messages(self) -> List[LintMessage]:
         return [x for x in self.message_list if x.level == "error"]
 
-    def __handle_message(self, level: str, message: str, *args, **kwargs) -> None:
+    def __handle_message(self, level: str, message: str, linter: Optional[str] = None, *args, **kwargs) -> None:
         if args:
             message = message % args
-        self.message_list.append(self.lint_message_class(level=level, message=message, **kwargs))
+        self.message_list.append(self.lint_message_class(level=level, message=message, linter=linter, **kwargs))
 
-    def valid(self, message: str, *args, **kwargs) -> None:
-        self.__handle_message("check", message, *args, **kwargs)
+    def valid(self, message: str, linter: Optional[str] = None, *args, **kwargs) -> None:
+        self.__handle_message("check", message, linter, *args, **kwargs)
 
-    def info(self, message: str, *args, **kwargs) -> None:
-        self.__handle_message("info", message, *args, **kwargs)
+    def info(self, message: str, linter: Optional[str] = None, *args, **kwargs) -> None:
+        self.__handle_message("info", message, linter, *args, **kwargs)
 
-    def error(self, message: str, *args, **kwargs) -> None:
-        self.__handle_message("error", message, *args, **kwargs)
+    def error(self, message: str, linter: Optional[str] = None, *args, **kwargs) -> None:
+        self.__handle_message("error", message, linter, *args, **kwargs)
 
-    def warn(self, message: str, *args, **kwargs) -> None:
-        self.__handle_message("warning", message, *args, **kwargs)
+    def warn(self, message: str, linter: Optional[str] = None, *args, **kwargs) -> None:
+        self.__handle_message("warning", message, linter, *args, **kwargs)
 
     def failed(self, fail_level: Union[LintLevel, str]) -> bool:
         if isinstance(fail_level, str):
             fail_level = LintLevel[fail_level.upper()]
         found_warns = self.found_warns
         found_errors = self.found_errors
         if fail_level == LintLevel.WARN:
@@ -315,20 +340,24 @@
     lint_xml_with(lint_context, tool_xml, extra_modules)
 
     return not lint_context.failed(fail_level)
 
 
 def lint_tool_source_with(lint_context, tool_source, extra_modules=None) -> LintContext:
     extra_modules = extra_modules or []
-    import galaxy.tool_util.linters
 
-    tool_xml = getattr(tool_source, "xml_tree", None)
-    tool_type = tool_source.parse_tool_type() or "default"
     linter_modules = submodules.import_submodules(galaxy.tool_util.linters)
     linter_modules.extend(extra_modules)
+    return lint_tool_source_with_modules(lint_context, tool_source, linter_modules)
+
+
+def lint_tool_source_with_modules(lint_context: LintContext, tool_source, linter_modules) -> LintContext:
+    tool_xml = getattr(tool_source, "xml_tree", None)
+    tool_type = tool_source.parse_tool_type() or "default"
+
     for module in linter_modules:
         lint_tool_types = getattr(module, "lint_tool_types", ["default", "manage_data"])
         if not ("*" in lint_tool_types or tool_type in lint_tool_types):
             continue
 
         for name, value in inspect.getmembers(module):
             if callable(value) and name.startswith("lint_"):
@@ -340,14 +369,16 @@
                     if tool_xml is None:
                         # XML linter and non-XML tool, skip for now
                         continue
                     else:
                         lint_context.lint(name, value, tool_xml)
                 else:
                     lint_context.lint(name, value, tool_source)
+            elif inspect.isclass(value) and issubclass(value, Linter) and not inspect.isabstract(value):
+                lint_context.lint(name, value.lint, tool_source)
     return lint_context
 
 
 def lint_xml_with(lint_context, tool_xml, extra_modules=None) -> LintContext:
     extra_modules = extra_modules or []
     tool_source = get_tool_source(xml_tree=tool_xml)
     return lint_tool_source_with(lint_context, tool_source, extra_modules=extra_modules)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/stdio.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/stdio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 """This module contains a linting functions for tool error detection."""
+
 import re
+from typing import TYPE_CHECKING
 
-from galaxy.util import etree
-from .command import get_command
+from packaging.version import Version
 
+from galaxy.tool_util.lint import Linter
 
-def lint_stdio(tool_source, lint_ctx):
-    tool_xml = getattr(tool_source, "xml_tree", None)
-    if not tool_xml:
-        # Can only lint XML tools at this point.
-        # Should probably use tool_source.parse_stdio() to abstract away XML details
-        return
-    stdios = tool_xml.findall("./stdio") if tool_xml else []
-    # determine node to report for general problems with stdio
-    tool_node = tool_xml.find("./stdio")
-    if tool_node is None:
+if TYPE_CHECKING:
+    from galaxy.tool_util.lint import LintContext
+    from galaxy.tool_util.parser.interface import ToolSource
+
+
+class StdIOAbsenceLegacy(Linter):
+    @classmethod
+    def lint(cls, tool_source: "ToolSource", lint_ctx: "LintContext"):
+        tool_xml = getattr(tool_source, "xml_tree", None)
+        if not tool_xml:
+            # Can only lint XML tools at this point.
+            # Should probably use tool_source.parse_stdio() to abstract away XML details
+            return
+        stdios = tool_xml.findall("./stdio") if tool_xml else []
+        if stdios:
+            return
         tool_node = tool_xml.getroot()
-
-    if not stdios:
-        command = get_command(tool_xml) if tool_xml else None
+        command = tool_xml.find("./command")
         if command is None or not command.get("detect_errors"):
-            if tool_source.parse_profile() <= "16.01":
+            if Version(tool_source.parse_profile()) <= Version("16.01"):
                 lint_ctx.info(
                     "No stdio definition found, tool indicates error conditions with output written to stderr.",
+                    linter=cls.name(),
                     node=tool_node,
                 )
-            else:
+
+
+class StdIOAbsence(Linter):
+    @classmethod
+    def lint(cls, tool_source: "ToolSource", lint_ctx: "LintContext"):
+        tool_xml = getattr(tool_source, "xml_tree", None)
+        if not tool_xml:
+            # Can only lint XML tools at this point.
+            # Should probably use tool_source.parse_stdio() to abstract away XML details
+            return
+        stdios = tool_xml.findall("./stdio") if tool_xml else []
+        if stdios:
+            return
+        tool_node = tool_xml.getroot()
+        command = tool_xml.find("./command")
+        if command is None or not command.get("detect_errors"):
+            if Version(tool_source.parse_profile()) > Version("16.01"):
                 lint_ctx.info(
                     "No stdio definition found, tool indicates error conditions with non-zero exit codes.",
+                    linter=cls.name(),
                     node=tool_node,
                 )
-        return
 
-    if len(stdios) > 1:
-        lint_ctx.error("More than one stdio tag found, behavior undefined.", node=stdios[1])
-        return
-
-    stdio = stdios[0]
-    for child in list(stdio):
-        if child.tag is etree.Comment:
-            continue
-        if child.tag == "regex":
-            _lint_regex(tool_xml, child, lint_ctx)
-        elif child.tag == "exit_code":
-            _lint_exit_code(tool_xml, child, lint_ctx)
-        else:
-            message = "Unknown stdio child tag discovered [%s]. "
-            message += "Valid options are exit_code and regex."
-            lint_ctx.warn(message % child.tag, node=child)
-
-
-def _lint_exit_code(tool_xml, child, lint_ctx):
-    for key in child.attrib.keys():
-        if key not in ["description", "level", "range"]:
-            lint_ctx.warn(f"Unknown attribute [{key}] encountered on exit_code tag.", node=child)
-
-
-def _lint_regex(tool_xml, child, lint_ctx):
-    for key in child.attrib.keys():
-        if key not in ["description", "level", "match", "source"]:
-            lint_ctx.warn(f"Unknown attribute [{key}] encountered on regex tag.", node=child)
-    match = child.attrib.get("match")
-    if match:
-        try:
-            re.compile(match)
-        except Exception as e:
-            lint_ctx.error(f"Match '{match}' is no valid regular expression: {str(e)}", node=child)
+
+class StdIORegex(Linter):
+    @classmethod
+    def lint(cls, tool_source: "ToolSource", lint_ctx: "LintContext"):
+        tool_xml = getattr(tool_source, "xml_tree", None)
+        if not tool_xml:
+            # Can only lint XML tools at this point.
+            # Should probably use tool_source.parse_stdio() to abstract away XML details
+            return
+        stdios = tool_xml.findall("./stdio") if tool_xml else []
+
+        if len(stdios) != 1:
+            return
+
+        stdio = stdios[0]
+        for child in list(stdio):
+            if child.tag == "regex":
+                match = child.attrib.get("match")
+                if match:
+                    try:
+                        re.compile(match)
+                    except Exception as e:
+                        lint_ctx.error(
+                            f"Match '{match}' is no valid regular expression: {str(e)}", linter=cls.name(), node=child
+                        )
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/linters/xml_order.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xml_order.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,31 @@
-"""This module contains a linting functions for tool XML block order.
+"""This module contains a linter for tool XML block order.
 
 For more information on the IUC standard for XML block order see -
 https://github.com/galaxy-iuc/standards.
 """
 
+from typing import (
+    Optional,
+    TYPE_CHECKING,
+)
+
+from galaxy.tool_util.lint import Linter
+from ._util import is_datasource
+
+if TYPE_CHECKING:
+    from galaxy.tool_util.lint import LintContext
+    from galaxy.tool_util.parser.interface import ToolSource
+
 # https://github.com/galaxy-iuc/standards
 # https://github.com/galaxy-iuc/standards/pull/7/files
 TAG_ORDER = [
     "description",
     "macros",
+    "options",
     "edam_topics",
     "edam_operations",
     "xrefs",
     "parallelism",
     "requirements",
     "required_files",
     "code",
@@ -27,44 +40,48 @@
     "help",
     "citations",
 ]
 
 DATASOURCE_TAG_ORDER = [
     "description",
     "macros",
+    "requirements",
     "command",
     "configfiles",
     "inputs",
     "request_param_translation",
     "uihints",
     "outputs",
     "options",
     "help",
     "citations",
 ]
 
 
-# Ensure the XML blocks appear in the correct order prescribed
-# by the tool author best practices.
-def lint_xml_order(tool_xml, lint_ctx):
-    tool_root = tool_xml.getroot()
-
-    if tool_root.attrib.get("tool_type", "") == "data_source":
-        tag_ordering = DATASOURCE_TAG_ORDER
-    else:
-        tag_ordering = TAG_ORDER
-
-    last_tag = None
-    last_key = None
-    for elem in tool_root:
-        tag = elem.tag
-        if tag in tag_ordering:
+class XMLOrder(Linter):
+    @classmethod
+    def lint(cls, tool_source: "ToolSource", lint_ctx: "LintContext"):
+        tool_xml = getattr(tool_source, "xml_tree", None)
+        if not tool_xml:
+            return
+        tool_root = tool_xml.getroot()
+
+        if is_datasource(tool_xml):
+            tag_ordering = DATASOURCE_TAG_ORDER
+        else:
+            tag_ordering = TAG_ORDER
+        last_tag = None
+        last_key: Optional[int] = None
+        for elem in tool_root:
+            tag = elem.tag
+            if tag not in tag_ordering:
+                continue
             key = tag_ordering.index(tag)
             if last_key:
                 if last_key > key:
                     lint_ctx.warn(
-                        f"Best practice violation [{tag}] elements should come before [{last_tag}]", node=elem
+                        f"Best practice violation [{tag}] elements should come before [{last_tag}]",
+                        linter=cls.name(),
+                        node=elem,
                     )
             last_tag = tag
             last_key = key
-        else:
-            lint_ctx.info(f"Unknown tag [{tag}] encountered, this may result in a warning in the future.", node=elem)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/loader_directory.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/loader_directory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for loading and reasoning about unparsed tools in directories."""
+
 import fnmatch
 import glob
 import logging
 import os
 import re
 import sys
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/locations/dockstore.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/locations/dockstore.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/biotools_mappings.tsv` & `galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/biotools_mappings.tsv`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/ontologies/ontology_data.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/ontology_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/output_checker.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/output_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,41 @@
 import re
 from enum import Enum
 from logging import getLogger
+from typing import (
+    Any,
+    Dict,
+    List,
+    Tuple,
+    TYPE_CHECKING,
+)
 
 from galaxy.tool_util.parser.stdio import StdioErrorLevel
-from galaxy.util import unicodify
+
+if TYPE_CHECKING:
+    from galaxy.tool_util.parser.stdio import (
+        ToolStdioExitCode,
+        ToolStdioRegex,
+    )
 
 log = getLogger(__name__)
 
 
 class DETECTED_JOB_STATE(str, Enum):
     OK = "ok"
     OUT_OF_MEMORY_ERROR = "oom_error"
     GENERIC_ERROR = "generic_error"
 
 
 ERROR_PEEK_SIZE = 2000
 
 
-def check_output_regex(job_id_tag, regex, stream, stream_name, job_messages, max_error_level):
+def check_output_regex(
+    regex: "ToolStdioRegex", stream: str, stream_name: str, job_messages: List[Dict[str, Any]], max_error_level: int
+) -> int:
     """
     check a single regex against a stream
 
     regex the regex to check
     stream the stream to search in
     job_messages a list where the descriptions of the detected regexes can be appended
     max_error_level the maximum error level that has been detected so far
@@ -31,15 +45,21 @@
     if regex_match:
         reason = __regex_err_msg(regex_match, stream_name, regex)
         job_messages.append(reason)
         return max(max_error_level, regex.error_level)
     return max_error_level
 
 
-def check_output(stdio_regexes, stdio_exit_codes, stdout, stderr, tool_exit_code, job_id_tag):
+def check_output(
+    stdio_regexes: List["ToolStdioRegex"],
+    stdio_exit_codes: List["ToolStdioExitCode"],
+    stdout: str,
+    stderr: str,
+    tool_exit_code: int,
+) -> Tuple[str, str, str, List[Dict[str, Any]]]:
     """
     Check the output of a tool - given the stdout, stderr, and the tool's
     exit code, return DETECTED_JOB_STATE.OK if the tool exited succesfully or
     error type otherwise. No exceptions should be thrown. If this code encounters
     an exception, it returns OK so that the workflow can continue;
     otherwise, a bug in this code could halt workflow progress.
 
@@ -47,17 +67,14 @@
     any stdio/stderr handling, then it reverts back to previous behavior:
     if stderr contains anything, then False is returned.
     """
     # By default, the tool succeeded. This covers the case where the code
     # has a bug but the tool was ok, and it lets a workflow continue.
     state = DETECTED_JOB_STATE.OK
 
-    stdout = unicodify(stdout, strip_null=True)
-    stderr = unicodify(stderr, strip_null=True)
-
     # messages (descriptions of the detected exit_code and regexes)
     # to be prepended to the stdout/stderr after all exit code and regex tests
     # are done (otherwise added messages are searched again).
     # messages are added it the order of detection
 
     # If job is failed, track why.
     job_messages = []
@@ -114,36 +131,32 @@
                 # a fatal error yet
                 for regex in stdio_regexes:
                     # If ( this regex should be matched against stdout )
                     #   - Run the regex's match pattern against stdout
                     #   - If it matched, then determine the error level.
                     #       o If it was fatal, then we're done - break.
                     if regex.stderr_match:
-                        max_error_level = check_output_regex(
-                            job_id_tag, regex, stderr, "stderr", job_messages, max_error_level
-                        )
+                        max_error_level = check_output_regex(regex, stderr, "stderr", job_messages, max_error_level)
                         if max_error_level >= StdioErrorLevel.MAX:
                             break
 
                     if regex.stdout_match:
-                        max_error_level = check_output_regex(
-                            job_id_tag, regex, stdout, "stdout", job_messages, max_error_level
-                        )
+                        max_error_level = check_output_regex(regex, stdout, "stdout", job_messages, max_error_level)
                         if max_error_level >= StdioErrorLevel.MAX:
                             break
 
             # If we encountered a fatal error, then we'll need to set the
             # job state accordingly. Otherwise the job is ok:
             if max_error_level == StdioErrorLevel.FATAL_OOM:
                 state = DETECTED_JOB_STATE.OUT_OF_MEMORY_ERROR
             elif max_error_level >= StdioErrorLevel.FATAL:
-                reason = ""
+                error_reason = ""
                 if job_messages:
-                    reason = f" Reasons are {job_messages}"
-                log.info(f"Job error detected, failing job.{reason}")
+                    error_reason = f" Reasons are {job_messages}"
+                log.info(f"Job error detected, failing job.{error_reason}")
                 state = DETECTED_JOB_STATE.GENERIC_ERROR
 
         # When there are no regular expressions and no exit codes to check,
         # default to the previous behavior: when there's anything on stderr
         # the job has an error, and the job is ok otherwise.
         else:
             # TODO: Add in the tool and job id:
@@ -155,15 +168,15 @@
                 log.info(f"Job failed because of contents in the standard error stream: [{peek}]")
     except Exception:
         log.exception("Job state check encountered unexpected exception; assuming execution successful")
 
     return state, stdout, stderr, job_messages
 
 
-def __regex_err_msg(match, stream, regex):
+def __regex_err_msg(match: re.Match, stream: str, regex: "ToolStdioRegex"):
     """
     Return a message about the match on tool output using the given
     ToolStdioRegex regex object. The regex_match is a MatchObject
     that will contain the string matched on.
     """
     # Get the description for the error level:
     desc = f"{StdioErrorLevel.desc(regex.error_level)}: "
@@ -173,15 +186,15 @@
         match_str = f"{match.string[mstart:mstart + 256]}..."
     else:
         match_str = match.string[mstart:mend]
 
     # If there's a description for the regular expression, then use it.
     # Otherwise, we'll take the first 256 characters of the match.
     if regex.desc is not None:
-        desc += regex.desc
+        desc += match.expand(regex.desc)
     else:
         desc += f"Matched on {match_str}"
     return {
         "type": "regex",
         "stream": stream,
         "desc": desc,
         "code_desc": regex.desc,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/cwl.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/factory.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/interface.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 NOT_IMPLEMENTED_MESSAGE = "Galaxy tool format does not yet support this tool feature."
 
 
 class AssertionDict(TypedDict):
     tag: str
     attributes: Dict[str, Any]
-    children: Optional[List[Dict[str, Any]]]
+    children: "AssertionList"
 
 
 AssertionList = Optional[List[AssertionDict]]
 XmlInt = Union[str, int]
 
 
 class ToolSourceTest(TypedDict):
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_actions.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
                     self.default,
                     context=other_values,
                     python_template_version=other_values.get("__python_template_version__"),
                 ).split(",")
             else:
                 # fallback when Cheetah not available, equivalent to how this was handled prior 23.0
                 # definitely not needed for CWL tool parsing
-                log.warning("Cheetah not installed, falling back to legacy 'apply_action' behavior.")
+                log.warning("Cheetah not installed, falling back to legacy 'apply_action' behavior.")  # type: ignore[unreachable]
                 value = self.default
         if value is not None:
             setattr(output_dataset.metadata, self.name, value)
 
 
 class FormatToolOutputAction(ToolOutputAction):
     tag = "format"
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_collection_def.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_collection_def.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ This module define an abstract class for reasoning about Galaxy's
 dataset collection after jobs are finished.
 """
+
 from typing import List
 
 from galaxy.util import asbool
 from .util import is_dict
 
 DEFAULT_EXTRA_FILENAME_PATTERN = (
     r"primary_DATASET_ID_(?P<designation>[^_]+)_(?P<visible>[^_]+)_(?P<ext>[^_]+)(_(?P<dbkey>[^_]+))?"
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/output_objects.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_objects.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/stdio.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from collections import OrderedDict
 
 DEFAULT_DELTA = 10000
 DEFAULT_DELTA_FRAC = None
 
+DEFAULT_METRIC = "mae"
+DEFAULT_EPS = 0.01
+
 
 def is_dict(item):
     return isinstance(item, dict) or isinstance(item, OrderedDict)
 
 
 def _parse_name(name, argument):
     """Determine name of an input source from name and argument
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/xml.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 
 from packaging.version import Version
 
 from galaxy.tool_util.deps import requirements
 from galaxy.tool_util.parser.util import (
     DEFAULT_DELTA,
     DEFAULT_DELTA_FRAC,
+    DEFAULT_EPS,
+    DEFAULT_METRIC,
 )
 from galaxy.util import (
     Element,
     ElementTree,
     string_as_bool,
     xml_text,
     xml_to_string,
@@ -89,15 +91,14 @@
 
     del tree
 
 
 def parse_change_format(change_format: Iterable[Element]) -> List[ChangeFormatModel]:
     change_models: List[ChangeFormatModel] = []
     for change_elem in change_format:
-        change_elem = cast(Element, change_elem)
         for when_elem in change_elem.findall("when"):
             when_elem = cast(Element, when_elem)
             value: Optional[str] = when_elem.get("value", None)
             format_: Optional[str] = when_elem.get("format", None)
             check: Optional[str] = when_elem.get("input", None)
             input_dataset: Optional[str] = None
             check_attribute: Optional[str] = None
@@ -119,22 +120,21 @@
     return change_models
 
 
 class XmlToolSource(ToolSource):
     """Responsible for parsing a tool from classic Galaxy representation."""
 
     language = "xml"
-    root: Element
 
     def __init__(self, xml_tree: ElementTree, source_path=None, macro_paths=None):
         self.xml_tree = xml_tree
         self.root = self.xml_tree.getroot()
         self._source_path = source_path
         self._macro_paths = macro_paths or []
-        self.legacy_defaults = self.parse_profile() == "16.01"
+        self.legacy_defaults = Version(self.parse_profile()) == Version("16.01")
         self._string = xml_to_string(self.root)
 
     def to_string(self):
         return self._string
 
     def mem_optimize(self):
         destroy_tree(self.xml_tree)
@@ -246,15 +246,15 @@
                 "inject": inject,
                 "strip": string_as_bool(environment_variable_el.get("strip", False)),
             }
             environment_variables.append(definition)
         return environment_variables
 
     def parse_home_target(self):
-        target = "job_home" if self.parse_profile() >= "18.01" else "shared_home"
+        target = "job_home" if Version(self.parse_profile()) >= Version("18.01") else "shared_home"
         command_el = self._command_el
         command_legacy = (command_el is not None) and command_el.get("use_shared_home", None)
         if command_legacy is not None:
             target = "shared_home" if string_as_bool(command_legacy) else "job_home"
         return target
 
     def parse_tmp_target(self):
@@ -393,15 +393,15 @@
     def parse_provided_metadata_style(self):
         style = None
         out_elem = self.root.find("outputs")
         if out_elem is not None and "provided_metadata_style" in out_elem.attrib:
             style = out_elem.attrib["provided_metadata_style"]
 
         if style is None:
-            style = "legacy" if self.parse_profile() < "17.09" else "default"
+            style = "legacy" if Version(self.parse_profile()) < Version("17.09") else "default"
 
         assert style in ["legacy", "default"]
         return style
 
     def parse_provided_metadata_file(self):
         provided_metadata_file = "galaxy.json"
         out_elem = self.root.find("outputs")
@@ -535,15 +535,15 @@
         output.metadata_source = data_elem.get("metadata_source", default_metadata_source)
         output.parent = data_elem.get("parent", None)
         output.label = xml_text(data_elem, "label")
         output.count = int(data_elem.get("count", 1))
         output.filters = data_elem.findall("filter")
         output.tool = tool
         output.from_work_dir = data_elem.get("from_work_dir", None)
-        if output.from_work_dir and getattr(tool, "profile", 0) < 21.09:
+        if output.from_work_dir and Version(str(getattr(tool, "profile", 0))) < Version("21.09"):
             # We started quoting from_work_dir outputs in 21.09.
             # Prior to quoting, trailing spaces had no effect.
             # This ensures that old tools continue to work.
             output.from_work_dir = output.from_work_dir.strip()
         output.hidden = string_as_bool(data_elem.get("hidden", ""))
         output.actions = ToolOutputActionGroup(output, data_elem.find("actions"))
         output.dataset_collector_descriptions = dataset_collector_descriptions_from_elem(
@@ -756,15 +756,15 @@
         element_attrib = dict(element.attrib)
         identifier = element_attrib.pop("name", None)
         if identifier is None:
             raise Exception("Test primary dataset does not have a 'identifier'")
         element_tests[identifier] = __parse_test_attributes(
             element, element_attrib, parse_elements=True, profile=profile
         )
-        if profile and profile >= "20.09":
+        if profile and Version(profile) >= Version("20.09"):
             element_tests[identifier][1]["expected_sort_order"] = idx
 
     return element_tests
 
 
 def __parse_test_attributes(output_elem, attrib, parse_elements=False, parse_discovered_datasets=False, profile=None):
     assert_list = __parse_assert_list(output_elem)
@@ -786,14 +786,17 @@
     # Allow a file size to vary if sim_size compare
     attributes["delta"] = int(attrib.pop("delta", DEFAULT_DELTA))
     attributes["delta_frac"] = float(attrib["delta_frac"]) if "delta_frac" in attrib else DEFAULT_DELTA_FRAC
     attributes["sort"] = string_as_bool(attrib.pop("sort", False))
     attributes["decompress"] = string_as_bool(attrib.pop("decompress", False))
     # `location` may contain an URL to a remote file that will be used to download `file` (if not already present on disk).
     location = attrib.get("location")
+    # Parameters for "image_diff" comparison
+    attributes["metric"] = attrib.pop("metric", DEFAULT_METRIC)
+    attributes["eps"] = float(attrib.pop("eps", DEFAULT_EPS))
     if location and file is None:
         file = os.path.basename(location)  # If no file specified, try to get filename from URL last component
     attributes["location"] = location
     try:
         attributes["count"] = int(attrib.pop("count"))
     except KeyError:
         attributes["count"] = None
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/parser/yaml.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/yaml.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,18 +283,19 @@
         # not sure these are used though.
         if "that" not in assertion:
             new_assertion = {}
             for assertion_key, assertion_value in assertion.items():
                 new_assertion["that"] = assertion_key
                 new_assertion.update(assertion_value)
             assertion = new_assertion
-        children = []
-        if "children" in assertion:
-            children = assertion["children"]
-            del assertion["children"]
+        children = assertion.pop("asserts", assertion.pop("children", []))
+        # if there are no nested assertions then children should be []
+        # but to_test_assert_list would return None
+        if children:
+            children = to_test_assert_list(children)
         assert_dict: AssertionDict = dict(
             tag=assertion["that"],
             attributes=assertion,
             children=children,
         )
         assert_list.append(assert_dict)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/provided_metadata.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/provided_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/base.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,22 +257,22 @@
     def _init_tools_from_configs(self, config_filenames):
         """Read through all tool config files and initialize tools in each
         with init_tools_from_config below.
         """
         execution_timer = ExecutionTimer()
         self._tool_tag_manager.reset_tags()
         config_filenames = listify(config_filenames)
-        for config_filename in config_filenames:
-            if os.path.isdir(config_filename):
-                directory_contents = sorted(os.listdir(config_filename))
-                directory_config_files = [
-                    config_file for config_file in directory_contents if config_file.endswith(".xml")
-                ]
-                config_filenames.remove(config_filename)
-                config_filenames.extend(directory_config_files)
+        config_directories = [config_filename for config_filename in config_filenames if os.path.isdir(config_filename)]
+        config_filenames = [
+            config_filename for config_filename in config_filenames if config_filename not in config_directories
+        ]
+        for config_directory in config_directories:
+            directory_contents = sorted(os.listdir(config_directory))
+            directory_config_files = [config_file for config_file in directory_contents if config_file.endswith(".xml")]
+            config_filenames.extend(directory_config_files)
         for config_filename in config_filenames:
             if not self.can_load_config_file(config_filename):
                 continue
             try:
                 self._init_tools_from_config(config_filename)
             except etree.ParseError:
                 # Occasionally we experience "Missing required parameter 'shed_tool_conf'."
@@ -371,15 +371,15 @@
 
         return None
 
     def panel_views(self) -> List[ToolPanelViewModel]:
         return [v.to_model() for v in self._tool_panel_views.values()]
 
     def panel_view_dicts(self) -> Dict[str, Dict]:
-        return {m.id: m.dict() for m in self.panel_views()}
+        return {m.id: m.model_dump(mode="json") for m in self.panel_views()}
 
     def panel_has_tool(self, tool, panel_view_id):
         panel_view_rendered = self._tool_panel_view_rendered[panel_view_id]
         return panel_view_rendered.has_item_recursive(tool)
 
     def load_dynamic_tool(self, dynamic_tool):
         if not dynamic_tool.active:
@@ -657,14 +657,17 @@
                 self._integrated_tool_panel.stub_tool(key)
             elif elem.tag == "workflow":
                 self._integrated_tool_panel.stub_workflow(key)
             elif elem.tag == "section":
                 section = ToolSection(elem)
                 for section_elem in elem:
                     section_id = section_elem.get("id")
+                    assert (
+                        section_id
+                    ), f"Element '{etree.tostring(section_elem, encoding='unicode')}' did not specify 'id' attribute"
                     if section_elem.tag == "tool":
                         section.elems.stub_tool(section_id)
                     elif section_elem.tag == "workflow":
                         section.elems.stub_workflow(section_id)
                     elif section_elem.tag == "label":
                         section.elems.stub_label(section_id)
                 self._integrated_tool_panel.append_section(key, section)
@@ -756,17 +759,14 @@
         return None
 
     def has_tool(self, tool_id: str, tool_version: Optional[str] = None, exact: bool = False):
         return self.get_tool(tool_id, tool_version=tool_version, exact=exact) is not None
 
     def is_missing_shed_tool(self, tool_id: str) -> bool:
         """Confirm that the tool ID does reference a shed tool and is not installed."""
-        if tool_id is None:
-            # This is not a tool ID.
-            return False
         if "repos" not in tool_id:
             # This is not a shed tool.
             return False
         # This is a valid tool, and it is from a toolshed. Check if it's
         # missing from the toolbox.
         if tool_id not in self._tools_by_id:
             return True
@@ -1382,16 +1382,15 @@
 
     def _build_filter_method(self, trans):
         context = Bunch(toolbox=self, trans=trans)
         filters = self._filter_factory.build_filters(trans)
         return lambda element, item_type: _filter_for_panel(element, item_type, filters, context)
 
     @abc.abstractmethod
-    def _looks_like_a_tool(self, path: str) -> bool:
-        ...
+    def _looks_like_a_tool(self, path: str) -> bool: ...
 
 
 def _filter_for_panel(item, item_type, filters, context):
     """
     Filters tool panel elements so that only those that are compatible
     with provided filters are kept.
     """
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/filters/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/filters/examples.py.sample` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/examples.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/integrated_panel.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/integrated_panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/factory.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/lineages/interface.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/panel.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/parser.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module is used to parse tool_conf files.
 
 These files define tool lists, sections, labels, etc... the elements of the
 Galaxy tool panel.
 """
+
 from abc import (
     ABCMeta,
     abstractmethod,
 )
 
 import yaml
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/definitions.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/definitions.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,21 @@
     List,
     Optional,
     Union,
 )
 
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
 )
-from typing_extensions import Literal
+from typing_extensions import (
+    Annotated,
+    Literal,
+)
 
 
 class StaticToolBoxViewTypeEnum(str, Enum):
     generic = "generic"
     activity = "activity"
     publication = "publication"
     training = "training"
@@ -34,49 +38,43 @@
 
 
 Exclusions = Union[
     ExcludeTool,
     ExcludeToolRegex,
     ExcludeTypes,
 ]
-OptionalExclusionList = Optional[List[Exclusions]]
+OptionalExclusionList = Annotated[Optional[List[Exclusions]], Field(None)]
 
 
 class Tool(BaseModel):
     content_type: Literal["tool"] = Field("tool", alias="type")
     id: str
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class Label(BaseModel):
     content_type: Literal["label"] = Field(alias="type", default="label")
-    id: Optional[str]
+    id: Optional[str] = None
     text: str
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class LabelShortcut(BaseModel):
-    content_type = "simple_label"
+    content_type: Literal["simple_label"] = "simple_label"
     label: str
 
 
 class Workflow(BaseModel):
     content_type: Literal["workflow"] = Field(alias="type", default="workflow")
     id: str
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class ItemsFrom(BaseModel):
-    content_type = "items_from"
+    content_type: Literal["items_from"] = "items_from"
     items_from: str
     excludes: OptionalExclusionList
 
 
 SectionContent = Union[
     Tool,
     Label,
@@ -116,33 +114,31 @@
             else:
                 items.append(item)
         return items
 
 
 class Section(BaseModel, HasItems):
     content_type: Literal["section"] = Field(alias="type")
-    id: Optional[str]
-    name: Optional[str]
-    items: Optional[List[SectionContent]]
+    id: Optional[str] = None
+    name: Optional[str] = None
+    items: Optional[List[SectionContent]] = None
     excludes: OptionalExclusionList
-
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
 
 
 class SectionAlias(BaseModel):
-    content_type = "section_alias"
+    content_type: Literal["section_alias"] = "section_alias"
     section: str
-    excludes: OptionalExclusionList
+    excludes: OptionalExclusionList = None
 
 
 class SectionAliases(BaseModel):
-    content_type = "section_aliases"
+    content_type: Literal["section_aliases"] = "section_aliases"
     sections: List[str]
-    excludes: OptionalExclusionList
+    excludes: OptionalExclusionList = None
 
 
 RootContent = Union[
     Section,
     SectionAlias,
     SectionAliases,
     Tool,
@@ -161,18 +157,17 @@
     ItemsFrom,
 ]
 
 
 class StaticToolBoxView(BaseModel, HasItems):
     id: str
     name: str
-    description: Optional[str]
+    description: Optional[str] = None
     view_type: StaticToolBoxViewTypeEnum = Field(alias="type")
-    items: Optional[List[RootContent]]  # if empty, use integrated tool panel
+    items: Optional[List[RootContent]] = None  # if empty, use integrated tool panel
     excludes: OptionalExclusionList
 
     @staticmethod
     def from_dict(as_dict):
         return StaticToolBoxView(**as_dict)
 
-    class Config:
-        allow_population_by_field_name = True
+    model_config = ConfigDict(populate_by_name=True)
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/edam.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/edam.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/interface.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/interface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from abc import abstractmethod
 from enum import Enum
 from typing import Optional
 
-from pydantic import BaseModel
+from pydantic import (
+    BaseModel,
+    ConfigDict,
+)
 
 from ..panel import (
     HasPanelItems,
     panel_item_types,
     ToolPanelElements,
 )
 
@@ -22,17 +25,18 @@
 
 class ToolPanelViewModel(BaseModel):
     """A view of ToolPanelView objects serialized for the API."""
 
     id: str
     model_class: str
     name: str
-    description: Optional[str]
+    description: Optional[str] = None
     view_type: ToolPanelViewModelType
     searchable: bool  # Allow for more dynamic views that don't plug into fixed search indicies in the future...
+    model_config = ConfigDict(protected_namespaces=())
 
 
 class ToolBoxRegistry:
     """View of ToolBox provided to ToolPanelView to reason about tools loaded."""
 
     @abstractmethod
     def has_tool(self, tool_id: str) -> bool:
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/sources.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/sources.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/views/static.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/static.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                     else:
                         closest_section = base_tool_panel.closest_section(section_def.id, section_def.name)
                         if closest_section is None:
                             log.warning(
                                 f"Failed to find matching section for (id, name) = ({section_def.id}, {section_def.name})"
                             )
                             continue
-                        section = closest_section.copy()
+                        section = closest_section.copy(merge_tools=True)
                         if section_def.id is not None:
                             section.id = section_def.id
                         if section_def.name is not None:
                             section.name = section_def.name
                         apply_filter(section_def, section.elems)
                     new_panel.append_section(section.id, section)
                 elif element.content_type == "section_alias":
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/toolbox/watcher.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/watcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
                             do_reload = True
                 except OSError:
                     # in rare cases `path` may be deleted between `os.path.exists` calls
                     # and reading the file from the filesystem. We do not want the watcher
                     # thread to die in these cases.
                     if path in drop_now:
                         log.warning("'%s' could not be read, removing from watched files", path)
-                        del paths[path]
+                        del self.paths[path]
                         if path in hashes:
                             del hashes[path]
                     else:
                         log.debug("'%s could not be read", path)
                         drop_on_next_loop.add(path)
                     if self.cache:
                         self.cache.cleanup()
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/unittest_utils/interactor.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,77 @@
 """Module of utilities for verifying test results."""
 
 import difflib
 import filecmp
 import hashlib
 import json
 import logging
+import math
 import os
 import os.path
 import re
 import shutil
 import tempfile
 from typing import (
     Any,
     Callable,
     Dict,
+    List,
     Optional,
+    TYPE_CHECKING,
 )
 
 try:
+    import numpy
+except ImportError:
+    pass
+try:
     import pysam
 except ImportError:
-    pysam = None  # type: ignore[assignment]
+    pass
+try:
+    from PIL import Image
+except ImportError:
+    pass
 
 from galaxy.tool_util.parser.util import (
     DEFAULT_DELTA,
     DEFAULT_DELTA_FRAC,
+    DEFAULT_EPS,
+    DEFAULT_METRIC,
 )
 from galaxy.util import unicodify
 from galaxy.util.compression_utils import get_fileobj
 from .asserts import verify_assertions
 from .test_data import TestDataResolver
 
+if TYPE_CHECKING:
+    import numpy.typing
+
 log = logging.getLogger(__name__)
 
 DEFAULT_TEST_DATA_RESOLVER = TestDataResolver()
 
 
 def verify(
     item_label: str,
     output_content: bytes,
-    attributes: Dict[str, Any],
+    attributes: Optional[Dict[str, Any]],
     filename: Optional[str] = None,
     get_filecontent: Optional[Callable[[str], bytes]] = None,
     get_filename: Optional[Callable[[str], str]] = None,
     keep_outputs_dir: Optional[str] = None,
     verify_extra_files: Optional[Callable] = None,
     mode="file",
 ):
     """Verify the content of a test output using test definitions described by attributes.
 
     Throw an informative assertion error if any of these tests fail.
     """
+    attributes = attributes or {}
     if get_filename is None:
         get_filecontent_: Callable[[str], bytes]
         if get_filecontent is None:
             get_filecontent_ = DEFAULT_TEST_DATA_RESOLVER.get_filecontent
         else:
             get_filecontent_ = get_filecontent
 
@@ -63,17 +80,17 @@
             local_name = make_temp_fname(fname=filename)
             with open(local_name, "wb") as f:
                 f.write(file_content)
             return local_name
 
     # Check assertions...
     assertions = attributes.get("assert_list", None)
-    if attributes is not None and assertions is not None:
+    if assertions is not None:
         try:
-            verify_assertions(output_content, attributes["assert_list"], attributes.get("decompress"))
+            verify_assertions(output_content, attributes["assert_list"], attributes.get("decompress", False))
         except AssertionError as err:
             errmsg = f"{item_label} different than expected\n"
             errmsg += unicodify(err)
             raise AssertionError(errmsg)
 
     # Verify checksum attributes...
     # works with older Galaxy style md5=<expected_sum> or cwltest
@@ -91,17 +108,14 @@
         try:
             _verify_checksum(output_content, expected_checksum_type, expected_checksum)
         except AssertionError as err:
             errmsg = f"{item_label} different than expected\n"
             errmsg += unicodify(err)
             raise AssertionError(errmsg)
 
-    if attributes is None:
-        attributes = {}
-
     # expected object might be None, so don't pull unless available
     has_expected_object = "object" in attributes
     if has_expected_object:
         assert filename is None
         expected_object = attributes.get("object")
         actual_object = json.loads(output_content)
 
@@ -169,14 +183,16 @@
                 files_re_match(local_name, temp_name, attributes=attributes)
             elif compare == "re_match_multiline":
                 files_re_match_multiline(local_name, temp_name, attributes=attributes)
             elif compare == "sim_size":
                 files_delta(local_name, temp_name, attributes=attributes)
             elif compare == "contains":
                 files_contains(local_name, temp_name, attributes=attributes)
+            elif compare == "image_diff":
+                files_image_diff(local_name, temp_name, attributes=attributes)
             else:
                 raise Exception(f"Unimplemented Compare type: {compare}")
         except AssertionError as err:
             errmsg = f"{item_label} different than expected, difference (using {compare}):\n"
             errmsg += f"( {local_name} v. {temp_name} )\n"
             errmsg += unicodify(err)
             raise AssertionError(errmsg)
@@ -430,7 +446,72 @@
     line_diff_count = 0
     for contains in local_file:
         contains = contains.rstrip(to_strip)
         if contains not in history_data:
             line_diff_count += 1
         if line_diff_count > lines_diff:
             raise AssertionError(f"Failed to find '{contains}' in history data. (lines_diff={lines_diff}).")
+
+
+def _multiobject_intersection_over_union(
+    mask1: "numpy.typing.NDArray", mask2: "numpy.typing.NDArray", repeat_reverse: bool = True
+) -> List["numpy.floating"]:
+    iou_list = []
+    for label1 in numpy.unique(mask1):
+        cc1 = mask1 == label1
+        cc1_iou_list = []
+        for label2 in numpy.unique(mask2[cc1]):
+            cc2 = mask2 == label2
+            cc1_iou_list.append(intersection_over_union(cc1, cc2))
+        iou_list.append(max(cc1_iou_list))
+    if repeat_reverse:
+        iou_list.extend(_multiobject_intersection_over_union(mask2, mask1, repeat_reverse=False))
+    return iou_list
+
+
+def intersection_over_union(mask1: "numpy.typing.NDArray", mask2: "numpy.typing.NDArray") -> "numpy.floating":
+    assert mask1.dtype == mask2.dtype
+    assert mask1.ndim == mask2.ndim == 2
+    assert mask1.shape == mask2.shape
+    if mask1.dtype == bool:
+        return numpy.logical_and(mask1, mask2).sum() / numpy.logical_or(mask1, mask2).sum()
+    else:
+        return min(_multiobject_intersection_over_union(mask1, mask2))
+
+
+def get_image_metric(
+    attributes: Dict[str, Any]
+) -> Callable[["numpy.typing.NDArray", "numpy.typing.NDArray"], "numpy.floating"]:
+    metric_name = attributes.get("metric", DEFAULT_METRIC)
+    metrics = {
+        "mae": lambda arr1, arr2: numpy.abs(arr1 - arr2).mean(),
+        # Convert to float before squaring to prevent overflows
+        "mse": lambda arr1, arr2: numpy.square((arr1 - arr2).astype(float)).mean(),
+        "rms": lambda arr1, arr2: math.sqrt(numpy.square((arr1 - arr2).astype(float)).mean()),
+        "fro": lambda arr1, arr2: numpy.linalg.norm((arr1 - arr2).reshape(1, -1), "fro"),
+        "iou": lambda arr1, arr2: 1 - intersection_over_union(arr1, arr2),
+    }
+    try:
+        return metrics[metric_name]
+    except KeyError:
+        raise ValueError(f'No such metric: "{metric_name}"')
+
+
+def files_image_diff(file1: str, file2: str, attributes: Optional[Dict[str, Any]] = None) -> None:
+    """Check the pixel data of 2 image files for differences."""
+    attributes = attributes or {}
+
+    with Image.open(file1) as im1:
+        arr1 = numpy.array(im1)
+    with Image.open(file2) as im2:
+        arr2 = numpy.array(im2)
+
+    if arr1.dtype != arr2.dtype:
+        raise AssertionError(f"Image data types did not match ({arr1.dtype}, {arr2.dtype}).")
+
+    if arr1.shape != arr2.shape:
+        raise AssertionError(f"Image dimensions did not match ({arr1.shape}, {arr2.shape}).")
+
+    distance = get_image_metric(attributes)(arr1, arr2)
+    distance_eps = attributes.get("eps", DEFAULT_EPS)
+    if distance > distance_eps:
+        raise AssertionError(f"Image difference {distance} exceeds eps={distance_eps}.")
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/__init__.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         log.exception("Failed to load assertion module: %s", assertion_module_name)
         continue
     for member, value in getmembers(assertion_module):
         if member.startswith("assert_"):
             assertion_functions[member] = value
 
 
-def verify_assertions(data: bytes, assertion_description_list, decompress=None):
+def verify_assertions(data: bytes, assertion_description_list, decompress: bool = False):
     """This function takes a list of assertions and a string to check
     these assertions against."""
     if decompress:
         with NamedTemporaryFile() as tmpfh:
             tmpfh.write(data)
             tmpfh.flush()
             with get_fileobj(tmpfh.name, mode="rb", compressed_formats=None) as fh:
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/_util.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/archive.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/archive.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/hdf5.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/hdf5.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/json.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/size.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/size.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 
 from ._util import _assert_number
 
 
 def assert_has_size(
     output_bytes: bytes,
     value: Optional[Union[int, str]] = None,
+    size: Optional[Union[int, str]] = None,
     delta: Union[int, str] = 0,
     min: Optional[Union[int, str]] = None,
     max: Optional[Union[int, str]] = None,
     negate: Union[bool, str] = False,
 ) -> None:
     """
-    Asserts the specified output has a size of the specified value,
+    Asserts the specified output has a size of the specified value
+    (size and value or synonyms),
     allowing for absolute (delta) and relative (delta_frac) difference.
     """
     output_size = len(output_bytes)
+    if size is None:
+        size = value
     _assert_number(
         output_size,
         value,
         delta,
         min,
         max,
         negate,
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/tabular.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/tabular.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/text.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/text.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/asserts/xml.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/xml.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     # check sub-assertions
     if len(children) == 0 or verify_assertions_function is None:
         return
     for occ in xml.findall(path):
         if attribute is None or attribute == "":
             content = occ.text
         else:
-            content = occ.attrib[attribute]
+            content = occ.attrib[attribute]  # type: ignore[assignment] # https://github.com/lxml/lxml-stubs/pull/99
         try:
             verify_assertions_function(content, children)
         except AssertionError as e:
             if attribute is not None and attribute != "":
                 raise AssertionError(f"Attribute '{attribute}' on element with path '{path}': {str(e)}")
             else:
                 raise AssertionError(f"Text of element with path '{path}': {str(e)}")
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/interactor.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/interactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -955,22 +955,29 @@
     def _put(self, path, data=None, key=None, headers=None, admin=False, anon=False, json=False):
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
         url = self.get_api_url(path)
         kwd = self._prepare_request_params(data=data, as_json=json, headers=headers)
         kwd["timeout"] = kwd.pop("timeout", util.DEFAULT_SOCKET_TIMEOUT)
         return requests.put(url, **kwd)
 
-    def _get(self, path, data=None, key=None, headers=None, admin=False, anon=False):
+    def _get(self, path, data=None, key=None, headers=None, admin=False, anon=False, allow_redirects=True):
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
         url = self.get_api_url(path)
         kwargs: Dict[str, Any] = {}
         if self.cookies:
             kwargs["cookies"] = self.cookies
         # no data for GET
-        return requests.get(url, params=data, headers=headers, timeout=util.DEFAULT_SOCKET_TIMEOUT, **kwargs)
+        return requests.get(
+            url,
+            params=data,
+            headers=headers,
+            timeout=util.DEFAULT_SOCKET_TIMEOUT,
+            allow_redirects=allow_redirects,
+            **kwargs,
+        )
 
     def _head(self, path, data=None, key=None, headers=None, admin=False, anon=False):
         headers = self.api_key_header(key=key, admin=admin, anon=anon, headers=headers)
         url = self.get_api_url(path)
         kwargs: Dict[str, Any] = {}
         if self.cookies:
             kwargs["cookies"] = self.cookies
@@ -1267,16 +1274,15 @@
             )
     finally:
         for path in cleanup_directories:
             shutil.rmtree(path)
 
 
 class TestConfig(Protocol):
-    def get_test_config(self, job_data: Dict[str, Any]) -> Optional[Dict[str, Any]]:
-        ...
+    def get_test_config(self, job_data: Dict[str, Any]) -> Optional[Dict[str, Any]]: ...
 
 
 class NullClientTestConfig(TestConfig):
     def get_test_config(self, job_data):
         return None
 
 
@@ -1420,16 +1426,14 @@
             else:
                 expected_failure_occurred = True
         except Exception as e:
             tool_execution_exception = e
             raise e
 
         if not expected_failure_occurred:
-            assert data_list or data_collection_list
-
             try:
                 job_stdio = _verify_outputs(
                     testdef, test_history, jobs, data_list, data_collection_list, galaxy_interactor, quiet=quiet
                 )
             except JobOutputsError as e:
                 job_stdio = e.job_stdio
                 job_output_exceptions = e.output_exceptions
@@ -1479,15 +1483,14 @@
         else:
             raise Exception("Test parse failure")
 
 
 def _verify_outputs(testdef, history, jobs, data_list, data_collection_list, galaxy_interactor, quiet=False):
     assert len(jobs) == 1, "Test framework logic error, somehow tool test resulted in more than one job."
     job = jobs[0]
-
     found_exceptions: List[Exception] = []
 
     def register_exception(e: Exception):
         if not found_exceptions and not quiet:
             # Only print this stuff out once.
             for stream in ["stdout", "stderr"]:
                 if stream in job_stdio:
@@ -1532,37 +1535,44 @@
 
     for output_index, output_dict in enumerate(testdef.outputs):
         # Get the correct hid
         name = output_dict["name"]
         outfile = output_dict["value"]
         attributes = output_dict["attributes"]
         output_testdef = Bunch(name=name, outfile=outfile, attributes=attributes)
+        output_data = None
         try:
             output_data = data_list[name]
         except (TypeError, KeyError):
             # Legacy - fall back on ordered data list access if data_list is
             # just a list (case with twill variant or if output changes its
             # name).
-            if hasattr(data_list, "values"):
-                output_data = list(data_list.values())[output_index]
-            else:
-                output_data = data_list[len(data_list) - len(testdef.outputs) + output_index]
-        assert output_data is not None
-        try:
-            galaxy_interactor.verify_output(
-                history,
-                jobs,
-                output_data,
-                output_testdef=output_testdef,
-                tool_id=job["tool_id"],
-                maxseconds=maxseconds,
-                tool_version=testdef.tool_version,
-            )
-        except Exception as e:
-            register_exception(e)
+            try:
+                if hasattr(data_list, "values"):
+                    output_data = list(data_list.values())[output_index]
+                else:
+                    output_data = data_list[len(data_list) - len(testdef.outputs) + output_index]
+            except IndexError:
+                error = AssertionError(
+                    f"Tool did not produce an output with name '{name}' (or at index {output_index})"
+                )
+                register_exception(error)
+        if output_data:
+            try:
+                galaxy_interactor.verify_output(
+                    history,
+                    jobs,
+                    output_data,
+                    output_testdef=output_testdef,
+                    tool_id=job["tool_id"],
+                    maxseconds=maxseconds,
+                    tool_version=testdef.tool_version,
+                )
+            except Exception as e:
+                register_exception(e)
 
     other_checks = {
         "command_line": "Command produced by the job",
         "command_version": "Tool version indicated during job execution",
         "stdout": "Standard output of the job",
         "stderr": "Standard error of the job",
     }
@@ -1644,27 +1654,64 @@
     def __init__(self, output_exceptions, job_stdio):
         big_message = "\n".join(map(util.unicodify, output_exceptions))
         super().__init__(big_message)
         self.job_stdio = job_stdio
         self.output_exceptions = output_exceptions
 
 
+class ToolTestDescriptionDict(TypedDict):
+    name: str
+    inputs: Any
+    outputs: Any
+    output_collections: List[Dict[str, Any]]
+    stdout: Optional[AssertionList]
+    stderr: Optional[AssertionList]
+    expect_exit_code: Optional[int]
+    expect_failure: bool
+    expect_test_failure: bool
+    num_outputs: Optional[int]
+    command_line: Optional[AssertionList]
+    command_version: Optional[AssertionList]
+    required_files: List[Any]
+    required_data_tables: List[Any]
+    required_loc_files: List[str]
+    error: bool
+    tool_id: str
+    tool_version: Optional[str]
+    test_index: int
+    exception: Optional[str]
+
+
 class ToolTestDescription:
     """
     Encapsulates information about a tool test, and allows creation of a
     dynamic TestCase class (the unittest framework is very class oriented,
     doing dynamic tests in this way allows better integration)
     """
 
+    name: str
+    num_outputs: Optional[int]
+    stdout: Optional[AssertionList]
+    stderr: Optional[AssertionList]
+    command_line: Optional[AssertionList]
+    command_version: Optional[AssertionList]
+    required_files: List[Any]
+    required_data_tables: List[Any]
+    required_loc_files: List[str]
+    expect_exit_code: Optional[int]
+    expect_failure: bool
+    expect_test_failure: bool
+    exception: Optional[str]
+
     def __init__(self, processed_test_dict: ToolTestDict):
         assert (
             "test_index" in processed_test_dict
         ), "Invalid processed test description, must have a 'test_index' for naming, etc.."
         test_index = processed_test_dict["test_index"]
-        name = processed_test_dict.get("name", f"Test-{test_index + 1}")
+        name = cast(str, processed_test_dict.get("name", f"Test-{test_index + 1}"))
         error_in_test_definition = processed_test_dict["error"]
         if not error_in_test_definition:
             processed_test_dict = cast(ValidToolTestDict, processed_test_dict)
             maxseconds = int(processed_test_dict.get("maxseconds") or DEFAULT_TOOL_TEST_WAIT or 86400)
             output_collections = processed_test_dict.get("output_collections", [])
         else:
             processed_test_dict = cast(InvalidToolTestDict, processed_test_dict)
@@ -1675,49 +1722,49 @@
         assert (
             "tool_id" in processed_test_dict
         ), "Invalid processed test description, must have a 'tool_id' for naming, etc.."
         self.tool_id = processed_test_dict["tool_id"]
         self.tool_version = processed_test_dict.get("tool_version")
         self.name = name
         self.maxseconds = maxseconds
-        self.required_files = processed_test_dict.get("required_files", [])
-        self.required_data_tables = processed_test_dict.get("required_data_tables", [])
-        self.required_loc_files = processed_test_dict.get("required_loc_files", [])
+        self.required_files = cast(List[Any], processed_test_dict.get("required_files", []))
+        self.required_data_tables = cast(List[Any], processed_test_dict.get("required_data_tables", []))
+        self.required_loc_files = cast(List[str], processed_test_dict.get("required_loc_files", []))
 
         inputs = processed_test_dict.get("inputs", {})
         loaded_inputs = {}
         for key, value in inputs.items():
             if isinstance(value, dict) and value.get("model_class"):
                 loaded_inputs[key] = TestCollectionDef.from_dict(value)
             else:
                 loaded_inputs[key] = value
 
         self.inputs = loaded_inputs
         self.outputs = processed_test_dict.get("outputs", [])
-        self.num_outputs = processed_test_dict.get("num_outputs", None)
+        self.num_outputs = cast(Optional[int], processed_test_dict.get("num_outputs", None))
 
         self.error = processed_test_dict.get("error", False)
-        self.exception = processed_test_dict.get("exception", None)
+        self.exception = cast(Optional[str], processed_test_dict.get("exception", None))
 
         self.output_collections = [TestCollectionOutputDef.from_dict(d) for d in output_collections]
-        self.command_line = processed_test_dict.get("command_line", None)
-        self.command_version = processed_test_dict.get("command_version", None)
-        self.stdout = processed_test_dict.get("stdout", None)
-        self.stderr = processed_test_dict.get("stderr", None)
-        self.expect_exit_code = processed_test_dict.get("expect_exit_code", None)
-        self.expect_failure = processed_test_dict.get("expect_failure", False)
-        self.expect_test_failure = processed_test_dict.get("expect_test_failure", False)
+        self.command_line = cast(Optional[AssertionList], processed_test_dict.get("command_line", None))
+        self.command_version = cast(Optional[AssertionList], processed_test_dict.get("command_version", None))
+        self.stdout = cast(Optional[AssertionList], processed_test_dict.get("stdout", None))
+        self.stderr = cast(Optional[AssertionList], processed_test_dict.get("stderr", None))
+        self.expect_exit_code = cast(Optional[int], processed_test_dict.get("expect_exit_code", None))
+        self.expect_failure = cast(bool, processed_test_dict.get("expect_failure", False))
+        self.expect_test_failure = cast(bool, processed_test_dict.get("expect_test_failure", False))
 
     def test_data(self):
         """
         Iterator over metadata representing the required files for upload.
         """
         return test_data_iter(self.required_files)
 
-    def to_dict(self):
+    def to_dict(self) -> ToolTestDescriptionDict:
         inputs_dict = {}
         for key, value in self.inputs.items():
             if hasattr(value, "to_dict"):
                 inputs_dict[key] = value.to_dict()
             else:
                 inputs_dict[key] = value
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/script.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/test_config.sample.yml` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_config.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/test_data.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/verify/wait.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/wait.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/version.py` & `galaxy-tool-util-24.0.0/galaxy/tool_util/version.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/LICENSE` & `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/README.md` & `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/galaxy.jxb` & `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.jxb`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.xsd`

 * *Files 0% similar despite different names*

#### Comparing `galaxy-tool-util-23.2.dev0/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.xsd`

```diff
@@ -48,20 +48,26 @@
 
 - Exit immediately if a command exits with a non-zero status (`set -e`).
 - Assume sort order for collection elements.
 
 ### 21.09
 
 - Do not strip leading and trailing whitespaces in `from_work_dir` attribute.
+- Do not use Galaxy Python virtual environment for `data_source` tools. `data_source` tools should explicitly use the `galaxy-util` package.
 
 ### 23.0
 
 - Text parameters that are inferred to be optional (i.e the `optional` tag is not set, but the tool parameter accepts an empty string)
   are set to `None` for templating in Cheetah. Older tools receive the empty string `""` as the templated value.
 
+### 24.0
+
+- Do not use Galaxy python environment for `data_source_async` tools.
+- Drop request parameters received by data source tools that are not declared in `<request_param_translation>` section.
+
 ### Examples
 
 A normal tool:
 
 ```xml
 <tool id="seqtk_seq"
       name="Convert FASTQ to FASTA"
@@ -208,21 +214,22 @@
         </xs:annotation>
       </xs:attribute>
       <xs:attribute name="tool_type" type="ToolTypeType">
         <xs:annotation>
           <xs:documentation xml:lang="en">Allows for certain framework
 functionality to be performed on certain types of tools. Normal tools that execute
 typical command-line jobs do not need to specify this, special kinds of tools such
-as [Data Source](https://galaxyproject.org/admin/internals/data-sources/) and
+as [Data Source](https://docs.galaxyproject.org/en/latest/dev/data_source.html) and
 [Data Manager](https://galaxyproject.org/admin/tools/data-managers/) tools should
-set this to have values such as ``data_source`` or ``manage_data``.</xs:documentation>
+set this to have values such as ``data_source``, ``data_source_async`` or
+``manage_data``.</xs:documentation>
         </xs:annotation>
       </xs:attribute>
       <xs:attribute name="profile" type="xs:string">
-        <xs:annotation>
+        <xs:annotation gxdocs:best_practices="tool-profile">
           <xs:documentation xml:lang="en">This string specifies the minimum Galaxy
 version that should be required to run this tool. Certain legacy behaviors such
 as using standard error content to detect errors instead of exit code are disabled
 automatically if profile is set to any version newer than ``16.01``. See above
 for the list of behavior changes associated with profile versions.</xs:documentation>
         </xs:annotation>
       </xs:attribute>
@@ -250,17 +257,24 @@
           <xs:documentation xml:lang="en">This attribute indicates if
 this tool is usable within a workflow (defaults to ``true`` for normal tools and
 ``false`` for data sources).</xs:documentation>
         </xs:annotation>
       </xs:attribute>
       <xs:attribute name="URL_method" type="URLmethodType">
         <xs:annotation>
-          <xs:documentation xml:lang="en">Only used if ``tool_type`` attribute value
-is ``data_source`` - this attribute defines the HTTP request method to use when
-communicating with an external data source application (the default is ``get``).</xs:documentation>
+          <xs:documentation xml:lang="en">*Deprecated* and ignored,
+use a [request_param](#tool-request-param-translation-request-param) element with ``galaxy_name=&quot;URL_method&quot;`` instead.
+Was only used if ``tool_type`` attribute value is ``data_source`` or ``data_source_async`` -
+this attribute defined the HTTP request method to use when communicating with an external data source application
+(default: ``get``).</xs:documentation>
+        </xs:annotation>
+      </xs:attribute>
+      <xs:attribute name="require_login" type="xs:boolean">
+        <xs:annotation>
+          <xs:documentation xml:lang="en">Documentation needed</xs:documentation>
         </xs:annotation>
       </xs:attribute>
     </xs:complexType>
   </xs:element>
   <xs:complexType name="Macros">
     <xs:annotation>
       <xs:documentation xml:lang="en">Frequently, tools may require the same XML
@@ -324,14 +338,26 @@
 Usage example:
 ````
 <expand macro="citations" />
 ````
        ]]></xs:documentation>
         </xs:annotation>
       </xs:element>
+      <xs:element name="macro" type="xs:anyType" minOccurs="0" maxOccurs="unbounded">
+        <xs:annotation>
+          <xs:documentation xml:lang="en"><![CDATA[
+A generalisation for macro tokens, templates and xml macros, i.e.
+`<macro name="an_xml_macro" type="xml">` is identical to `<xml name="an_xml_macro">`,
+`<macro name="a_template" type="template">` is identical to `<template name="a_template">`, and
+`<macro name="a_token" type="xml">` is identical to `<token name="a_token">`.
+
+Note that 
+       ]]></xs:documentation>
+        </xs:annotation>
+      </xs:element>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="EntryPoints">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[
 
 This is a container tag set for the ``entry_point`` tag that contains ``port`` and ``url`` tags
@@ -1584,15 +1610,15 @@
 ``file`` attribute value or checked against assertions made by a child
 ``assert_contents`` tag to verify that the tool is functionally correct.
 
 Different methods can be chosen for the comparison with the local file specified
 by ``file`` using the ``compare`` attribute:
 
 - ``diff``: uses diff to compare the history data set and the file provided by
-  ``file``. Compressed files are decompressed before the compariopm if
+  ``file``. Compressed files are decompressed before the comparison if
   ``decompress`` is set to ``true``. BAM files are converted to SAM before the
   comparision and for pdf some special rules are implemented. The number of
   allowed differences can be set with ``lines_diff``.  If ``sort="true"`` history
   and local data is sorted before the comparison.
 - ``re_match``: each line of the history data set is compared to the regular
   expression specified in the corresponding line of the ``file``. The allowed
   number of non matching lines can be set with ``lines_diff`` and the history
@@ -1602,14 +1628,18 @@
   before the comparison if the ``sort`` atrribute is set to ``true``.
 - ``contains``: check if each line in ``file`` is contained in the history data set.
   The allowed number of lines that are not contained in the history dataset
   can be set with ``lines_diff``.
 - ``sim_size``: compares the size of the history dataset and the ``file`` subject to
   the values of the ``delta`` and ``delta_frac`` attributes. Note that a ``has_size``
   content assertion should be preferred, because this avoids storing the test file.
+- ``image_diff``: compares the pixel data of the history data set and the file
+  provided by ``file``. The difference of the images is quantified according to their
+  pixel-wise distance with respect to a specific ``metric``. The check passes if the
+  distance is not larger than the value set for ``eps``. Only 2-D images can be used.
 
         ]]></xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:group ref="TestOutputElement" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
     <!-- TODO: This would be more percise if this was required if at the top-level. -->
@@ -1670,28 +1700,28 @@
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="md5" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en"><![CDATA[
 
 If specified, the target output's MD5 hash should match the value specified
-here. For large static files it may be inconvenient to upload the entiry file
+here. For large static files it may be inconvenient to upload the entire file
 and this can be used instead.
 
 ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="checksum" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en"><![CDATA[
 
 If specified, the target output's checksum should match the value specified
 here. This value should have the form ``hash_type$hash_value``
 (e.g. ``sha1$8156d7ca0f46ed7abac98f82e36cfaddb2aca041``). For large static files
-it may be inconvenient to upload the entiry file and this can be used instead.
+it may be inconvenient to upload the entire file and this can be used instead.
 
 ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="compare" type="TestOutputCompareType"/>
     <xs:attribute name="lines_diff" type="xs:integer">
       <xs:annotation>
@@ -1737,14 +1767,20 @@
 - In combination with `file` it will look for the output file in the `test-data` folder, if it's not available on disk it will
 download the file pointed by `location` using the same name as in `file` (or `value`).
 - Specifiying the `location` without a `file` (or `value`), it will download the file and use it as an alias of `file`. The name of the file
 will be infered from the last component of the location URL. For example, `location=&quot;https://my_url/my_file.txt&quot;` will be equivalent to `file=&quot;my_file.txt&quot;`.
 If you specify a `checksum`, it will be also used to check the integrity of the download.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
+    <xs:attribute name="metric" type="TestOutputMetricType" default="mae"/>
+    <xs:attribute name="eps" type="xs:float" default="0.01">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">If ``compare`` is set to ``image_diff``, this is the maximum allowed distance between the data set that is generated in the test and the file in ``test-data/`` that is referenced by the ``file`` attribute, with distances computed with respect to the specified ``metric``. Default value is 0.01.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
   </xs:complexType>
   <xs:group name="TestOutputElement">
     <xs:choice>
       <xs:element name="element" type="TestOutput"/>
       <!-- TODO: This would be more precise if this was only allowed at the top-level. -->
       <xs:element name="discovered_dataset" type="TestDiscoveredDataset"/>
       <!-- TODO: To be more precise only one assert_contents is allowed - this should not be in here. -->
@@ -2172,19 +2208,24 @@
 ``delta``, e.g. ``<has_size value="10000" delta="100" />``.
 Alternatively the range of the expected size can be specified by ``min`` and/or
 ``max``.
 
 $attribute_list::5
 ]]></xs:documentation>
     </xs:annotation>
-    <xs:attribute name="value" type="Bytes" use="optional">
+    <xs:attribute name="size" type="Bytes" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Desired size of the output (in bytes), can be suffixed by ``(k|M|G|T|P|E)i?``</xs:documentation>
       </xs:annotation>
     </xs:attribute>
+    <xs:attribute name="value" type="Bytes" use="optional">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">An outdated alias for `size`</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
     <xs:attribute name="delta" type="Bytes" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Maximum allowed size difference (default is 0). The observed size has to be in the range ``value +- delta``. Can be suffixed by ``(k|M|G|T|P|E)i?``</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="min" type="Bytes" use="optional">
       <xs:annotation>
@@ -2771,15 +2812,17 @@
     <xs:attribute name="check_values" type="PermissiveBoolean" default="true">
       <xs:annotation>
         <xs:documentation xml:lang="en">Set to ``false`` to disable parameter checking in data source tools.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="method" type="URLmethodType">
       <xs:annotation>
-        <xs:documentation xml:lang="en">Data source HTTP action (e.g. ``get`` or ``put``) to use.</xs:documentation>
+        <xs:documentation xml:lang="en">*Deprecated* and ignored,
+use a [request_param](#tool-request-param-translation-request-param) element with ``galaxy_name=&quot;URL_method&quot;`` instead.
+Data source HTTP action (e.g. ``get`` or ``put``) to use.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="target" type="TargetType">
       <xs:annotation>
         <xs:documentation xml:lang="en">UI link target to use for data source tools (e.g. ``_top``).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
@@ -2896,18 +2939,18 @@
 The Bowtie 2 wrapper also demonstrates other conditional paths - such as choosing
 between paired inputs of single stranded inputs.
 ]]></xs:documentation>
     </xs:annotation>
     <xs:complexContent>
       <xs:extension base="InputType">
         <xs:sequence>
-          <xs:group ref="InputElement" minOccurs="0" maxOccurs="1"/>
+          <xs:element name="param" type="Param" minOccurs="1" maxOccurs="1"/>
           <xs:element name="when" type="ConditionalWhen" minOccurs="0" maxOccurs="unbounded"/>
         </xs:sequence>
-        <xs:attribute name="name" type="xs:string">
+        <xs:attribute name="name" type="xs:string" use="required">
           <xs:annotation>
             <xs:documentation xml:lang="en">Name for this element</xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="value_from" type="xs:string">
           <xs:annotation>
             <xs:documentation xml:lang="en"><![CDATA[Infrequently used option to dynamically access Galaxy internals, this should be avoided.
@@ -3329,15 +3372,17 @@
 </param>
 ```
 
 $attribute_list:data_ref,dynamic_options,display,multiple:5
 
 #### ``data_column``
 
-This parameter type is used to select columns from a parameter.
+This parameter type is used to select columns from a data parameter.
+It uses the ``column_names`` metadata if present (only since 24.0)
+and as a fallback the tab separated values of the first line.
 
 $attribute_list:force_select,numerical,use_header_name,multiple:5
 
 #### ``drill_down``
 
 Allows to select values from a hierarchy. The default (``hierarchy="exact"``) is
 that only exactly the selected options are used. With ``hierarchy="recurse"``
@@ -3437,15 +3482,15 @@
           <xs:annotation>
             <xs:documentation xml:lang="en">Boolean indicating if this should be
 rendered as a one line text box (if ``false``, the default) or a multi-line text
  area (if ``true``). Used only when the ``type`` attribute value is ``text``.</xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="argument" type="xs:string">
-          <xs:annotation>
+          <xs:annotation gxdocs:best_practices="parameter-name-argument-and-help">
             <xs:documentation xml:lang="en"><![CDATA[
 
 If the parameter reflects just one command line argument of a certain tool, this
 tag should be set to that particular argument. It is rendered in parenthesis
 after the help section, and it will create the name attribute (if not given explicitly)
 from the argument attribute by stripping leading dashes and replacing all remaining
 dashes by underscores (e.g. if ``argument="--long-parameter"`` then
@@ -3458,15 +3503,15 @@
           <xs:annotation>
             <xs:documentation xml:lang="en">The attribute value will be
 displayed on the tool page as the label of the form field
 (``label=&quot;Sort Query&quot;``).</xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="help" type="xs:string">
-          <xs:annotation gxdocs:best_practices="parameter-help">
+          <xs:annotation>
             <xs:documentation xml:lang="en">Short bit of text, rendered on the
 tool form just below the associated field to provide information about the
 field.</xs:documentation>
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="load_contents" type="xs:integer">
           <xs:annotation>
@@ -3839,16 +3884,16 @@
 Name | Description
 ---- | -----------
 ``$__tool_directory__`` | The directory the tool description (XML file) currently resides in (new in 15.03)
 ``$__new_file_path__`` | ``config/galaxy.ini``'s ``new_file_path`` value
 ``$__tool_data_path__`` | ``config/galaxy.ini``'s tool_data_path value
 ``$__root_dir__`` | Top-level Galaxy source directory made absolute via ``os.path.abspath()``
 ``$__datatypes_config__`` | ``config/galaxy.ini``'s datatypes_config value
-``$__user_id__`` | Email's numeric ID (id column of ``galaxy_user`` table in the database)
-``$__user_email__`` | User's email address
+``$__user_id__`` | Numeric ID of user (id column of ``galaxy_user`` table in the database)
+``$__user_email__`` | Email address of user
 ``$__app__`` | The ``galaxy.app.UniverseApplication`` instance, gives access to all other configuration file variables (e.g. $__app__.config.output_size_limit). Should be used as a last resort, may go away in future releases.
 ``$__target_datatype__`` | Only available in converter tools when run internally by Galaxy. Contains the target datatype of the conversion
 
 
 Additional runtime properties are available as environment variables. Since these
 are not Cheetah variables (the values aren't available until runtime) these should likely
 be escaped with a backslash (``\``) when appearing in ``command`` or ``configfile`` elements.
@@ -3936,14 +3981,23 @@
     <xs:annotation>
       <xs:documentation xml:lang="en"/>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:enumeration value="ecma5.1"/>
     </xs:restriction>
   </xs:simpleType>
+  <xs:simpleType name="RequestMethodType">
+    <xs:annotation>
+      <xs:documentation xml:lang="en">Select a request method, defaults to GET if unspecified</xs:documentation>
+    </xs:annotation>
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="GET"/>
+      <xs:enumeration value="POST"/>
+    </xs:restriction>
+  </xs:simpleType>
   <xs:complexType name="ParamSelectOption">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[
 
 See [/tools/filters/sorter.xml](https://github.com/galaxyproject/galaxy/blob/dev/tools/filters/sorter.xml)
 for typical examples of how to use this tag set. This directive is used to described
 static lists of options and is contained
@@ -4100,34 +4154,36 @@
 Galaxy-aware URI for the default file for collection element.
         ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
   </xs:complexType>
   <xs:complexType name="ParamOptions">
     <xs:annotation>
-      <xs:documentation xml:lang="en"><![CDATA[
+      <xs:documentation xml:lang="en">
+<![CDATA[
 See [/tools/extract/liftOver_wrapper.xml](https://github.com/galaxyproject/galaxy/blob/dev/tools/extract/liftOver_wrapper.xml)
 for an example of how to use this tag set. This tag set is optionally contained
 within the ``<param>`` tag when the ``type`` attribute value is ``select`` or
 ``data`` and used to dynamically generated lists of options.
 
 For data parameters this tag can be used to restrict possible input datasets to datasets that match the ``dbkey`` of another data input by including a ``data_meta`` filter. See for
 instance here: [/tools/maf/interval2maf.xml](https://github.com/galaxyproject/galaxy/blob/dev/tools/maf/interval2maf.xml)
 
 For select parameters this tag set dynamically creates a list of options whose
-values can be obtained from a predefined file stored locally or a dataset
-selected from the current history.
+values can be obtained from a predefined file stored locally, a dataset
+selected from the current history or data fetched from a URL.
 
 There are at least five basic ways to use this tag - four of these correspond to
 a ``from_XXX`` attribute on the ``options`` directive and the other is to
 exclusively use ``filter``s to populate options.
 
 * ``from_data_table`` - The options for the select list are dynamically obtained
   from a file specified in the Galaxy configuration file
   ``tool_data_table_conf.xml`` or from a Tool Shed installed data manager.
+* `from_url` - Fetches a list of available options from a remote server.
 * ``from_dataset`` - The options for the select list are dynamically obtained
   from input dataset selected for the tool from the current history.
 * ``from_file`` - The options for the select list are dynamically obtained from
   a file. This mechanism is discouraged in favor of the more generic
   ``from_data_table``.
 * ``from_parameter`` - The options for the select list are dynamically obtained
   from a parameter.
@@ -4233,14 +4289,70 @@
 <param name="species1" type="select" label="When Species" multiple="false">
     <options>
         <filter type="data_meta" ref="input1" key="species" />
     </options>
 </param>
 ```
 
+### ``from_url``
+
+The following example demonstrates getting options from a third-party server
+with server side requests.
+
+```xml
+<param name="url_param_value" type="select">
+    <options from_url="https://usegalaxy.org/api/genomes">
+    </options>
+</param>
+```
+
+Here a GET request is made to [https://usegalaxy.org/api/genomes](https://usegalaxy.org/api/genomes), which returns
+an array of arrays, such as
+
+```json
+[
+    ["unspecified (?)", "?"],
+    ["A. ceylanicum Mar. 2014 (WS243/Acey_2013.11.30.genDNA/ancCey1) (ancCey1)", "ancCey1"],
+    ...
+]
+```
+Each inner array is a user-selectable option, where the first item in the inner array
+is the `name` of the option (as shown in the select field in the user interface), and
+the second option is the `value` that is passed on to the tool. An optional third
+element can be added to the inner array which corresponds to the `selected` state.
+If the third item is `true` then this particular option is pre-selected.
+
+A more complicated example is shown below, where a POST request is made with a templated
+request header and body. The upstream response is then also transformed using an ecma 5.1
+expression:
+
+```xml
+<param name="url_param_value_header_and_body" type="select">
+    <options from_url="https://postman-echo.com/post" request_method="POST">
+        <!-- Example for accessing user secrets via extra preferences -->
+        <request_headers type="json">
+            {"x-api-key": "${__user__.extra_preferences.fake_api_key if $__user__ else "anon"}"}
+        </request_headers>
+        <request_body type="json">
+            {"name": "value"}
+        </request_body>
+        <!-- https://postman-echo.com/post echos values sent to it, so here we list the response headers -->
+        <postprocess_expression type="ecma5.1"><![CDATA[${
+            return Object.keys(inputs.headers).map((header) => [header, header])
+        }]]]]><![CDATA[></postprocess_expression>
+    </options>
+</param>
+```
+
+The header and body templating mechanism can be used to access protected resources,
+and the `postprocess_expression` can be used to transform arbitrary JSON responses
+to arrays of `name` and `value`, or arrays of `name`, `value` and `selected`.
+
+For an example tool see [select_from_url.xml](https://github.com/galaxyproject/galaxy/tree/dev/test/functional/tools/select_from_url.xml).
+
 ### ``from_file``
 
 The following example is for Blast databases. In this example users maybe select
 a database that is pre-formatted and cached in Galaxy clusters. When a new
 dataset is available, admins must add the database to the local file named
 "blastdb.loc". All such databases in that file are included in the options of
 the select list. For a local instance, the file (e.g. ``blastdb.loc`` or
@@ -4269,15 +4381,15 @@
 wrappers for an example of these.
 
 ### Other Ways to Dynamically Generate Options
 
 Though deprecated and discouraged, [code](#tool-code) blocks can also be
 used to generate dynamic options.
 
-]]></xs:documentation>
+]]>      </xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:group ref="OptionsElement" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
     <xs:attribute name="from_dataset" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">Determine options from (the first MB of) the dataset given in the referred input parameter. If 'meta_file_key' is given, the options are determined from (the first MB of) the data in the metadata file of the input.</xs:documentation>
@@ -4289,14 +4401,24 @@
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="from_data_table" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">Determine options from a data table.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
+    <xs:attribute name="from_url" type="xs:string">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">Determine options from data hosted at specified URL.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
+    <xs:attribute name="request_method" type="RequestMethodType">
+      <xs:annotation>
+        <xs:documentation xml:lang="en">Set the request method to use for options provided using 'from_url'.</xs:documentation>
+      </xs:annotation>
+    </xs:attribute>
     <xs:attribute name="from_parameter" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">Deprecated.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="options_filter_attribute" type="xs:string">
       <xs:annotation>
@@ -4325,22 +4447,39 @@
     </xs:attribute>
   </xs:complexType>
   <xs:group name="OptionsElement">
     <xs:choice>
       <xs:element name="filter" type="Filter" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="column" type="Column" minOccurs="0" maxOccurs="unbounded"/>
       <xs:element name="validator" type="Validator" minOccurs="0" maxOccurs="1"/>
+      <xs:element name="postprocess_expression" type="Expression" minOccurs="0" maxOccurs="1"/>
+      <xs:element name="request_body" type="RequestBody" minOccurs="0" maxOccurs="1"/>
+      <xs:element name="request_headers" type="RequestHeaders" minOccurs="0" maxOccurs="1"/>
       <xs:element name="file" type="xs:string" minOccurs="0" maxOccurs="unbounded">
         <xs:annotation>
           <xs:documentation xml:lang="en">Documentation for file</xs:documentation>
         </xs:annotation>
       </xs:element>
       <xs:element name="option" type="ParamDrillDownOption" minOccurs="0" maxOccurs="unbounded"/>
     </xs:choice>
   </xs:group>
+  <xs:complexType name="RequestBody">
+    <xs:simpleContent>
+      <xs:extension base="xs:string">
+        <xs:attribute name="type" type="xs:string"/>
+      </xs:extension>
+    </xs:simpleContent>
+  </xs:complexType>
+  <xs:complexType name="RequestHeaders">
+    <xs:simpleContent>
+      <xs:extension base="xs:string">
+        <xs:attribute name="type" type="xs:string"/>
+      </xs:extension>
+    </xs:simpleContent>
+  </xs:complexType>
   <xs:complexType name="Column">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[Optionally contained within an
 ``<options>`` tag set - specifies columns used in building select options from a
 file stored locally (i.e. index or tool data) or a dataset in the
 current history.
 
@@ -5280,19 +5419,33 @@
     </xs:sequence>
     <!-- TODO: add a unique constraint for action. -->
     <xs:attributeGroup ref="OutputCommon"/>
     <xs:attributeGroup ref="OutputDataAttributes"/>
   </xs:complexType>
   <xs:group name="OutputCollectionElement">
     <xs:choice>
-      <xs:element name="data" type="OutputData"/>
+      <xs:element name="data" type="OutputCollectionDataElement"/>
       <xs:element name="discover_datasets" type="OutputCollectionDiscoverDatasets"/>
       <xs:element name="filter" type="OutputFilter"/>
     </xs:choice>
   </xs:group>
+  <xs:complexType name="OutputCollectionDataElement">
+    <xs:annotation>
+      <xs:documentation xml:lang="en"><![CDATA[
+
+This tag set is contained within the ``<collection>`` tag set, and can be used to
+define the elements of a collection statically. See also [Planemo's documentation](https://planemo.readthedocs.io/en/latest/writing_advanced.html#static-element-count).
+]]></xs:documentation>
+    </xs:annotation>
+    <xs:sequence>
+      <xs:group ref="OutputCollectionElement" minOccurs="0" maxOccurs="unbounded"/>
+    </xs:sequence>
+    <xs:attributeGroup ref="OutputCommon"/>
+    <xs:attributeGroup ref="OutputDataAttributes"/>
+  </xs:complexType>
   <xs:complexType name="OutputCollection">
     <xs:annotation>
       <xs:documentation xml:lang="en"><![CDATA[
 
 This tag set is contained within the ``<outputs>`` tag set, and it defines the
 output dataset collection description resulting from the tool's execution. The
 value of the attribute ``label`` can be acquired from input parameters or
@@ -5331,15 +5484,14 @@
       <xs:documentation xml:lang="en"><![CDATA[
 
 This tag describes an output to the tool.
 ]]></xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:group ref="OutputDataElement" minOccurs="0" maxOccurs="unbounded"/>
-      <xs:group ref="OutputCollectionElement" minOccurs="0" maxOccurs="unbounded"/>
     </xs:sequence>
     <xs:attributeGroup ref="OutputCommon"/>
     <xs:attributeGroup ref="OutputCollectionAttributes"/>
     <xs:attribute name="type" type="xs:string">
       <xs:annotation>
         <xs:documentation xml:lang="en">Output type. This could be older more established Galaxy types (e.g. data and collection) - in which case the semantics of this largely reflect the corresponding ``data`` and ``collection`` tags. This could also be newer non-data types such as ``integer`` or ``boolean``.</xs:documentation>
       </xs:annotation>
@@ -5488,15 +5640,20 @@
     <xs:attribute name="ext" type="xs:string" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Format (or datatype) of discovered datasets (an alias with ``format``).</xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="sort_by" type="xs:string" use="optional">
       <xs:annotation>
-        <xs:documentation xml:lang="en">A string `[reverse_][SORT_COMP_]SORTBY` describing the desired sort order of the collection elements. `SORTBY` can be `filename`, `name`, `designation`, `dbkey` and the optional `SORT_COMP` can be either `lexical` or `numeric`. Default is lexical sorting by filename.</xs:documentation>
+        <xs:documentation xml:lang="en"><![CDATA[
+        A string `[reverse_][SORT_COMP_]SORTBY` describing the desired sort order of the collection elements.
+        `SORTBY` can be `filename`, `name`, `designation`, `dbkey` and the optional `SORT_COMP` can be either
+        `lexical` or `numeric`. Default is lexical sorting by filename. 
+        Note that lexical sorting is case sensitive, i.e. upper case characters come before lower case characters (e.g. "Apple" < "Banana" < "apple" < "banana").
+        ]]></xs:documentation>
       </xs:annotation>
     </xs:attribute>
     <xs:attribute name="visible" type="xs:boolean" use="optional">
       <xs:annotation>
         <xs:documentation xml:lang="en">Indication if this dataset is visible in output history. This defaults to ``false``, but probably shouldn't - be sure to set to ``true`` if that is your intention.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
@@ -6260,17 +6417,20 @@
 ```
 
 A contrived example of a tool that uses this is the test tool
 [inputs_as_json.xml](https://github.com/galaxyproject/galaxy/blob/dev/test/functional/tools/inputs_as_json.xml).
 
 By default this file will not contain paths for data or collection inputs. To include simple
 paths for data or collection inputs set the ``data_style`` attribute to ``paths`` (see [inputs_as_json_with_paths.xml](https://github.com/galaxyproject/galaxy/blob/dev/test/functional/tools/inputs_as_json_with_paths.xml) for an example).
-To include a dictionary with staging paths, paths and metadata files set the ``data_style`` attribute to ``staging_path_and_source_path``.
+To include a dictionary with element identifiers, datatypes, staging paths, paths and metadata files set the ``data_style`` attribute to ``staging_path_and_source_path`` (element identifiers and datatypes are available since 24.0).
 An example tool that uses ``staging_path_and_source_path`` is [inputs_as_json_with_staging_path_and_source_path.xml](https://github.com/galaxyproject/galaxy/blob/dev/test/functional/tools/inputs_as_json_with_staging_path_and_source_path.xml)
 
+Note that the element identifiers are stored as lists, where the last element is the actual element identifier of the dataset
+and the other elements the identifiers of the collections containing the dataset.
+
 For tools with profile >= 20.05 a select with ``multiple="true"`` is rendered as an array which is empty if nothing is selected. For older profile versions select lists are rendered as comma separated strings or a literal ``null`` in case nothing is selected.
 ]]></xs:documentation>
     </xs:annotation>
     <xs:simpleContent>
       <xs:extension base="xs:string">
         <xs:attribute name="name" type="xs:string">
           <xs:annotation>
@@ -6281,17 +6441,17 @@
           </xs:annotation>
         </xs:attribute>
         <xs:attribute name="filename" type="xs:string">
           <xs:annotation>
             <xs:documentation xml:lang="en">Path relative to the working directory of the tool for the inputs JSON file created in response to this directive.</xs:documentation>
           </xs:annotation>
         </xs:attribute>
-        <xs:attribute name="data_style" type="xs:string">
+        <xs:attribute name="data_style" type="InputsConfigfileDatastyleType">
           <xs:annotation>
-            <xs:documentation xml:lang="en">Set to 'paths' to include dataset paths in the resulting file. Set to 'staging_path_and_source_path' to include a staging path, a source path and all metadata files.</xs:documentation>
+            <xs:documentation xml:lang="en">Set to 'paths' to include dataset paths in the resulting file. Set to 'staging_path_and_source_path' to include element identifiers, datatype, staging path, a source path and all metadata files.</xs:documentation>
           </xs:annotation>
         </xs:attribute>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <xs:complexType name="ConfigFileSources">
     <xs:annotation>
@@ -6359,15 +6519,15 @@
           </xs:annotation>
         </xs:attribute>
       </xs:extension>
     </xs:simpleContent>
   </xs:complexType>
   <xs:complexType name="RequestParameterTranslation">
     <xs:annotation>
-      <xs:documentation xml:lang="en"><![CDATA[See [/tools/data_source/ucsc_tablebrowser.xml](https://github.com/galaxyproject/galaxy/blob/dev/tools/data_source/ucsc_tablebrowser.xml) for an example of how to use this tag set. This tag set is used only in "data_source" tools (i.e. whose ``tool_type`` attribute is ``data_source``). This tag set contains a set of [request_param](#tool-request-param-translation-request-param) elements.]]></xs:documentation>
+      <xs:documentation xml:lang="en"><![CDATA[See [/tools/data_source/ucsc_tablebrowser.xml](https://github.com/galaxyproject/galaxy/blob/dev/tools/data_source/ucsc_tablebrowser.xml) for an example of how to use this tag set. This tag set is used only in "data_source" tools (i.e. whose ``tool_type`` attribute is ``data_source`` or ``data_source_async``). This tag set contains a set of [request_param](#tool-request-param-translation-request-param) elements.]]></xs:documentation>
     </xs:annotation>
     <xs:sequence>
       <xs:element name="request_param" minOccurs="0" maxOccurs="unbounded" type="RequestParameter"/>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="RequestParameter">
     <xs:annotation>
@@ -6398,14 +6558,15 @@
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:enumeration value="URL"/>
       <xs:enumeration value="URL_method"/>
       <xs:enumeration value="dbkey"/>
       <xs:enumeration value="organism"/>
       <xs:enumeration value="table"/>
+      <xs:enumeration value="position"/>
       <xs:enumeration value="description"/>
       <xs:enumeration value="name"/>
       <xs:enumeration value="info"/>
       <xs:enumeration value="data_type"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:group name="RequestParameterElement">
@@ -6696,14 +6857,35 @@
 
 Finally, if the tool did not match any of the fatal errors, then the fifth
 regular expression is checked. Since no source is specified, both stdout and
 stderr are checked. If ``Branch A`` is at the beginning of stdout or stderr, then
 a warning will be registered and the source that contained ``Branch A`` will be
 prepended with the warning ``Warning: Branch A was taken in execution``.
 
+Since Galaxy 24.0 groups defined in the regular expression are expanded in the
+description (using the syntax of the [``expand`` function](https://docs.python.org/3/library/re.html#re.Match.expand)).
+For the first ``regex`` in the following example the ``\1`` will be replaced
+by the content of the text matching ``.*`` that follows on ``INFO: ``,
+i.e. the content of the first group.
+The second regular expression defines a named group ``error_message``
+which then replaces the corresponding placeholder ``\g<error_message>`` in the
+description. Note the quoting of the ``<`` and ``>`` characters in XML.
+
+```xml
+<stdio>
+    <regex match="\(INFO\): (.*)"
+           source="stderr"
+           level="warning"
+           description="\1" />
+    <regex match="\(ERROR|WARNING\): (?P&lt;error_message&gt;.*)"
+           source="stderr"
+           level="fatal"
+           description="\g&lt;error_message&gt;" />
+</stdio>
+```
 ]]></xs:documentation>
     </xs:annotation>
     <xs:attribute name="source" type="SourceType">
       <xs:annotation>
         <xs:documentation xml:lang="en">This tells whether the regular expression should be matched against stdout, stderr, or both. If this attribute is missing or is incorrect, then both stdout and stderr will be checked.</xs:documentation>
       </xs:annotation>
     </xs:attribute>
@@ -6954,14 +7136,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="cuda_device_count_max">
         <xs:annotation>
           <xs:documentation xml:lang="en">Maximum CUDA device count, if runtime allows it (not yet implemented in Galaxy).</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="shm_size">
+        <xs:annotation>
+          <xs:documentation xml:lang="en"><![CDATA[Size of /dev/shm. The format is `<number><unit>`. <number> must be greater than 0. Unit is optional and can be `b` (bytes), `k` (kilobytes), `m` (megabytes), or `g` (gigabytes). If you omit the unit, the default is bytes. If you omit the size entirely, the value is `64m`.]]></xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="ContainerType">
     <xs:annotation>
       <xs:documentation xml:lang="en">Type of container for tool execution.</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
@@ -6971,14 +7158,15 @@
   </xs:simpleType>
   <xs:simpleType name="ToolTypeType">
     <xs:annotation>
       <xs:documentation xml:lang="en">Documentation for ToolTypeType</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:enumeration value="data_source"/>
+      <xs:enumeration value="data_source_async"/>
       <xs:enumeration value="manage_data"/>
       <xs:enumeration value="interactive"/>
       <xs:enumeration value="expression"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="URLmethodType">
     <xs:annotation>
@@ -7141,43 +7329,57 @@
       <xs:enumeration value="both"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="TestOutputCompareType">
     <xs:annotation>
       <xs:documentation xml:lang="en">Type of comparison to use when comparing
 test generated output files to expected output files. Currently valid value are
-``diff`` (the default), ``re_match``, ``re_match_multiline``,
-and ``contains``. In addition there is ``sim_size`` which is discouraged in favour of a ``has_size`` assertion.</xs:documentation>
+``diff`` (the default), ``re_match``, ``re_match_multiline``, ``contains``,
+and ``image_diff``. In addition there is ``sim_size`` which is discouraged in
+favour of a ``has_size`` assertion.</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:enumeration value="diff"/>
       <xs:enumeration value="re_match"/>
       <xs:enumeration value="sim_size"/>
       <xs:enumeration value="re_match_multiline"/>
       <xs:enumeration value="contains"/>
+      <xs:enumeration value="image_diff"/>
+    </xs:restriction>
+  </xs:simpleType>
+  <xs:simpleType name="TestOutputMetricType">
+    <xs:annotation>
+      <xs:documentation xml:lang="en">If ``compare`` is set to ``image_diff``, this is the metric used to compute the distance between images for quantification of their difference. For intensity images, possible metrics are *mean absolute error* (``mae``, the default), *mean squared error* (``mse``), *root mean squared* error (``rms``), and the *Frobenius norm* (``fro``). In addition, for binary images and label maps (with multiple objects), ``iou`` can be used to compute *one minus* the *intersection over the union* (IoU). Object correspondances are established by taking the pair of objects, for which the IoU is highest, and the distance of the images is the worst value determined for any pair of corresponding objects.</xs:documentation>
+    </xs:annotation>
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="mae"/>
+      <xs:enumeration value="mse"/>
+      <xs:enumeration value="rms"/>
+      <xs:enumeration value="fro"/>
+      <xs:enumeration value="iou"/>
     </xs:restriction>
   </xs:simpleType>
   <xs:simpleType name="PermissiveBoolean">
     <xs:annotation>
       <xs:documentation xml:lang="en">Documentation for PermissiveBoolean</xs:documentation>
     </xs:annotation>
     <xs:union>
       <xs:simpleType>
         <xs:restriction base="xs:boolean"/>
       </xs:simpleType>
       <xs:simpleType>
         <xs:restriction base="xs:string">
-          <xs:enumeration value="0"/>
-          <xs:enumeration value="1"/>
           <xs:enumeration value="true"/>
           <xs:enumeration value="false"/>
           <xs:enumeration value="True"/>
           <xs:enumeration value="False"/>
           <xs:enumeration value="yes"/>
           <xs:enumeration value="no"/>
+          <xs:enumeration value="0"/>
+          <xs:enumeration value="1"/>
         </xs:restriction>
       </xs:simpleType>
     </xs:union>
   </xs:simpleType>
   <xs:simpleType name="Bytes">
     <xs:annotation>
       <xs:documentation xml:lang="en">Number of bytes allowing for suffix (k|K|M|G|P|E)i?</xs:documentation>
@@ -7190,15 +7392,15 @@
         <xs:restriction base="xs:string">
           <xs:pattern value="(0|[1-9][0-9]*)([kKMGTPE]i?)?"/>
         </xs:restriction>
       </xs:simpleType>
     </xs:union>
   </xs:simpleType>
   <xs:complexType name="EdamTopics">
-    <xs:annotation>
+    <xs:annotation gxdocs:best_practices="tool-annotations-edam">
       <xs:documentation xml:lang="en"><![CDATA[
 Container tag set for the ``<edam_topic>`` tags.
 A tool can have any number of EDAM topic references.
 
 ```xml
 <!-- Example: this tool is about 'Statistics and probability' (http://edamontology.org/topic_2269) -->
 <edam_topics>
@@ -7214,15 +7416,15 @@
             <xs:pattern value="topic_[0-9]{4}"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:element>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="EdamOperations">
-    <xs:annotation>
+    <xs:annotation gxdocs:best_practices="tool-annotations-edam">
       <xs:documentation xml:lang="en"><![CDATA[
 Container tag set for the ``<edam_operation>`` tags.
 A tool can have any number of EDAM operation references.
 
 ```xml
 <!-- Example: this tool performs a 'Conversion' operation (http://edamontology.org/operation_3434) -->
 <edam_operations>
@@ -7239,15 +7441,15 @@
             <xs:pattern value="operation_[0-9]{4}"/>
           </xs:restriction>
         </xs:simpleType>
       </xs:element>
     </xs:sequence>
   </xs:complexType>
   <xs:complexType name="xrefs">
-    <xs:annotation>
+    <xs:annotation gxdocs:best_practices="tool-cross-references-bio-tools">
       <xs:documentation xml:lang="en"><![CDATA[
 Container tag set for the ``<xref>`` tags.
 A tool can refer multiple reference IDs.
 
 ```xml
    <!-- Example: this tool is dada2 -->
    <xrefs>
@@ -7314,8 +7516,17 @@
     <xs:annotation>
       <xs:documentation xml:lang="en">Allowed collection types</xs:documentation>
     </xs:annotation>
     <xs:restriction base="xs:string">
       <xs:pattern value="(list|paired)([:,](list|paired))*"/>
     </xs:restriction>
   </xs:simpleType>
+  <xs:simpleType name="InputsConfigfileDatastyleType">
+    <xs:annotation>
+      <xs:documentation xml:lang="en">Allowed collection types</xs:documentation>
+    </xs:annotation>
+    <xs:restriction base="xs:string">
+      <xs:enumeration value="paths"/>
+      <xs:enumeration value="staging_path_and_source_path"/>
+    </xs:restriction>
+  </xs:simpleType>
 </xs:schema>
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/SOURCES.txt` & `galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 galaxy/tool_util/linters/general.py
 galaxy/tool_util/linters/help.py
 galaxy/tool_util/linters/inputs.py
 galaxy/tool_util/linters/outputs.py
 galaxy/tool_util/linters/stdio.py
 galaxy/tool_util/linters/tests.py
 galaxy/tool_util/linters/xml_order.py
+galaxy/tool_util/linters/xsd.py
 galaxy/tool_util/locations/__init__.py
 galaxy/tool_util/locations/dockstore.py
 galaxy/tool_util/locations/file.py
 galaxy/tool_util/locations/http.py
 galaxy/tool_util/ontologies/__init__.py
 galaxy/tool_util/ontologies/biotools_mappings.tsv
 galaxy/tool_util/ontologies/edam_operation_mappings.tsv
```

### Comparing `galaxy-tool-util-23.2.dev0/galaxy_tool_util.egg-info/entry_points.txt` & `galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-23.2.dev0/setup.cfg` & `galaxy-tool-util-24.0.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy tool and tool dependency utilities
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tool-util
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.dev0
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util>=22.1
 	conda-package-streaming
-	lxml
+	lxml!=4.2.2
 	MarkupSafe
 	packaging
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	PyYAML
 	requests
 	sortedcontainers
 	typing-extensions
 packages = find:
 python_requires = >=3.7
 
@@ -55,20 +56,24 @@
 	mulled-hash = galaxy.tool_util.deps.mulled.mulled_hash:main
 	mulled-list = galaxy.tool_util.deps.mulled.mulled_list:main
 	mulled-search = galaxy.tool_util.deps.mulled.mulled_search:main
 	mulled-update-singularity-containers = galaxy.tool_util.deps.mulled.mulled_update_singularity_containers:main
 
 [options.extras_require]
 cwl = 
-	cwltool==3.1.20221109155812
+	cwltool>=3.1.20230624081518
 mulled = 
 	jinja2
 	Whoosh
 edam = 
 	edam-ontology
+extended-assertions = 
+	numpy
+	pysam
+	pillow
 
 [options.packages.find]
 exclude = 
 	tests*
 
 [egg_info]
 tag_build =
```

