# Comparing `tmp/lightnet-3.1.0.tar.gz` & `tmp/lightnet-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lightnet-3.1.0.tar", last modified: Mon Dec  5 11:20:34 2022, max compression
+gzip compressed data, was "/builds/EAVISE/lightnet/dist/.tmp-e4mx1zy6/lightnet-4.0.0.tar", last modified: Wed Apr  3 07:38:55 2024, max compression
```

## Comparing `lightnet-3.1.0.tar` & `lightnet-4.0.0.tar`

### file list

```diff
@@ -1,143 +1,146 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/test/
--rw-rw-rw-   0 root         (0) root         (0)     3678 2022-12-05 11:19:07.000000 lightnet-3.1.0/test/test_fusion.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2022-12-05 11:19:07.000000 lightnet-3.1.0/test/test_remap.py
--rw-rw-rw-   0 root         (0) root         (0)     4933 2022-12-05 11:19:07.000000 lightnet-3.1.0/test/test_layer_reorg.py
--rw-rw-rw-   0 root         (0) root         (0)    13947 2022-12-05 11:19:07.000000 lightnet-3.1.0/test/test_networks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/
--rw-rw-rw-   0 root         (0) root         (0)     1422 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/_imports.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/_compat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/util/
--rw-rw-rw-   0 root         (0) root         (0)     1861 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/_coords.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/_mask.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3117 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/_module.py
--rw-rw-rw-   0 root         (0) root         (0)    38464 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/_anchors.py
--rw-rw-rw-   0 root         (0) root         (0)     6967 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/util/_iou.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/loss/
--rw-rw-rw-   0 root         (0) root         (0)    18359 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/_region_masked.py
--rw-rw-rw-   0 root         (0) root         (0)    16150 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/_region_oriented.py
--rw-rw-rw-   0 root         (0) root         (0)     7887 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    11783 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/_corner.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18407 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/loss/_region.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/backbone/
--rw-rw-rw-   0 root         (0) root         (0)    11078 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_mobilenet.py
--rw-rw-rw-   0 root         (0) root         (0)    14684 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_resnet.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20126 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)    20817 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_vgg.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_deform_resnet.py
--rw-rw-rw-   0 root         (0) root         (0)     8053 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_cornernet.py
--rw-rw-rw-   0 root         (0) root         (0)    18547 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_mobile_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/backbone/_alexnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/layer/
--rw-rw-rw-   0 root         (0) root         (0)     7715 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_mobilenet.py
--rw-rw-rw-   0 root         (0) root         (0)      262 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5040 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)    22710 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_fusion.py
--rw-rw-rw-   0 root         (0) root         (0)     6165 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_deform.py
--rw-rw-rw-   0 root         (0) root         (0)     6538 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_fpn.py
--rw-rw-rw-   0 root         (0) root         (0)     8415 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_conv.py
--rw-rw-rw-   0 root         (0) root         (0)     9557 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_hourglass.py
--rw-rw-rw-   0 root         (0) root         (0)     5621 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_cornernet.py
--rw-rw-rw-   0 root         (0) root         (0)    21867 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/layer/_util.py
--rw-rw-rw-   0 root         (0) root         (0)     3372 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/_basemodule.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/head/
--rw-rw-rw-   0 root         (0) root         (0)      301 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2166 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_classification_conv.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_classification_fc.py
--rw-rw-rw-   0 root         (0) root         (0)     5570 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_detection_corner.py
--rw-rw-rw-   0 root         (0) root         (0)     2386 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_detection_anchor_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     4369 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_detection_anchor_masked.py
--rw-rw-rw-   0 root         (0) root         (0)     4262 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_detection_yolact.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/head/_detection_anchor_oriented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/network/module/
--rw-rw-rw-   0 root         (0) root         (0)      132 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/module/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10137 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/module/_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)    18908 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/module/_fusion.py
--rw-rw-rw-   0 root         (0) root         (0)    21161 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/network/module/_lightnet.py
--rw-rw-rw-   0 root         (0) root         (0)      372 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/data/
--rw-rw-rw-   0 root         (0) root         (0)      276 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/data/transform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/data/transform/post/
--rw-rw-rw-   0 root         (0) root         (0)     6525 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_anchor_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     8092 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_anchor_masked.py
--rw-rw-rw-   0 root         (0) root         (0)    10061 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_brambox.py
--rw-rw-rw-   0 root         (0) root         (0)     5596 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5306 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_corner.py
--rw-rw-rw-   0 root         (0) root         (0)      374 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6103 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_anchor_oriented.py
--rw-rw-rw-   0 root         (0) root         (0)     8930 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_reverse_fit.py
--rw-rw-rw-   0 root         (0) root         (0)    16847 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/post/_nms.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16563 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/_compose.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/data/transform/pre/
--rw-rw-rw-   0 root         (0) root         (0)    20331 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/pre/_fit.py
--rw-rw-rw-   0 root         (0) root         (0)    16157 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/pre/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      325 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/pre/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14381 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/transform/pre/_augment.py
--rw-rw-rw-   0 root         (0) root         (0)     9492 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/data/_dataloading.py
--rw-rw-rw-   0 root         (0) root         (0)     4381 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/prune/
--rw-rw-rw-   0 root         (0) root         (0)    13240 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/_multi.py
--rw-rw-rw-   0 root         (0) root         (0)     3000 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/_l2.py
--rw-rw-rw-   0 root         (0) root         (0)     2574 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/_gm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/prune/dependency/
--rw-rw-rw-   0 root         (0) root         (0)     4933 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/dependency/_tree.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/dependency/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8018 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/dependency/_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4350 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/dependency/_dependency.py
--rw-rw-rw-   0 root         (0) root         (0)     3503 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/prune/dependency/_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/models/
--rw-rw-rw-   0 root         (0) root         (0)     7627 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolo_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     7707 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolt.py
--rw-rw-rw-   0 root         (0) root         (0)     3286 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_tiny_yolo_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_tiny_yolo_v3.py
--rw-rw-rw-   0 root         (0) root         (0)     2287 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobilenet_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     7564 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_dyolo.py
--rw-rw-rw-   0 root         (0) root         (0)     1755 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_alexnet.py
--rw-rw-rw-   0 root         (0) root         (0)     8938 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolact.py
--rw-rw-rw-   0 root         (0) root         (0)     1227 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7280 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_resnet.py
--rw-rw-rw-   0 root         (0) root         (0)     5412 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_vgg.py
--rw-rw-rw-   0 root         (0) root         (0)     9652 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolo_fusion.py
--rw-rw-rw-   0 root         (0) root         (0)    13366 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_cornernet.py
--rw-rw-rw-   0 root         (0) root         (0)     4358 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobile_yolo_v2_upsample.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobilenet_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_darknet19.py
--rw-rw-rw-   0 root         (0) root         (0)     5100 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_darknet53.py
--rw-rw-rw-   0 root         (0) root         (0)    16847 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolo_v3.py
--rw-rw-rw-   0 root         (0) root         (0)     4397 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_yolo_v2_upsample.py
--rw-rw-rw-   0 root         (0) root         (0)    10809 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_resnet_yolo.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobilenet_v1.py
--rw-rw-rw-   0 root         (0) root         (0)     2666 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_dataset_brambox.py
--rw-rw-rw-   0 root         (0) root         (0)     1579 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobile_darknet19.py
--rw-rw-rw-   0 root         (0) root         (0)     2968 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_dataset_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)     1864 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_darknet.py
--rw-rw-rw-   0 root         (0) root         (0)    15909 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_cornernet_squeeze.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/models/_network_mobile_yolo_v2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet/engine/
--rw-rw-rw-   0 root         (0) root         (0)    18010 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/engine/_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)      196 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/engine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20347 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/engine/_engine.py
--rw-rw-rw-   0 root         (0) root         (0)     5742 2022-12-05 11:19:07.000000 lightnet-3.1.0/lightnet/engine/_scheduler.py
--rw-r--r--   0 root         (0) root         (0)     3971 2022-12-05 11:20:34.000000 lightnet-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1050 2022-12-05 11:19:07.000000 lightnet-3.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-05 11:19:07.000000 lightnet-3.1.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 11:20:34.000000 lightnet-3.1.0/lightnet.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3971 2022-12-05 11:20:33.000000 lightnet-3.1.0/lightnet.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4160 2022-12-05 11:20:33.000000 lightnet-3.1.0/lightnet.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 11:20:33.000000 lightnet-3.1.0/lightnet.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-12-05 11:20:33.000000 lightnet-3.1.0/lightnet.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      109 2022-12-05 11:20:33.000000 lightnet-3.1.0/lightnet.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      968 2022-12-05 11:19:07.000000 lightnet-3.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     3668 2022-12-05 11:19:07.000000 lightnet-3.1.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      761 2022-12-05 11:20:34.000000 lightnet-3.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    80947 2022-12-05 11:19:07.000000 lightnet-3.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-04-03 07:37:46.000000 lightnet-4.0.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-03 07:37:46.000000 lightnet-4.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-04-03 07:38:55.000000 lightnet-4.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-03 07:37:46.000000 lightnet-4.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      364 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/_compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/_imports.py
+-rw-rw-rw-   0 root         (0) root         (0)     4381 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/_log.py
+-rw-r--r--   0 root         (0) root         (0)      497 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/data/
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9462 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/_dataloading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/data/transform/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16646 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/_compose.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/data/transform/post/
+-rw-rw-rw-   0 root         (0) root         (0)      374 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8092 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_anchor_masked.py
+-rw-rw-rw-   0 root         (0) root         (0)     6103 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_anchor_oriented.py
+-rw-rw-rw-   0 root         (0) root         (0)     6954 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_anchor_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     5596 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    10048 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_brambox.py
+-rw-rw-rw-   0 root         (0) root         (0)     5320 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_corner.py
+-rw-rw-rw-   0 root         (0) root         (0)    18342 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_nms.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/post/_reverse_fit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/data/transform/pre/
+-rw-rw-rw-   0 root         (0) root         (0)      325 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/pre/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14411 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/pre/_augment.py
+-rw-rw-rw-   0 root         (0) root         (0)    17028 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/pre/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24112 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/data/transform/pre/_fit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/engine/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/engine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20614 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/engine/_engine.py
+-rw-rw-rw-   0 root         (0) root         (0)    18010 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/engine/_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5742 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/engine/_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/models/
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2666 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_dataset_brambox.py
+-rw-rw-rw-   0 root         (0) root         (0)     2968 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_dataset_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1906 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_alexnet.py
+-rw-rw-rw-   0 root         (0) root         (0)    13382 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_cornernet.py
+-rw-rw-rw-   0 root         (0) root         (0)    13923 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_cornernet_squeeze.py
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_cspdarknet53.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_darknet19.py
+-rw-rw-rw-   0 root         (0) root         (0)     5102 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_darknet53.py
+-rw-rw-rw-   0 root         (0) root         (0)     7607 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_dyolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobile_darknet19.py
+-rw-rw-rw-   0 root         (0) root         (0)     4065 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobile_yolo_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobile_yolo_v2_upsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     2430 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobilenet_v1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2426 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobilenet_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3586 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_mobilenet_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)    11004 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_resnet.py
+-rw-rw-rw-   0 root         (0) root         (0)    10838 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_resnet_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     3329 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_tiny_yolo_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4888 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_tiny_yolo_v3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6022 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_vgg.py
+-rw-rw-rw-   0 root         (0) root         (0)     8951 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolact.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolo_fusion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7692 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolo_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4462 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolo_v2_upsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    20879 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolo_v3.py
+-rw-rw-rw-   0 root         (0) root         (0)    20761 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolo_v4.py
+-rw-rw-rw-   0 root         (0) root         (0)     7761 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/models/_network_yolt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3372 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/_basemodule.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/backbone/
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_alexnet.py
+-rw-rw-rw-   0 root         (0) root         (0)     8041 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_cornernet.py
+-rw-rw-rw-   0 root         (0) root         (0)    13323 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_csp.py
+-rw-rw-rw-   0 root         (0) root         (0)    22378 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)    20864 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_mobile_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)    12450 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_mobilenet.py
+-rw-rw-rw-   0 root         (0) root         (0)    22187 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_resnet.py
+-rw-rw-rw-   0 root         (0) root         (0)    23913 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/backbone/_vgg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/head/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_classification_conv.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_classification_fc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4363 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_detection_anchor_masked.py
+-rw-rw-rw-   0 root         (0) root         (0)     2271 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_detection_anchor_oriented.py
+-rw-rw-rw-   0 root         (0) root         (0)     2474 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_detection_anchor_yolo.py
+-rw-rw-rw-   0 root         (0) root         (0)     5554 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_detection_corner.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/head/_detection_yolact.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/layer/
+-rw-rw-rw-   0 root         (0) root         (0)      290 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11574 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_aggregation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9742 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_conv.py
+-rw-rw-rw-   0 root         (0) root         (0)     6117 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_cornernet.py
+-rw-rw-rw-   0 root         (0) root         (0)     4936 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_csp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5040 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)     6165 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_deform.py
+-rw-rw-rw-   0 root         (0) root         (0)    20208 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_fusion.py
+-rw-rw-rw-   0 root         (0) root         (0)     9552 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_hourglass.py
+-rw-rw-rw-   0 root         (0) root         (0)     8726 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_mobilenet.py
+-rw-rw-rw-   0 root         (0) root         (0)    22479 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/layer/_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/loss/
+-rw-rw-rw-   0 root         (0) root         (0)      162 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7887 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11783 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/_corner.py
+-rw-rw-rw-   0 root         (0) root         (0)    22817 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/_region.py
+-rw-rw-rw-   0 root         (0) root         (0)    18321 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/_region_masked.py
+-rw-rw-rw-   0 root         (0) root         (0)    16150 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/loss/_region_oriented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/network/module/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/module/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11077 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/module/_darknet.py
+-rw-rw-rw-   0 root         (0) root         (0)    12822 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/module/_fusion.py
+-rw-rw-rw-   0 root         (0) root         (0)    21419 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/network/module/_lightnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/prune/
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13240 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2574 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/_gm.py
+-rw-rw-rw-   0 root         (0) root         (0)     3000 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/_l2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/_multi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/prune/dependency/
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/dependency/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8018 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/dependency/_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4350 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/dependency/_dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)     4933 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/dependency/_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)     3503 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/prune/dependency/_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet/util/
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38785 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/_anchors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/_coords.py
+-rw-rw-rw-   0 root         (0) root         (0)    14460 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/_iou.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     3117 2024-04-03 07:37:46.000000 lightnet-4.0.0/lightnet/util/_module.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4266 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-03 07:38:55.000000 lightnet-4.0.0/lightnet.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      775 2024-04-03 07:38:55.000000 lightnet-4.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      968 2024-04-03 07:37:46.000000 lightnet-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 07:38:55.000000 lightnet-4.0.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)     3678 2024-04-03 07:37:46.000000 lightnet-4.0.0/test/test_fusion.py
+-rw-rw-rw-   0 root         (0) root         (0)     4933 2024-04-03 07:37:46.000000 lightnet-4.0.0/test/test_layer_reorg.py
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2024-04-03 07:37:46.000000 lightnet-4.0.0/test/test_networks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2024-04-03 07:37:46.000000 lightnet-4.0.0/test/test_remap.py
+-rw-rw-rw-   0 root         (0) root         (0)    80947 2024-04-03 07:37:46.000000 lightnet-4.0.0/versioneer.py
```

### Comparing `lightnet-3.1.0/test/test_fusion.py` & `lightnet-4.0.0/test/test_fusion.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/test/test_remap.py` & `lightnet-4.0.0/test/test_remap.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     (ln.models.Darknet19,       ln.models.YoloV2,                   ln.models.YoloV2.remap_darknet19),
     (ln.models.Darknet19,       ln.models.O_YoloV2,                 ln.models.O_YoloV2.remap_darknet19),
     (ln.models.Darknet19,       ln.models.M_YoloV2,                 ln.models.M_YoloV2.remap_darknet19),
     (ln.models.Darknet19,       ln.models.YoloV2Upsample,           ln.models.YoloV2Upsample.remap_darknet19),
     (ln.models.Darknet53,       ln.models.YoloV3,                   ln.models.YoloV3.remap_darknet53),
     (ln.models.Darknet53,       ln.models.O_YoloV3,                 ln.models.O_YoloV3.remap_darknet53),
     (ln.models.Darknet53,       ln.models.M_YoloV3,                 ln.models.M_YoloV3.remap_darknet53),
+    (ln.models.CSPDarknet53,    ln.models.YoloV4,                   ln.models.YoloV4.remap_cspdarknet53),
     (ln.models.Darknet19,       ln.models.Yolt,                     ln.models.Yolt.remap_darknet19),
     (ln.models.Darknet19,       ln.models.O_Yolt,                   ln.models.O_Yolt.remap_darknet19),
     (ln.models.Darknet19,       ln.models.M_Yolt,                   ln.models.M_Yolt.remap_darknet19),
     (ln.models.MobileDarknet19, ln.models.MobileYoloV2,             ln.models.MobileYoloV2.remap_mobile_darknet19),
     (ln.models.MobileDarknet19, ln.models.MobileYoloV2Upsample,     ln.models.MobileYoloV2Upsample.remap_mobile_darknet19),
     (ln.models.MobilenetV1,     ln.models.MobilenetYolo,            ln.models.MobilenetYolo.remap_mobilenet_v1),
     (ln.models.Resnet50,        ln.models.Yolact50,                 ln.models.Yolact50.remap_resnet),
@@ -39,17 +40,20 @@
     ln.models.Cornernet.remap_princeton_vl,
     ln.models.CornernetSqueeze.remap_princeton_vl,
     ln.models.Alexnet.remap_torchvision,
     ln.models.VGG11.remap_torchvision,
     ln.models.VGG13.remap_torchvision,
     ln.models.VGG16.remap_torchvision,
     ln.models.VGG19.remap_torchvision,
+    ln.models.Resnet18.remap_torchvision,
+    ln.models.Resnet34.remap_torchvision,
     ln.models.Resnet50.remap_torchvision,
     ln.models.Resnet101.remap_torchvision,
     ln.models.Resnet152.remap_torchvision,
+    ln.models.YoloV4.remap_tianxiaomo,
     ln.models.Yolact50.remap_dbolya,
     ln.models.Yolact101.remap_dbolya,
 ]
 
 
 @pytest.mark.parametrize('remap', remaps)
 def test_remapping(remap, tmp_path):
```

### Comparing `lightnet-3.1.0/test/test_layer_reorg.py` & `lightnet-4.0.0/test/test_layer_reorg.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/test/test_networks.py` & `lightnet-4.0.0/test/test_networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,23 @@
 import inspect
 import pytest
 import torch
 import lightnet as ln
 
 classification_networks = [
     'Alexnet',
+    'CSPDarknet53',
     'Darknet',
     'Darknet19',
     'Darknet53',
     'MobileDarknet19',
     'MobilenetV1',
     'MobilenetV2',
+    'Resnet18',
+    'Resnet34',
     'Resnet50',
     'Resnet101',
     'Resnet152',
     'VGG11',
     'VGG13',
     'VGG16',
     'VGG19',
@@ -31,14 +34,15 @@
     'MobileYoloV2Upsample',
     'ResnetYolo',
     'TinyYoloV2',
     'TinyYoloV3',
     'YoloV2',
     'YoloV2Upsample',
     'YoloV3',
+    'YoloV4',
     'Yolt',
 ]
 oriented_anchor_detection_networks = [
     'O_DYolo',
     'O_YoloV2',
     'O_YoloV3',
     'O_Yolt',
```

### Comparing `lightnet-3.1.0/lightnet/_imports.py` & `lightnet-4.0.0/lightnet/_imports.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,42 +19,42 @@
 ]
 log = logging.getLogger(__name__)
 
 
 try:
     import brambox as bb
 except ModuleNotFoundError:
-    warnings.warn('Brambox is not installed and thus all data functionality related to it cannot be used', category=ImportWarning)
+    warnings.warn('Brambox is not installed and thus all data functionality related to it cannot be used', category=ImportWarning, stacklevel=2)
     bb = None
 
 try:
     import cv2
 except ModuleNotFoundError:
-    warnings.warn('OpenCV is not installed and cannot be used', category=ImportWarning)
+    warnings.warn('OpenCV is not installed and cannot be used', category=ImportWarning, stacklevel=2)
     cv2 = None
 
 try:
     from PIL import Image, ImageOps
 except ModuleNotFoundError:
-    warnings.warn('Pillow is not installed and cannot be used', category=ImportWarning)
+    warnings.warn('Pillow is not installed and cannot be used', category=ImportWarning, stacklevel=2)
     Image, ImageOps = None, None
 
 try:
     import onnx
     from onnx import numpy_helper as onnx_numpy_helper
 except ModuleNotFoundError:
-    warnings.warn('ONNX is not installed and thus no pruning functionality will work', category=ImportWarning)
+    warnings.warn('ONNX is not installed and thus no pruning functionality will work', category=ImportWarning, stacklevel=2)
     onnx = None
     onnx_numpy_helper = None
 
 try:
     import pygeos
     import pgpd
 except ModuleNotFoundError:
-    warnings.warn('PyGEOS and PyGEOS-Pandas are not installed and thus no instance segmentation functionality will work', category=ImportWarning)
+    warnings.warn('PyGEOS and PyGEOS-Pandas are not installed and thus no instance segmentation functionality will work', category=ImportWarning, stacklevel=2)
     pygeos = None
     pgpd = None
 
 try:
     from tqdm.auto import tqdm
     tqdm.pandas()
 except ModuleNotFoundError:
```

### Comparing `lightnet-3.1.0/lightnet/util/_coords.py` & `lightnet-4.0.0/lightnet/util/_coords.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #
 #   Coordinate Utilities
 #   Copyright EAVISE
 #
+import numpy as np
 import torch
 
 __all__ = ['cwh_xyxy', 'tlwh_xyxy', 'xyxy_cwh']
 
 
 def cwh_xyxy(coords, cat=True):
     """ Transform coordinates from the (xc, yc, w, h) to the (x1, y1, x2, y2) format.
@@ -17,17 +18,18 @@
     Returns:
         torch.Tensor or tuple<torch.Tensor>
     """
     xy1 = (coords[:, :2] - (coords[:, 2:4] / 2))
     xy2 = (coords[:, :2] + (coords[:, 2:4] / 2))
 
     if cat:
-        return torch.cat((xy1, xy2), dim=1)
+        cat = torch.concatenate if isinstance(coords, torch.Tensor) else np.concatenate
+        return cat((xy1, xy2), axis=1)
     else:
-        return (*xy1.split(1, 1), *xy2.split(1, 1))
+        return (xy1[:, 0:1], xy1[:, 1:2], xy2[:, 0:1], xy2[:, 1:2])
 
 
 def tlwh_xyxy(coords, cat=True):
     """ Transform coordinates from the (xtl, ytl, w, h) to the (x1, y1, x2, y2) format.
 
     Args:
         coords (torch.Tensor): List of bounding boxes in the TLWH format.
@@ -36,16 +38,17 @@
     Returns:
         torch.Tensor or tuple<torch.Tensor>
     """
     x1, y1 = coords[:, 0:1], coords[:, 1:2]
     xy2 = coords[:, :2] + coords[:, 2:4]
 
     if cat:
-        return torch.cat((x1, y1, xy2), dim=1)
-    return (x1, y1, *xy2.split(1, 1))
+        cat = torch.concatenate if isinstance(coords, torch.Tensor) else np.concatenate
+        return cat((x1, y1, xy2), axis=1)
+    return (x1, y1, xy2[:, 0:1], xy2[:, 1:2])
 
 
 def xyxy_cwh(coords, cat=True):
     """ Transform coordinates from the (x1, y1, x2, y2) to the (xc, yc, w, h) format.
 
     Args:
         coords (torch.Tensor): List of bounding boxes in the XYXY format.
@@ -54,10 +57,11 @@
     Returns:
         torch.Tensor or tuple<torch.Tensor>
     """
     xy = (coords[:, :2] + coords[:, 2:4]) / 2
     wh = coords[:, 2:4] - coords[:, :2]
 
     if cat:
-        return torch.cat((xy, wh), dim=1)
+        cat = torch.concatenate if isinstance(coords, torch.Tensor) else np.concatenate
+        return cat((xy, wh), axis=1)
     else:
-        return (*xy.split(1, 1), *wh.split(1, 1))
+        return (xy[:, 0:1], xy[:, 1:2], wh[:, 0:1], wh[:, 1:2])
```

### Comparing `lightnet-3.1.0/lightnet/util/_mask.py` & `lightnet-4.0.0/lightnet/util/_mask.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/util/_module.py` & `lightnet-4.0.0/lightnet/util/_module.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/util/_anchors.py` & `lightnet-4.0.0/lightnet/util/_anchors.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,23 @@
         """ YoloV3 Anchors for the MS COCO dataset. """
         return Anchors.from_darknet(
             (32, 16, 8),
             ((116, 90), (156, 198), (373, 326), (30, 61), (62, 45), (59, 119), (10, 13), (16, 30), (33, 23)),
             (0, 0, 0, 1, 1, 1, 2, 2, 2),
         )
 
+    @property
+    def YoloV4_COCO(cls):
+        """ YoloV4 Anchors for the MS COCO dataset. """
+        return Anchors.from_darknet(
+            (32, 16, 8),
+            ((142, 110), (192, 243), (459, 401), (36, 75), (76, 55), (72, 146), (12, 16), (19, 36), (40, 28)),
+            (0, 0, 0, 1, 1, 1, 2, 2, 2),
+        )
+
 
 class Anchors(metaclass=anchor_meta):
     """ This class allows to define anchors in a predictable way. |br|
     Darknet anchors are inconsistent, because they get specified differently depending on whether the model is multiscale or not:
 
     Single Scale
         The anchors are defined relative to the output feature map size. |br|
```

### Comparing `lightnet-3.1.0/lightnet/network/loss/_region_masked.py` & `lightnet-4.0.0/lightnet/network/loss/_region_masked.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,15 @@
 
         # Get target masks
         if str(ground_truth.dtypes['segmentation']) == 'geos':
             gt_mask = torch.from_numpy(np.stack(bb.util.get_rasterized(ground_truth, (mH, mW), rescale=mH/nH/self.network_stride))).to(dtype=torch.bool, device=device)
         else:
             gt_mask = torch.from_numpy(np.stack(ground_truth['segmentation'].tolist())).to(dtype=torch.bool, device=device)
             if (gt_mask.shape[-2] != mH) or (gt_mask.shape[-1] != mW):
-                gt_mask = torch.nn.functional.interpolate(gt_mask.float().unsqueeze(0), (mH, mW), mode='bilinear', align_corners=False).squeeze(0).gt(0.5)
+                gt_mask = torch.nn.functional.interpolate(gt_mask.float().unsqueeze(0), (mH, mW)).squeeze(0).gt(0.5)
 
         # Get relative target coordinates
         tcoord = torch.from_numpy(ground_truth[['x_top_left', 'y_top_left', 'width', 'height']].to_numpy(copy=True)).to(dtype=torch.float, device=device)
         tcoord /= self.network_stride * torch.tensor((nW, nH, nW, nH), device=device)
 
         # Select which masks to train on
         pos_mask = match_mask > 0
```

### Comparing `lightnet-3.1.0/lightnet/network/loss/_region_oriented.py` & `lightnet-4.0.0/lightnet/network/loss/_region_oriented.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/loss/_base.py` & `lightnet-4.0.0/lightnet/network/loss/_base.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/loss/_corner.py` & `lightnet-4.0.0/lightnet/network/loss/_corner.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/loss/_region.py` & `lightnet-4.0.0/lightnet/network/loss/_region.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,102 +10,137 @@
 from ._base import Loss, MultiScale
 
 __all__ = ['RegionLoss', 'MultiScaleRegionLoss']
 log = logging.getLogger(__name__)
 
 
 class RegionLoss(Loss):
-    """ Computes the region loss for anchor detection networks. |br|
+    """
+    Computes the region loss for anchor detection networks. |br|
     This loss is is meant to be used on the output of a :class:`~lightnet.network.head.DetectionAnchor` module,
     together with a brambox dataframe of target annotations.
 
     Args:
         num_classes (int): number of classes to detect
         anchors (ln.util.Anchors): single-scale list of anchor boxes
         network_stride (int): Downsampling factors of the network (most lightnet networks have a `stride` attribute)
         seen (optional, torch.Tensor): How many images the network has already been trained on; Default **0**
         coord_scale (optional, float): weight of bounding box coordinates; Default **1.0**
         noobject_scale (optional, float): weight of regions without target boxes; Default **1.0**
         object_scale (optional, float): weight of regions with target boxes; Default **5.0**
         class_scale (optional, float): weight of categorical predictions; Default **1.0**
         iou_thresh (optional, float): minimum iou between a predicted box and ground truth for them to be considered matching; Default **0.6**
         coord_prefill (optional, int): This parameter controls for how many training samples the network will prefill the target coordinates, biassing the network to predict the center at **.5,.5**; Default **12800**
+        class_smoothing (optional, float): TODO
+        coord_regression (optional, 'mse' | 'ciou'): TODO
+        coord_grid_offset (optional, float): TODO
     """
     VALUES = ('total', 'conf', 'coord', 'class')
     ENABLE_REDUCTION = True
 
     def __init__(
         self,
         num_classes,
         anchors,
         network_stride,
+        *,
         seen=0,
+        iou_ignore_thresh=0.6,
+        iou_merge_thresh=1,
         coord_scale=1.0,
-        noobject_scale=1.0,
+        coord_regression='mse',
+        coord_grid_sensitivity=1,
+        coord_prefill=0,
         object_scale=5.0,
+        noobject_scale=1.0,
         class_scale=1.0,
-        iou_thresh=0.6,
-        coord_prefill=12800,
+        class_smoothing=0,
+        iou_thresh=None,    # Deprecated
     ):
         super().__init__()
         self.num_classes = num_classes
         self.num_anchors = anchors.num_anchors
         self.anchors = anchors.as_output(network_stride)
         self.network_stride = network_stride
         self.register_buffer('seen', torch.tensor(seen))
+
+        self.iou_ignore_thresh = iou_ignore_thresh
+        self.iou_merge_thresh = iou_merge_thresh
         self.coord_scale = coord_scale
-        self.noobject_scale = noobject_scale
+        self.coord_regression = coord_regression.lower()
+        self.coord_grid_sensitivity = coord_grid_sensitivity
+        self.coord_prefill = coord_prefill
         self.object_scale = object_scale
+        self.noobject_scale = noobject_scale
         self.class_scale = class_scale
