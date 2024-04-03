# Comparing `tmp/graphdatascience-1.8.tar.gz` & `tmp/graphdatascience-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdatascience-1.8.tar", last modified: Tue Oct 10 09:36:18 2023, max compression
+gzip compressed data, was "graphdatascience-1.9.tar", last modified: Wed Jan 17 15:02:48 2024, max compression
```

## Comparing `graphdatascience-1.8.tar` & `graphdatascience-1.9.tar`

### file list

```diff
@@ -1,140 +1,148 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.272594 graphdatascience-1.8/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-10-10 09:33:27.000000 graphdatascience-1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      324 2023-10-10 09:33:27.000000 graphdatascience-1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7533 2023-10-10 09:36:18.272594 graphdatascience-1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5841 2023-10-10 09:33:27.000000 graphdatascience-1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.244593 graphdatascience-1.8/graphdatascience/
--rw-r--r--   0 root         (0) root         (0)      195 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.244593 graphdatascience-1.8/graphdatascience/algo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/algo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      959 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/algo/algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1742 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/algo/algo_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      738 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/algo/single_mode_algo_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/call_builder.py
--rw-r--r--   0 root         (0) root         (0)      812 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/caller_base.py
--rw-r--r--   0 root         (0) root         (0)     2835 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.248593 graphdatascience-1.8/graphdatascience/error/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1233 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/client_only_endpoint.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/cypher_warning_handler.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/endpoint_suggester.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/gds_not_installed.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/illegal_attr_checker.py
--rw-r--r--   0 root         (0) root         (0)       48 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/unable_to_connect.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/error/uncallable_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.252593 graphdatascience-1.8/graphdatascience/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3691 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_alpha_project_runner.py
--rw-r--r--   0 root         (0) root         (0)     1794 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_create_result.py
--rw-r--r--   0 root         (0) root         (0)     4570 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_cypher_runner.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_endpoints.py
--rw-r--r--   0 root         (0) root         (0)    13988 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_entity_ops_runner.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_export_runner.py
--rw-r--r--   0 root         (0) root         (0)     7103 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_object.py
--rw-r--r--   0 root         (0) root         (0)    20929 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_project_runner.py
--rw-r--r--   0 root         (0) root         (0)     2794 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_sample_runner.py
--rw-r--r--   0 root         (0) root         (0)     1643 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/graph_type_check.py
--rw-r--r--   0 root         (0) root         (0)     5526 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/nx_loader.py
--rw-r--r--   0 root         (0) root         (0)    14488 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph/ogb_loader.py
--rw-r--r--   0 root         (0) root         (0)    10569 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/graph_data_science.py
--rw-r--r--   0 root         (0) root         (0)     3480 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/ignored_server_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.252593 graphdatascience-1.8/graphdatascience/model/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1634 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/graphsage_model.py
--rw-r--r--   0 root         (0) root         (0)     1325 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/link_prediction_model.py
--rw-r--r--   0 root         (0) root         (0)     9087 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     5776 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1066 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/model_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2314 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/node_classification_model.py
--rw-r--r--   0 root         (0) root         (0)      773 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/node_regression_model.py
--rw-r--r--   0 root         (0) root         (0)     3297 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/pipeline_model.py
--rw-r--r--   0 root         (0) root         (0)     9823 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/model/simple_rel_embedding_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.256593 graphdatascience-1.8/graphdatascience/pipeline/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/classification_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/lp_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/lp_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/nc_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     1772 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/nc_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      663 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/nr_pipeline_create_runner.py
--rw-r--r--   0 root         (0) root         (0)     2795 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/nr_training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)      444 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/pipeline_alpha_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/pipeline_beta_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     2661 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/pipeline_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2883 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/pipeline_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)     8391 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/pipeline/training_pipeline.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.260594 graphdatascience-1.8/graphdatascience/query_runner/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4385 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/arrow_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)    11748 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/arrow_query_runner.py
--rw-r--r--   0 root         (0) root         (0)     6214 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/aura_db_arrow_query_runner.py
--rw-r--r--   0 root         (0) root         (0)    19215 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/cypher_graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)      243 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/graph_constructor.py
--rw-r--r--   0 root         (0) root         (0)     8594 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/neo4j_query_runner.py
--rw-r--r--   0 root         (0) root         (0)     1412 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/query_runner/query_runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.260594 graphdatascience-1.8/graphdatascience/resources/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.260594 graphdatascience-1.8/graphdatascience/resources/cora/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/cora/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93288 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/cora/cora_nodes.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    26318 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/cora/cora_rels.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)     1024 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/cora/serialize_cora.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.264593 graphdatascience-1.8/graphdatascience/resources/imdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    61198 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_acted_in.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    87832 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_actors.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    29417 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_directed_in.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    34089 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_directors.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    33370 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_movies_with_genre.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    18736 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/imdb_movies_without_genre.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)     3486 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/imdb/serialize_imdb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.264593 graphdatascience-1.8/graphdatascience/resources/karate/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/karate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3397 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/karate/karate_club.parquet.gzip
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.264593 graphdatascience-1.8/graphdatascience/resources/lastfm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126910 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/artist_nodes.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)     5447 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/serialize_lastfm.py
--rw-r--r--   0 root         (0) root         (0)    36340 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/user_friend_df_directed.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)   353081 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/user_listen_artist_rels.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)    13965 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/user_nodes.parquet.gzip
--rw-r--r--   0 root         (0) root         (0)   725313 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/resources/lastfm/user_tag_artist_rels.parquet.gzip
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.268594 graphdatascience-1.8/graphdatascience/server_version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/server_version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/server_version/compatible_with.py
--rw-r--r--   0 root         (0) root         (0)     1244 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/server_version/server_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.268594 graphdatascience-1.8/graphdatascience/system/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/system/config_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     5032 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/system/system_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.272594 graphdatascience-1.8/graphdatascience/topological_lp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/topological_lp/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2295 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/topological_lp/topological_lp_alpha_runner.py
--rw-r--r--   0 root         (0) root         (0)      343 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/topological_lp/topological_lp_endpoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.272594 graphdatascience-1.8/graphdatascience/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3937 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/utils/util_endpoints.py
--rw-r--r--   0 root         (0) root         (0)     2137 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/utils/util_proc_runner.py
--rw-r--r--   0 root         (0) root         (0)       20 2023-10-10 09:33:27.000000 graphdatascience-1.8/graphdatascience/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.244593 graphdatascience-1.8/graphdatascience.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7533 2023-10-10 09:36:18.000000 graphdatascience-1.8/graphdatascience.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5341 2023-10-10 09:36:18.000000 graphdatascience-1.8/graphdatascience.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-10 09:36:18.000000 graphdatascience-1.8/graphdatascience.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-10 09:36:17.000000 graphdatascience-1.8/graphdatascience.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      194 2023-10-10 09:36:18.000000 graphdatascience-1.8/graphdatascience.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-10-10 09:36:18.000000 graphdatascience-1.8/graphdatascience.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-10-10 09:33:27.000000 graphdatascience-1.8/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.240593 graphdatascience-1.8/requirements/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-10 09:36:18.272594 graphdatascience-1.8/requirements/base/
--rw-r--r--   0 root         (0) root         (0)      170 2023-10-10 09:33:27.000000 graphdatascience-1.8/requirements/base/base.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-10-10 09:33:27.000000 graphdatascience-1.8/requirements/base/networkx.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-10-10 09:33:27.000000 graphdatascience-1.8/requirements/base/ogb.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-10 09:36:18.272594 graphdatascience-1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2132 2023-10-10 09:33:27.000000 graphdatascience-1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.923633 graphdatascience-1.9/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-01-17 15:02:16.000000 graphdatascience-1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      324 2024-01-17 15:02:16.000000 graphdatascience-1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7654 2024-01-17 15:02:48.923633 graphdatascience-1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5937 2024-01-17 15:02:16.000000 graphdatascience-1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.883633 graphdatascience-1.9/graphdatascience/
+-rw-r--r--   0 root         (0) root         (0)     1230 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.887633 graphdatascience-1.9/graphdatascience/algo/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/algo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      959 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/algo/algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/algo/algo_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      738 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/algo/single_mode_algo_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/call_builder.py
+-rw-r--r--   0 root         (0) root         (0)      273 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/call_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      872 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/caller_base.py
+-rw-r--r--   0 root         (0) root         (0)     2782 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.887633 graphdatascience-1.9/graphdatascience/error/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/client_only_endpoint.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/cypher_warning_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/endpoint_suggester.py
+-rw-r--r--   0 root         (0) root         (0)       39 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/gds_not_installed.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/illegal_attr_checker.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/unable_to_connect.py
+-rw-r--r--   0 root         (0) root         (0)      568 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/error/uncallable_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.891633 graphdatascience-1.9/graphdatascience/gds_session/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/aura_api.py
+-rw-r--r--   0 root         (0) root         (0)     6368 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/aura_graph_data_science.py
+-rw-r--r--   0 root         (0) root         (0)      267 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/dbms_connection_info.py
+-rw-r--r--   0 root         (0) root         (0)     6755 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/gds_sessions.py
+-rw-r--r--   0 root         (0) root         (0)      283 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/schema.py
+-rw-r--r--   0 root         (0) root         (0)      403 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/gds_session/session_sizes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.895633 graphdatascience-1.9/graphdatascience/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3552 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      644 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_create_result.py
+-rw-r--r--   0 root         (0) root         (0)     4571 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_cypher_runner.py
+-rw-r--r--   0 root         (0) root         (0)      560 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)    13942 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_entity_ops_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_export_runner.py
+-rw-r--r--   0 root         (0) root         (0)     7120 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_object.py
+-rw-r--r--   0 root         (0) root         (0)    21238 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_project_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_sample_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1643 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/graph_type_check.py
+-rw-r--r--   0 root         (0) root         (0)     5526 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/nx_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14488 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph/ogb_loader.py
+-rw-r--r--   0 root         (0) root         (0)     7925 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/graph_data_science.py
+-rw-r--r--   0 root         (0) root         (0)     3480 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/ignored_server_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.899633 graphdatascience-1.9/graphdatascience/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/graphsage_model.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/link_prediction_model.py
+-rw-r--r--   0 root         (0) root         (0)     9480 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model.py
+-rw-r--r--   0 root         (0) root         (0)     1811 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)      798 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     5728 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1066 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/model_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2411 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/node_classification_model.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/node_regression_model.py
+-rw-r--r--   0 root         (0) root         (0)     3297 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/pipeline_model.py
+-rw-r--r--   0 root         (0) root         (0)     7547 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/model/simple_rel_embedding_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.903633 graphdatascience-1.9/graphdatascience/pipeline/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2258 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/classification_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      716 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/lp_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1798 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/lp_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      701 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/nc_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1834 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/nc_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      710 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/nr_pipeline_create_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2883 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/nr_training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      444 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/pipeline_alpha_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/pipeline_beta_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     2661 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/pipeline_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/pipeline_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)     8555 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/pipeline/training_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.907633 graphdatascience-1.9/graphdatascience/query_runner/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/arrow_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)    14992 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     7153 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/aura_db_arrow_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)    19218 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/cypher_graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)      243 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/graph_constructor.py
+-rw-r--r--   0 root         (0) root         (0)    12125 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/neo4j_query_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/query_runner/query_runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.907633 graphdatascience-1.9/graphdatascience/resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.907633 graphdatascience-1.9/graphdatascience/resources/cora/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/cora/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93288 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/cora/cora_nodes.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    26318 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/cora/cora_rels.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)     1024 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/cora/serialize_cora.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.911633 graphdatascience-1.9/graphdatascience/resources/imdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61198 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_acted_in.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    87832 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_actors.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    29417 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_directed_in.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    34089 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_directors.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    33370 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_movies_with_genre.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    18736 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/imdb_movies_without_genre.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)     3486 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/imdb/serialize_imdb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.911633 graphdatascience-1.9/graphdatascience/resources/karate/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/karate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/karate/karate_club.parquet.gzip
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.915633 graphdatascience-1.9/graphdatascience/resources/lastfm/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126910 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/artist_nodes.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)     5447 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/serialize_lastfm.py
+-rw-r--r--   0 root         (0) root         (0)    36340 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/user_friend_df_directed.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)   353081 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/user_listen_artist_rels.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)    13965 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/user_nodes.parquet.gzip
+-rw-r--r--   0 root         (0) root         (0)   725313 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/resources/lastfm/user_tag_artist_rels.parquet.gzip
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.919633 graphdatascience-1.9/graphdatascience/server_version/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/server_version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/server_version/compatible_with.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/server_version/server_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.919633 graphdatascience-1.9/graphdatascience/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/system/config_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     5189 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/system/system_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.919633 graphdatascience-1.9/graphdatascience/topological_lp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/topological_lp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2297 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/topological_lp/topological_lp_alpha_runner.py
+-rw-r--r--   0 root         (0) root         (0)      343 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/topological_lp/topological_lp_endpoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.919633 graphdatascience-1.9/graphdatascience/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/utils/util_endpoints.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/utils/util_proc_runner.py
+-rw-r--r--   0 root         (0) root         (0)       20 2024-01-17 15:02:17.000000 graphdatascience-1.9/graphdatascience/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.923633 graphdatascience-1.9/graphdatascience.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7654 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5645 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      204 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-01-17 15:02:48.000000 graphdatascience-1.9/graphdatascience.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2024-01-17 15:02:17.000000 graphdatascience-1.9/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.879633 graphdatascience-1.9/requirements/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-17 15:02:48.923633 graphdatascience-1.9/requirements/base/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-01-17 15:02:17.000000 graphdatascience-1.9/requirements/base/base.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-01-17 15:02:17.000000 graphdatascience-1.9/requirements/base/networkx.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-01-17 15:02:17.000000 graphdatascience-1.9/requirements/base/ogb.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-17 15:02:48.923633 graphdatascience-1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-01-17 15:02:17.000000 graphdatascience-1.9/setup.py
```

### Comparing `graphdatascience-1.8/LICENSE` & `graphdatascience-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/PKG-INFO` & `graphdatascience-1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.8
+Version: 1.9
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
@@ -26,18 +26,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multimethod<2.0,>=1.0
 Requires-Dist: neo4j<6.0,>=4.4.2
 Requires-Dist: pandas<3.0,>=1.0
-Requires-Dist: pyarrow<14.0,>=4.0
+Requires-Dist: pyarrow<15.0,>=10.0
 Requires-Dist: textdistance<5.0,>=4.0
 Requires-Dist: tqdm<5.0,>=4.0
 Requires-Dist: typing-extensions<5.0,>=4.0
+Requires-Dist: requests
 Provides-Extra: ogb
 Requires-Dist: ogb<2.0,>=1.0; extra == "ogb"
 Provides-Extra: networkx
 Requires-Dist: networkx<4.0,>=2.0; extra == "networkx"
 
 # Neo4j Graph Data Science Client
 
