# Comparing `tmp/cognite_neat-0.68.8.tar.gz` & `tmp/cognite_neat-0.68.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_neat-0.68.8.tar", max compression
+gzip compressed data, was "cognite_neat-0.68.9.tar", max compression
```

## Comparing `cognite_neat-0.68.8.tar` & `cognite_neat-0.68.9.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0    11351 2024-03-25 17:07:56.723192 cognite_neat-0.68.8/LICENSE
--rw-r--r--   0        0        0     6775 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/README.md
--rw-r--r--   0        0        0       61 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/__init__.py
--rw-r--r--   0        0        0       23 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/_version.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/__init__.py
--rw-r--r--   0        0        0      152 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/asgi/metrics.py
--rw-r--r--   0        0        0     4606 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/configuration.py
--rw-r--r--   0        0        0       90 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/context_manager/__init__.py
--rw-r--r--   0        0        0      380 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/context_manager/manager.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/data_classes/__init__.py
--rw-r--r--   0        0        0     4208 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/data_classes/configuration.py
--rw-r--r--   0        0        0     1675 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/data_classes/rest.py
--rw-r--r--   0        0        0     1855 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/explorer.py
--rw-r--r--   0        0        0      554 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/configuration.py
--rw-r--r--   0        0        0     4646 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/crud.py
--rw-r--r--   0        0        0    13653 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/data_exploration.py
--rw-r--r--   0        0        0      210 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/metrics.py
--rw-r--r--   0        0        0     6369 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/rules.py
--rw-r--r--   0        0        0    11564 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/routers/workflows.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/utils/__init__.py
--rw-r--r--   0        0        0      564 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/utils/data_mapping.py
--rw-r--r--   0        0        0      806 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/utils/logging.py
--rw-r--r--   0        0        0     4594 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/api/utils/query_templates.py
--rw-r--r--   0        0        0      357 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/main.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/monitoring/__init__.py
--rw-r--r--   0        0        0     2690 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/monitoring/metrics.py
--rw-r--r--   0        0        0       16 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/index.html
--rw-r--r--   0        0        0      312 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/.gitignore
--rw-r--r--   0        0        0     3359 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/README.md
--rw-r--r--   0        0        0      464 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/asset-manifest.json
--rw-r--r--   0        0        0     3870 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/favicon.ico
--rw-r--r--   0        0        0      630 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/index.html
--rw-r--r--   0        0        0     5347 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/logo192.png
--rw-r--r--   0        0        0      492 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/manifest.json
--rw-r--r--   0        0        0       67 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/robots.txt
--rw-r--r--   0        0        0     8524 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
--rw-r--r--   0        0        0    13319 2024-03-25 17:07:56.727192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
--rw-r--r--   0        0        0  1403536 2024-03-25 17:07:56.735192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
--rw-r--r--   0        0        0     2667 2024-03-25 17:07:56.735192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
--rw-r--r--   0        0        0  5996918 2024-03-25 17:07:56.755192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
--rw-r--r--   0        0        0     2633 2024-03-25 17:07:56.759192 cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
--rw-r--r--   0        0        0     1503 2024-03-25 17:07:56.763192 cognite_neat-0.68.8/cognite/neat/config.py
--rw-r--r--   0        0        0     1228 2024-03-25 17:07:56.763192 cognite_neat-0.68.8/cognite/neat/constants.py
--rw-r--r--   0        0        0     4268 2024-03-25 17:07:56.763192 cognite_neat-0.68.8/cognite/neat/exceptions.py
--rw-r--r--   0        0        0       73 2024-03-25 17:07:56.763192 cognite_neat-0.68.8/cognite/neat/graph/__init__.py
--rw-r--r--   0        0        0  1439359 2024-03-25 17:07:56.767192 cognite_neat-0.68.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
--rw-r--r--   0        0        0  1437996 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
--rw-r--r--   0        0        0      368 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/examples/__init__.py
--rw-r--r--   0        0        0    45798 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
--rw-r--r--   0        0        0     3402 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/exceptions.py
--rw-r--r--   0        0        0      258 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractor/__init__.py
--rw-r--r--   0        0        0      356 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractor/_base.py
--rw-r--r--   0        0        0    11232 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractor/_dexpi.py
--rw-r--r--   0        0        0    17408 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractor/_graph_capturing_sheet.py
--rw-r--r--   0        0        0    14872 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractor/_mock_graph_generator.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractors/__init__.py
--rw-r--r--   0        0        0      356 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractors/_base.py
--rw-r--r--   0        0        0    14811 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/extractors/_mock_graph_generator.py
--rw-r--r--   0        0        0      693 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/__init__.py
--rw-r--r--   0        0        0    23838 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/_asset_loader.py
--rw-r--r--   0        0        0     2370 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/_base.py
--rw-r--r--   0        0        0     2837 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/_exceptions.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/core/__init__.py
--rw-r--r--   0        0        0     2306 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/core/labels.py
--rw-r--r--   0        0        0     5016 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/core/models.py
--rw-r--r--   0        0        0    40458 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/core/rdf_to_assets.py
--rw-r--r--   0        0        0    22678 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/core/rdf_to_relationships.py
--rw-r--r--   0        0        0    12957 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/rdf_to_dms.py
--rw-r--r--   0        0        0     3327 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/loader/validator.py
--rw-r--r--   0        0        0      149 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/models.py
--rw-r--r--   0        0        0      543 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/__init__.py
--rw-r--r--   0        0        0    14254 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_base.py
--rw-r--r--   0        0        0     1776 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_graphdb_store.py
--rw-r--r--   0        0        0     1420 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_memory_store.py
--rw-r--r--   0        0        0     5377 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_oxigraph_store.py
--rw-r--r--   0        0        0     9569 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_oxrdflib.py
--rw-r--r--   0        0        0     1244 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/stores/_rdf_to_graph.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/transformation/__init__.py
--rw-r--r--   0        0        0     4758 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/transformation/entity_matcher.py
--rw-r--r--   0        0        0       73 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/transformation/query_generator/__init__.py
--rw-r--r--   0        0        0    18659 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/transformation/query_generator/sparql.py
--rw-r--r--   0        0        0    14673 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/graph/transformation/transformer.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/py.typed
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/__init__.py
--rw-r--r--   0        0        0    11635 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/_analysis.py
--rw-r--r--   0        0        0      177 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/_shared.py
--rw-r--r--   0        0        0     8596 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/analysis.py
--rw-r--r--   0        0        0    58987 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
--rw-r--r--   0        0        0    80226 2024-03-25 17:07:56.771192 cognite_neat-0.68.8/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
--rw-r--r--   0        0        0      858 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/__init__.py
--rw-r--r--   0        0        0     2538 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-containers.yaml
--rw-r--r--   0        0        0    77055 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-example.xlsx
--rw-r--r--   0        0        0     5501 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-model.yaml
--rw-r--r--   0        0        0    75865 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/rules-template.xlsx
--rw-r--r--   0        0        0    52433 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
--rw-r--r--   0        0        0    26008 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/skos-rules.xlsx
--rw-r--r--   0        0        0    79981 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
--rw-r--r--   0        0        0    65934 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/examples/wind-energy.owl
--rw-r--r--   0        0        0   123867 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exceptions.py
--rw-r--r--   0        0        0      574 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/__init__.py
--rw-r--r--   0        0        0     1439 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_base.py
--rw-r--r--   0        0        0      102 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_core/__init__.py
--rw-r--r--   0        0        0      764 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_core/rules2labels.py
--rw-r--r--   0        0        0    37099 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2dms.py
--rw-r--r--   0        0        0     8220 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2excel.py
--rw-r--r--   0        0        0     6215 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2graphql.py
--rw-r--r--   0        0        0    18414 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2ontology.py
--rw-r--r--   0        0        0    28745 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2pydantic_models.py
--rw-r--r--   0        0        0     3866 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2rules.py
--rw-r--r--   0        0        0     1104 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2triples.py
--rw-r--r--   0        0        0     5769 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporter/_validation.py
--rw-r--r--   0        0        0      413 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/__init__.py
--rw-r--r--   0        0        0     1472 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_base.py
--rw-r--r--   0        0        0     1645 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_models.py
--rw-r--r--   0        0        0    12394 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2dms.py
--rw-r--r--   0        0        0     8717 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2excel.py
--rw-r--r--   0        0        0    19618 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2ontology.py
--rw-r--r--   0        0        0     4379 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2rules.py
--rw-r--r--   0        0        0     2990 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2yaml.py
--rw-r--r--   0        0        0     4092 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/exporters/_validation.py
--rw-r--r--   0        0        0      636 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/__init__.py
--rw-r--r--   0        0        0     2316 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_base.py
--rw-r--r--   0        0        0     6469 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_dict2rules.py
--rw-r--r--   0        0        0     7890 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_dms2rules.py
--rw-r--r--   0        0        0    12097 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_graph2rules.py
--rw-r--r--   0        0        0     1610 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_json2rules.py
--rw-r--r--   0        0        0       63 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/__init__.py
--rw-r--r--   0        0        0     8304 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     9320 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     8019 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0    10521 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     1529 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_spreadsheet2rules.py
--rw-r--r--   0        0        0      448 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_xsd2rules.py
--rw-r--r--   0        0        0     1628 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importer/_yaml2rules.py
--rw-r--r--   0        0        0      408 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importers/__init__.py
--rw-r--r--   0        0        0     4265 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importers/_base.py
--rw-r--r--   0        0        0     8176 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dms2rules.py
--rw-r--r--   0        0        0       68 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/__init__.py
--rw-r--r--   0        0        0    12134 2024-03-25 17:07:56.775192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
--rw-r--r--   0        0        0    12554 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
--rw-r--r--   0        0        0     6925 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
--rw-r--r--   0        0        0    11926 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/spec.py
--rw-r--r--   0        0        0       63 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/__init__.py
--rw-r--r--   0        0        0     7610 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
--rw-r--r--   0        0        0     7674 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
--rw-r--r--   0        0        0     7304 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
--rw-r--r--   0        0        0     5594 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
--rw-r--r--   0        0        0     7121 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_spreadsheet2rules.py
--rw-r--r--   0        0        0     4198 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/importers/_yaml2rules.py
--rw-r--r--   0        0        0      563 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/__init__.py
--rw-r--r--   0        0        0     5730 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/base.py
--rw-r--r--   0        0        0    10419 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/dms.py
--rw-r--r--   0        0        0     4492 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/fileread.py
--rw-r--r--   0        0        0     3346 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/formatters.py
--rw-r--r--   0        0        0     6916 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/importing.py
--rw-r--r--   0        0        0    13763 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/spreadsheet.py
--rw-r--r--   0        0        0     3179 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/issues/spreadsheet_file.py
--rw-r--r--   0        0        0      127 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/__init__.py
--rw-r--r--   0        0        0     4989 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_base.py
--rw-r--r--   0        0        0      517 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/__init__.py
--rw-r--r--   0        0        0     1227 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/__init__.py
--rw-r--r--   0        0        0    13343 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_base.py
--rw-r--r--   0        0        0     9677 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_field.py
--rw-r--r--   0        0        0     5207 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_value.py
--rw-r--r--   0        0        0    10038 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/base.py
--rw-r--r--   0        0        0    46388 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/dms_architect_rules.py
--rw-r--r--   0        0        0    16197 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/dms_schema.py
--rw-r--r--   0        0        0     1878 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/domain_rules.py
--rw-r--r--   0        0        0    18914 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/_rules/information_rules.py
--rw-r--r--   0        0        0    12368 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/raw_rules.py
--rw-r--r--   0        0        0     7228 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/rdfpath.py
--rw-r--r--   0        0        0    51063 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/rules.py
--rw-r--r--   0        0        0      171 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/tables.py
--rw-r--r--   0        0        0     4316 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/rules/models/value_types.py
--rw-r--r--   0        0        0       68 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/__init__.py
--rw-r--r--   0        0        0      309 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/auxiliary.py
--rw-r--r--   0        0        0      711 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf.py
--rw-r--r--   0        0        0      483 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/__init__.py
--rw-r--r--   0        0        0     2057 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_base.py
--rw-r--r--   0        0        0     9719 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_data_modeling.py
--rw-r--r--   0        0        0     6319 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_ingestion.py
--rw-r--r--   0        0        0     3759 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/data_classes.py
--rw-r--r--   0        0        0      981 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/exceptions.py
--rw-r--r--   0        0        0     2453 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/spreadsheet.py
--rw-r--r--   0        0        0     3082 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/text.py
--rw-r--r--   0        0        0    12826 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/utils.py
--rw-r--r--   0        0        0      992 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/utils/xml.py
--rw-r--r--   0        0        0      396 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/__init__.py
--rw-r--r--   0        0        0     1348 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/_exceptions.py
--rw-r--r--   0        0        0    26223 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/base.py
--rw-r--r--   0        0        0    18016 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/cdf_store.py
--rw-r--r--   0        0        0     1987 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Export DMS/workflow.yaml
--rw-r--r--   0        0        0     3604 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
--rw-r--r--   0        0        0     3384 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
--rw-r--r--   0        0        0     6205 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
--rw-r--r--   0        0        0     1364 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Import DMS/workflow.yaml
--rw-r--r--   0        0        0     2722 2024-03-25 17:07:56.779192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
--rw-r--r--   0        0        0     1395 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
--rw-r--r--   0        0        0     1326 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
--rw-r--r--   0        0        0     2296 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
--rw-r--r--   0        0        0     2579 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
--rw-r--r--   0        0        0    15674 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/manager.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/migration/__init__.py
--rw-r--r--   0        0        0     3992 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/migration/steps.py
--rw-r--r--   0        0        0     1556 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/migration/wf_manifests.py
--rw-r--r--   0        0        0     6528 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/model.py
--rw-r--r--   0        0        0        0 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/__init__.py
--rw-r--r--   0        0        0     2994 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/data_contracts.py
--rw-r--r--   0        0        0      257 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/__init__.py
--rw-r--r--   0        0        0     5161 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_extractor.py
--rw-r--r--   0        0        0     2341 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_loader.py
--rw-r--r--   0        0        0     6040 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_store.py
--rw-r--r--   0        0        0    16874 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/io_steps.py
--rw-r--r--   0        0        0    18272 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_exporter.py
--rw-r--r--   0        0        0     7327 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_importer.py
--rw-r--r--   0        0        0     4785 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_validator.py
--rw-r--r--   0        0        0      274 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/__init__.py
--rw-r--r--   0        0        0     3921 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
--rw-r--r--   0        0        0    29390 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
--rw-r--r--   0        0        0    27269 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_loader.py
--rw-r--r--   0        0        0    12274 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_store.py
--rw-r--r--   0        0        0     2345 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
--rw-r--r--   0        0        0    20657 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
--rw-r--r--   0        0        0    28072 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/rules_importer.py
--rw-r--r--   0        0        0     3010 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps/step_model.py
--rw-r--r--   0        0        0    10467 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/steps_registry.py
--rw-r--r--   0        0        0      788 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/tasks.py
--rw-r--r--   0        0        0     7071 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/triggers.py
--rw-r--r--   0        0        0      453 2024-03-25 17:07:56.783192 cognite_neat-0.68.8/cognite/neat/workflows/utils.py
--rw-r--r--   0        0        0     4543 2024-03-25 17:07:57.167192 cognite_neat-0.68.8/pyproject.toml
--rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.68.8/PKG-INFO
+-rw-r--r--   0        0        0    11351 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/LICENSE
+-rw-r--r--   0        0        0     6775 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/README.md
+-rw-r--r--   0        0        0       61 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/__init__.py
+-rw-r--r--   0        0        0       23 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/_version.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/__init__.py
+-rw-r--r--   0        0        0      152 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/asgi/metrics.py
+-rw-r--r--   0        0        0     4606 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/configuration.py
+-rw-r--r--   0        0        0       90 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/context_manager/__init__.py
+-rw-r--r--   0        0        0      380 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/context_manager/manager.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/data_classes/__init__.py
+-rw-r--r--   0        0        0     4208 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/data_classes/configuration.py
+-rw-r--r--   0        0        0     1675 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/data_classes/rest.py
+-rw-r--r--   0        0        0     1855 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/explorer.py
+-rw-r--r--   0        0        0      554 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/configuration.py
+-rw-r--r--   0        0        0     4646 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/crud.py
+-rw-r--r--   0        0        0    13653 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/data_exploration.py
+-rw-r--r--   0        0        0      210 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/metrics.py
+-rw-r--r--   0        0        0     6369 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/rules.py
+-rw-r--r--   0        0        0    11564 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/routers/workflows.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/utils/__init__.py
+-rw-r--r--   0        0        0      564 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/utils/data_mapping.py
+-rw-r--r--   0        0        0      806 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/utils/logging.py
+-rw-r--r--   0        0        0     4594 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/api/utils/query_templates.py
+-rw-r--r--   0        0        0      357 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/monitoring/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/monitoring/metrics.py
+-rw-r--r--   0        0        0       16 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/index.html
+-rw-r--r--   0        0        0      312 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/.gitignore
+-rw-r--r--   0        0        0     3359 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/README.md
+-rw-r--r--   0        0        0      464 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/asset-manifest.json
+-rw-r--r--   0        0        0     3870 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/favicon.ico
+-rw-r--r--   0        0        0      630 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/index.html
+-rw-r--r--   0        0        0     5347 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/logo192.png
+-rw-r--r--   0        0        0      492 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/manifest.json
+-rw-r--r--   0        0        0       67 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/robots.txt
+-rw-r--r--   0        0        0     8524 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css
+-rw-r--r--   0        0        0    13319 2024-04-03 12:53:19.930544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map
+-rw-r--r--   0        0        0  1403536 2024-04-03 12:53:19.938544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js
+-rw-r--r--   0        0        0     2667 2024-04-03 12:53:19.938544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt
+-rw-r--r--   0        0        0  5996918 2024-04-03 12:53:19.962544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map
+-rw-r--r--   0        0        0     2633 2024-04-03 12:53:19.962544 cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg
+-rw-r--r--   0        0        0     1503 2024-04-03 12:53:19.966544 cognite_neat-0.68.9/cognite/neat/config.py
+-rw-r--r--   0        0        0     1228 2024-04-03 12:53:19.966544 cognite_neat-0.68.9/cognite/neat/constants.py
+-rw-r--r--   0        0        0     4268 2024-04-03 12:53:19.966544 cognite_neat-0.68.9/cognite/neat/exceptions.py
+-rw-r--r--   0        0        0       73 2024-04-03 12:53:19.966544 cognite_neat-0.68.9/cognite/neat/graph/__init__.py
+-rw-r--r--   0        0        0  1439359 2024-04-03 12:53:19.970544 cognite_neat-0.68.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml
+-rw-r--r--   0        0        0  1437996 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml
+-rw-r--r--   0        0        0      368 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/examples/__init__.py
+-rw-r--r--   0        0        0    45798 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx
+-rw-r--r--   0        0        0     3402 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/exceptions.py
+-rw-r--r--   0        0        0      258 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractor/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractor/_base.py
+-rw-r--r--   0        0        0    11232 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractor/_dexpi.py
+-rw-r--r--   0        0        0    17408 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractor/_graph_capturing_sheet.py
+-rw-r--r--   0        0        0    14872 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractor/_mock_graph_generator.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractors/__init__.py
+-rw-r--r--   0        0        0      356 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractors/_base.py
+-rw-r--r--   0        0        0    14811 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/extractors/_mock_graph_generator.py
+-rw-r--r--   0        0        0      693 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/__init__.py
+-rw-r--r--   0        0        0    23838 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/_asset_loader.py
+-rw-r--r--   0        0        0     2370 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/_base.py
+-rw-r--r--   0        0        0     2837 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/_exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/core/__init__.py
+-rw-r--r--   0        0        0     2306 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/core/labels.py
+-rw-r--r--   0        0        0     5016 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/core/models.py
+-rw-r--r--   0        0        0    40458 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/core/rdf_to_assets.py
+-rw-r--r--   0        0        0    22678 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/core/rdf_to_relationships.py
+-rw-r--r--   0        0        0    12957 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/rdf_to_dms.py
+-rw-r--r--   0        0        0     3327 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/loader/validator.py
+-rw-r--r--   0        0        0      149 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/models.py
+-rw-r--r--   0        0        0      543 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/stores/__init__.py
+-rw-r--r--   0        0        0    14254 2024-04-03 12:53:19.974544 cognite_neat-0.68.9/cognite/neat/graph/stores/_base.py
+-rw-r--r--   0        0        0     1776 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/stores/_graphdb_store.py
+-rw-r--r--   0        0        0     1420 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/stores/_memory_store.py
+-rw-r--r--   0        0        0     5377 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/stores/_oxigraph_store.py
+-rw-r--r--   0        0        0     9569 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/stores/_oxrdflib.py
+-rw-r--r--   0        0        0     1244 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/stores/_rdf_to_graph.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/transformation/__init__.py
+-rw-r--r--   0        0        0     4758 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/transformation/entity_matcher.py
+-rw-r--r--   0        0        0       73 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/transformation/query_generator/__init__.py
+-rw-r--r--   0        0        0    18659 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/transformation/query_generator/sparql.py
+-rw-r--r--   0        0        0    14673 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/graph/transformation/transformer.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/py.typed
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/__init__.py
+-rw-r--r--   0        0        0    11635 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/_analysis.py
+-rw-r--r--   0        0        0      177 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/_shared.py
+-rw-r--r--   0        0        0     8596 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/analysis.py
+-rw-r--r--   0        0        0    58987 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx
+-rw-r--r--   0        0        0    80226 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx
+-rw-r--r--   0        0        0      858 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/__init__.py
+-rw-r--r--   0        0        0     2538 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-containers.yaml
+-rw-r--r--   0        0        0    77055 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-example.xlsx
+-rw-r--r--   0        0        0     5501 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-model.yaml
+-rw-r--r--   0        0        0    75865 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/rules-template.xlsx
+-rw-r--r--   0        0        0    52433 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx
+-rw-r--r--   0        0        0    26008 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/skos-rules.xlsx
+-rw-r--r--   0        0        0    79981 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx
+-rw-r--r--   0        0        0    65934 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/examples/wind-energy.owl
+-rw-r--r--   0        0        0   123868 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exceptions.py
+-rw-r--r--   0        0        0      574 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/__init__.py
+-rw-r--r--   0        0        0     1439 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_base.py
+-rw-r--r--   0        0        0      102 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_core/__init__.py
+-rw-r--r--   0        0        0      764 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_core/rules2labels.py
+-rw-r--r--   0        0        0    37099 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2dms.py
+-rw-r--r--   0        0        0     8220 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2excel.py
+-rw-r--r--   0        0        0     6215 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2graphql.py
+-rw-r--r--   0        0        0    18414 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2ontology.py
+-rw-r--r--   0        0        0    28745 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2pydantic_models.py
+-rw-r--r--   0        0        0     3866 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2rules.py
+-rw-r--r--   0        0        0     1104 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2triples.py
+-rw-r--r--   0        0        0     5769 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporter/_validation.py
+-rw-r--r--   0        0        0      413 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporters/__init__.py
+-rw-r--r--   0        0        0     1472 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_base.py
+-rw-r--r--   0        0        0     1645 2024-04-03 12:53:19.978544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_models.py
+-rw-r--r--   0        0        0     9638 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2dms.py
+-rw-r--r--   0        0        0     8717 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2excel.py
+-rw-r--r--   0        0        0    19618 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2ontology.py
+-rw-r--r--   0        0        0     4379 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2rules.py
+-rw-r--r--   0        0        0     2990 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2yaml.py
+-rw-r--r--   0        0        0     4092 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/exporters/_validation.py
+-rw-r--r--   0        0        0      636 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/__init__.py
+-rw-r--r--   0        0        0     2316 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_base.py
+-rw-r--r--   0        0        0     6469 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_dict2rules.py
+-rw-r--r--   0        0        0     7890 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_dms2rules.py
+-rw-r--r--   0        0        0    12097 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_graph2rules.py
+-rw-r--r--   0        0        0     1610 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_json2rules.py
+-rw-r--r--   0        0        0       63 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     8304 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     9320 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     8019 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0    10521 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0     1529 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_spreadsheet2rules.py
+-rw-r--r--   0        0        0      448 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_xsd2rules.py
+-rw-r--r--   0        0        0     1628 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importer/_yaml2rules.py
+-rw-r--r--   0        0        0      408 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/__init__.py
+-rw-r--r--   0        0        0     4265 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_base.py
+-rw-r--r--   0        0        0     8581 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dms2rules.py
+-rw-r--r--   0        0        0       68 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/__init__.py
+-rw-r--r--   0        0        0    12134 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py
+-rw-r--r--   0        0        0    12554 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py
+-rw-r--r--   0        0        0     6925 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py
+-rw-r--r--   0        0        0    11926 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/spec.py
+-rw-r--r--   0        0        0       63 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2classes.py
+-rw-r--r--   0        0        0     7674 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py
+-rw-r--r--   0        0        0     7304 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2properties.py
+-rw-r--r--   0        0        0     5594 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2rules.py
+-rw-r--r--   0        0        0    10579 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_spreadsheet2rules.py
+-rw-r--r--   0        0        0     4198 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/importers/_yaml2rules.py
+-rw-r--r--   0        0        0      563 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/__init__.py
+-rw-r--r--   0        0        0     5856 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/base.py
+-rw-r--r--   0        0        0    10419 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/dms.py
+-rw-r--r--   0        0        0     4492 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/fileread.py
+-rw-r--r--   0        0        0     3346 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/formatters.py
+-rw-r--r--   0        0        0     6916 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/importing.py
+-rw-r--r--   0        0        0    13763 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/spreadsheet.py
+-rw-r--r--   0        0        0     4964 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/issues/spreadsheet_file.py
+-rw-r--r--   0        0        0      127 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/__init__.py
+-rw-r--r--   0        0        0     4989 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_base.py
+-rw-r--r--   0        0        0      517 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/__init__.py
+-rw-r--r--   0        0        0     1227 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/__init__.py
+-rw-r--r--   0        0        0    13343 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_base.py
+-rw-r--r--   0        0        0     9677 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_field.py
+-rw-r--r--   0        0        0     5207 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_value.py
+-rw-r--r--   0        0        0    10149 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/base.py
+-rw-r--r--   0        0        0    46469 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/dms_architect_rules.py
+-rw-r--r--   0        0        0    28761 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/dms_schema.py
+-rw-r--r--   0        0        0     1878 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/domain_rules.py
+-rw-r--r--   0        0        0    19266 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/_rules/information_rules.py
+-rw-r--r--   0        0        0    12368 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/raw_rules.py
+-rw-r--r--   0        0        0     7228 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/rdfpath.py
+-rw-r--r--   0        0        0    51063 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/rules.py
+-rw-r--r--   0        0        0      171 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/tables.py
+-rw-r--r--   0        0        0     4316 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/rules/models/value_types.py
+-rw-r--r--   0        0        0       68 2024-04-03 12:53:19.982544 cognite_neat-0.68.9/cognite/neat/utils/__init__.py
+-rw-r--r--   0        0        0      309 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/auxiliary.py
+-rw-r--r--   0        0        0      711 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf.py
+-rw-r--r--   0        0        0      483 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_base.py
+-rw-r--r--   0        0        0     9719 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_data_modeling.py
+-rw-r--r--   0        0        0     6319 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_ingestion.py
+-rw-r--r--   0        0        0     3844 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/data_classes.py
+-rw-r--r--   0        0        0      981 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/exceptions.py
+-rw-r--r--   0        0        0     2468 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/spreadsheet.py
+-rw-r--r--   0        0        0     3082 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/text.py
+-rw-r--r--   0        0        0    12826 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/utils.py
+-rw-r--r--   0        0        0      992 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/utils/xml.py
+-rw-r--r--   0        0        0      396 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/__init__.py
+-rw-r--r--   0        0        0     1348 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/_exceptions.py
+-rw-r--r--   0        0        0    26223 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/base.py
+-rw-r--r--   0        0        0    18016 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/cdf_store.py
+-rw-r--r--   0        0        0     1987 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Export DMS/workflow.yaml
+-rw-r--r--   0        0        0     3604 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml
+-rw-r--r--   0        0        0     3384 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml
+-rw-r--r--   0        0        0     6205 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml
+-rw-r--r--   0        0        0     1364 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Import DMS/workflow.yaml
+-rw-r--r--   0        0        0     2722 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml
+-rw-r--r--   0        0        0     1395 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Validate Rules/workflow.yaml
+-rw-r--r--   0        0        0     1326 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml
+-rw-r--r--   0        0        0     2296 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml
+-rw-r--r--   0        0        0     2579 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml
+-rw-r--r--   0        0        0    15674 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/manager.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/migration/__init__.py
+-rw-r--r--   0        0        0     3992 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/migration/steps.py
+-rw-r--r--   0        0        0     1556 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/migration/wf_manifests.py
+-rw-r--r--   0        0        0     6528 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/model.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/__init__.py
+-rw-r--r--   0        0        0     2994 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/data_contracts.py
+-rw-r--r--   0        0        0      257 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/__init__.py
+-rw-r--r--   0        0        0     5161 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_extractor.py
+-rw-r--r--   0        0        0     2341 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_loader.py
+-rw-r--r--   0        0        0     6040 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_store.py
+-rw-r--r--   0        0        0    16874 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/io_steps.py
+-rw-r--r--   0        0        0    18272 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_exporter.py
+-rw-r--r--   0        0        0     7327 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_importer.py
+-rw-r--r--   0        0        0     4785 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_validator.py
+-rw-r--r--   0        0        0      274 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/__init__.py
+-rw-r--r--   0        0        0     3921 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py
+-rw-r--r--   0        0        0    29390 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_extractor.py
+-rw-r--r--   0        0        0    27269 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_loader.py
+-rw-r--r--   0        0        0    12274 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_store.py
+-rw-r--r--   0        0        0     2345 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_transformer.py
+-rw-r--r--   0        0        0    20657 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/rules_exporter.py
+-rw-r--r--   0        0        0    28072 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/rules_importer.py
+-rw-r--r--   0        0        0     3010 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps/step_model.py
+-rw-r--r--   0        0        0    10467 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/steps_registry.py
+-rw-r--r--   0        0        0      788 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/tasks.py
+-rw-r--r--   0        0        0     7071 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/triggers.py
+-rw-r--r--   0        0        0      453 2024-04-03 12:53:19.986544 cognite_neat-0.68.9/cognite/neat/workflows/utils.py
+-rw-r--r--   0        0        0     4543 2024-04-03 12:53:20.374546 cognite_neat-0.68.9/pyproject.toml
+-rw-r--r--   0        0        0     9321 1970-01-01 00:00:00.000000 cognite_neat-0.68.9/PKG-INFO
```

### Comparing `cognite_neat-0.68.8/LICENSE` & `cognite_neat-0.68.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/README.md` & `cognite_neat-0.68.9/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/configuration.py` & `cognite_neat-0.68.9/cognite/neat/app/api/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/data_classes/configuration.py` & `cognite_neat-0.68.9/cognite/neat/app/api/data_classes/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/data_classes/rest.py` & `cognite_neat-0.68.9/cognite/neat/app/api/data_classes/rest.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/explorer.py` & `cognite_neat-0.68.9/cognite/neat/app/api/explorer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/routers/configuration.py` & `cognite_neat-0.68.9/cognite/neat/app/api/routers/configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/routers/crud.py` & `cognite_neat-0.68.9/cognite/neat/app/api/routers/crud.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/routers/data_exploration.py` & `cognite_neat-0.68.9/cognite/neat/app/api/routers/data_exploration.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/routers/rules.py` & `cognite_neat-0.68.9/cognite/neat/app/api/routers/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/routers/workflows.py` & `cognite_neat-0.68.9/cognite/neat/app/api/routers/workflows.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/utils/data_mapping.py` & `cognite_neat-0.68.9/cognite/neat/app/api/utils/data_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/utils/logging.py` & `cognite_neat-0.68.9/cognite/neat/app/api/utils/logging.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/api/utils/query_templates.py` & `cognite_neat-0.68.9/cognite/neat/app/api/utils/query_templates.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/monitoring/metrics.py` & `cognite_neat-0.68.9/cognite/neat/app/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/README.md` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/README.md`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/favicon.ico` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/index.html` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/index.html`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/logo192.png` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/logo192.png`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/css/main.38a62222.css.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/js/main.ed960141.js.map`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg` & `cognite_neat-0.68.9/cognite/neat/app/ui/neat-app/build/static/media/logo.4bdbcf8396881de06a6723a92fed910b.svg`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/config.py` & `cognite_neat-0.68.9/cognite/neat/config.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/constants.py` & `cognite_neat-0.68.9/cognite/neat/constants.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/exceptions.py` & `cognite_neat-0.68.9/cognite/neat/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml` & `cognite_neat-0.68.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44-dirty.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml` & `cognite_neat-0.68.9/cognite/neat/graph/examples/Knowledge-Graph-Nordic44.xml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx` & `cognite_neat-0.68.9/cognite/neat/graph/examples/skos-capturing-sheet-wind-topics.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/exceptions.py` & `cognite_neat-0.68.9/cognite/neat/graph/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/extractor/_dexpi.py` & `cognite_neat-0.68.9/cognite/neat/graph/extractor/_dexpi.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/extractor/_graph_capturing_sheet.py` & `cognite_neat-0.68.9/cognite/neat/graph/extractor/_graph_capturing_sheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/extractor/_mock_graph_generator.py` & `cognite_neat-0.68.9/cognite/neat/graph/extractor/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/extractors/_mock_graph_generator.py` & `cognite_neat-0.68.9/cognite/neat/graph/extractors/_mock_graph_generator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/__init__.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/_asset_loader.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/_asset_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/_base.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/_exceptions.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/core/labels.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/core/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/core/models.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/core/models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/core/rdf_to_assets.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/core/rdf_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/core/rdf_to_relationships.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/core/rdf_to_relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/rdf_to_dms.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/rdf_to_dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/loader/validator.py` & `cognite_neat-0.68.9/cognite/neat/graph/loader/validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/__init__.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_base.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_graphdb_store.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_graphdb_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_memory_store.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_memory_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_oxigraph_store.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_oxigraph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_oxrdflib.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_oxrdflib.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/stores/_rdf_to_graph.py` & `cognite_neat-0.68.9/cognite/neat/graph/stores/_rdf_to_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/transformation/entity_matcher.py` & `cognite_neat-0.68.9/cognite/neat/graph/transformation/entity_matcher.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/transformation/query_generator/sparql.py` & `cognite_neat-0.68.9/cognite/neat/graph/transformation/query_generator/sparql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/graph/transformation/transformer.py` & `cognite_neat-0.68.9/cognite/neat/graph/transformation/transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/_analysis.py` & `cognite_neat-0.68.9/cognite/neat/rules/_analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/analysis.py` & `cognite_neat-0.68.9/cognite/neat/rules/analysis.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/Rules-Nordic44-to-TNT.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/Rules-Nordic44-to-graphql.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-containers.yaml` & `cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-containers.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-example.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-example.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/power-grid-model.yaml` & `cognite_neat-0.68.9/cognite/neat/rules/examples/power-grid-model.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/rules-template.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/rules-template.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/sheet2cdf-transformation-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/skos-rules.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/skos-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx` & `cognite_neat-0.68.9/cognite/neat/rules/examples/source-to-solution-mapping-rules.xlsx`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/examples/wind-energy.owl` & `cognite_neat-0.68.9/cognite/neat/rules/examples/wind-energy.owl`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exceptions.py` & `cognite_neat-0.68.9/cognite/neat/rules/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - 0 - 99: errors and warnings raised when dealing with TransformationRules pydantic model
 - 100 - 199: errors and warnings raised when parsing actual transformation rules, i.e. `rdfpath`
 - 200 - 299: errors and warnings raised when dealing TransformationRules importers
 - 300 - 399: errors and warnings raised when dealing TransformationRules parsers
 - 400 - 499: errors and warnings raised when dealing TransformationRules exporters
 
 """
+
 from typing import Any
 
 from cognite.client.data_classes.data_modeling import ContainerId, DataModelId, ViewId
 from rdflib import Namespace, URIRef
 
 from cognite.neat.constants import DEFAULT_DOCS_URL
 from cognite.neat.exceptions import NeatException, NeatWarning
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_core/rules2labels.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_core/rules2labels.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2dms.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2excel.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2graphql.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2graphql.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2ontology.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2pydantic_models.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2pydantic_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_rules2triples.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_rules2triples.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporter/_validation.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporter/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_models.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_models.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2dms.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2dms.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import warnings
-import zipfile
 from collections.abc import Collection, Iterable
 from pathlib import Path
 from typing import Literal, TypeAlias
 
 from cognite.client import CogniteClient
 from cognite.client.data_classes._base import CogniteResourceList
 from cognite.client.exceptions import CogniteAPIError
@@ -84,65 +83,31 @@
         if filepath.is_dir():
             self._export_to_directory(filepath, rules)
         else:
             self._export_to_zip_file(filepath, rules)
 
     def _export_to_directory(self, directory: Path, rules: Rules) -> None:
         schema = self.export(rules)
-        data_models = directory / "data_models"
-        data_models.mkdir(exist_ok=True, parents=True)
-        if self.export_components.intersection({"all", "spaces"}):
-            for space in schema.spaces:
-                (data_models / f"{space.space}.space.yaml").write_text(space.dump_yaml())
-        if self.export_components.intersection({"all", "data_models"}):
-            for model in schema.data_models:
-                (data_models / f"{model.external_id}.datamodel.yaml").write_text(model.dump_yaml())
-        if self.export_components.intersection({"all", "views"}):
-            for view in schema.views:
-                (data_models / f"{view.external_id}.view.yaml").write_text(view.dump_yaml())
-        if self.export_components.intersection({"all", "containers"}):
-            for container in schema.containers:
-                (data_models / f"{container.external_id}.container.yaml").write_text(container.dump_yaml())
-        if isinstance(schema, PipelineSchema):
-            transformations = directory / "transformations"
-            transformations.mkdir(exist_ok=True, parents=True)
-            for transformation in schema.transformations:
-                (transformations / f"{transformation.external_id}.yaml").write_text(transformation.dump_yaml())
-            # The RAW Databases are not written to file. This is because cognite-toolkit expects the RAW databases
-            # to be in the same file as the RAW tables.
-            raw = directory / "raw"
-            raw.mkdir(exist_ok=True, parents=True)
-            for raw_table in schema.raw_tables:
-                (raw / f"{raw_table.name}.yaml").write_text(raw_table.dump_yaml())
+        exclude = self._create_exclude_set()
+        schema.to_directory(directory, exclude=exclude)
 
     def _export_to_zip_file(self, filepath: Path, rules: Rules) -> None:
         if filepath.suffix not in {".zip"}:
             warnings.warn("File extension is not .zip, adding it to the file name", stacklevel=2)
             filepath = filepath.with_suffix(".zip")
         schema = self.export(rules)
-        with zipfile.ZipFile(filepath, "w") as zip_ref:
-            if self.export_components.intersection({"all", "spaces"}):
-                for space in schema.spaces:
-                    zip_ref.writestr(f"data_models/{space.space}.space.yaml", space.dump_yaml())
-            if self.export_components.intersection({"all", "data_models"}):
-                for model in schema.data_models:
-                    zip_ref.writestr(f"data_models/{model.external_id}.datamodel.yaml", model.dump_yaml())
-            if self.export_components.intersection({"all", "views"}):
-                for view in schema.views:
-                    zip_ref.writestr(f"data_models/{view.external_id}.view.yaml", view.dump_yaml())
-            if self.export_components.intersection({"all", "containers"}):
-                for container in schema.containers:
-                    zip_ref.writestr(f"data_models/{container.external_id}.container.yaml", container.dump_yaml())
-            if isinstance(schema, PipelineSchema):
-                for transformation in schema.transformations:
-                    zip_ref.writestr(f"transformations/{transformation.external_id}.yaml", transformation.dump_yaml())
-                # The RAW Databases are not written to file. This is because cognite-toolkit expects the RAW databases
-                # to be in the same file as the RAW tables.
-                for raw_table in schema.raw_tables:
-                    zip_ref.writestr(f"raw/{raw_table.name}.yaml", raw_table.dump_yaml())
+        exclude = self._create_exclude_set()
+        schema.to_zip(filepath, exclude=exclude)
+
+    def _create_exclude_set(self):
+        if "all" in self.export_components:
+            exclude = set()
+        else:
+            exclude = {"spaces", "data_models", "views", "containers"} - self.export_components
+        return exclude
 
     def export(self, rules: Rules) -> DMSSchema:
         if isinstance(rules, DMSRules):
             return rules.as_schema(self.standardize_casing, self.export_pipeline, self.instance_space)
         elif isinstance(rules, InformationRules):
             return rules.as_dms_architect_rules().as_schema(
                 self.standardize_casing, self.export_pipeline, self.instance_space
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2excel.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2excel.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2ontology.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2ontology.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_rules2yaml.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_rules2yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/exporters/_validation.py` & `cognite_neat-0.68.9/cognite/neat/rules/exporters/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_dict2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_dict2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_dms2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_dms2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_graph2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_graph2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_json2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_json2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2classes.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2properties.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_owl2rules/_owl2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_spreadsheet2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_spreadsheet2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importer/_yaml2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importer/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_dms2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_dms2rules.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Literal, cast, overload
 
 from cognite.client import CogniteClient
 from cognite.client import data_modeling as dm
 from cognite.client.data_classes.data_modeling import DataModelIdentifier
 from cognite.client.data_classes.data_modeling.containers import BTreeIndex, InvertedIndex
 from cognite.client.data_classes.data_modeling.data_types import ListablePropertyType
@@ -30,14 +31,24 @@
     def __init__(self, schema: DMSSchema):
         self.schema = schema
 
     @classmethod
     def from_data_model_id(cls, client: CogniteClient, data_model_id: DataModelIdentifier) -> "DMSImporter":
         return cls(DMSSchema.from_model_id(client, data_model_id))
 
+    @classmethod
+    def from_directory(cls, directory: str | Path) -> "DMSImporter":
+        return cls(DMSSchema.from_directory(directory))
+
+    @classmethod
+    def from_zip_file(cls, zip_file: str | Path) -> "DMSImporter":
+        if Path(zip_file).suffix != ".zip":
+            raise ValueError("File extension is not .zip")
+        return cls(DMSSchema.from_zip(zip_file))
+
     @overload
     def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
         ...
 
     @overload
     def to_rules(
         self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/_unit_lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_converter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/dtdl_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_dtdl2rules/spec.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_dtdl2rules/spec.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2classes.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2classes.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2metadata.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2properties.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2properties.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_owl2rules/_owl2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_owl2rules/_owl2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_spreadsheet2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_spreadsheet2rules.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,127 +1,226 @@
 """This module performs importing of graph to TransformationRules pydantic class.
 In more details, it traverses the graph and abstracts class and properties, basically
 generating a list of rules based on which nodes that form the graph are made.
 """
-from collections import defaultdict
+
+from collections import UserDict, defaultdict
 from pathlib import Path
 from typing import Literal, cast, overload
 
 import pandas as pd
+from pandas import ExcelFile
 
-import cognite.neat.rules.issues.spreadsheet_file
 from cognite.neat.rules import issues
 from cognite.neat.rules.issues import IssueList
 from cognite.neat.rules.models._rules import RULES_PER_ROLE, DMSRules, DomainRules, InformationRules
-from cognite.neat.rules.models._rules.base import RoleTypes
+from cognite.neat.rules.models._rules.base import RoleTypes, SchemaCompleteness
 from cognite.neat.utils.auxiliary import local_import
-from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_spreadsheet
+from cognite.neat.utils.spreadsheet import SpreadsheetRead, read_individual_sheet
 
 from ._base import BaseImporter, Rules, _handle_issues
 
+SOURCE_SHEET__TARGET_FIELD__HEADERS = [
+    ("Properties", "Properties", "Class"),
+    ("Classes", "Classes", "Class"),
+    ("Containers", "Containers", "Container"),
+    ("Views", "Views", "View"),
+]
+
+MANDATORY_SHEETS_BY_ROLE: dict[RoleTypes, set[str]] = {
+    role_type: {str(sheet_name) for sheet_name in RULES_PER_ROLE[role_type].mandatory_fields(use_alias=True)}
+    for role_type in RoleTypes.__members__.values()
+}
+
+
+class MetadataRaw(UserDict):
+    @classmethod
+    def from_excel(cls, excel_file: ExcelFile, metadata_sheet_name: str) -> "MetadataRaw":
+        return cls(pd.read_excel(excel_file, metadata_sheet_name, header=None).replace(float("nan"), None).values)
+
+    @property
+    def has_role_field(self) -> bool:
+        return self.get("role") in [role.value for role in RoleTypes.__members__.values()]
+
+    @property
+    def role(self) -> RoleTypes:
+        return RoleTypes(self["role"])
+
+    @property
+    def has_schema_field(self) -> bool:
+        return self.get("schema") in [schema.value for schema in SchemaCompleteness.__members__.values()]
+
+    def is_valid(self, issue_list: IssueList, filepath: Path) -> bool:
+        if not self.has_role_field:
+            issue_list.append(issues.spreadsheet_file.RoleMissingOrUnsupportedError(filepath))
+            return False
+
+        # check if there is a schema field if role is not domain expert
+        if self.role != RoleTypes.domain_expert and not self.has_schema_field:
+            issue_list.append(issues.spreadsheet_file.SchemaMissingOrUnsupportedError(filepath))
+            return False
+        return True
+
+
+class SpreadsheetReader:
+    def __init__(self, issue_list: IssueList, is_reference: bool = False):
+        self.issue_list = issue_list
+        self._is_reference = is_reference
+
+    @property
+    def metadata_sheet_name(self) -> str:
+        metadata_name = "Metadata"
+        return self.to_reference_sheet(metadata_name) if self._is_reference else metadata_name
+
+    def sheet_names(self, role: RoleTypes) -> set[str]:
+        names = MANDATORY_SHEETS_BY_ROLE[role]
+        return {self.to_reference_sheet(sheet_name) for sheet_name in names} if self._is_reference else names
+
+    @classmethod
+    def to_reference_sheet(cls, sheet_name: str) -> str:
+        return f"Reference{sheet_name}"
+
+    def read(self, filepath: Path) -> Rules | None:
+        with pd.ExcelFile(filepath) as excel_file:
+            if self.metadata_sheet_name not in excel_file.sheet_names:
+                self.issue_list.append(
+                    issues.spreadsheet_file.MetadataSheetMissingOrFailedError(
+                        filepath, sheet_name=self.metadata_sheet_name
+                    )
+                )
+                return None
+
+            metadata = MetadataRaw.from_excel(excel_file, self.metadata_sheet_name)
+
+            if not metadata.is_valid(self.issue_list, filepath):
+                return None
+
+            sheets, read_info_by_sheet = self._read_sheets(metadata, excel_file)
+            if self.issue_list.has_errors:
+                return None
+
+            rules_cls = RULES_PER_ROLE[metadata.role]
+            with _handle_issues(
+                self.issue_list,
+                error_cls=issues.spreadsheet.InvalidSheetError,
+                error_args={"read_info_by_sheet": read_info_by_sheet},
+            ) as future:
+                rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
+
+            if future.result == "failure" or self.issue_list.has_errors:
+                return None
+
+        return rules
+
+    def _read_sheets(
+        self, metadata: MetadataRaw, excel_file: ExcelFile
+    ) -> tuple[dict[str, dict | list] | None, dict[str, SpreadsheetRead]]:
+        read_info_by_sheet: dict[str, SpreadsheetRead] = defaultdict(SpreadsheetRead)
+
+        sheets: dict[str, dict | list] = {"Metadata": dict(metadata)}
+
+        expected_sheet_names = self.sheet_names(metadata.role)
+
+        if missing_sheets := expected_sheet_names.difference(set(excel_file.sheet_names)):
+            self.issue_list.append(
+                issues.spreadsheet_file.SheetMissingError(cast(Path, excel_file.io), list(missing_sheets))
+            )
+            return None, read_info_by_sheet
+
+        for source_sheet_name, target_sheet_name, headers in SOURCE_SHEET__TARGET_FIELD__HEADERS:
+            source_sheet_name = self.to_reference_sheet(source_sheet_name) if self._is_reference else source_sheet_name
+
+            if source_sheet_name not in excel_file.sheet_names:
+                continue
+
+            try:
+                sheets[target_sheet_name], read_info_by_sheet[source_sheet_name] = read_individual_sheet(
+                    excel_file, source_sheet_name, return_read_info=True, expected_headers=[headers]
+                )
+            except Exception as e:
+                self.issue_list.append(issues.spreadsheet_file.ReadSpreadsheetsError(cast(Path, excel_file.io), str(e)))
+                continue
+
+        return sheets, read_info_by_sheet
+
 
 class ExcelImporter(BaseImporter):
     def __init__(self, filepath: Path):
         self.filepath = filepath
 
     @overload
     def to_rules(self, errors: Literal["raise"], role: RoleTypes | None = None, is_reference: bool = False) -> Rules:
         ...
 
     @overload
     def to_rules(
-        self, errors: Literal["continue"] = "continue", role: RoleTypes | None = None, is_reference: bool = False
+        self,
+        errors: Literal["continue"] = "continue",
+        role: RoleTypes | None = None,
+        is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList]:
         ...
 
     def to_rules(
         self,
         errors: Literal["raise", "continue"] = "continue",
         role: RoleTypes | None = None,
         is_reference: bool = False,
     ) -> tuple[Rules | None, IssueList] | Rules:
         issue_list = IssueList(title=f"'{self.filepath.name}'")
+
         if not self.filepath.exists():
-            issue_list.append(cognite.neat.rules.issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
-            if errors == "raise":
-                raise issue_list.as_errors() from None
-            return None, issue_list
+            issue_list.append(issues.spreadsheet_file.SpreadsheetNotFoundError(self.filepath))
+            return self._return_or_raise(issue_list, errors)
 
-        with pd.ExcelFile(self.filepath) as excel_file:
-            try:
-                metadata = dict(pd.read_excel(excel_file, "Metadata", header=None).values)
-            except ValueError:
-                issue_list.append(
-                    cognite.neat.rules.issues.spreadsheet_file.MetadataSheetMissingOrFailedError(self.filepath)
-                )
-                if errors == "raise":
-                    raise issue_list.as_errors() from None
-                return None, issue_list
-
-            role_input = RoleTypes(metadata.get("role", RoleTypes.domain_expert))
-            role_enum = RoleTypes(role_input)
-            rules_model = RULES_PER_ROLE[role_enum]
-            sheet_names = {str(name) for name in excel_file.sheet_names}
-            expected_sheet_names = rules_model.mandatory_fields(use_alias=True)
-
-            if missing_sheets := expected_sheet_names.difference(sheet_names):
-                issue_list.append(
-                    cognite.neat.rules.issues.spreadsheet_file.SheetMissingError(self.filepath, list(missing_sheets))
-                )
-                if errors == "raise":
-                    raise issue_list.as_errors()
-                return None, issue_list
-
-            sheets: dict[str, dict | list] = {"Metadata": metadata}
-            read_info_by_sheet: dict[str, SpreadsheetRead] = defaultdict(SpreadsheetRead)
-            for sheet_name, headers in [
-                ("Properties", "Class"),
-                ("Classes", "Class"),
-                ("Containers", "Container"),
-                ("Views", "View"),
-            ]:
-                if sheet_name in excel_file.sheet_names:
-                    try:
-                        sheets[sheet_name], read_info_by_sheet[sheet_name] = read_spreadsheet(
-                            excel_file, sheet_name, return_read_info=True, expected_headers=[headers]
-                        )
-                    except Exception as e:
-                        issue_list.append(
-                            cognite.neat.rules.issues.spreadsheet_file.ReadSpreadsheetsError(self.filepath, str(e))
-                        )
-                        continue
-            if issue_list:
-                if errors == "raise":
-                    raise issue_list.as_errors()
-                return None, issue_list
-
-        rules_cls = {
-            RoleTypes.domain_expert: DomainRules,
-            RoleTypes.information_architect: InformationRules,
-            RoleTypes.dms_architect: DMSRules,
-        }.get(role_enum)
-        if rules_cls is None:
-            issue_list.append(cognite.neat.rules.issues.spreadsheet_file.InvalidRoleError(str(role_input)))
-            if errors == "raise":
-                raise issue_list.as_errors()
-            return None, issue_list
+        user_rules: Rules | None = None
+        if not is_reference:
+            user_rules = SpreadsheetReader(issue_list, is_reference=False).read(self.filepath)
+            if issue_list.has_errors:
+                return self._return_or_raise(issue_list, errors)
+
+        reference_rules: Rules | None = None
+        if is_reference or (
+            user_rules
+            and user_rules.metadata.role != RoleTypes.domain_expert
+            and cast(DMSRules | InformationRules, user_rules).metadata.schema_ == SchemaCompleteness.extended
+        ):
+            reference_rules = SpreadsheetReader(issue_list, is_reference=True).read(self.filepath)
+            if issue_list.has_errors:
+                return self._return_or_raise(issue_list, errors)
+
+        if user_rules and reference_rules and user_rules.metadata.role != reference_rules.metadata.role:
+            issue_list.append(issues.spreadsheet_file.RoleMismatchError(self.filepath))
+            return self._return_or_raise(issue_list, errors)
+
+        if user_rules and reference_rules:
+            rules = user_rules
+            rules.reference = reference_rules
+        elif user_rules:
+            rules = user_rules
+        elif reference_rules:
+            rules = reference_rules
+        else:
+            raise ValueError(
+                "No rules were generated. This should have been caught earlier. " f"Bug in {type(self).__name__}."
+            )
 
-        with _handle_issues(
+        return self._to_output(
+            rules,
             issue_list,
-            error_cls=issues.spreadsheet.InvalidSheetError,
-            error_args={"read_info_by_sheet": read_info_by_sheet},
-        ) as future:
-            rules = rules_cls.model_validate(sheets)  # type: ignore[attr-defined]
-        if future.result == "failure":
-            if errors == "continue":
-                return None, issue_list
-            else:
-                raise issue_list.as_errors()
-
-        return self._to_output(rules, issue_list, errors=errors, role=role, is_reference=is_reference)
+            errors=errors,
+            role=role,
+            is_reference=is_reference,
+        )
+
+    @classmethod
+    def _return_or_raise(cls, issue_list: IssueList, errors: Literal["raise", "continue"]) -> tuple[None, IssueList]:
+        if errors == "raise":
+            raise issue_list.as_errors()
+        return None, issue_list
 
 
 class GoogleSheetImporter(BaseImporter):
     def __init__(self, sheet_id: str, skiprows: int = 1):
         self.sheet_id = sheet_id
         self.skiprows = skiprows
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/importers/_yaml2rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/importers/_yaml2rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/base.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,14 +154,18 @@
         self.title = title
 
     @property
     def errors(self) -> "IssueList":
         return IssueList([issue for issue in self if isinstance(issue, NeatValidationError)])
 
     @property
+    def has_errors(self) -> bool:
+        return any(isinstance(issue, NeatValidationError) for issue in self)
+
+    @property
     def warnings(self) -> "IssueList":
         return IssueList([issue for issue in self if isinstance(issue, ValidationWarning)])
 
     def as_errors(self) -> ExceptionGroup:
         return ExceptionGroup(
             "Validation failed",
             [ValueError(issue.message()) for issue in self if isinstance(issue, NeatValidationError)],
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/dms.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/dms.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/fileread.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/fileread.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/formatters.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/formatters.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/importing.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/importing.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/spreadsheet.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/issues/spreadsheet_file.py` & `cognite_neat-0.68.9/cognite/neat/rules/issues/spreadsheet_file.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,20 +35,68 @@
         return output
 
 
 @dataclass(frozen=True)
 class MetadataSheetMissingOrFailedError(SpreadsheetFileError):
     description: ClassVar[str] = "Metadata sheet is missing or it failed validation for one or more fields"
     fix: ClassVar[str] = "Make sure to define compliant Metadata sheet before proceeding"
+    hint: str | None = None
+    sheet_name: str = "Metadata"
+
+    def message(self) -> str:
+        output = (
+            f" {self.sheet_name} sheet is missing or it failed"
+            + f" validation for one or more fields in {self.filepath.name}. "
+            + self.fix
+        )
+        if self.hint:
+            output += f" Hint: {self.hint}"
+        return output
+
+
+@dataclass(frozen=True)
+class RoleMissingOrUnsupportedError(SpreadsheetFileError):
+    description: ClassVar[str] = "Role field in Metadata sheet is missing or its value is unsupported"
+    fix: ClassVar[str] = "Make sure to define compliant role in Metadata sheet before proceeding"
+
+    hint: str | None = None
+
+    def message(self) -> str:
+        output = (
+            f"Role field in Metadata sheet is missing or its value is unsupported {self.filepath.name}. " + self.fix
+        )
+        if self.hint:
+            output += f" Hint: {self.hint}"
+        return output
+
+
+@dataclass(frozen=True)
+class RoleMismatchError(SpreadsheetFileError):
+    description: ClassVar[str] = "Roles between user and reference Metadata sheets do not match"
+    fix: ClassVar[str] = "Make sure that both user and reference Metadata sheets have the same role defined"
+
+    hint: str | None = None
+
+    def message(self) -> str:
+        output = f"Roles between user and reference Metadata sheets do not match {self.filepath.name}. " + self.fix
+        if self.hint:
+            output += f" Hint: {self.hint}"
+        return output
+
+
+@dataclass(frozen=True)
+class SchemaMissingOrUnsupportedError(SpreadsheetFileError):
+    description: ClassVar[str] = "Schema field in Metadata sheet is missing or its value unsupported"
+    fix: ClassVar[str] = "Make sure to define compliant schema in Metadata sheet before proceeding"
 
     hint: str | None = None
 
     def message(self) -> str:
         output = (
-            f"Metadata sheet is missing or it failed validation for one or more fields in {self.filepath.name}. "
+            f"Schema field in Metadata sheet is missing or its value unsupported in file {self.filepath.name}. "
             + self.fix
         )
         if self.hint:
             output += f" Hint: {self.hint}"
         return output
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/__init__.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_base.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_field.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_field.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/_types/_value.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/_types/_value.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/base.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module contains the definition of `TransformationRules` pydantic model and all
 its sub-models and validators.
 """
+
 from __future__ import annotations
 
 import math
 import sys
 import types
 from collections.abc import Callable, Iterator
 from functools import wraps
@@ -115,14 +116,20 @@
 
 class SchemaCompleteness(StrEnum):
     complete = "complete"
     partial = "partial"
     extended = "extended"
 
 
+class ExtensionCategory(StrEnum):
+    addition = "addition"
+    reshape = "reshape"
+    rebuild = "rebuild"
+
+
 class RoleTypes(StrEnum):
     domain_expert = "domain expert"
     information_architect = "information architect"
     dms_architect = "DMS Architect"
 
 
 class MatchType(StrEnum):
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/dms_architect_rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/dms_architect_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     VersionType,
     ViewEntity,
     ViewListType,
     ViewPropEntity,
     ViewType,
     XSDValueType,
 )
-from .base import BaseMetadata, BaseRules, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
+from .base import BaseMetadata, BaseRules, ExtensionCategory, RoleTypes, SchemaCompleteness, SheetEntity, SheetList
 from .dms_schema import DMSSchema, PipelineSchema
 
 if TYPE_CHECKING:
     from .information_rules import InformationRules
 
 
 subclasses = list(CognitePropertyType.__subclasses__())
@@ -58,14 +58,15 @@
         ...
 del subclasses  # cleanup namespace
 
 
 class DMSMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.dms_architect
     schema_: SchemaCompleteness = Field(alias="schema")
+    extension: ExtensionCategory = ExtensionCategory.addition
     space: ExternalIdType
     name: str | None = Field(
         None,
         description="Human readable name of the data model",
         min_length=1,
         max_length=255,
     )
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/domain_rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/domain_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/_rules/information_rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/_rules/information_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,24 @@
     SemanticValueType,
     StrListType,
     Undefined,
     VersionType,
     ViewPropEntity,
     XSDValueType,
 )
-from .base import BaseMetadata, MatchType, RoleTypes, RuleModel, SchemaCompleteness, SheetEntity, SheetList
+from .base import (
+    BaseMetadata,
+    ExtensionCategory,
+    MatchType,
+    RoleTypes,
+    RuleModel,
+    SchemaCompleteness,
+    SheetEntity,
+    SheetList,
+)
 from .domain_rules import DomainRules
 
 if TYPE_CHECKING:
     from .dms_architect_rules import DMSProperty, DMSRules
 
 
 if sys.version_info >= (3, 11):
@@ -52,14 +61,15 @@
 else:
     from typing_extensions import Self
 
 
 class InformationMetadata(BaseMetadata):
     role: ClassVar[RoleTypes] = RoleTypes.information_architect
     schema_: SchemaCompleteness = Field(alias="schema")
+    extension: ExtensionCategory | None = ExtensionCategory.addition
     prefix: PrefixType
     namespace: NamespaceType
 
     name: str = Field(
         alias="title",
         description="Human readable name of the data model",
         min_length=1,
@@ -78,14 +88,21 @@
     creator: StrListType = Field(
         description=(
             "List of contributors to the data model creation, "
             "typically information architects are considered as contributors."
         ),
     )
 
+    @model_validator(mode="after")
+    def extension_none_but_schema_extend(self) -> Self:
+        if self.extension is None:
+            self.extension = ExtensionCategory.addition
+            return self
+        return self
+
 
 class InformationClass(SheetEntity):
     """
     Class is a category of things that share a common set of attributes and relationships.
 
     Args:
         class_: The class ID of the class.
```

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/raw_rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/raw_rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/rdfpath.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/rdfpath.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/rules.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/rules.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/rules/models/value_types.py` & `cognite_neat-0.68.9/cognite/neat/rules/models/value_types.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/cdf.py` & `cognite_neat-0.68.9/cognite/neat/utils/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_base.py` & `cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_data_modeling.py` & `cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_data_modeling.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/_ingestion.py` & `cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/_ingestion.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/cdf_loaders/data_classes.py` & `cognite_neat-0.68.9/cognite/neat/utils/cdf_loaders/data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 
 @dataclass(frozen=True)
 class RawTableID:
     table: str
     database: str
 
