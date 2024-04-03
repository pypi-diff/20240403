# Comparing `tmp/curies-0.7.8.tar.gz` & `tmp/curies-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curies-0.7.8.tar", last modified: Wed Mar 13 14:01:47 2024, max compression
+gzip compressed data, was "curies-0.7.9.tar", last modified: Wed Apr  3 08:07:41 2024, max compression
```

## Comparing `curies-0.7.8.tar` & `curies-0.7.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.230106 curies-0.7.8/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-08-12 11:39:10.000000 curies-0.7.8/LICENSE
--rw-r--r--   0 cthoyt     (501) staff       (20)      430 2023-11-01 18:28:25.000000 curies-0.7.8/MANIFEST.in
--rw-r--r--   0 cthoyt     (501) staff       (20)     9265 2024-03-13 14:01:47.230032 curies-0.7.8/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     7079 2024-02-04 10:52:36.000000 curies-0.7.8/README.md
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.208536 curies-0.7.8/docs/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.212058 curies-0.7.8/docs/source/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.220500 curies-0.7.8/docs/source/api/
--rw-r--r--   0 cthoyt     (501) staff       (20)     2844 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.Converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      101 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.DuplicatePrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      110 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.DuplicateURIPrefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      107 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.DuplicateValueError.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      648 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.Record.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      658 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.Reference.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      545 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.ReferenceTuple.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       64 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.chain.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.discover.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.discover_from_rdf.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_bioregistry_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_go_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_monarch_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_obo_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_prefixcommons_converter.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.get_version.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      121 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.load_extended_prefix_map.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.load_jsonld_context.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       94 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.load_prefix_map.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       79 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.load_shacl.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      296 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      332 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      134 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      119 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      128 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.remap_curie_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.remap_uri_prefixes.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      111 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.resolver_service.get_fastapi_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      120 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.resolver_service.get_fastapi_router.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      105 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.resolver_service.get_flask_app.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      123 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.resolver_service.get_flask_blueprint.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       67 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.rewire.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.upgrade_prefix_map.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.write_extended_prefix_map.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.write_jsonld_context.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.write_shacl.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       76 2024-03-13 13:42:14.000000 curies-0.7.8/docs/source/api/curies.write_tsv.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)       95 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/api.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     7498 2024-03-13 14:01:46.000000 curies-0.7.8/docs/source/conf.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13858 2023-11-28 16:44:19.000000 curies-0.7.8/docs/source/discovery.rst
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.220994 curies-0.7.8/docs/source/img/
--rw-r--r--   0 cthoyt     (501) staff       (20)   159090 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/img/trie.png
--rw-r--r--   0 cthoyt     (501) staff       (20)     2610 2024-03-13 11:55:13.000000 curies-0.7.8/docs/source/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)    10668 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/reconciliation.rst
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.222057 curies-0.7.8/docs/source/services/
--rw-r--r--   0 cthoyt     (501) staff       (20)      138 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/services/index.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      137 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/services/mapping_service.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      118 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/services/resolver_service.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)     5380 2024-01-16 09:52:36.000000 curies-0.7.8/docs/source/struct.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)    98117 2023-11-01 18:28:25.000000 curies-0.7.8/docs/source/syntax_demo.svg
--rw-r--r--   0 cthoyt     (501) staff       (20)    32683 2024-03-13 13:46:37.000000 curies-0.7.8/docs/source/tutorial.rst
--rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-11-01 18:28:25.000000 curies-0.7.8/pyproject.toml
--rw-r--r--   0 cthoyt     (501) staff       (20)     2513 2024-03-13 14:01:47.230639 curies-0.7.8/setup.cfg
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.208958 curies-0.7.8/src/
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.224950 curies-0.7.8/src/curies/
--rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2024-03-13 13:38:18.000000 curies-0.7.8/src/curies/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-08-12 11:39:10.000000 curies-0.7.8/src/curies/__main__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      625 2024-02-04 10:40:09.000000 curies-0.7.8/src/curies/_pydantic_compat.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    94560 2024-03-13 13:45:23.000000 curies-0.7.8/src/curies/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5112 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/cli.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    11408 2023-11-28 16:44:19.000000 curies-0.7.8/src/curies/discovery.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.226566 curies-0.7.8/src/curies/mapping_service/
--rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/mapping_service/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/mapping_service/api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/mapping_service/rdflib_custom.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     4797 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/mapping_service/utils.py
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-12 11:39:10.000000 curies-0.7.8/src/curies/py.typed
--rw-r--r--   0 cthoyt     (501) staff       (20)     9621 2023-11-22 23:07:21.000000 curies-0.7.8/src/curies/reconciliation.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     9669 2023-11-01 18:28:25.000000 curies-0.7.8/src/curies/resolver_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5083 2024-01-16 09:52:36.000000 curies-0.7.8/src/curies/sources.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      233 2024-03-13 14:01:46.000000 curies-0.7.8/src/curies/version.py
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.229278 curies-0.7.8/src/curies.egg-info/
--rw-r--r--   0 cthoyt     (501) staff       (20)     9265 2024-03-13 14:01:47.000000 curies-0.7.8/src/curies.egg-info/PKG-INFO
--rw-r--r--   0 cthoyt     (501) staff       (20)     3087 2024-03-13 14:01:47.000000 curies-0.7.8/src/curies.egg-info/SOURCES.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-03-13 14:01:47.000000 curies-0.7.8/src/curies.egg-info/dependency_links.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-09-07 14:58:40.000000 curies-0.7.8/src/curies.egg-info/not-zip-safe
--rw-r--r--   0 cthoyt     (501) staff       (20)      221 2024-03-13 14:01:47.000000 curies-0.7.8/src/curies.egg-info/requires.txt
--rw-r--r--   0 cthoyt     (501) staff       (20)        7 2024-03-13 14:01:47.000000 curies-0.7.8/src/curies.egg-info/top_level.txt
-drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-03-13 14:01:47.229041 curies-0.7.8/tests/
--rw-r--r--   0 cthoyt     (501) staff       (20)       56 2023-08-12 11:39:10.000000 curies-0.7.8/tests/__init__.py
--rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-12 07:07:17.000000 curies-0.7.8/tests/constants.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    37095 2024-03-13 11:55:13.000000 curies-0.7.8/tests/test_api.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3052 2023-11-28 16:44:19.000000 curies-0.7.8/tests/test_discovery.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-11-01 18:28:25.000000 curies-0.7.8/tests/test_federated_sparql.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3788 2023-11-01 18:44:30.000000 curies-0.7.8/tests/test_io.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    13569 2023-11-01 18:28:25.000000 curies-0.7.8/tests/test_mapping_service.py
--rw-r--r--   0 cthoyt     (501) staff       (20)    14719 2023-11-28 16:44:19.000000 curies-0.7.8/tests/test_reconciliation.py
--rw-r--r--   0 cthoyt     (501) staff       (20)     3286 2023-11-01 18:28:25.000000 curies-0.7.8/tests/test_resolver_service.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.358856 curies-0.7.9/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1076 2023-08-12 11:39:10.000000 curies-0.7.9/LICENSE
+-rw-r--r--   0 cthoyt     (501) staff       (20)      430 2023-11-01 18:28:25.000000 curies-0.7.9/MANIFEST.in
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9265 2024-04-03 08:07:41.358776 curies-0.7.9/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7079 2024-02-04 10:52:36.000000 curies-0.7.9/README.md
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.346535 curies-0.7.9/docs/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.349197 curies-0.7.9/docs/source/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.353429 curies-0.7.9/docs/source/api/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2844 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.Converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      101 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.DuplicatePrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      110 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.DuplicateURIPrefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      107 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.DuplicateValueError.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      648 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.Record.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      658 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.Reference.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      545 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.ReferenceTuple.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       64 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.chain.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       73 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.discover.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.discover_from_rdf.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_bioregistry_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       97 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_go_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      112 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_monarch_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      100 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_obo_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_prefixcommons_converter.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.get_version.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      121 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.load_extended_prefix_map.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      106 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.load_jsonld_context.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       94 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.load_prefix_map.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       79 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.load_shacl.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      296 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.MappingServiceGraph.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      332 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.MappingServiceSPARQLProcessor.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      134 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.get_fastapi_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      119 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      128 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.get_flask_mapping_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.mapping_service.get_flask_mapping_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.remap_curie_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.remap_uri_prefixes.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      111 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.resolver_service.get_fastapi_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      120 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.resolver_service.get_fastapi_router.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      105 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.resolver_service.get_flask_app.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      123 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.resolver_service.get_flask_blueprint.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       67 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.rewire.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      103 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.upgrade_prefix_map.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      124 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.write_extended_prefix_map.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      109 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.write_jsonld_context.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       82 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.write_shacl.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       76 2024-03-13 13:42:14.000000 curies-0.7.9/docs/source/api/curies.write_tsv.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)       95 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/api.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     7498 2024-04-03 08:07:40.000000 curies-0.7.9/docs/source/conf.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13858 2023-11-28 16:44:19.000000 curies-0.7.9/docs/source/discovery.rst
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.353524 curies-0.7.9/docs/source/img/
+-rw-r--r--   0 cthoyt     (501) staff       (20)   159090 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/img/trie.png
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2610 2024-03-13 11:55:13.000000 curies-0.7.9/docs/source/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)    10668 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/reconciliation.rst
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.354418 curies-0.7.9/docs/source/services/
+-rw-r--r--   0 cthoyt     (501) staff       (20)      138 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/services/index.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      137 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/services/mapping_service.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      118 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/services/resolver_service.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5380 2024-01-16 09:52:36.000000 curies-0.7.9/docs/source/struct.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)    98117 2023-11-01 18:28:25.000000 curies-0.7.9/docs/source/syntax_demo.svg
+-rw-r--r--   0 cthoyt     (501) staff       (20)    32683 2024-03-13 13:46:37.000000 curies-0.7.9/docs/source/tutorial.rst
+-rw-r--r--   0 cthoyt     (501) staff       (20)      377 2023-11-01 18:28:25.000000 curies-0.7.9/pyproject.toml
+-rw-r--r--   0 cthoyt     (501) staff       (20)     2513 2024-04-03 08:07:41.359338 curies-0.7.9/setup.cfg
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.346865 curies-0.7.9/src/
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.355714 curies-0.7.9/src/curies/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     1503 2024-03-13 13:38:18.000000 curies-0.7.9/src/curies/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      146 2023-08-12 11:39:10.000000 curies-0.7.9/src/curies/__main__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      625 2024-02-04 10:40:09.000000 curies-0.7.9/src/curies/_pydantic_compat.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    94721 2024-04-03 08:07:31.000000 curies-0.7.9/src/curies/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5112 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/cli.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    11408 2023-11-28 16:44:19.000000 curies-0.7.9/src/curies/discovery.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.356696 curies-0.7.9/src/curies/mapping_service/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4478 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/mapping_service/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     8224 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/mapping_service/api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3343 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/mapping_service/rdflib_custom.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     4797 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/mapping_service/utils.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-08-12 11:39:10.000000 curies-0.7.9/src/curies/py.typed
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9621 2023-11-22 23:07:21.000000 curies-0.7.9/src/curies/reconciliation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9669 2023-11-01 18:28:25.000000 curies-0.7.9/src/curies/resolver_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5083 2024-01-16 09:52:36.000000 curies-0.7.9/src/curies/sources.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      233 2024-04-03 08:07:40.000000 curies-0.7.9/src/curies/version.py
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.358115 curies-0.7.9/src/curies.egg-info/
+-rw-r--r--   0 cthoyt     (501) staff       (20)     9265 2024-04-03 08:07:41.000000 curies-0.7.9/src/curies.egg-info/PKG-INFO
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3087 2024-04-03 08:07:41.000000 curies-0.7.9/src/curies.egg-info/SOURCES.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2024-04-03 08:07:41.000000 curies-0.7.9/src/curies.egg-info/dependency_links.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        1 2023-09-07 14:58:40.000000 curies-0.7.9/src/curies.egg-info/not-zip-safe
+-rw-r--r--   0 cthoyt     (501) staff       (20)      221 2024-04-03 08:07:41.000000 curies-0.7.9/src/curies.egg-info/requires.txt
+-rw-r--r--   0 cthoyt     (501) staff       (20)        7 2024-04-03 08:07:41.000000 curies-0.7.9/src/curies.egg-info/top_level.txt
+drwxr-xr-x   0 cthoyt     (501) staff       (20)        0 2024-04-03 08:07:41.357992 curies-0.7.9/tests/
+-rw-r--r--   0 cthoyt     (501) staff       (20)       56 2023-08-12 11:39:10.000000 curies-0.7.9/tests/__init__.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)      130 2024-03-12 07:07:17.000000 curies-0.7.9/tests/constants.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    37095 2024-03-13 11:55:13.000000 curies-0.7.9/tests/test_api.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3052 2023-11-28 16:44:19.000000 curies-0.7.9/tests/test_discovery.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     5198 2023-11-01 18:28:25.000000 curies-0.7.9/tests/test_federated_sparql.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3788 2023-11-01 18:44:30.000000 curies-0.7.9/tests/test_io.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    13569 2023-11-01 18:28:25.000000 curies-0.7.9/tests/test_mapping_service.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)    14719 2023-11-28 16:44:19.000000 curies-0.7.9/tests/test_reconciliation.py
+-rw-r--r--   0 cthoyt     (501) staff       (20)     3286 2023-11-01 18:28:25.000000 curies-0.7.9/tests/test_resolver_service.py
```

### Comparing `curies-0.7.8/LICENSE` & `curies-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/PKG-INFO` & `curies-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.7.8
+Version: 0.7.9
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.7.8 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.7.9 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies,IRIs
```

### Comparing `curies-0.7.8/README.md` & `curies-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/api/curies.Converter.rst` & `curies-0.7.9/docs/source/api/curies.Converter.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/api/curies.Record.rst` & `curies-0.7.9/docs/source/api/curies.Record.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/api/curies.Reference.rst` & `curies-0.7.9/docs/source/api/curies.Reference.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/api/curies.ReferenceTuple.rst` & `curies-0.7.9/docs/source/api/curies.ReferenceTuple.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/conf.py` & `curies-0.7.9/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "curies"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.7.8"
+release = "0.7.9"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `curies-0.7.8/docs/source/discovery.rst` & `curies-0.7.9/docs/source/discovery.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/img/trie.png` & `curies-0.7.9/docs/source/img/trie.png`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/index.rst` & `curies-0.7.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/reconciliation.rst` & `curies-0.7.9/docs/source/reconciliation.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/struct.rst` & `curies-0.7.9/docs/source/struct.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/syntax_demo.svg` & `curies-0.7.9/docs/source/syntax_demo.svg`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/docs/source/tutorial.rst` & `curies-0.7.9/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/setup.cfg` & `curies-0.7.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = curies
-version = 0.7.8
+version = 0.7.9
 description = Idiomatic conversion between URIs and compact URIs (CURIEs).
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cthoyt/curies
 download_url = https://github.com/cthoyt/curies/releases
 project_urls = 
 	Bug Tracker = https://github.com/cthoyt/curies/issues
```

