# Comparing `tmp/neuralogic-0.7.8.tar.gz` & `tmp/neuralogic-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralogic-0.7.8.tar", last modified: Sat Oct 28 23:21:04 2023, max compression
+gzip compressed data, was "neuralogic-0.7.9.tar", last modified: Tue Nov 14 21:04:34 2023, max compression
```

## Comparing `neuralogic-0.7.8.tar` & `neuralogic-0.7.9.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.917375 neuralogic-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-10-28 23:20:51.000000 neuralogic-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2023-10-28 23:21:04.917375 neuralogic-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2023-10-28 23:20:51.000000 neuralogic-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic/
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic/core/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/core/builder/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/builder/components.py
--rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/builder/dataset_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/core/constructs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/core/constructs/function/
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/concat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/slice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/function/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)    13541 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/java_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/constructs/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/core/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/settings/settings_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/core/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/dataset/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/db/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/db/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/db/pg/
--rw-r--r--   0 runner    (1001) docker     (127)    11287 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/db/pg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/db/pg/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.897374 neuralogic-0.7.8/neuralogic/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/inference/evaluation_inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/inference/inference_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.901374 neuralogic-0.7.8/neuralogic/jar/
--rw-r--r--   0 runner    (1001) docker     (127)  2007735 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/jar/NeuraLogic.jar
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/jar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.901374 neuralogic-0.7.8/neuralogic/logging/
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.901374 neuralogic-0.7.8/neuralogic/nn/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4870 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.901374 neuralogic-0.7.8/neuralogic/nn/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/evaluator/java.py
--rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/java.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.901374 neuralogic-0.7.8/neuralogic/nn/module/
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/nn/module/general/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     8637 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6053 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/positional_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/rvnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8722 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/general/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/nn/module/gnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4746 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/appnp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/gatv2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/gcn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/gin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/gsage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/res_gated.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/rgcn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3679 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/sg.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/gnn/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/nn/module/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/meta/magnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/meta/meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/module/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/nn/torch_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/adam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/lr_scheduler/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/lr_scheduler/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/lr_scheduler/lr_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.905375 neuralogic-0.7.8/neuralogic/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic/utils/data/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/
--rw-r--r--   0 runner    (1001) docker     (127)   402216 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
--rw-r--r--   0 runner    (1001) docker     (127)      278 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/embeddings.txt
--rw-r--r--   0 runner    (1001) docker     (127)    38585 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)   205423 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/queries.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/family/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/family/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/family/queries.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/family/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.909375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/queries.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/template.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/generalized/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
--rw-r--r--   0 runner    (1001) docker     (127)      496 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/naive/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/solution/
--rw-r--r--   0 runner    (1001) docker     (127)      218 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/vectorized/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/neuralogic/utils/visualize/
--rw-r--r--   0 runner    (1001) docker     (127)     5003 2023-10-28 23:20:51.000000 neuralogic-0.7.8/neuralogic/utils/visualize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.893374 neuralogic-0.7.8/neuralogic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11533 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-28 23:21:04.000000 neuralogic-0.7.8/neuralogic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-28 23:20:51.000000 neuralogic-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-28 23:21:04.917375 neuralogic-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2023-10-28 23:20:51.000000 neuralogic-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-28 23:21:04.913375 neuralogic-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5690 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_constructs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_csv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7904 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_evaluation_inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_general_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_inference_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10461 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_java_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7218 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_quick_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_recurrent_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_special_predicates.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_torch_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-28 23:20:51.000000 neuralogic-0.7.8/tests/test_xor_generalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.028421 neuralogic-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-11-14 21:04:19.000000 neuralogic-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2023-11-14 21:04:34.028421 neuralogic-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2023-11-14 21:04:19.000000 neuralogic-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.008421 neuralogic-0.7.9/neuralogic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/core/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/builder/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/builder/dataset_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/core/constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/core/constructs/function/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/slice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/function/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/java_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/constructs/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/core/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/settings/settings_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/core/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/dataset/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/db/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.012421 neuralogic-0.7.9/neuralogic/db/pg/
+-rw-r--r--   0 runner    (1001) docker     (127)    11287 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/db/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/db/pg/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/inference/evaluation_inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/inference/inference_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/jar/
+-rw-r--r--   0 runner    (1001) docker     (127)  2004765 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/jar/NeuraLogic.jar
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/jar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/nn/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/evaluator/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6816 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.016421 neuralogic-0.7.9/neuralogic/nn/module/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/nn/module/general/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8637 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5646 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6053 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/positional_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/rvnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8722 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/general/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/nn/module/gnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/appnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/gatv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/gin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/gsage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/res_gated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/rgcn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/sg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/gnn/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/nn/module/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/meta/magnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/meta/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/module/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/nn/torch_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/adam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/lr_scheduler/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/lr_scheduler/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/lr_scheduler/lr_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.008421 neuralogic-0.7.9/neuralogic/utils/data/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.020421 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/bondEmbeddings3.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/
+-rw-r--r--   0 runner    (1001) docker     (127)   402216 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_crosssum.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_elementProduct.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_gnn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_graphlets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_partial.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/templates/template_product.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/embeddings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   205423 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.008421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/family/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/family/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/family/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/family/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/queries.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/template.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.008421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/generalized/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/generalized/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/generalized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/generalized/texamples.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/generalized/ztexamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/naive/
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/naive/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/naive/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.024421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/solution/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/solution/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/solution/testExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.028421 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/vectorized/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/vectorized/template.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/xor/vectorized/trainExamples.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.028421 neuralogic-0.7.9/neuralogic/utils/visualize/
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2023-11-14 21:04:19.000000 neuralogic-0.7.9/neuralogic/utils/visualize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.008421 neuralogic-0.7.9/neuralogic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5935 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-14 21:04:33.000000 neuralogic-0.7.9/neuralogic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-11-14 21:04:19.000000 neuralogic-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 21:04:34.028421 neuralogic-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-11-14 21:04:19.000000 neuralogic-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 21:04:34.028421 neuralogic-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_constructs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_csv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7904 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_evaluation_inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_general_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_inference_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10461 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_java_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7268 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_quick_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_recurrent_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_special_predicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_torch_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-11-14 21:04:19.000000 neuralogic-0.7.9/tests/test_xor_generalization.py
```

### Comparing `neuralogic-0.7.8/LICENSE` & `neuralogic-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/PKG-INFO` & `neuralogic-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.8
+Version: 0.7.9
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: JPype1>=1.3.0
-Requires-Dist: numpy>=1.19.0
+Requires-Dist: numpy>=1.20.4
+Requires-Dist: matplotlib
 Requires-Dist: tqdm
 
 
 <p align="center">
 <img src="https://github.com/LukasZahradnik/PyNeuraLogic/blob/master/docs/_static/readme_logo.svg" alt="PyNeuraLogic" title="PyNeuraLogic"/>
 </p>
 