-        self.iou_thresh = iou_thresh
-        self.coord_prefill = coord_prefill
+        self.class_smoothing = class_smoothing
+
+        assert self.coord_regression in ('mse', 'ciou'), 'The `coord_regression` parameter should be mse or ciou'
+        if self.coord_regression == 'ciou' and self.coord_prefill > 0:
+            log.warn('It is not recommended to use `coord_prefill` together with the CIoU regression method')
+
+        if iou_thresh is not None:
+            import warnings
+            warnings.warn(
+                'The `iou_thresh` argument is deprecated for the `iou_ignore_thresh`',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            self.iou_ignore_thresh = iou_thresh
 
     @property
     def loss(self):
+        """
+        .. deprecated:: 2.0.0
+            |br| This "loss" attribute is deprecated in favor for "loss_total".
+        """
         import warnings
         warnings.warn(
             'The "loss" attribute is deprecated in favor for "loss_total"',
             category=DeprecationWarning,
             stacklevel=2,
         )
         return self.loss_total
 
     def extra_repr(self):
+        # TODO: Rework with new parameters
         anchors = ' '.join(f'[{a[0]:.5g}, {a[1]:.5g}]' for a in self.anchors)
         return (
-            f'classes={self.num_classes}, network_stride={self.network_stride}, IoU threshold={self.iou_thresh}, seen={self.seen.item()}\n'
+            f'classes={self.num_classes}, network_stride={self.network_stride}, IoU threshold={self.iou_ignore_thresh}, seen={self.seen.item()}\n'
             f'coord_scale={self.coord_scale}, object_scale={self.object_scale}, noobject_scale={self.noobject_scale}, class_scale={self.class_scale}\n'
             f'anchors={anchors}'
         )
 
     def forward(self, output, target, *, seen=None):
-        """ Compute Region loss.
+        """
+        Compute Region loss.
 
         Args:
             output (torch.autograd.Variable): Output from the network
             target (brambox annotation dataframe or torch.Tensor): Brambox annotations or tensor containing the annotation targets.
             seen (int, optional): How many images the network has already been trained on; Default **Add batch_size to previous seen value**
 
         Note:
-            If using a target tensor, it should have the dimensions `[num_batch, num_anno, 5]` and following format per image:
+            If using a target tensor, it should have the dimensions `[num_batch, num_anno, 5]`
+            and have its coordinates relative to the image size (x divided by width, y divided by height).
+            Since the annotations from all images of a batch should be made of the same length, you can pad them with: `[-1, 0, 0, 0, 0]`.
+
+            More specifically, this is what the tensor should look like for one image:
 
             .. math::
 
                 \\begin{bmatrix}
                     class\\_idx & x\\_center & y\\_center & width & height \\\\
                     class\\_idx & x\\_center & y\\_center & width & height \\\\
                     ... \\\\
                     -1 & 0 & 0 & 0 & 0 \\\\
                     -1 & 0 & 0 & 0 & 0 \\\\
                     ...
                 \\end{bmatrix}
 
-            With all coordinates being relative to the image size. |br|
-            Since the annotations from all images of a batch should be made of the same length, you can pad them with: `[-1, 0, 0, 0, 0]`.
-
         Note:
             Besides being easier to work with, brambox dataframes have the added benefit that
             this loss function will also consider the ``ignore`` flag of annotations and ignore detections that match with it.
             This allows you to have annotations that will not influence the loss in any way,
             as opposed to having them removed and counting them as false detections.
         """
         # Parameters
@@ -118,16 +153,16 @@
             self.seen = torch.tensor(seen)
         elif self.training:
             self.seen += nB
 
         # Get x,y,w,h,conf,cls
         output = output.view(nB, nA, -1, nPixels)
         coord = torch.empty_like(output[:, :, :4])
-        coord[:, :, :2] = output[:, :, :2].sigmoid()    # tx,ty
-        coord[:, :, 2:4] = output[:, :, 2:4]            # tw,th
+        coord[:, :, :2] = self.coord_grid_sensitivity * output[:, :, :2].sigmoid() - 0.5 * (self.coord_grid_sensitivity - 1)    # tx,ty
+        coord[:, :, 2:4] = output[:, :, 2:4]                                                                                    # tw,th
         conf = output[:, :, 4].sigmoid()
         if nC > 1:
             cls = output[:, :, 5:].transpose(-1, -2).reshape(-1, nC)
 
         with torch.no_grad():
             # Create prediction boxes
             pred_boxes = torch.FloatTensor(nB*nA*nPixels, 4)
@@ -148,15 +183,15 @@
             pred_boxes[:, 1] = (coord[:, :, 1].detach() + lin_y).view(-1)
             pred_boxes[:, 2] = (coord[:, :, 2].detach().clamp(max=max_w).exp() * anchor_w).view(-1)
             pred_boxes[:, 3] = (coord[:, :, 3].detach().clamp(max=max_h).exp() * anchor_h).view(-1)
             pred_boxes = pred_boxes.cpu()
 
             # Get target values
             coord_mask, conf_mask, cls_mask, tcoord, tconf, tcls = self.build_targets(pred_boxes, target, nB, nH, nW)
-            coord_mask = coord_mask.expand_as(tcoord).to(device).sqrt()
+            coord_mask = coord_mask.to(device).sqrt()
             conf_mask = conf_mask.to(device).sqrt()
             tcoord = tcoord.to(device)
             tconf = tconf.to(device)
             if nC > 1:
                 tcls[~cls_mask] = -100                  # -100: ignored index CEL
                 tcls = tcls.view(-1).long().to(device)
 
@@ -166,23 +201,43 @@
         else:
             self.loss_conf = torch.nn.functional.mse_loss(conf*conf_mask, tconf*conf_mask, reduction='none')
             self.loss_conf = self.loss_conf.sum(dim=tuple(range(1, self.loss_conf.ndim))) / 2
 
         # Coordinate loss
         if self.coord_scale == 0:
             self.loss_coord = torch.tensor([0.0] * nB, device=device)
+        elif self.coord_regression == 'ciou':
+            coord[:, :, 2] = coord[:, :, 2].clone().clamp(max=max_w).exp() * anchor_w
+            coord[:, :, 3] = coord[:, :, 3].clone().clamp(max=max_h).exp() * anchor_h
+
+            coord = coord.transpose(-1, -2)
+            tcoord = tcoord.transpose(-1, -2)
+            coord_mask = coord_mask.transpose(-1, -2)
+
+            ciou = torch.ones_like(coord_mask)
+            coord_mask = coord_mask > 0
+            coord_mask_exp = coord_mask.expand_as(coord)
+            ciou[coord_mask] = iou_cwh(coord[coord_mask_exp].reshape(-1, 4), tcoord[coord_mask_exp].reshape(-1, 4), pairwise=True, type=iou_cwh.Types.CIoU).squeeze()
+
+            self.loss_coord = self.coord_scale * (1 - ciou).sum(dim=tuple(range(1, ciou.ndim)))
         else:
+            with torch.no_grad():
+                coord_mask = coord_mask.expand_as(tcoord)
+                coord_wh = tcoord[:, :, 2:4, :] / self.anchors[:, :2].reshape(1, nA, 2, 1).to(device)
+                coord_wh[coord_wh > 0] = coord_wh[coord_wh > 0].log()
+                tcoord[:, :, 2:4, :] = coord_wh
+
             self.loss_coord = torch.nn.functional.mse_loss(coord*coord_mask, tcoord*coord_mask, reduction='none')
             self.loss_coord = self.coord_scale * self.loss_coord.sum(dim=tuple(range(1, self.loss_coord.ndim))) / 2
 
         # Class loss
         if self.class_scale == 0 or nC == 1 or tcls.numel() == 0:
             self.loss_class = torch.tensor([0.0] * nB, device=device)
         else:
-            self.loss_class = torch.nn.functional.cross_entropy(cls, tcls, reduction='none')
+            self.loss_class = torch.nn.functional.cross_entropy(cls, tcls, reduction='none', ignore_index=-100, label_smoothing=self.class_smoothing)
             self.loss_class = self.loss_class.view(nB, -1)
             self.loss_class = self.class_scale * self.loss_class.sum(dim=tuple(range(1, self.loss_class.ndim)))
 
         # Total loss
         self.loss_total = self.loss_conf + self.loss_coord + self.loss_class
         return self.loss_total
 
@@ -193,14 +248,15 @@
         elif pd is not None and isinstance(ground_truth, pd.DataFrame):
             return self.__build_targets_brambox(pred_boxes, ground_truth, nB, nH, nW)
         else:
             raise TypeError(f'Unkown ground truth format [{type(ground_truth)}]')
 
     def __build_targets_tensor(self, pred_boxes, ground_truth, nB, nH, nW):
         """ Compare prediction boxes and ground truths, convert ground truths to network output tensors """
+        # TODO : Deprecate this ?
         # Parameters
         nA = self.num_anchors
         nAnchors = nA*nH*nW
         nPixels = nH*nW
 
         # Tensors
         coord_mask = torch.zeros(nB, nA, nH, nW, requires_grad=False)
@@ -225,15 +281,15 @@
             cur_pred_boxes = pred_boxes[b*nAnchors:(b+1)*nAnchors]
             gt = gt[:, 1:]
             gt[:, ::2] *= nW
             gt[:, 1::2] *= nH
 
             # Set confidence mask of matching detections to 0
             iou_gt_pred = iou_cwh(gt, cur_pred_boxes)
-            mask = (iou_gt_pred > self.iou_thresh).sum(0) >= 1
+            mask = (iou_gt_pred > self.iou_ignore_thresh).any(0)
             conf_mask[b][mask.view_as(conf_mask[b])] = 0
 
             # Find best anchor for each gt
             iou_gt_anchors = iou_wh(gt[:, 2:], self.anchors)
             _, best_anchors = iou_gt_anchors.max(1)
 
             # Set masks and target values for each gt
@@ -242,15 +298,15 @@
             gj = gt[:, 1].clamp(0, nH-1).long()
 
             conf_mask[b, best_anchors, gj, gi] = self.object_scale
             tconf[b, best_anchors, gj, gi] = iou_gt_pred.view(nGT, nA, nH, nW)[torch.arange(nGT), best_anchors, gj, gi]
             coord_mask[b, best_anchors, gj, gi] = 2 - torch.clamp(gt[:, 2] * gt[:, 3] / nPixels, max=1.5)
             tcoord[b, best_anchors, 0, gj, gi] = gt[:, 0] - gi.float()
             tcoord[b, best_anchors, 1, gj, gi] = gt[:, 1] - gj.float()
-            tcoord[b, best_anchors, 2:4, gj, gi] = (gt[:, 2:4] / self.anchors[best_anchors, 0:2]).log()
+            tcoord[b, best_anchors, 2:4, gj, gi] = gt[:, 2:4]
             cls_mask[b, best_anchors, gj, gi] = 1
             tcls[b, best_anchors, gj, gi] = ground_truth[b, torch.arange(nGT), 0]
 
         return (
             coord_mask.view(nB, nA, 1, nPixels),
             conf_mask.view(nB, nA, nPixels),
             cls_mask.view(nB, nA, nPixels),
@@ -280,45 +336,73 @@
             tcoord[:, :, 1].fill_(0.5)
 
         # Loop over GT
         for b, gt_filtered in ground_truth.groupby('batch_number', sort=False):
             cur_pred_boxes = pred_boxes[b*nAnchors:(b+1)*nAnchors]
 
             # Create ground_truth tensor
-            gt = torch.from_numpy(
-                gt_filtered[['x_top_left', 'y_top_left', 'width', 'height']].to_numpy(copy=True),
-            ).float()
+            gt = torch.from_numpy(gt_filtered[['x_top_left', 'y_top_left', 'width', 'height']].to_numpy(copy=True)).float()
+            nGT = gt.shape[0]
 
             # Convert from topleft -> center
             gt[:, 0] += gt[:, 2] / 2
             gt[:, 1] += gt[:, 3] / 2
 
             # Divide coordinates by stride
             gt[:, :4] /= self.network_stride
 
-            # Set confidence mask of matching detections to 0
+            # Get grid cell coordinate
+            gi = gt[:, 0].clamp(0, nW-1).long()
+            gj = gt[:, 1].clamp(0, nH-1).long()
+
+            # Compute IoU between GT and predictions
             iou_gt_pred = iou_cwh(gt, cur_pred_boxes)
-            mask = (iou_gt_pred > self.iou_thresh).sum(0) >= 1
-            conf_mask[b][mask.view_as(conf_mask[b])] = 0
+
+            # Set mask and target values for each matching detection (iou_merge_thresh)
+            match_iou, match_gt = iou_gt_pred.max(0)
+            mask = match_iou > self.iou_merge_thresh
+            if gt_filtered.ignore.any():
+                ignore_mask = torch.from_numpy(gt_filtered.ignore.values)
+                mask &= torch.isin(match_gt, ignore_mask.nonzero(), invert=True)
+
+            if mask.any():
+                mask = mask.nonzero().flatten()
+                anchor_match = mask // nPixels
+                gi_match = (mask % nPixels) % nW
+                gj_match = (mask % nPixels) // nW
+                gt_match_idx = match_gt[mask]
+                gt_match = gt[gt_match_idx]
+
+                conf_mask[b, anchor_match, gj_match, gi_match] = 1
+                tconf[b, anchor_match, gj_match, gi_match] = iou_gt_pred.view(nGT, nA, nH, nW)[gt_match_idx, anchor_match, gj_match, gi_match]
+                coord_mask[b, anchor_match, gj_match, gi_match] = 2 - torch.clamp(gt_match[:, 2] * gt_match[:, 3] / nPixels, max=1.5)
+                tcoord[b, anchor_match, 0, gj_match, gi_match] = gt_match[:, 0] - gi_match.float()
+                tcoord[b, anchor_match, 1, gj_match, gi_match] = gt_match[:, 1] - gj_match.float()
+                tcoord[b, anchor_match, 2:4, gj_match, gi_match] = gt_match[:, 2:4]
+                cls_mask[b, anchor_match, gj_match, gi_match] = 1
+                tcls[b, anchor_match, gj_match, gi_match] = torch.from_numpy(gt_filtered.class_id.values)[gt_match_idx].float()
+
+            # Set masks of matching detections to 0 (iou_ignore_thresh)
+            mask = (iou_gt_pred > self.iou_ignore_thresh).any(dim=0)
+            mask = mask.view_as(conf_mask[b])
+            conf_mask[b, mask] = 0
+            # coord_mask[b, mask] = 0
+            # cls_mask[b, mask] = 0
 
             # Find best anchor for each gt
             iou_gt_anchors = iou_wh(gt[:, 2:], self.anchors)
             _, best_anchors = iou_gt_anchors.max(1)
 
-            # Set masks and target values for each gt
-            nGT = gt.shape[0]
-            gi = gt[:, 0].clamp(0, nW-1).long()
-            gj = gt[:, 1].clamp(0, nH-1).long()
-
+            # Set masks and target values for each best matching (anchor, gt) pair
             conf_mask[b, best_anchors, gj, gi] = self.object_scale
             tconf[b, best_anchors, gj, gi] = iou_gt_pred.view(nGT, nA, nH, nW)[torch.arange(nGT), best_anchors, gj, gi]
             coord_mask[b, best_anchors, gj, gi] = 2 - torch.clamp(gt[:, 2] * gt[:, 3] / nPixels, max=1.5)
             tcoord[b, best_anchors, 0, gj, gi] = gt[:, 0] - gi.float()
             tcoord[b, best_anchors, 1, gj, gi] = gt[:, 1] - gj.float()
-            tcoord[b, best_anchors, 2:4, gj, gi] = (gt[:, 2:4] / self.anchors[best_anchors, 0:2]).log()
+            tcoord[b, best_anchors, 2:4, gj, gi] = gt[:, 2:4]
             cls_mask[b, best_anchors, gj, gi] = 1
             tcls[b, best_anchors, gj, gi] = torch.from_numpy(gt_filtered.class_id.values).float()
 
             # Set masks of ignored to zero
             if gt_filtered.ignore.any():
                 ignore_mask = torch.from_numpy(gt_filtered.ignore.values)
                 gi = gi[ignore_mask]
@@ -336,15 +420,16 @@
             tcoord.view(nB, nA, 4, nPixels),
             tconf.view(nB, nA, nPixels),
             tcls.view(nB, nA, nPixels),
         )
 
 
 class MultiScaleRegionLoss(MultiScale, RegionLoss):
-    """ Computes the region loss for multiscale anchor detection networks. |br|
+    """
+    Computes the region loss for multiscale anchor detection networks. |br|
     This class is is meant to be used on the output of multiple :class:`~lightnet.network.head.DetectionAnchor` modules,
     together with a brambox dataframe of target annotations.
 
     Args:
         num_classes (int): number of classes to detect
         anchors (ln.util.Anchors): multi-scale list of anchor boxes
         network_stride (list): Downsampling factors of the network (most lightnet networks have a `stride` attribute)
```

### Comparing `lightnet-3.1.0/lightnet/network/backbone/_mobilenet.py` & `lightnet-4.0.0/lightnet/network/backbone/_mobilenet.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,44 +8,45 @@
 from .._basemodule import BaseModule
 
 __all__ = ['Mobilenet']
 
 
 class Mobilenet(BaseModule):
     """ Mobilenet backbones. """
-    default_relu = partial(nn.ReLU6, inplace=True)
+    default_activation = partial(nn.ReLU6, inplace=True)
 
     @BaseModule.layers(named=True, primary=True)
     def V1(
         in_channels,
         out_channels,
         alpha=1,
         momentum=0.1,
-        relu=default_relu,
+        activation=default_activation,
+        relu=None,
     ):
         """
         Mobilenet V1 backbone.
 
         Args:
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
             alpha (float, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
             momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.1**
-            relu (class, optional): Which ReLU to use; Default :class:`torch.nn.ReLU6`
+            activation (class, optional): Which activation function to use; Default :class:`torch.nn.ReLU6`
 
         .. rubric:: Models:
 
         - :class:`~lightnet.models.MobilenetV1`
         - :class:`~lightnet.models.MobilenetYolo`
 
         Examples:
             >>> backbone = ln.network.backbone.Mobilenet.V1(3, 1024)
             >>> print(backbone)
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (2_convdw): Conv2dDepthWise(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU6(inplace=True))
               (3_convdw): Conv2dDepthWise(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (4_convdw): Conv2dDepthWise(128, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU6(inplace=True))
               (5_convdw): Conv2dDepthWise(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (6_convdw): Conv2dDepthWise(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU6(inplace=True))
               (7_convdw): Conv2dDepthWise(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (8_convdw): Conv2dDepthWise(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU6(inplace=True))
@@ -56,59 +57,72 @@
               (13_convdw): Conv2dDepthWise(512, 1024, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (14_convdw): Conv2dDepthWise(1024, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU6(inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 1024, 20, 20])
+
+        .. deprecated:: 4.0.0
+            |br| The `relu` argument is deprecated in favor for the more generic name "activation".
         """
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_convbatch', lnl.Conv2dBatchReLU(in_channels, int(alpha*32), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('2_convdw',    lnl.Conv2dDepthWise(int(alpha*32), int(alpha*64), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('3_convdw',    lnl.Conv2dDepthWise(int(alpha*64), int(alpha*128), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('4_convdw',    lnl.Conv2dDepthWise(int(alpha*128), int(alpha*128), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('5_convdw',    lnl.Conv2dDepthWise(int(alpha*128), int(alpha*256), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('6_convdw',    lnl.Conv2dDepthWise(int(alpha*256), int(alpha*256), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('7_convdw',    lnl.Conv2dDepthWise(int(alpha*256), int(alpha*512), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('8_convdw',    lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('9_convdw',    lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('10_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('11_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('12_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('13_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*1024), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('14_convdw',   lnl.Conv2dDepthWise(int(alpha*1024), out_channels, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('1_convbatch', lnl.Conv2dBatchAct(in_channels, int(alpha*32), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('2_convdw',    lnl.Conv2dDepthWise(int(alpha*32), int(alpha*64), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('3_convdw',    lnl.Conv2dDepthWise(int(alpha*64), int(alpha*128), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('4_convdw',    lnl.Conv2dDepthWise(int(alpha*128), int(alpha*128), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('5_convdw',    lnl.Conv2dDepthWise(int(alpha*128), int(alpha*256), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('6_convdw',    lnl.Conv2dDepthWise(int(alpha*256), int(alpha*256), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('7_convdw',    lnl.Conv2dDepthWise(int(alpha*256), int(alpha*512), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('8_convdw',    lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('9_convdw',    lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('10_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('11_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('12_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*512), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('13_convdw',   lnl.Conv2dDepthWise(int(alpha*512), int(alpha*1024), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('14_convdw',   lnl.Conv2dDepthWise(int(alpha*1024), out_channels, 3, 1, 1, activation=activation, momentum=momentum)),
         )
 
     @BaseModule.layers(named=True)
     def V2(
         in_channels,
         out_channels,
         alpha=1,
         momentum=0.1,
-        relu=default_relu,
+        activation=default_activation,
+        relu=None,
     ):
         """
         Mobilenet V2 backbone.
 
         Args:
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
             alpha (float, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
             momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.1**
-            relu (class, optional): Which ReLU to use; Default :class:`torch.nn.ReLU6`
+            activation (class, optional): Which activation function to use; Default :class:`torch.nn.ReLU6`
 
         .. rubric:: Models:
 
         - :class:`~lightnet.models.MobilenetV2`
 
         Examples:
             >>> backbone = ln.network.backbone.Mobilenet.V2(3, 1024)
             >>> print(backbone)
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU6(inplace=True))
               (2_bottleneck): InvertedBottleneck(32, 16, kernel_size=(3, 3), stride=(1, 1), expansion=1, ReLU6(inplace=True))
               (3_bottleneck): InvertedBottleneck(16, 24, kernel_size=(3, 3), stride=(2, 2), expansion=6, ReLU6(inplace=True))
               (4_bottleneck): InvertedBottleneck(24, 24, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (5_bottleneck): InvertedBottleneck(24, 32, kernel_size=(3, 3), stride=(2, 2), expansion=6, ReLU6(inplace=True))
               (6_bottleneck): InvertedBottleneck(32, 32, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (7_bottleneck): InvertedBottleneck(32, 32, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (8_bottleneck): InvertedBottleneck(32, 64, kernel_size=(3, 3), stride=(2, 2), expansion=6, ReLU6(inplace=True))
@@ -118,35 +132,47 @@
               (12_bottleneck): InvertedBottleneck(64, 96, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True))
               (13_bottleneck): InvertedBottleneck(96, 96, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (14_bottleneck): InvertedBottleneck(96, 96, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (15_bottleneck): InvertedBottleneck(96, 160, kernel_size=(3, 3), stride=(2, 2), expansion=6, ReLU6(inplace=True))
               (16_bottleneck): InvertedBottleneck(160, 160, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (17_bottleneck): InvertedBottleneck(160, 160, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True), residual_connection)
               (18_bottleneck): InvertedBottleneck(160, 320, kernel_size=(3, 3), stride=(1, 1), expansion=6, ReLU6(inplace=True))
-              (19_convbatch): Conv2dBatchReLU(320, 1024, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU6(inplace=True))
+              (19_convbatch): Conv2dBatchAct(320, 1024, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU6(inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 1024, 20, 20])
+
+        .. deprecated:: 4.0.0
+            |br| The `relu` argument is deprecated in favor for the more generic name "activation".
         """
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_convbatch',     lnl.Conv2dBatchReLU(in_channels, int(alpha*32), 3, 2, 1, relu=relu, momentum=momentum)),
-            ('2_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*16), 3, 1, 1, relu=relu, momentum=momentum)),
-            ('3_bottleneck',    lnl.InvertedBottleneck(int(alpha*16), int(alpha*24), 3, 2, 6, relu=relu, momentum=momentum)),
-            ('4_bottleneck',    lnl.InvertedBottleneck(int(alpha*24), int(alpha*24), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('5_bottleneck',    lnl.InvertedBottleneck(int(alpha*24), int(alpha*32), 3, 2, 6, relu=relu, momentum=momentum)),
-            ('6_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*32), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('7_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*32), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('8_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*64), 3, 2, 6, relu=relu, momentum=momentum)),
-            ('9_bottleneck',    lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('10_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('11_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('12_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*96), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('13_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*96), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('14_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*96), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('15_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*160), 3, 2, 6, relu=relu, momentum=momentum)),
-            ('16_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*160), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('17_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*160), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('18_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*320), 3, 1, 6, relu=relu, momentum=momentum)),
-            ('19_convbatch',    lnl.Conv2dBatchReLU(int(alpha*320), out_channels,  1, 1, 0, relu=relu, momentum=momentum)),
+            ('1_convbatch',     lnl.Conv2dBatchAct(in_channels, int(alpha*32), 3, 2, 1, activation=activation, momentum=momentum)),
+            ('2_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*16), 3, 1, 1, activation=activation, momentum=momentum)),
+            ('3_bottleneck',    lnl.InvertedBottleneck(int(alpha*16), int(alpha*24), 3, 2, 6, activation=activation, momentum=momentum)),
+            ('4_bottleneck',    lnl.InvertedBottleneck(int(alpha*24), int(alpha*24), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('5_bottleneck',    lnl.InvertedBottleneck(int(alpha*24), int(alpha*32), 3, 2, 6, activation=activation, momentum=momentum)),
+            ('6_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*32), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('7_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*32), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('8_bottleneck',    lnl.InvertedBottleneck(int(alpha*32), int(alpha*64), 3, 2, 6, activation=activation, momentum=momentum)),
+            ('9_bottleneck',    lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('10_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('11_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*64), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('12_bottleneck',   lnl.InvertedBottleneck(int(alpha*64), int(alpha*96), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('13_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*96), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('14_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*96), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('15_bottleneck',   lnl.InvertedBottleneck(int(alpha*96), int(alpha*160), 3, 2, 6, activation=activation, momentum=momentum)),
+            ('16_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*160), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('17_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*160), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('18_bottleneck',   lnl.InvertedBottleneck(int(alpha*160), int(alpha*320), 3, 1, 6, activation=activation, momentum=momentum)),
+            ('19_convbatch',    lnl.Conv2dBatchAct(int(alpha*320), out_channels,  1, 1, 0, activation=activation, momentum=momentum)),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/backbone/_darknet.py` & `lightnet-4.0.0/lightnet/network/backbone/_darknet.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,294 +8,330 @@
 from .._basemodule import BaseModule
 
 __all__ = ['Darknet']
 
 
 class Darknet(BaseModule):
     """ Darknet backbones. """
-    default_relu = partial(nn.LeakyReLU, 0.1, inplace=True)
+    default_activation = partial(nn.LeakyReLU, 0.1, inplace=True)
 
     @BaseModule.layers(named=True, primary=True)
-    def DN(in_channels, out_channels, momentum=0.01, relu=default_relu):
+    def DN(in_channels, out_channels, momentum=0.01, activation=default_activation, relu=None):
         """
         Base Darknet backbone.
 
         Args:
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
             momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.01**
-            relu (class, optional): Which ReLU to use; Default :class:`torch.nn.LeakyReLU(0.1)`
+            activation (class, optional): Which activation function to use; Default :class:`torch.nn.LeakyReLU(0.1)`
 
         .. rubric:: Models:
 
         - :class:`~lightnet.models.Darknet`
         - :class:`~lightnet.models.TinyYoloV2`
         - :class:`~lightnet.models.TinyYoloV3`
 
         Examples:
             >>> backbone = ln.network.backbone.Darknet(3, 512)
             >>> print(backbone)
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (2_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (3_convbatch): Conv2dBatchReLU(16, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (3_convbatch): Conv2dBatchAct(16, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (4_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (5_convbatch): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (5_convbatch): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (6_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (7_convbatch): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (7_convbatch): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (8_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (9_convbatch): Conv2dBatchReLU(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (9_convbatch): Conv2dBatchAct(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (10_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (11_convbatch): Conv2dBatchReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (11_convbatch): Conv2dBatchAct(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 512, 20, 20])
+
+        .. deprecated:: 4.0.0
+            |br| The `relu` argument is deprecated in favor for the more generic name "activation".
         """
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_convbatch',     lnl.Conv2dBatchReLU(in_channels, 16, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('1_convbatch',     lnl.Conv2dBatchAct(in_channels, 16, 3, 1, 1, activation=activation, momentum=momentum)),
             ('2_max',           nn.MaxPool2d(2, 2)),
-            ('3_convbatch',     lnl.Conv2dBatchReLU(16, 32, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('3_convbatch',     lnl.Conv2dBatchAct(16, 32, 3, 1, 1, activation=activation, momentum=momentum)),
             ('4_max',           nn.MaxPool2d(2, 2)),
-            ('5_convbatch',     lnl.Conv2dBatchReLU(32, 64, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('5_convbatch',     lnl.Conv2dBatchAct(32, 64, 3, 1, 1, activation=activation, momentum=momentum)),
             ('6_max',           nn.MaxPool2d(2, 2)),
-            ('7_convbatch',     lnl.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('7_convbatch',     lnl.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum)),
             ('8_max',           nn.MaxPool2d(2, 2)),
-            ('9_convbatch',     lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('9_convbatch',     lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum)),
             ('10_max',          nn.MaxPool2d(2, 2)),
-            ('11_convbatch',    lnl.Conv2dBatchReLU(256, out_channels, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('11_convbatch',    lnl.Conv2dBatchAct(256, out_channels, 3, 1, 1, activation=activation, momentum=momentum)),
         )
 
     @BaseModule.layers(named=True)
-    def DN_19(in_channels, out_channels, momentum=0.01, relu=default_relu):
+    def DN_19(in_channels, out_channels, momentum=0.01, activation=default_activation, relu=None):
         """
         Darknet19 backbone.
 
         Args:
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
             momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.01**
-            relu (class, optional): Which ReLU to use; Default :class:`torch.nn.LeakyReLU(0.1)`
+            activation (class, optional): Which activation function to use; Default :class:`torch.nn.LeakyReLU(0.1)`
 
         .. rubric:: Models:
 
         - :class:`~lightnet.models.Darknet19`
         - :class:`~lightnet.models.DYolo`
         - :class:`~lightnet.models.YoloV2`
         - :class:`~lightnet.models.YoloV2Upsample`
         - :class:`~lightnet.models.Yolt`
 
         Examples:
             >>> backbone = ln.network.backbone.Darknet.DN_19(3, 1024)
             >>> print(backbone)
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (2_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (3_convbatch): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (3_convbatch): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (4_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (5_convbatch): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (6_convbatch): Conv2dBatchReLU(128, 64, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (7_convbatch): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (5_convbatch): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (6_convbatch): Conv2dBatchAct(128, 64, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (7_convbatch): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (8_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (9_convbatch): Conv2dBatchReLU(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (10_convbatch): Conv2dBatchReLU(256, 128, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (11_convbatch): Conv2dBatchReLU(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (9_convbatch): Conv2dBatchAct(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (10_convbatch): Conv2dBatchAct(256, 128, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (11_convbatch): Conv2dBatchAct(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (12_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (13_convbatch): Conv2dBatchReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (14_convbatch): Conv2dBatchReLU(512, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (15_convbatch): Conv2dBatchReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (16_convbatch): Conv2dBatchReLU(512, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (17_convbatch): Conv2dBatchReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (13_convbatch): Conv2dBatchAct(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (14_convbatch): Conv2dBatchAct(512, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (15_convbatch): Conv2dBatchAct(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (16_convbatch): Conv2dBatchAct(512, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (17_convbatch): Conv2dBatchAct(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (18_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              (19_convbatch): Conv2dBatchReLU(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (20_convbatch): Conv2dBatchReLU(1024, 512, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (21_convbatch): Conv2dBatchReLU(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (22_convbatch): Conv2dBatchReLU(1024, 512, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
-              (23_convbatch): Conv2dBatchReLU(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (19_convbatch): Conv2dBatchAct(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (20_convbatch): Conv2dBatchAct(1024, 512, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (21_convbatch): Conv2dBatchAct(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (22_convbatch): Conv2dBatchAct(1024, 512, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), LeakyReLU(negative_slope=0.1, inplace=True))
+              (23_convbatch): Conv2dBatchAct(512, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 1024, 20, 20])
+
+        .. deprecated:: 4.0.0
+            |br| The `relu` argument is deprecated in favor for the more generic name "activation".
         """
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_convbatch',     lnl.Conv2dBatchReLU(in_channels, 32, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('1_convbatch',     lnl.Conv2dBatchAct(in_channels, 32, 3, 1, 1, activation=activation, momentum=momentum)),
             ('2_max',           nn.MaxPool2d(2, 2)),
-            ('3_convbatch',     lnl.Conv2dBatchReLU(32, 64, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('3_convbatch',     lnl.Conv2dBatchAct(32, 64, 3, 1, 1, activation=activation, momentum=momentum)),
             ('4_max',           nn.MaxPool2d(2, 2)),
-            ('5_convbatch',     lnl.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('6_convbatch',     lnl.Conv2dBatchReLU(128, 64, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('7_convbatch',     lnl.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('5_convbatch',     lnl.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('6_convbatch',     lnl.Conv2dBatchAct(128, 64, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('7_convbatch',     lnl.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum)),
             ('8_max',           nn.MaxPool2d(2, 2)),
-            ('9_convbatch',     lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('10_convbatch',    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('11_convbatch',    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('9_convbatch',     lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('10_convbatch',    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('11_convbatch',    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum)),
             ('12_max',          nn.MaxPool2d(2, 2)),
-            ('13_convbatch',    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('14_convbatch',    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('15_convbatch',    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('16_convbatch',    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('17_convbatch',    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('13_convbatch',    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('14_convbatch',    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('15_convbatch',    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('16_convbatch',    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('17_convbatch',    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
             ('18_max',          nn.MaxPool2d(2, 2)),
-            ('19_convbatch',    lnl.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('20_convbatch',    lnl.Conv2dBatchReLU(1024, 512, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('21_convbatch',    lnl.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('22_convbatch',    lnl.Conv2dBatchReLU(1024, 512, 1, 1, 0, relu=relu, momentum=momentum)),
-            ('23_convbatch',    lnl.Conv2dBatchReLU(512, out_channels, 3, 1, 1, relu=relu, momentum=momentum)),
+            ('19_convbatch',    lnl.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('20_convbatch',    lnl.Conv2dBatchAct(1024, 512, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('21_convbatch',    lnl.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('22_convbatch',    lnl.Conv2dBatchAct(1024, 512, 1, 1, 0, activation=activation, momentum=momentum)),
+            ('23_convbatch',    lnl.Conv2dBatchAct(512, out_channels, 3, 1, 1, activation=activation, momentum=momentum)),
         )
 
     @BaseModule.layers(named=True)
-    def DN_53(in_channels, out_channels, momentum=0.01, relu=default_relu):
+    def DN_53(in_channels, out_channels, momentum=0.01, activation=default_activation, relu=None):
         """
         Darknet53 backbone.
 
         Args:
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
             momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.01**
-            relu (class, optional): Which ReLU to use; Default :class:`torch.nn.LeakyReLU(0.1)`
+            activation (class, optional): Which activation function to use; Default :class:`torch.nn.LeakyReLU(0.1)`
 
         .. rubric:: Models:
 
         - :class:`~lightnet.models.Darknet53`
         - :class:`~lightnet.models.YoloV3`
 
         Examples:
             >>> backbone = ln.network.backbone.Darknet.DN_53(3, 1024)
             >>> print(backbone)     # doctest: +SKIP
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
-              (2_convbatch): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (2_convbatch): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (3_residual): Residual(...)
-              (4_convbatch): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (4_convbatch): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (5_residual): Residual(...)
               (6_residual): Residual(...)
-              (7_convbatch): Conv2dBatchReLU(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (7_convbatch): Conv2dBatchAct(128, 256, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (8_residual): Residual(...)
               (9_residual): Residual(...)
               (10_residual): Residual(...)
               (11_residual): Residual(...)
               (12_residual): Residual(...)
               (13_residual): Residual(...)
               (14_residual): Residual(...)
               (15_residual): Residual(...)
-              (16_convbatch): Conv2dBatchReLU(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (16_convbatch): Conv2dBatchAct(256, 512, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (17_residual): Residual(...)
               (18_residual): Residual(...)
               (19_residual): Residual(...)
               (20_residual): Residual(...)
               (21_residual): Residual(...)
               (22_residual): Residual(...)
               (23_residual): Residual(...)
               (24_residual): Residual(...)
-              (25_convbatch): Conv2dBatchReLU(512, 1024, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+              (25_convbatch): Conv2dBatchAct(512, 1024, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
               (26_residual): Residual(...)
               (27_residual): Residual(...)
               (28_residual): Residual(...)
               (29_residual): Residual(...)
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 1024, 20, 20])
+
+        .. deprecated:: 4.0.0
+            |br| The `relu` argument is deprecated in favor for the more generic name "activation".
         """
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_convbatch',         lnl.Conv2dBatchReLU(in_channels, 32, 3, 1, 1, relu=relu, momentum=momentum)),
-            ('2_convbatch',         lnl.Conv2dBatchReLU(32, 64, 3, 2, 1, relu=relu, momentum=momentum)),
+            ('1_convbatch',         lnl.Conv2dBatchAct(in_channels, 32, 3, 1, 1, activation=activation, momentum=momentum)),
+            ('2_convbatch',         lnl.Conv2dBatchAct(32, 64, 3, 2, 1, activation=activation, momentum=momentum)),
             ('3_residual',          lnl.Residual(
-                                    lnl.Conv2dBatchReLU(64, 32, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(32, 64, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(64, 32, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(32, 64, 3, 1, 1, activation=activation, momentum=momentum),
             )),
-            ('4_convbatch',         lnl.Conv2dBatchReLU(64, 128, 3, 2, 1, relu=relu, momentum=momentum)),
+            ('4_convbatch',         lnl.Conv2dBatchAct(64, 128, 3, 2, 1, activation=activation, momentum=momentum)),
             ('5_residual',          lnl.Residual(
-                                    lnl.Conv2dBatchReLU(128, 64, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 64, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('6_residual',          lnl.Residual(
-                                    lnl.Conv2dBatchReLU(128, 64, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 64, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum),
             )),
-            ('7_convbatch',         lnl.Conv2dBatchReLU(128, 256, 3, 2, 1, relu=relu, momentum=momentum)),
+            ('7_convbatch',         lnl.Conv2dBatchAct(128, 256, 3, 2, 1, activation=activation, momentum=momentum)),
             ('8_residual',          lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('9_residual',          lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('10_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('11_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('12_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('13_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('14_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('15_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum),
             )),
-            ('16_convbatch',        lnl.Conv2dBatchReLU(256, 512, 3, 2, 1, relu=relu, momentum=momentum)),
+            ('16_convbatch',        lnl.Conv2dBatchAct(256, 512, 3, 2, 1, activation=activation, momentum=momentum)),
             ('17_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('18_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('19_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('20_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('21_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('22_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('23_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('24_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum),
             )),
-            ('25_convbatch',        lnl.Conv2dBatchReLU(512, out_channels, 3, 2, 1, relu=relu, momentum=momentum)),
+            ('25_convbatch',        lnl.Conv2dBatchAct(512, out_channels, 3, 2, 1, activation=activation, momentum=momentum)),
             ('26_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(out_channels, 512, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(512, out_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(out_channels, 512, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, out_channels, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('27_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(out_channels, 512, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(512, out_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(out_channels, 512, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, out_channels, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('28_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(out_channels, 512, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(512, out_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(out_channels, 512, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, out_channels, 3, 1, 1, activation=activation, momentum=momentum),
             )),
             ('29_residual',         lnl.Residual(
-                                    lnl.Conv2dBatchReLU(out_channels, 512, 1, 1, 0, relu=relu, momentum=momentum),
-                                    lnl.Conv2dBatchReLU(512, out_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                                    lnl.Conv2dBatchAct(out_channels, 512, 1, 1, 0, activation=activation, momentum=momentum),
+                                    lnl.Conv2dBatchAct(512, out_channels, 3, 1, 1, activation=activation, momentum=momentum),
             )),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/backbone/_cornernet.py` & `lightnet-4.0.0/lightnet/network/backbone/_cornernet.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,51 +28,51 @@
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
 
         Examples:
             >>> backbone = ln.network.backbone.Cornernet(3, 256)
             >>> print(backbone)     # doctest: +SKIP
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 128, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), ReLU(inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 128, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), ReLU(inplace=True))
               (2_residual): Residual(...)
               (para): ParallelSum(
                 (0): Sequential(
                   (3_hourglass): HourGlass(order=5, ...)
-                  (4_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                  (4_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                   (5_conv): Conv2d(256, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
                   (6_batchnorm): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 )
                 (1): Sequential(
                   (7_conv): Conv2d(256, 256, kernel_size=(1, 1), stride=(1, 1), bias=False)
                   (8_batchnorm): BatchNorm2d(256, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
                 )
                 (post): ReLU(inplace=True)
               )
               (9_residual): Residual(...)
               (10_hourglass): HourGlass(order=5, ...)
-              (11_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+              (11_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 256, 160, 160])
         """
         return (
-            ('1_convbatch',         lnl.Conv2dBatchReLU(in_channels, 128, 7, 2, 3)),
+            ('1_convbatch',         lnl.Conv2dBatchAct(in_channels, 128, 7, 2, 3)),
             ('2_residual',          cls.get_residual(128, 256, stride=2)),
             ('residual',            lnl.Residual(OrderedDict([
                 ('3_hourglass',     cls.get_hourglass(cls.get_residual)),
-                ('4_convbatch',     lnl.Conv2dBatchReLU(256, 256, 3, 1, 1)),
+                ('4_convbatch',     lnl.Conv2dBatchAct(256, 256, 3, 1, 1)),
                 ('5_convbatch',     lnl.Conv2dBatch(256, 256, 1, 1, 0)),
                 ('skip',            lnl.Conv2dBatch(256, 256, 1, 1, 0)),
                 ('post',            nn.ReLU(inplace=True)),
             ]))),
             ('6_residual',          cls.get_residual(256, 256)),
             ('7_hourglass',         cls.get_hourglass(cls.get_residual)),
-            ('8_convbatch',         lnl.Conv2dBatchReLU(256, out_channels, 3, 1, 1)),
+            ('8_convbatch',         lnl.Conv2dBatchAct(256, out_channels, 3, 1, 1)),
         )
 
     @BaseModule.layers(named=True, classmethod=True)
     def Squeeze(cls, in_channels, out_channels):
         """
         Cornernet Squeeze backbone.
 
@@ -80,47 +80,47 @@
             in_channels (int): Number of input channels
             out_channels (int): Number of output channels
 
         Examples:
             >>> backbone = ln.network.backbone.Cornernet.Squeeze(3, 256)
             >>> print(backbone)     # doctest: +SKIP
             Sequential(
-              (1_convbatch): Conv2dBatchReLU(3, 128, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), ReLU(inplace=True))
+              (1_convbatch): Conv2dBatchAct(3, 128, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), ReLU(inplace=True))
               (2_residual): Residual(...)
               (3_residual): Residual(...)
               (residual): Residual(
                 (4_hourglass): HourGlass(order=4, ...)
-                (5_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (5_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (6_convbatch): Conv2dBatch(256, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0))
                 (skip): Conv2dBatch(256, 256, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0))
                 (post): ReLU(inplace=True)
               )
               (7_residual): Residual(...)
               (8_hourglass): HourGlass(order=4, ...)
-              (9_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+              (9_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             )
             >>> in_tensor = torch.rand(1, 3, 640, 640)
             >>> out_tensor = backbone(in_tensor)
             >>> print(out_tensor.shape)
             torch.Size([1, 256, 80, 80])
         """
         return (
-            ('1_convbatch',         lnl.Conv2dBatchReLU(in_channels, 128, 7, 2, 3)),
+            ('1_convbatch',         lnl.Conv2dBatchAct(in_channels, 128, 7, 2, 3)),
             ('2_residual',          cls.get_residual(128, 256, stride=2)),
             ('3_residual',          cls.get_residual(256, 256, stride=2)),
             ('residual',            lnl.Residual(OrderedDict([
                 ('4_hourglass',     cls.get_hourglass_squeeze(cls.get_fire)),
-                ('5_convbatch',     lnl.Conv2dBatchReLU(256, 256, 3, 1, 1)),
+                ('5_convbatch',     lnl.Conv2dBatchAct(256, 256, 3, 1, 1)),
                 ('6_convbatch',     lnl.Conv2dBatch(256, 256, 1, 1, 0)),
                 ('skip',            lnl.Conv2dBatch(256, 256, 1, 1, 0)),
                 ('post',            nn.ReLU(inplace=True)),
             ]))),
             ('7_residual',          cls.get_residual(256, 256)),
             ('8_hourglass',         cls.get_hourglass_squeeze(cls.get_fire)),
-            ('9_convbatch',         lnl.Conv2dBatchReLU(256, out_channels, 3, 1, 1)),
+            ('9_convbatch',         lnl.Conv2dBatchAct(256, out_channels, 3, 1, 1)),
         )
 
     @staticmethod
     def get_residual(in_channels, out_channels, kernel=3, stride=1, padding=1):
         return lnl.Residual(
             nn.Conv2d(in_channels, out_channels, kernel, stride, padding, bias=False),
             nn.BatchNorm2d(out_channels),
```

### Comparing `lightnet-3.1.0/lightnet/network/backbone/_alexnet.py` & `lightnet-4.0.0/lightnet/network/backbone/_alexnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,50 +7,63 @@
 from .. import layer as lnl
 from .._basemodule import BaseModule
 
 __all__ = ['Alexnet']
 
 
 class Alexnet(BaseModule):
-    """ Alexnet backbone.
+    """
+    Alexnet backbone.
 
     Args:
         in_channels (int): Number of input channels
         out_channels (int): Number of output channels
-        relu (class, optional): Which ReLU to use; Default :class:`torch.nn.ReLU`
+        activation (class, optional): Which activation function to use; Default :class:`torch.nn.ReLU`
 
     .. rubric:: Models:
 
     - :class:`~lightnet.models.Alexnet`
 
     Examples:
         >>> backbone = ln.network.backbone.Alexnet(3, 256)
         >>> print(backbone)
         Sequential(
-          (1_conv): Conv2dReLU(3, 64, kernel_size=(11, 11), stride=(4, 4), padding=(2, 2), ReLU(inplace=True))
+          (1_conv): Conv2dAct(3, 64, kernel_size=(11, 11), stride=(4, 4), padding=(2, 2), ReLU(inplace=True))
           (2_max): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False)
-          (3_conv): Conv2dReLU(64, 192, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2), ReLU(inplace=True))
+          (3_conv): Conv2dAct(64, 192, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2), ReLU(inplace=True))
           (4_max): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False)
-          (5_conv): Conv2dReLU(192, 384, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (6_conv): Conv2dReLU(384, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (7_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (5_conv): Conv2dAct(192, 384, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (6_conv): Conv2dAct(384, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (7_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (8_max): MaxPool2d(kernel_size=3, stride=2, padding=0, dilation=1, ceil_mode=False)
         )
         >>> in_tensor = torch.rand(1, 3, 640, 640)
         >>> out_tensor = backbone(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 256, 19, 19])
+
+    .. deprecated:: 4.0.0
+        |br| The `relu` argument is deprecated in favor for the more generic name "activation".
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
     @BaseModule.layers(named=True)
-    def Default(in_channels, out_channels, relu=default_relu):
+    def Default(in_channels, out_channels, activation=default_activation, relu=None):
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         return (
-            ('1_conv',  lnl.Conv2dReLU(in_channels, 64, 11, 4, 2, bias=True, relu=relu)),
+            ('1_conv',  lnl.Conv2dAct(in_channels, 64, 11, 4, 2, bias=True, activation=activation)),
             ('2_max',   nn.MaxPool2d(3, 2)),
-            ('3_conv',  lnl.Conv2dReLU(64, 192, 5, 1, 2, bias=True, relu=relu)),
+            ('3_conv',  lnl.Conv2dAct(64, 192, 5, 1, 2, bias=True, activation=activation)),
             ('4_max',   nn.MaxPool2d(3, 2)),
-            ('5_conv',  lnl.Conv2dReLU(192, 384, 3, 1, 1, bias=True, relu=relu)),
-            ('6_conv',  lnl.Conv2dReLU(384, 256, 3, 1, 1, bias=True, relu=relu)),
-            ('7_conv',  lnl.Conv2dReLU(256, out_channels, 3, 1, 1, bias=True, relu=relu)),
+            ('5_conv',  lnl.Conv2dAct(192, 384, 3, 1, 1, bias=True, activation=activation)),
+            ('6_conv',  lnl.Conv2dAct(384, 256, 3, 1, 1, bias=True, activation=activation)),
+            ('7_conv',  lnl.Conv2dAct(256, out_channels, 3, 1, 1, bias=True, activation=activation)),
             ('8_max',   nn.MaxPool2d(3, 2)),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_mobilenet.py` & `lightnet-4.0.0/lightnet/network/layer/_mobilenet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #
 #   Mobilenet related layers
 #   Copyright EAVISE
 #
+import logging
 from functools import partial
 import torch.nn as nn
 
 __all__ = ['Conv2dDepthWise', 'InvertedBottleneck']
+log = logging.getLogger(__name__)
 
 
 class Conv2dDepthWise(nn.Module):
     """ This layer implements the depthwise separable convolution :cite:`mobilenet_v1`. |br|
     Instead of performing a regular convolution,
     this layer first does a depthwise convolution, followed by a pointwise convolution.
     This reduces the number of computations, while maintaining a similar accuracy.
@@ -34,40 +36,52 @@
         >>> module = ln.network.layer.Conv2dDepthWise(3, 32, 3, 1, 1)
         >>> print(module)
         Conv2dDepthWise(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
+
+    .. deprecated:: 4.0.0
+        |br| The `relu` argument is deprecated in favor for the more generic name "activation".
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
-    def __init__(self, in_channels, out_channels, kernel_size, stride, padding, momentum=0.1, relu=default_relu):
+    def __init__(self, in_channels, out_channels, kernel_size, stride, padding, momentum=0.1, activation=default_activation, relu=None):
         super().__init__()
 
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         self.layers = nn.Sequential(
             nn.Conv2d(in_channels, in_channels, kernel_size, stride, padding, groups=in_channels, bias=False),
             nn.BatchNorm2d(in_channels, momentum=momentum),
-            relu(),
+            activation(),
 
             nn.Conv2d(in_channels, out_channels, 1, 1, 0, bias=False),
             nn.BatchNorm2d(out_channels, momentum=momentum),
-            relu(),
+            activation(),
         )
 
     def __repr__(self):
-        s = '{name}({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {relu})'
+        s = '{name}({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {activation})'
         return s.format(
             name=self.__class__.__name__,
             in_channels=self.layers[0].in_channels,
             out_channels=self.layers[3].out_channels,
             kernel_size=self.layers[0].kernel_size,
             stride=self.layers[0].stride,
             padding=self.layers[0].padding,
-            relu=self.layers[2],
+            activation=self.layers[2],
         )
 
     def forward(self, x):
         x = self.layers(x)
         return x
 
     @property
@@ -130,49 +144,61 @@
         >>> module = ln.network.layer.InvertedBottleneck(32, 32, 3, 1, 3)
         >>> print(module)
         InvertedBottleneck(32, 32, kernel_size=(3, 3), stride=(1, 1), expansion=3, ReLU(inplace=True), residual_connection)
         >>> in_tensor = torch.rand(1, 32, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
+
+    .. deprecated:: 4.0.0
+        |br| The `relu` argument is deprecated in favor for the more generic name "activation".
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
-    def __init__(self, in_channels, out_channels, kernel_size, stride, expansion, momentum=0.1, relu=default_relu):
+    def __init__(self, in_channels, out_channels, kernel_size, stride, expansion, momentum=0.1, activation=default_activation, relu=None):
         super().__init__()
 
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         # Parameters
         self.expansion = expansion
         self.residual_connect = stride == 1 and in_channels == out_channels
 
         # Layer
         self.layers = nn.Sequential(
             nn.Conv2d(in_channels, in_channels*expansion, 1, 1, 0, bias=False),
             nn.BatchNorm2d(in_channels*expansion, momentum=momentum),
-            relu(),
+            activation(),
 
             nn.Conv2d(in_channels*expansion, in_channels*expansion, kernel_size, stride, 1, groups=in_channels*expansion, bias=False),
             nn.BatchNorm2d(in_channels*expansion, momentum=momentum),
-            relu(),
+            activation(),
 
             nn.Conv2d(in_channels*expansion, out_channels, 1, 1, 0, bias=False),
             nn.BatchNorm2d(out_channels, momentum=momentum),
         )
 
     def __repr__(self):
         residual = ', residual_connection' if self.residual_connect else ''
-        s = '{name}({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, expansion={expansion}, {relu}{residual})'
+        s = '{name}({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, expansion={expansion}, {activation}{residual})'
         return s.format(
             name=self.__class__.__name__,
             in_channels=self.layers[0].in_channels,
             out_channels=self.layers[6].out_channels,
             kernel_size=self.layers[3].kernel_size,
             stride=self.layers[3].stride,
             expansion=self.expansion,
-            relu=self.layers[2],
+            activation=self.layers[2],
             residual=residual,
         )
 
     def forward(self, x):
         if self.residual_connect:
             return x + self.layers(x)
         else:
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_darknet.py` & `lightnet-4.0.0/lightnet/network/layer/_darknet.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/layer/_fusion.py` & `lightnet-4.0.0/lightnet/network/layer/_fusion.py`

 * *Files 16% similar despite different names*

```diff
@@ -60,71 +60,71 @@
         In :cite:`rgbd_fusion_v2`, we demonstrated that mid to late fusion gives the best results. |br|
         As such, we developed a new :class:`~lightnet.network.layer.FusionModule`, which can run any module (and not only Sequentials) and simply fuses the outputs of that module.
         While this new module does not offer the choice of fusion layer, it is much simpler to use and allows to perform N fusions instead of being limited to only two.
         Transforming eg. a backbone to a :class:`~lightnet.network.layer.FusionModule` is more or less equal to mid/late fusion and should thus yield optimal results.
 
     Example:
         >>> layers = [
-        ...   ln.network.layer.Conv2dBatchReLU(3,  32, 3, 1, 1),
-        ...   ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...   ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(3,  32, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
         ... ]
         >>> # Streams are fused in the middle of the module
         >>> module = ln.network.layer.FusionSequential(layers, fuse_layer=1)
         >>> print(module)
         FusionSequential(
           (Regular & Fusion): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
           (Fuse): Conv2d(64, 32, kernel_size=(1, 1), stride=(1, 1), bias=False)
           (Combined): Sequential(
-            (0): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
         )
         >>> # Streams are fused at the end of the module (after last convolution)
         >>> module = ln.network.layer.FusionSequential(layers, fuse_layer=3)
         >>> print(module)
         FusionSequential(
           (Regular & Fusion): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
           (Fuse): Conv2d(64, 32, kernel_size=(1, 1), stride=(1, 1), bias=False)
         )
         >>> # Streams are fused before the first layer
         >>> module = ln.network.layer.FusionSequential(layers, fuse_layer=0)
         >>> print(module)
         FusionSequential(
           (Fuse): Conv2d(6, 3, kernel_size=(1, 1), stride=(1, 1), bias=False)
           (Combined): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
         )
         >>> # Streams were fused before this module and thus there is no fusion involved (only combined sequential)
         >>> module = ln.network.layer.FusionSequential(layers, fuse_layer=None)
         >>> print(module)
         FusionSequential(
           (Combined): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
         )
         >>> # Streams are not fused in this module (duplicated regular and fusion sequentials)
         >>> module = ln.network.layer.FusionSequential(layers, fuse_layer=4)
         >>> print(module)
         FusionSequential(
           (Regular & Fusion): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
         )
     """
     def __init__(self, layers, fuse_layer=None):
         super().__init__()
 
         # Parameters
@@ -259,42 +259,31 @@
     Note:
         The ``input_shape`` argument is used during initialization in order to get the different outputs which come from the original module.
         This is then used to build correct fusion convolutions, which are used to combine the various outputs.
 
     Example:
         >>> # Perform data fusion on 3 different input types
         >>> layers = torch.nn.Sequential(
-        ...   ln.network.layer.Conv2dBatchReLU(3,  32, 3, 1, 1),
-        ...   ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...   ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(3,  32, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...   ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
         ... )
         >>> module = ln.network.layer.FusionModule(layers, (2, 2, 1), (1, 3, 416, 416))
         >>> print(module)
         FusionModule(
           in_channels=(2, 2, 1)
           (channel_conv): ModuleList(
-            (0): Conv2d(2, 3, kernel_size=(1, 1), stride=(1, 1))
-            (1): Conv2d(2, 3, kernel_size=(1, 1), stride=(1, 1))
+            (0-1): 2 x Conv2d(2, 3, kernel_size=(1, 1), stride=(1, 1))
             (2): Conv2d(1, 3, kernel_size=(1, 1), stride=(1, 1))
           )
           (fusion_module): ModuleList(
-            (0): Sequential(
-              (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            )
-            (1): Sequential(
-              (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            )
-            (2): Sequential(
-              (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-              (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0-2): 3 x Sequential(
+              (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+              (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+              (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             )
           )
           (fusion_conv): ModuleList(
             (0): Conv2d(96, 32, kernel_size=(1, 1), stride=(1, 1))
           )
         )
         >>> # Input should be a single tensor
@@ -311,54 +300,35 @@
         FusionModule(
           in_channels=(3, 1)
           (channel_conv): ModuleList(
             (0): Conv2d(3, 3, kernel_size=(1, 1), stride=(1, 1))
             (1): Conv2d(1, 3, kernel_size=(1, 1), stride=(1, 1))
           )
           (fusion_module): ModuleList(
-            (0): FeatureExtractor(
-              selection=[8_conv], return=True
-              (module): Sequential(
-                (1_conv): Conv2dReLU(3, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (2_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (3_conv): Conv2dReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (4_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (5_conv): Conv2dReLU(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (6_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (7_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (8_conv): Conv2dReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (9_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (10_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (11_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (12_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (13_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-              )
-            )
-            (1): FeatureExtractor(
+            (0-1): 2 x FeatureExtractor(
               selection=[8_conv], return=True
               (module): Sequential(
-                (1_conv): Conv2dReLU(3, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (1_conv): Conv2dAct(3, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (2_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (3_conv): Conv2dReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (3_conv): Conv2dAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (4_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (5_conv): Conv2dReLU(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (6_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (5_conv): Conv2dAct(128, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (6_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (7_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (8_conv): Conv2dReLU(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (9_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (8_conv): Conv2dAct(256, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (9_conv): Conv2dAct(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (10_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-                (11_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (12_conv): Conv2dReLU(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (11_conv): Conv2dAct(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (12_conv): Conv2dAct(512, 512, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (13_max): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
               )
             )
           )
           (fusion_conv): ModuleList(
-            (0): Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1))
-            (1): Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1))
+            (0-1): 2 x Conv2d(1024, 512, kernel_size=(1, 1), stride=(1, 1))
           )
         )
         >>> input_tensor = torch.rand(1, 4, 96, 96)
         >>> output_tensors = module(input_tensor)
         >>> print([o.shape for o in output_tensors])
         [torch.Size([1, 512, 3, 3]), torch.Size([1, 512, 12, 12])]
     """
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_deform.py` & `lightnet-4.0.0/lightnet/network/layer/_deform.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/layer/_conv.py` & `lightnet-4.0.0/lightnet/network/layer/_conv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #
 #   Convolutional layers
 #   Copyright EAVISE
 #
 from functools import partial
 import torch.nn as nn
 
-__all__ = ['Conv2dBatch', 'Conv2dBatchReLU', 'Conv2dReLU']
+__all__ = ['Conv2dBatch', 'Conv2dBatchAct', 'Conv2dAct', 'Conv2dBatchReLU', 'Conv2dReLU']
 
 
 class Conv2dBatch(nn.Module):
-    """ This convenience layer groups a 2D convolution and a batchnorm.
+    """
+    This convenience layer groups a 2D convolution and a batchnorm.
     They are executed in a sequential manner.
 
     Args:
         in_channels (int): Number of input channels
         out_channels (int): Number of output channels
         kernel_size (int or tuple): Size of the kernel of the convolution
         stride (int or tuple): Stride of the convolution
@@ -81,169 +82,219 @@
         return self.layers[0].in_channels
 
     @property
     def out_channels(self):
         return self.layers[0].out_channels
 
 
-class Conv2dBatchReLU(nn.Module):
-    """ This convenience layer groups a 2D convolution, a batchnorm and a ReLU.
+class Conv2dBatchAct(nn.Module):
+    """
+    This convenience layer groups a 2D convolution, a batchnorm and an activation function.
     They are executed in a sequential manner.
 
     Args:
         in_channels (int): Number of input channels
         out_channels (int): Number of output channels
         kernel_size (int or tuple): Size of the kernel of the convolution
         stride (int or tuple): Stride of the convolution
         padding (int or tuple): padding of the convolution
         bias (bool, optional): Whether or not to enable the bias term for the convolution; Default **False**
         momentum (number, optional): momentum of the moving averages of the normalization; Default **0.1**
-        relu (class, optional): Which ReLU to use; Default :class:`torch.nn.ReLU`
+        activation (class, optional): Which activation function to use; Default :class:`torch.nn.ReLU`
         conv (nn.Module class, optional): Kind of 2D convolution to use; Default :class`~torch.nn.Conv2d`
 
-    .. figure:: /.static/api/conv2dbatchrelu.*
+    .. figure:: /.static/api/conv2dbatchact.*
        :width: 100%
-       :alt: Conv2dBatchReLU module design
+       :alt: Conv2dBatchAct module design
 
     Note:
         Possible options for the `conv` argument are:
 
         - :class:`torch.nn.Conv2d`
         - :class:`lightnet.network.layer.DeformableConv2d`
         - :class:`lightnet.network.layer.ModulatedDeformableConv2d`
 
     Example:
-        >>> module = ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1)
+        >>> module = ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1)
         >>> print(module)
-        Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+        Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
     def __init__(
         self,
         in_channels,
         out_channels,
         kernel_size,
         stride,
         padding,
         bias=False,
         momentum=0.1,
-        relu=default_relu,
+        activation=default_activation,
         conv=nn.Conv2d,
     ):
         super().__init__()
 
         self.layers = nn.ModuleList([
             conv(in_channels, out_channels, kernel_size, stride, padding, bias=bias),
             nn.BatchNorm2d(out_channels, momentum=momentum),
-            relu(),
+            activation(),
         ])
 
     def forward(self, x):
         x = self.layers[0](x)
         x = self.layers[1](x)
         x = self.layers[2](x)
         return x
 
     def __repr__(self):
-        s = '{name}BatchReLU({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {relu})'
+        s = '{name}BatchAct({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {activation})'
         return s.format(
             name=self.layers[0].__class__.__name__,
             in_channels=self.layers[0].in_channels,
             out_channels=self.layers[0].out_channels,
             kernel_size=self.layers[0].kernel_size,
             stride=self.layers[0].stride,
             padding=self.layers[0].padding,
-            relu=self.layers[2],
+            activation=self.layers[2],
         )
 
     @property
     def in_channels(self):
         return self.layers[0].in_channels
 
     @property
     def out_channels(self):
         return self.layers[0].out_channels
 
 
-class Conv2dReLU(nn.Module):
-    """ This convenience layer groups a 2D convolution and a ReLU.
+def Conv2dBatchReLU(
+    in_channels,
+    out_channels,
+    kernel_size,
+    stride,
+    padding,
+    bias=False,
+    momentum=0.1,
+    relu=Conv2dBatchAct.default_activation,
+    conv=nn.Conv2d,
+):
+    """
+    .. deprecated:: 4.0.0
+        |br| Conv2dBatchReLU is deprecated in favor for Conv2dBatchAct.
+    """
+    import warnings
+    warnings.warn(
+        'Conv2dBatchReLU is deprecated in favor for Conv2dBatchAct',
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
+    return Conv2dBatchAct(in_channels, out_channels, kernel_size, stride, padding, bias, momentum, relu, conv)
+
+
+class Conv2dAct(nn.Module):
+    """
+    This convenience layer groups a 2D convolution and an activation function.
     They are executed in a sequential manner.
 
     Args:
         in_channels (int): Number of input channels
         out_channels (int): Number of output channels
         kernel_size (int or tuple): Size of the kernel of the convolution
         stride (int or tuple): Stride of the convolution
         padding (int or tuple): padding of the convolution
         bias (bool, optional): Whether or not to enable the bias term for the convolution; Default **False**
-        relu (class, optional): Which ReLU to use; Default :class:`torch.nn.ReLU`
+        activation (class, optional): Which activation  to use; Default :class:`torch.nn.ReLU`
         conv (nn.Module class, optional): Kind of 2D convolution to use; Default :class`~torch.nn.Conv2d`
 
-    .. figure:: /.static/api/conv2drelu.*
+    .. figure:: /.static/api/conv2dact.*
        :width: 100%
-       :alt: Conv2dBatchReLU module design
+       :alt: Conv2dAct module design
 
     Note:
         Possible options for the `conv` argument are:
 
         - :class:`torch.nn.Conv2d`
         - :class:`lightnet.network.layer.DeformableConv2d`
         - :class:`lightnet.network.layer.ModulatedDeformableConv2d`
 
     Example:
-        >>> module = ln.network.layer.Conv2dReLU(3, 32, 3, 1, 1)
+        >>> module = ln.network.layer.Conv2dAct(3, 32, 3, 1, 1)
         >>> print(module)
-        Conv2dReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+        Conv2dAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
     def __init__(
         self,
         in_channels,
         out_channels,
         kernel_size,
         stride,
         padding,
         bias=False,
-        relu=default_relu,
+        activation=default_activation,
         conv=nn.Conv2d,
     ):
         super().__init__()
 
         self.layers = nn.ModuleList([
             conv(in_channels, out_channels, kernel_size, stride, padding, bias=bias),
-            relu(),
+            activation(),
         ])
 
     def forward(self, x):
         x = self.layers[0](x)
         x = self.layers[1](x)
         return x
 
     def __repr__(self):
-        s = '{name}ReLU({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {relu})'
+        s = '{name}Act({in_channels}, {out_channels}, kernel_size={kernel_size}, stride={stride}, padding={padding}, {activation})'
         return s.format(
             name=self.layers[0].__class__.__name__,
             in_channels=self.layers[0].in_channels,
             out_channels=self.layers[0].out_channels,
             kernel_size=self.layers[0].kernel_size,
             stride=self.layers[0].stride,
             padding=self.layers[0].padding,
-            relu=self.layers[1],
+            activation=self.layers[1],
         )
 
     @property
     def in_channels(self):
         return self.layers[0].in_channels
 
     @property
     def out_channels(self):
         return self.layers[0].out_channels
+
+
+def Conv2dReLU(
+    in_channels,
+    out_channels,
+    kernel_size,
+    stride,
+    padding,
+    bias=False,
+    momentum=0.1,
+    relu=Conv2dAct.default_activation,
+    conv=nn.Conv2d,
+):
+    """
+    .. deprecated:: 4.0.0
+        |br| Conv2dReLU is deprecated in favor for Conv2dAct.
+    """
+    import warnings
+    warnings.warn(
+        'Conv2dReLU is deprecated in favor for Conv2dAct',
+        category=DeprecationWarning,
+        stacklevel=2,
+    )
+    return Conv2dAct(in_channels, out_channels, kernel_size, stride, padding, bias, momentum, relu, conv)
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_hourglass.py` & `lightnet-4.0.0/lightnet/network/layer/_hourglass.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,52 +53,52 @@
 
     Example:
         >>> module = ln.network.layer.HourGlass(
         ...     2,                  # 2 nested hourglasses
         ...     [3, 32, 64],        # 2+1 channels, one for each hourglass level and a last one for the inner module
         ...
         ...     # UPPER: single convbatchrelu
-        ...     make_upper=lambda ci, co: ln.network.layer.Conv2dBatchReLU(ci, co, 3, 1, 1),
+        ...     make_upper=lambda ci, co: ln.network.layer.Conv2dBatchAct(ci, co, 3, 1, 1),
         ...
         ...     # DOWN 1: Providing keyword arguments
-        ...     make_down1=lambda ci, co, **kwargs: ln.network.layer.Conv2dBatchReLU(ci, co, **kwargs),
+        ...     make_down1=lambda ci, co, **kwargs: ln.network.layer.Conv2dBatchAct(ci, co, **kwargs),
         ...     down1_kwargs={'kernel_size': 3, 'stride': 2, 'padding': 1},
         ...
         ...     # INNER: Conv2dDepthWise
         ...     make_inner=lambda ci, co: ln.network.layer.Conv2dDepthWise(ci, co, 3, 1, 1),
         ...
         ...     # DOWN 2: Separate kwargs for each hourglass level
         ...     make_down2=lambda ci, co, **kwargs: torch.nn.Sequential(
-        ...         ln.network.layer.Conv2dBatchReLU(ci, co, **kwargs),
+        ...         ln.network.layer.Conv2dBatchAct(ci, co, **kwargs),
         ...         torch.nn.Upsample(scale_factor=2, mode='nearest'),
         ...     ),
         ...     down2_kwargs=[{'kernel_size': 3, 'stride': 1, 'padding': 1}, {'kernel_size': 1, 'stride': 1, 'padding': 0}],
         ... )
         >>> print(module)
         HourGlass(
           (layers): ParallelSum(
-            (upper): Conv2dBatchReLU(3, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (upper): Conv2dBatchAct(3, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             (down): Sequential(
-              (down1): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU(inplace=True))
+              (down1): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU(inplace=True))
               (inner): HourGlass(
                 (layers): ParallelSum(
-                  (upper): Conv2dBatchReLU(32, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                  (upper): Conv2dBatchAct(32, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                   (down): Sequential(
-                    (down1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU(inplace=True))
+                    (down1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), ReLU(inplace=True))
                     (inner): Conv2dDepthWise(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                     (down2): Sequential(
-                      (0): Conv2dBatchReLU(64, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
-                      (1): Upsample(scale_factor=2.0, mode=nearest)
+                      (0): Conv2dBatchAct(64, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+                      (1): Upsample(scale_factor=2.0, mode='nearest')
                     )
                   )
                 )
               )
               (down2): Sequential(
-                (0): Conv2dBatchReLU(32, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-                (1): Upsample(scale_factor=2.0, mode=nearest)
+                (0): Conv2dBatchAct(32, 3, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (1): Upsample(scale_factor=2.0, mode='nearest')
               )
             )
           )
         )
 
     .. _hgrepo: https://github.com/princeton-vl/pose-hg-train
     """
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_cornernet.py` & `lightnet-4.0.0/lightnet/network/layer/_cornernet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 #   Cornernet pooling layers
 #   Copyright EAVISE
 #
 from functools import partial
 from collections import OrderedDict
 import torch.nn as nn
-from ._conv import Conv2dBatch, Conv2dBatchReLU
+from ._conv import Conv2dBatch, Conv2dBatchAct
 from ._util import ParallelSum
 
 __all__ = ['TopPool', 'BottomPool', 'LeftPool', 'RightPool', 'CornerPool']
 
 
 class TopPool(nn.Module):
     """ Top pooling implementation :cite:`cornernet`. |br|
@@ -109,47 +109,60 @@
         >>> in_tensor = torch.rand(1, 32, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
 
     Warning:
         Compared to the `official CornerNet implementation <cornernetImpl_>`_,
-        this version of cornerpooling does not add the last 3x3 Conv2dBatchReLU module.
+        this version of cornerpooling does not add the last 3x3 Conv2dBatchAct module.
+
+    .. deprecated:: 4.0.0
+        |br| The `relu` argument is deprecated in favor for the more generic name "activation".
 
     .. _cornernetImpl: https://github.com/princeton-vl/CornerNet-Lite/blob/6a54505d830a9d6afe26e99f0864b5d06d0bbbaf/core/models/py_utils/utils.py#L187
     """
-    default_relu = partial(nn.ReLU, inplace=True)
+    default_activation = partial(nn.ReLU, inplace=True)
 
-    def __init__(self, channels, pool1, pool2, inter_channels=128, momentum=0.1, relu=default_relu):
+    def __init__(self, channels, pool1, pool2, inter_channels=128, momentum=0.1, activation=default_activation, relu=None):
         super().__init__()
+
+        if relu is not None:
+            import warnings
+            warnings.warn(
+                'The "relu" argument is deprecated in favor for the more generic name "activation"',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
+            activation = relu
+
         self.layers = ParallelSum(OrderedDict([
             ('pool', ParallelSum(
                 nn.Sequential(
-                    Conv2dBatchReLU(channels, inter_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                    Conv2dBatchAct(channels, inter_channels, 3, 1, 1, activation=activation, momentum=momentum),
                     pool1(),
                 ),
                 nn.Sequential(
-                    Conv2dBatchReLU(channels, inter_channels, 3, 1, 1, relu=relu, momentum=momentum),
+                    Conv2dBatchAct(channels, inter_channels, 3, 1, 1, activation=activation, momentum=momentum),
                     pool2(),
                 ),
                 post=Conv2dBatch(inter_channels, channels, 3, 1, 1),
             )),
             ('conv', Conv2dBatch(channels, channels, 1, 1, 0)),
-            ('post', relu()),
+            ('post', activation()),
         ]))
 
     def __repr__(self):
-        s = '{name}({channels}, {pool1}, {pool2}, inter_channels={inter_channels}, {relu})'
+        s = '{name}({channels}, {pool1}, {pool2}, inter_channels={inter_channels}, {activation})'
         return s.format(
             name=self.__class__.__name__,
             channels=self.layers.pool[0][0].layers[0].in_channels,
             pool1=self.layers.pool[0][1].__class__.__name__,
             pool2=self.layers.pool[1][1].__class__.__name__,
             inter_channels=self.layers.pool[0][0].layers[0].out_channels,
-            relu=self.layers.post,
+            activation=self.layers.post,
         )
 
     def forward(self, x):
         return self.layers(x)
 
     @property
     def in_channels(self):
```

### Comparing `lightnet-3.1.0/lightnet/network/layer/_util.py` & `lightnet-4.0.0/lightnet/network/layer/_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,46 @@
 #   Copyright EAVISE
 #
 import logging
 import torch
 import torch.nn as nn
 
 
-__all__ = ['FeatureExtractor', 'Parallel', 'ParallelCat', 'ParallelSum', 'Residual', 'SequentialSelect']
+__all__ = ['Combinator', 'FeatureExtractor', 'Parallel', 'ParallelCat', 'ParallelSum', 'Residual', 'SequentialSelect']
 log = logging.getLogger(__name__)
 
 
+class Combinator(nn.Module):
+    """
+    Combines N tensors together by either summing or concatenating them. |br|
+    The tensors are considered as batched tensors and are thus merged on dimension 1.
+
+    Args:
+        type('sum' | 'cat'): How to combine the different tensors.
+    """
+    def __init__(self, type='sum'):
+        super().__init__()
+
+        assert type in ('sum', 'cat'), 'Combinator type must be one of "sum", "cat"'
+        self.type = type
+
+    def forward(self, *x):
+        # Unpack input if it is passed as a list/tuple
+        if len(x) == 1 and isinstance(x[0], (list, tuple)):
+            x = x[0]
+
+        if self.type == 'cat':
+            return torch.cat(x, dim=1)
+        else:
+            return torch.sum(torch.stack(x, dim=1), dim=1)
+
+
 class FeatureExtractor(nn.Module):
-    """ Runs an nn.Module whilst storing intermediate features. |br|
+    """
+    Runs an nn.Module whilst storing intermediate features.
 
     Args:
         module (nn.Module): Module to run
         selection (list): names of the layers for which you want to get the output (See Note)
         return_selection (bool, optional): Whether to return the selected features, or just store the as `self.features`
 
     Note:
@@ -25,60 +51,60 @@
 
     Example:
         Usage of this module depends on the `return_selection` value. |br|
         The default, **False**, means that the module simply returns the output
         and the intermediate features can be accessed through the `self.features` dictionary:
 
         >>> layers = torch.nn.Sequential(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 128, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 128, 3, 1, 1),
         ... )
         >>> module = ln.network.layer.FeatureExtractor(
         ...     layers,
         ...     # We want to return the output from layers '1' and '3'
         ...     [1, 3],
         ...     # Since we specify False, the selected outputs will not be returned,
         ...     # but we can access them as `module.features`
         ...     # This is the default behaviour
         ...     False
         ... )
         >>> print(module)
         FeatureExtractor(
           selection=[1, 3], return=False
           (module): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (3): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (4): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (5): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (3): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (4): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (5): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
         )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 128, 10, 10])
         >>> print(module.features['1'].shape)
         torch.Size([1, 64, 10, 10])
         >>> print(module.features['3'].shape)
         torch.Size([1, 32, 10, 10])
 
         Setting `return_selection` to **True** means the module will return a tuple of ``(output, *selected)``:
 
         >>> layers = torch.nn.Sequential(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 128, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 128, 3, 1, 1),
         ... )
         >>> module = ln.network.layer.FeatureExtractor(layers, [1, 3], True)
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out, feat_1, feat_3 = module(in_tensor)
         >>> print(out.shape)
         torch.Size([1, 128, 10, 10])
         >>> print(feat_1.shape)
@@ -107,59 +133,61 @@
         x = self.module(x)
 
         if self.return_selection:
             return (x, *(self.features[s] for s in self.selection))
         else:
             return x
 
-    def _register_hooks(self):
-        def save_feature_hook(layer, inp, out):
-            layer.feature_extractor = out.clone()
+    @property
+    def features(self):
+        """ Return dictionary with extracted feature maps. """
+        return {name: self.module.get_submodule(name).feature_extractor for name in self.selection}
 
+    def _register_hooks(self):
         self.hook_handles = []
         for name in self.selection:
             mod = self.module.get_submodule(name)
             mod.register_buffer('feature_extractor', None, persistent=False)
-            self.hook_handles.append(mod.register_forward_hook(save_feature_hook))
+            self.hook_handles.append(mod.register_forward_hook(self._save_feature_hook))
 
-    @property
-    def features(self):
-        """ Return dictionary with extracted feature maps. """
-        return {name: self.module.get_submodule(name).feature_extractor for name in self.selection}
+    @staticmethod
+    def _save_feature_hook(layer, inp, out):
+        layer.feature_extractor = out.clone()
 
 
 class Parallel(nn.Sequential):
-    """ Container that runs each module on the input.
+    """
+    Container that runs each module on the input.
     The ouput is a list that contains the output of each of the different modules.
 
     Args:
         *args: Modules to run in parallel (similar to :class:`torch.nn.Sequential`)
 
     .. figure:: /.static/api/parallel.*
        :width: 100%
        :alt: Parallel module design
 
     Example:
         >>> # Note that the input channels should be the same for each branch (ic. 3)
         >>> module = ln.network.layer.Parallel(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 16, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 16, 3, 1, 1),
         ...     torch.nn.Sequential(
-        ...         ln.network.layer.Conv2dBatchReLU(3, 8, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(8, 16, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(16, 32, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(3, 8, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(8, 16, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(16, 32, 3, 1, 1),
         ...     ),
         ...     ln.network.layer.InvertedBottleneck(3, 64, 3, 1, 1),
         ... )
         >>> print(module)
         Parallel(
-          (0): Conv2dBatchReLU(3, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dBatchAct(3, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (1): Sequential(
-            (0): Conv2dBatchReLU(3, 8, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(8, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(16, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 8, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(8, 16, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(16, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
           (2): InvertedBottleneck(3, 64, kernel_size=(3, 3), stride=(1, 1), expansion=1, ReLU(inplace=True))
         )
         >>>
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out1, out2, out3 = module(in_tensor)
         >>> out1.shape
@@ -173,15 +201,16 @@
         super().__init__(*args)
 
     def forward(self, x):
         return [module(x) for module in self]
 
 
 class ParallelCat(nn.Sequential):
-    """ Parallel container that runs each module on the input and combines the different outputs by concatenating them.
+    """
+    Parallel container that runs each module on the input and combines the different outputs by concatenating them.
     The tensors are considered as batched tensors and are thus concatenated in dimension 1.
 
     Args:
         *args: Arguments passed to :class:`~lightnet.network.layer._util.Parallel`
         post (nn.Module, optional): Extra module that is run on the sum of the outputs of the other modules; Default **None**
 
     .. figure:: /.static/api/parallelcat.*
@@ -191,36 +220,36 @@
     Note:
         If you are using an `OrderedDict` to pass the modules to the sequential,
         you can set the `post` value inside of that dict as well.
 
     Example:
         >>> # Note that the input channels should be the same for each branch (ic. 3)
         >>> module = ln.network.layer.ParallelCat(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
         ...     torch.nn.Sequential(
-        ...         ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
         ...     ),
         ...     ln.network.layer.InvertedBottleneck(3, 32, 3, 1, 1),
         ...
         ...     # The post block should run on the concatenated tensor,
         ...     # so the in_channels are equal to the sum of the out_channels of the parallel modules
-        ...     post=ln.network.layer.Conv2dBatchReLU(96, 32, 1, 1, 0)
+        ...     post=ln.network.layer.Conv2dBatchAct(96, 32, 1, 1, 0)
         ... )
         >>> print(module)
         ParallelCat(
-          (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (1): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
           (2): InvertedBottleneck(3, 32, kernel_size=(3, 3), stride=(1, 1), expansion=1, ReLU(inplace=True))
-          (post): Conv2dBatchReLU(96, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (post): Conv2dBatchAct(96, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 32, 10, 10])
     """
     def __init__(self, *args, post=None):
@@ -236,15 +265,16 @@
         if self.post is not None:
             output = self.post(output)
 
         return output
 
 
 class ParallelSum(nn.Sequential):
-    """ Parallel container that runs each module on the input and combines the different outputs by summing them.
+    """
+    Parallel container that runs each module on the input and combines the different outputs by summing them.
 
     Args:
         *args: Arguments passed to :class:`~lightnet.network.layer._util.Parallel`
         post (nn.Module, optional): Extra module that is run on the sum of the outputs of the other modules; Default **None**
 
     .. figure:: /.static/api/parallelsum.*
        :width: 100%
@@ -253,36 +283,36 @@
     Note:
         If you are using an `OrderedDict` to pass the modules to the sequential,
         you can set the `post` value inside of that dict as well.
 
     Example:
         >>> # Note that the input channels and output channels should be the same for each branch (ic. 3 and 32)
         >>> module = ln.network.layer.ParallelSum(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
         ...     torch.nn.Sequential(
-        ...         ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...         ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...         ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
         ...     ),
         ...     ln.network.layer.InvertedBottleneck(3, 32, 3, 1, 1),
         ...
         ...     # The post block should run on the summed tensor,
         ...     # so the in_channels are equal to the out_channels of the parallel modules
-        ...     post=ln.network.layer.Conv2dBatchReLU(32, 1, 1, 1, 0),
+        ...     post=ln.network.layer.Conv2dBatchAct(32, 1, 1, 1, 0),
         ... )
         >>> print(module)
         ParallelSum(
-          (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (1): Sequential(
-            (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-            (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           )
           (2): InvertedBottleneck(3, 32, kernel_size=(3, 3), stride=(1, 1), expansion=1, ReLU(inplace=True))
-          (post): Conv2dBatchReLU(32, 1, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (post): Conv2dBatchAct(32, 1, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 1, 10, 10])
     """
     def __init__(self, *args, post=None):
@@ -298,85 +328,78 @@
         if self.post is not None:
             output = self.post(output)
 
         return output
 
 
 class Residual(nn.Sequential):
-    """ Residual block that runs like a Sequential, but then adds the original input to the output tensor.
+    """
+    Residual block that runs like a Sequential, but then adds the original input to the output tensor.
     See :class:`torch.nn.Sequential` for more information.
 
     Args:
         *args: Arguments passed to :class:`torch.nn.Sequential`
-        skip (nn.Module, optional): Extra module that is run on the input before adding it to the main block; Default **None**
-        post (nn.Module, optional): Extra module that is run on the output after everything is added; Default **None**
+        skip (nn.Module, optional): Extra module that is run on the input before adding it to the main block; Default :class:`torch.nn.Identity`
+        post (nn.Module, optional): Extra module that is run on the output after everything is added; Default :class:`torch.nn.Identity`
 
     .. figure:: /.static/api/residual.*
        :width: 100%
        :alt: Residual module design
 
     Note:
         If you are using an OrderedDict to pass the modules to the sequential,
         you can set the `skip` and `post` values inside of that dict as well.
 
     Example:
         >>> # Note that the input channels and output channels should be the same for each branch (ic. 3 and 32)
         >>> module = ln.network.layer.Residual(
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
         ...     # The skip block should ensure that the output tensor has the same number of channels
-        ...     skip=ln.network.layer.Conv2dBatchReLU(3, 32, 1, 1, 0),
+        ...     skip=ln.network.layer.Conv2dBatchAct(3, 32, 1, 1, 0),
         ...     # The post block should run on the summed tensor,
         ...     # so the in_channels are equal to the out_channels of the output of the residual
-        ...     post=ln.network.layer.Conv2dBatchReLU(32, 1, 1, 1, 0)
+        ...     post=ln.network.layer.Conv2dBatchAct(32, 1, 1, 1, 0)
         ... )
         >>> print(module)
         Residual(
-          (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (2): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (skip): Conv2dBatchReLU(3, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
-          (post): Conv2dBatchReLU(32, 1, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (2): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (skip): Conv2dBatchAct(3, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (post): Conv2dBatchAct(32, 1, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> out_tensor.shape
         torch.Size([1, 1, 10, 10])
     """
     def __init__(self, *args, skip=None, post=None):
         super().__init__(*args)
-        if skip is None and 'skip' in dir(self):
-            self.skip = self._modules['skip']
-        else:
-            self.skip = skip
 
-        if post is None and 'post' in dir(self):
-            self.post = self._modules['post']
-        else:
-            self.post = post
+        self.skip = skip if skip is not None else self._modules.get('skip', nn.Identity())
+        self.post = post if post is not None else self._modules.get('post', nn.Identity())
 
     def forward(self, x):
         y = x
         for name, module in self.named_children():
             if name not in ('skip', 'post'):
                 y = module(y)
 
-        if self.skip is not None:
-            x = self.skip(x)
-
+        x = self.skip(x)
         z = x + y
-        if self.post is not None:
-            z = self.post(z)
+        z = self.post(z)
 
         return z
 
 
 class SequentialSelect(nn.Sequential):
-    """ Sequential that allows to select which layers are to be considered as output.
+    """
+    Sequential that allows to select which layers are to be considered as output.
     See :class:`torch.nn.Sequential` for more information.
 
     .. deprecated:: 3.0.0
         |br| This class is deprectated in favor for the more powerful :class:`~lightnet.network.layer.FeatureExtractor`.
 
     Args:
         selection (list): names of the layers for which you want to get the output
@@ -409,49 +432,49 @@
         ...     [1, 3],
         ...
         ...     # Since we specify False, the selected outputs will not be returned,
         ...     # but we can access them as `module.selected`
         ...     False,
         ...
         ...     # Sequential
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 128, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 128, 3, 1, 1),
         ... )
         >>> print(module)
         SequentialSelect(
           selection=['1', '3'], return=False
-          (0): Conv2dBatchReLU(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (1): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (2): Conv2dBatchReLU(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (3): Conv2dBatchReLU(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (4): Conv2dBatchReLU(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (5): Conv2dBatchReLU(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dBatchAct(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (1): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (2): Conv2dBatchAct(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (3): Conv2dBatchAct(64, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (4): Conv2dBatchAct(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (5): Conv2dBatchAct(64, 128, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_tensor = module(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 128, 10, 10])
         >>> print(module.selected['1'].shape)
         torch.Size([1, 64, 10, 10])
         >>> print(module.selected['3'].shape)
         torch.Size([1, 32, 10, 10])
 
         >>> # Setting return_selection to True means the module will return a tuple of (output, *selected)
         >>> module = ln.network.layer.SequentialSelect(
         ...     [1, 3], True,
-        ...     ln.network.layer.Conv2dBatchReLU(3, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 32, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(32, 64, 3, 1, 1),
-        ...     ln.network.layer.Conv2dBatchReLU(64, 128, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(3, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 32, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(32, 64, 3, 1, 1),
+        ...     ln.network.layer.Conv2dBatchAct(64, 128, 3, 1, 1),
         ... )
         >>> in_tensor = torch.rand(1, 3, 10, 10)
         >>> out_5, out_1, out_3 = module(in_tensor)
         >>> print(out_5.shape)
         torch.Size([1, 128, 10, 10])
         >>> print(out_1.shape)
         torch.Size([1, 64, 10, 10])
```

### Comparing `lightnet-3.1.0/lightnet/network/_basemodule.py` & `lightnet-4.0.0/lightnet/network/_basemodule.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/network/head/_classification_conv.py` & `lightnet-4.0.0/lightnet/network/head/_classification_conv.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 class ClassificationConv(BaseModule):
     """ Convolutional Classification head.
 
     Args:
         in_channels (int): Number of input channels
         num_classes (int): Number of classes
         conv_first (bool, optional): Whether to place the convolution before or after the :class:`~torch.nn.AdaptiveAvgPool2d`; Default **False**
-        dropout (bool, optional): Whether to add a dropout layer before the convolution; Default **False**
-        relu (bool, optional): Whether to add a :class:`~torch.nn.ReLU` after the convolution; Default **False**
+        dropout (float, optional): Dropout probability (set to zero to disable); Default **0**
+        activation (nn.Module, optional): Activation function to add after the convolution; Default **None**
 
     .. rubric:: Models:
 
     - :class:`~lightnet.models.Darknet`
     - :class:`~lightnet.models.Darknet19`
     - :class:`~lightnet.models.Darknet53`
     - :class:`~lightnet.models.MobilenetV1`
@@ -41,25 +41,25 @@
         torch.Size([1, 1000])
     """
     @BaseModule.layers
     def Default(
         in_channels,
         num_classes,
         conv_first=False,
-        dropout=False,
-        relu=False,
+        dropout=0,
+        activation=None,
     ):
         conv_layers = [
             nn.Conv2d(in_channels, num_classes, 1, 1, 0),
         ]
 
-        if dropout:
-            conv_layers.insert(0, nn.Dropout())
-        if relu:
-            conv_layers.append(nn.ReLU(inplace=True))
+        if dropout > 0:
+            conv_layers.insert(0, nn.Dropout(p=dropout))
+        if activation is not None:
+            conv_layers.append(activation)
 
         if conv_first:
             return (
                 *conv_layers,
                 nn.AdaptiveAvgPool2d(1),
                 nn.Flatten(),
             )
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_classification_fc.py` & `lightnet-4.0.0/lightnet/network/head/_classification_fc.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,38 +12,45 @@
     """ Fully Connected Classification head.
 
     Args:
         in_channels (int): Number of input channels
         num_classes (int): Number of classes
         pooling_size (int or tuple, optional): output_size of the :class:`~torch.nn.AdaptiveAvgPool2d` layer; Default **1**
         inter_channels (int, optional): How many channels to use for the intermediate layers (See Note); Default **0**
+        dropout (float, optional): Dropout probability (set to zero to disable); Default **0**
         dropout_first (bool, optional): Whether to add dropout layers before or after each of the intermediate Linear+ReLU layers; Default **False**
 
     .. rubric:: Models:
 
     - :class:`~lightnet.models.Alexnet`
     - :class:`~lightnet.models.VGG11`
     - :class:`~lightnet.models.VGG13`
     - :class:`~lightnet.models.VGG16`
     - :class:`~lightnet.models.VGG19`
 
+    Note:
+        If `inter_channels` is set to a number greater than zero, we add the following additional layers twice:
+            - Linear > ReLU (`dropout` = **0**)
+            - Dropout > Linear > ReLU (`dropout` > **0** and `dropout_first` = **True**)
+            - Linear > ReLU > Dropout (`dropout` > **0** and `dropout_first` = **False**)
+
     Examples:
         >>> head = ln.network.head.ClassificationFC(256, 1000)
         >>> print(head)
         Sequential(
           (0): AdaptiveAvgPool2d(output_size=1)
           (1): Flatten(start_dim=1, end_dim=-1)
           (2): Linear(in_features=256, out_features=1000, bias=True)
         )
         >>> in_tensor = torch.rand(1, 256, 13, 13)
         >>> out_tensor = head(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 1000])
 
-        >>> head = ln.network.head.ClassificationFC(256, 1000, inter_channels=4096)
+        >>> head = ln.network.head.ClassificationFC(256, 1000, inter_channels=4096, dropout=0.5)
         >>> print(head)
         Sequential(
           (0): AdaptiveAvgPool2d(output_size=1)
           (1): Flatten(start_dim=1, end_dim=-1)
           (2): Linear(in_features=256, out_features=4096, bias=True)
           (3): ReLU(inplace=True)
           (4): Dropout(p=0.5, inplace=False)
@@ -59,14 +66,15 @@
     """
     @BaseModule.layers
     def Default(
         in_channels,
         num_classes,
         pooling_size=1,
         inter_channels=0,
+        dropout=0,
         dropout_first=False,
     ):
         if isinstance(pooling_size, int):
             in_channels *= pooling_size ** 2
         else:
             in_channels *= pooling_size[0] * pooling_size[1]
 
@@ -75,20 +83,21 @@
                 nn.Linear(in_channels, inter_channels),
                 nn.ReLU(inplace=True),
                 nn.Linear(inter_channels, inter_channels),
                 nn.ReLU(inplace=True),
             ]
             in_channels = inter_channels
 
-            if dropout_first:
-                inter_layers.insert(0, nn.Dropout())
-                inter_layers.insert(3, nn.Dropout())
-            else:
-                inter_layers.insert(2, nn.Dropout())
-                inter_layers.insert(5, nn.Dropout())
+            if dropout > 0:
+                if dropout_first:
+                    inter_layers.insert(0, nn.Dropout(p=dropout))
+                    inter_layers.insert(3, nn.Dropout(p=dropout))
+                else:
+                    inter_layers.insert(2, nn.Dropout(p=dropout))
+                    inter_layers.insert(5, nn.Dropout(p=dropout))
         else:
             inter_layers = []
 
         return (
             nn.AdaptiveAvgPool2d(pooling_size),
             nn.Flatten(),
             *inter_layers,
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_detection_corner.py` & `lightnet-4.0.0/lightnet/network/head/_detection_corner.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,44 +25,44 @@
 
     Examples:
         >>> head = ln.network.head.DetectionCorner(256, 20)
         >>> print(head)
         ParallelCat(
           (topleft): Sequential(
             (1_corner): CornerPool(256, TopPool, LeftPool, inter_channels=128, ReLU(inplace=True))
-            (2_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             (output): ParallelCat(
               (heatmap): Sequential(
-                (3_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (3_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (4_conv): Conv2d(256, 20, kernel_size=(1, 1), stride=(1, 1))
               )
               (embedding): Sequential(
-                (5_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (5_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (6_conv): Conv2d(256, 1, kernel_size=(1, 1), stride=(1, 1))
               )
               (offset): Sequential(
-                (7_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (7_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (8_conv): Conv2d(256, 2, kernel_size=(1, 1), stride=(1, 1))
               )
             )
           )
           (bottomright): Sequential(
             (1_corner): CornerPool(256, BottomPool, RightPool, inter_channels=128, ReLU(inplace=True))
-            (2_convbatch): Conv2dBatchReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+            (2_convbatch): Conv2dBatchAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
             (output): ParallelCat(
               (heatmap): Sequential(
-                (3_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (3_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (4_conv): Conv2d(256, 20, kernel_size=(1, 1), stride=(1, 1))
               )
               (embedding): Sequential(
-                (5_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (5_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (6_conv): Conv2d(256, 1, kernel_size=(1, 1), stride=(1, 1))
               )
               (offset): Sequential(
-                (7_conv): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+                (7_conv): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
                 (8_conv): Conv2d(256, 2, kernel_size=(1, 1), stride=(1, 1))
               )
             )
           )
         )
         >>> in_tensor = torch.rand(1, 256, 104, 104)
         >>> out_tensor = head(in_tensor)
@@ -75,42 +75,42 @@
         num_classes,
         squeeze=False,
     ):
         kernel = (1, 1, 0) if squeeze else (3, 1, 1)
         return (
             ('topleft',                 nn.Sequential(OrderedDict([
                 ('1_corner',            lnl.CornerPool(in_channels, lnl.TopPool, lnl.LeftPool)),
-                ('2_convbatch',         lnl.Conv2dBatchReLU(in_channels, 256, 3, 1, 1)),
+                ('2_convbatch',         lnl.Conv2dBatchAct(in_channels, 256, 3, 1, 1)),
                 ('output',              lnl.ParallelCat(OrderedDict([
                     ('heatmap',         nn.Sequential(OrderedDict([
-                        ('3_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('3_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('4_conv',      nn.Conv2d(256, num_classes, 1, 1, 0)),
                     ]))),
                     ('embedding',       nn.Sequential(OrderedDict([
-                        ('5_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('5_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('6_conv',      nn.Conv2d(256, 1, 1, 1, 0)),
                     ]))),
                     ('offset',          nn.Sequential(OrderedDict([
-                        ('7_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('7_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('8_conv',      nn.Conv2d(256, 2, 1, 1, 0)),
                     ]))),
                 ]))),
             ]))),
             ('bottomright',             nn.Sequential(OrderedDict([
                 ('1_corner',            lnl.CornerPool(in_channels, lnl.BottomPool, lnl.RightPool)),
-                ('2_convbatch',         lnl.Conv2dBatchReLU(in_channels, 256, 3, 1, 1)),
+                ('2_convbatch',         lnl.Conv2dBatchAct(in_channels, 256, 3, 1, 1)),
                 ('output',              lnl.ParallelCat(OrderedDict([
                     ('heatmap',         nn.Sequential(OrderedDict([
-                        ('3_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('3_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('4_conv',      nn.Conv2d(256, num_classes, 1, 1, 0)),
                     ]))),
                     ('embedding',       nn.Sequential(OrderedDict([
-                        ('5_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('5_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('6_conv',      nn.Conv2d(256, 1, 1, 1, 0)),
                     ]))),
                     ('offset',          nn.Sequential(OrderedDict([
-                        ('7_conv',      lnl.Conv2dReLU(256, 256, *kernel, bias=True)),
+                        ('7_conv',      lnl.Conv2dAct(256, 256, *kernel, bias=True)),
                         ('8_conv',      nn.Conv2d(256, 2, 1, 1, 0)),
                     ]))),
                 ]))),
             ]))),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_detection_anchor_yolo.py` & `lightnet-4.0.0/lightnet/network/head/_detection_anchor_yolo.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,51 +16,52 @@
     Args:
         in_channels (int): Number of input channels
         num_anchors (int): Number of anchors
         num_classes (int): Number of classes
         inter_channels (int, optional): How many channels to use for the intermediate convolution; Default **1024**
         point_wise (bool, optional): Whether to use a 1x1 pointwise or a regular 3x3 intermediate convolution; Default **False**
         momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.01**
-        relu (class, optional): Which ReLU to use; Default :class:`torch.nn.LeakyReLU(0.1)`
+        activation (class, optional): Which activation function to use; Default :class:`torch.nn.LeakyReLU(0.1)`
 
     .. rubric:: Models:
 
     - :class:`~lightnet.models.DYolo`
     - :class:`~lightnet.models.MobilenetYolo`
     - :class:`~lightnet.models.MobileYoloV2`
     - :class:`~lightnet.models.MobileYoloV2Upsample`
     - :class:`~lightnet.models.TinyYoloV2`
     - :class:`~lightnet.models.TinyYoloV3`
     - :class:`~lightnet.models.YoloV2`
     - :class:`~lightnet.models.YoloV2Upsample`
     - :class:`~lightnet.models.YoloV3`
+    - :class:`~lightnet.models.YoloV4`
     - :class:`~lightnet.models.Yolt`
 
     Examples:
         >>> head = ln.network.head.DetectionYoloAnchor(1280, 5, 20)
         >>> print(head)
         Sequential(
-          (0): Conv2dBatchReLU(1280, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+          (0): Conv2dBatchAct(1280, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
           (1): Conv2d(1024, 125, kernel_size=(1, 1), stride=(1, 1))
         )
         >>> in_tensor = torch.rand(1, 1280, 13, 13)
         >>> out_tensor = head(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 125, 13, 13])
     """
-    default_relu = partial(nn.LeakyReLU, 0.1, inplace=True)
+    default_activation = partial(nn.LeakyReLU, 0.1, inplace=True)
 
     @BaseModule.layers
     def Default(
         in_channels,
         num_anchors,
         num_classes,
         inter_channels=1024,
         point_wise=False,
         momentum=0.01,
-        relu=default_relu,
+        activation=default_activation,
     ):
         kernel = (1, 1, 0) if point_wise else (3, 1, 1)
         return (
-            lnl.Conv2dBatchReLU(in_channels, inter_channels, *kernel, relu=relu, momentum=momentum),
+            lnl.Conv2dBatchAct(in_channels, inter_channels, *kernel, activation=activation, momentum=momentum),
             nn.Conv2d(inter_channels, num_anchors*(5+num_classes), 1, 1, 0),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_detection_anchor_masked.py` & `lightnet-4.0.0/lightnet/network/head/_detection_anchor_masked.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from .. import layer as lnl
 from .._basemodule import BaseModule
 
 __all__ = ['DetectionMaskedAnchor']
 
 
 class DetectionMaskedAnchor(BaseModule):
-    """ Masked Anchor Detection head. |br|
+    """
+    Masked Anchor Detection head. |br|
     This heads predicts instance segmentation masks as well as bounding boxes.
 
     It works in a similar way as :cite:`yolact`, where it outputs prototype masks as well as the bounding boxes.
     Each bounding box then outputs a number for each mask, which are then used to generate the final mask foreach bounding box by taking a linear combination.
 
     .. rubric:: Models:
 
@@ -27,31 +28,31 @@
         Every model needs at least one detection head and one mask protonet head.
 
     Examples:
         >>> detection_head = ln.network.head.DetectionMaskedAnchor.Prediction(1280, 5, 20, 32)
         >>> mask_head = ln.network.head.DetectionMaskedAnchor.Protonet(1280, 32)
         >>> print(detection_head)
         Sequential(
-          (0): Conv2dReLU(1280, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dAct(1280, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (1): ParallelCat(
             (0): Conv2d(256, 125, kernel_size=(1, 1), stride=(1, 1))
             (1): Sequential(
               (0): Conv2d(256, 160, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
               (1): Tanh()
             )
           )
         )
         >>> print(mask_head)
         Sequential(
-          (0): Conv2dReLU(1280, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (1): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (2): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (3): Upsample(scale_factor=2.0, mode=bilinear)
-          (4): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (5): Conv2dReLU(256, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (0): Conv2dAct(1280, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (1): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (2): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (3): Upsample(scale_factor=2.0, mode='bilinear')
+          (4): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (5): Conv2dAct(256, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 1280, 13, 13)
         >>> out = detection_head(in_tensor)
         >>> mask = mask_head(in_tensor)
         >>> print(out.shape)
         torch.Size([1, 285, 13, 13])
         >>> print(mask.shape)
@@ -72,15 +73,15 @@
             in_channels (int): Number of input channels
             num_anchors (int): Number of anchors
             num_classes (int): Number of classes
             num_masks (int): Number of prototype masks
             inter_channels (int, optional): How many channels to use for the intermediate convolutions; Default **256**
         """
         return (
-            lnl.Conv2dReLU(in_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(in_channels, inter_channels, 3, 1, 1, bias=True),
             lnl.ParallelCat(
                 nn.Conv2d(inter_channels, num_anchors*(5+num_classes), 1, 1, 0),
                 nn.Sequential(
                     nn.Conv2d(inter_channels, num_anchors*num_masks, 3, 1, 1, bias=True),
                     nn.Tanh(),
                 ),
             ),
@@ -97,14 +98,14 @@
 
         Args:
             in_channels (int): Number of input channels
             num_masks (int): Number of prototype masks
             inter_channels (int, optional): How many channels to use for the intermediate convolutions; Default **256**
         """
         return (
-            lnl.Conv2dReLU(in_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(in_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
             nn.Upsample(scale_factor=2, mode='bilinear', align_corners=False),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, num_masks, 1, 1, 0, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, num_masks, 1, 1, 0, bias=True),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_detection_yolact.py` & `lightnet-4.0.0/lightnet/network/head/_detection_yolact.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,32 +24,32 @@
     - :class:`~lightnet.models.Yolact101`
 
     Examples:
         >>> detection_head = ln.network.head.DetectionYolact.Prediction(256, 3, 20, 32)
         >>> mask_head = ln.network.head.DetectionYolact.Protonet(256, 32)
         >>> print(detection_head)
         Sequential(
-          (0): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (1): ParallelCat(
             (0): Conv2d(256, 12, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
             (1): Conv2d(256, 63, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
             (2): Sequential(
               (0): Conv2d(256, 96, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
               (1): Tanh()
             )
           )
         )
         >>> print(mask_head)
         Sequential(
-          (0): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (1): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (2): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (0): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (1): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (2): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
           (3): Upsample(scale_factor=2.0, mode=bilinear)
-          (4): Conv2dReLU(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
-          (5): Conv2dReLU(256, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
+          (4): Conv2dAct(256, 256, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), ReLU(inplace=True))
+          (5): Conv2dAct(256, 32, kernel_size=(1, 1), stride=(1, 1), padding=(0, 0), ReLU(inplace=True))
         )
         >>> in_tensor = torch.rand(1, 256, 8, 8)
         >>> out_tensor = prediction_head(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 171, 8, 8])
         >>> mask_tensor = mask_head(in_tensor)
         >>> print(mask_tensor.shape)
@@ -72,15 +72,15 @@
             in_channels (int): Number of input channels
             num_anchors (int): Number of anchors
             num_classes (int): Number of classes
             num_masks (int): Number of prototype masks
             inter_channels (int, optional): How many channels to use for the intermediate convolutions; Default **256**
         """
         return (
-            lnl.Conv2dReLU(in_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(in_channels, inter_channels, 3, 1, 1, bias=True),
             lnl.ParallelCat(
                 nn.Conv2d(inter_channels, 4*num_anchors, 3, 1, 1, bias=True),
                 nn.Conv2d(inter_channels, (num_classes+1)*num_anchors, 3, 1, 1, bias=True),
                 nn.Sequential(
                     nn.Conv2d(inter_channels, num_masks*num_anchors, 3, 1, 1, bias=True),
                     nn.Tanh(),
                 ),
@@ -98,14 +98,14 @@
 
         Args:
             in_channels (int): Number of input channels
             num_masks (int): Number of prototype masks
             inter_channels (int, optional): How many channels to use for the intermediate convolutions; Default **256**
         """
         return (
-            lnl.Conv2dReLU(in_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(in_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
             nn.Upsample(scale_factor=2, mode='bilinear', align_corners=False),
-            lnl.Conv2dReLU(inter_channels, inter_channels, 3, 1, 1, bias=True),
-            lnl.Conv2dReLU(inter_channels, num_masks, 1, 1, 0, bias=True),
+            lnl.Conv2dAct(inter_channels, inter_channels, 3, 1, 1, bias=True),
+            lnl.Conv2dAct(inter_channels, num_masks, 1, 1, 0, bias=True),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/head/_detection_anchor_oriented.py` & `lightnet-4.0.0/lightnet/network/head/_detection_anchor_oriented.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,45 +17,45 @@
     Args:
         in_channels (int): Number of input channels
         num_anchors (int): Number of anchors
         num_classes (int): Number of classes
         inter_channels (int, optional): How many channels to use for the intermediate convolution; Default **1024**
         point_wise (bool, optional): Whether to use a 1x1 pointwise or a regular 3x3 intermediate convolution; Default **False**
         momentum (float, optional): Momentum of the moving averages of the normalization; Default **0.01**
-        relu (class, optional): Which ReLU to use; Default :class:`torch.nn.LeakyReLU(0.1)`
+        activation (class, optional): Which activation function to use; Default :class:`torch.nn.LeakyReLU(0.1)`
 
     .. rubric:: Models:
 
     - :class:`~lightnet.models.O_DYolo`
     - :class:`~lightnet.models.O_YoloV2`
     - :class:`~lightnet.models.O_YoloV3`
     - :class:`~lightnet.models.O_Yolt`
 
     Examples:
         >>> head = ln.network.head.DetectionOrientedAnchor(1280, 5, 20)
         >>> print(head)
         Sequential(
-          (0): Conv2dBatchReLU(1280, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
+          (0): Conv2dBatchAct(1280, 1024, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), LeakyReLU(negative_slope=0.1, inplace=True))
           (1): Conv2d(1024, 130, kernel_size=(1, 1), stride=(1, 1))
         )
         >>> in_tensor = torch.rand(1, 1280, 13, 13)
         >>> out_tensor = head(in_tensor)
         >>> print(out_tensor.shape)
         torch.Size([1, 130, 13, 13])
     """
-    default_relu = partial(nn.LeakyReLU, 0.1, inplace=True)
+    default_activation = partial(nn.LeakyReLU, 0.1, inplace=True)
 
     @BaseModule.layers
     def Default(
         in_channels,
         num_anchors,
         num_classes,
         inter_channels=1024,
         point_wise=False,
         momentum=0.01,
-        relu=default_relu,
+        activation=default_activation,
     ):
         kernel = (1, 1, 0) if point_wise else (3, 1, 1)
         return (
-            lnl.Conv2dBatchReLU(in_channels, inter_channels, *kernel, relu=relu, momentum=momentum),
+            lnl.Conv2dBatchAct(in_channels, inter_channels, *kernel, activation=activation, momentum=momentum),
             nn.Conv2d(inter_channels, num_anchors*(6+num_classes), 1, 1, 0),
         )
```

### Comparing `lightnet-3.1.0/lightnet/network/module/_darknet.py` & `lightnet-4.0.0/lightnet/network/module/_darknet.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             *args, \*\*kwargs: Extra arguments passed to :func:`lightnet.network.module.Lightnet.load` when loading pytorch weights
 
         Note:
             Darknet weight files also contain the number of images the network has been trained on. |br|
             In Lightnet however, this is a parameter from the loss function and as such this value cannot be correctly set on that object.
             This value will thus be ignored by lightnet and when saving a darknet file, this value will be set to zero.
         """
-        if os.path.splitext(weights_file)[1] == '.pt':
+        if os.path.splitext(weights_file)[1] in ('.pt', '.pth'):
             log.debug('Loading weights from pytorch file')
             super().load(weights_file, *args, **kwargs)
         else:
             log.debug('Loading weights from darknet file')
             self._load_darknet_weights(weights_file)
 
     def save(self, weights_file, *args, **kwargs):
@@ -44,54 +44,71 @@
         If the file extension is ``.pt``, it will be considered as a `pytorch pickle file <http://pytorch.org/docs/stable/notes/serialization.html#recommended-approach-for-saving-a-model>`_.
         Otherwise, the file is considered to be a darknet binary weight file.
 
         Args:
             weights_file (str): path to file
             *args, \*\*kwargs: Extra arguments passed to :func:`lightnet.network.module.Lightnet.save` when saving as pytorch weights
         """
-        if os.path.splitext(weights_file)[1] == '.pt':
+        if os.path.splitext(weights_file)[1] in ('.pt', '.pth'):
             log.debug('Saving weights to pytorch file')
             super().save(weights_file, *args, **kwargs)
         else:
             log.debug('Saving weights to darknet file')
             self._save_darknet_weights(weights_file)
 
     def _load_darknet_weights(self, weights_file):
         weights = WeightLoader(weights_file)
         self.header = weights.header
 
         done_loading = False
-        for name, module in self.named_modules(types=weights.layers, recurse_into_matched=False):
+        for name, module in self._loop_modules(weights.layers):
             if not done_loading:
                 weights.load_layer(module)
                 log.debug('Layer loaded: %s', name)
                 if weights.start >= weights.size:
                     log.debug('Finished loading weights [%d/%d weights]', weights.start, weights.size)
                     done_loading = True
             else:
                 log.warning('No more weigths for layer: %s', name)
 
         if not done_loading:
-            log.debug('Finished loading weights [%d/%d weights]', weights.start, weights.size)
+            if weights.start != weights.size:
+                log.warn('Not all weights were loaded [%d/%d weights]', weights.start, weights.size)
+            else:
+                log.debug('Finished loading weights [%d/%d weights]', weights.start, weights.size)
 
     def _save_darknet_weights(self, weights_file):
         weights = WeightSaver(self.header, 0)
 
-        for name, module in self.named_modules(types=weights.layers, recurse_into_matched=False):
+        for name, module in self._loop_modules(weights.layers):
             weights.save_layer(module)
             log.debug('Layer saved: %s', name)
 
         weights.write_file(weights_file)
 
+    def _loop_modules(self, layer_types):
+        """
+        Generator that returns `name, module` tuples.
+        Internally, it calls :func:`~lightnet.network.module.Lightnet.named_modules`, unless the module has a `darknet_order` attribute.
+        This `darknet_order` attribute should be a list of module names or be a generator that yields the module names in a certain order.
+        """
+        if hasattr(self, 'darknet_order'):
+            for name in self.darknet_order:
+                module = self.get_submodule(name)
+                if isinstance(module, layer_types):
+                    yield name, module
+        else:
+            yield from self.named_modules(types=layer_types, recurse_into_matched=False)
+
 
 class WeightLoader:
     """ Load darknet weight files into pytorch layers """
     layers = (
-        lnl.Conv2dBatchReLU,
-        lnl.Conv2dReLU,
+        lnl.Conv2dBatchAct,
+        lnl.Conv2dAct,
         nn.Conv2d,
         nn.Linear,
     )
 
     def __init__(self, filename):
         with open(filename, 'rb') as fp:
             self.header = tuple(np.fromfile(fp, count=3, dtype=np.int32))
@@ -104,28 +121,29 @@
             elif ver_num <= 29:
                 log.warning('Weight file uses sizeof to compute variable size, which might lead to undefined behaviour. (choosing int=int32, float=float32, size_t=int64)')
                 self.seen = int(np.fromfile(fp, count=1, dtype=np.int64)[0])
             else:
                 log.error('New weight file syntax! Loading of weights might not work properly. Please submit an issue with the weight file version number. [Run with DEBUG logging level]')
                 self.seen = int(np.fromfile(fp, count=1, dtype=np.int64)[0])
 
+            log.debug('Weight file has seen %d images', self.seen)
             self.buf = np.fromfile(fp, dtype=np.float32)
 
         self.start = 0
         self.size = self.buf.size
 
     def load_layer(self, layer):
         """ Load weights for a layer from the weights file """
-        if type(layer) == nn.Conv2d:
+        if isinstance(layer, nn.Conv2d):
             self._load_conv(layer)
-        elif type(layer) == lnl.Conv2dReLU:
+        elif isinstance(layer, lnl.Conv2dAct):
             self._load_conv(layer.layers[0])
-        elif type(layer) == lnl.Conv2dBatchReLU:
+        elif isinstance(layer, lnl.Conv2dBatchAct):
             self._load_convbatch(layer)
-        elif type(layer) == nn.Linear:
+        elif isinstance(layer, nn.Linear):
             self._load_fc(layer)
         else:
             raise NotImplementedError(f'The layer you are trying to load is not supported [{type(layer)}]')
 
     def _load_conv(self, model):
         num_b = model.bias.numel()
         model.bias.data.copy_(torch.from_numpy(self.buf[self.start:self.start+num_b])
@@ -168,16 +186,16 @@
                                      .view_as(model.weight.data))
         self.start += num_w
 
 
 class WeightSaver:
     """ Save darknet weight files from pytorch layers """
     layers = (
-        lnl.Conv2dBatchReLU,
-        lnl.Conv2dReLU,
+        lnl.Conv2dBatchAct,
+        lnl.Conv2dAct,
         nn.Conv2d,
         nn.Linear,
     )
 
     def __init__(self, header, seen):
         self.weights = []
         self.header = np.array(header, dtype=np.int32)
@@ -198,21 +216,21 @@
             self.seen.tofile(fp)
             for np_arr in self.weights:
                 np_arr.tofile(fp)
         log.info('Weight file saved as %s', filename)
 
     def save_layer(self, layer):
         """ save weights for a layer """
-        if type(layer) == nn.Conv2d:
+        if isinstance(layer, nn.Conv2d):
             self._save_conv(layer)
-        elif type(layer) == lnl.Conv2dReLU:
+        elif isinstance(layer, lnl.Conv2dAct):
             self._save_conv(layer.layers[0])
-        elif type(layer) == lnl.Conv2dBatchReLU:
+        elif isinstance(layer, lnl.Conv2dBatchAct):
             self._save_convbatch(layer)
-        elif type(layer) == nn.Linear:
+        elif isinstance(layer, nn.Linear):
             self._save_fc(layer)
         else:
             raise NotImplementedError(f'The layer you are trying to save is not supported [{type(layer)}]')
 
     def _save_conv(self, model):
         self.weights.append(model.bias.cpu().data.numpy())
         self.weights.append(model.weight.cpu().data.numpy())
```

### Comparing `lightnet-3.1.0/lightnet/network/module/_lightnet.py` & `lightnet-4.0.0/lightnet/network/module/_lightnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 from lightnet.network.layer import DeformableConv2d, ModulatedDeformableConv2d
 
 __all__ = ['Lightnet']
 log = logging.getLogger(__name__)
 
 
 class Lightnet(nn.Module):
-    """ This class provides an abstraction layer on top of :class:`pytorch:torch.nn.Module`
+    """
+    This class provides an abstraction layer on top of :class:`pytorch:torch.nn.Module`
     and is used as a base for every network implemented in this framework.
 
     The default initialization will first call :func:`~lightnet.network.module.Lightnet.__init_module`,
     which is meant to initialize all the layers of the network.
     Afterwards, it will loop through :func:`torch.nn.Module.named_modules`
     and call :func:`~lightnet.network.module.Lightnet.__init_weights` on each module, in order to initialize the weights.
     """
@@ -63,35 +64,42 @@
             mod (nn.Module): layer module
 
         Note:
             As a user, you can overwrite this method and set values for some layers.
             Call `return super().__init_weights(name, mod)` add the end of your custom method,
             so that other layers get this default behaviour.
         """
+        # Deformable convolutions
         if isinstance(mod, (DeformableConv2d, ModulatedDeformableConv2d)):
             nn.init.kaiming_normal_(mod.conv.weight, nonlinearity='relu')
             if mod.conv.bias is not None:
                 nn.init.constant_(mod.conv.bias, 0)
 
             nn.init.constant_(mod.deformable_module.weight, 0)
             if mod.deformable_module.bias is not None:
                 nn.init.constant_(mod.deformable_module.bias, 0)
 
             return True
-        elif isinstance(mod, nn.Conv2d):
+
+        # Convolutions
+        if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='relu')
             if mod.bias is not None:
                 nn.init.constant_(mod.bias, 0)
             return True
-        elif isinstance(mod, (nn.BatchNorm2d, nn.GroupNorm)):
-            nn.init.constant_(mod.weight, 1)
+
+        # Fully Connected
+        if isinstance(mod, nn.Linear):
+            nn.init.normal_(mod.weight, 0, 0.01)
             nn.init.constant_(mod.bias, 0)
             return True
-        elif isinstance(mod, nn.Linear):
-            nn.init.normal_(mod.weight, 0, 0.01)
+
+        # Normalisation
+        if isinstance(mod, (nn.BatchNorm2d, nn.GroupNorm)):
+            nn.init.constant_(mod.weight, 1)
             nn.init.constant_(mod.bias, 0)
             return True
 
     def modules(self, types=None, recurse_into_matched=True):
         """ Overload for :func:`torch.nn.Modules.modules` that provides extra features. |br|
         This version of the method allows you to pass in a list of module types for which you are interested.
         Only those modules will be returned from the generator.
@@ -109,15 +117,16 @@
             We use the ``isinstance`` function in order to check whether a module is of a certain type.
             This does mean that if you are looking for :class:`torch.nn.Sequential`, any subclass will also be returned.
         """
         for _, m in self.named_modules(types=types, recurse_into_matched=recurse_into_matched):
             yield m
 
     def named_modules(self, memo=None, *args, types=None, recurse_into_matched=True, **kwargs):
-        """ Overload for :func:`torch.nn.Modules.named_modules` that provides extra features. |br|
+        """
+        Overload for :func:`torch.nn.Modules.named_modules` that provides extra features. |br|
         This version of the method allows you to pass in a list of module types for which you are interested.
         Only those modules will be returned from the generator.
         Additionally, you can set `recurse_into_matched` to **False**,
         so that the generator will not yield submodules from previously matched modules.
 
         Args:
             memo (set, optional): a memo to store the set of modules already added to the result
@@ -279,20 +288,21 @@
 
         Note:
             This function will load the weights to CPU,
             so you should use ``network.to(device)`` afterwards to send it to the device of your choice.
         """
         state = torch.load(weights_file, 'cpu')
 
-        remap = ''
         if remap is not None:
             state = self.weight_remapping(state, remap)
             remap = ' remapped'
             if '_LN_MODEL_VERSION' in state:
                 del state['_LN_MODEL_VERSION']
+        else:
+            remap = ''
 
         log.info('Loading%s weights from file [%s]', remap, weights_file)
         if not strict and state.keys() != self.state_dict().keys():
             log.warning('Modules not matching, performing partial update')
 
         self.load_state_dict(state, strict=strict)
 
@@ -352,28 +362,31 @@
             log.warning('Modules not matching, performing partial update')
 
         # We already remapped versions, so run super load_state_dict straight away
         super().load_state_dict(state, strict=strict)
 
     def state_dict(self, **kwargs):
         state = super().state_dict(**kwargs)
-        state['_LN_MODEL_VERSION'] = getattr(self, 'MODEL_VERSION', 0)
+        state['_LN_MODEL_VERSION'] = torch.tensor(getattr(self, 'MODEL_VERSION', 0))
         return state
 
     def load_state_dict(self, state_dict, strict=True):
         if '_LN_MODEL_VERSION' not in state_dict:
             try:
                 # Remapped weights do not contain MODEL_VERSION
                 return super().load_state_dict(state_dict, strict=strict)
             except RuntimeError:
                 # Attempt automatic version adaptation from lightnet < 3
                 state_dict = self._remap_model_version(state_dict, 0)
                 return super().load_state_dict(state_dict, strict=strict)
         else:
             state_version = state_dict.pop('_LN_MODEL_VERSION')
+            if isinstance(state_version, torch.Tensor):
+                state_version = state_version.item()
+
             state_dict = self._remap_model_version(state_dict, state_version)
             return super().load_state_dict(state_dict, strict=strict)
 
     def _remap_model_version(self, state, version):
         model_version = getattr(self, 'MODEL_VERSION', 0)
         if version > model_version:
             raise RuntimeError(
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_anchor_yolo.py` & `lightnet-4.0.0/lightnet/data/transform/post/_anchor_yolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,28 @@
         network_stride (int): Downsampling factors of the network (most lightnet networks have a `stride` attribute)
         anchors (ln.util.Anchors): single-scale list of anchor boxes
 
     Returns:
         torch.Tensor [Boxes x 7]:
             **[batch_num, x_c, y_c, width, height, confidence, class_id]** for every bounding box
     """
-    def __init__(self, conf_thresh, network_stride, anchors):
+    def __init__(
+            self,
+            conf_thresh,
+            network_stride,
+            anchors,
+            *,
+            coord_grid_sensitivity=1,
+    ):
         super().__init__()
         self.conf_thresh = torch.tensor(conf_thresh)
         self.network_stride = torch.tensor(network_stride)
         self.num_anchors = anchors.num_anchors
         self.anchors = anchors.as_output(network_stride)
+        self.coord_grid_sensitivity = torch.tensor(coord_grid_sensitivity)
 
     def forward(self, network_output):
         device = network_output.device
         batch, channels, h, w = network_output.shape
         num_classes = (channels // self.num_anchors) - 5
 
         lin_y, lin_x = torch.meshgrid(torch.arange(h), torch.arange(w), **meshgrid_kw)
@@ -44,20 +52,23 @@
         lin_y = lin_y.reshape(-1).to(device)
         anchor_wh = self.anchors.reshape(1, self.num_anchors, 2, 1).to(device)
 
         # Compute max possible width/height network output, before the computed width/height would reach inf
         max_value = torch.tensor(1e35, dtype=network_output.dtype, device=network_output.device)
         max_value = (max_value / anchor_wh.max() / self.network_stride).log().floor()
 
+        # Grid Sensitivity
+        grid_sensitivity = -0.5 * (self.coord_grid_sensitivity - 1)
+
         # Compute xc,yc, w,h, box_score on Tensor
-        network_output = network_output.view(batch, self.num_anchors, -1, h*w)                                  # -1 == 5+num_classes (we can drop feature maps if 1 class)
-        network_output[:, :, 0, :].sigmoid_().add_(lin_x).mul_(self.network_stride)                             # X center
-        network_output[:, :, 1, :].sigmoid_().add_(lin_y).mul_(self.network_stride)                             # Y center
-        network_output[:, :, 2:4, :].clamp_(max=max_value).exp_().mul_(anchor_wh).mul_(self.network_stride)     # Width, Height
-        network_output[:, :, 4, :].sigmoid_()                                                                   # Box score
+        network_output = network_output.view(batch, self.num_anchors, -1, h*w)                                                              # -1 == 5+num_classes (we can drop feature maps if 1 class)
+        network_output[:, :, 0, :].sigmoid_().mul_(self.coord_grid_sensitivity).add_(grid_sensitivity).add_(lin_x).mul_(self.network_stride)     # X center
+        network_output[:, :, 1, :].sigmoid_().mul_(self.coord_grid_sensitivity).add_(grid_sensitivity).add_(lin_y).mul_(self.network_stride)     # Y center
+        network_output[:, :, 2:4, :].clamp_(max=max_value).exp_().mul_(anchor_wh).mul_(self.network_stride)                                 # Width, Height
+        network_output[:, :, 4, :].sigmoid_()                                                                                               # Box score
 
         # Compute class_score
         if num_classes > 1:
             with torch.no_grad():
                 cls_scores = F.softmax(network_output[:, :, 5:, :], 2)
             cls_max, cls_max_idx = torch.max(cls_scores, 2)
             cls_max_idx = cls_max_idx.float()
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_anchor_masked.py` & `lightnet-4.0.0/lightnet/data/transform/post/_anchor_masked.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_brambox.py` & `lightnet-4.0.0/lightnet/data/transform/post/_brambox.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         # Set column types
         df[['image', 'class_label']] = df[['image', 'class_label']].astype(int)
         df['id'] = np.nan
         df[['x_top_left', 'y_top_left', 'width', 'height', 'confidence']] = df[['x_top_left', 'y_top_left', 'width', 'height', 'confidence']].astype(float)
 
         # Setup class labels
         if self.class_label_map is not None:
-            df['class_label'] = df['class_label'].map({i: v for i, v in enumerate(self.class_label_map)})
+            df['class_label'] = df['class_label'].map(dict(enumerate(self.class_label_map)))
         else:
             df['class_label'] = df['class_label'].astype(str)
 
         # Setup image column
         if image_dtype is not None:
             df['image'] = pd.Categorical.from_codes(df['image'], dtype=image_dtype)
         elif self.image_map is not None:
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_base.py` & `lightnet-4.0.0/lightnet/data/transform/post/_base.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_corner.py` & `lightnet-4.0.0/lightnet/data/transform/post/_corner.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     Note:
         If setting the subsample_kernel to **0**, you disable the subsampling.
         Otherwise this post-processing will perform maxpooling on the heatmap with the specified kernel.
     """
     def __init__(self, embedding_thresh, conf_thresh, network_stride, topk=100, subsample_kernel=0):
         super().__init__()
-        warnings.warn('GetCornerBoxes is still in development. Use at your own risk!', category=FutureWarning)
+        warnings.warn('GetCornerBoxes is still in development. Use at your own risk!', category=FutureWarning, stacklevel=2)
 
         self.embedding_thresh = embedding_thresh
         self.conf_thresh = conf_thresh
         self.network_stride = network_stride
         self.topk = topk
         self.subsample_kernel = subsample_kernel
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_anchor_oriented.py` & `lightnet-4.0.0/lightnet/data/transform/post/_anchor_oriented.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_reverse_fit.py` & `lightnet-4.0.0/lightnet/data/transform/post/_reverse_fit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 #
 #   Lightnet postprocessing reverse fit
 #   Copyright EAVISE
 #
 import torch.nn as nn
 
-__all__ = ['ReverseCrop', 'ReverseLetterbox', 'ReversePad']
+__all__ = ['ReverseCrop', 'ReverseLetterbox', 'ReverseRescale', 'ReversePad']
 
 
 class ReverseCrop(nn.Module):
-    """ Performs a reverse :class:`~lightnet.data.transform.Crop` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
+    """
+    Performs a reverse :class:`~lightnet.data.transform.Crop` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
 
     Args:
         network_size (tuple): Tuple containing the width and height of the images going in the network
         image_size (tuple, callable or dict-like): Width and height of the original images (See Note)
+        group_column (str, optional): Name of the column to group by, when `image_size` is a callable or dict-like; Default **'image'**
 
     Returns:
         pandas.DataFrame: brambox dataframe.
 
     Note:
         The `image_size` argument can be one of three different types:
 
         - tuple <width, height> : The same image size will be used for the entire dataframe
-        - callable : The argument will be called with the image column name and must return a (width, height) tuple
+        - callable : The argument will be called with the `group_column` name and must return a (width, height) tuple
         - dict-like : This is similar to the callable, but instead of calling the argument, it will use dictionary accessing (self.image_size[img_name])
 
         Note that if your dimensions are the same for all images, it is faster to pass a tuple,
         as the transformation will be applied to the entire dataframe at once as opposed to grouping it per image and applying the tranform to each group individually.
 
     Warning:
         This post-processing only works when center-cropping images.
         Make sure to set the `center` argument to **True** in your :class:`~lightnet.data.transform.Crop` pre-processing.
     """
-    def __init__(self, network_size, image_size):
+    def __init__(self, network_size, image_size, *, group_column='image'):
         super().__init__()
         self.network_size = network_size
         self.image_size = image_size
+        self.group_column = group_column
 
     def forward(self, boxes):
         if isinstance(self.image_size, (list, tuple)):
             net_w, net_h = self.network_size
             im_w, im_h = self.image_size
             scale, pad = self._get_params(net_w, net_h, im_w, im_h)
             return self._transform(boxes.copy(), scale, pad)
 
-        return boxes.groupby('image', group_keys=False).apply(self._apply_transform)
+        return boxes.groupby(self.group_column, group_keys=False).apply(self._apply_transform)
 
     def _apply_transform(self, boxes):
         net_w, net_h = self.network_size
         if callable(self.image_size):
             im_w, im_h = self.image_size(boxes.name)
         else:
             im_w, im_h = self.image_size[boxes.name]
@@ -85,46 +88,49 @@
                 pad[1] * scale,
             ))
 
         return boxes
 
 
 class ReverseLetterbox(nn.Module):
-    """ Performs a reverse :class:`~lightnet.data.transform.Letterbox` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
+    """
+    Performs a reverse :class:`~lightnet.data.transform.Letterbox` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
 
     Args:
         network_size (tuple): Tuple containing the width and height of the images going in the network
         image_size (tuple, callable or dict-like): Width and height of the original images (See Note)
+        group_column (str, optional): Name of the column to group by, when `image_size` is a callable or dict-like; Default **'image'**
 
     Returns:
         pandas.DataFrame: brambox dataframe.
 
     Note:
         The `image_size` argument can be one of three different types:
 
         - tuple <width, height> : The same image size will be used for the entire dataframe
-        - callable : The argument will be called with the image column name and must return a (width, height) tuple
+        - callable : The argument will be called with the `group_column` name and must return a (width, height) tuple
         - dict-like : This is similar to the callable, but instead of calling the argument, it will use dictionary accessing (self.image_size[img_name])
 
         Note that if your dimensions are the same for all images, it is faster to pass a tuple,
         as the transformation will be applied to the entire dataframe at once as opposed to grouping it per image and applying the tranform to each group individually.
     """
-    def __init__(self, network_size, image_size):
+    def __init__(self, network_size, image_size, *, group_column='image'):
         super().__init__()
         self.network_size = network_size
         self.image_size = image_size
+        self.group_column = group_column
 
     def forward(self, boxes):
         if isinstance(self.image_size, (list, tuple)):
             net_w, net_h = self.network_size
             im_w, im_h = self.image_size
             scale, pad = self._get_params(net_w, net_h, im_w, im_h)
             return self._transform(boxes.copy(), scale, pad)
 
-        return boxes.groupby('image', group_keys=False).apply(self._apply_transform)
+        return boxes.groupby(self.group_column, group_keys=False).apply(self._apply_transform)
 
     def _apply_transform(self, boxes):
         net_w, net_h = self.network_size
         if callable(self.image_size):
             im_w, im_h = self.image_size(boxes.name)
         else:
             im_w, im_h = self.image_size[boxes.name]
@@ -160,46 +166,113 @@
                 -pad[0] * scale,
                 -pad[1] * scale,
             ))
 
         return boxes
 
 
+class ReverseRescale(nn.Module):
+    """
+    Performs a reverse :class:`~lightnet.data.transform.Rescale` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
+
+    Args:
+        network_size (tuple): Tuple containing the width and height of the images going in the network
+        image_size (tuple, callable or dict-like): Width and height of the original images (See Note)
+        group_column (str, optional): Name of the column to group by, when `image_size` is a callable or dict-like; Default **'image'**
+
+    Returns:
+        pandas.DataFrame: brambox dataframe.
+
+    Note:
+        The `image_size` argument can be one of three different types:
+
+        - tuple <width, height> : The same image size will be used for the entire dataframe
+        - callable : The argument will be called with the `group_column` name and must return a (width, height) tuple
+        - dict-like : This is similar to the callable, but instead of calling the argument, it will use dictionary accessing (self.image_size[img_name])
+
+        Note that if your dimensions are the same for all images, it is faster to pass a tuple,
+        as the transformation will be applied to the entire dataframe at once as opposed to grouping it per image and applying the tranform to each group individually.
+    """
+    def __init__(self, network_size, image_size, *, group_column='image'):
+        super().__init__()
+        self.network_size = network_size
+        self.image_size = image_size
+        self.group_column = group_column
+
+    def forward(self, boxes):
+        if isinstance(self.image_size, (list, tuple)):
+            net_w, net_h = self.network_size
+            im_w, im_h = self.image_size
+            scale = self._get_params(net_w, net_h, im_w, im_h)
+            return self._transform(boxes.copy(), scale)
+
+        return boxes.groupby(self.group_column, group_keys=False).apply(self._apply_transform)
+
+    def _apply_transform(self, boxes):
+        net_w, net_h = self.network_size
+        if callable(self.image_size):
+            im_w, im_h = self.image_size(boxes.name)
+        else:
+            im_w, im_h = self.image_size[boxes.name]
+
+        scale = self._get_params(net_w, net_h, im_w, im_h)
+        return self._transform(boxes.copy(), scale)
+
+    @staticmethod
+    def _get_params(net_w, net_h, im_w, im_h):
+        return (im_w / net_w, im_h / net_h)
+
+    @staticmethod
+    def _transform(boxes, scale):
+        boxes.x_top_left *= scale[0]
+        boxes.width *= scale[0]
+        boxes.y_top_left *= scale[1]
+        boxes.height *= scale[1]
+
+        if 'segmentation' in boxes.columns:
+            boxes['segmentation'] = boxes['segmentation'].geos.scale(*scale)
+
+        return boxes
+
+
 class ReversePad(nn.Module):
-    """ Performs a reverse :class:`~lightnet.data.transform.Pad` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
+    """
+    Performs a reverse :class:`~lightnet.data.transform.Pad` operation on the bounding boxes, so that the bounding box coordinates are relative to the original image dimensions.
 
     Args:
         network_factor (int or tuple): Tuple containing the factor the width and height need to match
         image_size (tuple, callable or dict-like): Width and height of the original images (See Note)
+        group_column (str, optional): Name of the column to group by, when `image_size` is a callable or dict-like; Default **'image'**
 
     Returns:
         pandas.DataFrame: brambox dataframe.
 
     Note:
         The `image_size` argument can be one of three different types:
 
         - tuple <width, height> : The same image size will be used for the entire dataframe
-        - callable : The argument will be called with the image column name and must return a (width, height) tuple
+        - callable : The argument will be called with the `group_column` name and must return a (width, height) tuple
         - dict-like : This is similar to the callable, but instead of calling the argument, it will use dictionary accessing (self.image_size[img_name])
 
         Note that if your dimensions are the same for all images, it is faster to pass a tuple,
         as the transformation will be applied to the entire dataframe at once as opposed to grouping it per image and applying the tranform to each group individually.
     """
-    def __init__(self, network_factor, image_size):
+    def __init__(self, network_factor, image_size, *, group_column='image'):
         super().__init__()
         self.network_factor = network_factor
         self.image_size = image_size
+        self.group_column = group_column
 
     def forward(self, boxes):
         if isinstance(self.image_size, (list, tuple)):
             im_w, im_h = self.image_size
             self._get_params(im_w, im_h)
             return self._transform(boxes.copy(), self.pad)
 
-        return boxes.groupby('image', group_keys=False).apply(self._apply_transform)
+        return boxes.groupby(self.group_column, group_keys=False).apply(self._apply_transform)
 
     def _get_params(self, im_w, im_h):
         if isinstance(self.network_factor, int):
             net_w, net_h = self.network_factor, self.network_factor
         else:
             net_w, net_h = self.network_factor
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/post/_nms.py` & `lightnet-4.0.0/lightnet/data/transform/post/_nms.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 #   Copyright EAVISE
 #
 import logging
 import numpy as np
 import torch
 import torch.nn as nn
 from torchvision.ops import batched_nms, nms
-from lightnet.util import cwh_xyxy
+from lightnet.util import cwh_xyxy, iou_xyxy
 from lightnet._imports import bb
 
 
 __all__ = ['NMS', 'NMSFast', 'NMSSoft', 'NMSSoftFast']
 log = logging.getLogger(__name__)
 
 
 class NMS(nn.Module):
-    """ Performs non-maximal suppression on the bounding boxes, filtering boxes with a high overlap.
+    """
+    Performs non-maximal suppression on the bounding boxes, filtering boxes with a high overlap.
     This function can either work on a pytorch bounding box tensor or a brambox dataframe.
 
     Args:
         iou_thresh (Number [0-1]): Overlapping threshold to filter detections with non-maxima suppresion
         class_nms (bool, optional): Whether to perform nms per class; Default **True**
         memory_limit (int, optional): Threshold to the number of bounding boxes, before taking the slower NMS path, which consumes less memory (see Warning); Default **50000**
         reset_index (bool, optional): Whether to reset the index of the returned dataframe (dataframe only); Default **True**
@@ -41,26 +42,37 @@
         The brambox dataframe should be a detection dataframe,
         as it needs the x_top_left, y_top_left, width, height, confidence and class_label columns.
         If it contains a valid geos 'segmentation' column, we compute IoU using the segmentation data.
 
     Note:
         You can disable this transformation by setting the `iou_thresh` argument to zero.
     """
-    def __init__(self, iou_thresh, *, class_nms=True, memory_limit=50000, reset_index=True, force_cpu=None, box_type=None):
+    def __init__(
+        self,
+        iou_thresh,
+        *,
+        class_nms=True,
+        diou_nms=False,
+        memory_limit=50000,
+        reset_index=True,
+        force_cpu=None,
+        box_type=None,
+    ):
         super().__init__()
         if force_cpu is not None:
             import warnings
             warnings.warn(
                 'The "force_cpu" argument is deprecated, as Lightnet now uses the cuda implementation of NMS from the torchvision package, which does not need this flag.',
                 category=DeprecationWarning,
                 stacklevel=2,
             )
 
         self.iou_thresh = iou_thresh
         self.class_nms = class_nms
+        self.diou_nms = diou_nms
         self.memory_limit = memory_limit
         self.reset_index = reset_index
         self.box_type = box_type.lower() if box_type is not None else None
 
     def forward(self, boxes):
         """ Runs NMS on the boxes.
 
@@ -74,15 +86,24 @@
             return boxes
 
         if isinstance(boxes, torch.Tensor):
             if boxes.numel() == 0:
                 return boxes
             else:
                 coords = self._torch_coords(boxes)
-                keep = self._torch_fast(coords, boxes) if boxes.shape[0] <= self.memory_limit else self._torch_slow(coords, boxes)
+                if self.diou_nms:
+                    batches = boxes[:, 0]
+                    keep = torch.empty(boxes.shape[0], dtype=torch.bool, device=boxes.device)
+                    for batch in torch.unique(batches, sorted=False):
+                        mask = batches == batch
+                        keep[mask] = self._torch_cluster(coords[mask], boxes[mask])
+                elif boxes.shape[0] <= self.memory_limit:
+                    keep = self._torch_fast(coords, boxes)
+                else:
+                    keep = self._torch_slow(coords, boxes)
                 return boxes[keep]
         else:
             return self._pandas(boxes)
 
     def _torch_coords(self, boxes):
         if (self.box_type == 'obb') or (self.box_type is None and boxes.shape[1] == 8):
             angle_abs = boxes[:, 5].abs()
@@ -119,14 +140,42 @@
                 keep[mask] = torch.scatter(keep[mask], 0, keep_idx, 1)
             else:
                 keep_idx = nms(mask_coords, mask_boxes[:, -2], self.iou_thresh)
                 keep[mask] = torch.scatter(keep[mask], 0, keep_idx, 1)
 
         return keep
 
+    def _torch_cluster(self, coords, boxes):
+        """ NMS Clustering algorithm with DIoU. """
+        # Sort coordinates by descending score
+        _, order = boxes[:, 5].sort(0, descending=True)
+        coords = coords[order]
+
+        # Compute IoU
+        ious = iou_xyxy(coords, coords, type=iou_xyxy.Types.DIoU).triu(1)
+
+        # Filter IoU based on class
+        if self.class_nms:
+            classes = boxes[order, 6]
+            same_class = (classes.unsqueeze(0) == classes.unsqueeze(1))
+            ious[~same_class] = 0
+
+        # Cluster NMS
+        B = ious
+        for _ in range(boxes.shape[0]):
+            A = B
+            maxA, _ = torch.max(A, dim=0)
+            E = (maxA <= self.iou_thresh).float().unsqueeze(1).expand_as(A)
+            B = ious.mul(E)
+            if A.equal(B):
+                break
+
+        keep = maxA <= self.iou_thresh
+        return keep.scatter(0, order, keep)
+
     @torch.jit.unused
     def _pandas(self, boxes):
         if len(boxes.index) == 0:
             return boxes
         boxes = boxes.groupby('image', group_keys=False, observed=True).apply(self._pandas_nms)
         if self.reset_index:
             return boxes.reset_index(drop=True)
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/_compose.py` & `lightnet-4.0.0/lightnet/data/transform/_compose.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,16 @@
     This is lightnet's own version of :class:`torchvision.transforms.Compose`, which has some extra bells and whistles. |br|
     The main advantage this class offers compared to the PyTorch version,
     is that this class will inspect the call signatures of the transformations and feed it the correct amount of arguments.
 
     Check out the `tutorial <../notes/02-A-basics.html#Pre-processing-pipeline>`_ for more information.
 
     Args:
-        transforms (args): A list of all your transformations in the right order.
+        transforms (*args): A list of all your transformations in the right order
+        enabled (list[bool] or bool, kw-only): Which transforms are enabled; Default **True**
 
     Example:
         Variable number of arguments:
 
         >>> tf = ln.data.transform.Compose(
         ...     # 10,20,1  -> 30,21,11
         ...     lambda a,b,c: (a+b, b+c, c+a),
@@ -167,15 +168,15 @@
             Compose [
               <disabled> RandomHSV (
                 auto_recompute_params = True,
                 hue = 1,
                 saturation = 2,
                 value = 2,
               )
-              <disabled> Letterbox [MULTI-TF] (
+              <disabled> Letterbox (
                 auto_recompute_params = True,
                 dataset = None,
                 dimension = (416, 416),
                 fill_color = 0.5,
               )
             ]
         """
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/pre/_fit.py` & `lightnet-4.0.0/lightnet/data/transform/pre/_fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from collections.abc import Sequence
 import numpy as np
 import torch
 import torch.nn.functional as F
 from lightnet._imports import cv2, Image, ImageOps, pygeos
 from ._base import ImageAnnoTransform, AnnoTransform
 
-__all__ = ['Crop', 'Letterbox', 'Pad', 'FitAnno']
+__all__ = ['Crop', 'Letterbox', 'Rescale', 'Pad', 'FitAnno']
 
 
 class Crop(ImageAnnoTransform):
-    """ Rescale and crop images/annotations to the right network dimensions.
+    """
+    Rescale and crop images/annotations to the right network dimensions.
     This transform will first rescale to the closest (bigger) dimension possible and then take a crop to the exact dimensions.
 
     Args:
         dimension (tuple, optional): Default size for the letterboxing, expressed as a (width, height) tuple; Default **None**
         dataset (lightnet.data.Dataset, optional): Dataset that uses this transform; Default **None**
         center (Boolean, optional): Whether to take the crop from the center or randomly.
         kwargs: Passed on to :class:`~lightnet.data.transform.ImageTransform`
@@ -70,15 +71,15 @@
             self._crop = (dx, dy, dx + net_w, dy + net_h)
 
     @torch.jit.unused
     def _tf_pil(self, img):
         if self._scale != 1:
             img = img.resize(
                 (int(self._scale*self._img_width+0.5), int(self._scale*self._img_height+0.5)),
-                resample=Image.BILINEAR,
+                resample=Image.Resampling.BILINEAR,
                 reducing_gap=3,
             )
 
         if self._crop is not None:
             img = img.crop(self._crop)
 
         return img
@@ -91,24 +92,32 @@
         if self._crop is not None:
             img = img[self._crop[1]:self._crop[3], self._crop[0]:self._crop[2]]
 
         return img
 
     def _tf_torch(self, img):
         if self._scale != 1:
-            if img.ndim == 3:
+            ndim = img.ndim
+            if ndim == 3:
                 img = img[None, ...]
-            elif img.ndim == 2:
+            elif ndim == 2:
                 img = img[None, None, ...]
+
             img = F.interpolate(
                 img,
                 size=(int(self._scale*self._img_height+0.5), int(self._scale*self._img_width+0.5)),
                 mode='bilinear',
                 align_corners=False,
-            ).squeeze().clamp(min=0, max=255)
+                antialias=True,
+            ).clamp(min=0, max=255)
+
+            if ndim == 3:
+                img = img.squeeze(0)
+            elif ndim == 2:
+                img = img.squeeze(0).squeeze(0)
 
         # Crop
         if self._crop is not None:
             img = img[..., self._crop[1]:self._crop[3], self._crop[0]:self._crop[2]]
 
         return img
 
@@ -140,15 +149,16 @@
                 anno['x_top_left'] -= self._crop[0]
                 anno['y_top_left'] -= self._crop[1]
 
         return anno
 
 
 class Letterbox(ImageAnnoTransform):
-    """ Rescale images/annotations and add top/bottom borders to get to the right network dimensions.
+    """
+    Rescale images/annotations and add top/bottom borders to get to the right network dimensions.
 
     Args:
         dimension (tuple, optional): Default size for the letterboxing, expressed as a (width, height) tuple; Default **None**
         dataset (lightnet.data.Dataset, optional): Dataset that uses this transform; Default **None**
         fill_color (int or float, optional): Fill color to be used for padding (if int, will be divided by 255); Default **0.5**
         kwargs: Passed on to :class:`~lightnet.data.transform.ImageTransform`
 
@@ -191,15 +201,15 @@
         self._pad = (int(pad_w), int(pad_h), int(pad_w+.5), int(pad_h+.5))
 
     @torch.jit.unused
     def _tf_pil(self, img):
         if self._scale != 1:
             img = img.resize(
                 (int(self._scale*self._img_width+0.5), int(self._scale*self._img_height+0.5)),
-                resample=Image.BILINEAR,
+                resample=Image.Resampling.BILINEAR,
                 reducing_gap=3,
             )
 
         if self._pad != (0, 0, 0, 0):
             channels = len(img.getbands())
             img = ImageOps.expand(img, border=self._pad, fill=(int(self.fill_color*255),)*channels)
 
@@ -214,24 +224,32 @@
             channels = img.shape[2] if len(img.shape) > 2 else 1
             img = cv2.copyMakeBorder(img, self._pad[1], self._pad[3], self._pad[0], self._pad[2], cv2.BORDER_CONSTANT, value=(int(self.fill_color*255),)*channels)
 
         return img
 
     def _tf_torch(self, img):
         if self._scale != 1:
-            if img.ndim == 3:
+            ndim = img.ndim
+            if ndim == 3:
                 img = img[None, ...]
-            elif img.ndim == 2:
+            elif ndim == 2:
                 img = img[None, None, ...]
+
             img = F.interpolate(
                 img,
                 size=(int(self._scale*self._img_height+0.5), int(self._scale*self._img_width+0.5)),
                 mode='bilinear',
                 align_corners=False,
-            ).squeeze().clamp(min=0, max=255)
+                antialias=True,
+            ).clamp(min=0, max=255)
+
+            if ndim == 3:
+                img = img.squeeze(0)
+            elif ndim == 2:
+                img = img.squeeze(0).squeeze(0)
 
         if self._pad != (0, 0, 0, 0):
             img = F.pad(img, (self._pad[0], self._pad[2], self._pad[1], self._pad[3]), value=self.fill_color)
 
         return img
 
     @torch.jit.unused
@@ -253,16 +271,115 @@
                 self._pad[0],
                 self._pad[1],
             ))
 
         return anno
 
 
+class Rescale(ImageAnnoTransform):
+    """
+    Rescale images/annotations to the right network dimensions.
+    This transformation effectively warps images if necessary.
+
+    Args:
+        dimension (tuple, optional): Default size for the rescaling, expressed as a (width, height) tuple; Default **None**
+        dataset (lightnet.data.Dataset, optional): Dataset that uses this transform; Default **None**
+        kwargs: Passed on to :class:`~lightnet.data.transform.ImageTransform`
+
+    Note:
+        Create 1 Rescale object and use it for both image and annotation transforms.
+        This object will save data from the image transform and use that on the annotation transform.
+    """
+    def __init__(self, dimension=None, dataset=None, **kwargs):
+        super().__init__(**kwargs)
+        self.dimension = dimension
+        self.dataset = dataset
+        if self.dimension is None and self.dataset is None:
+            raise ValueError('This transform either requires a dimension or a dataset to infer the dimension')
+
+        # Parameters
+        self._img_width = None
+        self._img_height = None
+        self._scale = None
+
+    def get_parameters(self, img_width, img_height):
+        self._img_width = img_width
+        self._img_height = img_height
+
+        if self.dataset is not None:
+            net_w, net_h = self.dataset.input_dim
+        elif isinstance(self.dimension, int):
+            net_w, net_h = self.dimension, self.dimension
+        else:
+            net_w, net_h = self.dimension
+
+        self._scale = (net_w / img_width, net_h / img_height)
+
+    @torch.jit.unused
+    def _tf_pil(self, img):
+        if self._scale != (1, 1):
+            img = img.resize(
+                (int(self._scale[0]*self._img_width+0.5), int(self._scale[1]*self._img_height+0.5)),
+                resample=Image.Resampling.BILINEAR,
+                reducing_gap=3,
+            )
+
+        return img
+
+    @torch.jit.unused
+    def _tf_cv(self, img):
+        if self._scale != (1, 1):
+            img = cv2.resize(
+                img,
+                (int(self._scale[0]*self._img_width+0.5), int(self._scale[1]*self._img_height+0.5)),
+                interpolation=cv2.INTER_LINEAR,
+            )
+
+        return img
+
+    def _tf_torch(self, img):
+        if self._scale != (1, 1):
+            ndim = img.ndim
+            if ndim == 3:
+                img = img[None, ...]
+            elif ndim == 2:
+                img = img[None, None, ...]
+
+            img = F.interpolate(
+                img,
+                size=(int(self._scale[1]*self._img_height+0.5), int(self._scale[0]*self._img_width+0.5)),
+                mode='bilinear',
+                align_corners=False,
+                antialias=True,
+            ).clamp(min=0, max=255)
+
+            if ndim == 3:
+                img = img.squeeze(0)
+            elif ndim == 2:
+                img = img.squeeze(0).squeeze(0)
+
+        return img
+
+    @torch.jit.unused
+    def _tf_anno(self, anno):
+        if self._scale != (1, 1):
+            anno['x_top_left'] *= self._scale[0]
+            anno['width'] *= self._scale[0]
+            anno['y_top_left'] *= self._scale[1]
+            anno['height'] *= self._scale[1]
+
+        if 'segmentation' in anno.columns and (self._scale != (1, 1)):
+            anno['segmentation'] = anno['segmentation'].geos.scale(*self._scale)
+
+        return anno
+
+
 class Pad(ImageAnnoTransform):
-    """ Pad images/annotations to a certain dimension.
+    """
+    Pad images/annotations to a certain dimension.
 
     Args:
         dimension (int or tuple, optional): Default size for the padding, expressed as a single integer or as a (width, height) tuple; Default **None**
         dataset (lightnet.data.Dataset, optional): Dataset that uses this transform; Default **None**
         multiple_dim (boolean, optional): Consider given dimensions to be multiples instead of exact values; Default **True**
         fill_color (int or float, optional): Fill color to be used for padding (if int, will be divided by 255); Default **0.5**
         kwargs: Passed on to :class:`~lightnet.data.transform.ImageTransform`
@@ -342,15 +459,16 @@
             if 'segmentation' in anno.columns:
                 anno['segmentation'] = anno['segmentation'].geos.translate(*self._pad)
 
         return anno
 
 
 class FitAnno(AnnoTransform):
-    """ Crop and filter annotations to fit inside of the image boundaries. |br|
+    """
+    Crop and filter annotations to fit inside of the image boundaries. |br|
     This transformation also modifies the `truncated` columns of the annotations, by computing how much of the annotation was cut off.
 
     Args:
         crop (boolean, optional): Whether to actually crop annotations to fit inside the image boundaries; Default **True**
         filter (boolean, optional): Whether to filter the annotations if they are not completely inside of the image boundaries; Default **True**
         filter_type (string, optional): How to filter ('remove' or 'ignore'); Default **remove**
         filter_threshold (number, optional): Minimal percentage of the bounding box area that still needs to be inside the image; Default **0.001**
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/pre/_base.py` & `lightnet-4.0.0/lightnet/data/transform/pre/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 #
 #   Lightnet base pre-processing operators
 #   Copyright EAVISE
 #
 import logging
 import numpy as np
 import torch
+import types
 from lightnet._imports import Image
 
 __all__ = ['ImageTransform', 'ImageAnnoTransform', 'AnnoTransform']
 log = logging.getLogger(__name__)
 
 
 class ImageTransform(torch.nn.Module):
-    """ Base transform class for the pre-processing on images. |br|
+    """
+    Base transform class for the pre-processing on images. |br|
     Any transformation that inherits from this transform, should -in theory- work with any of the following image formats:
 
     - Pillow :
       RGB or grayscale image from pillow
     - OpenCV :
       NumPy arrays with RGB or grayscale data ([H,W] or [H,W,C])
     - PyTorch :
@@ -67,15 +69,16 @@
             log.error('%s only works with <PIL images>, <OpenCV images> or <torch Tensors> [%s]', self.__class__.__name__, type(image))
 
         return image
 
     @classmethod
     @torch.jit.unused
     def apply(cls, image, **kwargs):
-        """ Classmethod that applies the transformation once.
+        """
+        Classmethod that applies the transformation once.
 
         .. deprecated:: 3.0.0
             |br| This method is deprecated. Simple create the object and run it: ``Transform(...)(image)``.
 
         Args:
             data: Data to transform (eg. image)
             **kwargs: Same arguments that are passed to the ``__init__`` function
@@ -90,15 +93,16 @@
             stacklevel=2,
         )
         obj = cls(**kwargs)
         return obj(image)
 
     @torch.jit.unused
     def get_parameters(self, img_width, img_height):
-        """ This function gets the width and height of the image and should compute the necessary transformation parameters. |br|
+        """
+        This function gets the width and height of the image and should compute the necessary transformation parameters. |br|
         The reason for separating this is to reduce code duplication and to make sure that you would perform the exact same transformation, independent of which image format you choose.
         For the :class:`~lightnet.data.transform.ImageAnnoTransform` and :class:`~lightnet.data.transform.AnnoTransform` classes,
         it is very important to store all the details about a transformation on images, as you cannot get them afterwards.
 
         Implementations should store parameters of the transform on the object itself.
         If you care about pretty string/repr formats of your transformation objects, you should start the different parameter names with an underscore (otherwise they get shown in the repr).
 
@@ -106,43 +110,46 @@
             img_width (int): The width of the image
             img_height (int): The height of the image
         """
         pass
 
     @torch.jit.unused
     def _tf_pil(self, img):
-        """ Transformation for Pillow images.
+        """
+        Transformation for Pillow images.
         Implementations should overwrite this method and provide the correct transformation.
         The default implementation raises a ``NotImplementedError``.
 
         Args:
             img (PIL.Image): Image to transform
 
         Returns:
             any: Transformed image (most commonly a ``PIL.Image``, but you could return something else)
         """
         raise NotImplementedError('This transformation is not implemented for PIL images.')
 
     @torch.jit.unused
     def _tf_cv(self, img):
-        """ Transformation for OpenCV NumPy images.
+        """
+        Transformation for OpenCV NumPy images.
         Implementations should overwrite this method and provide the correct transformation.
         The default implementation raises a ``NotImplementedError``.
 
         Args:
             img (np.ndarray): Image to transform
 
         Returns:
             any: Transformed image (most commonly a ``np.ndarray``, but you could return something else)
         """
         raise NotImplementedError('This transformation is not implemented for OpenCV NumPy images.')
 
     @torch.jit.unused
     def _tf_torch(self, img):
-        """ Transformation for PyTorch image tensors.
+        """
+        Transformation for PyTorch image tensors.
         Implementations should overwrite this method and provide the correct transformation.
         The default implementation raises a ``NotImplementedError``.
 
         Args:
             img (torch.Tensor): Image to transform
 
         Returns:
@@ -150,32 +157,35 @@
         """
         raise NotImplementedError('This transformation is not implemented for PyTorch Tensor images.')
 
     def __str__(self):
         return self.__class__.__name__
 
     def __repr__(self):
-        string = f'{self.__class__.__name__} (\n'
+        string = f'{str(self)} (\n'
 
         for name in sorted(self.__dict__.keys()):
             if name.startswith('_') or name == 'training':
                 continue
             val = self.__dict__[name]
+            if isinstance(val, types.MethodType):
+                continue
 
             valrepr = repr(val)
             if '\n' in valrepr:
                 valrepr = val.__class__.__name__
 
             string += f'  {name} = {valrepr},\n'
 
         return string + ')'
 
 
 class ImageAnnoTransform(ImageTransform):
-    """ Base transform class that for the joint pre-processing of images and annotations. |br|
+    """
+    Base transform class that for the joint pre-processing of images and annotations. |br|
     Any transformation that inherits from this transform, should -in theory- work with any of the following formats:
 
     - Pillow :
       RGB or grayscale image from pillow
     - OpenCV :
       NumPy arrays with RGB or grayscale data ([H,W] or [H,W,C])
     - PyTorch :
@@ -196,36 +206,62 @@
     - :func:`~lightnet.data.transform.ImageTransform._tf_anno` :
       Perform the transformation on a brambox (annotation) dataframe
 
     Warning:
         These transformations are all subclasses from :class:`torch.nn.Module` in order to potentially allow tracing the entire pipeline.
         When implementing this class, you should thus call ``super().__init__()`` in order to intialize it properly.
     """
+    @classmethod
+    def ImageTransform(cls, *args, **kwargs):
+        """
+        Alternative constructor which creates a variant of the transform that only modifies the image and not the annotations.
+
+        Args:
+            All arguments are forwarded to the default ``__init__`` constructor.
+
+        Note:
+            This variant gets created by overriding the forward method of the object with :func:`ImageTransform.forward`.
+        """
+        new = cls(*args, **kwargs)
+        new._VARIANT = 'img'
+        new.forward = types.MethodType(ImageTransform.forward, new)
+        return new
+
+    @classmethod
+    def AnnoTransform(cls, *args, **kwargs):
+        """
+        Alternative constructor which creates a variant of the transform that only modifies the annotations and not the image.
+
+        Args:
+            All arguments are forwarded to the default ``__init__`` constructor.
+
+        Note:
+            This variant gets created by overriding the transform methods ``_tf_pil``, ``_tf_cv`` and ``_tf_torch`` with identity functions.
+            Do note that you should still call this transform with both an image and annotations, as the image might be used in :func:`ImageAnnoTransform.get_parameters`.
+        """
+        new = cls(*args, **kwargs)
+        new._VARIANT = 'anno'
+        new._tf_pil = types.MethodType(AnnoTransform._tf_pil, new)
+        new._tf_cv = types.MethodType(AnnoTransform._tf_cv, new)
+        new._tf_torch = types.MethodType(AnnoTransform._tf_torch, new)
+        return new
+
     def forward(self, image, anno=None):
-        if isinstance(image, torch.Tensor):
-            self.get_parameters(image.shape[-1], image.shape[-2])
-            image = self._tf_torch(image)
-        elif isinstance(image, np.ndarray):
-            self.get_parameters(image.shape[1], image.shape[0])
-            image = self._tf_cv(image)
-        elif Image is not None and isinstance(image, Image.Image):
-            self.get_parameters(*image.size)
-            image = self._tf_pil(image)
-        elif image is not None:
-            log.error('%s only works with <PIL images>, <OpenCV images> or <torch Tensors> [%s]', self.__class__.__name__, type(image))
+        image = super().forward(image)
 
         if anno is None:
             return image
         else:
             anno = self._tf_anno(anno.copy())
             return image, anno
 
     @classmethod
     def apply(cls, image, anno=None, **kwargs):
-        """ Classmethod that applies the transformation once.
+        """
+        Classmethod that applies the transformation once.
 
         .. deprecated:: 3.0.0
             |br| This method is deprecated. Simple create the object and run it: ``Transform(...)(image, anno)``.
 
         Args:
             image: Image to transform
             anno (optional): ground truth for that image; Default **None**
@@ -240,15 +276,16 @@
             category=DeprecationWarning,
             stacklevel=2,
         )
         obj = cls(**kwargs)
         return obj(image, anno)
 
     def _tf_anno(self, anno):
-        """ Transformation for Brambox dataframes.
+        """
+        Transformation for Brambox dataframes.
         Implementations should overwrite this method and provide the correct transformation.
         The default implementation raises a ``NotImplementedError``.
 
         Args:
             anno (pd.DataFrame): Annotations to transform
 
         Returns:
@@ -256,34 +293,27 @@
 
         Note:
             The dataframe gets copied before passing it to this function,
             so you can freely modify the dataframe, without worrying about overwriting the original data.
         """
         raise NotImplementedError('This transformation is not implemented for brambox dataframes.')
 
-    def __repr__(self):
-        string = f'{self.__class__.__name__} [MULTI-TF] (\n'
-
-        for name in sorted(self.__dict__.keys()):
-            if name.startswith('_') or name == 'training':
-                continue
-            val = self.__dict__[name]
-
-            valrepr = repr(val)
-            if '\n' in valrepr:
-                valrepr = val.__class__.__name__
-
-            string += f'  {name} = {valrepr},\n'
+    @property
+    def __name__(self):
+        if hasattr(self, '_VARIANT'):
+            return self.__class__.__name__ + f'<{self._VARIANT}>'
+        return self.__class__.__name__
 
-        return string + ')'
+    def __str__(self):
+        return self.__name__
 
 
 class AnnoTransform(ImageAnnoTransform):
-    """ Base transform class for the pre-processing on annotations. |br|
-
+    """
+    Base transform class for the pre-processing on annotations. |br|
     When implementing this class, you should overwrite the following methods:
 
     - :func:`~lightnet.data.transform.ImageTransform.get_parameters` :
       Compute the necessary parameters for the transformation and store them on the object.
       This method is optional and depends on whether your transformation requires parameters computed from the image size.
     - :func:`~lightnet.data.transform.ImageTransform._tf_anno` :
       Perform the transformation on a brambox (annotation) dataframe
@@ -292,15 +322,16 @@
        These transformations are all subclasses from :class:`torch.nn.Module` in order to potentially allow tracing the entire pipeline. |br|
         However, this class can be used straight away and thus already has a default init function that takes a callable.
 
         This does mean that you cannot simply call ``super().__init__()``, when implementing this class.
         If you inherit from this class, you should write ``super(AnnoTransform, self).__init__()`` to call the :class:`~torch.nn.Module` initializer.
     """
     def __init__(self, fn, *, auto_recompute_params=True, **kwargs):
-        """ Instead of building your own transform with this class,
+        """
+        Instead of building your own transform with this class,
         you can also simply pass a callable object (function, lambda, etc.) as the first argument of the init function.
         The resulting object will then use this function to transform your annotation data.
 
         Args:
             fn (callable): Transformation function for your annotations.
             auto_recompute_params (bool, optional): Whether to automatically recompute augmentation parameters for each new image.
             kwargs: Extra arguments passed on to the transformation function.
@@ -332,15 +363,16 @@
         return img
 
     def _tf_torch(self, img):
         """ Simply returns the image. """
         return img
 
     def _tf_anno(self, anno):
-        """ Transformation for Brambox dataframes.
+        """
+        Transformation for Brambox dataframes.
         Implementations should overwrite this method and provide the correct transformation.
         The default implementation runs ``self.fn`` on the dataframe if it exists (see :func:`~lightnet.data.trnasform.AnnoTransform.__init__`)
         or raises a ``NotImplementedError``.
 
         Args:
             anno (pd.DataFrame): Annotations to transform
 
@@ -361,17 +393,16 @@
             else:
                 return retval
         else:
             raise NotImplementedError('This transformation is not implemented for brambox dataframes.')
 
     @property
     def __name__(self):
-        """ Return a more suitable name. """
         fn = getattr(self, 'fn', None)
         if fn is not None:
             name = getattr(fn, '__name__', None)
             if name is None:
                 name = getattr(fn, '__class__', {'__name__': None}).__name__
             if name is not None:
-                return name.lower()
+                return self.__class__.__name__ + f'<{name.lower()}>'
 
         return self.__class__.__name__
```

### Comparing `lightnet-3.1.0/lightnet/data/transform/pre/_augment.py` & `lightnet-4.0.0/lightnet/data/transform/pre/_augment.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,19 @@
         self._img_height = img_height
         self._flip_h = random.random() < self.horizontal
         self._flip_v = random.random() < self.vertical
 
     @torch.jit.unused
     def _tf_pil(self, img):
         if self._flip_h and self._flip_v:
-            img = img.transpose(Image.ROTATE_180)
+            img = img.transpose(Image.Transpose.ROTATE_180)
         elif self._flip_h:
-            img = img.transpose(Image.FLIP_LEFT_RIGHT)
+            img = img.transpose(Image.Transpose.FLIP_LEFT_RIGHT)
         elif self._flip_v:
-            img = img.transpose(Image.FLIP_TOP_BOTTOM)
+            img = img.transpose(Image.Transpose.FLIP_TOP_BOTTOM)
 
         return img
 
     @torch.jit.unused
     def _tf_cv(self, img):
         if self._flip_h and self._flip_v:
             img = cv2.flip(img, -1)
```

### Comparing `lightnet-3.1.0/lightnet/data/_dataloading.py` & `lightnet-4.0.0/lightnet/data/_dataloading.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,23 +125,23 @@
         if len(args) > 5:
             shuffle = args[2]
             sampler = args[3]
             batch_sampler = args[4]
         elif len(args) > 4:
             shuffle = args[2]
             sampler = args[3]
-            batch_sampler = kwargs.get('batch_sampler', None)
+            batch_sampler = kwargs.get('batch_sampler')
         elif len(args) > 3:
             shuffle = args[2]
-            sampler = kwargs.get('sampler', None)
-            batch_sampler = kwargs.get('batch_sampler', None)
+            sampler = kwargs.get('sampler')
+            batch_sampler = kwargs.get('batch_sampler')
         else:
             shuffle = kwargs.get('shuffle', False)
-            sampler = kwargs.get('sampler', None)
-            batch_sampler = kwargs.get('batch_sampler', None)
+            sampler = kwargs.get('sampler')
+            batch_sampler = kwargs.get('batch_sampler')
 
         # Use custom BatchSampler
         if batch_sampler is None:
             if sampler is None:
                 if shuffle:
                     sampler = torch.utils.data.sampler.RandomSampler(self.dataset)
                 else:
```

### Comparing `lightnet-3.1.0/lightnet/_log.py` & `lightnet-4.0.0/lightnet/_log.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/_base.py` & `lightnet-4.0.0/lightnet/prune/_base.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/_multi.py` & `lightnet-4.0.0/lightnet/prune/_multi.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/_l2.py` & `lightnet-4.0.0/lightnet/prune/_l2.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/_gm.py` & `lightnet-4.0.0/lightnet/prune/_gm.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/dependency/_tree.py` & `lightnet-4.0.0/lightnet/prune/dependency/_tree.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/dependency/_create.py` & `lightnet-4.0.0/lightnet/prune/dependency/_create.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/dependency/_dependency.py` & `lightnet-4.0.0/lightnet/prune/dependency/_dependency.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/prune/dependency/_type.py` & `lightnet-4.0.0/lightnet/prune/dependency/_type.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/models/_network_yolo_v2.py` & `lightnet-4.0.0/lightnet/models/_network_yolo_v2.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         input_channels (int, optional): Number of input channels; Default **3**
         anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 32
@@ -62,39 +62,39 @@
             raise ln.util.AnchorError(anchors, f'Expected {self.values_per_anchor} values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.Darknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum),
+            lnn.backbone.Darknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum),
             ['17_convbatch'],
             True,
         )
 
         self.neck = nn.ModuleList([
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
             ),
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(512, 64, 1, 1, 0, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(512, 64, 1, 1, 0, activation=activation, momentum=momentum),
                 lnn.layer.Reorg(2),
             ),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
             (4*64)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            relu=relu,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_yolt.py` & `lightnet-4.0.0/lightnet/models/_network_dyolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 #
-#   Yolt model
+#   DYolo model
 #   Copyright EAVISE
 #
 import functools
 import torch
 import torch.nn as nn
 import lightnet as ln
 import lightnet.network as lnn
 
-__all__ = ['Yolt', 'O_Yolt', 'M_Yolt']
+__all__ = ['DYolo', 'O_DYolo', 'M_DYolo']
 
 
-class Yolt(lnn.module.Lightnet):
-    """ Yolt object detector :cite:`yolt`. |br|
-    This detector is optimized for detecting small objects and is more lightweight than YoloV2.
+class DYolo(lnn.module.Lightnet):
+    """ Deconvolutional Yolo (DYolo) object detector :cite:`dyolo`. |br|
+    This detector is optimized for detecting small objects, by adding feature pyramids to Yolo V2.
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
-    stride = 16
-    inner_stride = 16
+    stride = 8
+    inner_stride = 32
     values_per_anchor = 2
     remap_darknet19 = (
-        (r'^backbone.([1-9]_.*)', r'backbone.module.\1'),    # layers 1-9
-        (r'^backbone.(1[0-7]_.*)', r'backbone.module.\1'),   # layers 10-17
+        (r'^backbone\.(.*)',   r'backbone.module.\1'),
     )
 
     MODEL_VERSION = 1
     remap_v1 = (
-        (r'^layers.3.21_convbatch.(.*)', r'head.0.\1'),
-        (r'^layers.3.22_conv.(.*)', r'head.1.\1'),
-        (r'^layers.1.18_convbatch.(.*)', r'neck.0.0.\1'),
-        (r'^layers.1.19_convbatch.(.*)', r'neck.0.1.\1'),
-        (r'^layers.0.(.*)', r'backbone.module.\1'),
-        (r'^layers.1.(.*)', r'backbone.module.\1'),
+        (r'^layers.4.27_convbatch.(.*)', r'head.0.\1'),
+        (r'^layers.4.28_conv.(.*)', r'head.1.\1'),
+        (r'^layers.2.24_deconv.(.*)', r'neck.0.\1'),
+        (r'^layers.3.25_convbatch.(.*)', r'neck.1.0.\1'),
+        (r'^layers.3.26_deconv.(.*)', r'neck.1.1.\1'),
+        (r'^layers.[012].(.*)', r'backbone.module.\1'),
     )
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
-        anchors=ln.util.Anchors.TinyYoloV2_VOC,
+        anchors=ln.util.Anchors.YoloV2_VOC,
     ):
         if not isinstance(anchors, ln.util.Anchors):
             anchors = ln.util.Anchors.from_darknet(self, anchors)
         if anchors.num_scales != 1:
             raise ln.util.AnchorError(anchors, f'Expected 1 scale, but got {anchors.num_scales}')
         if anchors.values_per_anchor != self.values_per_anchor:
             raise ln.util.AnchorError(anchors, f'Expected {self.values_per_anchor} values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            # Yolt only has the 17 first layers from the orignal Darknet19 network
-            lnn.backbone.Darknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum)[:17],
-            ['11_convbatch'],
+            lnn.backbone.Darknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum),
+            ['11_convbatch', '17_convbatch'],
             True,
         )
 
         self.neck = nn.ModuleList([
+            nn.ConvTranspose2d(1024, 512, 2, 2),
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(512+512, 512, 1, 1, 0, activation=activation, momentum=momentum),
+                nn.ConvTranspose2d(512, 512, 2, 2),
             ),
-            lnn.layer.Reorg(2),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
-            (4*256)+1024,
+            512+256,
             self.anchors.num_anchors,
             self.num_classes,
-            relu=relu,
+            512,
+            True,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
                 nn.init.constant_(mod.bias, 0)
             return True
 
         return super().__init_weights__(name, mod)
 
     def forward(self, x):
-        x, feat_11 = self.backbone(x)
+        x, feat_11, feat_17 = self.backbone(x)
 
         x = self.neck[0](x)
-        feat_11 = self.neck[1](feat_11)
+        x = self.neck[1](torch.cat((x, feat_17), 1))
 
-        x = self.head(torch.cat((feat_11, x), 1))
+        x = self.head(torch.cat((x, feat_11), 1))
 
         return x
 
 
-class O_Yolt(Yolt):
-    """ Oriented Yolt variant. |br|
-    This detector is the oriented variant of :class:`~lightnet.models.Yolt`, which can predict bounding boxes with a rotation angle.
+class O_DYolo(DYolo):
+    """ Oriented Deconvolutional YoloV2 variant. |br|
+    This detector is the oriented variant of :class:`~lightnet.models.DYolo`, which can predict bounding boxes with a rotation angle.
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC (zero angle)**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC (zero angle)**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
 
     Note:
@@ -134,74 +134,75 @@
     """
     values_per_anchor = 3
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
-        anchors=ln.util.Anchors.TinyYoloV2_VOC.append_values(0.0),
+        anchors=ln.util.Anchors.YoloV2_VOC.append_values(0.0),
     ):
         super().__init_module__(num_classes, input_channels, anchors)
 
         self.head = lnn.head.DetectionOrientedAnchor(
-            (4*256)+1024,
+            512+256,
             self.anchors.num_anchors,
             self.num_classes,
+            512,
+            True,
         )
 
 
-class M_Yolt(Yolt):
-    """ Masked Yolt variant. |br|
-    This detector is the oriented variant of :class:`~lightnet.models.Yolt`, which can predict bounding boxes, as well as instance segmentation masks.
+class M_DYolo(DYolo):
+    """ Masked Deconvolutional YoloV2 variant. |br|
+    This detector is the oriented variant of :class:`~lightnet.models.DYolo`, which can predict bounding boxes, as well as instance segmentation masks.
 
     Args:
         num_classes (int): Number of classes
-        num_masks (int, optional): Number of prototype masks; Default **32**
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
-        self.stride: Subsampling factor of the network bounding box output (input_dim / output_dim)
+        self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.mask_stride: Subsampling factor of the network mask output (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
-    mask_stride = 8
+    mask_stride = 4
 
     def __init_module__(
         self,
         num_classes,
         num_masks=32,
         input_channels=3,
-        anchors=ln.util.Anchors.TinyYoloV2_VOC,
+        anchors=ln.util.Anchors.YoloV2_VOC,
     ):
         super().__init_module__(num_classes, input_channels, anchors)
         self.num_masks = num_masks
 
         self.detection_head = lnn.head.DetectionMaskedAnchor(
-            (4*256)+1024,
+            512+256,
             self.anchors.num_anchors,
             num_classes,
             num_masks,
         )
 
         self.mask_head = lnn.head.DetectionMaskedAnchor.Protonet(
-            (4*256)+1024,
+            512+256,
             num_masks,
         )
 
     def forward(self, x):
-        x, feat_11 = self.backbone(x)
+        x, feat_11, feat_17 = self.backbone(x)
 
         x = self.neck[0](x)
-        feat_11 = self.neck[1](feat_11)
+        x = self.neck[1](torch.cat((x, feat_17), 1))
         x = torch.cat((feat_11, x), 1)
 
         out = self.detection_head(x)
         mask = self.mask_head(x)
 
         return out, mask
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_tiny_yolo_v2.py` & `lightnet-4.0.0/lightnet/models/_network_mobilenet_yolo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,100 @@
 #
-#   Darknet Tiny YOLOv2 model
+#   Darknet YOLOv2 model with Mobilenet backend
 #   Copyright EAVISE
 #
 import functools
+import torch
 import torch.nn as nn
 import lightnet as ln
 import lightnet.network as lnn
 
-__all__ = ['TinyYoloV2']
+__all__ = ['MobilenetYolo']
 
 
-class TinyYoloV2(lnn.module.Darknet):
-    """ Tiny Yolo v2 implementation :cite:`yolo_v2`.
+class MobilenetYolo(lnn.module.Lightnet):
+    """ Yolo v2 implementation with a mobilenet v1 backend.
 
     Args:
         num_classes (int): Number of classes
+        alpha (float, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_darknet: Remapping rules for weights from the :class:`~lightnet.models.Darknet` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_mobilenet_v1: Remapping rules for weights from the :class:`~lightnet.models.MobileNetV1` model.
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
+
+    Warning:
+        When changing the ``alpha`` value, you are changing the network architecture.
+        This means you cannot use weights from this network with a different alpha value.
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 32
     inner_stride = 32
-    remap_darknet = (
-        (r'^backbone\.(.*)',   r'backbone.\1'),
+    remap_mobilenet_v1 = (
+        (r'^backbone\.(.*)',   r'backbone.module.\1'),
     )
 
     MODEL_VERSION = 1
     remap_v1 = (
-        (r'^layers.13_convbatch.(.*)', r'head.1.\1'),
-        (r'^layers.14_convbatch.(.*)', r'head.2.\1'),
-        (r'^layers.15_conv.(.*)', r'head.3.\1'),
-        (r'^layers.(.*)', r'backbone.\1'),
+        (r'^layers.0.(.*)', r'backbone.module.\1'),
+        (r'^layers.1.(.*)', r'backbone.module.\1'),
+        (r'^layers.2.15_convbatch.(.*)', r'neck.0.\1'),
+        (r'^layers.3.17_convbatch.(.*)', r'head.0.\1'),
+        (r'^layers.3.18_conv.(.*)', r'head.1.\1'),
     )
 
     def __init_module__(
         self,
         num_classes,
+        alpha=1.0,
         input_channels=3,
-        anchors=ln.util.Anchors.TinyYoloV2_VOC,
+        anchors=ln.util.Anchors.YoloV2_VOC,
     ):
         if not isinstance(anchors, ln.util.Anchors):
             anchors = ln.util.Anchors.from_darknet(self, anchors)
         if anchors.num_scales != 1:
             raise ln.util.AnchorError(anchors, f'Expected 1 scale, but got {anchors.num_scales}')
         if anchors.values_per_anchor != 2:
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
-        self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
-        momentum = 0.01
+        activation = functools.partial(nn.ReLU6, inplace=True)
+        momentum = 0.1
 
-        self.backbone = lnn.backbone.Darknet(input_channels, 512, relu=relu, momentum=momentum)
-        self.head = nn.Sequential(
-            lnn.layer.PaddedMaxPool2d(2, 1, (0, 1, 0, 1)),
-            lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-            *lnn.head.DetectionYoloAnchor(
-                1024,
-                self.anchors.num_anchors,
-                self.num_classes,
-                relu=relu,
-                momentum=momentum,
-            ),
+        self.backbone = lnn.layer.FeatureExtractor(
+            lnn.backbone.Mobilenet(input_channels, int(alpha*1024), alpha, activation=activation, momentum=momentum),
+            ['9_convdw'],
+            True,
         )
 
-    def __init_weights__(self, name, mod):
-        if isinstance(mod, nn.Conv2d):
-            nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
-            if mod.bias is not None:
-                nn.init.constant_(mod.bias, 0)
-            return True
+        self.neck = nn.Sequential(
+            lnn.layer.Conv2dBatchAct(int(alpha*512), 64, 1, 1, 0, activation=activation, momentum=momentum),
+            lnn.layer.Reorg(2),
+        )
 
-        return super().__init_weights__(name, mod)
+        self.head = lnn.head.DetectionYoloAnchor(
+            (4*64)+int(alpha*1024),
+            self.anchors.num_anchors,
+            self.num_classes,
+            activation=activation,
+            momentum=momentum,
+        )
 
     def forward(self, x):
-        x = self.backbone(x)
-        x = self.head(x)
+        x, feat_9 = self.backbone(x)
+
+        feat_9 = self.neck(feat_9)
+
+        x = self.head(torch.cat((feat_9, x), 1))
 
         return x
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_tiny_yolo_v3.py` & `lightnet-4.0.0/lightnet/models/_network_tiny_yolo_v3.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         input_channels (int, optional): Number of input channels; Default **3**
         anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV3 COCO**
 
     Attributes:
         self.stride: Subsampling factors of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet: Remapping rules for weights from the `~lightnet.models.Darknet` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Warning:
         The :class:`~lightnet.network.loss.MultiScaleRegionLoss` and :class:`~lightnet.data.transform.GetMultiScaleBoundingBoxes`
         do not implement the overlapping class labels of the original implementation.
         Your weight files from darknet will thus not have the same accuracies as in darknet itself.
 
     Note:
@@ -67,50 +67,50 @@
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.Darknet(input_channels, 512, relu=relu, momentum=momentum),
+            lnn.backbone.Darknet(input_channels, 512, activation=activation, momentum=momentum),
             ['9_convbatch'],
             True,
         )
 
         self.neck = lnn.layer.FeatureExtractor(
             nn.Sequential(
                 lnn.layer.PaddedMaxPool2d(2, 1, (0, 1, 0, 1)),
-                lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dBatchReLU(1024, 256, 1, 1, 0, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 256, 1, 1, 0, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum),
                 nn.Upsample(scale_factor=2, mode='nearest'),
             ),
             [2],
             True,
         )
 
         self.head = nn.ModuleList([
             lnn.head.DetectionYoloAnchor(
                 256,
                 self.anchors.get_scale(0).num_anchors,
                 self.num_classes,
                 512,
-                relu=relu,
+                activation=activation,
                 momentum=momentum,
             ),
             lnn.head.DetectionYoloAnchor(
                 128+256,
                 self.anchors.get_scale(1).num_anchors,
                 self.num_classes,
                 256,
-                relu=relu,
+                activation=activation,
                 momentum=momentum,
             ),
         ])
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobilenet_v2.py` & `lightnet-4.0.0/lightnet/models/_network_mobilenet_v2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 class MobilenetV2(lnn.module.Lightnet):
     """ Mobilenet v2 classification network implementation :cite:`mobilenet_v2`.
 
     Args:
         num_classes (int): Number of classes
         alpha (int, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
         input_channels (int, optional): Number of input channels; Default **3**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Warning:
         When changing the ``alpha`` value, you are changing the network architecture.
         This means you cannot use weights from this network with a different alpha value.
 
     Note:
         The average pooling is implemented with an :class:`~torch.nn.AdaptiveAvgPool2d` layer. |br|
@@ -41,21 +42,22 @@
     )
 
     def __init_module__(
         self,
         num_classes,
         alpha=1,
         input_channels=3,
+        dropout=0.5,
     ):
         self.num_classes = num_classes
         self.alpha = alpha
         self.input_channels = input_channels
 
         # Network
         self.backbone = lnn.backbone.Mobilenet.V2(input_channels, int(alpha*1280), alpha)
-        self.head = lnn.head.ClassificationConv(int(alpha*1280), num_classes, dropout=True)
+        self.head = lnn.head.ClassificationConv(int(alpha*1280), num_classes, dropout=dropout)
 
     def forward(self, x):
         x = self.backbone(x)
         x = self.head(x)
 
         return x
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_dyolo.py` & `lightnet-4.0.0/lightnet/models/_network_yolt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,130 +1,130 @@
 #
-#   DYolo model
+#   Yolt model
 #   Copyright EAVISE
 #
 import functools
 import torch
 import torch.nn as nn
 import lightnet as ln
 import lightnet.network as lnn
 
-__all__ = ['DYolo', 'O_DYolo', 'M_DYolo']
+__all__ = ['Yolt', 'O_Yolt', 'M_Yolt']
 
 
-class DYolo(lnn.module.Lightnet):
-    """ Deconvolutional Yolo (DYolo) object detector :cite:`dyolo`. |br|
-    This detector is optimized for detecting small objects, by adding feature pyramids to Yolo V2.
+class Yolt(lnn.module.Lightnet):
+    """ Yolt object detector :cite:`yolt`. |br|
+    This detector is optimized for detecting small objects and is more lightweight than YoloV2.
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
-    stride = 8
-    inner_stride = 32
+    stride = 16
+    inner_stride = 16
     values_per_anchor = 2
     remap_darknet19 = (
-        (r'^backbone\.(.*)',   r'backbone.module.\1'),
+        (r'^backbone.([1-9]_.*)', r'backbone.module.\1'),    # layers 1-9
+        (r'^backbone.(1[0-7]_.*)', r'backbone.module.\1'),   # layers 10-17
     )
 
     MODEL_VERSION = 1
     remap_v1 = (
-        (r'^layers.4.27_convbatch.(.*)', r'head.0.\1'),
-        (r'^layers.4.28_conv.(.*)', r'head.1.\1'),
-        (r'^layers.2.24_deconv.(.*)', r'neck.0.\1'),
-        (r'^layers.3.25_convbatch.(.*)', r'neck.1.0.\1'),
-        (r'^layers.3.26_deconv.(.*)', r'neck.1.1.\1'),
-        (r'^layers.[012].(.*)', r'backbone.module.\1'),
+        (r'^layers.3.21_convbatch.(.*)', r'head.0.\1'),
+        (r'^layers.3.22_conv.(.*)', r'head.1.\1'),
+        (r'^layers.1.18_convbatch.(.*)', r'neck.0.0.\1'),
+        (r'^layers.1.19_convbatch.(.*)', r'neck.0.1.\1'),
+        (r'^layers.0.(.*)', r'backbone.module.\1'),
+        (r'^layers.1.(.*)', r'backbone.module.\1'),
     )
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
-        anchors=ln.util.Anchors.YoloV2_VOC,
+        anchors=ln.util.Anchors.TinyYoloV2_VOC,
     ):
         if not isinstance(anchors, ln.util.Anchors):
             anchors = ln.util.Anchors.from_darknet(self, anchors)
         if anchors.num_scales != 1:
             raise ln.util.AnchorError(anchors, f'Expected 1 scale, but got {anchors.num_scales}')
         if anchors.values_per_anchor != self.values_per_anchor:
             raise ln.util.AnchorError(anchors, f'Expected {self.values_per_anchor} values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.Darknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum),
-            ['11_convbatch', '17_convbatch'],
+            # Yolt only has the 17 first layers from the orignal Darknet19 network
+            lnn.backbone.Darknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum)[:17],
+            ['11_convbatch'],
             True,
         )
 
         self.neck = nn.ModuleList([
-            nn.ConvTranspose2d(1024, 512, 2, 2),
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(512+512, 512, 1, 1, 0, relu=relu, momentum=momentum),
-                nn.ConvTranspose2d(512, 512, 2, 2),
+                lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
             ),
+            lnn.layer.Reorg(2),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
-            512+256,
+            (4*256)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            512,
-            True,
-            relu=relu,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
                 nn.init.constant_(mod.bias, 0)
             return True
 
         return super().__init_weights__(name, mod)
 
     def forward(self, x):
-        x, feat_11, feat_17 = self.backbone(x)
+        x, feat_11 = self.backbone(x)
 
         x = self.neck[0](x)
-        x = self.neck[1](torch.cat((x, feat_17), 1))
+        feat_11 = self.neck[1](feat_11)
 
-        x = self.head(torch.cat((x, feat_11), 1))
+        x = self.head(torch.cat((feat_11, x), 1))
 
         return x
 
 
-class O_DYolo(DYolo):
-    """ Oriented Deconvolutional YoloV2 variant. |br|
-    This detector is the oriented variant of :class:`~lightnet.models.DYolo`, which can predict bounding boxes with a rotation angle.
+class O_Yolt(Yolt):
+    """ Oriented Yolt variant. |br|
+    This detector is the oriented variant of :class:`~lightnet.models.Yolt`, which can predict bounding boxes with a rotation angle.
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC (zero angle)**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC (zero angle)**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
 
     Note:
@@ -134,75 +134,74 @@
     """
     values_per_anchor = 3
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
-        anchors=ln.util.Anchors.YoloV2_VOC.append_values(0.0),
+        anchors=ln.util.Anchors.TinyYoloV2_VOC.append_values(0.0),
     ):
         super().__init_module__(num_classes, input_channels, anchors)
 
         self.head = lnn.head.DetectionOrientedAnchor(
-            512+256,
+            (4*256)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            512,
-            True,
         )
 
 
-class M_DYolo(DYolo):
-    """ Masked Deconvolutional YoloV2 variant. |br|
-    This detector is the oriented variant of :class:`~lightnet.models.DYolo`, which can predict bounding boxes, as well as instance segmentation masks.
+class M_Yolt(Yolt):
+    """ Masked Yolt variant. |br|
+    This detector is the oriented variant of :class:`~lightnet.models.Yolt`, which can predict bounding boxes, as well as instance segmentation masks.
 
     Args:
         num_classes (int): Number of classes
+        num_masks (int, optional): Number of prototype masks; Default **32**
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
 
     Attributes:
-        self.stride: Subsampling factor of the network (input_dim / output_dim)
+        self.stride: Subsampling factor of the network bounding box output (input_dim / output_dim)
         self.mask_stride: Subsampling factor of the network mask output (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
-    mask_stride = 4
+    mask_stride = 8
 
     def __init_module__(
         self,
         num_classes,
         num_masks=32,
         input_channels=3,
-        anchors=ln.util.Anchors.YoloV2_VOC,
+        anchors=ln.util.Anchors.TinyYoloV2_VOC,
     ):
         super().__init_module__(num_classes, input_channels, anchors)
         self.num_masks = num_masks
 
         self.detection_head = lnn.head.DetectionMaskedAnchor(
-            512+256,
+            (4*256)+1024,
             self.anchors.num_anchors,
             num_classes,
             num_masks,
         )
 
         self.mask_head = lnn.head.DetectionMaskedAnchor.Protonet(
-            512+256,
+            (4*256)+1024,
             num_masks,
         )
 
     def forward(self, x):
-        x, feat_11, feat_17 = self.backbone(x)
+        x, feat_11 = self.backbone(x)
 
         x = self.neck[0](x)
-        x = self.neck[1](torch.cat((x, feat_17), 1))
+        feat_11 = self.neck[1](feat_11)
         x = torch.cat((feat_11, x), 1)
 
         out = self.detection_head(x)
         mask = self.mask_head(x)
 
         return out, mask
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_alexnet.py` & `lightnet-4.0.0/lightnet/models/_network_alexnet.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class Alexnet(lnn.module.Lightnet):
     """ Alexnet implementation :cite:`alexnet`.
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_torchvision: Remapping rules for weights from the `torchvision implementation <torchvision_>`_.
 
     .. _torchvision: https://pytorch.org/hub/pytorch_vision_alexnet
     """
@@ -32,20 +33,21 @@
         (r'^classifier.6.(.*)', r'head.8.\1'),
     )
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
+        dropout=0.5,
     ):
         self.num_classes = num_classes
         self.input_channels = input_channels
 
         # Network
         self.backbone = lnn.backbone.Alexnet(input_channels, 256)
-        self.head = lnn.head.ClassificationFC(256, num_classes, pooling_size=6, inter_channels=4096, dropout_first=True)
+        self.head = lnn.head.ClassificationFC(256, num_classes, pooling_size=6, inter_channels=4096, dropout=dropout, dropout_first=True)
 
     def forward(self, x):
         x = self.backbone(x)
         x = self.head(x)
 
         return x
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_yolact.py` & `lightnet-4.0.0/lightnet/models/_network_yolact.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         num_classes,
         num_masks,
         aspect_ratios,
         scales,
         input_channels,
         inference_only=False,
     ):
-        warnings.warn('Yolact is still in development. Use at your own risk!', category=FutureWarning)
+        warnings.warn('Yolact is still in development. Use at your own risk!', category=FutureWarning, stacklevel=2)
 
         self.num_classes = num_classes
         self.num_masks = num_masks
         self.input_channels = input_channels
         self.aspect_ratios = aspect_ratios
         self.scales = scales
         self.inference_only = inference_only
@@ -45,15 +45,15 @@
             True,
         )
 
         self.neck = lnn.layer.FPN(
             [512, 1024, 2048],
             256,
             5,
-            make_prediction=lambda ci, co: lnn.layer.Conv2dReLU(ci, co, 3, 1, 1, bias=True),
+            make_prediction=lambda ci, co: lnn.layer.Conv2dAct(ci, co, 3, 1, 1, bias=True),
             make_downsample=lambda ci, co: nn.Conv2d(ci, co, 3, 2, 1, bias=True),
             interpolation_mode='bilinear',
         )
 
         self.detection_head = lnn.head.DetectionYolact(256, len(self.aspect_ratios), num_classes, num_masks)
         self.mask_head = lnn.head.DetectionYolact.Protonet(256, num_masks)
         if not inference_only:
```

### Comparing `lightnet-3.1.0/lightnet/models/__init__.py` & `lightnet-4.0.0/lightnet/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 # Datasets
 from ._dataset_brambox import *
 from ._dataset_darknet import *
 
 # Classification
 from ._network_alexnet import *
+from ._network_cspdarknet53 import *
 from ._network_darknet import *
 from ._network_darknet19 import *
 from ._network_darknet53 import *
 from ._network_mobilenet_v1 import *
 from ._network_mobilenet_v2 import *
 from ._network_resnet import *
 from ._network_vgg import *
@@ -22,14 +23,15 @@
 from ._network_mobile_darknet19 import *
 
 # Yolo
 from ._network_tiny_yolo_v2 import *
 from ._network_tiny_yolo_v3 import *
 from ._network_yolo_v2 import *
 from ._network_yolo_v3 import *
+from ._network_yolo_v4 import *
 from ._network_yolt import *
 from ._network_dyolo import *
 
 # Eavise Yolo
 from ._network_mobilenet_yolo import *
 from ._network_mobile_yolo_v2 import *
 from ._network_mobile_yolo_v2_upsample import *
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_vgg.py` & `lightnet-4.0.0/lightnet/models/_network_vgg.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,22 +13,23 @@
 
     def __init_module__(
         self,
         Backbone,
         num_classes,
         input_channels=3,
         batch_norm=False,
+        dropout=0.5,
     ):
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.batch_norm = batch_norm
 
         # Network
         self.backbone = Backbone(input_channels, 512, batch_norm=batch_norm)
-        self.head = lnn.head.ClassificationFC(512, num_classes, pooling_size=7, inter_channels=4096)
+        self.head = lnn.head.ClassificationFC(512, num_classes, pooling_size=7, inter_channels=4096, dropout=dropout)
 
     def forward(self, x):
         x = self.backbone(x)
         x = self.head(x)
 
         return x
 
@@ -62,93 +63,101 @@
     """ VGG11 implementation :cite:`vgg`. |br|
     This is configuration A from the paper.
 
     Args:
         num_classes (Number, optional): Number of classes; Default **1000**
         input_channels (Number, optional): Number of input channels; Default **3**
         batch_norm (bool, optional): Whether are not to have batchnorm after each convolution; Default **False**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_torchvision: Remapping rules for weights from the `torchvision implementation <torchvision_>`_.
 
     .. _torchvision: https://pytorch.org/hub/pytorch_vision_vgg
     """
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         batch_norm=False,
+        dropout=0.5,
     ):
-        super().__init_module__(lnn.backbone.VGG.A, num_classes, input_channels, batch_norm)
+        super().__init_module__(lnn.backbone.VGG.A, num_classes, input_channels, batch_norm, dropout)
 
 
 class VGG13(VGG):
     """ VGG13 implementation :cite:`vgg`. |br|
     This is configuration B from the paper.
 
     Args:
         num_classes (Number, optional): Number of classes; Default **1000**
         input_channels (Number, optional): Number of input channels; Default **3**
         batch_norm (bool, optional): Whether are not to have batchnorm after each convolution; Default **False**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_torchvision: Remapping rules for weights from the `torchvision implementation <torchvision_>`_.
 
     .. _torchvision: https://pytorch.org/hub/pytorch_vision_vgg
     """
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         batch_norm=False,
+        dropout=0.5,
     ):
-        super().__init_module__(lnn.backbone.VGG.B, num_classes, input_channels, batch_norm)
+        super().__init_module__(lnn.backbone.VGG.B, num_classes, input_channels, batch_norm, dropout)
 
 
 class VGG16(VGG):
     """ VGG16 implementation :cite:`vgg`. |br|
     This is configuration D from the paper.
 
     Args:
         num_classes (Number, optional): Number of classes; Default **1000**
         input_channels (Number, optional): Number of input channels; Default **3**
         batch_norm (bool, optional): Whether are not to have batchnorm after each convolution; Default **False**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_torchvision: Remapping rules for weights from the `torchvision implementation <torchvision_>`_.
 
     .. _torchvision: https://pytorch.org/hub/pytorch_vision_vgg
     """
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         batch_norm=False,
+        dropout=0.5,
     ):
-        super().__init_module__(lnn.backbone.VGG.D, num_classes, input_channels, batch_norm)
+        super().__init_module__(lnn.backbone.VGG.D, num_classes, input_channels, batch_norm, dropout)
 
 
 class VGG19(VGG):
     """ VGG19 implementation :cite:`vgg`. |br|
     This is configuration E from the paper.
 
     Args:
         num_classes (Number, optional): Number of classes; Default **1000**
         input_channels (Number, optional): Number of input channels; Default **3**
         batch_norm (bool, optional): Whether are not to have batchnorm after each convolution; Default **False**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_torchvision: Remapping rules for weights from the `torchvision implementation <torchvision_>`_.
 
     .. _torchvision: https://pytorch.org/hub/pytorch_vision_vgg
     """
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         batch_norm=False,
+        dropout=0.5,
     ):
-        super().__init_module__(lnn.backbone.VGG.E, num_classes, input_channels, batch_norm)
+        super().__init_module__(lnn.backbone.VGG.E, num_classes, input_channels, batch_norm, dropout)
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_yolo_fusion.py` & `lightnet-4.0.0/lightnet/models/_network_yolo_fusion.py`

 * *Files 25% similar despite different names*

```diff
@@ -57,77 +57,77 @@
         self.anchors = anchors
         self.input_channels = input_channels
         self.fusion_channels = fusion_channels
         self.fuse_layer = fuse_layer
         self.fuse_seq = None
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         # First layer
         if fuse_layer == 0:
             self.fuse_seq = 0
             self.layers = [
                 nn.Sequential(OrderedDict([
                     ('fuse', nn.Conv2d(input_channels+fusion_channels, input_channels, 1, 1, 0, bias=False)),
-                    ('1_convbatch', lnn.layer.Conv2dBatchReLU(input_channels, 32, 3, 1, 1, relu=relu, momentum=momentum)),
+                    ('1_convbatch', lnn.layer.Conv2dBatchAct(input_channels, 32, 3, 1, 1, activation=activation, momentum=momentum)),
                 ])),
             ]
         elif fuse_layer == 1:
             self.fuse_seq = 0
             self.layers = [
                 nn.ModuleDict({
-                    '1_convbatch_regular': lnn.layer.Conv2dBatchReLU(input_channels, 32, 3, 1, 1, relu=relu, momentum=momentum),
-                    '1_convbatch_fusion': lnn.layer.Conv2dBatchReLU(fusion_channels, 32, 3, 1, 1, relu=relu, momentum=momentum),
+                    '1_convbatch_regular': lnn.layer.Conv2dBatchAct(input_channels, 32, 3, 1, 1, activation=activation, momentum=momentum),
+                    '1_convbatch_fusion': lnn.layer.Conv2dBatchAct(fusion_channels, 32, 3, 1, 1, activation=activation, momentum=momentum),
                     'fuse': nn.Conv2d(32*2, 32, 1, 1, 0, bias=False),
                 }),
             ]
         else:
             self.layers = [
                 nn.ModuleDict({
-                    '1_convbatch_regular': lnn.layer.Conv2dBatchReLU(input_channels, 32, 3, 1, 1, relu=relu, momentum=momentum),
-                    '1_convbatch_fusion': lnn.layer.Conv2dBatchReLU(fusion_channels, 32, 3, 1, 1, relu=relu, momentum=momentum),
+                    '1_convbatch_regular': lnn.layer.Conv2dBatchAct(input_channels, 32, 3, 1, 1, activation=activation, momentum=momentum),
+                    '1_convbatch_fusion': lnn.layer.Conv2dBatchAct(fusion_channels, 32, 3, 1, 1, activation=activation, momentum=momentum),
                 }),
             ]
 
         # Main layers
         layer_list = [
             OrderedDict([
                 ('2_max',           nn.MaxPool2d(2, 2)),
-                ('3_convbatch',     lnn.layer.Conv2dBatchReLU(32, 64, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('3_convbatch',     lnn.layer.Conv2dBatchAct(32, 64, 3, 1, 1, activation=activation, momentum=momentum)),
                 ('4_max',           nn.MaxPool2d(2, 2)),
-                ('5_convbatch',     lnn.layer.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('6_convbatch',     lnn.layer.Conv2dBatchReLU(128, 64, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('7_convbatch',     lnn.layer.Conv2dBatchReLU(64, 128, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('5_convbatch',     lnn.layer.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('6_convbatch',     lnn.layer.Conv2dBatchAct(128, 64, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('7_convbatch',     lnn.layer.Conv2dBatchAct(64, 128, 3, 1, 1, activation=activation, momentum=momentum)),
                 ('8_max',           nn.MaxPool2d(2, 2)),
-                ('9_convbatch',     lnn.layer.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('10_convbatch',    lnn.layer.Conv2dBatchReLU(256, 128, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('11_convbatch',    lnn.layer.Conv2dBatchReLU(128, 256, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('9_convbatch',     lnn.layer.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('10_convbatch',    lnn.layer.Conv2dBatchAct(256, 128, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('11_convbatch',    lnn.layer.Conv2dBatchAct(128, 256, 3, 1, 1, activation=activation, momentum=momentum)),
                 ('12_max',          nn.MaxPool2d(2, 2)),
-                ('13_convbatch',    lnn.layer.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('14_convbatch',    lnn.layer.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('15_convbatch',    lnn.layer.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('16_convbatch',    lnn.layer.Conv2dBatchReLU(512, 256, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('17_convbatch',    lnn.layer.Conv2dBatchReLU(256, 512, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('13_convbatch',    lnn.layer.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('14_convbatch',    lnn.layer.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('15_convbatch',    lnn.layer.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('16_convbatch',    lnn.layer.Conv2dBatchAct(512, 256, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('17_convbatch',    lnn.layer.Conv2dBatchAct(256, 512, 3, 1, 1, activation=activation, momentum=momentum)),
             ]),
 
             OrderedDict([
                 ('18_max',          nn.MaxPool2d(2, 2)),
-                ('19_convbatch',    lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('20_convbatch',    lnn.layer.Conv2dBatchReLU(1024, 512, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('21_convbatch',    lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('22_convbatch',    lnn.layer.Conv2dBatchReLU(1024, 512, 1, 1, 0, relu=relu, momentum=momentum)),
-                ('23_convbatch',    lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('24_convbatch',    lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
-                ('25_convbatch',    lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('19_convbatch',    lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('20_convbatch',    lnn.layer.Conv2dBatchAct(1024, 512, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('21_convbatch',    lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('22_convbatch',    lnn.layer.Conv2dBatchAct(1024, 512, 1, 1, 0, activation=activation, momentum=momentum)),
+                ('23_convbatch',    lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('24_convbatch',    lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
+                ('25_convbatch',    lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
             ]),
 
             OrderedDict([
-                ('26_convbatch',    lnn.layer.Conv2dBatchReLU((4*64)+1024, 1024, 3, 1, 1, relu=relu, momentum=momentum)),
+                ('26_convbatch',    lnn.layer.Conv2dBatchAct((4*64)+1024, 1024, 3, 1, 1, activation=activation, momentum=momentum)),
                 ('27_conv',         nn.Conv2d(1024, self.anchors.num_anchors*(5+self.num_classes), 1, 1, 0)),
             ]),
         ]
         i = 1
         for e, l in enumerate(layer_list, 1):
             if fuse_layer - i <= 0:
                 fuse = None
@@ -143,22 +143,22 @@
         if self.fuse_seq is None:
             raise ValueError(f'Fuse_layer too high [{fuse_layer}/{sum(len(l) for l in layer_list)+1}]')
 
         # Passthrough layer
         if self.fuse_seq <= 2:
             self.layers.append(nn.Sequential(
                 OrderedDict([
-                    ('P1_convbatch',    lnn.layer.Conv2dBatchReLU(512, 64, 1, 1, 0, relu=relu, momentum=momentum)),
+                    ('P1_convbatch',    lnn.layer.Conv2dBatchAct(512, 64, 1, 1, 0, activation=activation, momentum=momentum)),
                     ('P2_reorg',        lnn.layer.Reorg(2)),
                 ]),
             ))
         else:
             self.layers.append(lnn.layer.FusionSequential(
                 OrderedDict([
-                    ('P1_convbatch',    lnn.layer.Conv2dBatchReLU(512, 64, 1, 1, 0, relu=relu, momentum=momentum)),
+                    ('P1_convbatch',    lnn.layer.Conv2dBatchAct(512, 64, 1, 1, 0, activation=activation, momentum=momentum)),
                     ('P2_reorg',        lnn.layer.Reorg(2)),
                 ]),
                 3,
             ))
 
         self.layers = nn.ModuleList(self.layers)
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_cornernet.py` & `lightnet-4.0.0/lightnet/models/_network_cornernet.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,29 +24,29 @@
         input_channels (int, optional): Number of input channels; Default **3**
         inference_only (boolean, optional): Whether to load the model purely for inference; Default **False**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_princeton_vl: Remapping rules for weights from the `official CornerNet implementation <cornernetImpl_>`_.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     .. _cornernetImpl: https://github.com/princeton-vl/CornerNet-Lite
     """
+    MODEL_VERSION = 1
     stride = 4
     inner_stride = 128
-    MODEL_VERSION = 1
 
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         inference_only=False,
     ):
-        warnings.warn('Cornernet is still in development. Use at your own risk!', category=FutureWarning)
+        warnings.warn('Cornernet is still in development. Use at your own risk!', category=FutureWarning, stacklevel=2)
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.inference_only = inference_only
 
         # Network
         self.backbone = lnn.layer.FeatureExtractor(
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobile_yolo_v2_upsample.py` & `lightnet-4.0.0/lightnet/models/_network_mobile_yolo_v2_upsample.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         input_channels (int, optional): Number of input channels; Default **3**
         anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_mobile_darknet19: Remapping rules for weights from the :class:`~lightnet.models.MobileDarknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 16
@@ -66,37 +66,37 @@
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.MobileDarknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum),
+            lnn.backbone.MobileDarknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum),
             ['13_convdw'],
             True,
         )
 
         self.neck = nn.ModuleList([
             nn.Sequential(
-                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
                 torch.nn.Upsample(scale_factor=2, mode='nearest'),
             ),
-            lnn.layer.Conv2dBatchReLU(512, 4*64, 1, 1, 0, relu=relu, momentum=momentum),
+            lnn.layer.Conv2dBatchAct(512, 4*64, 1, 1, 0, activation=activation, momentum=momentum),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
             (4*64)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            relu=relu,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobilenet_yolo.py` & `lightnet-4.0.0/lightnet/models/_network_tiny_yolo_v2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,100 +1,93 @@
 #
-#   Darknet YOLOv2 model with Mobilenet backend
+#   Darknet Tiny YOLOv2 model
 #   Copyright EAVISE
 #
 import functools
-import torch
 import torch.nn as nn
 import lightnet as ln
 import lightnet.network as lnn
 
-__all__ = ['MobilenetYolo']
+__all__ = ['TinyYoloV2']
 
 
-class MobilenetYolo(lnn.module.Lightnet):
-    """ Yolo v2 implementation with a mobilenet v1 backend.
+class TinyYoloV2(lnn.module.Darknet):
+    """ Tiny Yolo v2 implementation :cite:`yolo_v2`.
 
     Args:
         num_classes (int): Number of classes
-        alpha (float, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
         input_channels (int, optional): Number of input channels; Default **3**
-        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
+        anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet Tiny YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_mobilenet_v1: Remapping rules for weights from the :class:`~lightnet.models.MobileNetV1` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
-
-    Warning:
-        When changing the ``alpha`` value, you are changing the network architecture.
-        This means you cannot use weights from this network with a different alpha value.
+        self.remap_darknet: Remapping rules for weights from the :class:`~lightnet.models.Darknet` model.
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 32
     inner_stride = 32
-    remap_mobilenet_v1 = (
-        (r'^backbone\.(.*)',   r'backbone.module.\1'),
+    remap_darknet = (
+        (r'^backbone\.(.*)',   r'backbone.\1'),
     )
 
     MODEL_VERSION = 1
     remap_v1 = (
-        (r'^layers.0.(.*)', r'backbone.module.\1'),
-        (r'^layers.1.(.*)', r'backbone.module.\1'),
-        (r'^layers.2.15_convbatch.(.*)', r'neck.0.\1'),
-        (r'^layers.3.17_convbatch.(.*)', r'head.0.\1'),
-        (r'^layers.3.18_conv.(.*)', r'head.1.\1'),
+        (r'^layers.13_convbatch.(.*)', r'head.1.\1'),
+        (r'^layers.14_convbatch.(.*)', r'head.2.\1'),
+        (r'^layers.15_conv.(.*)', r'head.3.\1'),
+        (r'^layers.(.*)', r'backbone.\1'),
     )
 
     def __init_module__(
         self,
         num_classes,
-        alpha=1.0,
         input_channels=3,
-        anchors=ln.util.Anchors.YoloV2_VOC,
+        anchors=ln.util.Anchors.TinyYoloV2_VOC,
     ):
         if not isinstance(anchors, ln.util.Anchors):
             anchors = ln.util.Anchors.from_darknet(self, anchors)
         if anchors.num_scales != 1:
             raise ln.util.AnchorError(anchors, f'Expected 1 scale, but got {anchors.num_scales}')
         if anchors.values_per_anchor != 2:
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
+        self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.ReLU6, inplace=True)
-        momentum = 0.1
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        momentum = 0.01
 
-        self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.Mobilenet(input_channels, int(alpha*1024), alpha, relu=relu, momentum=momentum),
-            ['9_convdw'],
-            True,
+        self.backbone = lnn.backbone.Darknet(input_channels, 512, activation=activation, momentum=momentum)
+        self.head = nn.Sequential(
+            lnn.layer.PaddedMaxPool2d(2, 1, (0, 1, 0, 1)),
+            lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+            *lnn.head.DetectionYoloAnchor(
+                1024,
+                self.anchors.num_anchors,
+                self.num_classes,
+                activation=activation,
+                momentum=momentum,
+            ),
         )
 
-        self.neck = nn.Sequential(
-            lnn.layer.Conv2dBatchReLU(int(alpha*512), 64, 1, 1, 0, relu=relu, momentum=momentum),
-            lnn.layer.Reorg(2),
-        )
+    def __init_weights__(self, name, mod):
+        if isinstance(mod, nn.Conv2d):
+            nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
+            if mod.bias is not None:
+                nn.init.constant_(mod.bias, 0)
+            return True
 
-        self.head = lnn.head.DetectionYoloAnchor(
-            (4*64)+int(alpha*1024),
-            self.anchors.num_anchors,
-            self.num_classes,
-            relu=relu,
-            momentum=momentum,
-        )
+        return super().__init_weights__(name, mod)
 
     def forward(self, x):
-        x, feat_9 = self.backbone(x)
-
-        feat_9 = self.neck(feat_9)
-
-        x = self.head(torch.cat((feat_9, x), 1))
+        x = self.backbone(x)
+        x = self.head(x)
 
         return x
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_darknet19.py` & `lightnet-4.0.0/lightnet/models/_network_darknet19.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
     """
     inner_stride = 32
 
     MODEL_VERSION = 1
     remap_v1 = (
         (r'^layers.0.(.*)', r'backbone.\1'),
         (r'^layers.1.24_conv.(.*)', r'head.0.\1'),
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_darknet53.py` & `lightnet-4.0.0/lightnet/models/_network_darknet53.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
     """
     inner_stride = 32
 
     MODEL_VERSION = 1
     remap_v1 = (
         (r'^layers.a_residual.3_\w+.(.*)', r'backbone.3_residual.0.\1'),
         (r'^layers.a_residual.4_\w+.(.*)', r'backbone.3_residual.1.\1'),
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_yolo_v2_upsample.py` & `lightnet-4.0.0/lightnet/models/_network_yolo_v2_upsample.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         input_channels (int, optional): Number of input channels; Default **3**
         anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_darknet19: Remapping rules for weights from the :class:`~lightnet.models.Darknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 16
@@ -66,39 +66,39 @@
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.Darknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum),
+            lnn.backbone.Darknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum),
             ['17_convbatch'],
             True,
         )
 
         self.neck = nn.ModuleList([
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dBatchReLU(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
                 torch.nn.Upsample(scale_factor=2, mode='nearest'),
             ),
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(512, 4*64, 1, 1, 0, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(512, 4*64, 1, 1, 0, activation=activation, momentum=momentum),
             ),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
             (4*64)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            relu=relu,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_resnet_yolo.py` & `lightnet-4.0.0/lightnet/models/_network_resnet_yolo.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,17 +104,17 @@
         if self.type == NetworkTypes.MODULATED:
             Backbone = lnn.backbone.ModulatedResnet
         elif self.type == NetworkTypes.DEFORMABLE:
             Backbone = lnn.backbone.DeformableResnet
         else:
             Backbone = lnn.backbone.Resnet
 
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         self.backbone = lnn.layer.FeatureExtractor(
-            Backbone.RN_50(input_channels, 2048, relu=relu),
+            Backbone.RN_50(input_channels, 2048, activation=activation),
             ['6_residualgroup', '8_residualgroup'],
             True,
         )
 
         # Neck
         self.neck = self._create_neck(self.outputs)
 
@@ -126,15 +126,15 @@
         for idx, enabled in enumerate(self.outputs):
             if enabled:
                 self.head[str(idx - head_idx_start)] = lnn.head.DetectionYoloAnchor(
                     256,
                     self.anchors.get_scale(scale_idx).num_anchors,
                     self.num_classes,
                     512,
-                    relu=relu,
+                    activation=activation,
                 )
 
                 scale_idx += 1
                 any_enabled = True
             elif not any_enabled:
                 head_idx_start += 1
 
@@ -161,15 +161,15 @@
         num_outputs -= end
 
         return lnn.layer.FPN(
             [512, 1024, 2048],
             256,
             num_outputs=num_outputs,
             start_output=start_output,
-            make_prediction=lambda ci, co: lnn.layer.Conv2dReLU(ci, co, 3, 1, 1, bias=True),
+            make_prediction=lambda ci, co: lnn.layer.Conv2dAct(ci, co, 3, 1, 1, bias=True),
             make_downsample=lambda ci, co: nn.Conv2d(ci, co, 3, 2, 1, bias=True),
         )
 
     def forward(self, x):
         C5, C3, C4 = self.backbone(x)
         neck = self.neck(C3, C4, C5)[::-1]
         outputs = [head(neck[int(idx)]) for idx, head in self.head.items()]
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobilenet_v1.py` & `lightnet-4.0.0/lightnet/models/_network_mobilenet_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 class MobilenetV1(lnn.module.Lightnet):
     """ Mobilenet v1 classification network implementation :cite:`mobilenet_v1`.
 
     Args:
         num_classes (int): Number of classes
         alpha (int, optional): Number between [0-1] that controls the number of filters of the mobilenet convolutions; Default **1**
         input_channels (int, optional): Number of input channels; Default **3**
+        dropout (float, optional): Probability of the dropout layers in the classification head; Default **0.5**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Warning:
         When changing the ``alpha`` value, you are changing the network architecture.
         This means you cannot use weights from this network with a different alpha value.
 
     Note:
         The average pooling is implemented with an :class:`~torch.nn.AdaptiveAvgPool2d` layer. |br|
@@ -41,21 +42,22 @@
     )
 
     def __init_module__(
         self,
         num_classes,
         alpha=1,
         input_channels=3,
+        dropout=0.5,
     ):
         self.num_classes = num_classes
         self.alpha = alpha
         self.input_channels = input_channels
 
         # Network
         self.backbone = lnn.backbone.Mobilenet(input_channels, int(alpha*1024), alpha)
-        self.head = lnn.head.ClassificationConv(int(alpha*1024), num_classes, dropout=True)
+        self.head = lnn.head.ClassificationConv(int(alpha*1024), num_classes, dropout=dropout)
 
     def forward(self, x):
         x = self.backbone(x)
         x = self.head(x)
 
         return x
```

### Comparing `lightnet-3.1.0/lightnet/models/_dataset_brambox.py` & `lightnet-4.0.0/lightnet/models/_dataset_brambox.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobile_darknet19.py` & `lightnet-4.0.0/lightnet/models/_network_mobile_darknet19.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
     """
     inner_stride = 32
 
     MODEL_VERSION = 1
     remap_v1 = (
         (r'^layers.0.(.*)', r'backbone.\1'),
         (r'^layers.1.20_conv.(.*)', r'head.0.\1'),
```

### Comparing `lightnet-3.1.0/lightnet/models/_dataset_darknet.py` & `lightnet-4.0.0/lightnet/models/_dataset_darknet.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/models/_network_darknet.py` & `lightnet-4.0.0/lightnet/models/_network_darknet.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     Args:
         num_classes (int): Number of classes
         input_channels (int, optional): Number of input channels; Default **3**
 
     Attributes:
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
     """
     inner_stride = 64
 
     MODEL_VERSION = 1
     remap_v1 = (
         (r'^layers.0.13\w+.(.*)', r'head.1.\1'),
         (r'^layers.0.(.*)', r'backbone.\1'),
@@ -34,21 +34,21 @@
         num_classes,
         input_channels=3,
     ):
         self.num_classes = num_classes
         self.input_channels = input_channels
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
-        self.backbone = lnn.backbone.Darknet(input_channels, 512, relu=relu, momentum=momentum)
+        self.backbone = lnn.backbone.Darknet(input_channels, 512, activation=activation, momentum=momentum)
         self.head = nn.Sequential(
             nn.MaxPool2d(2, 2),
-            lnn.layer.Conv2dBatchReLU(512, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+            lnn.layer.Conv2dBatchAct(512, 1024, 3, 1, 1, activation=activation, momentum=momentum),
             *lnn.head.ClassificationConv(1024, num_classes),
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_cornernet_squeeze.py` & `lightnet-4.0.0/lightnet/models/_network_cornernet_squeeze.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,65 +24,29 @@
         input_channels (int, optional): Number of input channels; Default **3**
         inference_only (boolean, optional): Whether to load the model purely for inference; Default **False**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_princeton_vl: Remapping rules for weights from the `official CornerNet implementation <cornernetImpl_>`_.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     .. _cornernetImpl: https://github.com/princeton-vl/CornerNet-Lite
     """
+    MODEL_VERSION = 1
     stride = 8
     inner_stride = 128
 
-    MODEL_VERSION = 1
-    remap_v1 = [
-        (r'^extractor\.(.*)', r'backbone.module.\1'),
-        (r'^detector.(.*?).13_(.*)', r'head.\1.1_\2'),
-        (r'^detector.(.*?).14_(.*)', r'head.\1.2_\2'),
-        (r'^detector.(.*?).15_(.*)', r'head.\1.3_\2'),
-        (r'^detector.(.*?).17_(.*)', r'head.\1.5_\2'),
-        (r'^detector.(.*?).18_(.*)', r'head.\1.6_\2'),
-        (r'^detector.(.*?).20_(.*)', r'head.\1.8_\2'),
-        (r'^detector.(.*?).21_(.*)', r'head.\1.9_\2'),
-        (r'^detector.(.*?).23_(.*)', r'head.\1.11_\2'),
-        (r'^detector.(.*?).24_(.*)', r'head.\1.1_\2'),
-        (r'^detector.(.*?).25_(.*)', r'head.\1.2_\2'),
-        (r'^detector.(.*?).26_(.*)', r'head.\1.3_\2'),
-        (r'^detector.(.*?).28_(.*)', r'head.\1.5_\2'),
-        (r'^detector.(.*?).29_(.*)', r'head.\1.6_\2'),
-        (r'^detector.(.*?).31_(.*)', r'head.\1.8_\2'),
-        (r'^detector.(.*?).32_(.*)', r'head.\1.9_\2'),
-        (r'^detector.(.*?).34_(.*)', r'head.\1.11_\2'),
-        (r'^intermediate.(.*?).35_(.*)', r'inter_head.\1.1_\2'),
-        (r'^intermediate.(.*?).36_(.*)', r'inter_head.\1.2_\2'),
-        (r'^intermediate.(.*?).37_(.*)', r'inter_head.\1.3_\2'),
-        (r'^intermediate.(.*?).39_(.*)', r'inter_head.\1.5_\2'),
-        (r'^intermediate.(.*?).40_(.*)', r'inter_head.\1.6_\2'),
-        (r'^intermediate.(.*?).42_(.*)', r'inter_head.\1.8_\2'),
-        (r'^intermediate.(.*?).43_(.*)', r'inter_head.\1.9_\2'),
-        (r'^intermediate.(.*?).45_(.*)', r'inter_head.\1.11_\2'),
-        (r'^intermediate.(.*?).46_(.*)', r'inter_head.\1.1_\2'),
-        (r'^intermediate.(.*?).47_(.*)', r'inter_head.\1.2_\2'),
-        (r'^intermediate.(.*?).48_(.*)', r'inter_head.\1.3_\2'),
-        (r'^intermediate.(.*?).50_(.*)', r'inter_head.\1.5_\2'),
-        (r'^intermediate.(.*?).51_(.*)', r'inter_head.\1.6_\2'),
-        (r'^intermediate.(.*?).53_(.*)', r'inter_head.\1.8_\2'),
-        (r'^intermediate.(.*?).54_(.*)', r'inter_head.\1.9_\2'),
-        (r'^intermediate.(.*?).56_(.*)', r'inter_head.\1.11_\2'),
-    ]
-
     def __init_module__(
         self,
         num_classes,
         input_channels=3,
         inference_only=False,
     ):
-        warnings.warn('CornernetSqueeze is still in development. Use at your own risk!', category=FutureWarning)
+        warnings.warn('CornernetSqueeze is still in development. Use at your own risk!', category=FutureWarning, stacklevel=2)
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.inference_only = inference_only
 
         # Network
         self.backbone = lnn.layer.FeatureExtractor(
```

### Comparing `lightnet-3.1.0/lightnet/models/_network_mobile_yolo_v2.py` & `lightnet-4.0.0/lightnet/models/_network_mobile_yolo_v2.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         input_channels (int, optional): Number of input channels; Default **3**
         anchors (ln.util.Anchors, optional): single-scale list of anchor boxes; Default **Darknet YoloV2 VOC**
 
     Attributes:
         self.stride: Subsampling factor of the network (input_dim / output_dim)
         self.inner_stride: Maximal internal subsampling factor of the network (input dimension should be a multiple of this)
         self.remap_mobile_darknet19: Remapping rules for weights from the :class:`~lightnet.models.MobileDarknet19` model.
-        self.remap_v1: Remapping rules for weights from yolt models before lightnet v3.0.0
+        self.remap_v1: Remapping rules for weightfiles created with lightnet prior to v3.0.0
 
     Note:
         The preferred way to pass anchors is to use the :class:`~lightnet.util.Anchors`.
         However, for compatibility reasons, you can also pass in a list of tuples,
         which will be interpreted as darknet anchors (relative to output dimensions).
     """
     stride = 32
@@ -61,39 +61,39 @@
             raise ln.util.AnchorError(anchors, f'Expected 2 values per anchor, but got {anchors.values_per_anchor}')
 
         self.num_classes = num_classes
         self.input_channels = input_channels
         self.anchors = anchors
 
         # Network
-        relu = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
+        activation = functools.partial(nn.LeakyReLU, 0.1, inplace=True)
         momentum = 0.01
 
         self.backbone = lnn.layer.FeatureExtractor(
-            lnn.backbone.MobileDarknet.DN_19(input_channels, 1024, relu=relu, momentum=momentum),
+            lnn.backbone.MobileDarknet.DN_19(input_channels, 1024, activation=activation, momentum=momentum),
             ['13_convdw'],
             True,
         )
 
         self.neck = nn.ModuleList([
             nn.Sequential(
-                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
-                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
+                lnn.layer.Conv2dDepthWise(1024, 1024, 3, 1, 1, activation=activation, momentum=momentum),
             ),
             nn.Sequential(
-                lnn.layer.Conv2dBatchReLU(512, 64, 1, 1, 0, relu=relu, momentum=momentum),
+                lnn.layer.Conv2dBatchAct(512, 64, 1, 1, 0, activation=activation, momentum=momentum),
                 lnn.layer.Reorg(2),
             ),
         ])
 
         self.head = lnn.head.DetectionYoloAnchor(
             (4*64)+1024,
             self.anchors.num_anchors,
             self.num_classes,
-            relu=relu,
+            activation=activation,
             momentum=momentum,
         )
 
     def __init_weights__(self, name, mod):
         if isinstance(mod, nn.Conv2d):
             nn.init.kaiming_normal_(mod.weight, nonlinearity='leaky_relu', a=0.1)
             if mod.bias is not None:
```

### Comparing `lightnet-3.1.0/lightnet/engine/_parameter.py` & `lightnet-4.0.0/lightnet/engine/_parameter.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet/engine/_engine.py` & `lightnet-4.0.0/lightnet/engine/_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     def to_object(self, engine):
         new = self.__class__(self.type, engine)
         new.hooks = {k: v.to_object(engine) for k, v in self.hooks.items()}
         return new
 
     def copy(self):
         new = self.__class__(self.type, self.__engine)
-        new.hooks = {k: v for k, v in self.hooks.items()}
+        new.hooks = dict(self.hooks)
         return new
 
     def register(self, hook):
         self.hooks[hook.id] = hook
 
     def remove(self, hook):
         if hook.id not in self.hooks:
@@ -131,16 +131,25 @@
             hook = Hook(self.type, idx, fn)
             self.register(hook)
             return hook
 
         return wrapper
 
     def __call__(self, fn):
+        """
+        .. deprecated:: 3.0.0
+            |br| Calling Engine.<hook_type>(number) if deprecated, use Engine.<hook_type>[::number].
+        """
         if isinstance(fn, int):
-            log.deprecated(f'Calling Engine.{self.type}(number) is deprecated, use Engine.{self.type}[::number]')
+            import warnings
+            warnings.warn(
+                f'Calling Engine.{self.type}(number) is deprecated, use Engine.{self.type}[::number]',
+                category=DeprecationWarning,
+                stacklevel=2,
+            )
             return self[::fn]
         elif callable(fn):
             return self[::1](fn)
         else:
             raise TypeError('HookSetter should be called with a callable object')
```

### Comparing `lightnet-3.1.0/lightnet/engine/_scheduler.py` & `lightnet-4.0.0/lightnet/engine/_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/PKG-INFO` & `lightnet-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: lightnet
-Version: 3.1.0
+Version: 4.0.0
 Summary: Building blocks for recreating darknet networks in pytorch
-Home-page: UNKNOWN
 Author: EAVISE
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: segment
 Provides-Extra: training
 License-File: LICENSE
 
 <img src="https://gitlab.com/EAVISE/lightnet/raw/master/docs/.static/lightnet-long.png" alt="Logo" width="100%">  
 
@@ -41,17 +38,18 @@
 Then clone this repository and run one of the following commands:
 ```bash
 # If you just want to use Lightnet
 pip install brambox   # Optional (needed for training)
 pip install .
 
 # If you want to develop Lightnet
+pip install pillow opencv-python
 pip install -r develop.txt
 ```
-> This project is python 3.6 and higher so on some systems you might want to use 'pip3.6' instead of 'pip'
+> This project is python 3.7 and higher so on some systems you might want to use 'pip3.7' instead of 'pip'
 
 ## How to use
 [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation and guides on how to use this library.  
 The _examples_ folder contains code snippets to train and test networks with lightnet. For examples on how to implement your own networks, you can take a look at the files in _lightnet/models_.
 >If you are using a different version than the latest,
 >you can generate the documentation yourself by running `make clean html` in the _docs_ folder.
 >This does require some dependencies, like Sphinx.
@@ -74,21 +72,19 @@
 - [Tanguy Ophoff](https://gitlab.com/0phoff)
 - [Jon Crall](https://gitlab.com/Erotemic)
 - [Cedric Gullentops](https://github.com/CedricGullentops)
 
 
 [version-badge]: https://img.shields.io/pypi/v/lightnet.svg?label=version
 [doc-badge]: https://img.shields.io/badge/-Documentation-9B59B6.svg
-[python-badge]: https://img.shields.io/badge/Python-min%203.6%20%7C%20rec%203.9-FFD43B.svg
-[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.9.0-F05732.svg
+[python-badge]: https://img.shields.io/badge/Python-min%203.7%20%7C%20rec%203.9-FFD43B.svg
+[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.13.0-F05732.svg
 [pipeline-badge]: https://gitlab.com/EAVISE/lightnet/badges/master/pipeline.svg
 [release-url]: https://gitlab.com/EAVISE/lightnet/tags
 [documentation-url]: https://eavise.gitlab.io/lightnet
 [python-url]: https://python.org
 [pytorch-url]: https://pytorch.org
 [pipeline-url]: https://pypi.org/project/lightnet
 [voc-badge]: https://img.shields.io/badge/repository-Pascal%20VOC-%2300BFD8
 [voc-url]: https://gitlab.com/eavise/top/voc
 [coco-badge]: https://img.shields.io/badge/repository-MS%20COCO-%2300BFD8
 [coco-url]: https://gitlab.com/eavise/top/coco
-
-
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1 Name: lightnet Version: 3.1.0 Summary: Building blocks
-for recreating darknet networks in pytorch Home-page: UNKNOWN Author: EAVISE
-License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown
-Provides-Extra: segment Provides-Extra: training License-File: LICENSE
-[Logo]Building blocks to recreate Darknet networks in Pytorch [![Version]
-[version-badge]][release-url] [![Documentation][doc-badge]][documentation-url]
-[![Pipeline][pipeline-badge]][pipeline-url] _[_K_o_-_F_i_][![Python][python-badge]]
-[python-url] [![PyTorch][pytorch-badge]][pytorch-url] [![VOC][voc-badge]][voc-
-url] [![COCO][coco-badge]][coco-url] ## Why another framework [pytorch-yolo2]
-(https://github.com/marvis/pytorch-yolo2) is working perfectly fine, but does
-not easily allow a user to modify an existing network. This is why I decided to
-create a library, that gives the user all the necessary building blocks, to
-recreate any darknet network. This library has everything you need to control
-your network, weight loading & saving, datasets, dataloaders and data
-augmentation. Where it started as library to recreate the darknet networks in
-PyTorch, it has since grown into a more general purpose single-shot object
-detection library. ## Installing First install [PyTorch and Torchvision](https:
-//pytorch.org/get-started/locally). Then clone this repository and run one of
-the following commands: ```bash # If you just want to use Lightnet pip install
-brambox # Optional (needed for training) pip install . # If you want to develop
-Lightnet pip install -r develop.txt ``` > This project is python 3.6 and higher
-so on some systems you might want to use 'pip3.6' instead of 'pip' ## How to
-use [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation
-and guides on how to use this library. The _examples_ folder contains code
-snippets to train and test networks with lightnet. For examples on how to
-implement your own networks, you can take a look at the files in _lightnet/
-models_. >If you are using a different version than the latest, >you can
-generate the documentation yourself by running `make clean html` in the _docs_
-folder. >This does require some dependencies, like Sphinx. >The easiest way to
-install them is by using the __-r develop.txt__ option when installing
-lightnet. ## Cite If you use Lightnet in your research, please cite it. ```
-@misc{lightnet18, author = {Tanguy Ophoff}, title = {Lightnet: Building Blocks
-to Recreate Darknet Networks in Pytorch}, howpublished = {\url{https://
-gitlab.com/EAVISE/lightnet}}, year = {2018} } ``` ## Main Contributors Here is
-a list of people that made noteworthy contributions and helped to get this
-project where it stands today! - [Tanguy Ophoff](https://gitlab.com/0phoff) -
-[Jon Crall](https://gitlab.com/Erotemic) - [Cedric Gullentops](https://
-github.com/CedricGullentops) [version-badge]: https://img.shields.io/pypi/v/
+Metadata-Version: 2.1 Name: lightnet Version: 4.0.0 Summary: Building blocks
+for recreating darknet networks in pytorch Author: EAVISE Description-Content-
+Type: text/markdown Provides-Extra: segment Provides-Extra: training License-
+File: LICENSE [Logo]Building blocks to recreate Darknet networks in Pytorch [!
+[Version][version-badge]][release-url] [![Documentation][doc-badge]]
+[documentation-url] [![Pipeline][pipeline-badge]][pipeline-url] _[_K_o_-_F_i_][!
+[Python][python-badge]][python-url] [![PyTorch][pytorch-badge]][pytorch-url] [!
+[VOC][voc-badge]][voc-url] [![COCO][coco-badge]][coco-url] ## Why another
+framework [pytorch-yolo2](https://github.com/marvis/pytorch-yolo2) is working
+perfectly fine, but does not easily allow a user to modify an existing network.
+This is why I decided to create a library, that gives the user all the
+necessary building blocks, to recreate any darknet network. This library has
+everything you need to control your network, weight loading & saving, datasets,
+dataloaders and data augmentation. Where it started as library to recreate the
+darknet networks in PyTorch, it has since grown into a more general purpose
+single-shot object detection library. ## Installing First install [PyTorch and
+Torchvision](https://pytorch.org/get-started/locally). Then clone this
+repository and run one of the following commands: ```bash # If you just want to
+use Lightnet pip install brambox # Optional (needed for training) pip install .
+# If you want to develop Lightnet pip install pillow opencv-python pip install
+-r develop.txt ``` > This project is python 3.7 and higher so on some systems
+you might want to use 'pip3.7' instead of 'pip' ## How to use [Click Here]
+(https://eavise.gitlab.io/lightnet) for the API documentation and guides on how
+to use this library. The _examples_ folder contains code snippets to train and
+test networks with lightnet. For examples on how to implement your own
+networks, you can take a look at the files in _lightnet/models_. >If you are
+using a different version than the latest, >you can generate the documentation
+yourself by running `make clean html` in the _docs_ folder. >This does require
+some dependencies, like Sphinx. >The easiest way to install them is by using
+the __-r develop.txt__ option when installing lightnet. ## Cite If you use
+Lightnet in your research, please cite it. ``` @misc{lightnet18, author =
+{Tanguy Ophoff}, title = {Lightnet: Building Blocks to Recreate Darknet
+Networks in Pytorch}, howpublished = {\url{https://gitlab.com/EAVISE/
+lightnet}}, year = {2018} } ``` ## Main Contributors Here is a list of people
+that made noteworthy contributions and helped to get this project where it
+stands today! - [Tanguy Ophoff](https://gitlab.com/0phoff) - [Jon Crall](https:
+//gitlab.com/Erotemic) - [Cedric Gullentops](https://github.com/
+CedricGullentops) [version-badge]: https://img.shields.io/pypi/v/
 lightnet.svg?label=version [doc-badge]: https://img.shields.io/badge/-
 Documentation-9B59B6.svg [python-badge]: https://img.shields.io/badge/Python-
-min%203.6%20%7C%20rec%203.9-FFD43B.svg [pytorch-badge]: https://img.shields.io/
-badge/PyTorch-1.9.0-F05732.svg [pipeline-badge]: https://gitlab.com/EAVISE/
+min%203.7%20%7C%20rec%203.9-FFD43B.svg [pytorch-badge]: https://img.shields.io/
+badge/PyTorch-1.13.0-F05732.svg [pipeline-badge]: https://gitlab.com/EAVISE/
 lightnet/badges/master/pipeline.svg [release-url]: https://gitlab.com/EAVISE/
 lightnet/tags [documentation-url]: https://eavise.gitlab.io/lightnet [python-
 url]: https://python.org [pytorch-url]: https://pytorch.org [pipeline-url]:
 https://pypi.org/project/lightnet [voc-badge]: https://img.shields.io/badge/
 repository-Pascal%20VOC-%2300BFD8 [voc-url]: https://gitlab.com/eavise/top/voc
 [coco-badge]: https://img.shields.io/badge/repository-MS%20COCO-%2300BFD8
 [coco-url]: https://gitlab.com/eavise/top/coco
```

### Comparing `lightnet-3.1.0/LICENSE` & `lightnet-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/lightnet.egg-info/PKG-INFO` & `lightnet-4.0.0/lightnet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 Metadata-Version: 2.1
 Name: lightnet
-Version: 3.1.0
+Version: 4.0.0
 Summary: Building blocks for recreating darknet networks in pytorch
-Home-page: UNKNOWN
 Author: EAVISE
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: segment
 Provides-Extra: training
 License-File: LICENSE
 
 <img src="https://gitlab.com/EAVISE/lightnet/raw/master/docs/.static/lightnet-long.png" alt="Logo" width="100%">  
 
@@ -41,17 +38,18 @@
 Then clone this repository and run one of the following commands:
 ```bash
 # If you just want to use Lightnet
 pip install brambox   # Optional (needed for training)
 pip install .
 
 # If you want to develop Lightnet
+pip install pillow opencv-python
 pip install -r develop.txt
 ```
-> This project is python 3.6 and higher so on some systems you might want to use 'pip3.6' instead of 'pip'
+> This project is python 3.7 and higher so on some systems you might want to use 'pip3.7' instead of 'pip'
 
 ## How to use
 [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation and guides on how to use this library.  
 The _examples_ folder contains code snippets to train and test networks with lightnet. For examples on how to implement your own networks, you can take a look at the files in _lightnet/models_.
 >If you are using a different version than the latest,
 >you can generate the documentation yourself by running `make clean html` in the _docs_ folder.
 >This does require some dependencies, like Sphinx.
@@ -74,21 +72,19 @@
 - [Tanguy Ophoff](https://gitlab.com/0phoff)
 - [Jon Crall](https://gitlab.com/Erotemic)
 - [Cedric Gullentops](https://github.com/CedricGullentops)
 
 
 [version-badge]: https://img.shields.io/pypi/v/lightnet.svg?label=version
 [doc-badge]: https://img.shields.io/badge/-Documentation-9B59B6.svg
-[python-badge]: https://img.shields.io/badge/Python-min%203.6%20%7C%20rec%203.9-FFD43B.svg
-[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.9.0-F05732.svg
+[python-badge]: https://img.shields.io/badge/Python-min%203.7%20%7C%20rec%203.9-FFD43B.svg
+[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.13.0-F05732.svg
 [pipeline-badge]: https://gitlab.com/EAVISE/lightnet/badges/master/pipeline.svg
 [release-url]: https://gitlab.com/EAVISE/lightnet/tags
 [documentation-url]: https://eavise.gitlab.io/lightnet
 [python-url]: https://python.org
 [pytorch-url]: https://pytorch.org
 [pipeline-url]: https://pypi.org/project/lightnet
 [voc-badge]: https://img.shields.io/badge/repository-Pascal%20VOC-%2300BFD8
 [voc-url]: https://gitlab.com/eavise/top/voc
 [coco-badge]: https://img.shields.io/badge/repository-MS%20COCO-%2300BFD8
 [coco-url]: https://gitlab.com/eavise/top/coco
-
-
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
-Metadata-Version: 2.1 Name: lightnet Version: 3.1.0 Summary: Building blocks
-for recreating darknet networks in pytorch Home-page: UNKNOWN Author: EAVISE
-License: UNKNOWN Platform: UNKNOWN Description-Content-Type: text/markdown
-Provides-Extra: segment Provides-Extra: training License-File: LICENSE
-[Logo]Building blocks to recreate Darknet networks in Pytorch [![Version]
-[version-badge]][release-url] [![Documentation][doc-badge]][documentation-url]
-[![Pipeline][pipeline-badge]][pipeline-url] _[_K_o_-_F_i_][![Python][python-badge]]
-[python-url] [![PyTorch][pytorch-badge]][pytorch-url] [![VOC][voc-badge]][voc-
-url] [![COCO][coco-badge]][coco-url] ## Why another framework [pytorch-yolo2]
-(https://github.com/marvis/pytorch-yolo2) is working perfectly fine, but does
-not easily allow a user to modify an existing network. This is why I decided to
-create a library, that gives the user all the necessary building blocks, to
-recreate any darknet network. This library has everything you need to control
-your network, weight loading & saving, datasets, dataloaders and data
-augmentation. Where it started as library to recreate the darknet networks in
-PyTorch, it has since grown into a more general purpose single-shot object
-detection library. ## Installing First install [PyTorch and Torchvision](https:
-//pytorch.org/get-started/locally). Then clone this repository and run one of
-the following commands: ```bash # If you just want to use Lightnet pip install
-brambox # Optional (needed for training) pip install . # If you want to develop
-Lightnet pip install -r develop.txt ``` > This project is python 3.6 and higher
-so on some systems you might want to use 'pip3.6' instead of 'pip' ## How to
-use [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation
-and guides on how to use this library. The _examples_ folder contains code
-snippets to train and test networks with lightnet. For examples on how to
-implement your own networks, you can take a look at the files in _lightnet/
-models_. >If you are using a different version than the latest, >you can
-generate the documentation yourself by running `make clean html` in the _docs_
-folder. >This does require some dependencies, like Sphinx. >The easiest way to
-install them is by using the __-r develop.txt__ option when installing
-lightnet. ## Cite If you use Lightnet in your research, please cite it. ```
-@misc{lightnet18, author = {Tanguy Ophoff}, title = {Lightnet: Building Blocks
-to Recreate Darknet Networks in Pytorch}, howpublished = {\url{https://
-gitlab.com/EAVISE/lightnet}}, year = {2018} } ``` ## Main Contributors Here is
-a list of people that made noteworthy contributions and helped to get this
-project where it stands today! - [Tanguy Ophoff](https://gitlab.com/0phoff) -
-[Jon Crall](https://gitlab.com/Erotemic) - [Cedric Gullentops](https://
-github.com/CedricGullentops) [version-badge]: https://img.shields.io/pypi/v/
+Metadata-Version: 2.1 Name: lightnet Version: 4.0.0 Summary: Building blocks
+for recreating darknet networks in pytorch Author: EAVISE Description-Content-
+Type: text/markdown Provides-Extra: segment Provides-Extra: training License-
+File: LICENSE [Logo]Building blocks to recreate Darknet networks in Pytorch [!
+[Version][version-badge]][release-url] [![Documentation][doc-badge]]
+[documentation-url] [![Pipeline][pipeline-badge]][pipeline-url] _[_K_o_-_F_i_][!
+[Python][python-badge]][python-url] [![PyTorch][pytorch-badge]][pytorch-url] [!
+[VOC][voc-badge]][voc-url] [![COCO][coco-badge]][coco-url] ## Why another
+framework [pytorch-yolo2](https://github.com/marvis/pytorch-yolo2) is working
+perfectly fine, but does not easily allow a user to modify an existing network.
+This is why I decided to create a library, that gives the user all the
+necessary building blocks, to recreate any darknet network. This library has
+everything you need to control your network, weight loading & saving, datasets,
+dataloaders and data augmentation. Where it started as library to recreate the
+darknet networks in PyTorch, it has since grown into a more general purpose
+single-shot object detection library. ## Installing First install [PyTorch and
+Torchvision](https://pytorch.org/get-started/locally). Then clone this
+repository and run one of the following commands: ```bash # If you just want to
+use Lightnet pip install brambox # Optional (needed for training) pip install .
+# If you want to develop Lightnet pip install pillow opencv-python pip install
+-r develop.txt ``` > This project is python 3.7 and higher so on some systems
+you might want to use 'pip3.7' instead of 'pip' ## How to use [Click Here]
+(https://eavise.gitlab.io/lightnet) for the API documentation and guides on how
+to use this library. The _examples_ folder contains code snippets to train and
+test networks with lightnet. For examples on how to implement your own
+networks, you can take a look at the files in _lightnet/models_. >If you are
+using a different version than the latest, >you can generate the documentation
+yourself by running `make clean html` in the _docs_ folder. >This does require
+some dependencies, like Sphinx. >The easiest way to install them is by using
+the __-r develop.txt__ option when installing lightnet. ## Cite If you use
+Lightnet in your research, please cite it. ``` @misc{lightnet18, author =
+{Tanguy Ophoff}, title = {Lightnet: Building Blocks to Recreate Darknet
+Networks in Pytorch}, howpublished = {\url{https://gitlab.com/EAVISE/
+lightnet}}, year = {2018} } ``` ## Main Contributors Here is a list of people
+that made noteworthy contributions and helped to get this project where it
+stands today! - [Tanguy Ophoff](https://gitlab.com/0phoff) - [Jon Crall](https:
+//gitlab.com/Erotemic) - [Cedric Gullentops](https://github.com/
+CedricGullentops) [version-badge]: https://img.shields.io/pypi/v/
 lightnet.svg?label=version [doc-badge]: https://img.shields.io/badge/-
 Documentation-9B59B6.svg [python-badge]: https://img.shields.io/badge/Python-
-min%203.6%20%7C%20rec%203.9-FFD43B.svg [pytorch-badge]: https://img.shields.io/
-badge/PyTorch-1.9.0-F05732.svg [pipeline-badge]: https://gitlab.com/EAVISE/
+min%203.7%20%7C%20rec%203.9-FFD43B.svg [pytorch-badge]: https://img.shields.io/
+badge/PyTorch-1.13.0-F05732.svg [pipeline-badge]: https://gitlab.com/EAVISE/
 lightnet/badges/master/pipeline.svg [release-url]: https://gitlab.com/EAVISE/
 lightnet/tags [documentation-url]: https://eavise.gitlab.io/lightnet [python-
 url]: https://python.org [pytorch-url]: https://pytorch.org [pipeline-url]:
 https://pypi.org/project/lightnet [voc-badge]: https://img.shields.io/badge/
 repository-Pascal%20VOC-%2300BFD8 [voc-url]: https://gitlab.com/eavise/top/voc
 [coco-badge]: https://img.shields.io/badge/repository-MS%20COCO-%2300BFD8
 [coco-url]: https://gitlab.com/eavise/top/coco
```

### Comparing `lightnet-3.1.0/lightnet.egg-info/SOURCES.txt` & `lightnet-4.0.0/lightnet.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 lightnet/engine/_scheduler.py
 lightnet/models/__init__.py
 lightnet/models/_dataset_brambox.py
 lightnet/models/_dataset_darknet.py
 lightnet/models/_network_alexnet.py
 lightnet/models/_network_cornernet.py
 lightnet/models/_network_cornernet_squeeze.py
+lightnet/models/_network_cspdarknet53.py
 lightnet/models/_network_darknet.py
 lightnet/models/_network_darknet19.py
 lightnet/models/_network_darknet53.py
 lightnet/models/_network_dyolo.py
 lightnet/models/_network_mobile_darknet19.py
 lightnet/models/_network_mobile_yolo_v2.py
 lightnet/models/_network_mobile_yolo_v2_upsample.py
@@ -57,40 +58,42 @@
 lightnet/models/_network_tiny_yolo_v3.py
 lightnet/models/_network_vgg.py
 lightnet/models/_network_yolact.py
 lightnet/models/_network_yolo_fusion.py
 lightnet/models/_network_yolo_v2.py
 lightnet/models/_network_yolo_v2_upsample.py
 lightnet/models/_network_yolo_v3.py
+lightnet/models/_network_yolo_v4.py
 lightnet/models/_network_yolt.py
 lightnet/network/__init__.py
 lightnet/network/_basemodule.py
 lightnet/network/backbone/__init__.py
 lightnet/network/backbone/_alexnet.py
 lightnet/network/backbone/_cornernet.py
+lightnet/network/backbone/_csp.py
 lightnet/network/backbone/_darknet.py
-lightnet/network/backbone/_deform_resnet.py
 lightnet/network/backbone/_mobile_darknet.py
 lightnet/network/backbone/_mobilenet.py
 lightnet/network/backbone/_resnet.py
 lightnet/network/backbone/_vgg.py
 lightnet/network/head/__init__.py
 lightnet/network/head/_classification_conv.py
 lightnet/network/head/_classification_fc.py
 lightnet/network/head/_detection_anchor_masked.py
 lightnet/network/head/_detection_anchor_oriented.py
 lightnet/network/head/_detection_anchor_yolo.py
 lightnet/network/head/_detection_corner.py
 lightnet/network/head/_detection_yolact.py
 lightnet/network/layer/__init__.py
+lightnet/network/layer/_aggregation.py
 lightnet/network/layer/_conv.py
 lightnet/network/layer/_cornernet.py
+lightnet/network/layer/_csp.py
 lightnet/network/layer/_darknet.py
 lightnet/network/layer/_deform.py
-lightnet/network/layer/_fpn.py
 lightnet/network/layer/_fusion.py
 lightnet/network/layer/_hourglass.py
 lightnet/network/layer/_mobilenet.py
 lightnet/network/layer/_util.py
 lightnet/network/loss/__init__.py
 lightnet/network/loss/_base.py
 lightnet/network/loss/_corner.py
```

### Comparing `lightnet-3.1.0/setup.py` & `lightnet-4.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightnet-3.1.0/README.md` & `lightnet-4.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,18 @@
 Then clone this repository and run one of the following commands:
 ```bash
 # If you just want to use Lightnet
 pip install brambox   # Optional (needed for training)
 pip install .
 
 # If you want to develop Lightnet
+pip install pillow opencv-python
 pip install -r develop.txt
 ```
-> This project is python 3.6 and higher so on some systems you might want to use 'pip3.6' instead of 'pip'
+> This project is python 3.7 and higher so on some systems you might want to use 'pip3.7' instead of 'pip'
 
 ## How to use
 [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation and guides on how to use this library.  
 The _examples_ folder contains code snippets to train and test networks with lightnet. For examples on how to implement your own networks, you can take a look at the files in _lightnet/models_.
 >If you are using a different version than the latest,
 >you can generate the documentation yourself by running `make clean html` in the _docs_ folder.
 >This does require some dependencies, like Sphinx.
@@ -61,16 +62,16 @@
 - [Tanguy Ophoff](https://gitlab.com/0phoff)
 - [Jon Crall](https://gitlab.com/Erotemic)
 - [Cedric Gullentops](https://github.com/CedricGullentops)
 
 
 [version-badge]: https://img.shields.io/pypi/v/lightnet.svg?label=version
 [doc-badge]: https://img.shields.io/badge/-Documentation-9B59B6.svg
-[python-badge]: https://img.shields.io/badge/Python-min%203.6%20%7C%20rec%203.9-FFD43B.svg
-[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.9.0-F05732.svg
+[python-badge]: https://img.shields.io/badge/Python-min%203.7%20%7C%20rec%203.9-FFD43B.svg
+[pytorch-badge]: https://img.shields.io/badge/PyTorch-1.13.0-F05732.svg
 [pipeline-badge]: https://gitlab.com/EAVISE/lightnet/badges/master/pipeline.svg
 [release-url]: https://gitlab.com/EAVISE/lightnet/tags
 [documentation-url]: https://eavise.gitlab.io/lightnet
 [python-url]: https://python.org
 [pytorch-url]: https://pytorch.org
 [pipeline-url]: https://pypi.org/project/lightnet
 [voc-badge]: https://img.shields.io/badge/repository-Pascal%20VOC-%2300BFD8
```

#### html2text {}

```diff
@@ -10,36 +10,37 @@
 your network, weight loading & saving, datasets, dataloaders and data
 augmentation. Where it started as library to recreate the darknet networks in
 PyTorch, it has since grown into a more general purpose single-shot object
 detection library. ## Installing First install [PyTorch and Torchvision](https:
 //pytorch.org/get-started/locally). Then clone this repository and run one of
 the following commands: ```bash # If you just want to use Lightnet pip install
 brambox # Optional (needed for training) pip install . # If you want to develop
-Lightnet pip install -r develop.txt ``` > This project is python 3.6 and higher
-so on some systems you might want to use 'pip3.6' instead of 'pip' ## How to
-use [Click Here](https://eavise.gitlab.io/lightnet) for the API documentation
-and guides on how to use this library. The _examples_ folder contains code
-snippets to train and test networks with lightnet. For examples on how to
-implement your own networks, you can take a look at the files in _lightnet/
-models_. >If you are using a different version than the latest, >you can
-generate the documentation yourself by running `make clean html` in the _docs_
-folder. >This does require some dependencies, like Sphinx. >The easiest way to
-install them is by using the __-r develop.txt__ option when installing
-lightnet. ## Cite If you use Lightnet in your research, please cite it. ```
-@misc{lightnet18, author = {Tanguy Ophoff}, title = {Lightnet: Building Blocks
-to Recreate Darknet Networks in Pytorch}, howpublished = {\url{https://
-gitlab.com/EAVISE/lightnet}}, year = {2018} } ``` ## Main Contributors Here is
-a list of people that made noteworthy contributions and helped to get this
-project where it stands today! - [Tanguy Ophoff](https://gitlab.com/0phoff) -
-[Jon Crall](https://gitlab.com/Erotemic) - [Cedric Gullentops](https://
-github.com/CedricGullentops) [version-badge]: https://img.shields.io/pypi/v/
-lightnet.svg?label=version [doc-badge]: https://img.shields.io/badge/-
-Documentation-9B59B6.svg [python-badge]: https://img.shields.io/badge/Python-
-min%203.6%20%7C%20rec%203.9-FFD43B.svg [pytorch-badge]: https://img.shields.io/
-badge/PyTorch-1.9.0-F05732.svg [pipeline-badge]: https://gitlab.com/EAVISE/
-lightnet/badges/master/pipeline.svg [release-url]: https://gitlab.com/EAVISE/
-lightnet/tags [documentation-url]: https://eavise.gitlab.io/lightnet [python-
-url]: https://python.org [pytorch-url]: https://pytorch.org [pipeline-url]:
-https://pypi.org/project/lightnet [voc-badge]: https://img.shields.io/badge/
-repository-Pascal%20VOC-%2300BFD8 [voc-url]: https://gitlab.com/eavise/top/voc
-[coco-badge]: https://img.shields.io/badge/repository-MS%20COCO-%2300BFD8
-[coco-url]: https://gitlab.com/eavise/top/coco
+Lightnet pip install pillow opencv-python pip install -r develop.txt ``` > This
+project is python 3.7 and higher so on some systems you might want to use
+'pip3.7' instead of 'pip' ## How to use [Click Here](https://eavise.gitlab.io/
+lightnet) for the API documentation and guides on how to use this library. The
+_examples_ folder contains code snippets to train and test networks with
+lightnet. For examples on how to implement your own networks, you can take a
+look at the files in _lightnet/models_. >If you are using a different version
+than the latest, >you can generate the documentation yourself by running `make
+clean html` in the _docs_ folder. >This does require some dependencies, like
+Sphinx. >The easiest way to install them is by using the __-r develop.txt__
+option when installing lightnet. ## Cite If you use Lightnet in your research,
+please cite it. ``` @misc{lightnet18, author = {Tanguy Ophoff}, title =
+{Lightnet: Building Blocks to Recreate Darknet Networks in Pytorch},
+howpublished = {\url{https://gitlab.com/EAVISE/lightnet}}, year = {2018} } ```
+## Main Contributors Here is a list of people that made noteworthy
+contributions and helped to get this project where it stands today! - [Tanguy
+Ophoff](https://gitlab.com/0phoff) - [Jon Crall](https://gitlab.com/Erotemic) -
+[Cedric Gullentops](https://github.com/CedricGullentops) [version-badge]:
+https://img.shields.io/pypi/v/lightnet.svg?label=version [doc-badge]: https://
+img.shields.io/badge/-Documentation-9B59B6.svg [python-badge]: https://
+img.shields.io/badge/Python-min%203.7%20%7C%20rec%203.9-FFD43B.svg [pytorch-
+badge]: https://img.shields.io/badge/PyTorch-1.13.0-F05732.svg [pipeline-
+badge]: https://gitlab.com/EAVISE/lightnet/badges/master/pipeline.svg [release-
+url]: https://gitlab.com/EAVISE/lightnet/tags [documentation-url]: https://
+eavise.gitlab.io/lightnet [python-url]: https://python.org [pytorch-url]:
+https://pytorch.org [pipeline-url]: https://pypi.org/project/lightnet [voc-
+badge]: https://img.shields.io/badge/repository-Pascal%20VOC-%2300BFD8 [voc-
+url]: https://gitlab.com/eavise/top/voc [coco-badge]: https://img.shields.io/
+badge/repository-MS%20COCO-%2300BFD8 [coco-url]: https://gitlab.com/eavise/top/
+coco
```

### Comparing `lightnet-3.1.0/setup.cfg` & `lightnet-4.0.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 	B,
 	B9,
 	C4,
 	SIM,
 	Q0,
 	R5,
 ignore = 
+	B905,
+	B907,
 	E226,
 	E241,
 	E501,
 	E713,
-	W605,
-	W503,
 	G002,
 	G200,
 	SIM106,
 	SIM114,
+	W605,
+	W503,
 per-file-ignores = 
 	__init__.py:F401,F403
 	lightnet/network/backbone/*.py:B902,E126
 	lightnet/network/backbone/__init__.py:F401,F403
 	lightnet/network/head/*.py:B902,E126
 	lightnet/network/head/__init__.py:F401,F403
 	lightnet/models/_network*:B006,B008
```

### Comparing `lightnet-3.1.0/versioneer.py` & `lightnet-4.0.0/versioneer.py`

 * *Files identical despite different names*