### Comparing `curies-0.7.8/src/curies/__init__.py` & `curies-0.7.9/src/curies/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/_pydantic_compat.py` & `curies-0.7.9/src/curies/_pydantic_compat.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/api.py` & `curies-0.7.9/src/curies/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,18 @@
     overload,
 )
 
 import requests
 from pydantic import BaseModel, Field
 from pytrie import StringTrie
 
-from ._pydantic_compat import field_validator, get_field_validator_values
+from ._pydantic_compat import PYDANTIC_V1, field_validator, get_field_validator_values
+
+if not PYDANTIC_V1:
+    from pydantic import ConfigDict
 
 if TYPE_CHECKING:  # pragma: no cover
     import pandas
     import rdflib
 
 __all__ = [
     "Converter",
@@ -197,18 +200,23 @@
         ...,
         description="The prefix used in a compact URI (CURIE).",
     )
     identifier: str = Field(
         ..., description="The local unique identifier used in a compact URI (CURIE)."
     )
 
-    class Config:
-        """Pydantic configuration for references."""
+    if PYDANTIC_V1:
+
+        class Config:
+            """Pydantic configuration for references."""
+
+            frozen = True
 
-        frozen = True
+    else:
+        model_config = ConfigDict(frozen=True)
 
     @property
     def curie(self) -> str:
         """Get the reference as a CURIE string.
 
         :return:
             A string representation of a compact URI (CURIE).
```

### Comparing `curies-0.7.8/src/curies/cli.py` & `curies-0.7.9/src/curies/cli.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/discovery.py` & `curies-0.7.9/src/curies/discovery.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/mapping_service/__init__.py` & `curies-0.7.9/src/curies/mapping_service/__init__.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/mapping_service/api.py` & `curies-0.7.9/src/curies/mapping_service/api.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/mapping_service/rdflib_custom.py` & `curies-0.7.9/src/curies/mapping_service/rdflib_custom.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/mapping_service/utils.py` & `curies-0.7.9/src/curies/mapping_service/utils.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/reconciliation.py` & `curies-0.7.9/src/curies/reconciliation.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/resolver_service.py` & `curies-0.7.9/src/curies/resolver_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies/sources.py` & `curies-0.7.9/src/curies/sources.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/src/curies.egg-info/PKG-INFO` & `curies-0.7.9/src/curies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curies
-Version: 0.7.8
+Version: 0.7.9
 Summary: Idiomatic conversion between URIs and compact URIs (CURIEs).
 Home-page: https://github.com/cthoyt/curies
 Download-URL: https://github.com/cthoyt/curies/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curies Version: 0.7.8 Summary: Idiomatic conversion
+Metadata-Version: 2.1 Name: curies Version: 0.7.9 Summary: Idiomatic conversion
 between URIs and compact URIs (CURIEs). Home-page: https://github.com/cthoyt/
 curies Download-URL: https://github.com/cthoyt/curies/releases Author: Charles
 Tapley Hoyt Author-email: cthoyt@gmail.com Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com License: MIT Project-URL: Bug Tracker,
 https://github.com/cthoyt/curies/issues Project-URL: Source Code, https://
 github.com/cthoyt/curies Keywords: snekpack,cookiecutter,semantic web,compact
 uniform resource identifiers,uniform resource identifiers,curies,IRIs
```

### Comparing `curies-0.7.8/src/curies.egg-info/SOURCES.txt` & `curies-0.7.9/src/curies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_api.py` & `curies-0.7.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_discovery.py` & `curies-0.7.9/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_federated_sparql.py` & `curies-0.7.9/tests/test_federated_sparql.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_io.py` & `curies-0.7.9/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_mapping_service.py` & `curies-0.7.9/tests/test_mapping_service.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_reconciliation.py` & `curies-0.7.9/tests/test_reconciliation.py`

 * *Files identical despite different names*

### Comparing `curies-0.7.8/tests/test_resolver_service.py` & `curies-0.7.9/tests/test_resolver_service.py`

 * *Files identical despite different names*