@@ -125,15 +126,15 @@
 
 
 ### Prerequisites
 
 To use PyNeuraLogic, you need to install the following prerequisites:
 
 ```
-Python >= 3.7
+Python >= 3.8
 Java >= 1.8
 ```
 
 In case you want to use visualization provided in the library, it is required to have [Graphviz](https://graphviz.org/download/) installed.
 
 ## 🔬 Examples
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.8 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.9 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: JPype1>=1.3.0 Requires-Dist: numpy>=1.19.0 Requires-Dist: tqdm
+Dist: JPype1>=1.3.0 Requires-Dist: numpy>=1.20.4 Requires-Dist: matplotlib
+Requires-Dist: tqdm
                                 [PyNeuraLogic]
 [![PyPI version](https://badge.fury.io/py/neuralogic.svg)](https://
 badge.fury.io/py/neuralogic) [![License](https://img.shields.io/pypi/l/
 neuralogic)](https://badge.fury.io/py/neuralogic) [![Tests Status](https://
 github.com/LukasZahradnik/PyNeuraLogic/actions/workflows/tests.yml/badge.svg)]
 (https://github.com/LukasZahradnik/PyNeuraLogic/actions/workflows/tests.yml) [!
 [Code Quality Status](https://github.com/LukasZahradnik/PyNeuraLogic/actions/
@@ -87,15 +88,15 @@
 
 We hope you'll find the framework useful in designing _your own_ deep
 **relational** learning ideas beyond the GNNs! Please let us know if you need
 some guidance or would like to cooperate! ## ð¡ Getting started ###
 Installation To install PyNeuraLogic's latest release from the PyPI repository,
 use the following command: ```commandline $ pip install neuralogic ``` ###
 Prerequisites To use PyNeuraLogic, you need to install the following
-prerequisites: ``` Python >= 3.7 Java >= 1.8 ``` In case you want to use
+prerequisites: ``` Python >= 3.8 Java >= 1.8 ``` In case you want to use
 visualization provided in the library, it is required to have [Graphviz](https:
 //graphviz.org/download/) installed. ## ð¬ Examples [![Open In Colab](https:/
 /colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/
 examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/
 LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `neuralogic-0.7.8/README.md` & `neuralogic-0.7.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
 
 ### Prerequisites
 
 To use PyNeuraLogic, you need to install the following prerequisites:
 
 ```
-Python >= 3.7
+Python >= 3.8
 Java >= 1.8
 ```
 
 In case you want to use visualization provided in the library, it is required to have [Graphviz](https://graphviz.org/download/) installed.
 
 ## 🔬 Examples
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
```

#### html2text {}

```diff
@@ -74,15 +74,15 @@
 
 We hope you'll find the framework useful in designing _your own_ deep
 **relational** learning ideas beyond the GNNs! Please let us know if you need
 some guidance or would like to cooperate! ## ð¡ Getting started ###
 Installation To install PyNeuraLogic's latest release from the PyPI repository,
 use the following command: ```commandline $ pip install neuralogic ``` ###
 Prerequisites To use PyNeuraLogic, you need to install the following
-prerequisites: ``` Python >= 3.7 Java >= 1.8 ``` In case you want to use
+prerequisites: ``` Python >= 3.8 Java >= 1.8 ``` In case you want to use
 visualization provided in the library, it is required to have [Graphviz](https:
 //graphviz.org/download/) installed. ## ð¬ Examples [![Open In Colab](https:/
 /colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/
 examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/
 LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `neuralogic-0.7.8/neuralogic/__init__.py` & `neuralogic-0.7.9/neuralogic/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 _is_initialized = False
 _seed = int.from_bytes(os.urandom(4), byteorder="big")
 _initial_seed = _seed
 _rnd_generator = None
 _max_memory_size = None
+_graphviz_path = None
 
 jvm_params = {
     "classpath": os.path.join(os.path.abspath(os.path.dirname(__file__)), "jar", "NeuraLogic.jar"),
 }
 
 jvm_options = ["-Xms1g"]
 
@@ -102,16 +103,39 @@
 def is_initialized() -> bool:
     """
     Check whether the NeuraLogic backend has been initialized
     """
     return _is_initialized
 
 
+def set_graphviz_path(path: Optional[str]):
+    """
+    Set the default path to Graphviz
+
+    Parameters
+    ----------
+    path : Optional[str]
+        The Graphviz path
+    """
+    global _graphviz_path
+    _graphviz_path = path
+
+
+def get_default_graphviz_path() -> Optional[str]:
+    """
+    Get the default path to Graphviz
+    """
+    return _graphviz_path
+
+
 def initialize(
-    debug_mode: bool = False, debug_port: int = 12999, is_debug_server: bool = True, debug_suspend: bool = True
+    debug_mode: bool = False,
+    debug_port: int = 12999,
+    is_debug_server: bool = True,
+    debug_suspend: bool = True,
 ):
     """
     Initialize the NeuraLogic backend. This function is called implicitly when needed and should be called
     manually only for debugging.
 
     Parameters
     ----------
```

### Comparing `neuralogic-0.7.8/neuralogic/core/__init__.py` & `neuralogic-0.7.9/neuralogic/core/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from neuralogic.core.constructs.factories import Var, Constant, Relation, V, C, R
-from neuralogic.core.constructs.rule import Rule
+from neuralogic.core.constructs.rule import Rule, RuleBody
 from neuralogic.core.template import Template
-from neuralogic.core.builder import BuiltDataset
+from neuralogic.core.builder import BuiltDataset, GroundedDataset
 from neuralogic.core.constructs.metadata import Metadata
 from neuralogic.core.settings import Settings, SettingsProxy
 from neuralogic.core.enums import Grounder
 from neuralogic.core.constructs.function import Transformation, Aggregation, Combination
 
 
 __all__ = [
     "Var",
     "V",
     "Constant",
     "C",
     "Relation",
     "R",
     "Rule",
+    "RuleBody",
     "Template",
     "BuiltDataset",
+    "GroundedDataset",
     "Transformation",
     "Aggregation",
     "Combination",
     "Grounder",
     "Settings",
     "SettingsProxy",
     "Metadata",
```

### Comparing `neuralogic-0.7.8/neuralogic/core/builder/components.py` & `neuralogic-0.7.9/neuralogic/core/builder/components.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import json
 from typing import Any, Dict, Optional, List
 
+import jpype
 import numpy as np
 
 from neuralogic.core.constructs.java_objects import ValueFactory
-from neuralogic.utils.visualize import draw_sample
+from neuralogic.utils.visualize import draw_sample, draw_grounding
 
 
 class RawSample:
-    __slots__ = "java_sample", "fact_cache"
+    __slots__ = "java_sample", "fact_cache", "grounding"
 
-    def __init__(self, sample):
+    def __init__(self, sample, grounding):
         self.java_sample = sample
+        self.grounding = grounding
         self.fact_cache = {}
 
     @property
     def target(self):
         return ValueFactory.from_java(self.java_sample.target)
 
     def _find_fact(self, fact_str):
@@ -54,29 +56,29 @@
         sample_fact.getRawState().setValue(value)
         sample_fact.offset.value = value
         return sample_fact.index
 
     def draw(
         self,
         filename: Optional[str] = None,
-        draw_ipython=True,
+        show=True,
         img_type="png",
         value_detail: int = 0,
         graphviz_path: Optional[str] = None,
         *args,
         **kwargs,
     ):
-        return draw_sample(self, filename, draw_ipython, img_type, value_detail, graphviz_path, *args, **kwargs)
+        return draw_sample(self, filename, show, img_type, value_detail, graphviz_path, *args, **kwargs)
 
 
 class Sample(RawSample):
     __slots__ = ("id", "target", "neurons", "output_neuron", "java_sample")
 
     def __init__(self, sample, java_sample):
-        super().__init__(sample)
+        super().__init__(sample, None)
         serialized_sample = json.loads(str(sample.exportToJson()))
 
         self.id = serialized_sample["id"]
         self.target = json.loads(serialized_sample["target"])
         self.neurons = Sample.deserialize_network(serialized_sample["network"])
         self.output_neuron = self.neurons[-1].index
         self.java_sample = java_sample
@@ -162,7 +164,49 @@
         self.batch_size = batch_size
 
     def __len__(self):
         return len(self.samples)
 
     def __getitem__(self, item):
         return self.samples[item]
+
+
+class Grounding:
+    __slots__ = ("grounding",)
+
+    def __init__(self, grounding):
+        self.grounding = grounding
+
+    def draw_grounding(
+        self,
+        filename: Optional[str] = None,
+        show=True,
+        img_type="png",
+        value_detail: int = 0,
+        graphviz_path: Optional[str] = None,
+        *args,
+        **kwargs,
+    ):
+        return draw_grounding(self.grounding, filename, show, img_type, value_detail, graphviz_path, *args, **kwargs)
+
+
+class GroundedDataset:
+    """GroundedDataset represents grounded examples that are not neuralized yet."""
+
+    __slots__ = "length", "_groundings", "_groundings_list", "_builder"
+
+    def __init__(self, groundings, length, builder):
+        self.length = length
+        self._groundings = groundings
+        self._groundings_list = None
+        self._builder = builder
+
+    def __getitem__(self, item):
+        if self._groundings_list is None:
+            self._groundings = self._groundings.collect(jpype.JClass("java.util.stream.Collectors").toList())
+            self._groundings_list = [Grounding(g) for g in self._groundings]
+        return self._groundings_list[item]
+
+    def neuralize(self, progress: bool):
+        if self._groundings_list is not None:
+            return self._builder.neuralize(self._groundings.stream(), progress, self.length)
+        return self._builder.neuralize(self._groundings, progress, self.length)
```

### Comparing `neuralogic-0.7.8/neuralogic/core/builder/dataset_builder.py` & `neuralogic-0.7.9/neuralogic/core/builder/dataset_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Union, Set, Dict
 
 import jpype
 
 import neuralogic.dataset as datasets
 from neuralogic import is_initialized, initialize
 from neuralogic.core.builder.builder import Builder
-from neuralogic.core.builder.components import BuiltDataset
+from neuralogic.core.builder.components import BuiltDataset, GroundedDataset
 from neuralogic.core.constructs.relation import BaseRelation, WeightedRelation
 from neuralogic.core.constructs.rule import Rule
 from neuralogic.core.constructs.java_objects import JavaFactory
 from neuralogic.core.settings import SettingsProxy
 from neuralogic.core.sources import Sources
 
 
@@ -100,67 +100,65 @@
                 raise Exception("Inconsistent examples! Some examples have queries and some do not")
 
             examples_queries = example_query
             logic_samples.append(self.logic_sample(value, query_atom))
             self.examples_counter += 1
         return logic_samples, examples_queries
 
-    def build_dataset(
+    def ground_dataset(
         self,
         dataset: datasets.BaseDataset,
         settings: SettingsProxy,
         *,
         batch_size: int = 1,
         file_mode: bool = False,
         learnable_facts: bool = False,
-        progress: bool = False,
-    ) -> BuiltDataset:
-        """Builds the dataset (does grounding and neuralization) for this template instance and the backend
+    ) -> GroundedDataset:
+        """Grounds the dataset
 
         :param dataset:
         :param settings:
         :param batch_size:
         :param file_mode:
         :param learnable_facts:
-        :param progress:
         :return:
         """
-        if isinstance(dataset, datasets.TensorDataset):
-            if file_mode:
-                with tempfile.NamedTemporaryFile(mode="w", suffix=".txt") as q_tf, tempfile.NamedTemporaryFile(
-                    mode="w", suffix=".txt"
-                ) as e_tf:
-                    dataset.dump(q_tf, e_tf)
-
-                    q_tf.flush()
-                    e_tf.flush()
-
-                    return self.build_dataset(
-                        datasets.FileDataset(e_tf.name, q_tf.name),
-                        settings,
-                        batch_size=batch_size,
-                        file_mode=False,
-                        learnable_facts=learnable_facts,
-                        progress=progress,
-                    )
+        if isinstance(dataset, datasets.TensorDataset) and file_mode:
+            with tempfile.NamedTemporaryFile(mode="w", suffix=".txt") as q_tf, tempfile.NamedTemporaryFile(
+                mode="w", suffix=".txt"
+            ) as e_tf:
+                dataset.dump(q_tf, e_tf)
+
+                q_tf.flush()
+                e_tf.flush()
+
+                return self.ground_dataset(
+                    datasets.FileDataset(e_tf.name, q_tf.name),
+                    settings,
+                    batch_size=batch_size,
+                    file_mode=False,
+                    learnable_facts=learnable_facts,
+                )
 
         if isinstance(dataset, datasets.ConvertableDataset):
-            return self.build_dataset(
+            return self.ground_dataset(
                 dataset.to_dataset(),
                 settings,
                 batch_size=batch_size,
                 file_mode=False,
                 learnable_facts=learnable_facts,
-                progress=progress,
             )
 
         if batch_size > 1:
             settings.settings.minibatchSize = batch_size
             settings.settings.parallelTraining = True
 
+        builder = Builder(settings)
+        length = None
+
         if isinstance(dataset, datasets.Dataset):
             self.examples_counter = 0
             self.query_counter = 0
 
             weight_factory = self.java_factory.weight_factory
 
             examples_builder = self.examples_builder(settings.settings)
@@ -183,29 +181,59 @@
             self.java_factory.weight_factory = self.java_factory.get_new_weight_factory()
             queries, one_query_per_example = self.build_queries(queries, query_builder)
 
             logic_samples = DatasetBuilder.merge_queries_with_examples(
                 queries, examples, one_query_per_example, example_queries
             )
 
-            samples = Builder(settings).from_logic_samples(self.parsed_template, logic_samples, progress)
+            length = len(logic_samples)
+            groundings = builder.ground_from_logic_samples(self.parsed_template, logic_samples)
 
             self.java_factory.weight_factory = weight_factory
         elif isinstance(dataset, datasets.FileDataset):
             args = ["-t", dataset.examples_file or dataset.queries_file]
             if dataset.queries_file is not None:
                 args.extend(["-q", dataset.queries_file])
             if dataset.examples_file is not None:
                 args.extend(["-e", dataset.examples_file])
             sources = Sources.from_args(args, settings)
-            samples = Builder(settings).from_sources(self.parsed_template, sources, progress)
+
+            groundings = builder.ground_from_sources(self.parsed_template, sources)
         else:
             raise NotImplementedError
 
-        return BuiltDataset(samples, batch_size)
+        return GroundedDataset(groundings, length, builder)
+
+    def build_dataset(
+        self,
+        dataset: Union[datasets.BaseDataset, GroundedDataset],
+        settings: SettingsProxy,
+        *,
+        batch_size: int = 1,
+        file_mode: bool = False,
+        learnable_facts: bool = False,
+        progress: bool = False,
+    ) -> BuiltDataset:
+        """Builds the dataset (does grounding and neuralization)
+
+        :param dataset:
+        :param settings:
+        :param batch_size:
+        :param file_mode:
+        :param learnable_facts:
+        :param progress:
+        :return:
+        """
+        grounded_dataset = dataset
+
+        if not isinstance(dataset, GroundedDataset):
+            grounded_dataset = self.ground_dataset(
+                dataset, settings, batch_size=batch_size, file_mode=file_mode, learnable_facts=learnable_facts
+            )
+        return BuiltDataset(grounded_dataset.neuralize(progress), batch_size)
 
     @staticmethod
     def merge_queries_with_examples(queries, examples, one_query_per_example, example_queries=True):
         if len(examples) == 0:
             return queries
 
         if len(queries) == 0:
```

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/factories.py` & `neuralogic-0.7.9/neuralogic/core/constructs/factories.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/__init__.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/concat.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/concat.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/function.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/reshape.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/reshape.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/slice.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/slice.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/function/softmax.py` & `neuralogic-0.7.9/neuralogic/core/constructs/function/softmax.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/java_objects.py` & `neuralogic-0.7.9/neuralogic/core/constructs/java_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             if len(weight) == 1:
                 if weight[0] == 1:
                     value = self.scalar_value()
                 else:
                     value = self.vector_value(weight[0])
             elif len(weight) == 2:
                 if weight[0] == 1:
-                    value = self.vector_value(weight[1], True)
+                    value = self.scalar_value() if weight[1] == 1 else self.vector_value(weight[1], True)
                 elif weight[1] == 1:
                     value = self.vector_value(weight[0], False)
                 else:
                     value = self.matrix_value(weight[0], weight[1])
             else:
                 raise NotImplementedError
             return False, value
@@ -298,15 +298,15 @@
         java_rule.setBody(body_relation_list)
 
         offset = None  # TODO: Implement
 
         java_rule.setOffset(offset)
 
         if rule.metadata is not None:
-            java_rule.allowDuplicitGroundings = rule.metadata.duplicit_grounding
+            java_rule.allowDuplicitGroundings = bool(rule.metadata.duplicit_grounding)
 
         java_rule.setMetadata(self.get_metadata(rule.metadata, self.rule_metadata))
 
         return java_rule
 
     def get_predicate(self, predicate):
         return self.predicate_factory.construct(predicate.name, predicate.arity, predicate.special, predicate.hidden)
```

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/metadata.py` & `neuralogic-0.7.9/neuralogic/core/constructs/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import Union, Iterable, Callable
+from typing import Union, Iterable, Callable, Optional
 
 from neuralogic.core.constructs.function import Transformation, Combination, Aggregation, Function
 
 
 class Metadata:
     __slots__ = "learnable", "transformation", "aggregation", "duplicit_grounding", "combination"
 
     def __init__(
         self,
         learnable: bool = None,
         transformation: Union[str, Transformation, Combination] = None,
         combination: Union[str, Combination] = None,
         aggregation: Union[str, Aggregation] = None,
-        duplicit_grounding: bool = False,
+        duplicit_grounding: Optional[bool] = None,
     ):
         self.learnable = learnable
         self.combination = combination
         self.transformation = transformation
         self.aggregation = aggregation
         self.duplicit_grounding = duplicit_grounding
 
@@ -43,16 +43,22 @@
             metadata_list.append(f"learnable={str(self.learnable).lower()}")
         if self.transformation is not None:
             metadata_list.append(f"transformation={str(self.transformation)}")
         if self.combination is not None:
             metadata_list.append(f"combination={str(self.combination)}")
         if self.aggregation is not None:
             metadata_list.append(f"aggregation={str(self.aggregation)}")
+        if self.duplicit_grounding is not None:
+            metadata_list.append(f"duplicit_grounding={str(self.duplicit_grounding)}")
         return f"[{', '.join(metadata_list)}]"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def copy(self) -> "Metadata":
         return Metadata(
-            self.learnable, self.transformation, self.combination, self.aggregation, self.duplicit_grounding
+            learnable=self.learnable,
+            transformation=self.transformation,
+            combination=self.combination,
+            aggregation=self.aggregation,
+            duplicit_grounding=self.duplicit_grounding,
         )
```

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/predicate.py` & `neuralogic-0.7.9/neuralogic/core/constructs/predicate.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/relation.py` & `neuralogic-0.7.9/neuralogic/core/constructs/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,14 +110,19 @@
         relation.function = self.function
         relation.terms = self.terms
         relation.predicate = self.predicate
         relation.negated = self.negated
 
         return relation
 
+    def __and__(self, other) -> rule.RuleBody:
+        if isinstance(other, BaseRelation):
+            return rule.RuleBody(self, other)
+        raise NotImplementedError
+
 
 class WeightedRelation(BaseRelation):
     __slots__ = "weight", "weight_name", "is_fixed"
 
     def __init__(
         self, weight, predicate: Predicate, fixed=False, terms=None, function: Union[Transformation, Combination] = None
     ):
```

### Comparing `neuralogic-0.7.8/neuralogic/core/constructs/rule.py` & `neuralogic-0.7.9/neuralogic/core/constructs/rule.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,64 @@
-from neuralogic.core.constructs.metadata import Metadata
 from typing import Iterable, Optional
 
+from neuralogic.core.constructs.metadata import Metadata
+
+
+class RuleBody:
+    __slots__ = "literals", "metadata"
+
+    def __init__(self, lit1, lit2):
+        self.literals = [lit1, lit2]
+        self.metadata = None
+
+    def __and__(self, other):
+        from neuralogic.core.constructs.relation import BaseRelation
+
+        if isinstance(other, BaseRelation):
+            self.literals.append(other)
+            return self
+        raise NotImplementedError
+
+    def __str__(self) -> str:
+        return ", ".join(atom.to_str() for atom in self.literals)
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def __or__(self, other) -> "RuleBody":
+        if isinstance(other, Iterable):
+            other = Metadata.from_iterable(other)
+        elif not isinstance(other, Metadata):
+            raise NotImplementedError
+
+        self.metadata = other
+        return self
+
 
 class Rule:
     __slots__ = "head", "body", "metadata"
 
     def __init__(self, head, body):
         from neuralogic.core import Relation
 
         self.head = head
+        self.metadata: Optional[Metadata] = None
 
         if head.function is not None:
             raise NotImplementedError(f"Rule head {head} cannot have a function attached")
 
+        if isinstance(body, RuleBody):
+            if body.metadata is not None:
+                self._set_metadata(body.metadata)
+            body = body.literals
+
         if not isinstance(body, Iterable):
             body = [body]
 
         self.body = list(body)
-        self.metadata: Optional[Metadata] = None
 
         if self.is_ellipsis_templated():
             variable_set = {term for term in head.terms if term is not Ellipsis and str(term)[0].isupper()}
 
             for body_atom in self.body:
                 if body_atom.predicate.special and body_atom.predicate.name == "alldiff":
                     continue
@@ -76,14 +113,16 @@
 
     def __or__(self, other) -> "Rule":
         if isinstance(other, Iterable):
             other = Metadata.from_iterable(other)
         elif not isinstance(other, Metadata):
             raise NotImplementedError
 
-        if other.aggregation is not None and other.aggregation.rule_head_dependant():
-            other = other.copy()
-            other.aggregation = other.aggregation.process_head(self.head)
+        self._set_metadata(other)
+        return self
 
-        self.metadata = other
+    def _set_metadata(self, metadata: Metadata):
+        if metadata.aggregation is not None and metadata.aggregation.rule_head_dependant():
+            metadata = metadata.copy()
+            metadata.aggregation = metadata.aggregation.process_head(self.head)
 
-        return self
+        self.metadata = metadata
```

### Comparing `neuralogic-0.7.8/neuralogic/core/settings/__init__.py` & `neuralogic-0.7.9/neuralogic/core/settings/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from typing import Any, Optional
 import weakref
 
 from neuralogic.core.enums import Grounder
 from neuralogic.nn.init import Initializer, Uniform
 from neuralogic.nn.loss import MSE, ErrorFunction
 from neuralogic.core.settings.settings_proxy import SettingsProxy
-from neuralogic.core.constructs.function import Transformation, Combination
+from neuralogic.core.constructs.function import Transformation, Combination, Aggregation
 from neuralogic.optim import Optimizer, Adam
 
 
 class Settings:
     def __init__(
         self,
         *,
         optimizer: Optimizer = Adam(),
         learning_rate: Optional[float] = None,
         epochs: int = 3000,
         error_function: ErrorFunction = MSE(),
         initializer: Initializer = Uniform(),
         rule_transformation: Transformation = Transformation.TANH,
         rule_combination: Combination = Combination.SUM,
+        rule_aggregation: Aggregation = Aggregation.AVG,
         relation_transformation: Transformation = Transformation.TANH,
         relation_combination: Combination = Combination.SUM,
         iso_value_compression: bool = True,
         chain_pruning: bool = True,
         prune_only_identities: bool = False,
         grounder: Grounder = Grounder.BUP,
     ):
@@ -123,14 +124,22 @@
     def rule_combination(self) -> Combination:
         return self.params["rule_combination"]
 
     @rule_combination.setter
     def rule_combination(self, value: Combination):
         self._update("rule_combination", value)
 
+    @property
+    def rule_aggregation(self) -> Aggregation:
+        return self.params["rule_aggregation"]
+
+    @rule_aggregation.setter
+    def rule_aggregation(self, value: Aggregation):
+        self._update("rule_aggregation", value)
+
     def create_proxy(self) -> SettingsProxy:
         proxy = SettingsProxy(**self.params)
         self._proxies.add(proxy)
 
         return proxy
 
     def create_disconnected_proxy(self) -> SettingsProxy:
```

### Comparing `neuralogic-0.7.8/neuralogic/core/settings/settings_proxy.py` & `neuralogic-0.7.9/neuralogic/core/settings/settings_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import jpype
 
 import neuralogic
 from neuralogic import is_initialized, initialize
-from neuralogic.core.constructs.function import Transformation, Combination
+from neuralogic.core.constructs.function import Transformation, Combination, Aggregation
 from neuralogic.core.enums import Grounder
 from neuralogic.nn.init import Initializer
 from neuralogic.nn.loss import MSE, SoftEntropy, CrossEntropy, ErrorFunction
 from neuralogic.optim import Optimizer
 
 
 class SettingsProxy:
@@ -16,14 +16,15 @@
         optimizer: Optimizer,
         learning_rate: float,
         epochs: int,
         error_function: ErrorFunction,
         initializer: Initializer,
         rule_transformation: Transformation,
         rule_combination: Combination,
+        rule_aggregation: Aggregation,
         relation_transformation: Transformation,
         relation_combination: Combination,
         iso_value_compression: bool,
         chain_pruning: bool,
         prune_only_identities: bool,
         grounder: Grounder,
     ):
@@ -220,14 +221,22 @@
         return Combination(str(self.settings.ruleNeuronCombination))
 
     @rule_combination.setter
     def rule_combination(self, value: Combination):
         self.settings.ruleNeuronCombination = self.get_combination_function(value)
 
     @property
+    def rule_aggregation(self) -> Aggregation:
+        return Aggregation(str(self.settings.aggNeuronAggregation))
+
+    @rule_aggregation.setter
+    def rule_aggregation(self, value: Aggregation):
+        self.settings.aggNeuronAggregation = self.get_aggregation_function(value)
+
+    @property
     def debug_exporting(self) -> bool:
         return self.settings.debugExporting
 
     @debug_exporting.setter
     def debug_exporting(self, debug_export: bool):
         self.settings.debugExporting = debug_export
 
@@ -239,13 +248,17 @@
     def default_fact_value(self, value: float):
         self.settings.defaultFactValue = value
 
     def get_combination_function(self, combination: Combination):
         combination_name = str(combination)
         return self.settings_class.parseCombination(combination_name)
 
+    def get_aggregation_function(self, aggregation: Aggregation):
+        aggregation_name = str(aggregation)
+        return self.settings_class.parseCombination(aggregation_name)
+
     def get_transformation_function(self, transformation: Transformation):
         transformation_name = str(transformation)
         return self.settings_class.parseTransformation(transformation_name)
 
     def to_json(self) -> str:
         return self.settings.exportToJson()
```

### Comparing `neuralogic-0.7.8/neuralogic/core/sources.py` & `neuralogic-0.7.9/neuralogic/core/sources.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/core/template.py` & `neuralogic-0.7.9/neuralogic/core/template.py`

 * *Files 14% similar despite different names*

```diff
@@ -142,25 +142,25 @@
         model = Builder(settings_proxy).build_model(parsed_template, settings_proxy)
 
         return get_neuralogic_layer()(model, DatasetBuilder(parsed_template, java_factory), self, settings_proxy)
 
     def draw(
         self,
         filename: Optional[str] = None,
-        draw_ipython=True,
+        show=True,
         img_type="png",
         value_detail: int = 0,
         graphviz_path: Optional[str] = None,
         model=None,
         *args,
         **kwargs,
     ):
         if model is None:
             model = self.build(Settings())
-        return draw_model(model, filename, draw_ipython, img_type, value_detail, graphviz_path, *args, **kwargs)
+        return draw_model(model, filename, show, img_type, value_detail, graphviz_path, *args, **kwargs)
 
     def __str__(self) -> str:
         return "\n".join(str(r) for r in self.template)
 
     def __repr__(self) -> str:
         return self.__str__()
 
@@ -168,7 +168,18 @@
         if isinstance(other, Iterable):
             self.template.extend(other)
         elif isinstance(other, Module):
             self.template.extend(other())
         else:
             self.template.append(other)
         return self
+
+    def __getitem__(self, item) -> TemplateEntries:
+        return self.template[item]
+
+    def __delitem__(self, key):
+        self.template.pop(key)
+
+    def __setitem__(self, key, value):
+        if isinstance(value, (Iterable, Module)):
+            raise NotImplementedError
+        self.template[key] = value
```

### Comparing `neuralogic-0.7.8/neuralogic/dataset/__init__.py` & `neuralogic-0.7.9/neuralogic/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/base.py` & `neuralogic-0.7.9/neuralogic/dataset/base.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/csv.py` & `neuralogic-0.7.9/neuralogic/dataset/csv.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/db.py` & `neuralogic-0.7.9/neuralogic/dataset/db.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/file.py` & `neuralogic-0.7.9/neuralogic/dataset/file.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/logic.py` & `neuralogic-0.7.9/neuralogic/dataset/logic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/dataset/tensor.py` & `neuralogic-0.7.9/neuralogic/dataset/tensor.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/db/converter.py` & `neuralogic-0.7.9/neuralogic/db/converter.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/db/pg/__init__.py` & `neuralogic-0.7.9/neuralogic/db/pg/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/db/pg/helpers.py` & `neuralogic-0.7.9/neuralogic/db/pg/helpers.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/inference/evaluation_inference_engine.py` & `neuralogic-0.7.9/neuralogic/inference/evaluation_inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/inference/inference_engine.py` & `neuralogic-0.7.9/neuralogic/inference/inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/jar/NeuraLogic.jar` & `neuralogic-0.7.9/neuralogic/jar/NeuraLogic.jar`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,21 +1,15 @@
-Zip file size: 2007735 bytes, number of entries: 1481
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:27 META-INF/
--rw-r--r--  2.0 unx      174 b- defN 23-Oct-28 22:27 META-INF/MANIFEST.MF
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 generated/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/
--rw-r--r--  2.0 unx     1733 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/Main.class
--rw-r--r--  2.0 unx     6196 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
--rw-r--r--  2.0 unx    17210 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
+Zip file size: 2004765 bytes, number of entries: 1483
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:31 META-INF/
+-rw-r--r--  2.0 unx      174 b- defN 23-Nov-14 21:31 META-INF/MANIFEST.MF
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 generated/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/setup/
 -rw-r--r--  2.0 unx     1282 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ResultsType.class
 -rw-r--r--  2.0 unx      776 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$1.class
 -rw-r--r--  2.0 unx     1222 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$DataSelection.class
 -rw-r--r--  2.0 unx     1319 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ModelSelection.class
 -rw-r--r--  2.0 unx     1191 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$HitsClashes.class
 -rw-r--r--  2.0 unx     1243 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/setup/Settings$ErrorFcn.class
@@ -401,63 +395,63 @@
 -rw-r--r--  2.0 unx     8226 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Tuple.class
 -rw-r--r--  2.0 unx     2174 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Quintuple.class
 -rw-r--r--  2.0 unx     2000 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Quadruple.class
 -rw-r--r--  2.0 unx     1999 b- defN 23-Apr-07 21:20 cz/cvut/fel/ida/utils/generic/tuples/Triple.class
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/Utilities/
 -rw-r--r--  2.0 unx     1017 b- defN 23-Feb-13 21:15 META-INF/maven/io.github.gustiks/Utilities/pom.xml
 -rw-r--r--  2.0 unx      112 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Utilities/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/bulding/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/bulding/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/
--rw-r--r--  2.0 unx     4682 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiMerge.class
--rw-r--r--  2.0 unx     7115 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipe.class
--rw-r--r--  2.0 unx     3163 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ParallelPipe.class
--rw-r--r--  2.0 unx      958 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipe$1.class
--rw-r--r--  2.0 unx      375 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedSupplier.class
--rw-r--r--  2.0 unx      992 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Branch$1.class
--rw-r--r--  2.0 unx      380 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedConsumer.class
--rw-r--r--  2.0 unx      986 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ParallelPipe$1.class
--rw-r--r--  2.0 unx     2012 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/bulding/AbstractPipelineBuilder.class
--rw-r--r--  2.0 unx     6601 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Branch.class
--rw-r--r--  2.0 unx     1109 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$3.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$1.class
--rw-r--r--  2.0 unx     6552 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge.class
--rw-r--r--  2.0 unx     1389 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/RecurrentPipe.class
--rw-r--r--  2.0 unx      231 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Executable.class
--rw-r--r--  2.0 unx     1609 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/StreamifyPipe.class
--rw-r--r--  2.0 unx     1562 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/StreamParallelizationPipe.class
--rw-r--r--  2.0 unx     1612 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateListBranch.class
--rw-r--r--  2.0 unx     1416 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ListMerge.class
--rw-r--r--  2.0 unx     3053 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ExportingPipe.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairExtractionBranch.class
--rw-r--r--  2.0 unx     1612 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/LambdaPipe.class
--rw-r--r--  2.0 unx     1664 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairPipe.class
--rw-r--r--  2.0 unx     1208 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/IdentityGenPipe.class
--rw-r--r--  2.0 unx     1927 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairExtractionBranch.class
--rw-r--r--  2.0 unx     1650 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/PairBranch.class
--rw-r--r--  2.0 unx     1460 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/ListBranch.class
--rw-r--r--  2.0 unx     1659 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairPipe.class
--rw-r--r--  2.0 unx     1387 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateBranch.class
--rw-r--r--  2.0 unx     1683 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/pipes/generic/PairMerge.class
--rw-r--r--  2.0 unx     3706 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiBranch.class
--rw-r--r--  2.0 unx    14169 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Pipeline.class
--rw-r--r--  2.0 unx     1676 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ConnectBefore.class
--rw-r--r--  2.0 unx     1134 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/MultiMerge$1.class
--rw-r--r--  2.0 unx     1423 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Block$PipelineTiming.class
--rw-r--r--  2.0 unx     2863 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer$GenericTypeGetter.class
--rw-r--r--  2.0 unx     1277 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDebugger.class
--rw-r--r--  2.0 unx    10019 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer.class
--rw-r--r--  2.0 unx      418 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/CheckedFunction.class
--rw-r--r--  2.0 unx     3089 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Block.class
--rw-r--r--  2.0 unx     2125 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/ConnectAfter.class
--rw-r--r--  2.0 unx     1100 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/pipelines/Merge$2.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Pipelines/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/debuging/drawing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-12 00:36 META-INF/maven/io.github.gustiks/Pipelines/
+-rw-r--r--  2.0 unx     4682 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/MultiMerge.class
+-rw-r--r--  2.0 unx     7115 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Pipe.class
+-rw-r--r--  2.0 unx     3163 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/ParallelPipe.class
+-rw-r--r--  2.0 unx      958 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Pipe$1.class
+-rw-r--r--  2.0 unx      375 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/CheckedSupplier.class
+-rw-r--r--  2.0 unx      992 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Branch$1.class
+-rw-r--r--  2.0 unx      380 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/CheckedConsumer.class
+-rw-r--r--  2.0 unx      986 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/ParallelPipe$1.class
+-rw-r--r--  2.0 unx     2012 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/bulding/AbstractPipelineBuilder.class
+-rw-r--r--  2.0 unx     6601 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Branch.class
+-rw-r--r--  2.0 unx     1109 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Merge$3.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Merge$1.class
+-rw-r--r--  2.0 unx     6552 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Merge.class
+-rw-r--r--  2.0 unx     1389 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/RecurrentPipe.class
+-rw-r--r--  2.0 unx      231 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Executable.class
+-rw-r--r--  2.0 unx     1609 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/StreamifyPipe.class
+-rw-r--r--  2.0 unx     1562 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/StreamParallelizationPipe.class
+-rw-r--r--  2.0 unx     1612 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateListBranch.class
+-rw-r--r--  2.0 unx     1416 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/ListMerge.class
+-rw-r--r--  2.0 unx     3053 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/ExportingPipe.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairExtractionBranch.class
+-rw-r--r--  2.0 unx     1612 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/LambdaPipe.class
+-rw-r--r--  2.0 unx     1664 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/SecondFromPairPipe.class
+-rw-r--r--  2.0 unx     1208 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/IdentityGenPipe.class
+-rw-r--r--  2.0 unx     1927 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairExtractionBranch.class
+-rw-r--r--  2.0 unx     1650 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/PairBranch.class
+-rw-r--r--  2.0 unx     1460 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/ListBranch.class
+-rw-r--r--  2.0 unx     1659 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/FirstFromPairPipe.class
+-rw-r--r--  2.0 unx     1387 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/DuplicateBranch.class
+-rw-r--r--  2.0 unx     1683 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/pipes/generic/PairMerge.class
+-rw-r--r--  2.0 unx     3706 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/MultiBranch.class
+-rw-r--r--  2.0 unx    14169 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Pipeline.class
+-rw-r--r--  2.0 unx     1676 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/ConnectBefore.class
+-rw-r--r--  2.0 unx     1134 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/MultiMerge$1.class
+-rw-r--r--  2.0 unx     1423 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Block$PipelineTiming.class
+-rw-r--r--  2.0 unx     2863 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer$GenericTypeGetter.class
+-rw-r--r--  2.0 unx     1277 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDebugger.class
+-rw-r--r--  2.0 unx    10019 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/debuging/drawing/PipelineDrawer.class
+-rw-r--r--  2.0 unx      418 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/CheckedFunction.class
+-rw-r--r--  2.0 unx     3089 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Block.class
+-rw-r--r--  2.0 unx     2125 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/ConnectAfter.class
+-rw-r--r--  2.0 unx     1100 b- defN 23-Nov-12 00:36 cz/cvut/fel/ida/pipelines/Merge$2.class
 -rw-r--r--  2.0 unx     1228 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Pipelines/pom.xml
 -rw-r--r--  2.0 unx      112 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Pipelines/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/
 -rw-r--r--  2.0 unx     5124 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow.class
 -rw-r--r--  2.0 unx     2614 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel$MouseListener.class
 -rw-r--r--  2.0 unx    11843 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/GraphViz.class
 -rw-r--r--  2.0 unx     3976 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/drawing/DrawWindow$ImagePanel.class
@@ -471,120 +465,122 @@
 -rw-r--r--  2.0 unx     2938 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/NormalFormatter.class
 -rw-r--r--  2.0 unx     5562 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/Logging.class
 -rw-r--r--  2.0 unx     1098 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/FlushStreamHandler.class
 -rw-r--r--  2.0 unx     3344 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logging/ColoredFormatter.class
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Logging/
 -rw-r--r--  2.0 unx     1017 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Logging/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logging/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/drawing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/utils/
--rw-r--r--  2.0 unx     1558 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$2.class
--rw-r--r--  2.0 unx     1406 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$3.class
--rw-r--r--  2.0 unx     3793 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder$1.class
--rw-r--r--  2.0 unx     2616 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$8.class
--rw-r--r--  2.0 unx     1791 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder.class
--rw-r--r--  2.0 unx     1841 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$6.class
--rw-r--r--  2.0 unx     2558 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$NeuralLearningBuilder.class
--rw-r--r--  2.0 unx     7192 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$LogicTrainTestBuilder.class
--rw-r--r--  2.0 unx     1346 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TestingBuilder$1.class
--rw-r--r--  2.0 unx     3186 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder$1.class
--rw-r--r--  2.0 unx     3003 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$1.class
--rw-r--r--  2.0 unx     2042 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$7.class
--rw-r--r--  2.0 unx     6818 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$NeuralTrainTestBuilder.class
--rw-r--r--  2.0 unx     1822 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$1.class
--rw-r--r--  2.0 unx     2939 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$10.class
--rw-r--r--  2.0 unx     2596 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$1.class
--rw-r--r--  2.0 unx     1395 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$4.class
--rw-r--r--  2.0 unx     5327 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder$1.class
--rw-r--r--  2.0 unx     7466 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder.class
--rw-r--r--  2.0 unx     2122 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$3.class
--rw-r--r--  2.0 unx     1757 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$7.class
--rw-r--r--  2.0 unx     1510 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$4.class
--rw-r--r--  2.0 unx     7849 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder.class
--rw-r--r--  2.0 unx    27709 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder.class
--rw-r--r--  2.0 unx     2430 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TestingBuilder$NeuralTestingBuilder.class
--rw-r--r--  2.0 unx     3078 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder$1.class
--rw-r--r--  2.0 unx     6077 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/GroundingBuilder.class
--rw-r--r--  2.0 unx     7579 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder.class
--rw-r--r--  2.0 unx     6105 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder.class
--rw-r--r--  2.0 unx     1025 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder$1.class
--rw-r--r--  2.0 unx     2970 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$9.class
--rw-r--r--  2.0 unx     6351 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TestingBuilder.class
--rw-r--r--  2.0 unx     7794 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder.class
--rw-r--r--  2.0 unx     2383 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$2.class
--rw-r--r--  2.0 unx     2455 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$5.class
--rw-r--r--  2.0 unx     2105 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$6.class
--rw-r--r--  2.0 unx     8748 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder.class
--rw-r--r--  2.0 unx     5986 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$StructureTrainTestBuilder.class
--rw-r--r--  2.0 unx     2190 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$4.class
--rw-r--r--  2.0 unx     7030 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainingBuilder.class
--rw-r--r--  2.0 unx    17171 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/PythonBuilder.class
--rw-r--r--  2.0 unx     8874 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder.class
--rw-r--r--  2.0 unx     1720 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$8.class
--rw-r--r--  2.0 unx     1358 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$2.class
--rw-r--r--  2.0 unx     7508 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder.class
--rw-r--r--  2.0 unx     1511 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$2.class
--rw-r--r--  2.0 unx     2385 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$3.class
--rw-r--r--  2.0 unx     3801 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$5.class
--rw-r--r--  2.0 unx     1847 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$1.class
--rw-r--r--  2.0 unx     8130 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder$End2endNNBuilder.class
--rw-r--r--  2.0 unx     9130 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder.class
--rw-r--r--  2.0 unx     1518 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder$1.class
--rw-r--r--  2.0 unx     1819 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class
--rw-r--r--  2.0 unx     1524 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3$1.class
--rw-r--r--  2.0 unx     4125 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/GroundingDebugger.class
--rw-r--r--  2.0 unx     1462 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$1.class
--rw-r--r--  2.0 unx     6572 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger.class
--rw-r--r--  2.0 unx     2427 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$2.class
--rw-r--r--  2.0 unx     5603 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/TrainingDebugger.class
--rw-r--r--  2.0 unx    12872 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer$NeuronDrawer.class
--rw-r--r--  2.0 unx     7488 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/drawing/GroundingDrawer.class
--rw-r--r--  2.0 unx     9294 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/drawing/TemplateDrawer.class
--rw-r--r--  2.0 unx     4996 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer.class
--rw-r--r--  2.0 unx     1699 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3.class
--rw-r--r--  2.0 unx     4938 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/NeuralDebugger.class
--rw-r--r--  2.0 unx     3091 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/SampleDebugger.class
--rw-r--r--  2.0 unx     3637 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/debugging/TemplateDebugger.class
--rw-r--r--  2.0 unx     3630 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/CycleBreakingPipe.class
--rw-r--r--  2.0 unx     5816 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/GroundingSampleWrappingPipe.class
--rw-r--r--  2.0 unx     6781 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/NetworkFinalizationPipe.class
--rw-r--r--  2.0 unx     4329 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralTrainingPipe.class
--rw-r--r--  2.0 unx     7867 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralEvaluationPipe.class
--rw-r--r--  2.0 unx     2222 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/GlobalSharingGroundingPipe.class
--rw-r--r--  2.0 unx     3760 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/EdgeMergerPipe.class
--rw-r--r--  2.0 unx     4052 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/SequentiallySharedGroundingPipe.class
--rw-r--r--  2.0 unx     2838 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/TrainingResultTemplateMerge.class
--rw-r--r--  2.0 unx     6896 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/PruningPipe.class
--rw-r--r--  2.0 unx     6763 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/CompressionPipe.class
--rw-r--r--  2.0 unx     3146 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedGroundTemplatePruningPipe.class
--rw-r--r--  2.0 unx     2830 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/TemplateToNeuralPipe.class
--rw-r--r--  2.0 unx     5881 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedNeuralizationPipe.class
--rw-r--r--  2.0 unx     3931 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/StandardGroundingPipe.class
--rw-r--r--  2.0 unx     1712 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/ResultsFromProgressPipe.class
--rw-r--r--  2.0 unx     4576 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralSerializerPipe.class
--rw-r--r--  2.0 unx     2944 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedTemplateReducingPipe.class
--rw-r--r--  2.0 unx     1742 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/pipelines/utils/WorkflowUtils.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/drawing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
+-rw-r--r--  2.0 unx     1558 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$2.class
+-rw-r--r--  2.0 unx     1406 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$3.class
+-rw-r--r--  2.0 unx     3793 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder$1.class
+-rw-r--r--  2.0 unx     2616 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$8.class
+-rw-r--r--  2.0 unx     1791 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder.class
+-rw-r--r--  2.0 unx     1841 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$6.class
+-rw-r--r--  2.0 unx     2558 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$NeuralLearningBuilder.class
+-rw-r--r--  2.0 unx     7192 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$LogicTrainTestBuilder.class
+-rw-r--r--  2.0 unx     1346 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TestingBuilder$1.class
+-rw-r--r--  2.0 unx     3186 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder$1.class
+-rw-r--r--  2.0 unx     3003 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$1.class
+-rw-r--r--  2.0 unx     2042 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$7.class
+-rw-r--r--  2.0 unx     6818 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$NeuralTrainTestBuilder.class
+-rw-r--r--  2.0 unx     1822 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$1.class
+-rw-r--r--  2.0 unx     2939 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$10.class
+-rw-r--r--  2.0 unx     6345 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/PythonBuilder$PythonNeuralizationPipeline.class
+-rw-r--r--  2.0 unx     2596 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$1.class
+-rw-r--r--  2.0 unx     1395 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$4.class
+-rw-r--r--  2.0 unx     5327 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder$1.class
+-rw-r--r--  2.0 unx     7466 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder.class
+-rw-r--r--  2.0 unx     2122 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$3.class
+-rw-r--r--  2.0 unx     1757 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$7.class
+-rw-r--r--  2.0 unx     1510 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$4.class
+-rw-r--r--  2.0 unx     7849 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder.class
+-rw-r--r--  2.0 unx    27709 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder.class
+-rw-r--r--  2.0 unx     2430 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TestingBuilder$NeuralTestingBuilder.class
+-rw-r--r--  2.0 unx     3078 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder$1.class
+-rw-r--r--  2.0 unx     6077 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/GroundingBuilder.class
+-rw-r--r--  2.0 unx     7579 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder.class
+-rw-r--r--  2.0 unx     6105 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TestingBuilder$LogicTestingBuilder.class
+-rw-r--r--  2.0 unx     1025 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder$StructureLearningBuilder$1.class
+-rw-r--r--  2.0 unx     2970 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$9.class
+-rw-r--r--  2.0 unx     6351 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TestingBuilder.class
+-rw-r--r--  2.0 unx     7794 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder.class
+-rw-r--r--  2.0 unx     2383 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$2.class
+-rw-r--r--  2.0 unx     2455 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$5.class
+-rw-r--r--  2.0 unx     2105 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$6.class
+-rw-r--r--  2.0 unx     8748 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder.class
+-rw-r--r--  2.0 unx     5986 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$StructureTrainTestBuilder.class
+-rw-r--r--  2.0 unx     2190 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$4.class
+-rw-r--r--  2.0 unx     7030 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainingBuilder.class
+-rw-r--r--  2.0 unx     7366 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/PythonBuilder.class
+-rw-r--r--  2.0 unx     8874 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateSamplesBuilder.class
+-rw-r--r--  2.0 unx     1720 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$8.class
+-rw-r--r--  2.0 unx     1358 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$2.class
+-rw-r--r--  2.0 unx     7508 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder.class
+-rw-r--r--  2.0 unx     1511 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$2.class
+-rw-r--r--  2.0 unx     2385 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$3.class
+-rw-r--r--  2.0 unx     3801 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/SamplesProcessingBuilder$5.class
+-rw-r--r--  2.0 unx     1847 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TrainTestBuilder$1.class
+-rw-r--r--  2.0 unx     8130 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder$End2endNNBuilder.class
+-rw-r--r--  2.0 unx     9130 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/End2endTrainigBuilder.class
+-rw-r--r--  2.0 unx     1518 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder$1.class
+-rw-r--r--  2.0 unx     1819 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class
+-rw-r--r--  2.0 unx     5998 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/building/PythonBuilder$PythonGroundingPipeline.class
+-rw-r--r--  2.0 unx     1524 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3$1.class
+-rw-r--r--  2.0 unx     4125 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/GroundingDebugger.class
+-rw-r--r--  2.0 unx     1462 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$1.class
+-rw-r--r--  2.0 unx     6572 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger.class
+-rw-r--r--  2.0 unx     2427 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$2.class
+-rw-r--r--  2.0 unx     5603 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/TrainingDebugger.class
+-rw-r--r--  2.0 unx    12823 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer$NeuronDrawer.class
+-rw-r--r--  2.0 unx     7658 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/drawing/GroundingDrawer.class
+-rw-r--r--  2.0 unx     9294 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/drawing/TemplateDrawer.class
+-rw-r--r--  2.0 unx     5098 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer.class
+-rw-r--r--  2.0 unx     1699 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3.class
+-rw-r--r--  2.0 unx     4938 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/NeuralDebugger.class
+-rw-r--r--  2.0 unx     3091 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/SampleDebugger.class
+-rw-r--r--  2.0 unx     3637 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/debugging/TemplateDebugger.class
+-rw-r--r--  2.0 unx     3630 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/CycleBreakingPipe.class
+-rw-r--r--  2.0 unx     5816 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/GroundingSampleWrappingPipe.class
+-rw-r--r--  2.0 unx     6781 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/NetworkFinalizationPipe.class
+-rw-r--r--  2.0 unx     4329 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralTrainingPipe.class
+-rw-r--r--  2.0 unx     7867 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralEvaluationPipe.class
+-rw-r--r--  2.0 unx     2222 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/GlobalSharingGroundingPipe.class
+-rw-r--r--  2.0 unx     3760 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/EdgeMergerPipe.class
+-rw-r--r--  2.0 unx     4052 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/SequentiallySharedGroundingPipe.class
+-rw-r--r--  2.0 unx     2838 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/TrainingResultTemplateMerge.class
+-rw-r--r--  2.0 unx     6896 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/PruningPipe.class
+-rw-r--r--  2.0 unx     6763 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/CompressionPipe.class
+-rw-r--r--  2.0 unx     3146 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedGroundTemplatePruningPipe.class
+-rw-r--r--  2.0 unx     2830 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/TemplateToNeuralPipe.class
+-rw-r--r--  2.0 unx     5881 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedNeuralizationPipe.class
+-rw-r--r--  2.0 unx     3931 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/StandardGroundingPipe.class
+-rw-r--r--  2.0 unx     1712 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/ResultsFromProgressPipe.class
+-rw-r--r--  2.0 unx     4576 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/NeuralSerializerPipe.class
+-rw-r--r--  2.0 unx     2944 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedTemplateReducingPipe.class
+-rw-r--r--  2.0 unx     1742 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/pipelines/utils/WorkflowUtils.class
 -rw-r--r--  2.0 unx     1857 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.xml
 -rw-r--r--  2.0 unx      122 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/building/factories/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/example/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:10 cz/cvut/fel/ida/logic/constructs/template/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/transforming/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/metadata/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:10 cz/cvut/fel/ida/logic/constructs/template/components/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/bottomUp/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:10 cz/cvut/fel/ida/logic/grounding/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:10 cz/cvut/fel/ida/logic/grounding/bottomUp/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/topDown/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/constructs/
 -rw-r--r--  2.0 unx     3021 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/building/factories/ConstantFactory.class
 -rw-r--r--  2.0 unx     3015 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/building/factories/VariableFactory.class
 -rw-r--r--  2.0 unx     5412 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/building/factories/WeightedPredicateFactory.class
 -rw-r--r--  2.0 unx     5579 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/building/factories/WeightFactory.class
 -rw-r--r--  2.0 unx     1548 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/Conjunction.class
@@ -601,170 +597,170 @@
 -rw-r--r--  2.0 unx     1162 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/transforming/SimpleTemplateMerger.class
 -rw-r--r--  2.0 unx     1723 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateChainReducer.class
 -rw-r--r--  2.0 unx      343 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateMerging.class
 -rw-r--r--  2.0 unx     1095 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/transforming/TemplateReducing.class
 -rw-r--r--  2.0 unx     1729 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/metadata/TemplateMetadata.class
 -rw-r--r--  2.0 unx     5785 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/metadata/RuleMetadata.class
 -rw-r--r--  2.0 unx     6331 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/metadata/PredicateMetadata.class
--rw-r--r--  2.0 unx     2992 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/GroundRule.class
+-rw-r--r--  2.0 unx     2992 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/logic/constructs/template/components/GroundRule.class
 -rw-r--r--  2.0 unx     1664 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/HeadAtom.class
 -rw-r--r--  2.0 unx     2452 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/BodyAtom.class
--rw-r--r--  2.0 unx    10020 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/WeightedRule.class
+-rw-r--r--  2.0 unx    10020 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/logic/constructs/template/components/WeightedRule.class
 -rw-r--r--  2.0 unx     2414 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/components/GroundHeadRule.class
--rw-r--r--  2.0 unx    11218 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/Template.class
+-rw-r--r--  2.0 unx    11218 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/logic/constructs/template/Template.class
 -rw-r--r--  2.0 unx     4812 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$Stratification.class
 -rw-r--r--  2.0 unx     1737 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/ParsedTemplate.class
 -rw-r--r--  2.0 unx     1016 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/RichLogicTemplate.class
 -rw-r--r--  2.0 unx     8405 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate.class
 -rw-r--r--  2.0 unx     2092 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/constructs/template/types/GraphTemplate$UnsignedLiteral.class
 -rw-r--r--  2.0 unx    14044 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/Grounder.class
--rw-r--r--  2.0 unx    17765 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class
+-rw-r--r--  2.0 unx    18204 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class
 -rw-r--r--  2.0 unx    21335 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/topDown/Gringo.class
 -rw-r--r--  2.0 unx     1196 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/topDown/TopDown.class
 -rw-r--r--  2.0 unx      297 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$1.class
 -rw-r--r--  2.0 unx     1974 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection.class
 -rw-r--r--  2.0 unx     1112 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionDuplicit.class
 -rw-r--r--  2.0 unx     1109 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/constructs/GroundRulesCollection$GroundRulesCollectionUnique.class
 -rw-r--r--  2.0 unx     1610 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/GroundingSample.class
 -rw-r--r--  2.0 unx    10533 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/GroundTemplate.class
 -rw-r--r--  2.0 unx     1529 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/GroundingSample$Wrap.class
 -rw-r--r--  2.0 unx      885 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/grounding/Grounder$1.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/Logical/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 23:12 META-INF/maven/io.github.gustiks/Logical/
 -rw-r--r--  2.0 unx     1422 b- defN 22-Sep-14 19:24 META-INF/maven/io.github.gustiks/Logical/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logical/pom.properties
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/weights/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/inits/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:22 cz/cvut/fel/ida/algebra/functions/transformation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/error/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/
--rw-r--r--  2.0 unx      978 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/weights/ScalarWeight.class
--rw-r--r--  2.0 unx     3795 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/weights/Weight.class
--rw-r--r--  2.0 unx     1304 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/weights/StatefulWeight.class
--rw-r--r--  2.0 unx     2059 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/Parameter.class
--rw-r--r--  2.0 unx     1573 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/Parameter$Type.class
--rw-r--r--  2.0 unx     2994 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue.class
--rw-r--r--  2.0 unx     3813 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/Metadata.class
--rw-r--r--  2.0 unx     1512 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue$Type.class
--rw-r--r--  2.0 unx     4379 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/metadata/WeightMetadata.class
--rw-r--r--  2.0 unx     4509 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/utils/MathUtils.class
--rw-r--r--  2.0 unx    14886 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/ScalarValue.class
--rw-r--r--  2.0 unx     4553 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/Value.class
--rw-r--r--  2.0 unx    20912 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/MatrixValue.class
--rw-r--r--  2.0 unx     7790 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/StringValue.class
--rw-r--r--  2.0 unx     9025 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/TensorValue.class
--rw-r--r--  2.0 unx     2060 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/inits/SimpleInitializer.class
--rw-r--r--  2.0 unx     1609 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/inits/HeUniformInitializer.class
--rw-r--r--  2.0 unx     1285 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/inits/ValueInitializer.class
--rw-r--r--  2.0 unx     2726 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/inits/GlorotUniformInitializer.class
--rw-r--r--  2.0 unx     9459 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/Zero.class
--rw-r--r--  2.0 unx      990 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/Constant.class
--rw-r--r--  2.0 unx     1172 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/Longtail.class
--rw-r--r--  2.0 unx     1142 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/Uniform.class
--rw-r--r--  2.0 unx      978 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/Normal.class
--rw-r--r--  2.0 unx     2045 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/distributions/Distribution.class
--rw-r--r--  2.0 unx     1214 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/MatrixValue$ValueIterator.class
--rw-r--r--  2.0 unx     1137 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/VectorValue$ValueIterator.class
--rw-r--r--  2.0 unx     1129 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/ScalarValue$ValueIterator.class
--rw-r--r--  2.0 unx    23137 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/VectorValue.class
--rw-r--r--  2.0 unx     1415 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/Tensor.class
--rw-r--r--  2.0 unx     9847 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/values/One.class
--rw-r--r--  2.0 unx     2071 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex$State.class
--rw-r--r--  2.0 unx     2351 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape.class
--rw-r--r--  2.0 unx     4051 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization.class
--rw-r--r--  2.0 unx     2178 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape$State.class
--rw-r--r--  2.0 unx     3344 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization$State.class
--rw-r--r--  2.0 unx     2620 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex.class
--rw-r--r--  2.0 unx     2692 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition.class
--rw-r--r--  2.0 unx     2799 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice.class
--rw-r--r--  2.0 unx     1072 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity$State.class
--rw-r--r--  2.0 unx     1142 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne$State.class
--rw-r--r--  2.0 unx     2630 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice$State.class
--rw-r--r--  2.0 unx     1767 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity.class
--rw-r--r--  2.0 unx     1074 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition$State.class
--rw-r--r--  2.0 unx      316 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/XMax.class
--rw-r--r--  2.0 unx     1925 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne.class
--rw-r--r--  2.0 unx     2447 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/ReLu.class
--rw-r--r--  2.0 unx     2617 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LeakyReLu.class
--rw-r--r--  2.0 unx     2431 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Tanh.class
--rw-r--r--  2.0 unx     2421 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Inverse.class
--rw-r--r--  2.0 unx     2283 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Exponentiation.class
--rw-r--r--  2.0 unx     2505 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Reverse.class
--rw-r--r--  2.0 unx     2395 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/SquareRoot.class
--rw-r--r--  2.0 unx     2020 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Signum.class
--rw-r--r--  2.0 unx     2668 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LukasiewiczSigmoid.class
--rw-r--r--  2.0 unx     2374 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Logarithm.class
--rw-r--r--  2.0 unx     2597 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Sigmoid.class
--rw-r--r--  2.0 unx     1466 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Aggregation$Singletons.class
--rw-r--r--  2.0 unx     2558 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ActivationFcn$SimpleValueState.class
--rw-r--r--  2.0 unx     3079 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Combination.class
--rw-r--r--  2.0 unx     2232 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/error/SquaredDiff.class
--rw-r--r--  2.0 unx     3780 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/error/Crossentropy.class
--rw-r--r--  2.0 unx     3423 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/error/SoftEntropy.class
--rw-r--r--  2.0 unx     1029 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Transformation$1.class
--rw-r--r--  2.0 unx     1191 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Aggregation$State.class
--rw-r--r--  2.0 unx     3432 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ActivationFcn$State.class
--rw-r--r--  2.0 unx     3235 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Transformation$State.class
--rw-r--r--  2.0 unx      733 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Average$TransformationState.class
--rw-r--r--  2.0 unx     2280 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$TransformationState.class
--rw-r--r--  2.0 unx     3693 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Average.class
--rw-r--r--  2.0 unx     1877 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Count$AggregationState.class
--rw-r--r--  2.0 unx     4628 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum.class
--rw-r--r--  2.0 unx     1011 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Count$TransformationState.class
--rw-r--r--  2.0 unx      942 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$TransformationState.class
--rw-r--r--  2.0 unx     4628 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum.class
--rw-r--r--  2.0 unx     2279 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$TransformationState.class
--rw-r--r--  2.0 unx     2228 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Average$AggregationState.class
--rw-r--r--  2.0 unx     1410 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$AggregationState.class
--rw-r--r--  2.0 unx     3373 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Count.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$AggregationState.class
--rw-r--r--  2.0 unx     1811 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$AggregationState.class
--rw-r--r--  2.0 unx     3517 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/aggregation/Sum.class
--rw-r--r--  2.0 unx     1079 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State$Mapping.class
--rw-r--r--  2.0 unx     2382 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Product$State.class
--rw-r--r--  2.0 unx     4343 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Sparsemax.class
--rw-r--r--  2.0 unx     4078 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/CosineSim$State.class
--rw-r--r--  2.0 unx     2480 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Concatenation$State.class
--rw-r--r--  2.0 unx     2213 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Softmax$CombinationState.class
--rw-r--r--  2.0 unx     5670 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Concatenation.class
--rw-r--r--  2.0 unx     1632 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$TransformationState.class
--rw-r--r--  2.0 unx     1959 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$AggregationState.class
--rw-r--r--  2.0 unx     1596 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Softmax$TransformationState.class
--rw-r--r--  2.0 unx     4064 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct.class
--rw-r--r--  2.0 unx     2491 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Product.class
--rw-r--r--  2.0 unx     4103 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/CosineSim.class
--rw-r--r--  2.0 unx     6081 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/Softmax.class
--rw-r--r--  2.0 unx     3474 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/CrossSum.class
--rw-r--r--  2.0 unx     4817 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State.class
--rw-r--r--  2.0 unx     1521 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Combination$Singletons.class
--rw-r--r--  2.0 unx     1191 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ElementWise$State.class
--rw-r--r--  2.0 unx     2671 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ElementWise$Singletons.class
--rw-r--r--  2.0 unx      365 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ErrorFcn.class
--rw-r--r--  2.0 unx     1247 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Combination$State.class
--rw-r--r--  2.0 unx     1614 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Transformation$Singletons.class
--rw-r--r--  2.0 unx     1036 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Aggregation$1.class
--rw-r--r--  2.0 unx     1695 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Combination$InputArrayState.class
--rw-r--r--  2.0 unx     3830 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/CompoundState.class
--rw-r--r--  2.0 unx     2482 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Transformation.class
--rw-r--r--  2.0 unx     1319 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ActivationFcn.class
--rw-r--r--  2.0 unx     2363 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Aggregation.class
--rw-r--r--  2.0 unx     1309 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ElementWise$1.class
--rw-r--r--  2.0 unx     3856 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/ElementWise.class
--rw-r--r--  2.0 unx     1107 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/algebra/functions/Combination$1.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/Algebra/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:21 cz/cvut/fel/ida/algebra/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/weights/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/inits/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:21 cz/cvut/fel/ida/algebra/functions/transformation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/error/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 META-INF/maven/io.github.gustiks/Algebra/
+-rw-r--r--  2.0 unx      978 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/weights/ScalarWeight.class
+-rw-r--r--  2.0 unx     3837 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/weights/Weight.class
+-rw-r--r--  2.0 unx     1304 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/weights/StatefulWeight.class
+-rw-r--r--  2.0 unx     2059 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/Parameter.class
+-rw-r--r--  2.0 unx     1573 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/Parameter$Type.class
+-rw-r--r--  2.0 unx     2994 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue.class
+-rw-r--r--  2.0 unx     3813 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/Metadata.class
+-rw-r--r--  2.0 unx     1512 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/ParameterValue$Type.class
+-rw-r--r--  2.0 unx     4379 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/metadata/WeightMetadata.class
+-rw-r--r--  2.0 unx     4509 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/utils/MathUtils.class
+-rw-r--r--  2.0 unx    14886 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/ScalarValue.class
+-rw-r--r--  2.0 unx     4553 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/Value.class
+-rw-r--r--  2.0 unx    20912 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/MatrixValue.class
+-rw-r--r--  2.0 unx     7790 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/StringValue.class
+-rw-r--r--  2.0 unx     9025 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/TensorValue.class
+-rw-r--r--  2.0 unx     2060 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/inits/SimpleInitializer.class
+-rw-r--r--  2.0 unx     1609 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/inits/HeUniformInitializer.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/inits/ValueInitializer.class
+-rw-r--r--  2.0 unx     2726 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/inits/GlorotUniformInitializer.class
+-rw-r--r--  2.0 unx     9459 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/Zero.class
+-rw-r--r--  2.0 unx      990 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/Constant.class
+-rw-r--r--  2.0 unx     1172 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/Longtail.class
+-rw-r--r--  2.0 unx     1142 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/Uniform.class
+-rw-r--r--  2.0 unx      978 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/Normal.class
+-rw-r--r--  2.0 unx     2045 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/distributions/Distribution.class
+-rw-r--r--  2.0 unx     1214 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/MatrixValue$ValueIterator.class
+-rw-r--r--  2.0 unx     1137 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/VectorValue$ValueIterator.class
+-rw-r--r--  2.0 unx     1129 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/ScalarValue$ValueIterator.class
+-rw-r--r--  2.0 unx    23137 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/VectorValue.class
+-rw-r--r--  2.0 unx     1415 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/Tensor.class
+-rw-r--r--  2.0 unx     9847 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/values/One.class
+-rw-r--r--  2.0 unx     2071 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex$State.class
+-rw-r--r--  2.0 unx     2351 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape.class
+-rw-r--r--  2.0 unx     4051 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization.class
+-rw-r--r--  2.0 unx     2178 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Reshape$State.class
+-rw-r--r--  2.0 unx     3344 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Normalization$State.class
+-rw-r--r--  2.0 unx     2620 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/AtIndex.class
+-rw-r--r--  2.0 unx     2692 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition.class
+-rw-r--r--  2.0 unx     2799 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice.class
+-rw-r--r--  2.0 unx     1072 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity$State.class
+-rw-r--r--  2.0 unx     1142 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne$State.class
+-rw-r--r--  2.0 unx     2630 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Slice$State.class
+-rw-r--r--  2.0 unx     1767 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Identity.class
+-rw-r--r--  2.0 unx     1074 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/Transposition$State.class
+-rw-r--r--  2.0 unx      316 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/XMax.class
+-rw-r--r--  2.0 unx     1925 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/joint/ConstantOne.class
+-rw-r--r--  2.0 unx     2447 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/ReLu.class
+-rw-r--r--  2.0 unx     2617 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LeakyReLu.class
+-rw-r--r--  2.0 unx     2431 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Tanh.class
+-rw-r--r--  2.0 unx     2421 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Inverse.class
+-rw-r--r--  2.0 unx     2283 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Exponentiation.class
+-rw-r--r--  2.0 unx     2505 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Reverse.class
+-rw-r--r--  2.0 unx     2395 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/SquareRoot.class
+-rw-r--r--  2.0 unx     2020 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Signum.class
+-rw-r--r--  2.0 unx     2668 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/LukasiewiczSigmoid.class
+-rw-r--r--  2.0 unx     2374 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Logarithm.class
+-rw-r--r--  2.0 unx     2597 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/transformation/elementwise/Sigmoid.class
+-rw-r--r--  2.0 unx     1466 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Aggregation$Singletons.class
+-rw-r--r--  2.0 unx     2558 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ActivationFcn$SimpleValueState.class
+-rw-r--r--  2.0 unx     3079 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Combination.class
+-rw-r--r--  2.0 unx     2232 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/error/SquaredDiff.class
+-rw-r--r--  2.0 unx     3780 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/error/Crossentropy.class
+-rw-r--r--  2.0 unx     3423 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/error/SoftEntropy.class
+-rw-r--r--  2.0 unx     1029 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Transformation$1.class
+-rw-r--r--  2.0 unx     1191 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Aggregation$State.class
+-rw-r--r--  2.0 unx     3432 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ActivationFcn$State.class
+-rw-r--r--  2.0 unx     3235 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Transformation$State.class
+-rw-r--r--  2.0 unx      733 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Average$TransformationState.class
+-rw-r--r--  2.0 unx     2280 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$TransformationState.class
+-rw-r--r--  2.0 unx     3693 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Average.class
+-rw-r--r--  2.0 unx     1877 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Count$AggregationState.class
+-rw-r--r--  2.0 unx     4628 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum.class
+-rw-r--r--  2.0 unx     1011 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Count$TransformationState.class
+-rw-r--r--  2.0 unx      942 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$TransformationState.class
+-rw-r--r--  2.0 unx     4628 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum.class
+-rw-r--r--  2.0 unx     2279 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$TransformationState.class
+-rw-r--r--  2.0 unx     2228 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Average$AggregationState.class
+-rw-r--r--  2.0 unx     1410 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Sum$AggregationState.class
+-rw-r--r--  2.0 unx     3373 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Count.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Maximum$AggregationState.class
+-rw-r--r--  2.0 unx     1811 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Minimum$AggregationState.class
+-rw-r--r--  2.0 unx     3517 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/aggregation/Sum.class
+-rw-r--r--  2.0 unx     1079 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State$Mapping.class
+-rw-r--r--  2.0 unx     2382 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Product$State.class
+-rw-r--r--  2.0 unx     4343 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Sparsemax.class
+-rw-r--r--  2.0 unx     4078 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/CosineSim$State.class
+-rw-r--r--  2.0 unx     2480 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Concatenation$State.class
+-rw-r--r--  2.0 unx     2213 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Softmax$CombinationState.class
+-rw-r--r--  2.0 unx     5670 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Concatenation.class
+-rw-r--r--  2.0 unx     1632 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$TransformationState.class
+-rw-r--r--  2.0 unx     1959 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct$AggregationState.class
+-rw-r--r--  2.0 unx     1596 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Softmax$TransformationState.class
+-rw-r--r--  2.0 unx     4064 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/ElementProduct.class
+-rw-r--r--  2.0 unx     2491 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Product.class
+-rw-r--r--  2.0 unx     4103 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/CosineSim.class
+-rw-r--r--  2.0 unx     6081 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/Softmax.class
+-rw-r--r--  2.0 unx     3474 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/CrossSum.class
+-rw-r--r--  2.0 unx     4817 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/combination/CrossSum$State.class
+-rw-r--r--  2.0 unx     1521 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Combination$Singletons.class
+-rw-r--r--  2.0 unx     1191 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ElementWise$State.class
+-rw-r--r--  2.0 unx     2671 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ElementWise$Singletons.class
+-rw-r--r--  2.0 unx      365 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ErrorFcn.class
+-rw-r--r--  2.0 unx     1247 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Combination$State.class
+-rw-r--r--  2.0 unx     1614 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Transformation$Singletons.class
+-rw-r--r--  2.0 unx     1036 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Aggregation$1.class
+-rw-r--r--  2.0 unx     1695 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Combination$InputArrayState.class
+-rw-r--r--  2.0 unx     3830 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/CompoundState.class
+-rw-r--r--  2.0 unx     2482 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Transformation.class
+-rw-r--r--  2.0 unx     1319 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ActivationFcn.class
+-rw-r--r--  2.0 unx     2363 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Aggregation.class
+-rw-r--r--  2.0 unx     1309 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ElementWise$1.class
+-rw-r--r--  2.0 unx     3856 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/ElementWise.class
+-rw-r--r--  2.0 unx     1107 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/algebra/functions/Combination$1.class
 -rw-r--r--  2.0 unx     1658 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Algebra/pom.xml
--rw-r--r--  2.0 unx      110 b- defN 23-Apr-07 21:22 META-INF/maven/io.github.gustiks/Algebra/pom.properties
+-rw-r--r--  2.0 unx      110 b- defN 23-Apr-07 21:21 META-INF/maven/io.github.gustiks/Algebra/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 20-Feb-14 14:23 org/jetbrains/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Feb-14 14:23 org/jetbrains/annotations/
 -rw-r--r--  2.0 unx     1220 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nls$Capitalization.class
 -rw-r--r--  2.0 unx      787 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nls.class
 -rw-r--r--  2.0 unx      703 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/NotNull.class
 -rw-r--r--  2.0 unx      564 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Nullable.class
 -rw-r--r--  2.0 unx      463 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Range.class
@@ -812,37 +808,37 @@
 -rw-r--r--  2.0 unx      443 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Async.class
 -rw-r--r--  2.0 unx      577 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Contract.class
 -rw-r--r--  2.0 unx      931 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Debug$Renderer.class
 -rw-r--r--  2.0 unx      380 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/Debug.class
 -rw-r--r--  2.0 unx      508 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/NonNls.class
 -rw-r--r--  2.0 unx      525 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/PropertyKey.class
 -rw-r--r--  2.0 unx      478 b- defN 20-Feb-14 14:23 org/jetbrains/annotations/TestOnly.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/io/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/logic/special/
 -rw-r--r--  2.0 unx     4849 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/ParserUtils.class
 -rw-r--r--  2.0 unx     1447 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/Matching$1.class
 -rw-r--r--  2.0 unx     7011 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionUtils.class
 -rw-r--r--  2.0 unx     9526 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseE.class
 -rw-r--r--  2.0 unx      419 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SymmetricPredicates.class
 -rw-r--r--  2.0 unx      230 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SolutionConsumer.class
 -rw-r--r--  2.0 unx     7696 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/MaxCardXorConstraint.class
--rw-r--r--  2.0 unx      829 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap.class
--rw-r--r--  2.0 unx      255 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$1.class
+-rw-r--r--  2.0 unx      829 b- defN 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$HerbrandMap.class
+-rw-r--r--  2.0 unx      255 b- defN 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$1.class
 -rw-r--r--  2.0 unx     1633 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$2.class
 -rw-r--r--  2.0 unx    20139 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/ApproximateSubsetCounter.class
 -rw-r--r--  2.0 unx     3022 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$LowArityLiterals.class
--rw-r--r--  2.0 unx     1696 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$TupleNotIn.class
--rw-r--r--  2.0 unx     1889 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer.class
+-rw-r--r--  2.0 unx     1696 b- defN 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$TupleNotIn.class
+-rw-r--r--  2.0 unx     1889 b- defN 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/HerbrandModel$PredicateSolutionConsumer.class
 -rw-r--r--  2.0 unx      242 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/CustomPredicate.class
 -rw-r--r--  2.0 unx     2592 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SpecialBinaryPredicates.class
 -rw-r--r--  2.0 unx    35709 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2.class
 -rw-r--r--  2.0 unx     2851 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SpecialVarargPredicates.class
 -rw-r--r--  2.0 unx      559 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseStructure.class
--rw-r--r--  2.0 unx    11304 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/HerbrandModel.class
+-rw-r--r--  2.0 unx    11304 b- defN 23-Oct-29 01:09 cz/cvut/fel/ida/logic/subsumption/HerbrandModel.class
 -rw-r--r--  2.0 unx     1447 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/Matching$2.class
 -rw-r--r--  2.0 unx     4726 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$CompletelySymmetricLiterals.class
 -rw-r--r--  2.0 unx    31343 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/Matching.class
 -rw-r--r--  2.0 unx      347 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/GlobalConstraint.class
 -rw-r--r--  2.0 unx     5595 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals.class
 -rw-r--r--  2.0 unx    16949 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$ClauseC.class
 -rw-r--r--  2.0 unx     1633 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/subsumption/SubsumptionEngineJ2$HighArityLiterals$1.class
@@ -870,15 +866,15 @@
 -rw-r--r--  2.0 unx    10537 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/special/IsoClauseWrapper.class
 -rw-r--r--  2.0 unx      255 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/LGG$LiteralFilter.class
 -rw-r--r--  2.0 unx     3717 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/LGG.class
 -rw-r--r--  2.0 unx      117 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/Formula.class
 -rw-r--r--  2.0 unx      480 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/Term.class
 -rw-r--r--  2.0 unx      201 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/LGG$1.class
 -rw-r--r--  2.0 unx     6976 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/logic/HornClause.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/Logic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 23:12 META-INF/maven/io.github.gustiks/Logic/
 -rw-r--r--  2.0 unx      799 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Logic/pom.xml
 -rw-r--r--  2.0 unx      108 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Logic/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/results/metrics/Jesse/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/learning/crossvalidation/
@@ -932,15 +928,15 @@
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/modes/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 01:10 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/networks/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/training/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/training/optimizers/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/training/strategies/
@@ -983,20 +979,20 @@
 -rw-r--r--  2.0 unx     7980 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Evaluation.class
 -rw-r--r--  2.0 unx      240 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonHookHandler.class
 -rw-r--r--  2.0 unx     7735 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation.class
 -rw-r--r--  2.0 unx     4789 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/IndependentNeuronProcessing.class
 -rw-r--r--  2.0 unx     7015 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/PythonEvaluation$PythonUp.class
 -rw-r--r--  2.0 unx     9314 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/actions/Backpropagation.class
 -rw-r--r--  2.0 unx     4808 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Accumulator.class
--rw-r--r--  2.0 unx     3204 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted.class
--rw-r--r--  2.0 unx     2353 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor.class
+-rw-r--r--  2.0 unx     3204 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted.class
+-rw-r--r--  2.0 unx     2353 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor.class
 -rw-r--r--  2.0 unx     6105 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Up.class
 -rw-r--r--  2.0 unx     8143 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/StateInitializer.class
--rw-r--r--  2.0 unx     3060 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Indexed.class
--rw-r--r--  2.0 unx     4156 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Detailed.class
+-rw-r--r--  2.0 unx     3060 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Indexed.class
+-rw-r--r--  2.0 unx     4156 b- defN 23-Oct-29 01:10 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/NeuronVisitor$Weighted$Detailed.class
 -rw-r--r--  2.0 unx     3493 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Independent.class
 -rw-r--r--  2.0 unx     6912 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/neurons/Down.class
 -rw-r--r--  2.0 unx     3217 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightUpdater.class
 -rw-r--r--  2.0 unx      278 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/weights/WeightVisitor.class
 -rw-r--r--  2.0 unx     1584 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Invalidator.class
 -rw-r--r--  2.0 unx     3408 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Dropouter.class
 -rw-r--r--  2.0 unx     3266 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/computation/iteration/visitors/states/neurons/Backproper.class
@@ -1127,128 +1123,128 @@
 -rw-r--r--  2.0 unx     5493 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets.class
 -rw-r--r--  2.0 unx      597 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/NeuralLayer.class
 -rw-r--r--  2.0 unx     1404 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/NeuralSets$NeuronCounter.class
 -rw-r--r--  2.0 unx     6209 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork.class
 -rw-r--r--  2.0 unx    14189 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/types/DetailedNetwork.class
 -rw-r--r--  2.0 unx     5981 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/types/TopologicNetwork$TopoSorting.class
 -rw-r--r--  2.0 unx     1037 b- defN 23-Oct-28 22:25 cz/cvut/fel/ida/neural/networks/structure/components/types/LayeredNetwork.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-28 22:25 META-INF/maven/io.github.gustiks/Neural/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Oct-29 23:12 META-INF/maven/io.github.gustiks/Neural/
 -rw-r--r--  2.0 unx     1390 b- defN 22-Nov-29 16:47 META-INF/maven/io.github.gustiks/Neural/pom.xml
 -rw-r--r--  2.0 unx      109 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Neural/pom.properties
 -rw-r--r--  2.0 unx    19407 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuronFactory.class
 -rw-r--r--  2.0 unx    27873 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralNetBuilder.class
 -rw-r--r--  2.0 unx     2247 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralBuilder.class
 -rw-r--r--  2.0 unx     5365 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuralProcessingSample.class
 -rw-r--r--  2.0 unx     4259 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/NeuronMaps.class
 -rw-r--r--  2.0 unx    22653 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/neural/networks/structure/building/Neuralizer.class
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Neuralization/
 -rw-r--r--  2.0 unx     1008 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Neuralization/pom.xml
 -rw-r--r--  2.0 unx      116 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Neuralization/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/examples/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/queries/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/
 drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/
--rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTree.class
--rw-r--r--  2.0 unx     1985 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/ExamplesParseTreeExtractor.class
--rw-r--r--  2.0 unx     8650 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class
--rw-r--r--  2.0 unx     1494 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTree.class
--rw-r--r--  2.0 unx     7281 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTreeExtractor.class
--rw-r--r--  2.0 unx     1740 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/queries/QueriesParseTreeExtractor.class
--rw-r--r--  2.0 unx     2261 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class
--rw-r--r--  2.0 unx     3078 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class
--rw-r--r--  2.0 unx     5099 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class
--rw-r--r--  2.0 unx     4804 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class
--rw-r--r--  2.0 unx     3983 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class
--rw-r--r--  2.0 unx     2712 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainParseTree.class
--rw-r--r--  2.0 unx      541 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/GrammarVisitor.class
--rw-r--r--  2.0 unx      295 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1.class
--rw-r--r--  2.0 unx     7836 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class
--rw-r--r--  2.0 unx    11022 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class
--rw-r--r--  2.0 unx     4449 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class
--rw-r--r--  2.0 unx     2795 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor.class
--rw-r--r--  2.0 unx     7338 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class
--rw-r--r--  2.0 unx     1617 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/ParseTree.class
--rw-r--r--  2.0 unx     6462 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class
--rw-r--r--  2.0 unx     3608 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class
--rw-r--r--  2.0 unx     3785 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class
--rw-r--r--  2.0 unx     6585 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor.class
--rw-r--r--  2.0 unx     5042 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class
--rw-r--r--  2.0 unx     4569 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomConjunctionVisitor.class
--rw-r--r--  2.0 unx    38187 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser.class
--rw-r--r--  2.0 unx     4008 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateLineContext.class
--rw-r--r--  2.0 unx     2330 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext.class
--rw-r--r--  2.0 unx     2276 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ImpliedByContext.class
--rw-r--r--  2.0 unx     3345 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseVectorContext.class
--rw-r--r--  2.0 unx     3091 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext.class
--rw-r--r--  2.0 unx     2237 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.class
--rw-r--r--  2.0 unx     2951 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataValContext.class
--rw-r--r--  2.0 unx     2688 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext.class
--rw-r--r--  2.0 unx     2606 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FixedValueContext.class
--rw-r--r--  2.0 unx     3548 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext.class
--rw-r--r--  2.0 unx     3435 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseMatrixContext.class
--rw-r--r--  2.0 unx     3488 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$QueriesFileContext.class
--rw-r--r--  2.0 unx     2331 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConstantContext.class
--rw-r--r--  2.0 unx     2267 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NegationContext.class
--rw-r--r--  2.0 unx     2295 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext.class
--rw-r--r--  2.0 unx     3154 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermListContext.class
--rw-r--r--  2.0 unx     2648 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext.class
--rw-r--r--  2.0 unx     2987 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.class
--rw-r--r--  2.0 unx     3225 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext.class
--rw-r--r--  2.0 unx    11229 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicVisitor.class
--rw-r--r--  2.0 unx     2655 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ElementContext.class
--rw-r--r--  2.0 unx     2913 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext.class
--rw-r--r--  2.0 unx     3511 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ExamplesFileContext.class
--rw-r--r--  2.0 unx     2660 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateFileContext.class
--rw-r--r--  2.0 unx     3600 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ValueContext.class
--rw-r--r--  2.0 unx     2187 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VariableContext.class
--rw-r--r--  2.0 unx     2846 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MatrixContext.class
--rw-r--r--  2.0 unx     2488 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext.class
--rw-r--r--  2.0 unx     2319 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$OffsetContext.class
--rw-r--r--  2.0 unx     3152 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VectorContext.class
--rw-r--r--  2.0 unx     3178 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$DimensionsContext.class
--rw-r--r--  2.0 unx    17205 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor.class
--rw-r--r--  2.0 unx     2564 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext.class
--rw-r--r--  2.0 unx     8320 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicListener.class
--rw-r--r--  2.0 unx     3066 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext.class
--rw-r--r--  2.0 unx     8056 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicLexer.class
--rw-r--r--  2.0 unx     3001 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$Element2dContext.class
--rw-r--r--  2.0 unx     2671 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext.class
--rw-r--r--  2.0 unx    15880 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseListener.class
--rw-r--r--  2.0 unx     2423 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext.class
--rw-r--r--  2.0 unx      862 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/SQLdumpExampleParser.class
--rw-r--r--  2.0 unx      259 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextTemplateParser.class
--rw-r--r--  2.0 unx     1285 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/Parser.class
--rw-r--r--  2.0 unx      164 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/TemplateParser.class
--rw-r--r--  2.0 unx      868 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextExampleParser.class
--rw-r--r--  2.0 unx      376 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/ExampleParser.class
--rw-r--r--  2.0 unx      466 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/JsonTemplateParser.class
--rw-r--r--  2.0 unx     1188 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/DefaultQueryExampleParser.class
--rw-r--r--  2.0 unx     3314 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextQueryParser.class
--rw-r--r--  2.0 unx      435 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/QueryParser.class
--rw-r--r--  2.0 unx     8550 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$PredicatesMetadataVisitor.class
--rw-r--r--  2.0 unx     5530 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$ConjunctionsVisitor.class
--rw-r--r--  2.0 unx     7466 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$WeightsMetadataVisitor.class
--rw-r--r--  2.0 unx     1504 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTree.class
--rw-r--r--  2.0 unx     5043 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     5586 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$RuleLinesVisitor.class
--rw-r--r--  2.0 unx     5450 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$FactsVisitor.class
--rw-r--r--  2.0 unx     2773 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/TemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     1325 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/XmlPlainParseTree.class
--rw-r--r--  2.0 unx     3069 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/XmlTemplateParseTreeExtractor.class
--rw-r--r--  2.0 unx     6080 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$TemplateMetadataVisitor.class
--rw-r--r--  2.0 unx     9008 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/QueriesBuilder.class
--rw-r--r--  2.0 unx    10432 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/ExamplesBuilder.class
--rw-r--r--  2.0 unx     8733 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/TemplateBuilder.class
--rw-r--r--  2.0 unx    13362 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/SamplesBuilder.class
--rw-r--r--  2.0 unx     2590 b- defN 23-Apr-07 02:01 cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class
-drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:20 META-INF/maven/io.github.gustiks/Parsing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Nov-14 21:24 META-INF/maven/io.github.gustiks/Parsing/
+-rw-r--r--  2.0 unx     1504 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTree.class
+-rw-r--r--  2.0 unx     1985 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/examples/ExamplesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     8135 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1494 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTree.class
+-rw-r--r--  2.0 unx     7281 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/queries/PlainQueriesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1740 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/queries/QueriesParseTreeExtractor.class
+-rw-r--r--  2.0 unx     2261 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class
+-rw-r--r--  2.0 unx     2675 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class
+-rw-r--r--  2.0 unx     4766 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class
+-rw-r--r--  2.0 unx     4495 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class
+-rw-r--r--  2.0 unx     3580 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class
+-rw-r--r--  2.0 unx     2712 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainParseTree.class
+-rw-r--r--  2.0 unx      541 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/GrammarVisitor.class
+-rw-r--r--  2.0 unx      295 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$1.class
+-rw-r--r--  2.0 unx     7358 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class
+-rw-r--r--  2.0 unx    10659 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class
+-rw-r--r--  2.0 unx     4046 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class
+-rw-r--r--  2.0 unx     2795 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor.class
+-rw-r--r--  2.0 unx     6940 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class
+-rw-r--r--  2.0 unx     1617 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/ParseTree.class
+-rw-r--r--  2.0 unx     6083 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class
+-rw-r--r--  2.0 unx     3275 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class
+-rw-r--r--  2.0 unx     3430 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class
+-rw-r--r--  2.0 unx     6202 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor.class
+-rw-r--r--  2.0 unx     4709 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class
+-rw-r--r--  2.0 unx     4166 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomConjunctionVisitor.class
+-rw-r--r--  2.0 unx    38187 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser.class
+-rw-r--r--  2.0 unx     4008 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateLineContext.class
+-rw-r--r--  2.0 unx     2330 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext.class
+-rw-r--r--  2.0 unx     2276 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ImpliedByContext.class
+-rw-r--r--  2.0 unx     3345 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseVectorContext.class
+-rw-r--r--  2.0 unx     3091 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LiftedExampleContext.class
+-rw-r--r--  2.0 unx     2237 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NumberContext.class
+-rw-r--r--  2.0 unx     2951 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataValContext.class
+-rw-r--r--  2.0 unx     2688 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateMetadataContext.class
+-rw-r--r--  2.0 unx     2606 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FixedValueContext.class
+-rw-r--r--  2.0 unx     3548 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LrnnRuleContext.class
+-rw-r--r--  2.0 unx     3435 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$SparseMatrixContext.class
+-rw-r--r--  2.0 unx     3488 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$QueriesFileContext.class
+-rw-r--r--  2.0 unx     2331 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConstantContext.class
+-rw-r--r--  2.0 unx     2267 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$NegationContext.class
+-rw-r--r--  2.0 unx     2295 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$FactContext.class
+-rw-r--r--  2.0 unx     3154 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermListContext.class
+-rw-r--r--  2.0 unx     2648 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateOffsetContext.class
+-rw-r--r--  2.0 unx     2987 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.class
+-rw-r--r--  2.0 unx     3225 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MetadataListContext.class
+-rw-r--r--  2.0 unx    11229 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicVisitor.class
+-rw-r--r--  2.0 unx     2655 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ElementContext.class
+-rw-r--r--  2.0 unx     2913 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightContext.class
+-rw-r--r--  2.0 unx     3511 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ExamplesFileContext.class
+-rw-r--r--  2.0 unx     2660 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateFileContext.class
+-rw-r--r--  2.0 unx     3600 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ValueContext.class
+-rw-r--r--  2.0 unx     2187 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VariableContext.class
+-rw-r--r--  2.0 unx     2846 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$MatrixContext.class
+-rw-r--r--  2.0 unx     2488 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$PredicateContext.class
+-rw-r--r--  2.0 unx     2319 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$OffsetContext.class
+-rw-r--r--  2.0 unx     3152 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$VectorContext.class
+-rw-r--r--  2.0 unx     3178 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$DimensionsContext.class
+-rw-r--r--  2.0 unx    17205 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor.class
+-rw-r--r--  2.0 unx     2564 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TermContext.class
+-rw-r--r--  2.0 unx     8320 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicListener.class
+-rw-r--r--  2.0 unx     3066 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$AtomContext.class
+-rw-r--r--  2.0 unx     8056 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicLexer.class
+-rw-r--r--  2.0 unx     3001 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$Element2dContext.class
+-rw-r--r--  2.0 unx     2671 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$WeightMetadataContext.class
+-rw-r--r--  2.0 unx    15880 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseListener.class
+-rw-r--r--  2.0 unx     2423 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$TemplateMetadataContext.class
+-rw-r--r--  2.0 unx      862 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/SQLdumpExampleParser.class
+-rw-r--r--  2.0 unx      259 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextTemplateParser.class
+-rw-r--r--  2.0 unx     1285 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/Parser.class
+-rw-r--r--  2.0 unx      164 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/TemplateParser.class
+-rw-r--r--  2.0 unx      868 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextExampleParser.class
+-rw-r--r--  2.0 unx      376 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/ExampleParser.class
+-rw-r--r--  2.0 unx      466 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/JsonTemplateParser.class
+-rw-r--r--  2.0 unx     1188 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/DefaultQueryExampleParser.class
+-rw-r--r--  2.0 unx     3314 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/PlainTextQueryParser.class
+-rw-r--r--  2.0 unx      435 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/QueryParser.class
+-rw-r--r--  2.0 unx     8159 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$PredicatesMetadataVisitor.class
+-rw-r--r--  2.0 unx     5143 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$ConjunctionsVisitor.class
+-rw-r--r--  2.0 unx     7079 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$WeightsMetadataVisitor.class
+-rw-r--r--  2.0 unx     1504 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTree.class
+-rw-r--r--  2.0 unx     4418 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     5199 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$RuleLinesVisitor.class
+-rw-r--r--  2.0 unx     5063 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$FactsVisitor.class
+-rw-r--r--  2.0 unx     2773 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/TemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     1325 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/XmlPlainParseTree.class
+-rw-r--r--  2.0 unx     3069 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/XmlTemplateParseTreeExtractor.class
+-rw-r--r--  2.0 unx     5693 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$TemplateMetadataVisitor.class
+-rw-r--r--  2.0 unx     9008 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/constructs/building/QueriesBuilder.class
+-rw-r--r--  2.0 unx    10432 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/constructs/building/ExamplesBuilder.class
+-rw-r--r--  2.0 unx     8733 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/constructs/building/TemplateBuilder.class
+-rw-r--r--  2.0 unx    13362 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/constructs/building/SamplesBuilder.class
+-rw-r--r--  2.0 unx     2590 b- defN 23-Nov-14 21:24 cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class
 -rw-r--r--  2.0 unx     1212 b- defN 22-Jul-06 18:59 META-INF/maven/io.github.gustiks/Parsing/pom.xml
 -rw-r--r--  2.0 unx      110 b- defN 22-Oct-01 18:09 META-INF/maven/io.github.gustiks/Parsing/pom.properties
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/misc/
 drwxr-xr-x  2.0 unx        0 b- stor 20-Jan-18 13:39 org/antlr/v4/runtime/tree/
@@ -1476,8 +1472,14 @@
 -rw-r--r--  2.0 unx     1175 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/AtomTransition.class
 -rw-r--r--  2.0 unx      510 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/RuleStartState.class
 -rw-r--r--  2.0 unx     1799 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/LexerTypeAction.class
 -rw-r--r--  2.0 unx      425 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/TokensStartState.class
 -rw-r--r--  2.0 unx     1026 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/ATNSerializer$2.class
 -rw-r--r--  2.0 unx      506 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/atn/PlusBlockStartState.class
 -rw-r--r--  2.0 unx     4467 b- defN 20-Jan-18 13:39 org/antlr/v4/runtime/ANTLRInputStream.class
-1481 files, 4438106 bytes uncompressed, 1724725 bytes compressed:  61.1%
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/
+-rw-r--r--  2.0 unx     1733 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/Main.class
+-rw-r--r--  2.0 unx     6196 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
+-rw-r--r--  2.0 unx    17210 b- defN 23-Apr-07 21:43 cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
+1483 files, 4432606 bytes uncompressed, 1721283 bytes compressed:  61.2%
```

#### zipnote «TEMP»/diffoscope_36808_fg_/tmpgp1u7o9d_.zip

```diff
@@ -15,32 +15,14 @@
 
 Filename: cz/cvut/fel/
 Comment: 
 
 Filename: cz/cvut/fel/ida/
 Comment: 
 
-Filename: cz/cvut/fel/ida/neuralogic/
-Comment: 
-
-Filename: cz/cvut/fel/ida/neuralogic/cli/
-Comment: 
-
-Filename: cz/cvut/fel/ida/neuralogic/cli/utils/
-Comment: 
-
-Filename: cz/cvut/fel/ida/neuralogic/cli/Main.class
-Comment: 
-
-Filename: cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
-Comment: 
-
-Filename: cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
-Comment: 
-
 Filename: cz/cvut/fel/ida/setup/
 Comment: 
 
 Filename: cz/cvut/fel/ida/setup/Settings$ResultsType.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/setup/Settings$1.class
@@ -1230,14 +1212,17 @@
 
 Filename: cz/cvut/fel/ida/pipelines/debuging/
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/debuging/drawing/
 Comment: 
 
+Filename: META-INF/maven/io.github.gustiks/Pipelines/
+Comment: 
+
 Filename: cz/cvut/fel/ida/pipelines/MultiMerge.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/Pipe.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/ParallelPipe.class
@@ -1356,17 +1341,14 @@
 
 Filename: cz/cvut/fel/ida/pipelines/ConnectAfter.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/Merge$2.class
 Comment: 
 
-Filename: META-INF/maven/io.github.gustiks/Pipelines/
-Comment: 
-
 Filename: META-INF/maven/io.github.gustiks/Pipelines/pom.xml
 Comment: 
 
 Filename: META-INF/maven/io.github.gustiks/Pipelines/pom.properties
 Comment: 
 
 Filename: cz/cvut/fel/ida/drawing/
@@ -1437,14 +1419,17 @@
 
 Filename: cz/cvut/fel/ida/pipelines/pipes/specific/
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/utils/
 Comment: 
 
+Filename: META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
+Comment: 
+
 Filename: cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$2.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$3.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/TrainingBuilder$LogicLearningBuilder$1.class
@@ -1482,14 +1467,17 @@
 
 Filename: cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$1.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$10.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/pipelines/building/PythonBuilder$PythonNeuralizationPipeline.class
+Comment: 
+
 Filename: cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$1.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/CrossvalidationBuilder$4.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/NeuralNetsBuilder$1.class
@@ -1596,14 +1584,17 @@
 
 Filename: cz/cvut/fel/ida/pipelines/building/LearningSchemeBuilder$1.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/building/TemplateProcessingBuilder$5.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/pipelines/building/PythonBuilder$PythonGroundingPipeline.class
+Comment: 
+
 Filename: cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$3$1.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/debugging/GroundingDebugger.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/debugging/End2EndDebugger$1.class
@@ -1695,17 +1686,14 @@
 
 Filename: cz/cvut/fel/ida/pipelines/pipes/specific/SupervisedTemplateReducingPipe.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/pipelines/utils/WorkflowUtils.class
 Comment: 
 
-Filename: META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/
-Comment: 
-
 Filename: META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.xml
 Comment: 
 
 Filename: META-INF/maven/io.github.gustiks/NeuraLogic-Workflow/pom.properties
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/
@@ -1932,14 +1920,17 @@
 
 Filename: cz/cvut/fel/ida/algebra/functions/aggregation/
 Comment: 
 
 Filename: cz/cvut/fel/ida/algebra/functions/combination/
 Comment: 
 
+Filename: META-INF/maven/io.github.gustiks/Algebra/
+Comment: 
+
 Filename: cz/cvut/fel/ida/algebra/weights/ScalarWeight.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/algebra/weights/Weight.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/algebra/weights/StatefulWeight.class
@@ -2271,17 +2262,14 @@
 
 Filename: cz/cvut/fel/ida/algebra/functions/ElementWise.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/algebra/functions/Combination$1.class
 Comment: 
 
-Filename: META-INF/maven/io.github.gustiks/Algebra/
-Comment: 
-
 Filename: META-INF/maven/io.github.gustiks/Algebra/pom.xml
 Comment: 
 
 Filename: META-INF/maven/io.github.gustiks/Algebra/pom.properties
 Comment: 
 
 Filename: org/jetbrains/
@@ -3450,14 +3438,17 @@
 
 Filename: cz/cvut/fel/ida/logic/parsing/alternatives/parsing_old/
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/parsing/template/
 Comment: 
 
+Filename: META-INF/maven/io.github.gustiks/Parsing/
+Comment: 
+
 Filename: cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTree.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/parsing/examples/ExamplesParseTreeExtractor.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class
@@ -3729,17 +3720,14 @@
 
 Filename: cz/cvut/fel/ida/logic/constructs/building/SamplesBuilder.class
 Comment: 
 
 Filename: cz/cvut/fel/ida/logic/constructs/building/LogicSourceBuilder.class
 Comment: 
 
-Filename: META-INF/maven/io.github.gustiks/Parsing/
-Comment: 
-
 Filename: META-INF/maven/io.github.gustiks/Parsing/pom.xml
 Comment: 
 
 Filename: META-INF/maven/io.github.gustiks/Parsing/pom.properties
 Comment: 
 
 Filename: org/antlr/
@@ -4437,8 +4425,26 @@
 
 Filename: org/antlr/v4/runtime/atn/PlusBlockStartState.class
 Comment: 
 
 Filename: org/antlr/v4/runtime/ANTLRInputStream.class
 Comment: 
 
+Filename: cz/cvut/fel/ida/neuralogic/
+Comment: 
+
+Filename: cz/cvut/fel/ida/neuralogic/cli/
+Comment: 
+
+Filename: cz/cvut/fel/ida/neuralogic/cli/utils/
+Comment: 
+
+Filename: cz/cvut/fel/ida/neuralogic/cli/Main.class
+Comment: 
+
+Filename: cz/cvut/fel/ida/neuralogic/cli/utils/Runner.class
+Comment: 
+
+Filename: cz/cvut/fel/ida/neuralogic/cli/utils/CommandLineHandler.class
+Comment: 
+
 Zip file comment:
```

#### cz/cvut/fel/ida/pipelines/building/PythonBuilder.class

##### procyon -ec {}

```diff
@@ -1,127 +1,68 @@
 
 package cz.cvut.fel.ida.pipelines.building;
 
-import cz.cvut.fel.ida.pipelines.pipes.specific.NeuralSerializerPipe;
-import cz.cvut.fel.ida.neural.networks.structure.export.NeuralSerializer;
-import java.util.List;
-import java.util.concurrent.atomic.AtomicInteger;
-import cz.cvut.fel.ida.pipelines.Merge;
-import cz.cvut.fel.ida.pipelines.pipes.generic.PairMerge;
-import cz.cvut.fel.ida.pipelines.ConnectAfter;
-import cz.cvut.fel.ida.pipelines.ConnectBefore;
-import cz.cvut.fel.ida.pipelines.pipes.generic.LambdaPipe;
-import cz.cvut.fel.ida.pipelines.Branch;
-import cz.cvut.fel.ida.pipelines.pipes.generic.FirstFromPairExtractionBranch;
 import java.util.function.IntConsumer;
+import cz.cvut.fel.ida.neural.networks.computation.training.NeuralSample;
 import cz.cvut.fel.ida.logic.grounding.GroundingSample;
 import cz.cvut.fel.ida.logic.constructs.example.LogicSample;
+import java.util.stream.Stream;
+import cz.cvut.fel.ida.utils.generic.Pair;
 import cz.cvut.fel.ida.pipelines.Pipeline;
+import cz.cvut.fel.ida.setup.Sources;
 import cz.cvut.fel.ida.pipelines.pipes.specific.TemplateToNeuralPipe;
+import cz.cvut.fel.ida.neural.networks.computation.training.NeuralModel;
+import cz.cvut.fel.ida.logic.constructs.template.Template;
 import cz.cvut.fel.ida.pipelines.Pipe;
 import cz.cvut.fel.ida.setup.Settings;
-import cz.cvut.fel.ida.logic.constructs.template.Template;
-import cz.cvut.fel.ida.pipelines.pipes.generic.DuplicateBranch;
 import cz.cvut.fel.ida.logic.constructs.building.factories.WeightFactory;
-import cz.cvut.fel.ida.neural.networks.computation.training.NeuralSample;
-import java.util.stream.Stream;
-import cz.cvut.fel.ida.neural.networks.computation.training.NeuralModel;
-import cz.cvut.fel.ida.utils.generic.Pair;
-import cz.cvut.fel.ida.setup.Sources;
-import cz.cvut.fel.ida.pipelines.bulding.AbstractPipelineBuilder;
 
-public class PythonBuilder extends AbstractPipelineBuilder<Sources, Pair<NeuralModel, Stream<NeuralSample>>>
+public class PythonBuilder
 {
     private final WeightFactory weightFactory;
-    private DuplicateBranch<Template> templateDuplicateBranch;
+    private final Settings settings;
+    private final PythonBuilder.PythonGroundingPipeline groundingPipeline;
+    private final PythonBuilder.PythonNeuralizationPipeline neuralizationPipeline;
     
     public PythonBuilder(final Settings settings) {
-        super(settings);
+        this.settings = settings;
         this.weightFactory = new WeightFactory(settings.inferred.maxWeightCount);
+        this.groundingPipeline = new PythonBuilder.PythonGroundingPipeline(this, settings);
+        this.neuralizationPipeline = new PythonBuilder.PythonNeuralizationPipeline(this, settings);
     }
     
     public Pipe<Template, NeuralModel> convertModel() {
         return (Pipe<Template, NeuralModel>)new TemplateToNeuralPipe(this.settings);
     }
     
     public Pipeline<Sources, Pair<Template, Stream<LogicSample>>> buildFromSources(final Template template, final Sources sources, final Settings settings) {
         final TemplateSamplesBuilder templateSamplesBuilder = new TemplateSamplesBuilder(sources, settings, template);
         return (Pipeline<Sources, Pair<Template, Stream<LogicSample>>>)templateSamplesBuilder.buildPipeline();
     }
     
     public Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>> buildGrounding(final Settings settings, final WeightFactory weightFactory) {
         final GroundingBuilder groundingBuilder = new GroundingBuilder(settings, weightFactory);
-        final Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>> groundingPipeline = (Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>>)groundingBuilder.buildPipeline();
-        return groundingPipeline;
+        return (Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>>)groundingBuilder.buildPipeline();
     }
     
     public Pipeline<Stream<GroundingSample>, Stream<NeuralSample>> buildNeuralNets(final Settings settings, final WeightFactory weightFactory) {
         final NeuralNetsBuilder neuralNetsBuilder = new NeuralNetsBuilder(settings, weightFactory);
         return (Pipeline<Stream<GroundingSample>, Stream<NeuralSample>>)neuralNetsBuilder.buildPipeline();
     }
     
     public Template buildTemplate(final Sources sources) throws Exception {
         final TemplateSamplesBuilder templateSamplesBuilder = new TemplateSamplesBuilder(sources, this.settings);
         return (Template)templateSamplesBuilder.getSourcesTemplatePipeline(sources, this.settings).execute((Object)sources).s;
     }
     
-    public Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> buildPipeline(final Template template, final Stream<LogicSample> logicSamples, final IntConsumer progressCallback) {
-        final Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> pipeline = (Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>>)new Pipeline("PythonNNbuilding", (AbstractPipelineBuilder)this);
-        final FirstFromPairExtractionBranch<Template, Stream<LogicSample>> templateSamplesBranch = (FirstFromPairExtractionBranch<Template, Stream<LogicSample>>)pipeline.register((Branch)new FirstFromPairExtractionBranch());
-        this.templateDuplicateBranch = (DuplicateBranch<Template>)pipeline.register((Branch)new DuplicateBranch());
-        final LambdaPipe<Sources, Pair<Template, Stream<LogicSample>>> templateIdentityPipe = (LambdaPipe<Sources, Pair<Template, Stream<LogicSample>>>)pipeline.registerStart((Pipe)new LambdaPipe("TemplateIdentityPipe", s -> new Pair((Object)template, (Object)logicSamples), this.settings));
-        final Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>> groundingPipeline = (Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>>)pipeline.register((Pipeline)this.buildGrounding(this.settings, this.weightFactory));
-        final Pipeline<Stream<GroundingSample>, Stream<NeuralSample>> neuralizationPipeline = (Pipeline<Stream<GroundingSample>, Stream<NeuralSample>>)pipeline.register((Pipeline)this.buildNeuralNets(this.settings, this.weightFactory));
-        templateIdentityPipe.connectAfter((ConnectBefore)templateSamplesBranch);
-        templateSamplesBranch.connectAfterL((Pipeline)groundingPipeline).connectAfter((Pipeline)neuralizationPipeline);
-        templateSamplesBranch.connectAfterR((ConnectBefore)this.templateDuplicateBranch);
-        final PairMerge<NeuralModel, Stream<NeuralSample>> neuralMerge = this.attachProgressCallback(progressCallback, pipeline);
-        final Pipe<Template, NeuralModel> template2NeuralModelPipe = (Pipe<Template, NeuralModel>)pipeline.register((Pipe)this.convertModel());
-        this.templateDuplicateBranch.connectAfterL((ConnectBefore)template2NeuralModelPipe);
-        neuralMerge.connectBeforeL((ConnectAfter)template2NeuralModelPipe);
-        neuralMerge.connectBeforeR((ConnectAfter)neuralizationPipeline);
-        return pipeline;
-    }
-    
-    public Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> buildPipeline(final Template template, final Sources sources, final IntConsumer progressCallback) {
-        final Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> pipeline = (Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>>)new Pipeline("PythonNNbuilding", (AbstractPipelineBuilder)this);
-        final FirstFromPairExtractionBranch<Template, Stream<LogicSample>> templateSamplesBranch = (FirstFromPairExtractionBranch<Template, Stream<LogicSample>>)pipeline.register((Branch)new FirstFromPairExtractionBranch());
-        this.templateDuplicateBranch = (DuplicateBranch<Template>)pipeline.register((Branch)new DuplicateBranch());
-        final Pipeline<Sources, Pair<Template, Stream<LogicSample>>> sourcesPairPipeline = (Pipeline<Sources, Pair<Template, Stream<LogicSample>>>)pipeline.registerStart((Pipeline)this.buildFromSources(template, sources, this.settings));
-        final Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>> groundingPipeline = (Pipeline<Pair<Template, Stream<LogicSample>>, Stream<GroundingSample>>)pipeline.register((Pipeline)this.buildGrounding(this.settings, this.weightFactory));
-        final Pipeline<Stream<GroundingSample>, Stream<NeuralSample>> neuralizationPipeline = (Pipeline<Stream<GroundingSample>, Stream<NeuralSample>>)pipeline.register((Pipeline)this.buildNeuralNets(this.settings, this.weightFactory));
-        sourcesPairPipeline.connectAfter((ConnectBefore)templateSamplesBranch);
-        templateSamplesBranch.connectAfterL((Pipeline)groundingPipeline).connectAfter((Pipeline)neuralizationPipeline);
-        templateSamplesBranch.connectAfterR((ConnectBefore)this.templateDuplicateBranch);
-        final PairMerge<NeuralModel, Stream<NeuralSample>> neuralMerge = this.attachProgressCallback(progressCallback, pipeline);
-        final Pipe<Template, NeuralModel> template2NeuralModelPipe = (Pipe<Template, NeuralModel>)pipeline.register((Pipe)this.convertModel());
-        this.templateDuplicateBranch.connectAfterL((ConnectBefore)template2NeuralModelPipe);
-        neuralMerge.connectBeforeL((ConnectAfter)template2NeuralModelPipe);
-        neuralMerge.connectBeforeR((ConnectAfter)neuralizationPipeline);
-        return pipeline;
-    }
-    
-    private PairMerge<NeuralModel, Stream<NeuralSample>> attachProgressCallback(final IntConsumer callback, final Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> pipeline) {
-        if (callback == null) {
-            return (PairMerge<NeuralModel, Stream<NeuralSample>>)pipeline.registerEnd((Merge)new PairMerge());
-        }
-        final AtomicInteger counter = new AtomicInteger();
-        final PairMerge<NeuralModel, Stream<NeuralSample>> neuralMerge = (PairMerge<NeuralModel, Stream<NeuralSample>>)pipeline.register((Merge)new PairMerge());
-        final LambdaPipe<Pair<NeuralModel, Stream<NeuralSample>>, Pair<NeuralModel, Stream<NeuralSample>>> progressCallbackPipe = (LambdaPipe<Pair<NeuralModel, Stream<NeuralSample>>, Pair<NeuralModel, Stream<NeuralSample>>>)pipeline.registerEnd((Pipe)new LambdaPipe("ProgressCallbackPipe", pair -> {
-            final Stream<NeuralSample> stream = ((Stream)pair.s).peek(sample -> callback.accept(counter.incrementAndGet()));
-            return new Pair((Object)pair.r, (Object)stream);
-        }, this.settings));
-        neuralMerge.connectAfter((Pipe)progressCallbackPipe);
-        return neuralMerge;
-    }
-    
-    public Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> buildPipeline() {
-        return null;
-    }
-    
-    public Pair<List<NeuralSerializer.SerializedWeight>, Stream<NeuralSerializer.SerializedSample>> getSerializedNNs() throws Exception {
-        final Pipeline<Sources, Pair<NeuralModel, Stream<NeuralSample>>> buildNNsPipeline = this.buildPipeline();
-        final NeuralSerializerPipe neuralSerializerPipe = new NeuralSerializerPipe();
-        final Pipe<Pair<NeuralModel, Stream<NeuralSample>>, Pair<List<NeuralSerializer.SerializedWeight>, Stream<NeuralSerializer.SerializedSample>>> serializationPipe = (Pipe<Pair<NeuralModel, Stream<NeuralSample>>, Pair<List<NeuralSerializer.SerializedWeight>, Stream<NeuralSerializer.SerializedSample>>>)buildNNsPipeline.connectAfter((Pipe)neuralSerializerPipe);
-        return (Pair<List<NeuralSerializer.SerializedWeight>, Stream<NeuralSerializer.SerializedSample>>)serializationPipe.get();
+    public Pipeline<Sources, Stream<GroundingSample>> buildGroundings(final Template template, final Stream<LogicSample> logicSamples) {
+        return (Pipeline<Sources, Stream<GroundingSample>>)this.groundingPipeline.buildPipeline(template, (Stream)logicSamples);
+    }
+    
+    public Pipeline<Sources, Stream<GroundingSample>> buildGroundings(final Template template, final Sources sources) {
+        return (Pipeline<Sources, Stream<GroundingSample>>)this.groundingPipeline.buildPipeline(template, sources);
+    }
+    
+    public Pipeline<Stream<GroundingSample>, Stream<NeuralSample>> neuralize(final Stream<GroundingSample> groundings, final IntConsumer progressCallback) {
+        return (Pipeline<Stream<GroundingSample>, Stream<NeuralSample>>)this.neuralizationPipeline.buildPipeline((Stream)groundings, progressCallback);
     }
 }
```

#### cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer$NeuronDrawer.class

##### procyon -ec {}

```diff
@@ -76,17 +76,15 @@
         return sb.toString();
     }
     
     private String getEdgeLabel(final int from, final Integer to, final Weight weight) {
         final StringBuilder sb = new StringBuilder();
         sb.append(" [label=");
         sb.append("\"");
-        sb.append(weight.index).append(":");
         sb.append(weight.name).append(":");
-        sb.append(Arrays.toString(weight.value.size())).append(":");
         sb.append(weight.value.toString(this.this$0.numberFormat));
         sb.append("\"");
         if (weight.isFixed) {
             sb.append(", style=dashed ");
         }
         sb.append("]");
         return sb.toString();
```

#### cz/cvut/fel/ida/pipelines/debugging/drawing/GroundingDrawer.class

##### procyon -ec {}

```diff
@@ -24,19 +24,19 @@
     
     public GroundingDrawer(final Settings settings) {
         super(settings);
         this.compact = true;
         this.compact = settings.compactGroundingDrawing;
     }
     
-    public void loadGraph(final GroundingSample obj) {
+    public void loadGraph(final GroundingSample sample) {
         this.graphviz.start_graph();
-        this.nodeGraph(obj);
-        if (((QueryAtom)obj.query).headAtom != null) {
-            this.graphviz.addln(GraphViz.sanitize(((QueryAtom)obj.query).headAtom.literal.toString()) + "[shape = tripleoctagon]");
+        this.nodeGraph(sample);
+        if (((QueryAtom)sample.query).headAtom != null) {
+            this.graphviz.addln(GraphViz.sanitize(((QueryAtom)sample.query).headAtom.literal.toString()) + "[shape = tripleoctagon, xlabel=\"\n\n\ntarget = " + sample.target + "  \"]");
         }
         this.graphviz.end_graph();
     }
     
     public void nodeGraph(final GroundingSample obj) {
         final GroundTemplate groundTemplate = obj.groundingWrap.getGroundTemplate();
         final LinkedHashMap<Literal, LinkedHashMap<GroundHeadRule, Collection<GroundRule>>> groundRules = groundTemplate.groundRules;
```

#### cz/cvut/fel/ida/pipelines/debugging/drawing/NeuralNetDrawer.class

##### procyon -ec {}

```diff
@@ -28,15 +28,15 @@
     
     public void loadGraph(final NeuralSample sample) {
         this.neuronDrawer = new NeuralNetDrawer.NeuronDrawer(this, (NeuralNetwork)((QueryNeuron)sample.query).evidence, this.stateIndex, this.graphviz);
         this.bUpIterator = new Topologic.BUpIterator(new Topologic((TopologicNetwork)((QueryNeuron)sample.query).evidence), (Neurons)((QueryNeuron)sample.query).neuron, (NeuronVisitor.Weighted)this.neuronDrawer);
         this.graphviz.start_graph();
         this.iterateNetwork();
         if (((QueryNeuron)sample.query).neuron != null) {
-            this.graphviz.addln(((QueryNeuron)sample.query).neuron.getIndex() + " [shape = tripleoctagon]");
+            this.graphviz.addln(((QueryNeuron)sample.query).neuron.getIndex() + "[shape = tripleoctagon, xlabel=\"\n\n\ntarget = " + sample.target + "  \"]");
         }
         this.graphviz.end_graph();
     }
     
     private void iterateNetwork() {
         while (this.bUpIterator.hasNext()) {
             final BaseNeuron<Neurons, State.Neural> nextNeuron = (BaseNeuron<Neurons, State.Neural>)this.bUpIterator.next();
```

#### cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp.class

##### procyon -ec {}

```diff
@@ -117,15 +117,19 @@
             }
         }
         BottomUp.LOG.fine(groundRules.size() + " ground rules created.");
         this.totalGroundRules += groundRules.size();
         final GroundTemplate groundTemplate = new GroundTemplate((LinkedHashMap)groundRules, (Map)groundFacts);
         this.herbrandModel.clear();
         this.timing.toc();
-        return groundTemplate;
+        final GroundTemplate groundTemplate2 = groundTemplate;
+        if (groundTemplate2 == null) {
+            $$$reportNull$$$0(0);
+        }
+        return groundTemplate2;
     }
     
     public GroundTemplate groundRulesAndFacts(final LiftedExample example, final Template template, GroundTemplate memory) {
         if (memory == null) {
             memory = new GroundTemplate();
         }
         this.herbrandModel.populateHerbrand((Collection)memory.groundFacts.keySet());
@@ -189,8 +193,12 @@
         final Collection<GroundRule> ruleGroundings = (Collection<GroundRule>)groundHeadRules2groundings.computeIfAbsent(groundHeadRule, k -> GroundRulesCollection.getGroundingCollection(grounding.weightedRule));
         ruleGroundings.add(grounding);
     }
     
     static {
         LOG = Logger.getLogger(BottomUp.class.getName());
     }
+    
+    private static /* synthetic */ void $$$reportNull$$$0(final int n) {
+        throw new IllegalStateException(String.format("@NotNull method %s.%s must not return null", "cz/cvut/fel/ida/logic/grounding/bottomUp/BottomUp", "groundRulesAndFacts"));
+    }
 }
```

#### cz/cvut/fel/ida/algebra/weights/Weight.class

##### procyon -ec {}

```diff
@@ -92,15 +92,18 @@
     public String toString() {
         return this.toString(Settings.shortNumberFormat);
     }
     
     public String toString(final NumberFormat nf) {
         final StringBuilder sb = new StringBuilder();
         if (this.manualInitialization || this.isFixed || this.isShared) {
-            sb.append("<" + this.name + "> ");
+            sb.append("<" + this.name + ">:");
+        }
+        else {
+            sb.append(this.name + ":");
         }
         sb.append(this.value.toString(nf));
         return sb.toString();
     }
     
     public boolean isLearnable() {
         if (this.isLearnable != null) {
```

#### cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor.class

##### procyon -ec {}

```diff
@@ -19,75 +19,46 @@
     private static final Logger LOG;
     
     public PlainExamplesParseTreeExtractor(final PlainGrammarVisitor v) {
         super((GrammarVisitor)v);
     }
     
     public Stream<LiftedExample> getUnlabeledExamples(@NotNull final NeuralogicParser.ExamplesFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         PlainExamplesParseTreeExtractor.LOG.info("Parsing examples...");
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.LiftedExampleVisitor liftedExampleVisitor = new PlainGrammarVisitor.LiftedExampleVisitor(obj);
         if (ctx.liftedExample() != null) {
             final Stream<LiftedExample> listStream = ctx.liftedExample().stream().map(rule -> (Object)rule.accept((ParseTreeVisitor)liftedExampleVisitor));
             return listStream;
         }
         PlainExamplesParseTreeExtractor.LOG.severe("Could not extract any Unlabeled trainExamples");
         return null;
     }
     
     public Stream<Pair<Conjunction, LiftedExample>> getLabeledExamples(@NotNull final NeuralogicParser.ExamplesFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(1);
-        }
         if (ctx.label() == null || ctx.label().isEmpty()) {
             return this.getUnlabeledExamples(ctx).map(ex -> new Pair((Object)null, (Object)ex));
         }
         return Utilities.zipStreams((Stream)this.getQueries(ctx), (Stream)this.getUnlabeledExamples(ctx), (q, e) -> this.createSamplePair(q, e));
     }
     
     private Pair<Conjunction, LiftedExample> createSamplePair(final Conjunction q, final LiftedExample e) {
         PlainExamplesParseTreeExtractor.LOG.finer("Merging query/label " + q.toString() + " with example " + e);
         return (Pair<Conjunction, LiftedExample>)new Pair((Object)q, (Object)e);
     }
     
     public Stream<Conjunction> getQueries(@NotNull final NeuralogicParser.ExamplesFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(2);
-        }
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.LabelVisitor labelVisitor = new PlainGrammarVisitor.LabelVisitor(obj);
         if (ctx.label() != null && !ctx.label().isEmpty()) {
             return ctx.label().stream().map(line -> (Object)line.accept((ParseTreeVisitor)labelVisitor));
         }
         PlainExamplesParseTreeExtractor.LOG.severe("Could not extract any trainQueries (weighted facts)");
         return null;
     }
     
     static {
         LOG = Logger.getLogger(PlainExamplesParseTreeExtractor.class.getName());
     }
-    
-    private static /* synthetic */ void $$$reportNull$$$0(final int n) {
-        final String format = "Argument for @NotNull parameter '%s' of %s.%s must not be null";
-        final Object[] args = { "ctx", "cz/cvut/fel/ida/logic/parsing/examples/PlainExamplesParseTreeExtractor", null };
-        switch (n) {
-            default: {
-                args[2] = "getUnlabeledExamples";
-                break;
-            }
-            case 1: {
-                args[2] = "getLabeledExamples";
-                break;
-            }
-            case 2: {
-                args[2] = "getQueries";
-                break;
-            }
-        }
-        throw new IllegalArgumentException(String.format(format, args));
-    }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum bac9cfafad510b6370968ae0c9493606aa79822e9ac7be2f9dc015bf450242b0
+  SHA-256 checksum c0e6b605c77eac79265b9946c05751bb986d4f490401acee9e2534acf1077187
   Compiled from "PlainGrammarVisitor.java"
 public class cz.cvut.fel.ida.logic.parsing.grammarParsing.PlainGrammarVisitor$LabelVisitor extends cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicBaseVisitor<cz.cvut.fel.ida.logic.constructs.Conjunction>
   minor version: 0
   major version: 52
   flags: (0x0021) ACC_PUBLIC, ACC_SUPER
   this_class: #9                          // cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor
   super_class: #10                        // cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor
@@ -87,15 +87,15 @@
          0: aload_0
          1: aload_1
          2: putfield      #1                  // Field this$0:Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
          5: aload_0
          6: invokespecial #2                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor."<init>":()V
          9: return
       LineNumberTable:
-        line 174: 0
+        line 173: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      10     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
             0      10     1 this$0   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor;
 
   public cz.cvut.fel.ida.logic.constructs.Conjunction visitLabel(cz.cvut.fel.ida.logic.parsing.antlr.NeuralogicParser$LabelContext);
     descriptor: (Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
@@ -113,17 +113,17 @@
         16: aload_2
         17: invokevirtual #6                  // Method cz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$ConjunctionContext.accept:(Lorg/antlr/v4/runtime/tree/ParseTreeVisitor;)Ljava/lang/Object;
         20: checkcast     #7                  // class cz/cvut/fel/ida/logic/constructs/Conjunction
         23: astore_3
         24: aload_3
         25: areturn
       LineNumberTable:
-        line 179: 0
-        line 180: 12
-        line 181: 24
+        line 178: 0
+        line 179: 12
+        line 180: 24
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
             0      26     1   ctx   Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;
            12      14     2 factConjunctionVisitor   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor;
            24       2     3 label   Lcz/cvut/fel/ida/logic/constructs/Conjunction;
 
@@ -133,15 +133,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #8                  // Method visitLabel:(Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicParser$LabelContext;)Lcz/cvut/fel/ida/logic/constructs/Conjunction;
          5: areturn
       LineNumberTable:
-        line 174: 0
+        line 173: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lcz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LabelVisitor;
 }
 Signature: #37                          // Lcz/cvut/fel/ida/logic/parsing/antlr/NeuralogicBaseVisitor<Lcz/cvut/fel/ida/logic/constructs/Conjunction;>;
 SourceFile: "PlainGrammarVisitor.java"
 InnerClasses:
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TemplateMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -10,14 +10,11 @@
 public class TemplateMetadataVisitor extends NeuralogicBaseVisitor<Map<String, Object>>
 {
     public TemplateMetadataVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Map<String, Object> visitTemplateMetadata(@NotNull final NeuralogicParser.TemplateMetadataContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final Map<String, Object> metadata = (Map)ctx.metadataList().accept((ParseTreeVisitor)new PlainGrammarVisitor.MetadataListVisitor(this.this$0, (PlainGrammarVisitor.PlainGrammarVisitor$1)null));
         return metadata;
     }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -12,17 +12,14 @@
 public class PredicateMetadataVisitor extends NeuralogicBaseVisitor<Pair<WeightedPredicate, Map<String, Object>>>
 {
     public PredicateMetadataVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Pair<WeightedPredicate, Map<String, Object>> visitPredicateMetadata(@NotNull final NeuralogicParser.PredicateMetadataContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         int arity = -1;
         try {
             arity = Integer.parseInt(ctx.predicate().INT().getText());
         }
         catch (final Exception ex) {
             PlainGrammarVisitor.access$300().severe("Cannot parse arity of a predicate from " + ctx.getText());
         }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$MetadataListVisitor.class

##### procyon -ec {}

```diff
@@ -12,17 +12,14 @@
 private class MetadataListVisitor extends NeuralogicBaseVisitor<Map<String, Object>>
 {
     private MetadataListVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Map<String, Object> visitMetadataList(@NotNull final NeuralogicParser.MetadataListContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final Map<String, Object> metadata = new LinkedHashMap<String, Object>();
         for (final NeuralogicParser.MetadataValContext paramVal : ctx.metadataVal()) {
             final String parameter = paramVal.ATOMIC_NAME(0).getText();
             String valueText = null;
             if (paramVal.ATOMIC_NAME(1) != null) {
                 valueText = paramVal.ATOMIC_NAME(1).getText();
             }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -12,15 +12,12 @@
 public class WeightMetadataVisitor extends NeuralogicBaseVisitor<Pair<Weight, Map<String, Object>>>
 {
     public WeightMetadataVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Pair<Weight, Map<String, Object>> visitWeightMetadata(@NotNull final NeuralogicParser.WeightMetadataContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final Weight weight = this.this$0.builder.weightFactory.construct(ctx.ATOMIC_NAME().getText());
         final Map<String, Object> metadata = (Map)ctx.metadataList().accept((ParseTreeVisitor)new PlainGrammarVisitor.MetadataListVisitor(this.this$0, (PlainGrammarVisitor.PlainGrammarVisitor$1)null));
         return (Pair<Weight, Map<String, Object>>)new Pair((Object)weight, (Object)metadata);
     }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactVisitor.class

##### procyon -ec {}

```diff
@@ -22,24 +22,18 @@
     
     public FactVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
         this.variableFactory = new VariableFactory();
     }
     
     public ValuedFact visitFact(@NotNull final NeuralogicParser.FactContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         return this.visitAtom(ctx.atom());
     }
     
     public ValuedFact visitAtom(@NotNull final NeuralogicParser.AtomContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(1);
-        }
         final PlainGrammarVisitor.TermVisitor termVisitor = new PlainGrammarVisitor.TermVisitor(this.this$0, (PlainGrammarVisitor.PlainGrammarVisitor$1)null);
         termVisitor.variableFactory = this.variableFactory;
         List<Term> terms;
         if (ctx.termList() != null) {
             terms = (List)ctx.termList().term().stream().map(FactVisitor::lambda$visitAtom$0).collect(Collectors.toList());
         }
         else {
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$WeightVisitor.class

##### procyon -ec {}

```diff
@@ -21,17 +21,14 @@
 private class WeightVisitor extends NeuralogicBaseVisitor<Weight>
 {
     private WeightVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Weight visitWeight(@NotNull final NeuralogicParser.WeightContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         Pair<Boolean, Value> value = null;
         boolean fixed = false;
         if (ctx.fixedValue() != null) {
             fixed = true;
             value = (Pair<Boolean, Value>)this.parseValue(ctx.fixedValue().value());
         }
         else if (ctx.value() != null) {
@@ -100,15 +97,18 @@
                     value = (Value)new ScalarValue();
                 }
                 else {
                     value = (Value)new VectorValue((int)Integer.valueOf(dims.get(0)));
                 }
             }
             else if (dims.size() == 2) {
-                if (Integer.valueOf(dims.get(0)) == 1) {
+                if (Integer.valueOf(dims.get(0)) == 1 && Integer.valueOf(dims.get(1)) == 1) {
+                    value = (Value)new ScalarValue();
+                }
+                else if (Integer.valueOf(dims.get(0)) == 1) {
                     value = (Value)new VectorValue((int)Integer.valueOf(dims.get(1)));
                     ((VectorValue)value).rowOrientation = true;
                 }
                 else if (Integer.valueOf(dims.get(1)) == 1) {
                     value = (Value)new VectorValue((int)Integer.valueOf(dims.get(0)));
                     ((VectorValue)value).rowOrientation = false;
                 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$FactConjunctionVisitor.class

##### procyon -ec {}

```diff
@@ -18,16 +18,13 @@
     public VariableFactory variableFactory;
     
     public FactConjunctionVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Conjunction visitConjunction(@NotNull final NeuralogicParser.ConjunctionContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final PlainGrammarVisitor.FactVisitor factVisitor = new PlainGrammarVisitor.FactVisitor(this.this$0);
         factVisitor.variableFactory = this.variableFactory;
         final List<ValuedFact> conjunction = (List)ctx.atom().stream().map(FactConjunctionVisitor::lambda$visitConjunction$0).collect(Collectors.toList());
         return new Conjunction((List)conjunction);
     }
 }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomVisitor.class

##### procyon -ec {}

```diff
@@ -22,17 +22,14 @@
     VariableFactory variableFactory;
     
     public AtomVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public BodyAtom visitAtom(@NotNull final NeuralogicParser.AtomContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final PlainGrammarVisitor.TermVisitor termVisitor = new PlainGrammarVisitor.TermVisitor(this.this$0, (PlainGrammarVisitor.PlainGrammarVisitor$1)null);
         termVisitor.variableFactory = this.variableFactory;
         List<Term> terms;
         if (ctx.termList() != null) {
             terms = (List)ctx.termList().term().stream().map(AtomVisitor::lambda$visitAtom$0).collect(Collectors.toList());
         }
         else {
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$LiftedExampleVisitor.class

##### procyon -ec {}

```diff
@@ -20,17 +20,14 @@
     
     public LiftedExampleVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
         this.variableFactory = new VariableFactory();
     }
     
     public LiftedExample visitLiftedExample(@NotNull final NeuralogicParser.LiftedExampleContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final PlainGrammarVisitor.FactConjunctionVisitor factConjunctionVisitor = new PlainGrammarVisitor.FactConjunctionVisitor(this.this$0);
         factConjunctionVisitor.variableFactory = this.variableFactory;
         final PlainGrammarVisitor.RuleLineVisitor ruleLineVisitor = new PlainGrammarVisitor.RuleLineVisitor(this.this$0);
         ruleLineVisitor.variableFactory = this.variableFactory;
         final List<Conjunction> conjunctions = (List)ctx.conjunction().stream().map(LiftedExampleVisitor::lambda$visitLiftedExample$0).collect(Collectors.toList());
         final List<WeightedRule> rules = (List)ctx.lrnnRule().stream().map(LiftedExampleVisitor::lambda$visitLiftedExample$1).collect(Collectors.toList());
         final LiftedExample liftedExample = new LiftedExample((List)conjunctions, (List)rules);
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateVisitor.class

##### procyon -ec {}

```diff
@@ -13,17 +13,14 @@
     public PredicateVisitor(final PlainGrammarVisitor this$0, final int arity) {
         this.this$0 = this$0;
         this.arity = -1;
         this.arity = arity;
     }
     
     public WeightedPredicate visitPredicate(@NotNull final NeuralogicParser.PredicateContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         if (ctx.INT() != null) {
             try {
                 this.arity = Integer.parseInt(ctx.INT().getText());
             }
             catch (final Exception ex) {
                 PlainGrammarVisitor.access$300().severe("Cannot parse arity of a predicate from " + ctx.getText());
             }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$TermVisitor.class

##### procyon -ec {}

```diff
@@ -12,17 +12,14 @@
     public VariableFactory variableFactory;
     
     private TermVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Term visitTerm(@NotNull final NeuralogicParser.TermContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         Term term;
         if (ctx.constant() != null) {
             term = (Term)this.this$0.builder.constantFactory.construct(ctx.getText());
         }
         else if (ctx.variable() != null) {
             term = (Term)this.variableFactory.construct(ctx.getText());
         }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$RuleLineVisitor.class

##### procyon -ec {}

```diff
@@ -22,17 +22,14 @@
     VariableFactory variableFactory;
     
     public RuleLineVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public WeightedRule visitLrnnRule(@NotNull final NeuralogicParser.LrnnRuleContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         this.variableFactory = new VariableFactory();
         final WeightedRule rule = new WeightedRule();
         rule.setOriginalString(ctx.getText());
         final PlainGrammarVisitor.AtomVisitor headVisitor = new PlainGrammarVisitor.AtomVisitor(this.this$0);
         headVisitor.variableFactory = this.variableFactory;
         final BodyAtom headAtom = (BodyAtom)ctx.atom().accept((ParseTreeVisitor)headVisitor);
         final Weight weight = headAtom.getConjunctWeight();
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$PredicateOffsetVisitor.class

##### procyon -ec {}

```diff
@@ -12,17 +12,14 @@
 public class PredicateOffsetVisitor extends NeuralogicBaseVisitor<Pair<WeightedPredicate, Weight>>
 {
     public PredicateOffsetVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public Pair<WeightedPredicate, Weight> visitPredicateOffset(@NotNull final NeuralogicParser.PredicateOffsetContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         int arity = -1;
         try {
             arity = Integer.parseInt(ctx.predicate().INT().getText());
         }
         catch (final Exception ex) {
             PlainGrammarVisitor.access$300().severe("Cannot parse arity of a predicate from " + ctx.getText());
         }
```

#### cz/cvut/fel/ida/logic/parsing/grammarParsing/PlainGrammarVisitor$AtomConjunctionVisitor.class

##### procyon -ec {}

```diff
@@ -17,16 +17,13 @@
     VariableFactory variableFactory;
     
     public AtomConjunctionVisitor(final PlainGrammarVisitor this$0) {
         this.this$0 = this$0;
     }
     
     public List<BodyAtom> visitConjunction(@NotNull final NeuralogicParser.ConjunctionContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final PlainGrammarVisitor.AtomVisitor atomVisitor = new PlainGrammarVisitor.AtomVisitor(this.this$0);
         atomVisitor.variableFactory = this.variableFactory;
         final List<BodyAtom> atomList = (List)ctx.atom().stream().map(AtomConjunctionVisitor::lambda$visitConjunction$0).collect(Collectors.toList());
         return atomList;
     }
 }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$PredicatesMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -20,17 +20,14 @@
 public class PredicatesMetadataVisitor extends NeuralogicBaseVisitor<List<Pair<WeightedPredicate, Map<String, Object>>>>
 {
     public PredicatesMetadataVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public List<Pair<WeightedPredicate, Map<String, Object>>> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.PredicateOffsetVisitor predicateOffsetVisitor = new PlainGrammarVisitor.PredicateOffsetVisitor(obj);
         template_lines.stream().filter((Predicate<? super Object>)PredicatesMetadataVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)PredicatesMetadataVisitor::lambda$visitTemplateFile$1).collect((Collector<? super Object, ?, List<? super Object>>)Collectors.toList());
         final PlainGrammarVisitor obj2 = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj2);
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$ConjunctionsVisitor.class

##### procyon -ec {}

```diff
@@ -17,17 +17,14 @@
 public class ConjunctionsVisitor extends NeuralogicBaseVisitor<List<Conjunction>>
 {
     public ConjunctionsVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public List<Conjunction> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.FactConjunctionVisitor factConjunctionVisitor = new PlainGrammarVisitor.FactConjunctionVisitor(obj);
         final List<Conjunction> conjunctions = (List<Conjunction>)template_lines.stream().filter((Predicate<? super Object>)ConjunctionsVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)ConjunctionsVisitor::lambda$visitTemplateFile$1).collect((Collector<? super Object, ?, List<Conjunction>>)Collectors.toList());
         return conjunctions;
     }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$WeightsMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -20,17 +20,14 @@
 public class WeightsMetadataVisitor extends NeuralogicBaseVisitor<List<Pair<Weight, Map<String, Object>>>>
 {
     public WeightsMetadataVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public List<Pair<Weight, Map<String, Object>>> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.WeightMetadataVisitor weightMetadataVisitor = new PlainGrammarVisitor.WeightMetadataVisitor(obj);
         final List<Pair<Weight, Map<String, Object>>> weightMetadataList = (List<Pair<Weight, Map<String, Object>>>)((Map<Object, Object>)template_lines.stream().filter((Predicate<? super Object>)WeightsMetadataVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)WeightsMetadataVisitor::lambda$visitTemplateFile$1).collect(Collectors.toMap((Function<? super Object, ?>)WeightsMetadataVisitor::lambda$visitTemplateFile$2, (Function<? super Object, ?>)WeightsMetadataVisitor::lambda$visitTemplateFile$3, Metadata::merge))).entrySet().stream().map((Function<? super Object, ?>)WeightsMetadataVisitor::lambda$visitTemplateFile$4).collect((Collector<? super Object, ?, List<Pair<Weight, Map<String, Object>>>>)Collectors.toList());
         return weightMetadataList;
     }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor.class

##### procyon -ec {}

```diff
@@ -20,70 +20,34 @@
     private static final Logger LOG;
     
     public PlainTemplateParseTreeExtractor(final PlainGrammarVisitor visitor) {
         super((GrammarVisitor)visitor);
     }
     
     public List<WeightedRule> getWeightedRules(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         return new PlainTemplateParseTreeExtractor.RuleLinesVisitor(this).visitTemplateFile(ctx);
     }
     
     public List<ValuedFact> getWeightedFacts(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(1);
-        }
         return new PlainTemplateParseTreeExtractor.FactsVisitor(this).visitTemplateFile(ctx);
     }
     
     public List<Conjunction> getWeightedConjunctions(final NeuralogicParser.TemplateFileContext ctx) {
         return new PlainTemplateParseTreeExtractor.ConjunctionsVisitor(this).visitTemplateFile(ctx);
     }
     
     public List<Pair<Weight, Map<String, Object>>> getWeightsMetadata(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(2);
-        }
         return new PlainTemplateParseTreeExtractor.WeightsMetadataVisitor(this).visitTemplateFile(ctx);
     }
     
     public List<Pair<WeightedPredicate, Map<String, Object>>> getPredicatesMetadata(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(3);
-        }
         return new PlainTemplateParseTreeExtractor.PredicatesMetadataVisitor(this).visitTemplateFile(ctx);
     }
     
     public Map<String, Object> getTemplateMetadata(final NeuralogicParser.TemplateFileContext ctx) {
         return null;
     }
     
     static {
         LOG = Logger.getLogger(PlainTemplateParseTreeExtractor.class.getName());
     }
-    
-    private static /* synthetic */ void $$$reportNull$$$0(final int n) {
-        final String format = "Argument for @NotNull parameter '%s' of %s.%s must not be null";
-        final Object[] args = { "ctx", "cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor", null };
-        switch (n) {
-            default: {
-                args[2] = "getWeightedRules";
-                break;
-            }
-            case 1: {
-                args[2] = "getWeightedFacts";
-                break;
-            }
-            case 2: {
-                args[2] = "getWeightsMetadata";
-                break;
-            }
-            case 3: {
-                args[2] = "getPredicatesMetadata";
-                break;
-            }
-        }
-        throw new IllegalArgumentException(String.format(format, args));
-    }
 }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$RuleLinesVisitor.class

##### procyon -ec {}

```diff
@@ -17,17 +17,14 @@
 public class RuleLinesVisitor extends NeuralogicBaseVisitor<List<WeightedRule>>
 {
     public RuleLinesVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public List<WeightedRule> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.RuleLineVisitor ruleLineVisitor = new PlainGrammarVisitor.RuleLineVisitor(obj);
         final List<WeightedRule> rules = (List<WeightedRule>)template_lines.stream().filter((Predicate<? super Object>)RuleLinesVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)RuleLinesVisitor::lambda$visitTemplateFile$1).collect((Collector<? super Object, ?, List<WeightedRule>>)Collectors.toList());
         return rules;
     }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$FactsVisitor.class

##### procyon -ec {}

```diff
@@ -17,17 +17,14 @@
 public class FactsVisitor extends NeuralogicBaseVisitor<List<ValuedFact>>
 {
     public FactsVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public List<ValuedFact> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.FactVisitor factVisitor = new PlainGrammarVisitor.FactVisitor(obj);
         final List<ValuedFact> facts = (List<ValuedFact>)template_lines.stream().filter((Predicate<? super Object>)FactsVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)FactsVisitor::lambda$visitTemplateFile$1).collect((Collector<? super Object, ?, List<ValuedFact>>)Collectors.toList());
         return facts;
     }
```

#### cz/cvut/fel/ida/logic/parsing/template/PlainTemplateParseTreeExtractor$TemplateMetadataVisitor.class

##### procyon -ec {}

```diff
@@ -18,17 +18,14 @@
 public class TemplateMetadataVisitor extends NeuralogicBaseVisitor<Map<String, Object>>
 {
     public TemplateMetadataVisitor(final PlainTemplateParseTreeExtractor this$0) {
         this.this$0 = this$0;
     }
     
     public Map<String, Object> visitTemplateFile(@NotNull final NeuralogicParser.TemplateFileContext ctx) {
-        if (ctx == null) {
-            $$$reportNull$$$0(0);
-        }
         final List<NeuralogicParser.TemplateLineContext> template_lines = ctx.templateLine();
         final PlainGrammarVisitor obj = (PlainGrammarVisitor)this.this$0.visitor;
         Objects.requireNonNull(obj);
         final PlainGrammarVisitor.TemplateMetadataVisitor templateMetadataVisitor = new PlainGrammarVisitor.TemplateMetadataVisitor(obj);
         final Map<String, Object> metadata = (Map<String, Object>)template_lines.stream().filter((Predicate<? super Object>)TemplateMetadataVisitor::lambda$visitTemplateFile$0).map((Function<? super Object, ?>)TemplateMetadataVisitor::lambda$visitTemplateFile$1).flatMap((Function<? super Object, ? extends Stream<?>>)TemplateMetadataVisitor::lambda$visitTemplateFile$2).collect(Collectors.toMap((Function<? super Object, ? extends String>)Map.Entry::getKey, (Function<? super Object, ?>)Map.Entry::getValue, (BinaryOperator<Object>)null));
         return metadata;
     }
```

### Comparing `neuralogic-0.7.8/neuralogic/logging/__init__.py` & `neuralogic-0.7.9/neuralogic/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/base.py` & `neuralogic-0.7.9/neuralogic/nn/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, Optional, Union, Callable, List
 
 from neuralogic.core.settings import Settings
 from neuralogic.core.builder import DatasetBuilder
-from neuralogic.core import Template, BuiltDataset, SettingsProxy
+from neuralogic.core import Template, BuiltDataset, SettingsProxy, GroundedDataset
 from neuralogic.dataset.base import BaseDataset
 
 from neuralogic.utils.visualize import draw_model
 
 
 class AbstractNeuraLogic:
     def __init__(self, dataset_builder: DatasetBuilder, template: Template, settings: SettingsProxy):
@@ -20,23 +20,39 @@
 
         self.hooks_set = False
         self.hooks: Dict[str, List[Callable]] = {}
 
     def __call__(self, sample):
         raise NotImplementedError
 
-    def build_dataset(
+    def ground(
         self,
         dataset: BaseDataset,
         *,
         batch_size: int = 1,
         file_mode: bool = False,
         learnable_facts: bool = False,
+    ) -> GroundedDataset:
+        return self.dataset_builder.ground_dataset(
+            dataset,
+            self.settings,
+            batch_size=batch_size,
+            file_mode=file_mode,
+            learnable_facts=learnable_facts,
+        )
+
+    def build_dataset(
+        self,
+        dataset: Union[BaseDataset, GroundedDataset],
+        *,
+        batch_size: int = 1,
+        file_mode: bool = False,
+        learnable_facts: bool = False,
         progress: bool = False,
-    ):
+    ) -> BuiltDataset:
         return self.dataset_builder.build_dataset(
             dataset,
             self.settings,
             batch_size=batch_size,
             file_mode=file_mode,
             learnable_facts=learnable_facts,
             progress=progress,
@@ -86,22 +102,22 @@
 
     def load_state_dict(self, state_dict: Dict):
         raise NotImplementedError
 
     def draw(
         self,
         filename: Optional[str] = None,
-        draw_ipython=True,
+        show=True,
         img_type="png",
         value_detail: int = 0,
         graphviz_path: Optional[str] = None,
         *args,
         **kwargs,
     ):
-        return draw_model(self, filename, draw_ipython, img_type, value_detail, graphviz_path, *args, **kwargs)
+        return draw_model(self, filename, show, img_type, value_detail, graphviz_path, *args, **kwargs)
 
 
 class AbstractEvaluator:
     def __init__(self, template: Template, settings: Settings):
         self.settings = settings.create_proxy()
 
         self.neuralogic_model = template.build(settings)
@@ -147,17 +163,15 @@
 
     def reset_parameters(self):
         self.neuralogic_model.reset_parameters()
 
     def draw(
         self,
         filename: Optional[str] = None,
-        draw_ipython=True,
+        show=True,
         img_type="png",
         value_detail: int = 0,
         graphviz_path: Optional[str] = None,
         *args,
         **kwargs,
     ):
-        return self.neuralogic_model.draw(
-            filename, draw_ipython, img_type, value_detail, graphviz_path, *args, **kwargs
-        )
+        return self.neuralogic_model.draw(filename, show, img_type, value_detail, graphviz_path, *args, **kwargs)
```

### Comparing `neuralogic-0.7.8/neuralogic/nn/evaluator/java.py` & `neuralogic-0.7.9/neuralogic/nn/evaluator/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/functional.py` & `neuralogic-0.7.9/neuralogic/nn/functional.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/init.py` & `neuralogic-0.7.9/neuralogic/nn/init.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/java.py` & `neuralogic-0.7.9/neuralogic/nn/java.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/loss.py` & `neuralogic-0.7.9/neuralogic/nn/loss.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/__init__.py` & `neuralogic-0.7.9/neuralogic/nn/module/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/attention.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/attention.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/gru.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/gru.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/linear.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/linear.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/lstm.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/lstm.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/mlp.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/mlp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/pooling.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/pooling.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/positional_encoding.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/positional_encoding.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/rnn.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/rnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/rvnn.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/rvnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/general/transformer.py` & `neuralogic-0.7.9/neuralogic/nn/module/general/transformer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/appnp.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/appnp.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/gatv2.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/gatv2.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/gcn.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/gcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/gin.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/gin.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/gsage.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/gsage.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/res_gated.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/res_gated.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/rgcn.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/rgcn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/sg.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/sg.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/gnn/tag.py` & `neuralogic-0.7.9/neuralogic/nn/module/gnn/tag.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/meta/magnn.py` & `neuralogic-0.7.9/neuralogic/nn/module/meta/magnn.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/module/meta/meta.py` & `neuralogic-0.7.9/neuralogic/nn/module/meta/meta.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/nn/torch_function.py` & `neuralogic-0.7.9/neuralogic/nn/torch_function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/adam.py` & `neuralogic-0.7.9/neuralogic/optim/adam.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/lr_scheduler/arithmetic.py` & `neuralogic-0.7.9/neuralogic/optim/lr_scheduler/arithmetic.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/lr_scheduler/geometric.py` & `neuralogic-0.7.9/neuralogic/optim/lr_scheduler/geometric.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/lr_scheduler/lr_decay.py` & `neuralogic-0.7.9/neuralogic/optim/lr_scheduler/lr_decay.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/optimizer.py` & `neuralogic-0.7.9/neuralogic/optim/optimizer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/optim/sgd.py` & `neuralogic-0.7.9/neuralogic/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/__init__.py` & `neuralogic-0.7.9/neuralogic/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/atomEmbeddings3.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/molecules/mutagenesis/template.txt_merged.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/embeddings.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/embeddings.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/examples.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/nations/queries.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/nations/queries.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/examples.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/examples.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic/utils/data/datasets/simple/trains/template.txt` & `neuralogic-0.7.9/neuralogic/utils/data/datasets/simple/trains/template.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/neuralogic.egg-info/PKG-INFO` & `neuralogic-0.7.9/neuralogic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: neuralogic
-Version: 0.7.8
+Version: 0.7.9
 Summary: PyNeuraLogic lets you use Python to create Differentiable Logic Programs.
 Home-page: https://github.com/LukasZahradnik/PyNeuraLogic
 Author: Lukáš Zahradník
 Author-email: lukaszahradnik96@seznam.cz
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: JPype1>=1.3.0
-Requires-Dist: numpy>=1.19.0
+Requires-Dist: numpy>=1.20.4
+Requires-Dist: matplotlib
 Requires-Dist: tqdm
 
 
 <p align="center">
 <img src="https://github.com/LukasZahradnik/PyNeuraLogic/blob/master/docs/_static/readme_logo.svg" alt="PyNeuraLogic" title="PyNeuraLogic"/>
 </p>
 
@@ -125,15 +126,15 @@
 
 
 ### Prerequisites
 
 To use PyNeuraLogic, you need to install the following prerequisites:
 
 ```
-Python >= 3.7
+Python >= 3.8
 Java >= 1.8
 ```
 
 In case you want to use visualization provided in the library, it is required to have [Graphviz](https://graphviz.org/download/) installed.
 
 ## 🔬 Examples
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: neuralogic Version: 0.7.8 Summary: PyNeuraLogic
+Metadata-Version: 2.1 Name: neuralogic Version: 0.7.9 Summary: PyNeuraLogic
 lets you use Python to create Differentiable Logic Programs. Home-page: https:/
 /github.com/LukasZahradnik/PyNeuraLogic Author: LukÃ¡Å¡ ZahradnÃ­k Author-
 email: lukaszahradnik96@seznam.cz License: MIT Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Programming
 Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Topic :: Scientific/Engineering :: Artificial Intelligence Requires-Python:
 >=3.7.0 Description-Content-Type: text/markdown License-File: LICENSE Requires-
-Dist: JPype1>=1.3.0 Requires-Dist: numpy>=1.19.0 Requires-Dist: tqdm
+Dist: JPype1>=1.3.0 Requires-Dist: numpy>=1.20.4 Requires-Dist: matplotlib
+Requires-Dist: tqdm
                                 [PyNeuraLogic]
 [![PyPI version](https://badge.fury.io/py/neuralogic.svg)](https://
 badge.fury.io/py/neuralogic) [![License](https://img.shields.io/pypi/l/
 neuralogic)](https://badge.fury.io/py/neuralogic) [![Tests Status](https://
 github.com/LukasZahradnik/PyNeuraLogic/actions/workflows/tests.yml/badge.svg)]
 (https://github.com/LukasZahradnik/PyNeuraLogic/actions/workflows/tests.yml) [!
 [Code Quality Status](https://github.com/LukasZahradnik/PyNeuraLogic/actions/
@@ -87,15 +88,15 @@
 
 We hope you'll find the framework useful in designing _your own_ deep
 **relational** learning ideas beyond the GNNs! Please let us know if you need
 some guidance or would like to cooperate! ## ð¡ Getting started ###
 Installation To install PyNeuraLogic's latest release from the PyPI repository,
 use the following command: ```commandline $ pip install neuralogic ``` ###
 Prerequisites To use PyNeuraLogic, you need to install the following
-prerequisites: ``` Python >= 3.7 Java >= 1.8 ``` In case you want to use
+prerequisites: ``` Python >= 3.8 Java >= 1.8 ``` In case you want to use
 visualization provided in the library, it is required to have [Graphviz](https:
 //graphviz.org/download/) installed. ## ð¬ Examples [![Open In Colab](https:/
 /colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/LukasZahradnik/PyNeuraLogic/blob/master/
 examples/SimpleXOR.ipynb) [Simple XOR example](https://github.com/
 LukasZahradnik/PyNeuraLogic/blob/master/examples/SimpleXOR.ipynb)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
```

### Comparing `neuralogic-0.7.8/neuralogic.egg-info/SOURCES.txt` & `neuralogic-0.7.9/neuralogic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/setup.py` & `neuralogic-0.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 EMAIL = "lukaszahradnik96@seznam.cz"
 AUTHOR = "Lukáš Zahradník"
 REQUIRES_PYTHON = ">=3.7.0"
 VERSION = None
 
 REQUIRED = [
     "JPype1 >=1.3.0",
-    "numpy >= 1.19.0",
+    "numpy >= 1.20.4",
+    "matplotlib",
     "tqdm",
 ]
 
 EXTRAS: Dict = {}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
@@ -63,13 +64,13 @@
         "License :: OSI Approved :: MIT License",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
 )
```

### Comparing `neuralogic-0.7.8/tests/test_constructs.py` & `neuralogic-0.7.9/tests/test_constructs.py`

 * *Files 7% similar despite different names*

```diff
@@ -170,7 +170,22 @@
     assert terms[1] == V.Y
     assert terms[2] == V.Z
 
     my_rule = R.a <= R.b
 
     assert len(my_rule.body) == 1
     assert my_rule.body[0].predicate.name == "b"
+
+
+def test_rules_and():
+    my_rule: Rule = R.a(V.X) <= R.b(V.Y) & R.c(V.Z) & R.d
+
+    assert len(my_rule.body) == 3
+    assert str(my_rule.body[0]) == "b(Y)."
+    assert str(my_rule.body[1]) == "c(Z)."
+    assert str(my_rule.body[2]) == "d."
+
+
+def test_rules_and_with_metadata():
+    my_rule: Rule = R.a(V.X) <= R.b(V.Y) & R.c(V.Z) & R.d | [Transformation.SIGMOID]
+
+    assert str(my_rule) == "a(X) :- b(Y), c(Z), d. [transformation=sigmoid]"
```

### Comparing `neuralogic-0.7.8/tests/test_csv_datasets.py` & `neuralogic-0.7.9/tests/test_csv_datasets.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_datasets.py` & `neuralogic-0.7.9/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_drawing.py` & `neuralogic-0.7.9/tests/test_drawing.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,51 +6,51 @@
 from neuralogic.core import Settings
 
 
 def test_draw_model():
     template, dataset = XOR_Vectorized()
     model = template.build(Settings())
 
-    result = draw_model(model, draw_ipython=False)
+    result = draw_model(model, show=False)
 
     assert isinstance(result, bytes)
     assert len(result) > 0
 
 
 def test_draw_sample():
     template, dataset = XOR_Vectorized()
     model = template.build(Settings())
 
     built_dataset = model.build_dataset(dataset)
-    result = draw_sample(built_dataset.samples[0], draw_ipython=False)
+    result = draw_sample(built_dataset.samples[0], show=False)
 
     assert isinstance(result, bytes)
     assert len(result) > 0
 
 
 def test_draw_model_from_template():
     template, dataset = XOR_Vectorized()
-    result = template.draw(draw_ipython=False)
+    result = template.draw(show=False)
 
     assert isinstance(result, bytes)
     assert len(result) > 0
 
 
 def test_draw_model_from_evaluator():
     template, dataset = XOR_Vectorized()
 
     evaluator = get_evaluator(template)
-    result = evaluator.draw(draw_ipython=False)
+    result = evaluator.draw(show=False)
 
     assert isinstance(result, bytes)
     assert len(result) > 0
 
 
 def test_draw_sample_from_raw_sample():
     template, dataset = XOR_Vectorized()
     model = template.build(Settings())
 
     built_dataset = model.build_dataset(dataset)
-    result = built_dataset.samples[0].draw(draw_ipython=False)
+    result = built_dataset.samples[0].draw(show=False)
 
     assert isinstance(result, bytes)
     assert len(result) > 0
```

### Comparing `neuralogic-0.7.8/tests/test_evaluation_inference_engine.py` & `neuralogic-0.7.9/tests/test_evaluation_inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_function.py` & `neuralogic-0.7.9/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_general_modules.py` & `neuralogic-0.7.9/tests/test_general_modules.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_inference_engine.py` & `neuralogic-0.7.9/tests/test_inference_engine.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_java_evaluator.py` & `neuralogic-0.7.9/tests/test_java_evaluator.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_modules.py` & `neuralogic-0.7.9/tests/test_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,24 +117,24 @@
 
 
 def test_sgconv():
     template = Template()
 
     template += SGConv(1, 2, "h1", "h0", "_edge", k=2)
     template_str = str(template).split("\n")
-    rule = "{2, 1} h1(I0) :- h0(I2), *edge(I1, I0), *edge(I2, I1). [transformation=identity, aggregation=sum]"
+    rule = "{2, 1} h1(I0) :- h0(I2), *edge(I1, I0), *edge(I2, I1). [transformation=identity, aggregation=sum, duplicit_grounding=True]"
 
     assert template_str[0] == rule
     assert template_str[1] == "h1/1 [transformation=identity]"
 
     template = Template()
 
     template += SGConv(1, 2, "h1", "h0", "_edge")
     template_str = str(template).split("\n")
-    rule = "{2, 1} h1(I0) :- h0(I1), *edge(I1, I0). [transformation=identity, aggregation=sum]"
+    rule = "{2, 1} h1(I0) :- h0(I1), *edge(I1, I0). [transformation=identity, aggregation=sum, duplicit_grounding=True]"
 
     assert template_str[0] == rule
     assert template_str[1] == "h1/1 [transformation=identity]"
 
 
 def test_appnp():
     template = Template()
```

### Comparing `neuralogic-0.7.8/tests/test_quick_start.py` & `neuralogic-0.7.9/tests/test_quick_start.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_recurrent_modules.py` & `neuralogic-0.7.9/tests/test_recurrent_modules.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_settings.py` & `neuralogic-0.7.9/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_special_predicates.py` & `neuralogic-0.7.9/tests/test_special_predicates.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_torch_function.py` & `neuralogic-0.7.9/tests/test_torch_function.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_transformer.py` & `neuralogic-0.7.9/tests/test_transformer.py`

 * *Files identical despite different names*

### Comparing `neuralogic-0.7.8/tests/test_xor_generalization.py` & `neuralogic-0.7.9/tests/test_xor_generalization.py`

 * *Files identical despite different names*