+    def as_tuple(self) -> tuple[str, str]:
+        return self.database, self.table
+
 
 class RawTableCore(WriteableCogniteResource["RawTableWrite"], ABC):
     """A NoSQL database table to store customer data
 
     Args:
         name (str | None): Unique name of the table
     """
```

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/exceptions.py` & `cognite_neat-0.68.9/cognite/neat/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/spreadsheet.py` & `cognite_neat-0.68.9/cognite/neat/utils/spreadsheet.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,34 +28,34 @@
                 output += 1
             else:
                 break
         return output
 
 
 @overload
-def read_spreadsheet(
+def read_individual_sheet(
     excel_file: pd.ExcelFile,
     sheet_name: str,
     return_read_info: Literal[True],
     expected_headers: list[str] | None = None,
 ) -> tuple[list[dict], SpreadsheetRead]:
     ...
 
 
 @overload
-def read_spreadsheet(
+def read_individual_sheet(
     excel_file: pd.ExcelFile,
     sheet_name: str,
     return_read_info: Literal[False] = False,
     expected_headers: list[str] | None = None,
 ) -> list[dict]:
     ...
 
 
-def read_spreadsheet(
+def read_individual_sheet(
     excel_file: pd.ExcelFile,
     sheet_name: str,
     return_read_info: bool = False,
     expected_headers: list[str] | None = None,
 ) -> tuple[list[dict], SpreadsheetRead] | list[dict]:
     if expected_headers:
         target_row = _get_row_number(load_workbook(excel_file)[sheet_name], expected_headers)
```

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/text.py` & `cognite_neat-0.68.9/cognite/neat/utils/text.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/utils.py` & `cognite_neat-0.68.9/cognite/neat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/utils/xml.py` & `cognite_neat-0.68.9/cognite/neat/utils/xml.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/_exceptions.py` & `cognite_neat-0.68.9/cognite/neat/workflows/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/base.py` & `cognite_neat-0.68.9/cognite/neat/workflows/base.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/cdf_store.py` & `cognite_neat-0.68.9/cognite/neat/workflows/cdf_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Export DMS/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Export DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Export Rules to Ontology/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Extract DEXPI Graph and Export Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Extract RDF Graph and Generate Assets/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Import DMS/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Import DMS/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Ontology to Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Validate Rules/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Validate Rules/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Validate Solution Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Visualize Data Model Using Mock Graph/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml` & `cognite_neat-0.68.9/cognite/neat/workflows/examples/Visualize Semantic Data Model/workflow.yaml`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/manager.py` & `cognite_neat-0.68.9/cognite/neat/workflows/manager.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/migration/steps.py` & `cognite_neat-0.68.9/cognite/neat/workflows/migration/steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/migration/wf_manifests.py` & `cognite_neat-0.68.9/cognite/neat/workflows/migration/wf_manifests.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/model.py` & `cognite_neat-0.68.9/cognite/neat/workflows/model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/data_contracts.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/data_contracts.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_extractor.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_loader.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/graph_store.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/io_steps.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/io_steps.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_exporter.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_importer.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/rules_validator.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/rules_validator.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_extractor.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_extractor.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_loader.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_loader.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_store.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_store.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/graph_transformer.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/rules_exporter.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/rules_exporter.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/lib/v1/rules_importer.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/lib/v1/rules_importer.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps/step_model.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps/step_model.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/steps_registry.py` & `cognite_neat-0.68.9/cognite/neat/workflows/steps_registry.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/tasks.py` & `cognite_neat-0.68.9/cognite/neat/workflows/tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/cognite/neat/workflows/triggers.py` & `cognite_neat-0.68.9/cognite/neat/workflows/triggers.py`

 * *Files identical despite different names*

### Comparing `cognite_neat-0.68.8/pyproject.toml` & `cognite_neat-0.68.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-neat"
-version = "0.68.8"
+version = "0.68.9"
 readme = "README.md"
 description = "Knowledge graph transformation"
 authors = [
     "Nikola Vasiljevic <nikola.vasiljevic@cognite.com>",
     "Anders Albert <anders.albert@cognite.com>",
     "Aleksandrs Livincovs <aleksandrs.livincovs@cognite.com>",
 ]
```

### Comparing `cognite_neat-0.68.8/PKG-INFO` & `cognite_neat-0.68.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-neat
-Version: 0.68.8
+Version: 0.68.9
 Summary: Knowledge graph transformation
 Home-page: https://cognite-neat.readthedocs-hosted.com/
 License: Apache-2.0
 Author: Nikola Vasiljevic
 Author-email: nikola.vasiljevic@cognite.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