@@ -121,14 +122,15 @@
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
 * [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
 * [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
+* [Perform inference using pre-trained KGE models](examples/kge-predict-transe-pyg-train.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
 The manual is versioned to cover all GDS Python Client versions, so make sure to use the correct version to get the correct information.
```

### Comparing `graphdatascience-1.8/README.md` & `graphdatascience-1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
 * [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
 * [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
+* [Perform inference using pre-trained KGE models](examples/kge-predict-transe-pyg-train.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
 The manual is versioned to cover all GDS Python Client versions, so make sure to use the correct version to get the correct information.
```

### Comparing `graphdatascience-1.8/graphdatascience/algo/algo_endpoints.py` & `graphdatascience-1.9/graphdatascience/algo/algo_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/algo/algo_proc_runner.py` & `graphdatascience-1.9/graphdatascience/algo/algo_proc_runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,23 @@
 
 from pandas import DataFrame, Series
 
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..graph.graph_object import Graph
 from ..graph.graph_type_check import graph_type_check
 from ..model.graphsage_model import GraphSageModel
+from graphdatascience.call_parameters import CallParameters
 
 
 class AlgoProcRunner(IllegalAttrChecker, ABC):
     @graph_type_check
     def _run_procedure(self, G: Graph, config: Dict[str, Any], with_logging: bool = True) -> DataFrame:
-        query = f"CALL {self._namespace}($graph_name, $config)"
+        params = CallParameters(graph_name=G.name(), config=config)
 
-        params: Dict[str, Any] = {}
-        params["graph_name"] = G.name()
-        params["config"] = config
-
-        if with_logging:
-            return self._query_runner.run_query_with_logging(query, params)
-        else:
-            return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params, logging=with_logging)
 
     @graph_type_check
     def estimate(self, G: Graph, **config: Any) -> "Series[Any]":
         self._namespace += "." + "estimate"
         return self._run_procedure(G, config, with_logging=False).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/algo/single_mode_algo_endpoints.py` & `graphdatascience-1.9/graphdatascience/algo/single_mode_algo_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/call_builder.py` & `graphdatascience-1.9/graphdatascience/call_builder.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/caller_base.py` & `graphdatascience-1.9/graphdatascience/caller_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,11 +9,15 @@
 class CallerBase(ABC):
     def __init__(self, query_runner: QueryRunner, namespace: str, server_version: ServerVersion):
         self._query_runner = query_runner
         self._namespace = namespace
         self._server_version = server_version
 
     def _raise_suggestive_error_message(self, requested_endpoint: str) -> NoReturn:
-        list_result = self._query_runner.run_query("CALL gds.list() YIELD name", custom_error=False)
+        list_result = self._query_runner.call_procedure(
+            endpoint="gds.list",
+            yields=["name"],
+            custom_error=False,
+        )
         all_endpoints = list_result["name"].tolist()
 
         raise SyntaxError(generate_suggestive_error_message(requested_endpoint, all_endpoints))
```

### Comparing `graphdatascience-1.8/graphdatascience/endpoints.py` & `graphdatascience-1.9/graphdatascience/endpoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from .algo.single_mode_algo_endpoints import (
     SingleModeAlgoEndpoints,
     SingleModeAlphaAlgoEndpoints,
 )
 from .call_builder import IndirectAlphaCallBuilder, IndirectBetaCallBuilder
-from .graph.graph_endpoints import (
-    GraphAlphaEndpoints,
-    GraphBetaEndpoints,
-    GraphEndpoints,
-)
+from .graph.graph_endpoints import GraphAlphaEndpoints, GraphBetaEndpoints
 from .model.model_endpoints import (
     ModelAlphaEndpoints,
     ModelBetaEndpoints,
     ModelEndpoints,
 )
 from .pipeline.pipeline_endpoints import (
     PipelineAlphaEndpoints,
@@ -35,15 +31,14 @@
 """
 
 
 class DirectEndpoints(
     SingleModeAlgoEndpoints,
     DirectSystemEndpoints,
     DirectUtilEndpoints,
-    GraphEndpoints,
     PipelineEndpoints,
     ModelEndpoints,
     ConfigEndpoints,
 ):
     def __init__(self, query_runner: QueryRunner, namespace: str, server_version: ServerVersion):
         super().__init__(query_runner, namespace, server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/error/client_only_endpoint.py` & `graphdatascience-1.9/graphdatascience/error/client_only_endpoint.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/error/cypher_warning_handler.py` & `graphdatascience-1.9/graphdatascience/error/cypher_warning_handler.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/error/endpoint_suggester.py` & `graphdatascience-1.9/graphdatascience/error/endpoint_suggester.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/error/illegal_attr_checker.py` & `graphdatascience-1.9/graphdatascience/error/illegal_attr_checker.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/error/uncallable_namespace.py` & `graphdatascience-1.9/graphdatascience/error/uncallable_namespace.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_alpha_proc_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_alpha_proc_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from typing import List, Optional, Union
 
 from pandas import DataFrame
 
+from ..call_parameters import CallParameters
 from ..error.client_only_endpoint import client_deprecated, client_only_endpoint
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
-from .graph_alpha_project_runner import GraphAlphaProjectRunner
 from .graph_entity_ops_runner import GraphLabelRunner, GraphPropertyRunner
 from .graph_object import Graph
 from .graph_sample_runner import GraphAlphaSampleRunner
 
 
 class GraphAlphaProcRunner(UncallableNamespace, IllegalAttrChecker):
     @property
@@ -26,19 +26,14 @@
         return GraphPropertyRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
     def nodeLabel(self) -> GraphLabelRunner:
         self._namespace += ".nodeLabel"
         return GraphLabelRunner(self._query_runner, self._namespace, self._server_version)
 
-    @property
-    def project(self) -> GraphAlphaProjectRunner:
-        self._namespace += ".project"
-        return GraphAlphaProjectRunner(self._query_runner, self._namespace, self._server_version)
-
     @client_only_endpoint("gds.alpha.graph")
     @client_deprecated(old_endpoint="gds.alpha.graph.construct", new_endpoint="gds.graph.construct")
     @compatible_with("construct", min_inclusive=ServerVersion(2, 1, 0))
     def construct(
         self,
         graph_name: str,
         nodes: Union[DataFrame, List[DataFrame]],
@@ -47,16 +42,19 @@
         undirected_relationship_types: Optional[List[str]] = None,
     ) -> Graph:
         nodes = nodes if isinstance(nodes, List) else [nodes]
         relationships = relationships if isinstance(relationships, List) else [relationships]
 
         errors = []
 
-        exists = self._query_runner.run_query(
-            f"CALL gds.graph.exists('{graph_name}') YIELD exists", custom_error=False
+        exists = self._query_runner.call_procedure(
+            endpoint="gds.graph.exists",
+            yields=["exists"],
+            params=CallParameters(graph_name=graph_name),
+            custom_error=False,
         ).squeeze()
 
         # compare against True as (1) unit tests return None here and (2) numpys True does not work with `is True`.
         if exists == True:  # noqa: E712
             errors.append(
                 f"Graph '{graph_name}' already exists. Please drop the existing graph or use a different name."
             )
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_alpha_project_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_beta_proc_runner.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,43 @@
-from typing import Any
+from typing import Any, List, Union
 
-from graphdatascience.error.illegal_attr_checker import IllegalAttrChecker
+from ..error.illegal_attr_checker import IllegalAttrChecker
+from ..error.uncallable_namespace import UncallableNamespace
+from .graph_export_runner import GraphExportCsvEndpoints
+from .graph_object import Graph
+from .graph_project_runner import GraphProjectBetaRunner
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.graph.graph_create_result import GraphCreateResult
-from graphdatascience.graph.graph_object import Graph
-from graphdatascience.server_version.compatible_with import compatible_with
-from graphdatascience.server_version.server_version import ServerVersion
+from graphdatascience.graph.graph_entity_ops_runner import GraphRelationshipsBetaRunner
 
+Strings = Union[str, List[str]]
+
+
+class GraphBetaProcRunner(UncallableNamespace, IllegalAttrChecker):
+    @property
+    def project(self) -> GraphProjectBetaRunner:
+        self._namespace += ".project"
+        return GraphProjectBetaRunner(self._query_runner, self._namespace, self._server_version)
+
+    @property
+    def export(self) -> GraphExportCsvEndpoints:
+        self._namespace += ".export"
+        return GraphExportCsvEndpoints(self._query_runner, self._namespace, self._server_version)
+
+    @property
+    def relationships(self) -> GraphRelationshipsBetaRunner:
+        self._namespace += ".relationships"
+        return GraphRelationshipsBetaRunner(self._query_runner, self._namespace, self._server_version)
+
+    def generate(self, graph_name: str, node_count: int, average_degree: int, **config: Any) -> GraphCreateResult:
+        self._namespace += ".generate"
+
+        params = CallParameters(
+            graph_name=graph_name,
+            node_count=node_count,
+            average_degree=average_degree,
+            config=config,
+        )
+
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()
 
-class GraphAlphaProjectRunner(IllegalAttrChecker):
-    @compatible_with("remote", min_inclusive=ServerVersion(2, 4, 0))
-    def remote(self, graph_name: str, query: str, remote_database: str, **config: Any) -> GraphCreateResult:
-        self._namespace += ".remote"
-        procedure_query = f"CALL {self._namespace}($graph_name, $query, $token, $host, $remote_database, $config)"
-        params = {"graph_name": graph_name, "query": query, "remote_database": remote_database, "config": config}
-        result = self._query_runner.run_query(procedure_query, params).squeeze()
         return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_beta_proc_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_export_runner.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-from typing import Any, List, Union
+from typing import Any, Dict
 
+from pandas import Series
+
+from ..call_parameters import CallParameters
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
-from .graph_export_runner import GraphExportCsvEndpoints
 from .graph_object import Graph
-from .graph_project_runner import GraphProjectBetaRunner
-from graphdatascience.graph.graph_create_result import GraphCreateResult
-from graphdatascience.graph.graph_entity_ops_runner import GraphRelationshipsBetaRunner
+from .graph_type_check import graph_type_check
 
-Strings = Union[str, List[str]]
 
+class GraphExportCsvRunner(IllegalAttrChecker):
+    # TODO: Add an integration test for this call.
+    def __call__(self, G: Graph, **config: Any) -> "Series[Any]":
+        return self._export_call(G, config)
 
-class GraphBetaProcRunner(UncallableNamespace, IllegalAttrChecker):
-    @property
-    def project(self) -> GraphProjectBetaRunner:
-        self._namespace += ".project"
-        return GraphProjectBetaRunner(self._query_runner, self._namespace, self._server_version)
+    @graph_type_check
+    def _export_call(self, G: Graph, config: Dict[str, Any]) -> "Series[Any]":
+        params = CallParameters(graph_name=G.name(), config=config)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
+
+    @graph_type_check
+    def estimate(self, G: Graph, **config: Any) -> "Series[Any]":
+        self._namespace += ".estimate"
+
+        return self._export_call(G, config)
 
-    @property
-    def export(self) -> GraphExportCsvEndpoints:
-        self._namespace += ".export"
-        return GraphExportCsvEndpoints(self._query_runner, self._namespace, self._server_version)
 
+class GraphExportCsvEndpoints(UncallableNamespace, IllegalAttrChecker):
     @property
-    def relationships(self) -> GraphRelationshipsBetaRunner:
-        self._namespace += ".relationships"
-        return GraphRelationshipsBetaRunner(self._query_runner, self._namespace, self._server_version)
-
-    def generate(self, graph_name: str, node_count: int, average_degree: int, **config: Any) -> GraphCreateResult:
-        self._namespace += ".generate"
-
-        query = f"CALL {self._namespace}($graph_name, $node_count, $average_degree, $config)"
-        params = {
-            "graph_name": graph_name,
-            "node_count": node_count,
-            "average_degree": average_degree,
-            "config": config,
-        }
+    def csv(self) -> GraphExportCsvRunner:
+        self._namespace += ".csv"
 
-        result = self._query_runner.run_query(query, params).squeeze()
+        return GraphExportCsvRunner(self._query_runner, self._namespace, self._server_version)
+
+
+class GraphExportRunner(IllegalAttrChecker):
+    def __call__(self, G: Graph, **config: Any) -> "Series[Any]":
+        return self._export_call(G, config)
+
+    @graph_type_check
+    def _export_call(self, G: Graph, config: Dict[str, Any]) -> "Series[Any]":
+        params = CallParameters(graph_name=G.name(), config=config)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
+
+    @property
+    def csv(self) -> GraphExportCsvRunner:
+        self._namespace += ".csv"
 
-        return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
+        return GraphExportCsvRunner(self._query_runner, self._namespace, self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_create_result.py` & `graphdatascience-1.9/graphdatascience/graph/graph_create_result.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from __future__ import annotations
+
 from types import TracebackType
-from typing import Any, NamedTuple, Optional, Type, TypeVar
+from typing import Any, NamedTuple, Optional, Type
 
 from pandas import Series
 
 from .graph_object import Graph
 
-TGraphCreateResult = TypeVar("TGraphCreateResult", bound="GraphCreateResult")
-
 
 class GraphCreateResult(NamedTuple):
     """
     A result object returned by endpoints which create graphs.
     """
 
     graph: Graph
     result: "Series[Any]"
 
-    def __enter__(self: TGraphCreateResult) -> Graph:
+    def __enter__(self: GraphCreateResult) -> Graph:
         return self.graph
 
     def __exit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception_value: Optional[BaseException],
         traceback: Optional[TracebackType],
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_cypher_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_cypher_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         Returns
         -------
         A tuple of the projected graph and statistics about the projection
         """
 
         GraphCypherRunner._verify_query_ends_with_return_clause(self._namespace, query)
 
-        result = self._query_runner.run_query(query, params, database, False).squeeze()
+        result = self._query_runner.run_cypher(query, params, database, False).squeeze()
 
         try:
             graph_name = str(result["graphName"])
         except (KeyError, TypeError):
             raise ValueError(
                 f"Invalid query, the query must end with the `RETURN {self._namespace}(...)` call: {query}"
             )
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_endpoints.py` & `graphdatascience-1.9/graphdatascience/graph/graph_endpoints.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 from ..caller_base import CallerBase
 from .graph_alpha_proc_runner import GraphAlphaProcRunner
 from .graph_beta_proc_runner import GraphBetaProcRunner
-from .graph_proc_runner import GraphProcRunner
-
-
-class GraphEndpoints(CallerBase):
-    @property
-    def graph(self) -> GraphProcRunner:
-        return GraphProcRunner(self._query_runner, f"{self._namespace}.graph", self._server_version)
 
 
 class GraphAlphaEndpoints(CallerBase):
     @property
     def graph(self) -> GraphAlphaProcRunner:
         return GraphAlphaProcRunner(self._query_runner, f"{self._namespace}.graph", self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_entity_ops_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_entity_ops_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ..error.uncallable_namespace import UncallableNamespace
 from ..query_runner.query_runner import QueryRunner
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
 from ..utils.util_proc_runner import UtilProcRunner
 from .graph_object import Graph
 from .graph_type_check import graph_type_check
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.error.cypher_warning_handler import (
     filter_id_func_deprecation_warning,
 )
 
 Strings = Union[str, List[str]]
 
 
@@ -44,23 +45,25 @@
     def _handle_properties(
         self,
         G: Graph,
         properties: Strings,
         entities: Strings,
         config: Dict[str, Any],
     ) -> DataFrame:
-        query = f"CALL {self._namespace}($graph_name, $properties, $entities, $config)"
-        params = {
-            "graph_name": G.name(),
-            "properties": properties,
-            "entities": entities,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params)
+        params = CallParameters(
+            graph_name=G.name(),
+            properties=properties,
+            entities=entities,
+            config=config,
+        )
+
+        return self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=params,
+        )
 
 
 class GraphElementPropertyRunner(GraphEntityOpsBaseRunner):
     @compatible_with("stream", min_inclusive=ServerVersion(2, 2, 0))
     def stream(self, G: Graph, node_properties: str, node_labels: Strings = ["*"], **config: Any) -> DataFrame:
         self._namespace += ".stream"
         return self._handle_properties(G, node_properties, node_labels, config)
@@ -80,32 +83,36 @@
     ) -> DataFrame:
         self._namespace += ".stream"
 
         result = self._handle_properties(G, node_properties, node_labels, config)
 
         # new format was requested, but the query was run via Cypher
         if separate_property_columns and "propertyValue" in result.keys():
-            result = result.pivot(index="nodeId", columns="nodeProperty", values="propertyValue")
-            result = result.reset_index()
+            wide_result = result.pivot(index=["nodeId"], columns=["nodeProperty"], values="propertyValue")
+            if "listNodeLabels" in config.keys():
+                # nodeLabels cannot be an index column of the pivot as its not hashable
+                # so we need to manually join it back in
+                labels_df = result[["nodeId", "nodeLabels"]].set_index("nodeId")
+                wide_result = wide_result.join(labels_df, on="nodeId")
+            result = wide_result.reset_index()
             result.columns.name = None
         # old format was requested but the query was run via Arrow
         elif not separate_property_columns and "propertyValue" not in result.keys():
-            result = result.melt(id_vars=["nodeId"]).rename(
-                columns={"variable": "nodeProperty", "value": "propertyValue"}
-            )
+            id_vars = ["nodeId", "nodeLabels"] if config.get("listNodeLabels", False) else ["nodeId"]
+            result = result.melt(id_vars=id_vars).rename(columns={"variable": "nodeProperty", "value": "propertyValue"})
 
         if db_node_properties:
             duplicate_properties = set(db_node_properties).intersection(set(node_properties))
             if duplicate_properties:
                 raise ValueError(
                     f"Duplicate property keys '{duplicate_properties}' in db_node_properties and " f"node_properties."
                 )
 
             unique_node_ids = result["nodeId"].drop_duplicates().tolist()
-            db_properties_df = self._query_runner.run_query(
+            db_properties_df = self._query_runner.run_cypher(
                 self._build_query(db_node_properties), {"ids": unique_node_ids}
             )
 
             if "propertyValue" not in result.keys():
                 result = result.join(db_properties_df.set_index("nodeId"), on="nodeId")
             else:
                 db_properties_df = db_properties_df.melt(id_vars=["nodeId"]).rename(
@@ -129,22 +136,24 @@
         self._namespace += ".write"
         return self._handle_properties(G, node_properties, node_labels, config).squeeze()  # type: ignore
 
     @compatible_with("drop", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def drop(self, G: Graph, node_properties: List[str], **config: Any) -> "Series[Any]":
         self._namespace += ".drop"
-        query = f"CALL {self._namespace}($graph_name, $properties, $config)"
-        params = {
-            "graph_name": G.name(),
-            "properties": node_properties,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(
+            graph_name=G.name(),
+            properties=node_properties,
+            config=config,
+        )
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
 
 class GraphRelationshipPropertiesRunner(GraphEntityOpsBaseRunner):
     @compatible_with("stream", min_inclusive=ServerVersion(2, 2, 0))
     def stream(
         self,
         G: Graph,
@@ -180,111 +189,112 @@
         self,
         G: Graph,
         relationship_type: str,
         relationship_properties: List[str],
         **config: Any,
     ) -> "Series[Any]":
         self._namespace += ".write"
-
-        query = f"CALL {self._namespace}($graph_name, $relationship_type, $relationship_properties, $config)"
-        params = {
-            "graph_name": G.name(),
-            "relationship_type": relationship_type,
-            "relationship_properties": relationship_properties,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(
+            graph_name=G.name(),
+            relationship_type=relationship_type,
+            relationship_properties=relationship_properties,
+            config=config,
+        )
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
 
 class GraphRelationshipRunner(GraphEntityOpsBaseRunner):
     @compatible_with("write", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def write(self, G: Graph, relationship_type: str, relationship_property: str = "", **config: Any) -> "Series[Any]":
         self._namespace += ".write"
-        query = f"CALL {self._namespace}($graph_name, $relationship_type, $relationship_property, $config)"
-        params = {
-            "graph_name": G.name(),
-            "relationship_type": relationship_type,
-            "relationship_property": relationship_property,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(
+            graph_name=G.name(),
+            relationship_type=relationship_type,
+            relationship_property=relationship_property,
+            config=config,
+        )
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
 
 class ToUndirectedRunner(IllegalAttrChecker):
     def _run_procedure(
-        self, G: Graph, query: str, relationship_type: str, mutate_relationship_type: str, **config: Any
+        self, G: Graph, relationship_type: str, mutate_relationship_type: str, **config: Any
     ) -> "Series[Any]":
         actual_config = {
             **config,
             "relationshipType": relationship_type,
             "mutateRelationshipType": mutate_relationship_type,
         }
 
-        params = {"graph_name": G.name(), "config": actual_config}
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(graph_name=G.name(), config=actual_config)
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
     @graph_type_check
     def __call__(self, G: Graph, relationship_type: str, mutate_relationship_type: str, **config: Any) -> "Series[Any]":
-        query = f"CALL {self._namespace}($graph_name, $config)"
-        return self._run_procedure(G, query, relationship_type, mutate_relationship_type)
+        return self._run_procedure(G, relationship_type, mutate_relationship_type)
 
     @graph_type_check
     @compatible_with("estimate", min_inclusive=ServerVersion(2, 3, 0))
     def estimate(self, G: Graph, relationship_type: str, mutate_relationship_type: str, **config: Any) -> "Series[Any]":
-        query = f"CALL {self._namespace}.estimate($graph_name, $config)"
-        return self._run_procedure(G, query, relationship_type, mutate_relationship_type)
+        self._namespace += ".estimate"
+        return self._run_procedure(G, relationship_type, mutate_relationship_type)
 
 
 class GraphRelationshipsRunner(GraphEntityOpsBaseRunner):
     @compatible_with("drop", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def drop(
         self,
         G: Graph,
         relationship_type: str,
     ) -> "Series[Any]":
         self._namespace += ".drop"
-        query = f"CALL {self._namespace}($graph_name, $relationship_type)"
-        params = {
-            "graph_name": G.name(),
-            "relationship_type": relationship_type,
-        }
+        params = CallParameters(
+            graph_name=G.name(),
+            relationship_type=relationship_type,
+        )
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
 
     @compatible_with("stream", min_inclusive=ServerVersion(2, 5, 0))
     @graph_type_check
     def stream(self, G: Graph, relationship_types: List[str] = ["*"], **config: Any) -> TopologyDataFrame:
         self._namespace += ".stream"
-        query = f"CALL {self._namespace}($graph_name, $relationship_types, $config)"
+        params = CallParameters(graph_name=G.name(), relationship_types=relationship_types, config=config)
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
-        params = {"graph_name": G.name(), "relationship_types": relationship_types, "config": config}
-
-        return TopologyDataFrame(self._query_runner.run_query(query, params))
+        return TopologyDataFrame(result)
 
     @property
     @compatible_with("toUndirected", min_inclusive=ServerVersion(2, 5, 0))
     def toUndirected(self) -> ToUndirectedRunner:
         self._namespace += ".toUndirected"
         return ToUndirectedRunner(self._query_runner, self._namespace, self._server_version)
 
 
 class GraphRelationshipsBetaRunner(GraphEntityOpsBaseRunner):
     @compatible_with("stream", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def stream(self, G: Graph, relationship_types: List[str] = ["*"], **config: Any) -> TopologyDataFrame:
         self._namespace += ".stream"
-        query = f"CALL {self._namespace}($graph_name, $relationship_types, $config)"
-
-        params = {"graph_name": G.name(), "relationship_types": relationship_types, "config": config}
+        params = CallParameters(graph_name=G.name(), relationship_types=relationship_types, config=config)
 
-        return TopologyDataFrame(self._query_runner.run_query(query, params))
+        return TopologyDataFrame(self._query_runner.call_procedure(endpoint=self._namespace, params=params))
 
     @property
     @compatible_with("toUndirected", min_inclusive=ServerVersion(2, 3, 0))
     def toUndirected(self) -> ToUndirectedRunner:
         self._namespace += ".toUndirected"
         return ToUndirectedRunner(self._query_runner, self._namespace, self._server_version)
 
@@ -295,53 +305,41 @@
     def stream(
         self,
         G: Graph,
         graph_property: str,
         **config: Any,
     ) -> DataFrame:
         self._namespace += ".stream"
-        query = f"CALL {self._namespace}($graph_name, $graph_property, $config)"
-        params = {"graph_name": G.name(), "graph_property": graph_property, "config": config}
+        params = CallParameters(graph_name=G.name(), graph_property=graph_property, config=config)
 
-        return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
     @compatible_with("drop", min_inclusive=ServerVersion(2, 2, 0))
     @graph_type_check
     def drop(
         self,
         G: Graph,
         graph_property: str,
         **config: Any,
     ) -> "Series[Any]":
         self._namespace += ".drop"
-        query = f"CALL {self._namespace}($graph_name, $graph_property, $config)"
-        params = {"graph_name": G.name(), "graph_property": graph_property, "config": config}
+        params = CallParameters(graph_name=G.name(), graph_property=graph_property, config=config)
 
-        return self._query_runner.run_query(query, params)  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params)  # type: ignore
 
 
 class GraphLabelRunner(GraphEntityOpsBaseRunner):
     @compatible_with("write", min_inclusive=ServerVersion(2, 3, 0))
     @graph_type_check
     def write(self, G: Graph, node_label: str, **config: Any) -> "Series[Any]":
         self._namespace += ".write"
-        query = f"CALL {self._namespace}($graph_name, $node_label, $config)"
-        params = {
-            "graph_name": G.name(),
-            "node_label": node_label,
-            "config": config,
-        }
+        params = CallParameters(graph_name=G.name(), node_label=node_label, config=config)
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
 
     @compatible_with("mutate", min_inclusive=ServerVersion(2, 3, 0))
     @graph_type_check
     def mutate(self, G: Graph, node_label: str, **config: Any) -> "Series[Any]":
         self._namespace += ".mutate"
-        query = f"CALL {self._namespace}($graph_name, $node_label, $config)"
-        params = {
-            "graph_name": G.name(),
-            "node_label": node_label,
-            "config": config,
-        }
+        params = CallParameters(graph_name=G.name(), node_label=node_label, config=config)
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_object.py` & `graphdatascience-1.9/graphdatascience/graph/graph_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 from types import TracebackType
-from typing import Any, List, Optional, Type, TypeVar, Union
+from typing import Any, List, Optional, Type, Union
 
 from pandas import Series
 
 from ..query_runner.query_runner import QueryRunner
 from ..server_version.server_version import ServerVersion
-
-TGraph = TypeVar("TGraph", bound="Graph")
+from graphdatascience.call_parameters import CallParameters
 
 
 class Graph:
     """
     A graph object that represents a graph in the graph catalog.
     It can be passed into algorithm endpoints to compute over the corresponding graph.
     It contains summary information about the graph.
@@ -18,15 +19,15 @@
 
     def __init__(self, name: str, query_runner: QueryRunner, server_version: ServerVersion):
         self._name = name
         self._query_runner = query_runner
         self._db = query_runner.database()
         self._server_version = server_version
 
-    def __enter__(self: TGraph) -> TGraph:
+    def __enter__(self: Graph) -> Graph:
         return self
 
     def __exit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception_value: Optional[BaseException],
         traceback: Optional[TracebackType],
@@ -39,18 +40,20 @@
             the name of the graph
         """
         return self._name
 
     def _graph_info(self, yields: List[str] = []) -> "Series[Any]":
         yield_db = "database" in yields
         yields_with_db = yields if yield_db else yields + ["database"]
-        yield_suffix = "" if len(yields) == 0 else " YIELD " + ", ".join(yields_with_db)
 
-        info = self._query_runner.run_query(
-            f"CALL gds.graph.list($graph_name){yield_suffix}", {"graph_name": self._name}, custom_error=False
+        info = self._query_runner.call_procedure(
+            endpoint="gds.graph.list",
+            params=CallParameters(graph_name=self._name),
+            yields=yields_with_db,
+            custom_error=False,
         )
 
         if len(info) == 0:
             raise ValueError(f"There is no projected graph named '{self.name()}'")
         if len(info) > 1:
             # for multiple dbs we can have the same graph name. But db + graph name is unique
             info = info[info["database"] == self._db]
@@ -169,33 +172,33 @@
         return self._graph_info(["sizeInBytes"])  # type: ignore
 
     def exists(self) -> bool:
         """
         Returns:
             whether the graph exists
         """
-        result = self._query_runner.run_query(
-            "CALL gds.graph.exists($graph_name)",
-            {"graph_name": self._name},
+        result = self._query_runner.call_procedure(
+            endpoint="gds.graph.exists",
+            params=CallParameters(graph_name=self._name),
             custom_error=False,
         )
         return result.squeeze()["exists"]  # type: ignore
 
     def drop(self, failIfMissing: bool = False) -> "Series[str]":
         """
         Args:
             failIfMissing: whether to fail if the graph does not exist
 
         Returns:
             the result of the drop operation
 
         """
-        result = self._query_runner.run_query(
-            "CALL gds.graph.drop($graph_name, $fail_if_missing)",
-            {"graph_name": self._name, "fail_if_missing": failIfMissing},
+        result = self._query_runner.call_procedure(
+            endpoint="gds.graph.drop",
+            params=CallParameters(graph_name=self._name, failIfMissing=failIfMissing),
             custom_error=False,
         )
 
         return result.squeeze()  # type: ignore
 
     def creation_time(self) -> Any:  # neo4j.time.DateTime not exported
         """
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_proc_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_proc_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,31 +20,32 @@
     GraphPropertyRunner,
     GraphRelationshipPropertiesRunner,
     GraphRelationshipRunner,
     GraphRelationshipsRunner,
 )
 from .graph_export_runner import GraphExportRunner
 from .graph_object import Graph
-from .graph_project_runner import GraphProjectRunner
+from .graph_project_runner import GraphProjectRemoteRunner, GraphProjectRunner
 from .graph_sample_runner import GraphSampleRunner
 from .graph_type_check import (
     from_graph_type_check,
     graph_type_check,
     graph_type_check_optional,
 )
 from .ogb_loader import OGBLLoader, OGBNLoader
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.graph.graph_create_result import GraphCreateResult
 from graphdatascience.graph.graph_cypher_runner import GraphCypherRunner
 
 Strings = Union[str, List[str]]
 
 is_neo4j_4_driver = ServerVersion.from_string(neo4j_driver_version) < ServerVersion(5, 0, 0)
 
 
-class GraphProcRunner(UncallableNamespace, IllegalAttrChecker):
+class BaseGraphProcRunner(UncallableNamespace, IllegalAttrChecker):
     @staticmethod
     def _path(package: str, resource: str) -> pathlib.Path:
         if sys.version_info >= (3, 9):
             from importlib.resources import files
 
             # files() returns a Traversable, but usages require a Path object
             return pathlib.Path(str(files(package) / resource))
@@ -73,16 +74,19 @@
 
         # Filter empty dataframes
         nodes = [df for df in nodes if not df.empty]
         relationships = [df for df in relationships if not df.empty]
 
         errors = []
 
-        exists = self._query_runner.run_query(
-            f"CALL gds.graph.exists('{graph_name}') YIELD exists", custom_error=False
+        exists = self._query_runner.call_procedure(
+            endpoint="gds.graph.exists",
+            params=CallParameters(graph_name=graph_name),
+            yields=["exists"],
+            custom_error=False,
         ).squeeze()
 
         # compare against True as (1) unit tests return None here and (2) numpys True does not work with `is True`.
         if exists == True:  # noqa: E712
             errors.append(
                 f"Graph '{graph_name}' already exists. Please drop the existing graph or use a different name."
             )
@@ -210,71 +214,61 @@
                 "You can add NetworkX support by running `pip install graphdatascience[networkx]`"
             )
 
         self._namespace += ".networkx"
         return NXLoader(self._query_runner, self._namespace, self._server_version)
 
     @property
-    def project(self) -> GraphProjectRunner:
-        self._namespace += ".project"
-        return GraphProjectRunner(self._query_runner, self._namespace, self._server_version)
-
-    @property
     @compatible_with("graphProperty", min_inclusive=ServerVersion(2, 5, 0))
     def graphProperty(self) -> GraphPropertyRunner:
         self._namespace += ".graphProperty"
         return GraphPropertyRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
     @compatible_with("nodeLabel", min_inclusive=ServerVersion(2, 5, 0))
     def nodeLabel(self) -> GraphLabelRunner:
         self._namespace += ".nodeLabel"
         return GraphLabelRunner(self._query_runner, self._namespace, self._server_version)
 
-    @property
-    def cypher(self) -> GraphCypherRunner:
-        self._namespace += ".project"
-        return GraphCypherRunner(self._query_runner, self._namespace, self._server_version)
-
     @compatible_with("generate", min_inclusive=ServerVersion(2, 5, 0))
     def generate(self, graph_name: str, node_count: int, average_degree: int, **config: Any) -> GraphCreateResult:
         self._namespace += ".generate"
+        params = CallParameters(
+            graph_name=graph_name, node_count=node_count, average_degree=average_degree, config=config
+        )
 
-        query = f"CALL {self._namespace}($graph_name, $node_count, $average_degree, $config)"
-        params = {
-            "graph_name": graph_name,
-            "node_count": node_count,
-            "average_degree": average_degree,
-            "config": config,
-        }
-
-        result = self._query_runner.run_query(query, params).squeeze()
+        result = self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
         return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
 
     @from_graph_type_check
     @compatible_with("filter", min_inclusive=ServerVersion(2, 5, 0))
     def filter(
         self,
         graph_name: str,
         from_G: Graph,
         node_filter: str,
         relationship_filter: str,
         **config: Any,
     ) -> GraphCreateResult:
         self._namespace += ".filter"
-        result = self._query_runner.run_query_with_logging(
-            f"CALL {self._namespace}($graph_name, $from_graph_name, $node_filter, $relationship_filter, $config)",
-            {
-                "graph_name": graph_name,
-                "from_graph_name": from_G.name(),
-                "node_filter": node_filter,
-                "relationship_filter": relationship_filter,
-                "config": config,
-            },
+        params = CallParameters(
+            graph_name=graph_name,
+            from_graph_name=from_G.name(),
+            node_filter=node_filter,
+            relationship_filter=relationship_filter,
+            config=config,
+        )
+        result = self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            logging=True,
+            params=params,
         ).squeeze()
 
         return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
 
     @property
     def export(self) -> GraphExportRunner:
         self._namespace += ".export"
@@ -286,64 +280,72 @@
         return OGBNLoader(self._query_runner, self._namespace, self._server_version)
 
     @property
     def ogbl(self) -> OGBLLoader:
         self._namespace += ".ogbl"
         return OGBLLoader(self._query_runner, self._namespace, self._server_version)
 
-    @graph_type_check
     def drop(
         self,
-        G: Graph,
+        graph: Union[Graph, str],
         failIfMissing: bool = False,
         dbName: str = "",
         username: Optional[str] = None,
     ) -> Optional["Series[Any]"]:
         self._namespace += ".drop"
 
-        params = {
-            "graph_name": G.name(),
-            "fail_if_missing": failIfMissing,
-            "db_name": dbName,
-        }
+        if isinstance(graph, Graph):
+            graph = graph.name()
+
+        params = CallParameters(
+            graph_name=graph,
+            fail_if_missing=failIfMissing,
+            db_name=dbName,
+        )
         if username:
-            query = f"CALL {self._namespace}($graph_name, $fail_if_missing, $db_name, $username)"
             params["username"] = username
-        else:
-            query = f"CALL {self._namespace}($graph_name, $fail_if_missing, $db_name)"
 
-        result = self._query_runner.run_query(query, params)
+        result = self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=params,
+        )
         if not result.empty:
             return result.squeeze()  # type: ignore
 
         return None
 
     def exists(self, graph_name: str) -> "Series[Any]":
         self._namespace += ".exists"
-        result = self._query_runner.run_query(f"CALL {self._namespace}($graph_name)", {"graph_name": graph_name})
+        result = self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=CallParameters(graph_name=graph_name),
+        )
 
         return result.squeeze()  # type: ignore
 
     @graph_type_check_optional
     def list(self, G: Optional[Graph] = None) -> DataFrame:
         self._namespace += ".list"
 
+        params = CallParameters()
         if G:
-            query = f"CALL {self._namespace}($graph_name)"
-            params = {"graph_name": G.name()}
-        else:
-            query = "CALL gds.graph.list()"
-            params = {}
+            params["graph_name"] = G.name()
 
-        return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=params,
+        )
 
     @client_only_endpoint("gds.graph")
     def get(self, graph_name: str) -> Graph:
-        result = self._query_runner.run_query(
-            f"CALL gds.graph.list('{graph_name}') YIELD graphName", custom_error=False
+        result = self._query_runner.call_procedure(
+            endpoint="gds.graph.list",
+            params=CallParameters(graph_name=graph_name),
+            yields=["graphName"],
+            custom_error=False,
         )
         if len(result["graphName"]) == 0:
             raise ValueError(
                 f"No projected graph named '{graph_name}' exists in current database '{self._query_runner.database()}'"
             )
 
         return Graph(graph_name, self._query_runner, self._server_version)
@@ -352,23 +354,25 @@
     def _handle_properties(
         self,
         G: Graph,
         properties: Strings,
         entities: Strings,
         config: Dict[str, Any],
     ) -> DataFrame:
-        query = f"CALL {self._namespace}($graph_name, $properties, $entities, $config)"
-        params = {
-            "graph_name": G.name(),
-            "properties": properties,
-            "entities": entities,
-            "config": config,
-        }
+        params = CallParameters(
+            graph_name=G.name(),
+            properties=properties,
+            entities=entities,
+            config=config,
+        )
 
-        return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=params,
+        )
 
     @property
     def nodeProperty(self) -> GraphElementPropertyRunner:
         self._namespace += ".nodeProperty"
         return GraphElementPropertyRunner(self._query_runner, self._namespace, self._server_version)
 
     @property
@@ -487,47 +491,49 @@
         self,
         G: Graph,
         relationship_type: str,
         relationship_property: str = "",
         **config: Any,
     ) -> "Series[Any]":
         self._namespace += ".writeRelationship"
+        params = CallParameters(
+            graph_name=G.name(),
+            relationship_type=relationship_type,
+            relationship_property=relationship_property,
+            config=config,
+        )
 
-        query = f"CALL {self._namespace}($graph_name, $relationship_type, $relationship_property, $config)"
-        params = {
-            "graph_name": G.name(),
-            "relationship_type": relationship_type,
-            "relationship_property": relationship_property,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
     @multimethod
     def removeNodeProperties(self) -> None:
         ...
 
     @removeNodeProperties.register
     @graph_type_check
     def _(
         self,
         G: Graph,
         node_properties: List[str],
         **config: Any,
     ) -> Series:  # type: ignore
         self._namespace += ".removeNodeProperties"
+        params = CallParameters(
+            graph_name=G.name(),
+            properties=node_properties,
+            config=config,
+        )
 
-        query = f"CALL {self._namespace}($graph_name, $properties, $config)"
-        params = {
-            "graph_name": G.name(),
-            "properties": node_properties,
-            "config": config,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
     @removeNodeProperties.register
     @compatible_with("removeNodeProperties", max_exclusive=ServerVersion(2, 1, 0))
     @graph_type_check
     def _(
         self,
         G: Graph,
@@ -539,14 +545,35 @@
 
         return self._handle_properties(G, node_properties, node_labels, config).squeeze()  # type: ignore
 
     @graph_type_check
     def deleteRelationships(self, G: Graph, relationship_type: str) -> "Series[Any]":
         self._namespace += ".deleteRelationships"
 
-        query = f"CALL {self._namespace}($graph_name, $relationship_type)"
-        params = {
-            "graph_name": G.name(),
-            "relationship_type": relationship_type,
-        }
+        params = CallParameters(
+            graph_name=G.name(),
+            relationship_type=relationship_type,
+        )
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
+
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+class GraphProcRunner(BaseGraphProcRunner):
+    @property
+    def project(self) -> GraphProjectRunner:
+        self._namespace += ".project"
+        return GraphProjectRunner(self._query_runner, self._namespace, self._server_version)
+
+    @property
+    def cypher(self) -> GraphCypherRunner:
+        self._namespace += ".project"
+        return GraphCypherRunner(self._query_runner, self._namespace, self._server_version)
+
+
+class GraphRemoteProcRunner(BaseGraphProcRunner):
+    @property
+    def project(self) -> GraphProjectRemoteRunner:
+        self._namespace += ".project.remoteDb"
+        return GraphProjectRemoteRunner(self._query_runner, self._namespace, self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_sample_runner.py` & `graphdatascience-1.9/graphdatascience/graph/graph_sample_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pandas import Series
 
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
 from .graph_object import Graph
 from .graph_type_check import from_graph_type_check
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.graph.graph_create_result import GraphCreateResult
 
 
 class GraphAlphaSampleRunner(IllegalAttrChecker):
     @compatible_with("construct", min_inclusive=ServerVersion(2, 2, 0))
     @from_graph_type_check
     def rwr(self, graph_name: str, from_G: Graph, **config: Any) -> GraphCreateResult:
@@ -28,45 +29,42 @@
         return CNARWRunner(self._query_runner, self._namespace + ".cnarw", self._server_version)
 
 
 class RWRRunner(IllegalAttrChecker):
     @compatible_with("construct", min_inclusive=ServerVersion(2, 2, 0))
     @from_graph_type_check
     def __call__(self, graph_name: str, from_G: Graph, **config: Any) -> GraphCreateResult:
-        query = f"CALL {self._namespace}($graph_name, $from_graph_name, $config)"
-        params = {
-            "graph_name": graph_name,
-            "from_graph_name": from_G.name(),
-            "config": config,
-        }
+        params = CallParameters(
+            graph_name=graph_name,
+            from_graph_name=from_G.name(),
+            config=config,
+        )
 
-        result = self._query_runner.run_query_with_logging(query, params).squeeze()
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params, logging=True).squeeze()
 
         return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
 
 
 class CNARWRunner(IllegalAttrChecker):
     @compatible_with("construct", min_inclusive=ServerVersion(2, 4, 0))
     @from_graph_type_check
     def __call__(self, graph_name: str, from_G: Graph, **config: Any) -> GraphCreateResult:
-        query = f"CALL {self._namespace}($graph_name, $from_graph_name, $config)"
-        params = {
-            "graph_name": graph_name,
-            "from_graph_name": from_G.name(),
-            "config": config,
-        }
-
-        result = self._query_runner.run_query_with_logging(query, params).squeeze()
+        params = CallParameters(
+            graph_name=graph_name,
+            from_graph_name=from_G.name(),
+            config=config,
+        )
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params, logging=True).squeeze()
 
         return GraphCreateResult(Graph(graph_name, self._query_runner, self._server_version), result)
 
     def estimate(self, from_G: Graph, **config: Any) -> "Series[Any]":
         self._namespace += ".estimate"
-        result = self._query_runner.run_query(
-            f"CALL {self._namespace}($from_graph_name, $config)",
-            {
-                "from_graph_name": from_G.name(),
-                "config": config,
-            },
+        result = self._query_runner.call_procedure(
+            endpoint=self._namespace,
+            params=CallParameters(
+                from_graph_name=from_G.name(),
+                config=config,
+            ),
         )
 
         return result.squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/graph/graph_type_check.py` & `graphdatascience-1.9/graphdatascience/graph/graph_type_check.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/graph/nx_loader.py` & `graphdatascience-1.9/graphdatascience/graph/nx_loader.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/graph/ogb_loader.py` & `graphdatascience-1.9/graphdatascience/graph/ogb_loader.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/graph_data_science.py` & `graphdatascience-1.9/graphdatascience/graph_data_science.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-import warnings
-from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union
+from __future__ import annotations
 
-from neo4j import Driver, GraphDatabase
-from pandas import DataFrame, Series
+from typing import Any, Dict, Optional, Tuple, Type, Union
+
+from neo4j import Driver
+from pandas import DataFrame
 
 from .call_builder import IndirectCallBuilder
 from .endpoints import AlphaEndpoints, BetaEndpoints, DirectEndpoints
-from .error.gds_not_installed import GdsNotFound
-from .error.unable_to_connect import UnableToConnectError
 from .error.uncallable_namespace import UncallableNamespace
 from .query_runner.arrow_query_runner import ArrowQueryRunner
 from .query_runner.neo4j_query_runner import Neo4jQueryRunner
 from .query_runner.query_runner import QueryRunner
 from .server_version.server_version import ServerVersion
-from .version import __version__
-from graphdatascience.query_runner.aura_db_arrow_query_runner import (
-    AuraDbArrowQueryRunner,
-    AuraDbConnectionInfo,
-)
-
-GDS = TypeVar("GDS", bound="GraphDataScience")
+from graphdatascience.graph.graph_proc_runner import GraphProcRunner
 
 
 class GraphDataScience(DirectEndpoints, UncallableNamespace):
     """
     Primary API class for the Neo4j Graph Data Science Python Client.
     Always bind this object to a variable called `gds`.
     """
 
-    _AURA_DS_PROTOCOL = "neo4j+s"
-
     def __init__(
         self,
         endpoint: Union[str, Driver, QueryRunner],
         auth: Optional[Tuple[str, str]] = None,
         aura_ds: bool = False,
         database: Optional[str] = None,
         arrow: bool = True,
         arrow_disable_server_verification: bool = True,
         arrow_tls_root_certs: Optional[bytes] = None,
-        aura_db_connection_info: Optional[AuraDbConnectionInfo] = None,
         bookmarks: Optional[Any] = None,
     ):
         """
         Construct a new GraphDataScience object.
 
         Parameters
         ----------
@@ -65,90 +55,40 @@
             other TLS settings are overridden.
         arrow_tls_root_certs : Optional[bytes], default None
             PEM-encoded certificates that are used for the connecting to the
             Arrow Flight server.
         bookmarks : Optional[Any], default None
             The Neo4j bookmarks to require a certain state before the next query gets executed.
         """
+        if aura_ds:
+            GraphDataScience._validate_endpoint(endpoint)
 
-        if isinstance(endpoint, str):
-            self._config: Dict[str, Any] = {"user_agent": f"neo4j-graphdatascience-v{__version__}"}
-
-            if aura_ds:
-                self._configure_aura(endpoint, self._config)
-
-            driver = GraphDatabase.driver(endpoint, auth=auth, **self._config)
-
-            self._query_runner = Neo4jQueryRunner(driver, auto_close=True, bookmarks=bookmarks)
-
-        elif isinstance(endpoint, QueryRunner):
-            if arrow:
-                raise ValueError("Arrow cannot be used if the QueryRunner is provided directly")
-
+        if isinstance(endpoint, QueryRunner):
             self._query_runner = endpoint
-
         else:
-            driver = endpoint
-            self._query_runner = Neo4jQueryRunner(driver, auto_close=False, bookmarks=bookmarks)
-
-        if database:
-            self._query_runner.set_database(database)
-
-        try:
-            server_version_string = self._query_runner.run_query("RETURN gds.version()", custom_error=False).squeeze()
-        except Exception as e:
-            if "Unknown function 'gds.version'" in str(e):
-                # Some Python versions appear to not call __del__ of self._query_runner when an exception
-                # is raised, so we have to close the driver manually.
-                if isinstance(endpoint, str):
-                    driver.close()
-
-                raise GdsNotFound(
-                    """The Graph Data Science library is not correctly installed on the Neo4j server.
-                    Please refer to https://neo4j.com/docs/graph-data-science/current/installation/.
-                    """
-                )
+            self._query_runner = Neo4jQueryRunner.create(endpoint, auth, aura_ds, database, bookmarks)
 
-            raise UnableToConnectError(e)
-
-        self._server_version = ServerVersion.from_string(server_version_string)
-        self._query_runner.set_server_version(self._server_version)
+        self._server_version = self._query_runner.server_version()
 
         if arrow and self._server_version >= ServerVersion(2, 1, 0):
-            yield_fields = (
-                "running, listenAddress"
-                if self._server_version >= ServerVersion(2, 2, 1)
-                else "running, advertisedListenAddress"
+            self._query_runner = ArrowQueryRunner.create(
+                self._query_runner,
+                auth,
+                self._query_runner.encrypted(),
+                arrow_disable_server_verification,
+                arrow_tls_root_certs,
             )
-            arrow_info: "Series[Any]" = self._query_runner.run_query(
-                f"CALL gds.debug.arrow() YIELD {yield_fields}", custom_error=False
-            ).squeeze()
-            listen_address: str = arrow_info.get("advertisedListenAddress", arrow_info["listenAddress"])  # type: ignore
-            if arrow_info["running"]:
-                self._query_runner = ArrowQueryRunner(
-                    listen_address,
-                    self._query_runner,
-                    self._server_version,
-                    auth,
-                    driver.encrypted,
-                    arrow_disable_server_verification,
-                    arrow_tls_root_certs,
-                )
-        if aura_db_connection_info:
-            if self._server_version >= ServerVersion(2, 4, 0):
-                self._query_runner = AuraDbArrowQueryRunner(self._query_runner, aura_db_connection_info)
-            else:
-                warnings.warn(
-                    f"AuraDB connection info was provided but GDS version {self._server_version} \
-                        does not support connecting to AuraDB"
-                )
 
         super().__init__(self._query_runner, "gds", self._server_version)
 
     @property
+    def graph(self) -> GraphProcRunner:
+        return GraphProcRunner(self._query_runner, f"{self._namespace}.graph", self._server_version)
+
+    @property
     def alpha(self) -> AlphaEndpoints:
         return AlphaEndpoints(self._query_runner, "gds.alpha", self._server_version)
 
     @property
     def beta(self) -> BetaEndpoints:
         return BetaEndpoints(self._query_runner, "gds.beta", self._server_version)
 
@@ -226,28 +166,28 @@
         """
         qr = self._query_runner
 
         # The Arrow query runner should not be used to execute arbitrary Cypher
         if isinstance(self._query_runner, ArrowQueryRunner):
             qr = self._query_runner.fallback_query_runner()
 
-        return qr.run_query(query, params, database, False)
+        return qr.run_cypher(query, params, database, False)
 
     def driver_config(self) -> Dict[str, Any]:
         """
         Get the configuration used to create the underlying driver used to make queries to Neo4j.
 
         Returns:
             The configuration as a dictionary.
         """
-        return self._config
+        return self._query_runner.driver_config()
 
     @classmethod
     def from_neo4j_driver(
-        cls: Type[GDS],
+        cls: Type[GraphDataScience],
         driver: Driver,
         auth: Optional[Tuple[str, str]] = None,
         database: Optional[str] = None,
         arrow: bool = True,
         arrow_disable_server_verification: bool = True,
         arrow_tls_root_certs: Optional[bytes] = None,
         bookmarks: Optional[Any] = None,
@@ -258,24 +198,24 @@
             database=database,
             arrow=arrow,
             arrow_disable_server_verification=arrow_disable_server_verification,
             arrow_tls_root_certs=arrow_tls_root_certs,
             bookmarks=bookmarks,
         )
 
+    @staticmethod
+    def _validate_endpoint(endpoint: Union[str, Driver, QueryRunner]) -> None:
+        if isinstance(endpoint, str):
+            protocol = endpoint.split(":")[0]
+            if protocol != Neo4jQueryRunner._AURA_DS_PROTOCOL:
+                raise ValueError(
+                    (
+                        f"AuraDS requires using the '{Neo4jQueryRunner._AURA_DS_PROTOCOL}'"
+                        f" protocol ('{protocol}' was provided)",
+                    )
+                )
+
     def close(self) -> None:
         """
         Close the GraphDataScience object and release any resources held by it.
         """
         self._query_runner.close()
-
-    @classmethod
-    def _configure_aura(cls, uri: str, config: Dict[str, Any]) -> None:
-        protocol = uri.split(":")[0]
-        if not protocol == cls._AURA_DS_PROTOCOL:
-            raise ValueError(
-                f"AuraDS requires using the '{cls._AURA_DS_PROTOCOL}' protocol ('{protocol}' was provided)"
-            )
-
-        config["max_connection_lifetime"] = 60 * 8  # 8 minutes
-        config["keep_alive"] = True
-        config["max_connection_pool_size"] = 50
```

### Comparing `graphdatascience-1.8/graphdatascience/ignored_server_endpoints.py` & `graphdatascience-1.9/graphdatascience/ignored_server_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/model/link_prediction_model.py` & `graphdatascience-1.9/graphdatascience/model/link_prediction_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 class LPModel(PipelineModel):
     """
     Represents a link prediction model in the model catalog.
     Construct this using
     :func:`LPTrainingPipeline.train() <graphdatascience.pipeline.lp_training_pipeline.LPTrainingPipeline.train>`.
     """
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.beta.pipeline.linkPrediction.predict."
+    def _endpoint_prefix(self) -> str:
+        return "gds.beta.pipeline.linkPrediction.predict."
 
     def link_features(self) -> List[LinkFeature]:
         """
         Get the link features of the pipeline.
 
         Returns:
             A list of LinkFeatures of the pipeline.
```

### Comparing `graphdatascience-1.8/graphdatascience/model/model.py` & `graphdatascience-1.9/graphdatascience/model/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 from pandas import DataFrame, Series
 
 from ..graph.graph_object import Graph
 from ..graph.graph_type_check import graph_type_check
 from ..query_runner.query_runner import QueryRunner
 from ..server_version.compatible_with import compatible_with
 from ..server_version.server_version import ServerVersion
+from graphdatascience.call_parameters import CallParameters
 
 
 class Model(ABC):
     def __init__(self, name: str, query_runner: QueryRunner, server_version: ServerVersion):
         self._name = name
         self._query_runner = query_runner
         self._server_version = server_version
 
     @abstractmethod
-    def _query_prefix(self) -> str:
+    def _endpoint_prefix(self) -> str:
         pass
 
     def _list_info(self) -> DataFrame:
         if self._server_version < ServerVersion(2, 5, 0):
             query = "CALL gds.beta.model.list($name)"
         else:
             query = """
@@ -35,27 +36,31 @@
                       modelInfo {.*, modelName: modelName, modelType: modelType} AS modelInfo,
                       creationTime, trainConfig, graphSchema,
                       loaded, stored, published, published AS shared
                     """
 
         params = {"name": self.name()}
 
-        info = self._query_runner.run_query(query, params, custom_error=False)
+        # FIXME use call procedure + do post processing on the client side
+        info = self._query_runner.run_cypher(query, params, custom_error=False)
 
         if len(info) == 0:
             raise ValueError(f"There is no '{self.name()}' in the model catalog")
 
         return info
 
     def _estimate_predict(self, predict_mode: str, graph_name: str, config: Dict[str, Any]) -> "Series[Any]":
-        query = f"{self._query_prefix()}{predict_mode}.estimate($graph_name, $config)"
+        endpoint = f"{self._endpoint_prefix()}{predict_mode}.estimate"
         config["modelName"] = self.name()
-        params = {"graph_name": graph_name, "config": config}
+        params = CallParameters(graph_name=graph_name, config=config)
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=endpoint,
+            params=params,
+        ).squeeze()
 
     def name(self) -> str:
         """
         Get the name of the model.
 
         Returns:
             The name of the model.
@@ -161,19 +166,22 @@
         Check whether the model exists.
 
         Returns:
             True if the model exists, False otherwise.
 
         """
         name_space = "beta." if self._server_version < ServerVersion(2, 5, 0) else ""
-        query = f"CALL gds.{name_space}model.exists($model_name) YIELD exists"
+        endpoint = f"gds.{name_space}model.exists"
+        yields = ["exists"]
 
-        params = {"model_name": self._name}
+        params = CallParameters(model_name=self._name)
 
-        return self._query_runner.run_query(query, params, custom_error=False).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=endpoint, params=params, yields=yields, custom_error=False
+        ).squeeze()
 
     def drop(self, failIfMissing: bool = False) -> "Series[Any]":
         """
         Drop the model.
 
         Args:
             failIfMissing: If True, an error is thrown if the model does not exist. If False, no error is thrown.
@@ -195,16 +203,16 @@
                       modelName, modelType,
                       modelInfo {.*, modelName: modelName, modelType: modelType} AS modelInfo,
                       creationTime, trainConfig, graphSchema,
                       loaded, stored, published, published AS shared
                     """
 
         params = {"model_name": self._name, "fail_if_missing": failIfMissing}
-
-        return self._query_runner.run_query(query, params, custom_error=False).squeeze()  # type: ignore
+        # FIXME use call procedure + do post processing on the client side
+        return self._query_runner.run_cypher(query, params, custom_error=False).squeeze()  # type: ignore
 
     def metrics(self) -> "Series[Any]":
         """
         Get the metrics of the model.
 
         Returns:
             The metrics of the model.
@@ -223,19 +231,19 @@
             G: The graph to predict on.
             **config: The config for the prediction.
 
         Returns:
             The prediction results as DataFrame.
 
         """
-        query = f"{self._query_prefix()}stream($graph_name, $config)"
+        endpoint = f"{self._endpoint_prefix()}stream"
         config["modelName"] = self.name()
-        params = {"graph_name": G.name(), "config": config}
+        params = CallParameters(graph_name=G.name(), config=config)
 
-        return self._query_runner.run_query_with_logging(query, params)
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params, logging=True)
 
     @graph_type_check
     def predict_stream_estimate(self, G: Graph, **config: Any) -> "Series[Any]":
         """
         Estimate the prediction on the given graph using the model and stream the results as DataFrame
 
         Args:
@@ -257,19 +265,21 @@
             G: The graph to predict on.
             **config: The config for the prediction.
 
         Returns:
             The result of mutate operation.
 
         """
-        query = f"{self._query_prefix()}mutate($graph_name, $config)"
+        endpoint = f"{self._endpoint_prefix()}mutate"
         config["modelName"] = self.name()
-        params = {"graph_name": G.name(), "config": config}
+        params = CallParameters(graph_name=G.name(), config=config)
 
-        return self._query_runner.run_query_with_logging(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=endpoint, params=params, logging=True
+        ).squeeze()
 
     @graph_type_check
     def predict_mutate_estimate(self, G: Graph, **config: Any) -> "Series[Any]":
         """
         Estimate the memory needed to predict on the given graph using the model.
 
         Args:
```

### Comparing `graphdatascience-1.8/graphdatascience/model/model_alpha_proc_runner.py` & `graphdatascience-1.9/graphdatascience/model/model_alpha_proc_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
 from .model import Model
 from .model_proc_runner import ModelProcRunner
 from .model_resolver import ModelResolver
+from graphdatascience.call_parameters import CallParameters
 
 
 class ModelAlphaProcRunner(ModelResolver):
     def store(self, model: Model, failIfUnsupportedType: bool = True) -> "Series[Any]":
         self._namespace += ".store"
-
-        query = f"CALL {self._namespace}($model_name, $fail_flag)"
-        params = {
-            "model_name": model.name(),
-            "fail_flag": failIfUnsupportedType,
-        }
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(
+            model_name=model.name(),
+            fail_flag=failIfUnsupportedType,
+        )
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=self._namespace,
+            params=params,
+        ).squeeze()
 
     def publish(self, model: Model) -> Model:
         self._namespace += ".publish"
+        params = CallParameters(model_name=model.name())
 
-        query = f"CALL {self._namespace}($model_name)"
-        params = {"model_name": model.name()}
-
-        result = self._query_runner.run_query(query, params)
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
         model_name = result["modelInfo"][0]["modelName"]
         model_type = result["modelInfo"][0]["modelType"]
 
         return self._resolve_model(model_type, model_name)
 
     def load(self, model_name: str) -> Tuple[Model, "Series[Any]"]:
         self._namespace += ".load"
+        params = CallParameters(model_name=model_name)
 
-        query = f"CALL {self._namespace}($model_name)"
-        params = {"model_name": model_name}
-
-        result = self._query_runner.run_query(query, params).squeeze()
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()
 
         self._namespace = "gds.model"
         proc_runner = ModelProcRunner(self._query_runner, self._namespace, self._server_version)
 
         return proc_runner.get(result["modelName"]), result
 
     def delete(self, model: Model) -> "Series[Any]":
         self._namespace += ".delete"
-
-        query = f"CALL {self._namespace}($model_name)"
-        params = {"model_name": model.name()}
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        params = CallParameters(model_name=model.name())
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/model/model_beta_proc_runner.py` & `graphdatascience-1.9/graphdatascience/model/model_beta_proc_runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,31 @@
 from typing import Any, Optional
 
 from pandas import DataFrame, Series
 
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
 from .model import Model
+from graphdatascience.call_parameters import CallParameters
 
 
 class ModelBetaProcRunner(UncallableNamespace, IllegalAttrChecker):
     def list(self, model: Optional[Model] = None) -> DataFrame:
         self._namespace += ".list"
 
+        params = CallParameters()
         if model:
-            query = f"CALL {self._namespace}($model_name)"
-            params = {"model_name": model.name()}
-        else:
-            query = f"CALL {self._namespace}()"
-            params = {}
+            params["model_name"] = model.name()
 
-        return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
     def exists(self, model_name: str) -> "Series[Any]":
         self._namespace += ".exists"
+        params = CallParameters(model_name=model_name)
 
-        query = f"CALL {self._namespace}($model_name)"
-        params = {"model_name": model_name}
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
 
     def drop(self, model: Model) -> "Series[Any]":
         self._namespace += ".drop"
+        params = CallParameters(model_name=model.name())
 
-        query = f"CALL {self._namespace}($model_name)"
-        params = {"model_name": model.name()}
-
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/model/model_endpoints.py` & `graphdatascience-1.9/graphdatascience/model/model_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/model/model_resolver.py` & `graphdatascience-1.9/graphdatascience/model/model_resolver.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/model/node_classification_model.py` & `graphdatascience-1.9/graphdatascience/model/node_classification_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from typing import Any, Dict, List
 
 from pandas import Series
 
 from ..graph.graph_object import Graph
 from ..graph.graph_type_check import graph_type_check
 from .pipeline_model import PipelineModel
+from graphdatascience.call_parameters import CallParameters
 
 
 class NCModel(PipelineModel):
     """
     Represents a node classification model in the model catalog.
     Construct this using
     :func:`NCTrainingPipeline.train() <graphdatascience.pipeline.nc_training_pipeline.NCTrainingPipeline.train>`.
     """
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.beta.pipeline.nodeClassification.predict."
+    def _endpoint_prefix(self) -> str:
+        return "gds.beta.pipeline.nodeClassification.predict."
 
     @graph_type_check
     def predict_write(self, G: Graph, **config: Any) -> "Series[Any]":
         """
         Predict the node labels of a graph and write the results to the database.
 
         Args:
             G: The graph to predict on.
             **config: The config for the prediction.
 
         Returns:
             The result of the write operation.
 
         """
-        query = f"{self._query_prefix()}write($graph_name, $config)"
+        endpoint = f"{self._endpoint_prefix()}write"
         config["modelName"] = self.name()
-        params = {"graph_name": G.name(), "config": config}
+        params = CallParameters(graph_name=G.name(), config=config)
 
-        return self._query_runner.run_query_with_logging(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=endpoint, params=params, logging=True
+        ).squeeze()
 
     @graph_type_check
     def predict_write_estimate(self, G: Graph, **config: Any) -> "Series[Any]":
         """
         Estimate the memory needed to predict the node labels of a graph and write the results to the database.
 
         Args:
```

### Comparing `graphdatascience-1.8/graphdatascience/model/node_regression_model.py` & `graphdatascience-1.9/graphdatascience/model/node_regression_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 class NRModel(PipelineModel):
     """
     Represents a node regression model in the model catalog.
     Construct this using
     :func:`NRTrainingPipeline.train() <graphdatascience.pipeline.nr_training_pipeline.NRTrainingPipeline.train>`.
     """
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.alpha.pipeline.nodeRegression.predict."
+    def _endpoint_prefix(self) -> str:
+        return "gds.alpha.pipeline.nodeRegression.predict."
 
     def feature_properties(self) -> List[str]:
         """
         Get the feature properties of the model.
 
         Returns:
             The feature properties of the model.
```

### Comparing `graphdatascience-1.8/graphdatascience/model/pipeline_model.py` & `graphdatascience-1.9/graphdatascience/model/pipeline_model.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/model/simple_rel_embedding_model.py` & `graphdatascience-1.9/graphdatascience/model/simple_rel_embedding_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 from typing import Any, Dict, List, Union
 
 from pandas import DataFrame, Series
 
+from ..call_parameters import CallParameters
 from ..query_runner.query_runner import QueryRunner
 from ..server_version.server_version import ServerVersion
 
 NodeFilter = Union[int, List[int], str]
 
 
 class SimpleRelEmbeddingModel:
@@ -50,43 +50,27 @@
             top_k: How many target nodes to return for each source node
             general_config: General algorithm keyword parameters such as 'concurrency'
 
         Returns:
             The `top_k` highest scoring target nodes for each source node, along with the score for the node pair
         """
 
-        if general_config:
-            general_config_str = f",{os.linesep}{f',{os.linesep}'.join([f'{k}: ${k}' for k in general_config.keys()])}"
-        else:
-            general_config_str = ""
-
-        return self._query_runner.run_query(
-            f"""
-            CALL gds.ml.kge.predict.stream(
-                $graph_name,
-                {{
-                    sourceNodeFilter: $source_node_filter,
-                    targetNodeFilter: $target_node_filter,
-                    nodeEmbeddingProperty: $node_embedding_property,
-                    relationshipTypeEmbedding: $relationship_type_embedding,
-                    scoringFunction: $scoring_function,
-                    topK: $top_k{general_config_str}
-                }}
-            )
-            """,
-            {
-                "graph_name": self._graph_name,
-                "source_node_filter": source_node_filter,
-                "target_node_filter": target_node_filter,
-                "node_embedding_property": self._node_embedding_property,
-                "relationship_type_embedding": self._relationship_type_embeddings[relationship_type],
-                "scoring_function": self._scoring_function,
-                "top_k": top_k,
-                **general_config,
-            },
+        config = {
+            "sourceNodeFilter": source_node_filter,
+            "targetNodeFilter": target_node_filter,
+            "nodeEmbeddingProperty": self._node_embedding_property,
+            "relationshipTypeEmbedding": self._relationship_type_embeddings[relationship_type],
+            "scoringFunction": self._scoring_function,
+            "topK": top_k,
+            **general_config,
+        }
+
+        return self._query_runner.call_procedure(
+            endpoint="gds.ml.kge.predict.stream",
+            params=CallParameters(graph_name=self._graph_name, config=config),
         )
 
     def predict_mutate(
         self,
         source_node_filter: NodeFilter,
         target_node_filter: NodeFilter,
         relationship_type: str,
@@ -108,47 +92,29 @@
                 score
             general_config: General algorithm keyword parameters such as 'concurrency'
 
         Returns:
             A `pandas.Series` object with metadata about the performed computation and mutation
         """
 
-        if general_config:
-            general_config_str = f",{os.linesep}{f',{os.linesep}'.join([f'{k}: ${k}' for k in general_config.keys()])}"
-        else:
-            general_config_str = ""
-
-        return self._query_runner.run_query(  # type: ignore
-            f"""
-            CALL gds.ml.kge.predict.mutate(
-                $graph_name,
-                {{
-                    sourceNodeFilter: $source_node_filter,
-                    targetNodeFilter: $target_node_filter,
-                    nodeEmbeddingProperty: $node_embedding_property,
-                    relationshipTypeEmbedding: $relationship_type_embedding,
-                    scoringFunction: $scoring_function,
-                    topK: $top_k,
-                    mutateRelationshipType: $mutate_relationship_type,
-                    mutateProperty: $mutate_property{general_config_str}
-                }}
-            )
-            """,
-            {
-                "graph_name": self._graph_name,
-                "source_node_filter": source_node_filter,
-                "target_node_filter": target_node_filter,
-                "node_embedding_property": self._node_embedding_property,
-                "relationship_type_embedding": self._relationship_type_embeddings[relationship_type],
-                "scoring_function": self._scoring_function,
-                "top_k": top_k,
-                "mutate_relationship_type": mutate_relationship_type,
-                "mutate_property": mutate_property,
-                **general_config,
-            },
+        config = {
+            "sourceNodeFilter": source_node_filter,
+            "targetNodeFilter": target_node_filter,
+            "nodeEmbeddingProperty": self._node_embedding_property,
+            "relationshipTypeEmbedding": self._relationship_type_embeddings[relationship_type],
+            "scoringFunction": self._scoring_function,
+            "topK": top_k,
+            "mutateRelationshipType": mutate_relationship_type,
+            "mutateProperty": mutate_property,
+            **general_config,
+        }
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint="gds.ml.kge.predict.mutate",
+            params=CallParameters(graph_name=self._graph_name, config=config),
         ).squeeze()
 
     def predict_write(
         self,
         source_node_filter: NodeFilter,
         target_node_filter: NodeFilter,
         relationship_type: str,
@@ -170,47 +136,29 @@
                 score
             general_config: General algorithm keyword parameters such as 'concurrency'
 
         Returns:
             A `pandas.Series` object with metadata about the performed computation and write-back
         """
 
-        if general_config:
-            general_config_str = f",{os.linesep}{f',{os.linesep}'.join([f'{k}: ${k}' for k in general_config.keys()])}"
-        else:
-            general_config_str = ""
-
-        return self._query_runner.run_query(  # type: ignore
-            f"""
-            CALL gds.ml.kge.predict.write(
-                $graph_name,
-                {{
-                    sourceNodeFilter: $source_node_filter,
-                    targetNodeFilter: $target_node_filter,
-                    nodeEmbeddingProperty: $node_embedding_property,
-                    relationshipTypeEmbedding: $relationship_type_embedding,
-                    scoringFunction: $scoring_function,
-                    topK: $top_k,
-                    writeRelationshipType: $write_relationship_type,
-                    writeProperty: $write_property{general_config_str}
-                }}
-            )
-            """,
-            {
-                "graph_name": self._graph_name,
-                "source_node_filter": source_node_filter,
-                "target_node_filter": target_node_filter,
-                "node_embedding_property": self._node_embedding_property,
-                "relationship_type_embedding": self._relationship_type_embeddings[relationship_type],
-                "scoring_function": self._scoring_function,
-                "top_k": top_k,
-                "write_relationship_type": write_relationship_type,
-                "write_property": write_property,
-                **general_config,
-            },
+        config = {
+            "sourceNodeFilter": source_node_filter,
+            "targetNodeFilter": target_node_filter,
+            "nodeEmbeddingProperty": self._node_embedding_property,
+            "relationshipTypeEmbedding": self._relationship_type_embeddings[relationship_type],
+            "scoringFunction": self._scoring_function,
+            "topK": top_k,
+            "writeRelationshipType": write_relationship_type,
+            "writeProperty": write_property,
+            **general_config,
+        }
+
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint="gds.ml.kge.predict.write",
+            params=CallParameters(graph_name=self._graph_name, config=config),
         ).squeeze()
 
     def scoring_function(self) -> str:
         """
         Get the name of the scoring function the model is using
 
         Returns:
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/classification_training_pipeline.py` & `graphdatascience-1.9/graphdatascience/pipeline/classification_training_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 from abc import ABC
 from typing import Any
 
 from pandas import Series
 
 from ..server_version.server_version import ServerVersion
 from .training_pipeline import MODEL_TYPE, TrainingPipeline
+from graphdatascience.call_parameters import CallParameters
 
 
 class ClassificationTrainingPipeline(TrainingPipeline[MODEL_TYPE], ABC):
     def addLogisticRegression(self, **config: Any) -> "Series[Any]":
         """
         Add a logistic regression model candidate to the pipeline.
 
         Args:
             **config: The configuration for the logistic regression model.
 
         Returns:
             The result of the query.
         """
-        query = f"{self._query_prefix()}addLogisticRegression($pipeline_name, $config)"
-        params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
+        params = CallParameters(pipeline_name=self.name(), config=self._expand_ranges(config))
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=f"{self._endpoint_prefix()}addLogisticRegression",
+            params=params,
+        ).squeeze()
 
     def addRandomForest(self, **config: Any) -> "Series[Any]":
         """
         Add a random forest model candidate to the pipeline.
 
         Args:
             **config: The configuration for the random forest model.
 
         Returns:
             The result of the query.
 
         """
-        query_prefix = self._query_prefix()
+        endpoint_prefix = self._endpoint_prefix()
         if self._server_version < ServerVersion(2, 4, 0):
-            query_prefix = self._query_prefix().replace("beta", "alpha")
-        query = f"{query_prefix}addRandomForest($pipeline_name, $config)"
-        params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
+            endpoint_prefix = self._endpoint_prefix().replace("beta", "alpha")
+        params = CallParameters(pipeline_name=self.name(), config=self._expand_ranges(config))
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=f"{endpoint_prefix}addRandomForest", params=params
+        ).squeeze()
 
     def addMLP(self, **config: Any) -> "Series[Any]":
         """
         Add a multi-layer perceptron model candidate to the pipeline.
 
         Args:
             **config: The configuration for the multi-layer perceptron model.
 
         Returns:
             The result of the query.
 
         """
-        query_prefix = self._query_prefix().replace("beta", "alpha")
-        query = f"{query_prefix}addMLP($pipeline_name, $config)"
-        params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
+        endpoint_prefix = self._endpoint_prefix().replace("beta", "alpha")
+        params = CallParameters(pipeline_name=self.name(), config=self._expand_ranges(config))
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(  # type: ignore
+            endpoint=f"{endpoint_prefix}addMLP", params=params
+        ).squeeze()
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/lp_pipeline_create_runner.py` & `graphdatascience-1.9/graphdatascience/pipeline/nc_pipeline_create_runner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
+from ..call_parameters import CallParameters
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
-from .lp_training_pipeline import LPTrainingPipeline
+from .nc_training_pipeline import NCTrainingPipeline
 
 
-class LPPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
-    def create(self, name: str) -> Tuple[LPTrainingPipeline, "Series[Any]"]:
+class NCPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
+    def create(self, name: str) -> Tuple[NCTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
-        query = f"CALL {self._namespace}($name)"
-        params = {"name": name}
-        result = self._query_runner.run_query(query, params).squeeze()
+        params = CallParameters(name=name)
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()
 
-        return LPTrainingPipeline(name, self._query_runner, self._server_version), result
+        return NCTrainingPipeline(name, self._query_runner, self._server_version), result
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/lp_training_pipeline.py` & `graphdatascience-1.9/graphdatascience/pipeline/lp_training_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any
 
 from pandas import DataFrame, Series
 
 from ..model.link_prediction_model import LPModel
 from ..query_runner.query_runner import QueryRunner
 from .classification_training_pipeline import ClassificationTrainingPipeline
+from graphdatascience.call_parameters import CallParameters
 
 
 class LPTrainingPipeline(ClassificationTrainingPipeline[LPModel]):
     """
     Represents a link prediction training pipeline.
     Construct an instance of this class using :func:`graphdatascience.GraphDataScience.lp_pipe`.
     """
@@ -20,32 +21,30 @@
         Args:
             feature_type: The type of feature to add.
             **config: The configuration for the feature, this includes the node properties to use.
 
         Returns:
             The result of the query.
         """
-        query = f"{self._query_prefix()}addFeature($pipeline_name, $feature_type, $config)"
-        params = {
-            "pipeline_name": self.name(),
-            "feature_type": feature_type,
-            "config": config,
-        }
+        endpoint = f"{self._endpoint_prefix()}addFeature"
+        params = CallParameters(
+            pipeline_name=self.name(), feature_type=feature_type, config=self._expand_ranges(config)
+        )
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params).squeeze()  # type: ignore
 
     def feature_steps(self) -> DataFrame:
         """
         Get the feature steps of the pipeline.
 
         Returns:
             A DataFrame containing the feature steps of the pipeline.
 
         """
         pipeline_info = self._list_info()["pipelineInfo"][0]
         return DataFrame(pipeline_info["featurePipeline"]["featureSteps"])
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.beta.pipeline.linkPrediction."
+    def _endpoint_prefix(self) -> str:
+        return "gds.beta.pipeline.linkPrediction."
 
     def _create_trained_model(self, name: str, query_runner: QueryRunner) -> LPModel:
         return LPModel(name, query_runner, self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/nc_pipeline_create_runner.py` & `graphdatascience-1.9/graphdatascience/pipeline/nr_pipeline_create_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
+from ..call_parameters import CallParameters
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
-from .nc_training_pipeline import NCTrainingPipeline
+from .nr_training_pipeline import NRTrainingPipeline
 
 
-class NCPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
-    def create(self, name: str) -> Tuple[NCTrainingPipeline, "Series[Any]"]:
+class NRPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
+    def create(self, name: str) -> Tuple[NRTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
-        query = f"CALL {self._namespace}($name)"
-        params = {"name": name}
-        result = self._query_runner.run_query(query, params).squeeze()
+        params = CallParameters(pipeline_name=name)
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()
 
-        return NCTrainingPipeline(name, self._query_runner, self._server_version), result
+        return NRTrainingPipeline(name, self._query_runner, self._server_version), result
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/nc_training_pipeline.py` & `graphdatascience-1.9/graphdatascience/pipeline/nc_training_pipeline.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Any, List, Union
 
 from pandas import Series
 
 from ..model.node_classification_model import NCModel
 from ..pipeline.classification_training_pipeline import ClassificationTrainingPipeline
 from ..query_runner.query_runner import QueryRunner
+from graphdatascience.call_parameters import CallParameters
 
 
 class NCTrainingPipeline(ClassificationTrainingPipeline[NCModel], ABC):
     """
     Represents a node classification training pipeline.
     Construct an instance of this class using :func:`graphdatascience.GraphDataScience.nc_pipe`.
     """
@@ -21,29 +22,29 @@
         Args:
             node_properties: The node properties to use for training.
 
         Returns:
             The result of the query.
 
         """
-        query = f"{self._query_prefix()}selectFeatures($pipeline_name, $node_properties)"
-        params = {"pipeline_name": self.name(), "node_properties": node_properties}
+        endpoint = f"{self._endpoint_prefix()}selectFeatures"
+        params = CallParameters(pipeline_name=self.name(), node_properties=node_properties)
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params).squeeze()  # type: ignore
 
     def feature_properties(self) -> "Series[Any]":
         """
         Get the feature properties of the pipeline.
 
         Returns:
             A Series containing the feature properties of the pipeline.
 
         """
         pipeline_info = self._list_info()["pipelineInfo"][0]
         feature_properties: "Series[Any]" = Series(pipeline_info["featurePipeline"]["featureProperties"], dtype=object)
         return feature_properties
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.beta.pipeline.nodeClassification."
+    def _endpoint_prefix(self) -> str:
+        return "gds.beta.pipeline.nodeClassification."
 
     def _create_trained_model(self, name: str, query_runner: QueryRunner) -> NCModel:
         return NCModel(name, query_runner, self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/nr_pipeline_create_runner.py` & `graphdatascience-1.9/graphdatascience/pipeline/lp_pipeline_create_runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import Any, Tuple
 
 from pandas import Series
 
 from ..error.illegal_attr_checker import IllegalAttrChecker
 from ..error.uncallable_namespace import UncallableNamespace
-from .nr_training_pipeline import NRTrainingPipeline
+from .lp_training_pipeline import LPTrainingPipeline
+from graphdatascience.call_parameters import CallParameters
 
 
-class NRPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
-    def create(self, name: str) -> Tuple[NRTrainingPipeline, "Series[Any]"]:
+class LPPipelineCreateRunner(UncallableNamespace, IllegalAttrChecker):
+    def create(self, name: str) -> Tuple[LPTrainingPipeline, "Series[Any]"]:
         self._namespace += ".create"
 
-        query = f"CALL {self._namespace}($name)"
-        params = {"name": name}
-        result = self._query_runner.run_query(query, params).squeeze()
+        params = CallParameters(name=name)
+        result = self._query_runner.call_procedure(endpoint=self._namespace, params=params).squeeze()
 
-        return NRTrainingPipeline(name, self._query_runner, self._server_version), result
+        return LPTrainingPipeline(name, self._query_runner, self._server_version), result
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/nr_training_pipeline.py` & `graphdatascience-1.9/graphdatascience/pipeline/nr_training_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, List, Union
 
 from pandas import Series
 
 from ..model.node_regression_model import NRModel
 from ..query_runner.query_runner import QueryRunner
 from .training_pipeline import TrainingPipeline
+from graphdatascience.call_parameters import CallParameters
 
 
 class NRTrainingPipeline(TrainingPipeline[NRModel]):
     """
     Represents a node regression training pipeline.
     Construct an instance of this class using :func:`graphdatascience.GraphDataScience.nr_pipe`.
     """
@@ -20,61 +21,61 @@
         Args:
             **config: The configuration for the linear regression model.
 
         Returns:
             The result of the query.
 
         """
-        query = f"{self._query_prefix()}addLinearRegression($pipeline_name, $config)"
-        params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
+        endpoint = f"{self._endpoint_prefix()}addLinearRegression"
+        params = CallParameters(pipeline_name=self.name(), config=self._expand_ranges(config))
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params).squeeze()  # type: ignore
 
     def addRandomForest(self, **config: Any) -> "Series[Any]":
         """
         Add a random forest regressor candidate to the pipeline.
 
         Args:
             **config: The configuration for the random forest regressor.
 
         Returns:
             The result of the query.
 
         """
-        query = f"{self._query_prefix()}addRandomForest($pipeline_name, $config)"
-        params = {"pipeline_name": self.name(), "config": self._expand_ranges(config)}
+        endpoint = f"{self._endpoint_prefix()}addRandomForest"
+        params = CallParameters(pipeline_name=self.name(), config=self._expand_ranges(config))
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params).squeeze()  # type: ignore
 
     def selectFeatures(self, node_properties: Union[str, List[str]]) -> "Series[Any]":
         """
         Select the node properties to use for training.
 
         Args:
             node_properties: The node properties to use for training.
 
         Returns:
             The result of the query.
 
         """
-        query = f"{self._query_prefix()}selectFeatures($pipeline_name, $node_properties)"
-        params = {"pipeline_name": self.name(), "node_properties": node_properties}
+        endpoint = f"{self._endpoint_prefix()}selectFeatures"
+        params = CallParameters(pipeline_name=self.name(), node_properties=node_properties)
 
-        return self._query_runner.run_query(query, params).squeeze()  # type: ignore
+        return self._query_runner.call_procedure(endpoint=endpoint, params=params).squeeze()  # type: ignore
 
     def feature_properties(self) -> "Series[Any]":
         """
         Get the feature properties of the pipeline.
 
         Returns:
             A Series containing the feature properties of the pipeline.
 
         """
         pipeline_info = self._list_info()["pipelineInfo"][0]
         feature_properties: "Series[Any]" = Series(pipeline_info["featurePipeline"]["featureProperties"], dtype=object)
         return feature_properties
 
-    def _query_prefix(self) -> str:
-        return "CALL gds.alpha.pipeline.nodeRegression."
+    def _endpoint_prefix(self) -> str:
+        return "gds.alpha.pipeline.nodeRegression."
 
     def _create_trained_model(self, name: str, query_runner: QueryRunner) -> NRModel:
         return NRModel(name, query_runner, self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/pipeline_beta_proc_runner.py` & `graphdatascience-1.9/graphdatascience/pipeline/pipeline_beta_proc_runner.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/pipeline/pipeline_endpoints.py` & `graphdatascience-1.9/graphdatascience/pipeline/pipeline_endpoints.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/query_runner/arrow_graph_constructor.py` & `graphdatascience-1.9/graphdatascience/query_runner/arrow_graph_constructor.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/query_runner/arrow_query_runner.py` & `graphdatascience-1.9/graphdatascience/query_runner/arrow_query_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,62 @@
 import base64
 import json
 import time
 import warnings
 from typing import Any, Dict, List, Optional, Tuple
 
 import pyarrow.flight as flight
-from pandas import DataFrame
+from pandas import DataFrame, Series
+from pyarrow import ChunkedArray, Table, chunked_array
 from pyarrow.flight import ClientMiddleware, ClientMiddlewareFactory
+from pyarrow.types import is_dictionary  # type: ignore
 
+from ..call_parameters import CallParameters
 from ..server_version.server_version import ServerVersion
 from .arrow_graph_constructor import ArrowGraphConstructor
 from .graph_constructor import GraphConstructor
 from .query_runner import QueryRunner
 from graphdatascience.server_version.compatible_with import (
     IncompatibleServerVersionError,
 )
 
 
 class ArrowQueryRunner(QueryRunner):
+    @staticmethod
+    def create(
+        fallback_query_runner: QueryRunner,
+        auth: Optional[Tuple[str, str]] = None,
+        encrypted: bool = False,
+        disable_server_verification: bool = False,
+        tls_root_certs: Optional[bytes] = None,
+    ) -> "QueryRunner":
+        server_version = fallback_query_runner.server_version()
+
+        yield_fields = (
+            ["running", "listenAddress"]
+            if server_version >= ServerVersion(2, 2, 1)
+            else ["running", "advertisedListenAddress"]
+        )
+        arrow_info: "Series[Any]" = fallback_query_runner.call_procedure(
+            endpoint="gds.debug.arrow", yields=yield_fields, custom_error=False
+        ).squeeze()
+        listen_address: str = arrow_info.get("advertisedListenAddress", arrow_info["listenAddress"])  # type: ignore
+        if arrow_info["running"]:
+            return ArrowQueryRunner(
+                listen_address,
+                fallback_query_runner,
+                server_version,
+                auth,
+                encrypted,
+                disable_server_verification,
+                tls_root_certs,
+            )
+        else:
+            return fallback_query_runner
+
     def __init__(
         self,
         uri: str,
         fallback_query_runner: QueryRunner,
         server_version: ServerVersion,
         auth: Optional[Tuple[str, str]] = None,
         encrypted: bool = False,
@@ -48,68 +83,87 @@
         self._flight_client = flight.FlightClient(location, **client_options)
 
     def warn_about_deprecation(self, old_endpoint: str, new_endpoint: str) -> None:
         warnings.warn(
             DeprecationWarning(f"The endpoint '{old_endpoint}' is deprecated. Please use '{new_endpoint}' instead.")
         )
 
-    def run_query(
+    def run_cypher(
         self,
         query: str,
         params: Optional[Dict[str, Any]] = None,
         database: Optional[str] = None,
         custom_error: bool = True,
     ) -> DataFrame:
+        return self._fallback_query_runner.run_cypher(query, params, database, custom_error)
+
+    def call_procedure(
+        self,
+        endpoint: str,
+        params: Optional[CallParameters] = None,
+        yields: Optional[List[str]] = None,
+        database: Optional[str] = None,
+        logging: bool = False,
+        custom_error: bool = True,
+    ) -> DataFrame:
         if params is None:
-            params = {}
+            params = CallParameters()
 
         new_endpoint_server_version = ServerVersion(2, 2, 0)
         no_tier_in_namespace_server_version = ServerVersion(2, 5, 0)
 
         # We need to support the deprecated endpoints until they get removed on the server side
-        if (old_endpoint := ("gds.graph.streamNodeProperty" in query)) or "gds.graph.nodeProperty.stream" in query:
+        if (
+            old_endpoint := ("gds.graph.streamNodeProperty" == endpoint)
+        ) or "gds.graph.nodeProperty.stream" == endpoint:
             graph_name = params["graph_name"]
             property_name = params["properties"]
             node_labels = params["entities"]
 
+            config = {"node_property": property_name, "node_labels": node_labels}
+
+            if "listNodeLabels" in params["config"]:
+                config["list_node_labels"] = params["config"]["listNodeLabels"]
+
             if self._server_version < new_endpoint_server_version:
                 endpoint = "gds.graph.streamNodeProperty"
             else:
                 endpoint = "gds.graph.nodeProperty.stream"
                 if old_endpoint:
                     self.warn_about_deprecation(
                         old_endpoint="gds.graph.streamNodeProperty", new_endpoint="gds.graph.nodeProperty.stream"
                     )
 
-            return self._run_arrow_property_get(
-                graph_name, endpoint, {"node_property": property_name, "node_labels": node_labels}
-            )
+            return self._run_arrow_property_get(graph_name, endpoint, config)
         elif (
-            old_endpoint := ("gds.graph.streamNodeProperties" in query)
-        ) or "gds.graph.nodeProperties.stream" in query:
+            old_endpoint := ("gds.graph.streamNodeProperties" == endpoint)
+        ) or "gds.graph.nodeProperties.stream" == endpoint:
             graph_name = params["graph_name"]
-            property_names = params["properties"]
-            node_labels = params["entities"]
+
+            config = {"node_properties": params["properties"], "node_labels": params["entities"]}
+
+            if "listNodeLabels" in params["config"]:
+                config["list_node_labels"] = params["config"]["listNodeLabels"]
 
             if self._server_version < new_endpoint_server_version:
                 endpoint = "gds.graph.streamNodeProperties"
             else:
                 endpoint = "gds.graph.nodeProperties.stream"
                 if old_endpoint:
                     self.warn_about_deprecation(
                         old_endpoint="gds.graph.streamNodeProperties", new_endpoint="gds.graph.nodeProperties.stream"
                     )
             return self._run_arrow_property_get(
                 graph_name,
                 endpoint,
-                {"node_properties": property_names, "node_labels": node_labels},
+                config,
             )
         elif (
-            old_endpoint := ("gds.graph.streamRelationshipProperty" in query)
-        ) or "gds.graph.relationshipProperty.stream" in query:
+            old_endpoint := ("gds.graph.streamRelationshipProperty" == endpoint)
+        ) or "gds.graph.relationshipProperty.stream" == endpoint:
             graph_name = params["graph_name"]
             property_name = params["properties"]
             relationship_types = params["entities"]
 
             if self._server_version < new_endpoint_server_version:
                 endpoint = "gds.graph.streamRelationshipProperty"
             else:
@@ -121,16 +175,16 @@
                     )
             return self._run_arrow_property_get(
                 graph_name,
                 endpoint,
                 {"relationship_property": property_name, "relationship_types": relationship_types},
             )
         elif (
-            old_endpoint := ("gds.graph.streamRelationshipProperties" in query)
-        ) or "gds.graph.relationshipProperties.stream" in query:
+            old_endpoint := ("gds.graph.streamRelationshipProperties" == endpoint)
+        ) or "gds.graph.relationshipProperties.stream" == endpoint:
             graph_name = params["graph_name"]
             property_names = params["properties"]
             relationship_types = params["entities"]
 
             if self._server_version < new_endpoint_server_version:
                 endpoint = "gds.graph.streamRelationshipProperties"
             else:
@@ -143,16 +197,16 @@
 
             return self._run_arrow_property_get(
                 graph_name,
                 endpoint,
                 {"relationship_properties": property_names, "relationship_types": relationship_types},
             )
         elif (
-            old_endpoint := ("gds.beta.graph.relationships.stream" in query)
-        ) or "gds.graph.relationships.stream" in query:
+            old_endpoint := ("gds.beta.graph.relationships.stream" == endpoint)
+        ) or "gds.graph.relationships.stream" == endpoint:
             graph_name = params["graph_name"]
             relationship_types = params["relationship_types"]
 
             if self._server_version < new_endpoint_server_version:
                 raise IncompatibleServerVersionError(
                     f"The call gds.beta.graph.relationships.stream with parameters {params} via Arrow requires GDS "
                     f"server version >= 2.2.0. The current version is {self._server_version}"
@@ -166,21 +220,24 @@
                         self.warn_about_deprecation(
                             old_endpoint="gds.beta.graph.relationships.stream",
                             new_endpoint="gds.graph.relationships.stream",
                         )
 
             return self._run_arrow_property_get(graph_name, endpoint, {"relationship_types": relationship_types})
 
-        return self._fallback_query_runner.run_query(query, params, database, custom_error)
+        return self._fallback_query_runner.call_procedure(endpoint, params, yields, database, logging, custom_error)
 
-    def run_query_with_logging(
-        self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
-    ) -> DataFrame:
-        # For now there's no logging support with Arrow queries.
-        return self._fallback_query_runner.run_query_with_logging(query, params, database)
+    def server_version(self) -> ServerVersion:
+        return self._fallback_query_runner.server_version()
+
+    def driver_config(self) -> Dict[str, Any]:
+        return self._fallback_query_runner.driver_config()
+
+    def encrypted(self) -> bool:
+        return self._fallback_query_runner.encrypted()
 
     def set_database(self, database: str) -> None:
         self._fallback_query_runner.set_database(database)
 
     def set_bookmarks(self, bookmarks: Optional[Any]) -> None:
         self._fallback_query_runner.set_bookmarks(bookmarks)
 
@@ -214,17 +271,22 @@
             "graph_name": graph_name,
             "procedure_name": procedure_name,
             "configuration": configuration,
         }
         ticket = flight.Ticket(json.dumps(payload).encode("utf-8"))
 
         get = self._flight_client.do_get(ticket)
-        result: DataFrame = get.read_pandas()
+        arrow_table = get.read_all()
 
-        return result
+        if configuration.get("list_node_labels", False):
+            # GDS 2.5 had an inconsistent naming of the node labels column
+            new_colum_names = ["nodeLabels" if i == "labels" else i for i in arrow_table.column_names]
+            arrow_table = arrow_table.rename_columns(new_colum_names)
+
+        return self._sanitize_arrow_table(arrow_table).to_pandas()  # type: ignore
 
     def create_graph_constructor(
         self, graph_name: str, concurrency: int, undirected_relationship_types: Optional[List[str]]
     ) -> GraphConstructor:
         database = self.database()
         if not database:
             raise ValueError(
@@ -232,14 +294,30 @@
                 "using `GraphDataScience.set_database`."
             )
 
         return ArrowGraphConstructor(
             database, graph_name, self._flight_client, concurrency, undirected_relationship_types
         )
 
+    def _sanitize_arrow_table(self, arrow_table: Table) -> Table:
+        dict_encoded_fields = [
+            (idx, field) for idx, field in enumerate(arrow_table.schema) if is_dictionary(field.type)
+        ]
+        for idx, field in dict_encoded_fields:
+            try:
+                field.type.to_pandas_dtype()
+            except NotImplementedError:
+                # we need to decode the dictionary column before transforming to pandas
+                if isinstance(arrow_table[field.name], ChunkedArray):
+                    decoded_col = chunked_array([chunk.dictionary_decode() for chunk in arrow_table[field.name].chunks])
+                else:
+                    decoded_col = arrow_table[field.name].dictionary_decode()
+                arrow_table = arrow_table.set_column(idx, field.name, decoded_col)
+        return arrow_table
+
 
 class AuthFactory(ClientMiddlewareFactory):  # type: ignore
     def __init__(self, auth: Tuple[str, str], *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self._auth = auth
         self._token: Optional[str] = None
         self._token_timestamp = 0
```

### Comparing `graphdatascience-1.8/graphdatascience/query_runner/aura_db_arrow_query_runner.py` & `graphdatascience-1.9/graphdatascience/query_runner/aura_db_arrow_query_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,114 +1,140 @@
-from typing import Any, Dict, List, NamedTuple, Optional, Tuple
+from typing import Any, Dict, List, Optional, Tuple
 
-from neo4j import GraphDatabase
 from pandas import DataFrame, Series
 from pyarrow import flight
 from pyarrow.flight import ClientMiddleware, ClientMiddlewareFactory
 
+from ..call_parameters import CallParameters
+from ..gds_session.dbms_connection_info import DbmsConnectionInfo
 from .query_runner import QueryRunner
 from graphdatascience.query_runner.graph_constructor import GraphConstructor
-from graphdatascience.query_runner.neo4j_query_runner import Neo4jQueryRunner
-
-
-class AuraDbConnectionInfo(NamedTuple):
-    uri: str
-    auth: Tuple[str, str]
+from graphdatascience.server_version.server_version import ServerVersion
 
 
 class AuraDbArrowQueryRunner(QueryRunner):
-    def __init__(self, fallback_query_runner: QueryRunner, aura_db_connection_info: AuraDbConnectionInfo):
-        self._fallback_query_runner = fallback_query_runner
+    GDS_REMOTE_PROJECTION_PROC_NAME = "gds.graph.project.remoteDb"
 
-        aura_db_endpoint, auth = aura_db_connection_info
-        self._auth = auth
-
-        config: Dict[str, Any] = {"max_connection_lifetime": 60}
-        self._driver = GraphDatabase.driver(aura_db_endpoint, auth=auth, **config)
-        arrow_info: "Series[Any]" = (
-            Neo4jQueryRunner(self._driver, auto_close=True)
-            .run_query("CALL gds.debug.arrow.plugin()", custom_error=False)
-            .squeeze()
-        )
+    def __init__(
+        self,
+        gds_query_runner: QueryRunner,
+        db_query_runner: QueryRunner,
+        encrypted: bool,
+        aura_db_connection_info: DbmsConnectionInfo,
+    ):
+        self._gds_query_runner = gds_query_runner
+        self._db_query_runner = db_query_runner
+        self._auth = aura_db_connection_info.auth()
+
+        arrow_info: "Series[Any]" = db_query_runner.call_procedure(
+            endpoint="internal.arrow.status", custom_error=False
+        ).squeeze()
 
         if not arrow_info.get("running"):
-            raise RuntimeError("The plugin arrow server for AuraDB is not running")
+            raise RuntimeError(f"The Arrow Server is not running at `{aura_db_connection_info.uri}`")
         listen_address: Optional[str] = arrow_info.get("advertisedListenAddress")  # type: ignore
         if not listen_address:
             raise ConnectionError("Did not retrieve connection info from database")
 
         host, port_string = listen_address.split(":")
 
         self._auth_pair_middleware = AuthPairInterceptingMiddleware()
         client_options: Dict[str, Any] = {
             "middleware": [AuthPairInterceptingMiddlewareFactory(self._auth_pair_middleware)],
             "disable_server_verification": True,
         }
+
+        self._encrypted = encrypted
         location = (
             flight.Location.for_grpc_tls(host, int(port_string))
-            if self._driver.encrypted
+            if self._encrypted
             else flight.Location.for_grpc_tcp(host, int(port_string))
         )
         self._client = flight.FlightClient(location, **client_options)
 
-    def run_query(
+    def run_cypher(
         self,
         query: str,
         params: Optional[Dict[str, Any]] = None,
         database: Optional[str] = None,
         custom_error: bool = True,
     ) -> DataFrame:
+        return self._db_query_runner.run_cypher(query, params, database, custom_error)
+
+    def call_procedure(
+        self,
+        endpoint: str,
+        params: Optional[CallParameters] = None,
+        yields: Optional[List[str]] = None,
+        database: Optional[str] = None,
+        logging: bool = False,
+        custom_error: bool = True,
+    ) -> DataFrame:
         if params is None:
-            params = {}
+            params = CallParameters()
 
-        if "gds.alpha.graph.project.remote" in query:
+        if AuraDbArrowQueryRunner.GDS_REMOTE_PROJECTION_PROC_NAME == endpoint:
             token, aura_db_arrow_endpoint = self._get_or_request_auth_pair()
             params["token"] = token
             params["host"] = aura_db_arrow_endpoint
-            params["config"] = {"useEncryption": False}
+            params["config"]["useEncryption"] = self._encrypted
 
-        elif ".write" in query and "config" in params and "remote" in params["config"] and params["config"]["remote"]:
+        elif ".write" in endpoint and self.is_remote_projected_graph(params["graph_name"]):
             token, aura_db_arrow_endpoint = self._get_or_request_auth_pair()
             host, port_string = aura_db_arrow_endpoint.split(":")
-            del params["config"]["remote"]
             params["config"]["arrowConnectionInfo"] = {
                 "hostname": host,
                 "port": int(port_string),
                 "bearerToken": token,
-                "useEncryption": False,
+                "useEncryption": self._encrypted,
             }
 
-        return self._fallback_query_runner.run_query(query, params, database, custom_error)
+        return self._gds_query_runner.call_procedure(endpoint, params, yields, database, logging, custom_error)
+
+    def is_remote_projected_graph(self, graph_name: str) -> bool:
+        database_location: str = self._gds_query_runner.call_procedure(
+            endpoint="gds.graph.list",
+            yields=["databaseLocation"],
+            params=CallParameters(graph_name=graph_name),
+        ).squeeze()
+        return database_location == "remote"
+
+    def server_version(self) -> ServerVersion:
+        return self._db_query_runner.server_version()
+
+    def driver_config(self) -> Dict[str, Any]:
+        return self._db_query_runner.driver_config()
+
+    def encrypted(self) -> bool:
+        return self._db_query_runner.encrypted()
 
     def set_database(self, database: str) -> None:
-        self._fallback_query_runner.set_database(database)
+        self._db_query_runner.set_database(database)
 
     def set_bookmarks(self, bookmarks: Optional[Any]) -> None:
-        self._fallback_query_runner.set_bookmarks(bookmarks)
+        self._db_query_runner.set_bookmarks(bookmarks)
 
     def bookmarks(self) -> Optional[Any]:
-        return self._fallback_query_runner.bookmarks()
+        return self._db_query_runner.bookmarks()
 
     def last_bookmarks(self) -> Optional[Any]:
-        return self._fallback_query_runner.last_bookmarks()
+        return self._db_query_runner.last_bookmarks()
 
     def database(self) -> Optional[str]:
-        return self._fallback_query_runner.database()
+        return self._db_query_runner.database()
 
     def create_graph_constructor(
         self, graph_name: str, concurrency: int, undirected_relationship_types: Optional[List[str]]
     ) -> GraphConstructor:
-        return self._fallback_query_runner.create_graph_constructor(
-            graph_name, concurrency, undirected_relationship_types
-        )
+        return self._gds_query_runner.create_graph_constructor(graph_name, concurrency, undirected_relationship_types)
 
     def close(self) -> None:
         self._client.close()
-        self._driver.close()
-        self._fallback_query_runner.close()
+        self._gds_query_runner.close()
+        self._db_query_runner.close()
 
     def _get_or_request_auth_pair(self) -> Tuple[str, str]:
         self._client.authenticate_basic_token(self._auth[0], self._auth[1])
         return (self._auth_pair_middleware.token(), self._auth_pair_middleware.endpoint())
 
 
 class AuthPairInterceptingMiddlewareFactory(ClientMiddlewareFactory):  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/query_runner/cypher_graph_constructor.py` & `graphdatascience-1.9/graphdatascience/query_runner/cypher_graph_constructor.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
             self.LegacyCypherProjectionRunner(self._query_runner, self._graph_name, self._concurrency).run(
                 node_df, rel_df
             )
 
     def _should_warn_about_arrow_missing(self) -> bool:
         try:
-            license: str = self._query_runner.run_query(
+            license: str = self._query_runner.run_cypher(
                 "CALL gds.debug.sysInfo() YIELD key, value WHERE key = 'gdsEdition' RETURN value", custom_error=False
             ).squeeze()
             should_warn = license == "Licensed"
         except Exception as e:
             # It's not a user's concern whether Arrow is set up or not in AuraDS.
             if (
                 "There is no procedure with the name `gds.debug.sysInfo` "
@@ -207,15 +207,15 @@
             )
 
             configuration = {
                 "readConcurrency": self._concurrency,
                 "undirectedRelationshipTypes": self._undirected_relationship_types,
             }
 
-            self._query_runner.run_query(
+            self._query_runner.run_cypher(
                 query,
                 {
                     "data": combined_df.values.tolist(),
                     "graph_name": self._graph_name,
                     "configuration": configuration,
                 },
                 custom_error=False,
@@ -369,15 +369,15 @@
                 "$relationship_query, "
                 "{readConcurrency: $read_concurrency, parameters: { nodes: $nodes, relationships: $relationships }})"
             )
 
             node_query, nodes = self._node_query(node_df)
             relationship_query, relationships = self._relationship_query(relationship_df)
 
-            self._query_runner.run_query(
+            self._query_runner.run_cypher(
                 query,
                 {
                     "graph_name": self._graph_name,
                     "node_query": node_query,
                     "relationship_query": relationship_query,
                     "read_concurrency": self._concurrency,
                     "nodes": nodes,
```

### Comparing `graphdatascience-1.8/graphdatascience/query_runner/query_runner.py` & `graphdatascience-1.9/graphdatascience/query_runner/query_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,51 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Optional
 
 from pandas import DataFrame
 
+from ..call_parameters import CallParameters
 from ..server_version.server_version import ServerVersion
 from .graph_constructor import GraphConstructor
 
 
 class QueryRunner(ABC):
     @abstractmethod
-    def run_query(
+    def call_procedure(
+        self,
+        endpoint: str,
+        params: Optional[CallParameters] = None,
+        yields: Optional[List[str]] = None,
+        database: Optional[str] = None,
+        logging: bool = False,
+        custom_error: bool = True,
+    ) -> DataFrame:
+        pass
+
+    @abstractmethod
+    def run_cypher(
         self,
         query: str,
         params: Optional[Dict[str, Any]] = None,
         database: Optional[str] = None,
         custom_error: bool = True,
     ) -> DataFrame:
         pass
 
-    def run_query_with_logging(
-        self, query: str, params: Optional[Dict[str, Any]] = None, database: Optional[str] = None
-    ) -> DataFrame:
-        return self.run_query(query, params, database, True)
+    @abstractmethod
+    def server_version(self) -> ServerVersion:
+        pass
+
+    @abstractmethod
+    def driver_config(self) -> Dict[str, Any]:
+        pass
+
+    @abstractmethod
+    def encrypted(self) -> bool:
+        pass
 
     @abstractmethod
     def set_database(self, database: str) -> None:
         pass
 
     @abstractmethod
     def set_bookmarks(self, bookmarks: Optional[Any]) -> None:
```

### Comparing `graphdatascience-1.8/graphdatascience/resources/cora/cora_nodes.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/cora/cora_nodes.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/cora/cora_rels.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/cora/cora_rels.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/cora/serialize_cora.py` & `graphdatascience-1.9/graphdatascience/resources/cora/serialize_cora.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_acted_in.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_acted_in.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_actors.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_actors.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_directed_in.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_directed_in.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_directors.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_directors.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_movies_with_genre.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_movies_with_genre.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/imdb_movies_without_genre.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/imdb/imdb_movies_without_genre.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/imdb/serialize_imdb.py` & `graphdatascience-1.9/graphdatascience/resources/imdb/serialize_imdb.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/karate/karate_club.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/karate/karate_club.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/artist_nodes.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/lastfm/artist_nodes.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/serialize_lastfm.py` & `graphdatascience-1.9/graphdatascience/resources/lastfm/serialize_lastfm.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/user_friend_df_directed.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/lastfm/user_friend_df_directed.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/user_listen_artist_rels.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/lastfm/user_listen_artist_rels.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/user_nodes.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/lastfm/user_nodes.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/resources/lastfm/user_tag_artist_rels.parquet.gzip` & `graphdatascience-1.9/graphdatascience/resources/lastfm/user_tag_artist_rels.parquet.gzip`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/server_version/compatible_with.py` & `graphdatascience-1.9/graphdatascience/server_version/compatible_with.py`

 * *Files identical despite different names*

### Comparing `graphdatascience-1.8/graphdatascience/server_version/server_version.py` & `graphdatascience-1.9/graphdatascience/server_version/server_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import re
-from typing import Type, TypeVar
+from __future__ import annotations
 
-SV = TypeVar("SV", bound="ServerVersion")
+import re
 
 
 class InvalidServerVersionError(Exception):
     pass
 
 
 class ServerVersion:
@@ -15,31 +14,31 @@
 
     def __init__(self, major: int, minor: int, patch: int):
         self.major = major
         self.minor = minor
         self.patch = patch
 
     @classmethod
-    def from_string(cls: Type[SV], version: str) -> SV:
+    def from_string(cls, version: str) -> ServerVersion:
         server_version_match = re.search(r"^(\d+)\.(\d+)\.(\d+)", version)
         if not server_version_match:
             raise InvalidServerVersionError(f"{version} is not a valid GDS library version")
 
         return cls(*map(int, server_version_match.groups()))
 
-    def __lt__(self, other: SV) -> bool:
+    def __lt__(self, other: ServerVersion) -> bool:
         if self.major != other.major:
             return self.major < other.major
 
         if self.minor != other.minor:
             return self.minor < other.minor
 
         if self.patch != other.patch:
             return self.patch < other.patch
 
         return False
 
-    def __ge__(self, other: SV) -> bool:
+    def __ge__(self, other: ServerVersion) -> bool:
         return not self.__lt__(other)
 
     def __str__(self) -> str:
         return f"{self.major}.{self.minor}.{self.patch}"
```

### Comparing `graphdatascience-1.8/graphdatascience/system/config_endpoints.py` & `graphdatascience-1.9/graphdatascience/system/config_endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,45 @@
 from typing import Any, Dict, Optional
 
 from pandas import DataFrame
 
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.caller_base import CallerBase
 from graphdatascience.error.illegal_attr_checker import IllegalAttrChecker
 from graphdatascience.error.uncallable_namespace import UncallableNamespace
 from graphdatascience.server_version.compatible_with import compatible_with
 from graphdatascience.server_version.server_version import ServerVersion
 
 
 class ConfigProcRunner(IllegalAttrChecker, UncallableNamespace):
     def set(self, key: str, value: Any, username: Optional[str] = None) -> None:
         self._namespace += ".set"
 
-        params = {"key": key, "value": value}
+        params = CallParameters(key=key, value=value)
 
         # Checking for explicit None as '' is a valid user
         if username is not None:
-            query = f"CALL {self._namespace}($key, $value, $username)"
             params["username"] = username
-        else:
-            query = f"CALL {self._namespace}($key, $value)"
 
-        self._query_runner.run_query(query, params)
+        self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
     def list(self, key: Optional[str] = None, username: Optional[str] = None) -> DataFrame:
         self._namespace += ".list"
 
         config: Dict[str, Any] = {}
 
         if key:
             config["key"] = key
         # Checking for explicit None as '' is a valid user
         if username is not None:
             config["username"] = username
 
-        query = f"CALL {self._namespace}($config)"
-        params = {"config": config}
+        params = CallParameters(config=config)
 
-        return self._query_runner.run_query(query, params)
+        return self._query_runner.call_procedure(endpoint=self._namespace, params=params)
 
 
 class ConfigIntermediateSteps(CallerBase):
     @property
     def defaults(self) -> ConfigProcRunner:
         return ConfigProcRunner(self._query_runner, f"{self._namespace}.defaults", self._server_version)
```

### Comparing `graphdatascience-1.8/graphdatascience/topological_lp/topological_lp_alpha_runner.py` & `graphdatascience-1.9/graphdatascience/topological_lp/topological_lp_alpha_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         query = f"""
         MATCH (n1) WHERE id(n1) = {node1}
         MATCH (n2) WHERE id(n2) = {node2}
         RETURN {self._namespace}(n1, n2, $config) AS score
         """
         params = {"config": config}
 
-        return self._query_runner.run_query(query, params)["score"].squeeze()  # type: ignore
+        return self._query_runner.run_cypher(query, params)["score"].squeeze()  # type: ignore
 
     def adamicAdar(self, node1: int, node2: int, **config: Any) -> float:
         self._namespace += ".adamicAdar"
         return self._run_standard_function(node1, node2, config)
 
     def commonNeighbors(self, node1: int, node2: int, **config: Any) -> float:
         self._namespace += ".commonNeighbors"
@@ -42,12 +42,12 @@
 
         query = f"""
         MATCH (n1) WHERE id(n1) = {node1}
         MATCH (n2) WHERE id(n2) = {node2}
         RETURN {self._namespace}(n1, n2{community_property}) AS score
         """
 
-        return self._query_runner.run_query(query)["score"].squeeze()  # type: ignore
+        return self._query_runner.run_cypher(query)["score"].squeeze()  # type: ignore
 
     def totalNeighbors(self, node1: int, node2: int, **config: Any) -> float:
         self._namespace += ".totalNeighbors"
         return self._run_standard_function(node1, node2, config)
```

### Comparing `graphdatascience-1.8/graphdatascience/utils/util_endpoints.py` & `graphdatascience-1.9/graphdatascience/utils/util_endpoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Any, Dict, List
 
 from pandas import DataFrame
 
 from ..caller_base import CallerBase
 from ..error.client_only_endpoint import client_only_endpoint
 from .util_proc_runner import UtilProcRunner
+from graphdatascience.call_parameters import CallParameters
 from graphdatascience.error.cypher_warning_handler import (
     filter_id_func_deprecation_warning,
 )
 from graphdatascience.server_version.server_version import ServerVersion
 
 
 class DirectUtilEndpoints(CallerBase):
@@ -44,32 +45,29 @@
         elif label_match:
             query = f"MATCH (n) WHERE {label_match} RETURN id(n) AS id"
         elif prop_match:
             query = f"MATCH (n) WHERE {prop_match} RETURN id(n) AS id"
         else:
             query = "MATCH (n) RETURN id(n) AS id"
 
-        node_match = self._query_runner.run_query(query, custom_error=False)
+        node_match = self._query_runner.run_cypher(query, custom_error=False)
 
         if len(node_match) != 1:
             raise ValueError(f"Filter did not match with exactly one node: {node_match}")
 
         return node_match["id"][0].item()  # type: ignore
 
     def version(self) -> str:
         """
         Get the version of the GDS library.
 
         Returns:
             The version of the GDS library.
         """
-        namespace = self._namespace + ".version"
-        result = self._query_runner.run_query(f"RETURN {namespace}() as version", custom_error=False).squeeze()
-
-        return result  # type: ignore
+        return f"{self._server_version}"
 
     @client_only_endpoint("gds")
     def server_version(self) -> ServerVersion:
         """
         Get the version of the GDS library.
 
         Returns:
@@ -82,15 +80,15 @@
         """
         List all available GDS procedures.
 
         Returns:
             A DataFrame containing all available GDS procedures.
         """
         namespace = self._namespace + ".list"
-        return self._query_runner.run_query(f"CALL {namespace}()", custom_error=False)
+        return self._query_runner.call_procedure(endpoint=namespace, custom_error=False)
 
     @property
     def util(self) -> UtilProcRunner:
         return UtilProcRunner(self._query_runner, f"{self._namespace}.util", self._server_version)
 
 
 class IndirectUtilAlphaEndpoints(CallerBase):
@@ -103,15 +101,15 @@
             selected_values: The values to encode.
 
         Returns:
             The one hot encoded values.
         """
         namespace = self._namespace + ".oneHotEncoding"
 
-        query = f"RETURN {namespace}($available_values, $selected_values) AS embedding"
-        params = {
-            "available_values": available_values,
-            "selected_values": selected_values,
-        }
-        result = self._query_runner.run_query(query, params)
+        params = CallParameters(
+            available_values=available_values,
+            selected_values=selected_values,
+        )
+        query = f"RETURN {namespace}($available_values, $selected_values) AS encoded"
+        result = self._query_runner.run_cypher(query=query, params=params)
 
-        return result["embedding"].squeeze()  # type: ignore
+        return result.iat[0, 0]  # type: ignore
```

### Comparing `graphdatascience-1.8/graphdatascience/utils/util_proc_runner.py` & `graphdatascience-1.9/graphdatascience/utils/util_proc_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,33 +15,33 @@
             node_id: The id of the node to get.
 
         Returns:
             The node with the given id.
 
         """
         self._namespace += ".asNode"
-        result = self._query_runner.run_query(f"RETURN {self._namespace}({node_id}) AS node")
+        result = self._query_runner.run_cypher(f"RETURN {self._namespace}({node_id}) AS node")
 
-        return result["node"].squeeze()
+        return result.iat[0, 0]
 
     def asNodes(self, node_ids: List[int]) -> List[Any]:
         """
         Get a list of nodes from a list of node ids.
 
         Args:
             node_ids: The ids of the nodes to get.
 
         Returns:
             The nodes with the given ids.
 
         """
         self._namespace += ".asNodes"
-        result = self._query_runner.run_query(f"RETURN {self._namespace}({node_ids}) AS nodes")
+        result = self._query_runner.run_cypher(f"RETURN {self._namespace}({node_ids}) AS nodes")
 
-        return result["nodes"].squeeze()  # type: ignore
+        return result.iat[0, 0]  # type: ignore
 
     @graph_type_check
     def nodeProperty(self, G: Graph, node_id: int, property_key: str, node_label: str = "*") -> Any:
         """
         Get the property of a node with the given id.
 
         Args:
@@ -59,10 +59,10 @@
         query = f"RETURN {self._namespace}($graph_name, $node_id, $property_key, $node_label) as property"
         params = {
             "graph_name": G.name(),
             "node_id": node_id,
             "property_key": property_key,
             "node_label": node_label,
         }
-        result = self._query_runner.run_query(query, params)
+        result = self._query_runner.run_cypher(query, params)
 
-        return result["property"].squeeze()
+        return result.iat[0, 0]
```

### Comparing `graphdatascience-1.8/graphdatascience.egg-info/PKG-INFO` & `graphdatascience-1.9/graphdatascience.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdatascience
-Version: 1.8
+Version: 1.9
 Summary: A Python client for the Neo4j Graph Data Science (GDS) library
 Home-page: https://neo4j.com/product/graph-data-science/
 Author: Neo4j
 Author-email: team-gds@neo4j.org
 License: Apache License 2.0
 Project-URL: Documentation, https://neo4j.com/docs/graph-data-science-client/current/
 Project-URL: Source, https://github.com/neo4j/graph-data-science-client
@@ -26,18 +26,19 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: multimethod<2.0,>=1.0
 Requires-Dist: neo4j<6.0,>=4.4.2
 Requires-Dist: pandas<3.0,>=1.0
-Requires-Dist: pyarrow<14.0,>=4.0
+Requires-Dist: pyarrow<15.0,>=10.0
 Requires-Dist: textdistance<5.0,>=4.0
 Requires-Dist: tqdm<5.0,>=4.0
 Requires-Dist: typing-extensions<5.0,>=4.0
+Requires-Dist: requests
 Provides-Extra: ogb
 Requires-Dist: ogb<2.0,>=1.0; extra == "ogb"
 Provides-Extra: networkx
 Requires-Dist: networkx<4.0,>=2.0; extra == "networkx"
 
 # Neo4j Graph Data Science Client
 
@@ -121,14 +122,15 @@
 
 * [Machine learning pipelines: Node classification](examples/ml-pipelines-node-classification.ipynb)
 * [Node Regression with Subgraph and Graph Sample projections](examples/node-regression-with-subgraph-and-graph-sample.ipynb)
 * [Product recommendations with kNN based on FastRP embeddings](examples/fastrp-and-knn.ipynb)
 * [Sampling, Export and Integration with PyG example](examples/import-sample-export-gnn.ipynb)
 * [Load data to a projected graph via graph construction](examples/load-data-via-graph-construction.ipynb)
 * [Heterogeneous Node Classification with HashGNN and Autotuning](https://github.com/neo4j/graph-data-science-client/tree/main/examples/heterogeneous-node-classification-with-hashgnn.ipynb)
+* [Perform inference using pre-trained KGE models](examples/kge-predict-transe-pyg-train.ipynb)
 
 
 ## Documentation
 
 The primary source for learning everything about the GDS Python Client is the manual, hosted at https://neo4j.com/docs/graph-data-science-client/current/.
 The manual is versioned to cover all GDS Python Client versions, so make sure to use the correct version to get the correct information.
```

### Comparing `graphdatascience-1.8/graphdatascience.egg-info/SOURCES.txt` & `graphdatascience-1.9/graphdatascience.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 graphdatascience/__init__.py
 graphdatascience/call_builder.py
+graphdatascience/call_parameters.py
 graphdatascience/caller_base.py
 graphdatascience/endpoints.py
 graphdatascience/graph_data_science.py
 graphdatascience/ignored_server_endpoints.py
 graphdatascience/py.typed
 graphdatascience/version.py
 graphdatascience.egg-info/PKG-INFO
@@ -25,17 +26,23 @@
 graphdatascience/error/client_only_endpoint.py
 graphdatascience/error/cypher_warning_handler.py
 graphdatascience/error/endpoint_suggester.py
 graphdatascience/error/gds_not_installed.py
 graphdatascience/error/illegal_attr_checker.py
 graphdatascience/error/unable_to_connect.py
 graphdatascience/error/uncallable_namespace.py
+graphdatascience/gds_session/__init__.py
+graphdatascience/gds_session/aura_api.py
+graphdatascience/gds_session/aura_graph_data_science.py
+graphdatascience/gds_session/dbms_connection_info.py
+graphdatascience/gds_session/gds_sessions.py
+graphdatascience/gds_session/schema.py
+graphdatascience/gds_session/session_sizes.py
 graphdatascience/graph/__init__.py
 graphdatascience/graph/graph_alpha_proc_runner.py
-graphdatascience/graph/graph_alpha_project_runner.py
 graphdatascience/graph/graph_beta_proc_runner.py
 graphdatascience/graph/graph_create_result.py
 graphdatascience/graph/graph_cypher_runner.py
 graphdatascience/graph/graph_endpoints.py
 graphdatascience/graph/graph_entity_ops_runner.py
 graphdatascience/graph/graph_export_runner.py
 graphdatascience/graph/graph_object.py
```

### Comparing `graphdatascience-1.8/setup.py` & `graphdatascience-1.9/setup.py`

 * *Files identical despite different names*

