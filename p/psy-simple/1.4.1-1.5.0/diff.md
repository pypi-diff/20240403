# Comparing `tmp/psy-simple-1.4.1.tar.gz` & `tmp/psy-simple-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psy-simple-1.4.1.tar", last modified: Mon Feb 14 10:50:49 2022, max compression
+gzip compressed data, was "psy-simple-1.5.0.tar", last modified: Wed Apr  3 13:41:07 2024, max compression
```

## Comparing `psy-simple-1.4.1.tar` & `psy-simple-1.5.0.tar`

### file list

```diff
@@ -1,216 +1,242 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.389031 psy-simple-1.4.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    35149 2022-02-14 10:48:46.000000 psy-simple-1.4.1/COPYING
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7652 2022-02-14 10:48:46.000000 psy-simple-1.4.1/COPYING.LESSER
--rw-r--r--   0 circleci  (3434) circleci  (3434)      195 2022-02-14 10:48:46.000000 psy-simple-1.4.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5198 2022-02-14 10:50:49.389031 psy-simple-1.4.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3925 2022-02-14 10:48:46.000000 psy-simple-1.4.1/README.rst
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.389031 psy-simple-1.4.1/psy_simple/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1575 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      497 2022-02-14 10:50:49.389031 psy-simple-1.4.1/psy_simple/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    34461 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11960 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/colors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)   195044 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/plotters.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    42474 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/plugin.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.369031 psy-simple-1.4.1/psy_simple/widgets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2145 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    39045 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/colors.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.369031 psy-simple-1.4.1/psy_simple/widgets/icons/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      660 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/bold.png
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.389031 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      357 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Accent.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Accent_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      550 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Blues.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      547 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Blues_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BrBG.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      651 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BrBG_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuGn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuGn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuPu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuPu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      588 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/CMRmap.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      595 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/CMRmap_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      362 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Dark2.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      356 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Dark2_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/GnBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/GnBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greens.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greens_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      398 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greys.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      389 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greys_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      557 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/OrRd.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      546 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/OrRd_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Oranges.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Oranges_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PRGn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      655 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PRGn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Paired.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      401 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Paired_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Pastel1.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      341 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Pastel1_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      348 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Pastel2.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      343 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Pastel2_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      664 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PiYG.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      678 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PiYG_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      582 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBuGn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      592 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBuGn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      575 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuOr.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      646 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuOr_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuRd.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      621 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuRd_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      549 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Purples.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      559 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Purples_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      567 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdGy.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      551 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdGy_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdPu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdPu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      645 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      647 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      619 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlGn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      615 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlGn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Reds.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      558 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Reds_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      360 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set1.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      355 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set1_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      358 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set2.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set2_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      399 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set3.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      396 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Set3_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      667 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Spectral.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      658 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Spectral_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      467 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Wistia.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Wistia_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      580 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      617 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGnBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      613 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGnBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      578 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      555 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrBr.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      571 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrBr_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      567 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrRd.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      561 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrRd_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/afmhot.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      387 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/afmhot_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      288 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/autumn.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      292 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/autumn_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/binary.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      282 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/binary_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      307 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/blue_white_red.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/blue_white_red_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      482 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/bone.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      519 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/bone_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      361 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/brg.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      361 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/brg_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/bwr.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      322 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/bwr_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      591 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cividis.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cividis_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cool.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cool_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      662 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/coolwarm.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      662 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/coolwarm_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      492 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/copper.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      511 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/copper_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      671 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cubehelix.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      690 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cubehelix_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1359 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/flag.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1361 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/flag_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      675 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_earth.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      686 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_earth_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      282 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_gray.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_gray_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      412 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_heat.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      411 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_heat_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      776 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_ncar.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_ncar_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      471 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_rainbow.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      487 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_rainbow_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      496 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_stern.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      506 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_stern_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_yarg.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      282 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_yarg_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      647 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      417 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot2.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot2_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      656 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      282 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gray.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gray_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      345 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/hot.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      351 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/hot_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      452 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/hsv.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      461 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/hsv_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      660 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/inferno.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      669 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/inferno_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      512 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/jet.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/jet_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      616 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/magma.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      628 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/magma_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      606 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/nipy_spectral.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      624 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/nipy_spectral_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/ocean.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      479 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/ocean_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      573 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/pink.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      568 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/pink_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      604 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/plasma.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      629 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/plasma_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1132 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/prism.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1124 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/prism_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      672 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rainbow.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      651 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rainbow_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      302 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/red_white_blue.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      307 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/red_white_blue_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rwb.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rwb_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      401 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/seismic.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      395 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/seismic_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/spring.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      309 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/spring_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      339 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/summer.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      345 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/summer_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      372 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab10.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      371 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab10_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      488 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      493 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20b.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      467 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20b_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      465 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20c.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      462 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/tab20c_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      607 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/terrain.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      614 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/terrain_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      748 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      753 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      747 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_shifted.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      739 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_shifted_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/viridis.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      625 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/viridis_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      552 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Blues.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      563 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Greens.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      688 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_RdBu.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      680 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_RdBu_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      565 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Reds.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      267 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/wbr.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      263 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/wbr_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      282 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/white_blue_red.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      281 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/white_blue_red_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      286 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/white_red_blue.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/white_red_blue_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      340 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/winter.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/winter_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      269 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/wrb.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/wrb_r.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1381 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/font_color.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)      459 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/icons/italic.png
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16517 2022-02-14 10:48:46.000000 psy-simple-1.4.1/psy_simple/widgets/texts.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-14 10:50:49.365031 psy-simple-1.4.1/psy_simple.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5198 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8552 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)       31 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       11 2022-02-14 10:50:49.000000 psy-simple-1.4.1/psy_simple.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      210 2022-02-14 10:50:49.389031 psy-simple-1.4.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3634 2022-02-14 10:48:46.000000 psy-simple-1.4.1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    69729 2022-02-14 10:48:46.000000 psy-simple-1.4.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.174511 psy-simple-1.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.124509 psy-simple-1.5.0/LICENSES/
+-rw-rw-rw-   0 root         (0) root         (0)    17023 2024-04-03 13:40:40.000000 psy-simple-1.5.0/LICENSES/CC-BY-4.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7048 2024-04-03 13:40:40.000000 psy-simple-1.5.0/LICENSES/CC0-1.0.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42098 2024-04-03 13:40:40.000000 psy-simple-1.5.0/LICENSES/LGPL-3.0-only.txt
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-04-03 13:41:07.173511 psy-simple-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-03 13:40:40.000000 psy-simple-1.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.126510 psy-simple-1.5.0/psy_simple/
+-rw-rw-rw-   0 root         (0) root         (0)      755 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-04-03 13:41:07.174511 psy-simple-1.5.0/psy_simple/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    34434 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    11804 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)   199382 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/plotters.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.128510 psy-simple-1.5.0/psy_simple/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1451 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38666 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/colors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.129510 psy-simple-1.5.0/psy_simple/widgets/icons/
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/bold.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.165511 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Accent.png
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Accent_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)      547 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Blues_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BrBG.png
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BrBG_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuGn.png
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuGn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuPu.png
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuPu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/CMRmap.png
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/CMRmap_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      362 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Dark2.png
+-rw-rw-rw-   0 root         (0) root         (0)      356 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Dark2_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/GnBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/GnBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greens.png
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greens_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greys.png
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greys_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/OrRd.png
+-rw-rw-rw-   0 root         (0) root         (0)      546 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/OrRd_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      554 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Oranges.png
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Oranges_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PRGn.png
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PRGn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      404 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Paired.png
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Paired_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Pastel1.png
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Pastel1_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Pastel2.png
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Pastel2_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PiYG.png
+-rw-rw-rw-   0 root         (0) root         (0)      678 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PiYG_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBuGn.png
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBuGn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      575 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuOr.png
+-rw-rw-rw-   0 root         (0) root         (0)      646 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuOr_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuRd.png
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuRd_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Purples.png
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Purples_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      677 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdGy.png
+-rw-rw-rw-   0 root         (0) root         (0)      551 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdGy_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdPu.png
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdPu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      619 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlGn.png
+-rw-rw-rw-   0 root         (0) root         (0)      615 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlGn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Reds.png
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Reds_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set1.png
+-rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set1_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      358 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set2.png
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set2_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      399 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set3.png
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Set3_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Spectral.png
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Spectral_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Wistia.png
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Wistia_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGn.png
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGnBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGnBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrBr.png
+-rw-rw-rw-   0 root         (0) root         (0)      571 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrBr_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      567 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrRd.png
+-rw-rw-rw-   0 root         (0) root         (0)      561 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrRd_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/afmhot.png
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/afmhot_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/autumn.png
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/autumn_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/binary.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/binary_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/blue_white_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/blue_white_red_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/bone.png
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/bone_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/brg.png
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/brg_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/bwr.png
+-rw-rw-rw-   0 root         (0) root         (0)      322 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/bwr_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cividis.png
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cividis_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cool.png
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cool_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/coolwarm.png
+-rw-rw-rw-   0 root         (0) root         (0)      662 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/coolwarm_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/copper.png
+-rw-rw-rw-   0 root         (0) root         (0)      511 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/copper_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      671 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cubehelix.png
+-rw-rw-rw-   0 root         (0) root         (0)      690 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cubehelix_r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/flag.png
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/flag_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      675 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_earth.png
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_earth_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_gray.png
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_gray_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_heat.png
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_heat_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_ncar.png
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_ncar_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_rainbow.png
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_rainbow_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_stern.png
+-rw-rw-rw-   0 root         (0) root         (0)      506 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_stern_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_yarg.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_yarg_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      647 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot.png
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot2.png
+-rw-rw-rw-   0 root         (0) root         (0)      437 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot2_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      656 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gray.png
+-rw-rw-rw-   0 root         (0) root         (0)      299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gray_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/hot.png
+-rw-rw-rw-   0 root         (0) root         (0)      351 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/hot_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/hsv.png
+-rw-rw-rw-   0 root         (0) root         (0)      461 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/hsv_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/inferno.png
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/inferno_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      512 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/jet.png
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/jet_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      616 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/magma.png
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/magma_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/nipy_spectral.png
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/nipy_spectral_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/ocean.png
+-rw-rw-rw-   0 root         (0) root         (0)      479 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/ocean_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      573 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/pink.png
+-rw-rw-rw-   0 root         (0) root         (0)      568 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/pink_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/plasma.png
+-rw-rw-rw-   0 root         (0) root         (0)      629 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/plasma_r.png
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/prism.png
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/prism_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rainbow.png
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rainbow_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/red_white_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/red_white_blue_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rwb.png
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rwb_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/seismic.png
+-rw-rw-rw-   0 root         (0) root         (0)      395 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/seismic_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/spring.png
+-rw-rw-rw-   0 root         (0) root         (0)      309 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/spring_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/summer.png
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/summer_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab10.png
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab10_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20.png
+-rw-rw-rw-   0 root         (0) root         (0)      493 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      463 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20b.png
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20b_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      465 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20c.png
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/tab20c_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/terrain.png
+-rw-rw-rw-   0 root         (0) root         (0)      614 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/terrain_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      748 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight.png
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_shifted.png
+-rw-rw-rw-   0 root         (0) root         (0)      739 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_shifted_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/viridis.png
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/viridis_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Blues.png
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Greens.png
+-rw-rw-rw-   0 root         (0) root         (0)      688 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_RdBu.png
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_RdBu_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      565 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Reds.png
+-rw-rw-rw-   0 root         (0) root         (0)      267 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/wbr.png
+-rw-rw-rw-   0 root         (0) root         (0)      263 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/wbr_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      282 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/white_blue_red.png
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/white_blue_red_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/white_red_blue.png
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/white_red_blue_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      340 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/winter.png
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/winter_r.png
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/wrb.png
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/wrb_r.png
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/font_color.png
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/icons/italic.png
+-rw-rw-rw-   0 root         (0) root         (0)    16280 2024-04-03 13:40:40.000000 psy-simple-1.5.0/psy_simple/widgets/texts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.170511 psy-simple-1.5.0/psy_simple.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6241 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9175 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 13:41:06.000000 psy-simple-1.5.0/psy_simple.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      407 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 13:41:07.000000 psy-simple-1.5.0/psy_simple.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3263 2024-04-03 13:40:40.000000 psy-simple-1.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 13:41:07.174511 psy-simple-1.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-04-03 13:40:40.000000 psy-simple-1.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 13:41:07.169510 psy-simple-1.5.0/tests/
+-rwxrwxrwx   0 root         (0) root         (0)     4784 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_barplot.py
+-rwxrwxrwx   0 root         (0) root         (0)     1643 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_barplot_data.py
+-rwxrwxrwx   0 root         (0) root         (0)     1508 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_barplot_single.py
+-rwxrwxrwx   0 root         (0) root         (0)     6554 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2228 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_colors.py
+-rw-rw-rw-   0 root         (0) root         (0)    12936 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_combined.py
+-rw-rw-rw-   0 root         (0) root         (0)     5112 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_combined_icon.py
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_density.py
+-rw-rw-rw-   0 root         (0) root         (0)      794 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_density_kde.py
+-rw-rw-rw-   0 root         (0) root         (0)     5470 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_fldmean.py
+-rw-rw-rw-   0 root         (0) root         (0)     1810 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_fldmean_icon.py
+-rwxrwxrwx   0 root         (0) root         (0)    23792 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_lineplot.py
+-rwxrwxrwx   0 root         (0) root         (0)     1611 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_lineplot_single.py
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_plot2d.py
+-rw-rw-rw-   0 root         (0) root         (0)      988 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_plot2d_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     4300 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_plot2d_icon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1315 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_plot2d_icon_contour.py
+-rw-rw-rw-   0 root         (0) root         (0)     1545 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_plot2d_icon_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)     5435 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_vector.py
+-rw-rw-rw-   0 root         (0) root         (0)     2419 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_vector_icon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_vector_stream.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_violin.py
+-rwxrwxrwx   0 root         (0) root         (0)     1299 2024-04-03 13:40:40.000000 psy-simple-1.5.0/tests/test_violin_single.py
```

### Comparing `psy-simple-1.4.1/COPYING` & `psy-simple-1.5.0/LICENSES/LGPL-3.0-only.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,674 +1,304 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+GNU LESSER GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+This version of the GNU Lesser General Public License incorporates the terms and conditions of version 3 of the GNU General Public License, supplemented by the additional permissions listed below.
+
+0. Additional Definitions.
+
+As used herein, "this License" refers to version 3 of the GNU Lesser General Public License, and the "GNU GPL" refers to version 3 of the GNU General Public License.
+
+"The Library" refers to a covered work governed by this License, other than an Application or a Combined Work as defined below.
+
+An "Application" is any work that makes use of an interface provided by the Library, but which is not otherwise based on the Library. Defining a subclass of a class defined by the Library is deemed a mode of using an interface provided by the Library.
+
+A "Combined Work" is a work produced by combining or linking an Application with the Library.  The particular version of the Library with which the Combined Work was made is also called the "Linked Version".
+
+The "Minimal Corresponding Source" for a Combined Work means the Corresponding Source for the Combined Work, excluding any source code for portions of the Combined Work that, considered in isolation, are based on the Application, and not on the Linked Version.
+
+The "Corresponding Application Code" for a Combined Work means the object code and/or source code for the Application, including any data and utility programs needed for reproducing the Combined Work from the Application, but excluding the System Libraries of the Combined Work.
+
+1. Exception to Section 3 of the GNU GPL.
+You may convey a covered work under sections 3 and 4 of this License without being bound by section 3 of the GNU GPL.
+
+2. Conveying Modified Versions.
+If you modify a copy of the Library, and, in your modifications, a facility refers to a function or data to be supplied by an Application that uses the facility (other than as an argument passed when the facility is invoked), then you may convey a copy of the modified version:
+
+     a) under this License, provided that you make a good faith effort to ensure that, in the event an Application does not supply the function or data, the facility still operates, and performs whatever part of its purpose remains meaningful, or
+
+     b) under the GNU GPL, with none of the additional permissions of this License applicable to that copy.
+
+3. Object Code Incorporating Material from Library Header Files.
+The object code form of an Application may incorporate material from a header file that is part of the Library.  You may convey such object code under terms of your choice, provided that, if the incorporated material is not limited to numerical parameters, data structure layouts and accessors, or small macros, inline functions and templates (ten or fewer lines in length), you do both of the following:
+
+     a) Give prominent notice with each copy of the object code that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the object code with a copy of the GNU GPL and this license document.
+
+4. Combined Works.
+You may convey a Combined Work under terms of your choice that, taken together, effectively do not restrict modification of the portions of the Library contained in the Combined Work and reverse engineering for debugging such modifications, if you also do each of the following:
+
+     a) Give prominent notice with each copy of the Combined Work that the Library is used in it and that the Library and its use are covered by this License.
+
+     b) Accompany the Combined Work with a copy of the GNU GPL and this license document.
+
+     c) For a Combined Work that displays copyright notices during execution, include the copyright notice for the Library among these notices, as well as a reference directing the user to the copies of the GNU GPL and this license document.
+
+     d) Do one of the following:
+
+           0) Convey the Minimal Corresponding Source under the terms of this License, and the Corresponding Application Code in a form suitable for, and under terms that permit, the user to recombine or relink the Application with a modified version of the Linked Version to produce a modified Combined Work, in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.
+
+          1) Use a suitable shared library mechanism for linking with the Library.  A suitable mechanism is one that (a) uses at run time a copy of the Library already present on the user's computer system, and (b) will operate properly with a modified version of the Library that is interface-compatible with the Linked Version.
+
+     e) Provide Installation Information, but only if you would otherwise be required to provide such information under section 6 of the GNU GPL, and only to the extent that such information is necessary to install and execute a modified version of the Combined Work produced by recombining or relinking the Application with a modified version of the Linked Version. (If you use option 4d0, the Installation Information must accompany the Minimal Corresponding Source and Corresponding Application Code. If you use option 4d1, you must provide the Installation Information in the manner specified by section 6 of the GNU GPL for conveying Corresponding Source.)
+
+5. Combined Libraries.
+You may place library facilities that are a work based on the Library side by side in a single library together with other library facilities that are not Applications and are not covered by this License, and convey such a combined library under terms of your choice, if you do both of the following:
+
+     a) Accompany the combined library with a copy of the same work based on the Library, uncombined with any other library facilities, conveyed under the terms of this License.
+
+     b) Give prominent notice with the combined library that part of it is a work based on the Library, and explaining where to find the accompanying uncombined form of the same work.
+
+6. Revised Versions of the GNU Lesser General Public License.
+The Free Software Foundation may publish revised and/or new versions of the GNU Lesser General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Library as you received it specifies that a certain numbered version of the GNU Lesser General Public License "or any later version" applies to it, you have the option of following the terms and conditions either of that published version or of any later version published by the Free Software Foundation. If the Library as you received it does not specify a version number of the GNU Lesser General Public License, you may choose any version of the GNU Lesser General Public License ever published by the Free Software Foundation.
+
+If the Library as you received it specifies that a proxy can decide whether future versions of the GNU Lesser General Public License shall
+apply, that proxy's public statement of acceptance of any version is permanent authorization for you to choose that version for the Library.
+
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
+
+Copyright © 2007 Free Software Foundation, Inc. <http://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+Preamble
+
+The GNU General Public License is a free, copyleft license for software and other kinds of works.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
+
+Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and modification follow.
+
+TERMS AND CONDITIONS
+
+0. Definitions.
+
+“This License” refers to version 3 of the GNU General Public License.
+
+“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
+
+To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
+
+A “covered work” means either the unmodified Program or a work based on the Program.
+
+To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
+
+A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+
+2. Basic Permissions.
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+
+4. Conveying Verbatim Copies.
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+     a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+
+     b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
+
+     c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+
+     d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+     a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+
+     b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+
+     c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+
+     d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+
+     e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+
+7. Additional Terms.
+“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+     a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+
+     b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+
+     c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+
+     d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+
+     e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+
+     f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+
+8. Termination.
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+
+11. Patents.
+A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
+
+A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
+
+14. Revised Versions of this License.
+The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+
+15. Disclaimer of Warranty.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
+
+     <one line to give the program's name and a brief idea of what it does.>
+     Copyright (C) <year>  <name of author>
+
+     This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
+If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
+
+     <program>  Copyright (C) <year>  <name of author>
+     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+     This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
+
+You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <http://www.gnu.org/licenses/>.
 
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `psy-simple-1.4.1/README.rst` & `psy-simple-1.5.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,26 @@
+.. SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum hereon GmbH
+..
+.. SPDX-License-Identifier: CC-BY-4.0
+
 ========================================================
 psy-simple: The psyplot plugin for simple visualizations
 ========================================================
 
 .. start-badges
 
-.. list-table::
-    :stub-columns: 1
-    :widths: 10 90
-
-    * - docs
-      - |docs|
-    * - tests
-      - |circleci| |appveyor| |requires| |codecov|
-    * - package
-      - |version| |conda| |github| |zenodo|
-    * - implementations
-      - |supported-versions| |supported-implementations|
-
-.. |docs| image:: https://img.shields.io/github/deployments/psyplot/psy-simple/github-pages
-    :alt: Documentation
-    :target: http://psyplot.github.io/psy-simple/
-
-.. |circleci| image:: https://circleci.com/gh/psyplot/psy-simple/tree/master.svg?style=svg
-    :alt: CircleCI
-    :target: https://circleci.com/gh/psyplot/psy-simple/tree/master
-
-.. |appveyor| image:: https://ci.appveyor.com/api/projects/status/49u41l2f9k0r4xc0/branch/master?svg=true
-    :alt: AppVeyor
-    :target: https://ci.appveyor.com/project/psyplot/psy-simple
-
-.. |codecov| image:: https://codecov.io/gh/psyplot/psy-simple/branch/master/graph/badge.svg
-    :alt: Coverage
-    :target: https://codecov.io/gh/psyplot/psy-simple
-
-.. |requires| image:: https://requires.io/github/psyplot/psy-simple/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/psyplot/psy-simple/requirements/?branch=master
-
-.. |version| image:: https://img.shields.io/pypi/v/psy-simple.svg?style=flat
-    :alt: PyPI Package latest release
-    :target: https://pypi.python.org/pypi/psy-simple
-
-.. |conda| image:: https://anaconda.org/conda-forge/psy-simple/badges/version.svg
-    :alt: conda
-    :target: https://anaconda.org/conda-forge/psy-simple
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/psy-simple.svg?style=flat
-    :alt: Supported versions
-    :target: https://pypi.python.org/pypi/psy-simple
-
-.. |supported-implementations| image:: https://img.shields.io/pypi/implementation/psy-simple.svg?style=flat
-    :alt: Supported implementations
-    :target: https://pypi.python.org/pypi/psy-simple
-
-.. |zenodo| image:: https://zenodo.org/badge/81938204.svg
-    :alt: Zenodo
-    :target: https://zenodo.org/badge/latestdoi/81938204
-
-.. |github| image:: https://img.shields.io/github/release/psyplot/psy-simple.svg
-    :target: https://github.com/psyplot/psy-simple/releases/latest
-    :alt: Latest github release
 
+|CI|
+|Code coverage|
+|Latest Release|
+|PyPI version|
+|Code style: black|
+|Imports: isort|
+|PEP8|
+|REUSE status|
 
 .. end-badges
 
 Welcome to the psyplot plugin for simple visualization. This package targets
 simple visualization like line plots, 2D plots, bar plots, density plots, etc.
 It provides the basics for all the more advanced and specialized plugins like
 the psy-maps_ or psy-reg_ plugin.
@@ -76,16 +32,16 @@
 .. _psy-maps: http://psyplot.github.io/psy-maps/
 .. _psy-reg: http://psyplot.github.io/psy-reg/
 .. _plot methods: http://psyplot.github.io/psy-simple/plot_methods
 .. _examples: http://psyplot.github.io/examples/
 
 Copyright
 ---------
-Copyright © 2021 Helmholtz-Zentrum Hereon, 2020-2021 Helmholtz-Zentrum
-Geesthacht, 2016-2021 University of Lausanne
+Copyright © 2021-2024 Helmholtz-Zentrum Hereon, 2020-2021 Helmholtz-Zentrum
+Geesthacht, 2016-2024 University of Lausanne
 
 This file is part of psy-simple and is released under the GNU LGPL-3.O license.
 See COPYING and COPYING.LESSER in the root of the repository for full
 licensing details.
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License version 3.0 as
@@ -94,7 +50,26 @@
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU LGPL-3.0 license for more details.
 
 You should have received a copy of the GNU LGPL-3.0 license
 along with this program.  If not, see https://www.gnu.org/licenses/.
+
+.. |CI| image:: https://codebase.helmholtz.cloud/psyplot/psy-simple/badges/main/pipeline.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-simple/-/pipelines?page=1&scope=all&ref=main
+.. |Code coverage| image:: https://codebase.helmholtz.cloud/psyplot/psy-simple/badges/main/coverage.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-simple/-/graphs/main/charts
+.. |Latest Release| image:: https://codebase.helmholtz.cloud/psyplot/psy-simple/-/badges/release.svg
+   :target: https://codebase.helmholtz.cloud/psyplot/psy-simple
+.. |PyPI version| image:: https://img.shields.io/pypi/v/psy-simple.svg
+   :target: https://pypi.python.org/pypi/psy-simple/
+.. |Code style: black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+.. |Imports: isort| image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
+   :target: https://pycqa.github.io/isort/
+.. |PEP8| image:: https://img.shields.io/badge/code%20style-pep8-orange.svg
+   :target: https://www.python.org/dev/peps/pep-0008/
+.. |Checked with mypy| image:: http://www.mypy-lang.org/static/mypy_badge.svg
+   :target: http://mypy-lang.org/
+.. |REUSE status| image:: https://api.reuse.software/badge/codebase.helmholtz.cloud/psyplot/psy-simple
+   :target: https://api.reuse.software/info/codebase.helmholtz.cloud/psyplot/psy-simple
```

### Comparing `psy-simple-1.4.1/psy_simple/base.py` & `psy-simple-1.5.0/psy_simple/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,36 @@
 """Base formatoptions for psy-simple.
 
 This module defines several formatoptions that are the basis for many
 matplotlib figures, such as axes title, figure title, etc.
 """
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-simple and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum Hereon
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
+
+import inspect
 from abc import abstractmethod
 from collections import defaultdict
 from itertools import chain
+
+import matplotlib.pyplot as plt
 import numpy as np
-import inspect
 import pandas as pd
-import matplotlib.pyplot as plt
-from psyplot.docstring import docstrings, safe_modulo, dedent
+import six
 from psyplot.data import InteractiveList, open_dataset
-from psyplot.compat.pycompat import filter
-from psyplot.plotter import (
-    Plotter, Formatoption, rcParams, START)
+from psyplot.docstring import dedent, docstrings, safe_modulo
+from psyplot.plotter import START, Formatoption, Plotter, rcParams
 
-docstrings.params['replace_note'] = inspect.cleandoc("""
+docstrings.params["replace_note"] = inspect.cleandoc(
+    """
     You can insert any meta key from the :attr:`xarray.DataArray.attrs` via a
     string like ``'%%(key)s'``. Furthermore there are some special cases:
 
     - Strings like ``'%%Y'``, ``'%%b'``, etc. will be replaced using the
       :meth:`datetime.datetime.strftime` method as long as the data has a time
       coordinate and this can be converted to a :class:`~datetime.datetime`
       object.
@@ -54,19 +39,23 @@
       coordinate is one-dimensional in the data)
     - any attribute of one of the above coordinates is inserted via
       ``axis + key`` (e.g. the name of the x-coordinate can be inserted via
       ``'%%(xname)s'``).
     - Labels defined in the :class:`psyplot.rcParams` ``'texts.labels'`` key
       are also replaced when enclosed by '{}'. The standard labels are
 
-      - %s""" % '\n      - '.join(
-    '%s: ``%s``' % tuple(item) for item in six.iteritems(
-        rcParams['texts.labels'])))
+      - %s"""
+    % "\n      - ".join(
+        "%s: ``%s``" % tuple(item)
+        for item in six.iteritems(rcParams["texts.labels"])
+    )
+)
 
-docstrings.params['colors'] = inspect.cleandoc("""
+docstrings.params["colors"] = inspect.cleandoc(
+    """
     The following color abbreviations are supported:
 
     ==========  ========
     character   color
     ==========  ========
     'b'         blue
     'g'         green
@@ -77,44 +66,47 @@
     'k'         black
     'w'         white
     ==========  ========
 
     In addition, you can specify colors in many weird and wonderful ways,
     including full names (``'green'``), hex strings (``'#008000'``), RGB or
     RGBA tuples (``(0,1,0,1)``) or grayscale intensities as a string
-    (``'0.8'``).""")
+    (``'0.8'``)."""
+)
 
-docstrings.params['fontsizes'] = inspect.cleandoc("""
+docstrings.params["fontsizes"] = inspect.cleandoc(
+    """
     float
         The absolute font size in points (e.g., 12)
     string
         Strings might be 'xx-small', 'x-small', 'small', 'medium', 'large',
-        'x-large', 'xx-large'.""")
+        'x-large', 'xx-large'."""
+)
 
 
 class TextBase(object):
     """Abstract base class for formatoptions that provides a replace method"""
 
     delimiter = None
 
-    group = 'labels'
+    group = "labels"
 
     @property
     def enhanced_attrs(self):
         """The enhanced attributes of the array"""
         arr = self.data
         return self.get_enhanced_attrs(arr)
 
     @property
     def rc(self):
         """:class:`~psyplot.config.rcsetup.SubDict` of rcParams 'texts' key"""
         try:
             return self._rc
         except AttributeError:
-            return rcParams.find_and_replace(base_str=['texts.'])
+            return rcParams.find_and_replace(base_str=["texts."])
 
     data_dependent = True
 
     @docstrings.dedent
     def replace(self, s, data, attrs=None):
         """
         Replace the attributes of the plotter data in a string
@@ -133,35 +125,36 @@
             will be gained from `data.attrs`
 
         Returns
         -------
         str
             `s` with inserted informations"""
         # insert labels
-        s = s.format(**self.rc['labels'])
+        s = s.format(**self.rc["labels"])
         # replace attributes
         attrs = attrs or data.attrs
-        if hasattr(getattr(data, 'psy', None), 'arr_name'):
+        if hasattr(getattr(data, "psy", None), "arr_name"):
             attrs = attrs.copy()
-            attrs['arr_name'] = data.psy.arr_name
+            attrs["arr_name"] = data.psy.arr_name
         s = safe_modulo(s, attrs)
         # replace datetime.datetime like time informations
         if isinstance(data, InteractiveList):
             data = data[0]
         tname = self.any_decoder.get_tname(
-            next(self.plotter.iter_base_variables), data.coords)
+            next(self.plotter.iter_base_variables), data.coords
+        )
         if tname is not None and tname in data.coords:
             time = data.coords[tname]
             if not time.values.ndim:
                 try:  # assume a valid datetime.datetime instance
                     s = pd.to_datetime(str(time.values[()])).strftime(s)
                 except ValueError:
                     pass
         if six.PY2:
-            return s.decode('utf-8')
+            return s.decode("utf-8")
         return s
 
     def get_fig_data_attrs(self, delimiter=None):
         """Join the data attributes with other plotters in the project
 
         This method joins the attributes of the
         :class:`~psyplot.InteractiveBase` instances in the project that
@@ -176,57 +169,68 @@
 
         Returns
         -------
         dict
             A dictionary with all the meta attributes joined by the specified
             `delimiter`"""
         if self.project is not None:
-            delimiter = next(filter(lambda d: d is not None, [
-                delimiter, self.delimiter, self.rc['delimiter']]))
+            delimiter = next(
+                filter(
+                    lambda d: d is not None,
+                    [delimiter, self.delimiter, self.rc["delimiter"]],
+                )
+            )
             figs = self.project.figs
             fig = self.ax.get_figure()
             if self.plotter._initialized and fig in figs:
-                ret = figs[fig].joined_attrs(delimiter=delimiter,
-                                             plot_data=True)
+                ret = figs[fig].joined_attrs(
+                    delimiter=delimiter, plot_data=True
+                )
             else:
                 ret = self.get_enhanced_attrs(self.plotter.plot_data)
                 self.logger.debug(
-                    'Can not get the figure attributes because plot has not '
-                    'yet been initialized!')
+                    "Can not get the figure attributes because plot has not "
+                    "yet been initialized!"
+                )
             return ret
         else:
             return self.get_enhanced_attrs(self.plotter.plot_data)
 
     def get_enhanced_attrs(self, *args, **kwargs):
-        replot = kwargs.pop('replot', False)
-        if hasattr(self, '_enhanced_attrs') and not (
-                self.plotter.replot or replot):
+        replot = kwargs.pop("replot", False)
+        if hasattr(self, "_enhanced_attrs") and not (
+            self.plotter.replot or replot
+        ):
             return self._enhanced_attrs
         self._enhanced_attrs = self.plotter.get_enhanced_attrs(*args, **kwargs)
         return self._enhanced_attrs
 
     def get_fmt_widget(self, parent, project):
         """Create a combobox with the attributes"""
         from psy_simple.widgets.texts import LabelWidget
+
         return LabelWidget(parent, self, project)
 
 
-docstrings.params['fontweights'] = inspect.cleandoc("""
+docstrings.params["fontweights"] = inspect.cleandoc(
+    """
     float
         a float between 0 and 1000
     string
         Possible strings are one of 'ultralight', 'light', 'normal',
         'regular', 'book', 'medium', 'roman', 'semibold', 'demibold',
-        'demi', 'bold', 'heavy', 'extra bold', 'black'.""")
+        'demi', 'bold', 'heavy', 'extra bold', 'black'."""
+)
 
 
-@docstrings.get_sections(base='label_weight')
+@docstrings.get_sections(base="label_weight")
 @dedent
-def label_weight(base, label_name=None, children=[], parents=[],
-                 dependencies=[]):
+def label_weight(
+    base, label_name=None, children=[], parents=[], dependencies=[]
+):
     """
     Function that returns a Formatoption class for modifying the fontweight
 
     This function returns a :class:`~psyplot.plotter.Formatoption` instance
     that modifies the weight of the given `base` formatoption
 
     Parameters
@@ -268,42 +272,50 @@
 
         Possible types
         --------------
         %%(fontweights)s
 
         See Also
         --------
-        %s, %s, %s""" % (label_name, base.key, base.key + 'size',
-                         base.key + 'props')
-        children = [base.key] + \
-            cl_children
-        parent = [base.key + 'props'] + cl_parents
+        %s, %s, %s""" % (
+            label_name,
+            base.key,
+            base.key + "size",
+            base.key + "props",
+        )
+        children = [base.key] + cl_children
+        parent = [base.key + "props"] + cl_parents
         dependencies = cl_dependencies
 
-        group = 'labels'
+        group = "labels"
 
-        name = 'Font weight of ' + (base.name or base.key)
+        name = "Font weight of " + (base.name or base.key)
 
         def update(self, value):
             for text in getattr(self, base.key).texts:
                 text.set_weight(value)
 
         def get_fmt_widget(self, parent, project):
             """Get a widget with the different font weights"""
             from psy_simple.widgets.texts import FontWeightWidget
+
             return FontWeightWidget(
-                parent, self, next(iter(getattr(self, base.key).texts), None),
-                base)
+                parent,
+                self,
+                next(iter(getattr(self, base.key).texts), None),
+                base,
+            )
 
-    return LabelWeight(base.key + 'weight')
+    return LabelWeight(base.key + "weight")
 
 
 @docstrings.dedent
-def label_size(base, label_name=None, children=[], parents=[],
-               dependencies=[]):
+def label_size(
+    base, label_name=None, children=[], parents=[], dependencies=[]
+):
     """
     Function that returns a Formatoption class for modifying the fontsite
 
     This function returns a :class:`~psyplot.plotter.Formatoption` instance
     that modifies the size of the given `base` formatoption
 
     Parameters
@@ -329,44 +341,53 @@
 
         Possible types
         --------------
         %%(fontsizes)s
 
         See Also
         --------
-        %s, %s, %s""" % (label_name, base.key, base.key + 'weight',
-                         base.key + 'props')
+        %s, %s, %s""" % (
+            label_name,
+            base.key,
+            base.key + "weight",
+            base.key + "props",
+        )
         children = [base.key] + cl_children
-        parent = [base.key + 'props'] + cl_parents
+        parent = [base.key + "props"] + cl_parents
         dependencies = cl_dependencies
 
-        group = 'labels'
+        group = "labels"
 
-        name = 'Font size of ' + (base.name or base.key)
+        name = "Font size of " + (base.name or base.key)
 
         def update(self, value):
             for text in getattr(self, base.key).texts:
                 text.set_size(value)
 
         def get_fmt_widget(self, parent, project):
             """Get a widget with the different font weights"""
             from psy_simple.widgets.texts import FontSizeWidget
+
             return FontSizeWidget(
-                parent, self, next(iter(getattr(self, base.key).texts), None),
-                base)
+                parent,
+                self,
+                next(iter(getattr(self, base.key).texts), None),
+                base,
+            )
 
-    return LabelSize(base.key + 'size')
+    return LabelSize(base.key + "size")
 
 
-docstrings.keep_params('label_weight.parameters', 'base', 'label_name')
+docstrings.keep_params("label_weight.parameters", "base", "label_name")
 
 
 @docstrings.dedent
-def label_props(base, label_name=None, children=[], parents=[],
-                dependencies=[]):
+def label_props(
+    base, label_name=None, children=[], parents=[], dependencies=[]
+):
     """
     Function that returns a Formatoption class for modifying the fontsite
 
     This function returns a :class:`~psyplot.plotter.Formatoption` instance
     that modifies the size of the given `base` formatoption
 
     Parameters
@@ -402,24 +423,31 @@
         Possible types
         --------------
         dict
             Items may be any valid text property
 
         See Also
         --------
-        %s, %s, %s""" % (label_name, base.key, base.key + 'size',
-                         base.key + 'weight')
+        %s, %s, %s""" % (
+            label_name,
+            base.key,
+            base.key + "size",
+            base.key + "weight",
+        )
         children = cl_children
         parents = cl_parents
-        dependencies = [base.key, base.key + 'size', base.key + 'weight'] + \
-            cl_dependencies
+        dependencies = [
+            base.key,
+            base.key + "size",
+            base.key + "weight",
+        ] + cl_dependencies
 
-        group = 'labels'
+        group = "labels"
 
-        name = 'Font properties of ' + (base.name or base.key)
+        name = "Font properties of " + (base.name or base.key)
 
         def __init__(self, *args, **kwargs):
             super(LabelProps, self).__init__(*args, **kwargs)
             self.default_props = {}
             self._todefault = False
 
         def set_value(self, value, validate=True, todefault=False):
@@ -435,38 +463,42 @@
                 return
             # TODO: This handling of the default management is not really
             # satisfying because you run into troubles when using alternate
             # property names (e.g. if you use 'ha' and 'horizontalalignment'
             # at the same time)
             if not self._todefault:
                 for key in fontprops:
-                    if key == 'bbox':
-                        default = dict(facecolor='none', edgecolor='none')
+                    if key == "bbox":
+                        default = dict(facecolor="none", edgecolor="none")
                     else:
-                        default = getattr(text, 'get_' + key)()
+                        default = getattr(text, "get_" + key)()
                     self.default_props.setdefault(key, default)
             else:
                 fontprops = self.default_props.copy()
                 self.default_props.clear()
-            if 'size' not in fontprops and 'fontsize' not in fontprops:
-                fontprops['size'] = getattr(self, base.key + 'size').value
-            if 'weight' not in fontprops and 'fontweight' not in fontprops:
-                fontprops['weight'] = getattr(self, base.key + 'weight').value
+            if "size" not in fontprops and "fontsize" not in fontprops:
+                fontprops["size"] = getattr(self, base.key + "size").value
+            if "weight" not in fontprops and "fontweight" not in fontprops:
+                fontprops["weight"] = getattr(self, base.key + "weight").value
             for text in getattr(self, base.key).texts:
                 text.update(fontprops)
             self._todefault = False
 
         def get_fmt_widget(self, parent, project):
             """Get a widget with the different font weights"""
             from psy_simple.widgets.texts import FontPropertiesWidget
+
             return FontPropertiesWidget(
-                parent, self, next(iter(getattr(self, base.key).texts), None),
-                base)
+                parent,
+                self,
+                next(iter(getattr(self, base.key).texts), None),
+                base,
+            )
 
-    return LabelProps(base.key + 'props')
+    return LabelProps(base.key + "props")
 
 
 class Title(TextBase, Formatoption):
     """
     Show the title
 
     Set the title of the plot.
@@ -482,25 +514,29 @@
     This is the title of this specific subplot! For the title of the whole
     figure, see the :attr:`figtitle` formatoption.
 
     See Also
     --------
     figtitle, titlesize, titleweight, titleprops"""
 
-    name = 'Axes title'
+    name = "Axes title"
 
     def initialize_plot(self, value):
         arr = self.data
-        self.texts = [self.ax.set_title(
-            self.replace(value, arr, attrs=self.enhanced_attrs))]
+        self.texts = [
+            self.ax.set_title(
+                self.replace(value, arr, attrs=self.enhanced_attrs)
+            )
+        ]
 
     def update(self, value):
         arr = self.data
-        self.texts[0].set_text(self.replace(
-            value, arr, attrs=self.enhanced_attrs))
+        self.texts[0].set_text(
+            self.replace(value, arr, attrs=self.enhanced_attrs)
+        )
 
 
 class Figtitle(TextBase, Formatoption):
     """
     Plot a figure title
 
     Set the title of the figure.
@@ -522,35 +558,39 @@
     - This is the title of the whole figure! For the title of this specific
       subplot, see the :attr:`title` formatoption.
 
     See Also
     --------
     title, figtitlesize, figtitleweight, figtitleprops"""
 
-    name = 'Figure title'
+    name = "Figure title"
 
     @property
     def enhanced_attrs(self):
         return self.get_fig_data_attrs()
 
     def initialize_plot(self, s):
         if s:
-            self.texts = [self.ax.get_figure().suptitle(
-                self.replace(s, self.plotter.data, self.enhanced_attrs))]
+            self.texts = [
+                self.ax.get_figure().suptitle(
+                    self.replace(s, self.plotter.data, self.enhanced_attrs)
+                )
+            ]
             self.clear_other_texts()
         else:
-            self.texts = [self.ax.get_figure().suptitle('')]
+            self.texts = [self.ax.get_figure().suptitle("")]
 
     def update(self, s):
         if s:
-            self.texts[0].set_text(self.replace(s, self.plotter.data,
-                                                self.enhanced_attrs))
+            self.texts[0].set_text(
+                self.replace(s, self.plotter.data, self.enhanced_attrs)
+            )
             self.clear_other_texts()
         else:
-            self.texts[0].set_text('')
+            self.texts[0].set_text("")
 
     def clear_other_texts(self, remove=False):
         """Make sure that no other text is a the same position as this one
 
         This method clears all text instances in the figure that are at the
         same position as the :attr:`_text` attribute
 
@@ -564,15 +604,15 @@
         if len(fig.texts) == 1:
             return
         for i, text in enumerate(fig.texts):
             if text == self._text:
                 continue
             if text.get_position() == self._text.get_position():
                 if not remove:
-                    text.set_text('')
+                    text.set_text("")
                 else:
                     del fig[i]
 
 
 class Text(TextBase, Formatoption):
     """
     Add text anywhere on the plot
@@ -598,23 +638,25 @@
     empty list
         remove all texts from the plot
 
     See Also
     --------
     title, figtitle"""
 
-    name = 'Arbitrary text on the plot'
+    name = "Arbitrary text on the plot"
 
     @property
     def transform(self):
         """Dictionary containing the relevant transformations"""
         ax = self.ax
-        return {'axes': ax.transAxes,
-                'fig': ax.get_figure().transFigure,
-                'data': ax.transData}
+        return {
+            "axes": ax.transAxes,
+            "fig": ax.get_figure().transFigure,
+            "data": ax.transData,
+        }
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         #: texts that shall be removed when updating
         self._texts_to_remove = set()
         #: :class:`matplotlib.texts.Text` instances on the figure
         self._texts = defaultdict(set)
@@ -666,40 +708,45 @@
                 try:
                     self._update_texttuple(x, y, s, cs, d)
                 except ValueError:
                     self.value.append((x, y, s, cs, d))
 
     def update(self, value, texts_to_remove=None):
         # remove texts
-        for (x, y, cs) in texts_to_remove or self._texts_to_remove:
+        for x, y, cs in texts_to_remove or self._texts_to_remove:
             for t in self._texts[cs]:
                 if (x, y) == t.get_position():
                     self._texts[cs].remove(t)
                     t.remove()
                     break
         if self.plotter.replot:
             value = self.value + value
         # now update the old texts or create new ones
         for x, y, s, cs, d in value:
-            if cs == 'fig':
+            if cs == "fig":
                 s = self.replace(
-                    s, self.plotter.data, self.get_fig_data_attrs(
-                        d.pop('delimiter', None)))
+                    s,
+                    self.plotter.data,
+                    self.get_fig_data_attrs(d.pop("delimiter", None)),
+                )
             else:
                 s = self.replace(s, self.plotter.data, self.enhanced_attrs)
             found = False
             for t in self._texts[cs]:
                 if (x, y) == t.get_position():
                     t.set_text(s)
                     t.update(d.copy())
                     found = True
                     break
             if not found:
-                self._texts[cs].add(self.ax.text(
-                    x, y, s, d.copy(), transform=self.transform[cs]))
+                self._texts[cs].add(
+                    self.ax.text(
+                        x, y, s, d.copy(), transform=self.transform[cs]
+                    )
+                )
 
     def share(self, fmto, **kwargs):
         """Share the settings of this formatoption with other data objects
 
         Parameters
         ----------
         fmto: Formatoption
@@ -709,21 +756,22 @@
             method of `fmto`
 
         Notes
         -----
         The Text formatoption sets the 'texts_to_remove' keyword to the
         :attr:`_texts_to_remove` attribute of this instance (if not already
         specified in ``**kwargs``"""
-        kwargs.setdefault('texts_to_remove', self._texts_to_remove)
+        kwargs.setdefault("texts_to_remove", self._texts_to_remove)
         super(Text, self).share(fmto, **kwargs)
 
     def diff(self, value):
         my_value = self.value
         return (not len(value) and len(my_value)) or any(
-            val not in my_value for val in value)
+            val not in my_value for val in value
+        )
 
     def finish_update(self):
         """Clears the :attr:`_texts_to_remove` set"""
         self._texts_to_remove.clear()
 
     def remove(self):
         for t in chain.from_iterable(six.itervalues(self._texts)):
@@ -744,17 +792,17 @@
         True for automatic adjustment
 
     Warnings
     --------
     There is no update method to undo what happend after this formatoption is
     set to True!"""
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Tight layout'
+    name = "Tight layout"
 
     def update(self, value):
         if value:
             plt.sca(self.ax)
             plt.tight_layout()
 
 
@@ -767,39 +815,41 @@
         to use matplotlibs rc params
     None
         to use a transparent color
     color
         Any possible matplotlib color
     """
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Background color of the plot'
+    name = "Background color of the plot"
 
     def update(self, value):
-        if value == 'rc':
-            self.ax.patch.set_facecolor(plt.rcParams['axes.facecolor'])
-            self.ax.set_facecolor(plt.rcParams['axes.facecolor'])
+        if value == "rc":
+            self.ax.patch.set_facecolor(plt.rcParams["axes.facecolor"])
+            self.ax.set_facecolor(plt.rcParams["axes.facecolor"])
         elif value is None:
-            self.ax.patch.set_facecolor('none')
-            self.ax.set_facecolor('none')
+            self.ax.patch.set_facecolor("none")
+            self.ax.set_facecolor("none")
         else:
             self.ax.patch.set_facecolor(value)
             self.ax.set_facecolor(value)
 
     def get_fmt_widget(self, parent, project):
         from psy_simple.widgets.colors import BackGroundColorWidget
+
         return BackGroundColorWidget(parent, self, project)
 
 
 class ValueMaskBase(Formatoption):
     """Base class for masking formatoptions"""
+
     priority = START
 
-    group = 'masking'
+    group = "masking"
 
     data_dependent = True
 
     @abstractmethod
     def mask_func(self):
         """The masking function that is called"""
         return
@@ -810,15 +860,16 @@
         else:
             for i, data in enumerate(self.iter_data):
                 self.set_data(self._mask_data(data, value), i)
 
     def _mask_data(self, data, value):
         data = data.copy(data=np.copy(data.values))
         data.values[~np.isnan(data.values)] = self.mask_func(
-            data.values[~np.isnan(data.values)], value)
+            data.values[~np.isnan(data.values)], value
+        )
         return data
 
 
 class MaskLess(ValueMaskBase):
     """
     Mask data points smaller than a number
 
@@ -828,15 +879,15 @@
         The floating number to mask below
 
     See Also
     --------
     maskleq, maskgreater, maskgeq, maskbetween
     """
 
-    name = 'Mask less'
+    name = "Mask less"
 
     def mask_func(self, data, value):
         data[data < value] = np.nan
         return data
 
 
 class MaskLeq(ValueMaskBase):
@@ -849,15 +900,15 @@
         The floating number to mask below
 
     See Also
     --------
     maskless, maskgreater, maskgeq, maskbetween
     """
 
-    name = 'Mask lesser than or equal'
+    name = "Mask lesser than or equal"
 
     def mask_func(self, data, value):
         data[data <= value] = np.nan
         return data
 
 
 class MaskGreater(ValueMaskBase):
@@ -870,15 +921,15 @@
         The floating number to mask above
 
     See Also
     --------
     maskless, maskleq, maskgeq, maskbetween
     """
 
-    name = 'Mask greater'
+    name = "Mask greater"
 
     def mask_func(self, data, value):
         data[data > value] = np.nan
         return data
 
 
 class MaskGeq(ValueMaskBase):
@@ -891,15 +942,15 @@
         The floating number to mask above
 
     See Also
     --------
     maskless, maskleq, maskgreater, maskbetween
     """
 
-    name = 'Mask greater than or equal'
+    name = "Mask greater than or equal"
 
     def mask_func(self, data, value):
         data[data >= value] = np.nan
         return data
 
 
 class MaskBetween(ValueMaskBase):
@@ -912,15 +963,15 @@
         The floating number to mask above
 
     See Also
     --------
     maskless, maskleq, maskgreater, maskgeq
     """
 
-    name = 'Mask between two values'
+    name = "Mask between two values"
 
     def mask_func(self, data, value):
         data[np.all([data >= value[0], data <= value[1]], axis=0)] = np.nan
         return data
 
 
 class Mask(Formatoption):
@@ -949,15 +1000,15 @@
         The path to a netCDF file that shall be loaded
     xr.DataArray or np.ndarray
         An array that can be broadcasted to the shape of the data
     """
 
     priority = START
 
-    group = 'masking'
+    group = "masking"
 
     name = "Apply a mask"
 
     def update(self, value):
         if value is None:
             return
         for i, data in enumerate(self.iter_data):
@@ -967,81 +1018,94 @@
             new_data.psy.idims = data.psy.idims
             self.set_data(new_data, i)
 
     def diff(self, value):
         try:
             return bool(self.value != value)
         except ValueError:
-            if hasattr(value, 'shape') and hasattr(self.value, 'shape'):
-                return ((value.shape != self.value.shape) |
-                        (value != self.value).any())
+            if hasattr(value, "shape") and hasattr(self.value, "shape"):
+                return (value.shape != self.value.shape) | (
+                    value != self.value
+                ).any()
             else:
                 return True
 
     def load_mask(self, data, value):
         if isinstance(value, str) and value in data.psy.base:
             mask = data.psy.base[value]
             if not set(mask.dims).intersection(data.dims):
-                raise ValueError("No intersection between dimensions of mask "
-                                 f"{value}: {mask.dims}, and the data: "
-                                 f"{data.dims}")
+                raise ValueError(
+                    "No intersection between dimensions of mask "
+                    f"{value}: {mask.dims}, and the data: "
+                    f"{data.dims}"
+                )
         elif isinstance(value, str):
             try:
                 mask = open_dataset(value)
             except Exception:
                 raise ValueError(
                     f"{value} is not in the base dataset of "
                     f"{data.psy.arr_name} and could not be loaded with "
-                    f"psy.open_dataset({repr(value)})")
+                    f"psy.open_dataset({repr(value)})"
+                )
             else:
                 available_vars = [
-                    v for v in mask
-                    if set(mask[v].dims).intersection(data.dims)]
+                    v
+                    for v in mask
+                    if set(mask[v].dims).intersection(data.dims)
+                ]
                 if not available_vars:
-                    raise ValueError(f"No variable in {value} has an overlap "
-                                     f"with the data dimensions {data.dims}")
+                    raise ValueError(
+                        f"No variable in {value} has an overlap "
+                        f"with the data dimensions {data.dims}"
+                    )
                 else:
                     mask = mask[available_vars[0]]
         else:
             mask = value
         base_var = next(data.psy.iter_base_variables)
 
         # aggregate mask over dimensions that are not in the base variable
         dims2agg = set(mask.dims).difference(set(base_var.dims))
         if dims2agg:
             mask = mask.any(list(dims2agg))
 
         # select idims of mask
-        idims = {d: sl for d, sl in data.psy.idims.items()
-                 if d in mask.dims and d not in data.dims}
+        idims = {
+            d: sl
+            for d, sl in data.psy.idims.items()
+            if d in mask.dims and d not in data.dims
+        }
         if idims:
             mask = mask.isel(**idims)
 
         return mask
 
 
 class TitlesPlotter(Plotter):
     """Plotter class for labels"""
-    _rcparams_string = ['plotter.baseplotter.']
-    title = Title('title')
+
+    _rcparams_string = ["plotter.baseplotter."]
+    title = Title("title")
     titlesize = label_size(title)
     titleweight = label_weight(title)
     titleprops = label_props(title)
-    figtitle = Figtitle('figtitle')
-    figtitlesize = label_size(figtitle, 'figure title')
-    figtitleweight = label_weight(figtitle, 'figure title')
-    figtitleprops = label_props(figtitle, 'figure title')
-    text = Text('text')
+    figtitle = Figtitle("figtitle")
+    figtitlesize = label_size(figtitle, "figure title")
+    figtitleweight = label_weight(figtitle, "figure title")
+    figtitleprops = label_props(figtitle, "figure title")
+    text = Text("text")
 
 
 class BasePlotter(TitlesPlotter):
     """Base class with formatoptions for plotting on an matplotlib axes"""
-    _rcparams_string = ['plotter.baseplotter.']
 
-    tight = Tight('tight')
-    background = BackgroundColor('background')
-    maskless = MaskLess('maskless')
-    maskleq = MaskLeq('maskleq')
-    maskgreater = MaskGreater('maskgreater')
-    maskgeq = MaskGeq('maskgeq')
-    maskbetween = MaskBetween('maskbetween')
-    mask = Mask('mask')
+    _rcparams_string = ["plotter.baseplotter."]
+
+    tight = Tight("tight")
+    background = BackgroundColor("background")
+    maskless = MaskLess("maskless")
+    maskleq = MaskLeq("maskleq")
+    maskgreater = MaskGreater("maskgreater")
+    maskgeq = MaskGeq("maskgeq")
+    maskbetween = MaskBetween("maskbetween")
+    mask = Mask("mask")
```

### Comparing `psy-simple-1.4.1/psy_simple/plotters.py` & `psy-simple-1.5.0/psy_simple/plotters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 """Plotters and formatoptions for the psy-simple plugin."""
 
-# Disclaimer
-# ----------
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum Hereon
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
 #
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-simple and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
-#
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
 import re
-from warnings import warn
-from psyplot.warning import PsyPlotRuntimeWarning
-from abc import abstractproperty, abstractmethod
-from functools import partial
-from itertools import chain, starmap, cycle, islice, repeat
-from pandas import (
-    date_range, to_datetime, DatetimeIndex, to_timedelta, MultiIndex)
 import weakref
-from pandas.tseries import offsets
-import xarray as xr
+from abc import abstractmethod, abstractproperty
+from functools import partial
+from itertools import chain, cycle, islice, repeat, starmap
+from warnings import warn
+
 import matplotlib as mpl
-import matplotlib.axes
-from matplotlib.ticker import FormatStrFormatter, FixedLocator, FixedFormatter
-from matplotlib.dates import DateFormatter, AutoDateFormatter
-import matplotlib.colors as mcol
 import numpy as np
-from psyplot.docstring import docstrings, dedent
+import six
+import xarray as xr
+from matplotlib.dates import AutoDateFormatter, DateFormatter
+from matplotlib.ticker import FixedFormatter, FixedLocator, FormatStrFormatter
+from pandas import (
+    DatetimeIndex,
+    MultiIndex,
+    date_range,
+    to_datetime,
+    to_timedelta,
+)
+from pandas.tseries import offsets
+from psyplot.data import (
+    CFDecoder,
+    InteractiveList,
+    _infer_interval_breaks,
+    isstring,
+)
+from psyplot.docstring import dedent, docstrings
 from psyplot.plotter import (
-    Plotter, Formatoption, BEFOREPLOTTING, DictFormatoption, END, rcParams,
-    START)
+    BEFOREPLOTTING,
+    END,
+    START,
+    DictFormatoption,
+    Formatoption,
+    Plotter,
+)
+from psyplot.utils import is_iterable
+from psyplot.warning import PsyPlotRuntimeWarning
+
 from psy_simple.base import (
-    BasePlotter, TextBase, label_size, label_weight, label_props, MaskLess,
-    MaskGreater, MaskBetween, MaskLeq, MaskGeq, Mask)
+    BasePlotter,
+    Mask,
+    MaskBetween,
+    MaskGeq,
+    MaskGreater,
+    MaskLeq,
+    MaskLess,
+    TextBase,
+    label_props,
+    label_size,
+    label_weight,
+)
 from psy_simple.colors import get_cmap
-from psyplot.data import (
-    InteractiveList, isstring, CFDecoder, _infer_interval_breaks)
-from psyplot.compat.pycompat import map, zip, range
-from psy_simple.plugin import (
-    validate_color, validate_float, safe_list as slist)
-from psyplot.utils import is_iterable
+from psy_simple.plugin import safe_list as slist
+from psy_simple.plugin import validate_color, validate_float
 
 
 def _get_index_vals(index):
-    if (isinstance(index, MultiIndex) and
-            len(index.names) == 1):
+    if isinstance(index, MultiIndex) and len(index.names) == 1:
         return index.get_level_values(0).values
     else:
         return index.values
 
 
-mpl_version = float('.'.join(mpl.__version__.split('.')[:2]))
+mpl_version = float(".".join(mpl.__version__.split(".")[:2]))
 
 
-def round_to_05(n, exp=None, mode='s'):
+def round_to_05(n, exp=None, mode="s"):
     """
     Round to the next 0.5-value.
 
     This function applies the round function `func` to round `n` to the
     next 0.5-value with respect to its exponent with base 10 (i.e.
     1.3e-4 will be rounded to 1.5e-4) if `exp` is None or with respect
     to the given exponent in `exp`.
@@ -102,29 +107,33 @@
         >>> a = [-100.3, 40.6, 8.7, -0.00023]
         >>>round_to_05(a, mode='s')
         array([ -1.00000000e+02,   4.00000000e+01,   8.50000000e+00,
                 -2.00000000e-04])
 
         >>> round_to_05(a, mode='l')
         array([ -1.50000000e+02,   4.50000000e+01,   9.00000000e+00,
-                -2.50000000e-04])"""
+                -2.50000000e-04])
+    """
     n = np.asarray(n)
     if exp is None:
         exp = np.floor(np.log10(np.abs(n)))  # exponent for base 10
-    ntmp = np.abs(n)/10.**exp  # mantissa for base 10
-    if mode == 's':
+    ntmp = np.abs(n) / 10.0**exp  # mantissa for base 10
+    if mode == "s":
         n1 = ntmp
-        s = 1.
+        s = 1.0
         n2 = nret = np.floor(ntmp)
     else:
         n1 = nret = np.ceil(ntmp)
-        s = -1.
+        s = -1.0
         n2 = ntmp
-    return np.where(n1 - n2 > 0.5, np.sign(n)*(nret + s*0.5)*10.**exp,
-                    np.sign(n)*nret*10.**exp)
+    return np.where(
+        n1 - n2 > 0.5,
+        np.sign(n) * (nret + s * 0.5) * 10.0**exp,
+        np.sign(n) * nret * 10.0**exp,
+    )
 
 
 def convert_radian(coord, *variables):
     """Convert the given coordinate from radian to degree
 
     Parameters
     ----------
@@ -137,18 +146,18 @@
     -------
     xr.Variable
         The transformed variable if one of the given `variables` has units in
         radian"""
     warn(
         "The psy_simple.plotters.convert_radian method has been deprecated."
         "Please use the `plotter.convert_coordinate` instead.",
-        DeprecationWarning
+        DeprecationWarning,
     )
-    if any(v.attrs.get('units', '').startswith('radian') for v in variables):
-        return coord * 180. / np.pi
+    if any(v.attrs.get("units", "").startswith("radian") for v in variables):
+        return coord * 180.0 / np.pi
     return coord
 
 
 class AlternativeXCoord(Formatoption):
     """
     Use an alternative variable as x-coordinate
 
@@ -199,19 +208,20 @@
 
         >>> plotter = psy.plot.lineplot(
         ...     ds, name=['temp'], coord='std').plotters[0]
 
         >>> plotter.plot_data[0].dims
         ('std',)
 
-    and ``'std'`` is plotted on the x-axis."""
+    and ``'std'`` is plotted on the x-axis.
+    """
 
-    name = 'Alternative X-Variable'
+    name = "Alternative X-Variable"
 
-    group = 'data'
+    group = "data"
 
     priority = START
 
     data_dependent = True
 
     #: Bool. If True, this Formatoption directly uses the raw_data, otherwise
     #: use the normal data
@@ -224,16 +234,18 @@
     def update(self, value):
         if value is not None:
             for i, da in enumerate(self.data_iterator):
                 self.set_data(self.replace_coord(i), i)
 
     def diff(self, value):
         try:
-            return ~((np.shape(value) == np.shape(self.value)) &
-                     np.all(value == self.value))
+            return not (
+                (np.shape(value) == np.shape(self.value))
+                and np.all(value == self.value)
+            )
         except TypeError:
             return True
 
     def replace_coord(self, i):
         """Replace the coordinate for the data array at the given position
 
         Parameters
@@ -241,29 +253,34 @@
         i: int
             The number of the data array in the raw data (if the raw data is
             not an interactive list, use 0)
 
         Returns
         xarray.DataArray
             The data array with the replaced coordinate"""
-        da = next(islice(self.data_iterator, i, i+1))
+        da = next(islice(self.data_iterator, i, i + 1))
         name, coord = self.get_alternative_coord(da, i)
-        other_coords = {key: da.coords[key]
-                        for key in set(da.coords).difference(da.dims)}
-        ret = da.rename({da.dims[-1]: name}).assign_coords(
-            **{name: coord}).assign_coords(**other_coords)
+        other_coords = {
+            key: da.coords[key] for key in set(da.coords).difference(da.dims)
+        }
+        ret = (
+            da.rename({da.dims[-1]: name})
+            .assign_coords(**{name: coord})
+            .assign_coords(**other_coords)
+        )
         return ret
 
     def get_alternative_coord(self, da, i):
         if isinstance(self.value, xr.DataArray):
             return self.value.name, self.value.variable
-        alternative_name = next(islice(cycle(slist(self.value)), i, i+1))
+        alternative_name = next(islice(cycle(slist(self.value)), i, i + 1))
         coord_da = InteractiveList.from_dataset(
-            da.psy.base, name=alternative_name, dims=da.psy.idims)[0]
-        coord = xr.Variable((coord_da.name, ), coord_da, coord_da.attrs)
+            da.psy.base, name=alternative_name, dims=da.psy.idims
+        )[0]
+        coord = xr.Variable((coord_da.name,), coord_da, coord_da.attrs)
         return coord_da.name, coord
 
 
 class AlternativeXCoordPost(AlternativeXCoord):
     # The same as the :class:`AlternativeXCoord, but it uses the
     # :attr:`psyplot.plotter.Formatoption.data` attribute as a src, not the
     # :attr:`psyplot.plotter.Formatoption.raw_data`
@@ -291,17 +308,17 @@
     string, tuple.
         Defines the color of the grid.
 
     Notes
     -----
     %(colors)s"""
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Grid lines'
+    name = "Grid lines"
 
     def update(self, value):
         if self.plotter._initialized and mpl_version == 3.3:
             warn("Updating grids is known to malfunction for matplotlib 3.3!")
         try:
             value = validate_color(value)
             self.ax.grid(color=value)
@@ -321,51 +338,57 @@
         Keys may be one of {'right', 'left', 'bottom', 'top'},  the values can
         be any valid color or None.
 
     Notes
     -----
     %(colors)s"""
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Color of x- and y-axes'
+    name = "Color of x- and y-axes"
 
     @property
     def value2pickle(self):
         """Return the current axis colors"""
         return {key: s.get_edgecolor() for key, s in self.ax.spines.items()}
 
     def initialize_plot(self, value):
-        positions = ['right', 'left', 'bottom', 'top']
+        positions = ["right", "left", "bottom", "top"]
         #: :class:`dict` storing the default linewidths
-        self.default_lw = dict(zip(positions, map(
-            lambda pos: self.ax.spines[pos].get_linewidth(), positions)))
+        self.default_lw = dict(
+            zip(
+                positions,
+                map(
+                    lambda pos: self.ax.spines[pos].get_linewidth(), positions
+                ),
+            )
+        )
         self.update(value)
 
     def update(self, value):
         for pos, color in six.iteritems(value):
             spine = self.ax.spines[pos]
             spine.set_color(color)
             if color is not None and spine.get_linewidth() == 0.0:
                 spine.set_linewidth(1.0)
             elif color is None:
-                spine.set_color(mpl.rcParams['axes.edgecolor'])
+                spine.set_color(mpl.rcParams["axes.edgecolor"])
                 spine.set_linewidth(self.default_lw[pos])
 
 
 class TicksManagerBase(Formatoption):
     """
     Abstract base class for formatoptions handling ticks"""
 
     @abstractmethod
     def update_axis(self, val):
         pass
 
 
-@docstrings.get_sections(base='TicksManager')
+@docstrings.get_sections(base="TicksManager")
 class TicksManager(TicksManagerBase, DictFormatoption):
     """
     Abstract base class for ticks formatoptions controlling major and minor
     ticks
 
     This formatoption simply serves as a base that allows the simultaneous
     managment of major and minor ticks
@@ -375,23 +398,23 @@
     dict
         A dictionary with the keys ``'minor'`` and (or) ``'major'`` to specify
         which ticks are managed. If the given value is not a dictionary with
         those keys, it is put into a dictionary with the key determined by the
         rcParams ``'ticks.which'`` key (usually ``'major'``).
         The values in the dictionary can be one types below."""
 
-    group = 'ticks'
+    group = "ticks"
 
     def update(self, value):
         for which, val in six.iteritems(value):
             self.which = which
             self.update_axis(val)
 
 
-@docstrings.get_sections(base='DataTicksCalculator')
+@docstrings.get_sections(base="DataTicksCalculator")
 class DataTicksCalculator(Formatoption):
     """
     Abstract base formatoption to calculate ticks and bounds from the data
 
     Possible types
     --------------
     numeric array
@@ -455,35 +478,36 @@
 
     data_dependent = True
 
     @property
     def full_array(self):
         """The full array of this and the shared data"""
         return np.concatenate(
-            [self.array] + [fmto.array for fmto in self.shared])
+            [self.array] + [fmto.array for fmto in self.shared]
+        )
 
     @property
     def array(self):
         """The numpy array of the data"""
         data = self.data
-        if not hasattr(data, 'notnull'):
+        if not hasattr(data, "notnull"):
             data = data.to_series()
         mask = np.asarray(data.notnull())
         return data.values[mask]
 
     def _data_ticks(self, step=None, *args, **kwargs):
         step = step or 1
         """Array of ticks that match exactly the data"""
         return np.unique(self.array)[::step]
 
     def _mid_data_ticks(self, step=None, *args, **kwargs):
         step = step or 1
         """Array of ticks in the middle between the data points"""
         arr = np.unique(self.array)
-        return ((arr[:-1] + arr[1:])/2.)[::step]
+        return ((arr[:-1] + arr[1:]) / 2.0)[::step]
 
     def _collect_array(self, percmin=None, percmax=None):
         """Collect the data from the shared formatoptions (if necessary)."""
 
         def nanmin(arr):
             try:
                 return np.nanmin(arr)
@@ -511,25 +535,27 @@
                 fmto._release_children()
 
         if not self.shared:
             arr = self.array
         else:
             # np.concatenate all arrays if any of the percentiles are required
             if percmin is not None or percmax is not None:
-                arr = np.concatenate(tuple(chain(
-                    [self.array], shared_arrays())))
+                arr = np.concatenate(
+                    tuple(chain([self.array], shared_arrays()))
+                )
             # np.concatenate only min and max-values instead of the full arrays
             else:
-                arr = np.concatenate(tuple(map(minmax, chain(
-                    [self.array], shared_arrays()))))
+                arr = np.concatenate(
+                    tuple(map(minmax, chain([self.array], shared_arrays())))
+                )
         return arr
 
-    def _calc_vmin_vmax(self, percmin=None, percmax=None,
-                        vmin=None, vmax=None):
-
+    def _calc_vmin_vmax(
+        self, percmin=None, percmax=None, vmin=None, vmax=None
+    ):
         def nanmin(arr):
             try:
                 return np.nanmin(arr)
             except TypeError:
                 return arr.min()
 
         def nanmax(arr):
@@ -554,52 +580,55 @@
                 pass
             elif percmax is None or percmax == 100:
                 vmax = nanmax(arr)
             else:
                 percentiles.append(percmax)
         except ValueError:
             self.logger.warn(
-                'Cannot calculate minimum and maximum of the data!',
-                exc_info=True)
+                "Cannot calculate minimum and maximum of the data!",
+                exc_info=True,
+            )
             return 0, 1
         if percentiles:
             percentiles = iter(np.percentile(arr, percentiles))
             if percmin:
                 vmin = next(percentiles)
             if percmax and percmax < 100:
                 vmax = next(percentiles)
         return vmin, vmax
 
     @staticmethod
     def _round_min_max(vmin, vmax):
         if vmin == vmax:
             return vmin, vmax
         exp = np.floor(np.log10(abs(vmax - vmin)))
-        larger = round_to_05([vmin, vmax], exp, mode='l')
-        smaller = round_to_05([vmin, vmax], exp, mode='s')
+        larger = round_to_05([vmin, vmax], exp, mode="l")
+        smaller = round_to_05([vmin, vmax], exp, mode="s")
         return min([larger[0], smaller[0]]), max([larger[1], smaller[1]])
 
     def _rounded_ticks(self, N=None, *args, **kwargs):
         N = N or 11
         vmin, vmax = self._round_min_max(
-            *self._calc_vmin_vmax(*args, **kwargs))
+            *self._calc_vmin_vmax(*args, **kwargs)
+        )
         return np.linspace(vmin, vmax, N, endpoint=True)
 
     def _log_bounds(self, expmin, expmax, N):
         bounds = []
         for i in range(int(expmax - expmin)):
-            new_vals = np.linspace(1 * 10 ** (expmin + i),
-                                   9 * 10 ** (expmin + i), N + 1)[:-1]
+            new_vals = np.linspace(
+                1 * 10 ** (expmin + i), 9 * 10 ** (expmin + i), N + 1
+            )[:-1]
             bounds.extend(new_vals)
         return bounds
 
     def _log_ticks(self, symmetric=False, N=None, *args, **kwargs):
         vmin, vmax = self._calc_vmin_vmax(*args, **kwargs)
-        larger = round_to_05([vmin, vmax], mode='l')
-        smaller = round_to_05([vmin, vmax], mode='s')
+        larger = round_to_05([vmin, vmax], mode="l")
+        smaller = round_to_05([vmin, vmax], mode="s")
         vmin, vmax = min([larger[0], smaller[0]]), max([larger[1], smaller[1]])
 
         if symmetric and np.sign(vmin) == np.sign(vmax):
             if vmin < 0:  # make vmax positive
                 vmax = -vmax
             else:  # make vmin negative
                 vmin = -vmin
@@ -622,22 +651,22 @@
             dexp = int(expmax - expmin)
             expmax0 = np.inf
         else:  # vmin < 0, vmax > 0
             arr = self._collect_array()
             less0 = arr < 0
             greater0 = arr > 0
             if not less0.size:
-                vmin0 = round_to_05(arr[arr > 0].min(), mode='s')
+                vmin0 = round_to_05(arr[arr > 0].min(), mode="s")
                 vmax0 = -vmin0
             elif not greater0.size:
-                vmax0 = round_to_05(arr[arr < 0].max(), mode='l')
+                vmax0 = round_to_05(arr[arr < 0].max(), mode="l")
                 vmin0 = -vmax0
             else:
-                vmin0 = round_to_05(arr[arr > 0].min(), mode='s')
-                vmax0 = round_to_05(arr[arr < 0].max(), mode='l')
+                vmin0 = round_to_05(arr[arr > 0].min(), mode="s")
+                vmax0 = round_to_05(arr[arr < 0].max(), mode="l")
                 if symmetric:
                     vmin0 = min(-vmax0, vmin0)
                     vmax0 = -vmin0
 
             expmin, expmax0 = np.floor(np.log10(np.abs([vmax0, vmin])))
             expmin0, expmax = np.floor(np.log10(np.abs([vmin0, vmax])))
 
@@ -652,32 +681,42 @@
             return np.linspace(vmin, vmax, N, endpoint=True)
         else:
             if N is None:
                 # we go close to 11 bounds in total
                 N = int(max(np.floor((11 if not symmetric else 12) / dexp), 1))
             if not crossing0:
                 bounds = self._log_bounds(expmin, expmax, N)
-                bounds += [1*10**expmax]
+                bounds += [1 * 10**expmax]
                 if signs[0] == -1 and signs[1] == -1:
                     bounds = -np.array(bounds)
             else:
                 bounds_neg = -np.array(self._log_bounds(expmin, expmax0, N))
                 bounds_pos = self._log_bounds(expmin0, expmax, N)
                 bounds = np.unique(
-                    np.r_[bounds_neg, bounds_pos,
-                          -1 * 10 ** expmin, -1 * 10 ** expmax0,
-                          1 * 10 ** expmin0, 1 * 10 ** expmax])
+                    np.r_[
+                        bounds_neg,
+                        bounds_pos,
+                        -1 * 10**expmin,
+                        -1 * 10**expmax0,
+                        1 * 10**expmin0,
+                        1 * 10**expmax,
+                    ]
+                )
                 bounds = bounds[(bounds <= vmax0) | (bounds >= vmin0)]
 
             return np.unique(bounds)
 
     def _roundedsym_ticks(self, N=None, *args, **kwargs):
         N = N or 10
-        vmax = max(map(abs, self._round_min_max(
-            *self._calc_vmin_vmax(*args, **kwargs))))
+        vmax = max(
+            map(
+                abs,
+                self._round_min_max(*self._calc_vmin_vmax(*args, **kwargs)),
+            )
+        )
         vmin = -vmax
         return np.linspace(vmin, vmax, N, endpoint=True)
 
     def _data_minmax_ticks(self, N=None, *args, **kwargs):
         N = N or 11
         vmin, vmax = self._calc_vmin_vmax(*args, **kwargs)
         return np.linspace(vmin, vmax, N, endpoint=True)
@@ -687,41 +726,41 @@
         vmax = max(map(abs, self._calc_vmin_vmax(*args, **kwargs)))
         vmin = -vmax
         return np.linspace(vmin, vmax, N, endpoint=True)
 
     def __init__(self, *args, **kwargs):
         super(DataTicksCalculator, self).__init__(*args, **kwargs)
         self.calc_funcs = {
-            'data': self._data_ticks,
-            'mid': self._mid_data_ticks,
-            'rounded': self._rounded_ticks,
-            'roundedsym': self._roundedsym_ticks,
-            'minmax': self._data_minmax_ticks,
-            'sym': self._data_symminmax_ticks,
-            'log': partial(self._log_ticks, False),
-            'symlog': partial(self._log_ticks, True),
-            }
+            "data": self._data_ticks,
+            "mid": self._mid_data_ticks,
+            "rounded": self._rounded_ticks,
+            "roundedsym": self._roundedsym_ticks,
+            "minmax": self._data_minmax_ticks,
+            "sym": self._data_symminmax_ticks,
+            "log": partial(self._log_ticks, False),
+            "symlog": partial(self._log_ticks, True),
+        }
 
 
-@docstrings.get_sections(base='TicksBase')
+@docstrings.get_sections(base="TicksBase")
 class TicksBase(TicksManagerBase, DataTicksCalculator):
     """
     Abstract base class for calculating ticks
 
     Possible types
     --------------
     None
         use the default ticks
     int
         for an integer *i*, only every *i-th* tick of the default ticks are
         used"""
 
-    dependencies = ['transpose', 'plot']
+    dependencies = ["transpose", "plot"]
 
-    group = 'ticks'
+    group = "ticks"
 
     @abstractproperty
     def axis(self):
         pass
 
     def __init__(self, *args, **kwargs):
         super(TicksBase, self).__init__(*args, **kwargs)
@@ -737,24 +776,25 @@
             self.set_locator(self.default_locators[which])
         elif isinstance(value, int):
             return self._reduce_ticks(value)
         elif len(value) and isinstance(value[0], six.string_types):
             return self.set_ticks(self.calc_funcs[value[0]](*value[1:]))
         elif isinstance(value, tuple):
             steps = 11 if len(value) == 2 else value[3]
-            self.set_ticks(np.linspace(value[0], value[1], steps,
-                                       endpoint=True))
+            self.set_ticks(
+                np.linspace(value[0], value[1], steps, endpoint=True)
+            )
         else:
             self.set_ticks(value)
 
     def set_ticks(self, value):
-        self.axis.set_ticks(value, minor=self.which == 'minor')
+        self.axis.set_ticks(value, minor=self.which == "minor")
 
     def get_locator(self):
-        return getattr(self.axis, 'get_%s_locator' % self.which)()
+        return getattr(self.axis, "get_%s_locator" % self.which)()
 
     def set_locator(self, locator):
         """Sets the locator corresponding of the axis
 
         Parameters
         ----------
         locator: matplotlib.ticker.Locator
@@ -767,25 +807,25 @@
     def set_default_locators(self, which=None):
         """Sets the default locator that is used for updating to None or int
 
         Parameters
         ----------
         which: {None, 'minor', 'major'}
             Specify which locator shall be set"""
-        if which is None or which == 'minor':
-            self.default_locators['minor'] = self.axis.get_minor_locator()
-        if which is None or which == 'major':
-            self.default_locators['major'] = self.axis.get_major_locator()
+        if which is None or which == "minor":
+            self.default_locators["minor"] = self.axis.get_minor_locator()
+        if which is None or which == "major":
+            self.default_locators["major"] = self.axis.get_major_locator()
 
     def _reduce_ticks(self, i):
         loc = self.default_locators[self.which]
         self.set_locator(FixedLocator(loc()[::i]))
 
 
-@docstrings.get_sections(base='DtTicksBase')
+@docstrings.get_sections(base="DtTicksBase")
 class DtTicksBase(TicksBase, TicksManager):
     """
     Abstract base class for x- and y-tick formatoptions
 
     Possible types
     --------------
     %(TicksManager.possible_types)s
@@ -808,70 +848,85 @@
         can be an integer i determining that every i-th data point shall be
         used (by default, it is set to 1). For rounded, roundedsym, minmax and
         sym, the second value determines the total number of ticks (defaults to
         11)."""
 
     def __init__(self, *args, **kwargs):
         super(DtTicksBase, self).__init__(*args, **kwargs)
-        self.calc_funcs.update({
-            'hour': self._frequent_ticks('H'),
-            'day': self._frequent_ticks('D'),
-            'week': self._frequent_ticks(offsets.Week()),
-            'month': self._mid_dt_ticks('M'),
-            'monthend': self._frequent_ticks(
-                offsets.MonthEnd(), onset=offsets.MonthBegin()),
-            'monthbegin': self._frequent_ticks(
-                offsets.MonthBegin(), onset=offsets.MonthBegin(),
-                offset=offsets.MonthBegin()),
-            'year': self._mid_dt_ticks(offsets.YearBegin()),
-            'yearend': self._frequent_ticks(
-                offsets.YearEnd(), onset=offsets.YearBegin()),
-            'yearbegin': self._frequent_ticks(
-                offsets.YearBegin(), onset=offsets.YearBegin(),
-                offset=offsets.YearBegin())})
+        self.calc_funcs.update(
+            {
+                "hour": self._frequent_ticks("H"),
+                "day": self._frequent_ticks("D"),
+                "week": self._frequent_ticks(offsets.Week()),
+                "month": self._mid_dt_ticks("M"),
+                "monthend": self._frequent_ticks(
+                    offsets.MonthEnd(), onset=offsets.MonthBegin()
+                ),
+                "monthbegin": self._frequent_ticks(
+                    offsets.MonthBegin(),
+                    onset=offsets.MonthBegin(),
+                    offset=offsets.MonthBegin(),
+                ),
+                "year": self._mid_dt_ticks(offsets.YearBegin()),
+                "yearend": self._frequent_ticks(
+                    offsets.YearEnd(), onset=offsets.YearBegin()
+                ),
+                "yearbegin": self._frequent_ticks(
+                    offsets.YearBegin(),
+                    onset=offsets.YearBegin(),
+                    offset=offsets.YearBegin(),
+                ),
+            }
+        )
 
     def update(self, value):
-        value = value or {'minor': None, 'major': None}
+        value = value or {"minor": None, "major": None}
         super(DtTicksBase, self).update(value)
 
     @property
     def dtdata(self):
         """The np.unique :attr:`data` as datetime objects"""
         data = self.data
         # do nothing if the data is a pandas.Index without time informations
         # or not a pandas.Index
-        if not getattr(data, 'is_all_dates', None):
-            warn("[%s] - Could not convert time informations for %s ticks "
-                 "with object %r." % (self.logger.name, self.key, type(data)))
+        if not isinstance(data, DatetimeIndex):
+            warn(
+                "[%s] - Could not convert time informations for %s ticks "
+                "with object %r." % (self.logger.name, self.key, type(data))
+            )
             return None
         else:
             return data
 
     def _frequent_ticks(self, freq, onset=None, offset=None):
         def func(N=None, *args, **kwargs):
             step = N or 1
             data = self.dtdata
             if data is None:
                 return
             mindata = data.min() if onset is None else data.min() - onset
             maxdata = data.max() if offset is None else data.max() + offset
-            return date_range(
-                mindata, maxdata, freq=freq)[::step].to_pydatetime()
+            return date_range(mindata, maxdata, freq=freq)[
+                ::step
+            ].to_pydatetime()
+
         return func
 
     def _mid_dt_ticks(self, freq):
         def func(N=None, *args, **kwargs):
             step = N or 1
             data = self.dtdata
             if data is None:
                 return
             data = date_range(
-                data.min(), data.max(), freq=freq).to_pydatetime()
-            data[:-1] += (data[1:] - data[:-1])/2
+                data.min(), data.max(), freq=freq
+            ).to_pydatetime()
+            data[:-1] += (data[1:] - data[:-1]) / 2
             return data[:-1:step]
+
         return func
 
 
 class XTicks(DtTicksBase):
     """
     Modify the x-axis ticks
 
@@ -892,33 +947,35 @@
 
     Plot ticks every year and minor ticks every month::
 
         >>> plotter.update(xticks={'major': 'year', 'minor': 'month'})
 
     See Also
     --------
-    xticklabels, ticksize, tickweight, xtickprops, yticks"""
+    xticklabels, ticksize, tickweight, xtickprops, yticks
+    """
 
-    children = TicksBase.children + ['yticks']
+    children = TicksBase.children + ["yticks"]
 
-    dependencies = DtTicksBase.dependencies + ['plot']
+    dependencies = DtTicksBase.dependencies + ["plot"]
 
-    name = 'Location of the x-Axis ticks'
+    name = "Location of the x-Axis ticks"
 
     @property
     def axis(self):
         return self.ax.xaxis
 
     @property
     def data(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
-        data = getattr(self.plot, 'plotted_data', super(XTicks, self).data)
+
+        data = getattr(self.plot, "plotted_data", super(XTicks, self).data)
         if not len(data):
             data = super(XTicks, self).data
         if isinstance(data, InteractiveList):
             df = InteractiveList(map(select_array, data)).to_dataframe()
         else:
             df = data.to_series()
         if self.transpose.value:
@@ -927,15 +984,15 @@
             if isinstance(df.index, MultiIndex) and len(df.index.names) == 1:
                 return df.index.get_level_values(0)
             else:
                 return df.index
 
     def initialize_plot(self, *args, **kwargs):
         super(XTicks, self).initialize_plot(*args, **kwargs)
-        self.transpose.swap_funcs['ticks'] = self._swap_ticks
+        self.transpose.swap_funcs["ticks"] = self._swap_ticks
 
     def _swap_ticks(self):
         xticks = self
         yticks = self.yticks
         old_xlocators = xticks.default_locators
         xticks.default_locators = yticks.default_locators
         yticks.default_locators = old_xlocators
@@ -954,29 +1011,30 @@
     %(DtTicksBase.possible_types)s
 
     See Also
     --------
     yticklabels, ticksize, tickweight, ytickprops
     xticks: for possible examples"""
 
-    dependencies = DtTicksBase.dependencies + ['plot']
+    dependencies = DtTicksBase.dependencies + ["plot"]
 
-    name = 'Location of the y-Axis ticks'
+    name = "Location of the y-Axis ticks"
 
     @property
     def axis(self):
         return self.ax.yaxis
 
     @property
     def data(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
-        data = getattr(self.plot, 'plotted_data', super(XTicks, self).data)
+
+        data = getattr(self.plot, "plotted_data", super(XTicks, self).data)
         if not len(data):
             data = super(XTicks, self).data
         if isinstance(data, InteractiveList):
             df = InteractiveList(map(select_array, data)).to_dataframe()
         else:
             df = data.to_series()
         if self.transpose.value:
@@ -984,30 +1042,30 @@
                 return df.index.get_level_values(0)
             else:
                 return df.index
         else:
             return df
 
 
-@docstrings.get_sections(base='TickLabelsBase')
+@docstrings.get_sections(base="TickLabelsBase")
 class TickLabelsBase(TicksManagerBase):
     """
     Abstract base class for ticklabels
 
     Possible types
     --------------
     str
         A formatstring like ``'%%Y'`` for plotting the year (in the case that
         time is shown on the axis) or '%%i' for integers
     array
         An array of strings to use for the ticklabels"""
 
-    dependencies = ['transpose']
+    dependencies = ["transpose"]
 
-    group = 'ticks'
+    group = "ticks"
 
     @abstractproperty
     def axis(self):
         """The axis on the axes to modify the ticks of"""
         pass
 
     def __init__(self, *args, **kwargs):
@@ -1016,26 +1074,28 @@
 
     def initialize_plot(self, value):
         self.set_default_formatters()
         self.update(value)
 
     def update_axis(self, value):
         if value is None:
-            self.set_formatter(self.default_formatters['major'])
+            self.set_formatter(self.default_formatters["major"])
         elif isinstance(value, six.string_types):
             self.set_stringformatter(value)
         else:
-            ticks = self.axis.get_ticklocs(minor=self.which == 'minor')
+            ticks = self.axis.get_ticklocs(minor=self.which == "minor")
             if len(ticks) != len(value):
-                warn("[%s] - Length of ticks (%i) and ticklabels (%i)"
-                     "do not match!" % (self.key, len(ticks), len(value)))
+                warn(
+                    "[%s] - Length of ticks (%i) and ticklabels (%i)"
+                    "do not match!" % (self.key, len(ticks), len(value))
+                )
             self.set_ticklabels(value)
 
     def set_stringformatter(self, s):
-        default_formatter = self.default_formatters['major']
+        default_formatter = self.default_formatters["major"]
         if isinstance(default_formatter, AutoDateFormatter):
             self.set_formatter(DateFormatter(s))
         else:
             self.set_formatter(FormatStrFormatter(s))
 
     def set_ticklabels(self, labels):
         """Sets the given tick labels"""
@@ -1049,39 +1109,40 @@
     @abstractmethod
     def set_default_formatters(self):
         """Sets the default formatters that is used for updating to None"""
         pass
 
 
 class TickLabels(TickLabelsBase, TicksManager):
-
     def update(self, value):
-        if (getattr(self, self.key.replace('label', '')).value.get(
-                 'minor') is not None and
-                'minor' not in self.value):
-            items = chain(six.iteritems(value), [('minor', None)])
+        if (
+            getattr(self, self.key.replace("label", "")).value.get("minor")
+            is not None
+            and "minor" not in self.value
+        ):
+            items = chain(six.iteritems(value), [("minor", None)])
         else:
             items = six.iteritems(value)
         super(TickLabels, self).update(dict(items))
 
     def set_default_formatters(self, which=None):
         """Sets the default formatters that is used for updating to None
 
         Parameters
         ----------
         which: {None, 'minor', 'major'}
             Specify which locator shall be set"""
-        if which is None or which == 'minor':
-            self.default_formatters['minor'] = self.axis.get_minor_formatter()
-        if which is None or which == 'major':
-            self.default_formatters['major'] = self.axis.get_major_formatter()
+        if which is None or which == "minor":
+            self.default_formatters["minor"] = self.axis.get_minor_formatter()
+        if which is None or which == "major":
+            self.default_formatters["major"] = self.axis.get_major_formatter()
 
     def set_formatter(self, formatter, which=None):
         which = which or self.which
-        getattr(self.axis, 'set_%s_formatter' % which)(formatter)
+        getattr(self.axis, "set_%s_formatter" % which)(formatter)
 
 
 class XTickLabels(TickLabels):
     """
     Modify the x-axis ticklabels
 
     Possible types
@@ -1089,25 +1150,25 @@
     %(TicksManager.possible_types)s
     %(TickLabelsBase.possible_types)s
 
     See Also
     --------
     xticks, ticksize, tickweight, xtickprops, yticklabels"""
 
-    dependencies = TickLabelsBase.dependencies + ['xticks', 'yticklabels']
+    dependencies = TickLabelsBase.dependencies + ["xticks", "yticklabels"]
 
-    name = 'x-xxis Ticklabels'
+    name = "x-xxis Ticklabels"
 
     @property
     def axis(self):
         return self.ax.xaxis
 
     def initialize_plot(self, *args, **kwargs):
         super(XTickLabels, self).initialize_plot(*args, **kwargs)
-        self.transpose.swap_funcs['ticklabels'] = self._swap_ticklabels
+        self.transpose.swap_funcs["ticklabels"] = self._swap_ticklabels
 
     def _swap_ticklabels(self):
         xticklabels = self
         yticklabels = self.yticklabels
         old_xformatters = xticklabels.default_formatters
         xticklabels.default_formatters = yticklabels.default_formatters
         yticklabels.default_formatters = old_xformatters
@@ -1126,143 +1187,157 @@
     %(TicksManager.possible_types)s
     %(TickLabelsBase.possible_types)s
 
     See Also
     --------
     yticks, ticksize, tickweight, ytickprops, xticklabels"""
 
-    dependencies = TickLabelsBase.dependencies + ['yticks']
+    dependencies = TickLabelsBase.dependencies + ["yticks"]
 
-    name = 'y-xxis ticklabels'
+    name = "y-xxis ticklabels"
 
     @property
     def axis(self):
         return self.ax.yaxis
 
 
 class BarXTicks(XTicks):
-
     __doc__ = XTicks.__doc__
 
-    connections = XTicks.connections + ['xlim']
+    connections = XTicks.connections + ["xlim"]
 
-    dependencies = XTicks.dependencies + ['categorical']
+    dependencies = XTicks.dependencies + ["categorical"]
 
     def update(self, value):
         import matplotlib.ticker as mtick
+
         if self.categorical.is_categorical and not self.transpose.value:
-            self.default_locators['major'] = mtick.FixedLocator(
-                np.unique(self.array))
-            self.default_locators['minor'] = mtick.NullLocator()
+            self.default_locators["major"] = mtick.FixedLocator(
+                np.unique(self.array)
+            )
+            self.default_locators["minor"] = mtick.NullLocator()
         else:
             self.default_locators = self._orig_default_locators.copy()
         return super(BarXTicks, self).update(value)
 
     def set_default_locators(self):
         super(BarXTicks, self).set_default_locators()
         self._orig_default_locators = self.default_locators.copy()
 
     @property
     def array(self):
-        if self.transpose.value and 'stacked' in slist(self.plot.value):
+        if self.transpose.value and "stacked" in slist(self.plot.value):
             df = self.data.to_dataframe()
             return np.concatenate(
-                [[min([0, df.values.min()])], df.sum(axis=1).values])
+                [[min([0, df.values.min()])], df.sum(axis=1).values]
+            )
         elif self.transpose.value:
             return np.concatenate(
-                [self.plot.get_xys(arr)[1] for arr in self.plot.iter_data])
+                [self.plot.get_xys(arr)[1] for arr in self.plot.iter_data]
+            )
         else:
             return np.concatenate(
-                [self.plot.get_xys(arr)[0] for arr in self.plot.iter_data])
+                [self.plot.get_xys(arr)[0] for arr in self.plot.iter_data]
+            )
 
 
 class BarYTicks(YTicks):
-
     __doc__ = YTicks.__doc__
 
-    connections = YTicks.connections + ['ylim']
+    connections = YTicks.connections + ["ylim"]
 
-    dependencies = YTicks.dependencies + ['categorical']
+    dependencies = YTicks.dependencies + ["categorical"]
 
     def update(self, value):
         import matplotlib.ticker as mtick
+
         if self.categorical.is_categorical and self.transpose.value:
-            self.default_locators['major'] = mtick.FixedLocator(
-                np.unique(self.array))
-            self.default_locators['minor'] = mtick.NullLocator()
+            self.default_locators["major"] = mtick.FixedLocator(
+                np.unique(self.array)
+            )
+            self.default_locators["minor"] = mtick.NullLocator()
         else:
             self.default_locators = self._orig_default_locators.copy()
         return super(BarYTicks, self).update(value)
 
     def set_default_locators(self):
         super(BarYTicks, self).set_default_locators()
         self._orig_default_locators = self.default_locators.copy()
 
     @property
     def array(self):
-        if not self.transpose.value and 'stacked' in slist(self.plot.value):
+        if not self.transpose.value and "stacked" in slist(self.plot.value):
             df = self.data.to_dataframe()
             return np.concatenate(
-                [[min([0, df.values.min()])], df.sum(axis=1).values])
+                [[min([0, df.values.min()])], df.sum(axis=1).values]
+            )
         elif self.transpose.value:
             return np.concatenate(
-                [self.plot.get_xys(arr)[0] for arr in self.plot.iter_data])
+                [self.plot.get_xys(arr)[0] for arr in self.plot.iter_data]
+            )
         else:
             return np.concatenate(
-                [self.plot.get_xys(arr)[1] for arr in self.plot.iter_data])
+                [self.plot.get_xys(arr)[1] for arr in self.plot.iter_data]
+            )
 
 
 class BarXTickLabels(XTickLabels):
-
     __doc__ = XTickLabels.__doc__
 
-    dependencies = XTickLabels.dependencies + ['plot', 'categorical']
+    dependencies = XTickLabels.dependencies + ["plot", "categorical"]
 
     def set_stringformatter(self, s):
         if not self.transpose.value and self.plot.value is not None:
             index = self.data.to_dataframe().index
-            if index.is_all_dates:
+            if isinstance(index, DatetimeIndex):
                 if self.categorical.is_categorical:
-                    xticks = self.ax.get_xticks(minor=self.which == 'minor')
-                    arr = list(map(lambda t: t.toordinal(),
-                                   to_datetime(index[xticks.astype(int)])))
+                    xticks = self.ax.get_xticks(minor=self.which == "minor")
+                    arr = list(
+                        map(
+                            lambda t: t.toordinal(),
+                            to_datetime(index[xticks.astype(int)]),
+                        )
+                    )
                     self.ax.set_xticklabels(list(map(DateFormatter(s), arr)))
                 else:
                     self.set_formatter(DateFormatter(s))
                 return
         super(BarXTickLabels, self).set_stringformatter(s)
 
 
 class BarYTickLabels(YTickLabels):
-
     __doc__ = YTickLabels.__doc__
 
-    dependencies = YTickLabels.dependencies + ['plot', 'categorical']
+    dependencies = YTickLabels.dependencies + ["plot", "categorical"]
 
     def set_stringformatter(self, s):
         if self.transpose.value and self.plot.value is not None:
             index = self.data.to_dataframe().index
-            if index.is_all_dates:
+            if isinstance(index, DatetimeIndex):
                 if self.categorical.is_categorical:
-                    yticks = self.ax.get_yticks(self.which == 'minor')
-                    arr = list(map(lambda t: t.toordinal(),
-                                   to_datetime(index[yticks.astype(int)])))
+                    yticks = self.ax.get_yticks(self.which == "minor")
+                    arr = list(
+                        map(
+                            lambda t: t.toordinal(),
+                            to_datetime(index[yticks.astype(int)]),
+                        )
+                    )
                     self.ax.set_yticklabels(list(map(DateFormatter(s), arr)))
                 else:
                     self.set_formatter(DateFormatter(s))
                 return
         super(BarYTickLabels, self).set_stringformatter(s)
 
 
 class TicksOptions(TicksManagerBase):
     """Base class for ticklabels options that apply for x- and y-axis"""
 
     def update(self, value):
         for which, val in six.iteritems(value):
-            for axis, axisname in zip([self.ax.xaxis, self.ax.yaxis], 'xy'):
+            for axis, axisname in zip([self.ax.xaxis, self.ax.yaxis], "xy"):
                 self.which = which
                 self.axis = axis
                 self.axisname = axisname
                 self.update_axis(val)
 
 
 class TickSizeBase(TicksOptions):
@@ -1282,17 +1357,17 @@
     %(TicksManager.possible_types)s
     %(fontsizes)s
 
     See Also
     --------
     tickweight, xtickprops, ytickprops"""
 
-    dependencies = TicksOptions.dependencies + ['xtickprops', 'ytickprops']
+    dependencies = TicksOptions.dependencies + ["xtickprops", "ytickprops"]
 
-    name = 'Font size of the ticklabels'
+    name = "Font size of the ticklabels"
 
 
 class TickWeightBase(TicksOptions):
     """Abstract base class for modifying font weight of ticks"""
 
     def update_axis(self, value):
         for t in self.axis.get_ticklabels(which=self.which):
@@ -1308,20 +1383,20 @@
     %(TicksManager.possible_types)s
     %(fontweights)s
 
     See Also
     --------
     ticksize, xtickprops, ytickprops"""
 
-    dependencies = TicksOptions.dependencies + ['xtickprops', 'ytickprops']
+    dependencies = TicksOptions.dependencies + ["xtickprops", "ytickprops"]
 
-    name = 'Font weight of the ticklabels'
+    name = "Font weight of the ticklabels"
 
 
-@docstrings.get_sections(base='TickPropsBase')
+@docstrings.get_sections(base="TickPropsBase")
 class TickPropsBase(TicksManagerBase):
     """
     Abstract base class for tick parameters
 
     Possible types
     --------------
     dict
@@ -1331,21 +1406,22 @@
     @abstractproperty
     def axisname(self):
         """The name of the axis (either 'x' or 'y')"""
         pass
 
     def update_axis(self, value):
         value = value.copy()
-        if float('.'.join(mpl.__version__.split('.')[:2])) >= 1.5:
-            value.pop('visible', None)
+        if float(".".join(mpl.__version__.split(".")[:2])) >= 1.5:
+            value.pop("visible", None)
         self.ax.tick_params(
-            self.axisname, which=self.which, reset=True, **value)
+            self.axisname, which=self.which, reset=True, **value
+        )
 
 
-@docstrings.get_sections(base='XTickProps')
+@docstrings.get_sections(base="XTickProps")
 class XTickProps(TickPropsBase, TicksManager, DictFormatoption):
     """
     Specify the x-axis tick parameters
 
     This formatoption can be used to make a detailed change of the ticks
     parameters on the x-axis.
 
@@ -1354,17 +1430,17 @@
     %(TicksManager.possible_types)s
     %(TickPropsBase.possible_types)s
 
     See Also
     --------
     xticks, yticks, ticksize, tickweight, ytickprops"""
 
-    axisname = 'x'
+    axisname = "x"
 
-    name = 'Font properties of the x-ticklabels'
+    name = "Font properties of the x-ticklabels"
 
     @property
     def axis(self):
         return self.ax.xaxis
 
 
 class YTickProps(XTickProps):
@@ -1378,24 +1454,24 @@
     --------------
     %(XTickProps.possible_types)s
 
     See Also
     --------
     xticks, yticks, ticksize, tickweight, xtickprops"""
 
-    axisname = 'y'
+    axisname = "y"
 
-    name = 'Font properties of the y-ticklabels'
+    name = "Font properties of the y-ticklabels"
 
     @property
     def axis(self):
         return self.ax.xaxis
 
 
-@docstrings.get_sections(base='Xlabel')
+@docstrings.get_sections(base="Xlabel")
 class Xlabel(TextBase, Formatoption):
     """
     Set the x-axis label
 
     Set the label for the x-axis.
     %(replace_note)s
 
@@ -1404,37 +1480,41 @@
     str
         The text for the :func:`~matplotlib.pyplot.xlabel` function.
 
     See Also
     --------
     xlabelsize, xlabelweight, xlabelprops"""
 
-    children = ['transpose', 'ylabel']
+    children = ["transpose", "ylabel"]
 
-    name = 'x-axis label'
+    name = "x-axis label"
 
     @property
     def enhanced_attrs(self):
         arr = self.transpose.get_x(self.data)
-        replot = self.plotter.replot or not hasattr(self, '_enhanced_attrs')
+        replot = self.plotter.replot or not hasattr(self, "_enhanced_attrs")
         attrs = self.get_enhanced_attrs(arr, replot=replot)
         arr_attrs = self.get_enhanced_attrs(self.data, replot=replot)
         for attr, val in arr_attrs.items():
             attrs.setdefault(attr, val)
         self._enhanced_attrs = attrs
         return attrs
 
     def initialize_plot(self, value):
-        self.transpose.swap_funcs['labels'] = self._swap_labels
-        self._texts = [self.ax.set_xlabel(self.replace(
-            value, self.data, self.enhanced_attrs))]
+        self.transpose.swap_funcs["labels"] = self._swap_labels
+        self._texts = [
+            self.ax.set_xlabel(
+                self.replace(value, self.data, self.enhanced_attrs)
+            )
+        ]
 
     def update(self, value):
-        self._texts[0].set_text(self.replace(value, self.data,
-                                             self.enhanced_attrs))
+        self._texts[0].set_text(
+            self.replace(value, self.data, self.enhanced_attrs)
+        )
 
     def _swap_labels(self):
         plotter = self.plotter
         self.transpose._swap_labels()
         old_xlabel = self.value
         with plotter.no_validation:
             plotter[self.key] = self.ylabel.value
@@ -1457,15 +1537,15 @@
     xlabelsize, xlabelweight, xlabelprops"""
 
     #: Xlabel is modified by the pandas plot routine, therefore we update it
     #: after each plot
     update_after_plot = True
 
 
-@docstrings.get_sections(base='Ylabel')
+@docstrings.get_sections(base="Ylabel")
 class Ylabel(TextBase, Formatoption):
     """
     Set the y-axis label
 
     Set the label for the y-axis.
     %(replace_note)s
 
@@ -1474,36 +1554,40 @@
     str
         The text for the :func:`~matplotlib.pyplot.ylabel` function.
 
     See Also
     --------
     ylabelsize, ylabelweight, ylabelprops"""
 
-    children = ['transpose']
+    children = ["transpose"]
 
-    name = 'y-axis label'
+    name = "y-axis label"
 
     @property
     def enhanced_attrs(self):
         arr = self.transpose.get_y(self.data)
-        replot = self.plotter.replot or not hasattr(self, '_enhanced_attrs')
+        replot = self.plotter.replot or not hasattr(self, "_enhanced_attrs")
         attrs = self.get_enhanced_attrs(arr, replot=replot)
         arr_attrs = self.get_enhanced_attrs(self.data, replot=replot)
         for attr, val in arr_attrs.items():
             attrs.setdefault(attr, val)
         self._enhanced_attrs = attrs
         return attrs
 
     def initialize_plot(self, value):
-        self._texts = [self.ax.set_ylabel(self.replace(
-            value, self.data, self.enhanced_attrs))]
+        self._texts = [
+            self.ax.set_ylabel(
+                self.replace(value, self.data, self.enhanced_attrs)
+            )
+        ]
 
     def update(self, value):
-        self._texts[0].set_text(self.replace(
-            value, self.data, self.enhanced_attrs))
+        self._texts[0].set_text(
+            self.replace(value, self.data, self.enhanced_attrs)
+        )
 
 
 class BarYlabel(Ylabel):
     """
     Set the y-axis label
 
     Set the label for the y-axis.
@@ -1518,33 +1602,33 @@
     ylabelsize, ylabelweight, ylabelprops"""
 
     #: Ylabel is modified by the pandas plot routine, therefore we update it
     #: after each plot
     update_after_plot = True
 
 
-@docstrings.get_sections(base='LabelOptions')
+@docstrings.get_sections(base="LabelOptions")
 class LabelOptions(DictFormatoption):
     """
     Base formatoption class for label sizes
 
     Possible types
     --------------
     dict
         A dictionary with the keys ``'x'`` and (or) ``'y'`` to specify
         which ticks are managed. If the given value is not a dictionary with
         those keys, it is used for the x- and y-axis.
         The values in the dictionary can be one types below.
     """
 
-    children = ['xlabel', 'ylabel']
+    children = ["xlabel", "ylabel"]
 
     def update(self, value):
         for axis, val in value.items():
-            self._text = getattr(self, axis + 'label')._texts[0]
+            self._text = getattr(self, axis + "label")._texts[0]
             self.axis_str = axis
             self.update_axis(val)
 
     @abstractmethod
     def update_axis(self, value):
         pass
 
@@ -1558,19 +1642,19 @@
     %(LabelOptions.possible_types)s
     %(fontsizes)s
 
     See Also
     --------
     xlabel, ylabel, labelweight, labelprops"""
 
-    group = 'labels'
+    group = "labels"
 
-    parents = ['labelprops']
+    parents = ["labelprops"]
 
-    name = 'font size of x- and y-axis label'
+    name = "font size of x- and y-axis label"
 
     def update_axis(self, value):
         self._text.set_size(value)
 
 
 class LabelWeight(LabelOptions):
     """
@@ -1581,19 +1665,19 @@
     %(LabelOptions.possible_types)s
     %(fontweights)s
 
     See Also
     --------
     xlabel, ylabel, labelsize, labelprops"""
 
-    group = 'labels'
+    group = "labels"
 
-    parents = ['labelprops']
+    parents = ["labelprops"]
 
-    name = 'font weight of x- and y-axis label'
+    name = "font weight of x- and y-axis label"
 
     def update_axis(self, value):
         self._text.set_weight(value)
 
 
 class LabelProps(LabelOptions):
     """
@@ -1605,26 +1689,26 @@
     dict
         Items may be any valid text property
 
     See Also
     --------
     xlabel, ylabel, labelsize, labelweight"""
 
-    group = 'labels'
+    group = "labels"
 
-    children = ['xlabel', 'ylabel', 'labelsize', 'labelweight']
+    children = ["xlabel", "ylabel", "labelsize", "labelweight"]
 
-    name = 'font properties of x- and y-axis label'
+    name = "font properties of x- and y-axis label"
 
     def update_axis(self, fontprops):
         fontprops = fontprops.copy()
-        if 'size' not in fontprops and 'fontsize' not in fontprops:
-            fontprops['size'] = self.labelsize.value[self.axis_str]
-        if 'weight' not in fontprops and 'fontweight' not in fontprops:
-            fontprops['weight'] = self.labelweight.value[self.axis_str]
+        if "size" not in fontprops and "fontsize" not in fontprops:
+            fontprops["size"] = self.labelsize.value[self.axis_str]
+        if "weight" not in fontprops and "fontweight" not in fontprops:
+            fontprops["weight"] = self.labelweight.value[self.axis_str]
         self._text.update(fontprops)
 
 
 class Transpose(Formatoption):
     """
     Switch x- and y-axes
 
@@ -1633,28 +1717,28 @@
     x-axis. You can set this formatoption to True to change this behaviour
 
     Possible types
     --------------
     bool
         If True, axes are switched"""
 
-    group = 'axes'
+    group = "axes"
 
-    name = 'Switch x- and y-axes'
+    name = "Switch x- and y-axes"
 
     priority = START
 
     def __init__(self, *args, **kwargs):
         super(Transpose, self).__init__(*args, **kwargs)
         self.swap_funcs = {
-            'ticks': self._swap_ticks,
-            'ticklabels': self._swap_ticklabels,
-            'limits': self._swap_limits,
-            'labels': self._swap_labels,
-            }
+            "ticks": self._swap_ticks,
+            "ticklabels": self._swap_ticklabels,
+            "limits": self._swap_limits,
+            "labels": self._swap_labels,
+        }
 
     def initialize_plot(self, value):
         pass
 
     def update(self, value):
         for func in six.itervalues(self.swap_funcs):
             func()
@@ -1690,73 +1774,73 @@
 
     def _swap_labels(self):
         old_xlabel = self.ax.get_xlabel()
         self.ax.set_xlabel(self.ax.get_ylabel())
         self.ax.set_ylabel(old_xlabel)
 
     def get_x(self, arr):
-        if not hasattr(arr, 'ndim'):  # if the data object is an array list
+        if not hasattr(arr, "ndim"):  # if the data object is an array list
             arr = arr[0]
-        if arr.dims[0] == 'variable' and arr.ndim > 1:
-                arr = arr.psy[0]
+        if arr.dims[0] == "variable" and arr.ndim > 1:
+            arr = arr.psy[0]
         is_unstructured = arr.psy.decoder.is_unstructured(arr)
         if not is_unstructured and arr.ndim == 1:
             if self.value:
                 return arr
             else:
                 #: The x-coordinate name of the variable as stored in the
                 #: dataset (might differ from the one in this array because
                 #: this could also be time, z, y, etc.)
-                ds_coord = arr.psy.get_dim('x', True)
+                ds_coord = arr.psy.get_dim("x", True)
                 xname = arr.dims[0]
         else:
             if self.value:
-                ds_coord = arr.psy.get_dim('y', True)
+                ds_coord = arr.psy.get_dim("y", True)
                 xname = arr.dims[-2 if not is_unstructured else -1]
             else:
-                ds_coord = arr.psy.get_dim('x', True)
+                ds_coord = arr.psy.get_dim("x", True)
                 xname = arr.dims[-1]
         if xname == ds_coord:
             if self.value:
-                return arr.psy.get_coord('y', True)
-            return arr.psy.get_coord('x', True)
+                return arr.psy.get_coord("y", True)
+            return arr.psy.get_coord("x", True)
         else:
             return arr.coords[xname]
 
     def get_y(self, arr):
-        if not hasattr(arr, 'ndim'):  # if the data object is an array list
+        if not hasattr(arr, "ndim"):  # if the data object is an array list
             arr = arr[0]
-        elif arr.dims[0] == 'variable' and arr.ndim > 1:
-                arr = arr.psy[0]
+        elif arr.dims[0] == "variable" and arr.ndim > 1:
+            arr = arr.psy[0]
         is_unstructured = arr.psy.decoder.is_unstructured(arr)
         if not is_unstructured and arr.ndim == 1:
             if not self.value:
                 return arr
             else:
                 #: The x-coordinate name of the variable as stored in the
                 #: dataset (might differ from the one in this array because
                 #: this could also be time, z, y, etc.)
-                ds_coord = arr.psy.get_dim('x', True)
+                ds_coord = arr.psy.get_dim("x", True)
                 yname = arr.dims[0]
         else:
             if not self.value:
-                ds_coord = arr.psy.get_dim('y', True)
+                ds_coord = arr.psy.get_dim("y", True)
                 yname = arr.dims[-2 if not is_unstructured else -1]
             else:
-                ds_coord = arr.psy.get_dim('x', True)
+                ds_coord = arr.psy.get_dim("x", True)
                 yname = arr.dims[-1]
         if yname == ds_coord:
             if self.value:
-                return arr.psy.get_coord('x', True)
-            return arr.psy.get_coord('y', True)
+                return arr.psy.get_coord("x", True)
+            return arr.psy.get_coord("y", True)
         else:
             return arr.coords[yname]
 
 
-@docstrings.get_sections(base='LineColors')
+@docstrings.get_sections(base="LineColors")
 class LineColors(Formatoption):
     """
     Set the color coding
 
     This formatoptions sets the color of the lines, bars, etc.
 
     Possible types
@@ -1767,19 +1851,19 @@
         (e.g. list) to specify the colors manually
     str
         %(cmap_note)s
     matplotlib.colors.ColorMap
         to automatically choose the colors according to the number of lines,
         etc. from the given colormap"""
 
-    group = 'colors'
+    group = "colors"
 
     priority = BEFOREPLOTTING
 
-    name = 'Color cycle'
+    name = "Color cycle"
 
     @property
     def value2pickle(self):
         return self.colors
 
     @property
     def value2share(self):
@@ -1797,22 +1881,26 @@
             c = next(self.color_cycle)
             self.colors.append(c)
             yield c
 
     def update(self, value):
         changed = self.plotter.has_changed(self.key)
         if value is None:
-            prop_cycler = mpl.rcParams['axes.prop_cycle']
-            self.color_cycle = cycle((props['color'] for props in prop_cycler))
+            prop_cycler = mpl.rcParams["axes.prop_cycle"]
+            self.color_cycle = cycle((props["color"] for props in prop_cycler))
             prop_cycler._keys  # this should make a copy
         else:
             try:
-                self.color_cycle = cycle(get_cmap(value)(
-                    np.linspace(0., 1., len(list(self.iter_data)),
-                                endpoint=True)))
+                self.color_cycle = cycle(
+                    get_cmap(value)(
+                        np.linspace(
+                            0.0, 1.0, len(list(self.iter_data)), endpoint=True
+                        )
+                    )
+                )
             except (ValueError, TypeError, KeyError):
                 try:
                     # do not use safe_list, because it might be a generator
                     validate_color(value)
                 except (ValueError, TypeError, AttributeError):
                     pass
                 else:
@@ -1835,15 +1923,15 @@
         :mod:`matplotlib.markers`)
     """
 
     priority = BEFOREPLOTTING
 
     def update(self, value):
         if value is None:
-            self.markers = repeat(mpl.rcParams['lines.marker'])
+            self.markers = repeat(mpl.rcParams["lines.marker"])
         else:
             self.markers = cycle(value)
 
 
 class MarkerSize(Formatoption):
     """
     Choose the size of the markers for points
@@ -1852,46 +1940,46 @@
     --------------
     None
         Use the default from matplotlibs rcParams
     float
         The size of the marker
     """
 
-    connections = ['plot']
+    connections = ["plot"]
 
     priority = BEFOREPLOTTING
 
     def update(self, value):
         if value is None:
-            self.plot._kwargs.pop('markersize', None)
+            self.plot._kwargs.pop("markersize", None)
         else:
-            self.plot._kwargs['markersize'] = value
+            self.plot._kwargs["markersize"] = value
 
 
 class LineWidth(Formatoption):
     """
     Choose the width of the lines
 
     Possible types
     --------------
     None
         Use the default from matplotlibs rcParams
     float
         The width of the lines
     """
 
-    connections = ['plot']
+    connections = ["plot"]
 
     priority = BEFOREPLOTTING
 
     def update(self, value):
         if value is None:
-            self.plot._kwargs.pop('linewidth', None)
+            self.plot._kwargs.pop("linewidth", None)
         else:
-            self.plot._kwargs['linewidth'] = value
+            self.plot._kwargs["linewidth"] = value
 
 
 class LinePlot(Formatoption):
     """
     Choose the line style of the plot
 
     Possible types
@@ -1910,80 +1998,96 @@
         The line style string to use (['solid' | 'dashed', 'dashdot', 'dotted'
         | (offset, on-off-dash-seq) | '-' | '--' | '-.' | ':' | 'None' | ' ' |
         '']).
     """
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
     priority = BEFOREPLOTTING + 0.1
 
-    children = ['color', 'transpose', 'marker']
+    children = ["color", "transpose", "marker"]
 
-    name = 'Line plot type'
+    name = "Line plot type"
 
     @property
     def plotted_data(self):
         """The data that is shown to the user"""
         return InteractiveList(
-            [arr for arr, val in zip(self.iter_data,
-                                     cycle(slist(self.value)))
-             if val is not None])
+            [
+                arr
+                for arr, val in zip(self.iter_data, cycle(slist(self.value)))
+                if val is not None
+            ]
+        )
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._kwargs = {}
 
     def update(self, value):
         # the real plot making is done by make_plot
         pass
 
     def make_plot(self):
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             self.remove()
         value = self.value
         if value is not None:
-            if 'stacked' in value:
+            if "stacked" in value:
                 self._stacked_plot()
             else:
                 try:
                     markers = self.marker.markers
                 except AttributeError:
                     markers = repeat(None)
-                self._plot = list(filter(None, chain.from_iterable(starmap(
-                    self.plot_arr, zip(
-                        self.iter_data, self.color.extended_colors,
-                        cycle(slist(self.value)), markers)))))
+                self._plot = list(
+                    filter(
+                        None,
+                        chain.from_iterable(
+                            starmap(
+                                self.plot_arr,
+                                zip(
+                                    self.iter_data,
+                                    self.color.extended_colors,
+                                    cycle(slist(self.value)),
+                                    markers,
+                                ),
+                            )
+                        ),
+                    )
+                )
 
     def _stacked_plot(self):
         transpose = self.transpose.value
         data = self.data
         if isinstance(data, InteractiveList):
-            data = InteractiveList([arr[0] if arr.ndim == 2 else arr
-                                    for arr in data])
+            data = InteractiveList(
+                [arr[0] if arr.ndim == 2 else arr for arr in data]
+            )
             df = data.to_dataframe()
         else:
             df = data.to_series().to_frame()
         index = self._get_index(df)
         if not isinstance(index, DatetimeIndex):
             try:
                 x = np.asarray(index.values).astype(float)
             except ValueError:
                 x = np.arange(index.values.size)
         else:
             x = index.to_pydatetime()
         base = np.zeros_like(df.iloc[:, 0])
         self._plot = []
-        for (col, s), c, val in zip(df.items(), self.color.extended_colors,
-                                    cycle(slist(self.value))):
+        for (col, s), c, val in zip(
+            df.items(), self.color.extended_colors, cycle(slist(self.value))
+        ):
             if val is None:
                 continue
-            pm = self.ax.fill_betweenx if transpose else \
-                self.ax.fill_between
+            pm = self.ax.fill_betweenx if transpose else self.ax.fill_between
             y = np.where(s.isnull(), 0, s.values)
             self._plot.append(pm(x, base, base + y, facecolor=c))
             base += y
 
     def _get_index(self, df):
         if isinstance(df.index, MultiIndex) and len(df.index.names) == 1:
             index = df.index.get_level_values(0)
@@ -2010,26 +2114,26 @@
             except ValueError:
                 x = np.arange(index.values.size)
         else:
             x = index.to_pydatetime()
 
         if self.transpose.value:
             x, y = y, x
-        if ls in ['area', 'areay']:
+        if ls in ["area", "areay"]:
             ymin = np.vstack([y, np.zeros_like(y)]).min(axis=0)
             ymax = np.vstack([y, np.zeros_like(y)]).max(axis=0)
             return [self.ax.fill_between(x, ymin, ymax, color=c)]
-        elif ls == 'areax':
+        elif ls == "areax":
             xmin = np.vstack([x, np.zeros_like(x)]).min(axis=0)
             xmax = np.vstack([x, np.zeros_like(x)]).max(axis=0)
             return [self.ax.fill_betweenx(y, xmin, xmax, color=c)]
         else:
-            return self.ax.plot(x, y,
-                                color=c, linestyle=ls, marker=m,
-                                **self._kwargs)
+            return self.ax.plot(
+                x, y, color=c, linestyle=ls, marker=m, **self._kwargs
+            )
 
     def remove(self):
         for artist in self._plot:
             artist.remove()
         del self._plot
 
 
@@ -2069,49 +2173,54 @@
     See Also
     --------
     erroralpha
     """
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
     priority = BEFOREPLOTTING
 
-    children = ['color', 'transpose', 'plot']
+    children = ["color", "transpose", "plot"]
 
-    name = 'Error plot type'
+    name = "Error plot type"
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._kwargs = {}
 
     def update(self, value):
         pass  # the work is done in make_plot
 
     def make_plot(self):
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             self.remove()
         if self.value is not None:
             self._plot = []
             colors = self.color.extended_colors
             for da, line in zip(self.iter_data, self.plot._plot):
                 if da.ndim == 2 and da.shape[0] > 1:
                     data = da[0].to_series()
                     error = da[1:, :]
                     if error.shape[0] == 1:
                         min_range = data.values - error[0]
                         max_range = data.values + error[0]
                     else:
                         min_range = error[0]
                         max_range = error[1]
-                    if self.value == 'fill':
+                    if self.value == "fill":
                         vals = self._get_x_values(data)
-                        self.plot_fill(vals, min_range, max_range,
-                                       next(colors), zorder=line.zorder)
+                        self.plot_fill(
+                            vals,
+                            min_range,
+                            max_range,
+                            next(colors),
+                            zorder=line.zorder,
+                        )
                 else:
                     next(colors)
 
     def _get_x_values(self, df):
         if isinstance(df.index, MultiIndex) and len(df.index.names) == 1:
             index = df.index.get_level_values(0)
         else:
@@ -2127,17 +2236,22 @@
 
     def plot_fill(self, index, min_range, max_range, c, **kwargs):
         if self.transpose.value:
             plot_method = self.ax.fill_betweenx
         else:
             plot_method = self.ax.fill_between
         self._plot.append(
-            plot_method(index, min_range, max_range, facecolor=c,
-                        **dict(chain(*map(
-                            six.iteritems, [self._kwargs, kwargs])))))
+            plot_method(
+                index,
+                min_range,
+                max_range,
+                facecolor=c,
+                **dict(chain(*map(six.iteritems, [self._kwargs, kwargs]))),
+            )
+        )
 
     def remove(self):
         for artist in self._plot:
             artist.remove()
         del self._plot
 
 
@@ -2155,22 +2269,22 @@
 
     See Also
     --------
     error"""
 
     priority = BEFOREPLOTTING
 
-    name = 'Alpha value of the error range'
+    name = "Alpha value of the error range"
 
-    group = 'colors'
+    group = "colors"
 
-    connections = ['error']
+    connections = ["error"]
 
     def update(self, value):
-        self.error._kwargs['alpha'] = value
+        self.error._kwargs["alpha"] = value
 
 
 class BarWidths(Formatoption):
     """
     Specify the widths of the bars
 
     Possible types
@@ -2185,15 +2299,15 @@
     See Also
     --------
     categorical
     """
 
     priority = BEFOREPLOTTING
 
-    name = 'Width of the bars'
+    name = "Width of the bars"
 
     def update(self, value):
         # Does nothing, the work is done in the :class:`BarPlot` formatoption
         pass
 
 
 class CategoricalBars(Formatoption):
@@ -2211,35 +2325,35 @@
     See Also
     --------
     widths
     """
 
     priority = BEFOREPLOTTING
 
-    name = 'Categorical or non-categorical plotting'
+    name = "Categorical or non-categorical plotting"
 
-    dependencies = ['widths']
+    dependencies = ["widths"]
 
     def update(self, value):
         widths = self.widths.value
-        self.is_categorical = (value is None and widths == 'equal') or value
+        self.is_categorical = (value is None and widths == "equal") or value
 
 
 class BarAlpha(Formatoption):
     """
     Specify the transparency (alpha)
 
     Possible types
     --------------
     float
         A value between 0 (opaque) and 1 invisible"""
 
     priority = BEFOREPLOTTING
 
-    name = 'Transparency of the bars'
+    name = "Transparency of the bars"
 
     def update(self, value):
         pass
 
 
 class BarPlot(Formatoption):
     """
@@ -2253,23 +2367,23 @@
         Create a usual bar plot with the bars side-by-side
     'stacked'
         Create stacked plot
     """
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
     priority = BEFOREPLOTTING
 
-    children = ['color', 'transpose', 'alpha']
+    children = ["color", "transpose", "alpha"]
 
-    dependencies = ['widths', 'categorical']
+    dependencies = ["widths", "categorical"]
 
-    name = 'Bar plot type'
+    name = "Bar plot type"
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._kwargs = {}
 
     def update(self, value):
         # the real plot making is done by make_plot
@@ -2280,32 +2394,41 @@
             artist.remove()
         del self._plot
 
     @property
     def plotted_data(self):
         """The data that is shown to the user"""
         return InteractiveList(
-            [arr for arr, val in zip(self.iter_data,
-                                     cycle(slist(self.value)))
-             if val is not None])
+            [
+                arr
+                for arr, val in zip(self.iter_data, cycle(slist(self.value)))
+                if val is not None
+            ]
+        )
 
     def make_plot(self):
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             self.remove()
         if self.value is not None:
             ax = self.ax
             # for a transposed plot, we use the barh plot method of the axes
             pm = ax.barh if self.transpose.value else ax.bar
             alpha = self.alpha.value
-            if 'stacked' not in slist(self.value):
+            if "stacked" not in slist(self.value):
                 self._plot = [
-                    pm(*self.get_xys(arr), facecolor=c, alpha=alpha,
-                       align='edge')
-                    for arr, c in zip(self.iter_data,
-                                      self.color.extended_colors)]
+                    pm(
+                        *self.get_xys(arr),
+                        facecolor=c,
+                        alpha=alpha,
+                        align="edge",
+                    )
+                    for arr, c in zip(
+                        self.iter_data, self.color.extended_colors
+                    )
+                ]
                 if self._set_date:
                     if self.transpose.value:
                         ax.yaxis_date()
                     else:
                         ax.xaxis_date()
             else:  # make a stacked plot
                 if isinstance(self.data, InteractiveList):
@@ -2316,77 +2439,83 @@
                     df.index = df.index.get_level_values(0)
                 except AttributeError:
                     pass
                 x, y, s = self.get_xys(df.iloc[:, 0].to_xarray())
                 self._plot = containers = []
                 base = np.zeros_like(y)
                 for i, (col, c, plot) in enumerate(
-                        zip(df.columns, self.color.extended_colors,
-                            cycle(slist(self.value)))):
+                    zip(
+                        df.columns,
+                        self.color.extended_colors,
+                        cycle(slist(self.value)),
+                    )
+                ):
                     if not plot:
                         continue
                     y = df.iloc[:, i].values
                     y = np.where(np.isnan(y), 0, y)
                     if not i:
                         containers.append(
-                            pm(x, y, s, facecolor=c, alpha=alpha))
+                            pm(x, y, s, facecolor=c, alpha=alpha)
+                        )
                     elif self.transpose.value:
                         containers.append(
-                            pm(x, y, s, facecolor=c, alpha=alpha, left=base))
+                            pm(x, y, s, facecolor=c, alpha=alpha, left=base)
+                        )
                     else:
                         containers.append(
-                            pm(x, y, s, facecolor=c, alpha=alpha, bottom=base))
+                            pm(x, y, s, facecolor=c, alpha=alpha, bottom=base)
+                        )
                     base += y
 
     def get_xys(self, arr):
         width = self.widths.value
         y = arr.values
         self._set_date = False
         if self.categorical.is_categorical:
             x = np.arange(len(y))
-            if width == 'data':
+            if width == "data":
                 self.logger.warn(
-                    "Cannot use 'data'-based bar width for categorical plots!")
+                    "Cannot use 'data'-based bar width for categorical plots!"
+                )
                 width = 0.5
-            elif width == 'equal':
+            elif width == "equal":
                 width = 0.5  # pandas default value
-        elif width == 'data':
+        elif width == "data":
             x = _infer_interval_breaks(arr.coords[arr.dims[0]].values)
-            is_datelike = arr.indexes[arr.dims[0]].is_all_dates
+            is_datelike = isinstance(arr.indexes[arr.dims[0]], DatetimeIndex)
             s = x[1:] - x[:-1]
             if is_datelike:
                 # convert to datetime
                 x = to_datetime(x)
                 # calculate widths in days
-                s = to_timedelta(s).total_seconds() / 86400.
+                s = to_timedelta(s).total_seconds() / 86400.0
                 self._set_date = True
             x = x[:-1]
             width = s
         else:
-            if width == 'equal':
+            if width == "equal":
                 # Use half of the smalles step
                 x = _infer_interval_breaks(arr.coords[arr.dims[0]].values)
                 width = np.abs(np.diff(x)).min() / 2
             x = arr.coords[arr.dims[0]].values
         return x, y, width
 
 
 class ViolinXTicks(XTicks):
-
     __doc__ = XTicks.__doc__
 
     @property
     def array(self):
         if not self.transpose.value:
             return np.array(list(range(len(self.data))))
         return super(ViolinXTicks, self).array
 
 
 class ViolinYTicks(YTicks):
-
     __doc__ = YTicks.__doc__
 
     @property
     def array(self):
         if self.transpose.value:
             return np.array(list(range(len(self.data))))
         return super(ViolinYTicks, self).array
@@ -2397,39 +2526,59 @@
 
     data_dependent = True
 
     def update_axis(self, value):
         if self.transpose.value or value is None:
             return super(ViolinXTickLabels, self).update_axis(value)
         if isinstance(value, six.string_types):
-            self.set_ticklabels([
-                self.replace(value, arr, self.get_enhanced_attrs(
-                    arr, replot=True)) for arr in self.data])
-        else:
-            self.set_ticklabels([
-                self.replace(val, arr, self.get_enhanced_attrs(
-                    arr, replot=True)) for val, arr in zip(value, self.data)])
+            self.set_ticklabels(
+                [
+                    self.replace(
+                        value, arr, self.get_enhanced_attrs(arr, replot=True)
+                    )
+                    for arr in self.data
+                ]
+            )
+        else:
+            self.set_ticklabels(
+                [
+                    self.replace(
+                        val, arr, self.get_enhanced_attrs(arr, replot=True)
+                    )
+                    for val, arr in zip(value, self.data)
+                ]
+            )
 
 
 class ViolinYTickLabels(YTickLabels, TextBase):
     __doc__ = XTickLabels.__doc__
 
     data_dependent = True
 
     def update_axis(self, value):
         if self.transpose.value or value is None:
             return super(ViolinYTickLabels, self).update_axis(value)
         if isinstance(value, six.string_types):
-            self.set_ticklabels([
-                self.replace(value, arr, self.get_enhanced_attrs(
-                    arr, replot=True)) for arr in self.data])
-        else:
-            self.set_ticklabels([
-                self.replace(val, arr, self.get_enhanced_attrs(
-                    arr, replot=True)) for val, arr in zip(value, self.data)])
+            self.set_ticklabels(
+                [
+                    self.replace(
+                        value, arr, self.get_enhanced_attrs(arr, replot=True)
+                    )
+                    for arr in self.data
+                ]
+            )
+        else:
+            self.set_ticklabels(
+                [
+                    self.replace(
+                        val, arr, self.get_enhanced_attrs(arr, replot=True)
+                    )
+                    for val, arr in zip(value, self.data)
+                ]
+            )
 
 
 class ViolinPlot(Formatoption):
     """
     Choose how to make the violin plot
 
     Possible types
@@ -2438,21 +2587,21 @@
         Don't make any plotting
     bool
         If True, visualize the violins
     """
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
     priority = BEFOREPLOTTING
 
-    children = ['color', 'transpose']
+    children = ["color", "transpose"]
 
-    name = 'Violin plot type'
+    name = "Violin plot type"
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._kwargs = {}
 
     def update(self, value):
         # the real plot making is done by make_plot
@@ -2460,35 +2609,43 @@
 
     def remove(self):
         for artist in self._plot:
             artist.remove()
         del self._plot
 
     def make_plot(self):
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             self.remove()
         if self.value:
             from seaborn import violinplot
+
             if isinstance(self.data, InteractiveList):
                 df = self.data.to_dataframe()
             else:
                 df = self.data.to_series().to_frame()
-            old_artists = self.ax.containers[:] + self.ax.lines[:] \
+            old_artists = (
+                self.ax.containers[:]
+                + self.ax.lines[:]
                 + self.ax.collections[:]
+            )
             palette = list(islice(self.color.extended_colors, df.shape[1]))
-            violinplot(data=df, palette=palette, ax=self.ax,
-                       orient='h' if self.transpose.value else 'v',
-                       **self._kwargs)
+            violinplot(
+                data=df,
+                palette=palette,
+                ax=self.ax,
+                orient="h" if self.transpose.value else "v",
+                **self._kwargs,
+            )
             artists = self.ax.containers + self.ax.lines + self.ax.collections
             self._plot = [
-                artist for artist in artists
-                if artist not in old_artists]
+                artist for artist in artists if artist not in old_artists
+            ]
 
 
-@docstrings.get_sections(base='LimitBase')
+@docstrings.get_sections(base="LimitBase")
 @dedent
 class LimitBase(DataTicksCalculator):
     """
     Base class for x- and y-limits
 
     Possible types
     --------------
@@ -2515,19 +2672,19 @@
             Same as minmax but symmetric around zero
     tuple (xmin, xmax)
         `xmin` is the smaller value, `xmax` the larger. Any of those values can
         be None or one of the strings (or lists) above to use the corresponding
         value here
     """
 
-    group = 'axes'
+    group = "axes"
 
-    children = ['transpose']
+    children = ["transpose"]
 
-    connections = ['plot']
+    connections = ["plot"]
 
     @property
     def value2share(self):
         return self.range
 
     @abstractmethod
     def set_limit(self, min_val, max_val):
@@ -2540,27 +2697,29 @@
         max_val: float
             The value for the upper limit"""
         pass
 
     def __init__(self, *args, **kwargs):
         super(LimitBase, self).__init__(*args, **kwargs)
         self._calc_funcs = {
-            'rounded': self._round_min_max,
-            'roundedsym': self._roundedsym_min_max,
-            'minmax': self._min_max,
-            'sym': self._sym_min_max}
+            "rounded": self._round_min_max,
+            "roundedsym": self._roundedsym_min_max,
+            "minmax": self._min_max,
+            "sym": self._sym_min_max,
+        }
 
     def _round_min_max(self, vmin, vmax):
         try:
             exp = np.floor(np.log10(abs(vmax - vmin)))
-            larger = round_to_05([vmin, vmax], exp, mode='l')
-            smaller = round_to_05([vmin, vmax], exp, mode='s')
+            larger = round_to_05([vmin, vmax], exp, mode="l")
+            smaller = round_to_05([vmin, vmax], exp, mode="s")
         except TypeError:
-            self.logger.debug("Failed to calculate rounded limits!",
-                              exc_info=True)
+            self.logger.debug(
+                "Failed to calculate rounded limits!", exc_info=True
+            )
             return vmin, vmax
         return min([larger[0], smaller[0]]), max([larger[1], smaller[1]])
 
     def _min_max(self, vmin, vmax):
         return vmin, vmax
 
     def _roundedsym_min_max(self, vmin, vmax):
@@ -2571,29 +2730,29 @@
         vmax = max(abs(vmin), abs(vmax))
         return -vmax, vmax
 
     def update(self, value):
         value = list(value)
         value_lists = list(map(slist, value))
         kwargs = {}
-        for kw, l in zip(['percmin', 'percmax'], value_lists):
+        for kw, l in zip(["percmin", "percmax"], value_lists):
             if len(l) == 2:
                 kwargs[kw] = l[1]
         vmin, vmax = self._calc_vmin_vmax(**kwargs)
         if vmin == vmax:
             vmax = vmax + 1
             vmin = vmin - 1
         for key, func in self._calc_funcs.items():
             if key in value_lists[0] or key in value_lists[1]:
                 minmax = func(vmin, vmax)
                 for i, val in enumerate(value_lists):
                     if key in val:
                         value[i] = minmax[i]
         self.range = value
-        self.logger.debug('Setting %s with %s', self.key, value)
+        self.logger.debug("Setting %s with %s", self.key, value)
         self.set_limit(*value)
 
 
 class Xlim(LimitBase):
     """
     Set the x-axis limits
 
@@ -2602,58 +2761,62 @@
     %(LimitBase.possible_types)s
 
     See Also
     --------
     ylim
     """
 
-    children = LimitBase.children + ['ylim']
+    children = LimitBase.children + ["ylim"]
 
-    dependencies = ['xticks']
+    dependencies = ["xticks"]
 
-    connections = LimitBase.connections + ['sym_lims']
+    connections = LimitBase.connections + ["sym_lims"]
 
-    axisname = 'x'
+    axisname = "x"
 
-    name = 'x-axis limits'
+    name = "x-axis limits"
 
     @property
     def array(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
-        data = list(getattr(self.plot, 'plotted_data', self.iter_data)) or \
-            self.iter_data
+
+        data = (
+            list(getattr(self.plot, "plotted_data", self.iter_data))
+            or self.iter_data
+        )
         df = InteractiveList(map(select_array, data)).to_dataframe()
-        if (self.transpose.value and 'stacked' in slist(self.plot.value)):
+        if self.transpose.value and "stacked" in slist(self.plot.value):
             summed = df.sum(axis=1).values
             arr = np.concatenate(
-                [[min(summed.min(), 0)], df.sum(axis=1).values])
+                [[min(summed.min(), 0)], df.sum(axis=1).values]
+            )
         elif self.transpose.value:
             arr = df.values[df.notnull().values]
         else:
             arr = _get_index_vals(df.index)
         try:
             arr.astype(float)
-        except (ValueError,  TypeError):
+        except (ValueError, TypeError):
             arr = np.arange(len(arr))
         return arr
 
     def set_limit(self, *args):
         if self.ax.xaxis_inverted():
             args = reversed(args)
         try:
             self.ax.set_xlim(*args)
         except (AttributeError, TypeError):  # np.datetime64
             self.ax.set_xlim(*to_datetime(args))
 
     def initialize_plot(self, value):
         super(Xlim, self).initialize_plot(value)
-        self.transpose.swap_funcs['limits'] = self._swap_limits
+        self.transpose.swap_funcs["limits"] = self._swap_limits
 
     def _swap_limits(self):
         self.transpose._swap_limits()
         old_xlim = self.value
         with self.plotter.no_validation:
             self.plotter[self.key] = self.ylim.value
             self.plotter[self.ylim.key] = old_xlim
@@ -2667,37 +2830,42 @@
     --------------
     %(LimitBase.possible_types)s
 
     See Also
     --------
     xlim
     """
-    children = LimitBase.children + ['xlim']
 
-    dependencies = ['yticks']
+    children = LimitBase.children + ["xlim"]
 
-    connections = LimitBase.connections + ['sym_lims']
+    dependencies = ["yticks"]
 
-    axisname = 'y'
+    connections = LimitBase.connections + ["sym_lims"]
 
-    name = 'y-axis limits'
+    axisname = "y"
+
+    name = "y-axis limits"
 
     @property
     def array(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
-        data = list(getattr(self.plot, 'plotted_data', self.iter_data)) or \
-            self.iter_data
+
+        data = (
+            list(getattr(self.plot, "plotted_data", self.iter_data))
+            or self.iter_data
+        )
         df = InteractiveList(map(select_array, data)).to_dataframe()
-        if (not self.transpose.value and 'stacked' in slist(self.plot.value)):
+        if not self.transpose.value and "stacked" in slist(self.plot.value):
             summed = df.sum(axis=1).values
             arr = np.concatenate(
-                [[min(summed.min(), 0)], df.sum(axis=1).values])
+                [[min(summed.min(), 0)], df.sum(axis=1).values]
+            )
         elif self.transpose.value:
             arr = _get_index_vals(df.index)
         else:
             arr = df.values[df.notnull().values]
         try:
             arr.astype(float)
         except ValueError:
@@ -2726,72 +2894,74 @@
     'max'
         Use the maximum of x- and y-limits
     [str, str]
         A combination, ``None``, ``'min'`` and ``'max'`` specific for minimum
         and maximum limit
     """
 
-    dependencies = ['xlim', 'ylim']
+    dependencies = ["xlim", "ylim"]
 
-    name = 'Symmetric x- and y-axis limits'
+    name = "Symmetric x- and y-axis limits"
 
     def update(self, value):
         if all(v is None for v in value):
             return
         xlim = self.xlim.range[:]
         ylim = self.ylim.range[:]
         for i, v in enumerate(value):
-            if v == 'min':
+            if v == "min":
                 xlim[i] = ylim[i] = min(xlim[i], ylim[i])
-            elif v == 'max':
+            elif v == "max":
                 xlim[i] = ylim[i] = max(xlim[i], ylim[i])
         self.xlim.set_limit(*xlim)
         self.ylim.set_limit(*ylim)
 
 
 class ViolinXlim(Xlim):
     # xlim class for ViolinPlotter
     __doc__ = Xlim.__doc__
 
     @property
     def array(self):
         if not self.transpose.value:
-            return np.array(
-                [-0.5, len(list(self.iter_data)) - 0.5])
+            return np.array([-0.5, len(list(self.iter_data)) - 0.5])
         return super(ViolinXlim, self).array
 
     def _round_min_max(self, *args, **kwargs):
         if not self.transpose.value:
             return self.array
         return super(ViolinXlim, self)._round_min_max(*args, **kwargs)
 
 
 class BarXlim(ViolinXlim):
     # xlim class for bar plotter
     __doc__ = Xlim.__doc__
 
-    dependencies = ViolinXlim.dependencies + ['categorical']
+    dependencies = ViolinXlim.dependencies + ["categorical"]
 
     @property
     def array(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
+
         categorical = self.categorical.is_categorical
-        if self.transpose.value and 'stacked' in slist(self.plot.value):
-            data = list(getattr(self.plot, 'plotted_data',
-                                self.iter_data)) or self.iter_data
+        if self.transpose.value and "stacked" in slist(self.plot.value):
+            data = (
+                list(getattr(self.plot, "plotted_data", self.iter_data))
+                or self.iter_data
+            )
             df = InteractiveList(map(select_array, data)).to_dataframe()
             summed = df.sum(axis=1).values
             return np.concatenate(
-                [[min(summed.min(), 0)], df.sum(axis=1).values])
+                [[min(summed.min(), 0)], df.sum(axis=1).values]
+            )
         elif categorical and not self.transpose.value:
-            return np.array(
-                [-0.5, len(self.data.to_dataframe().index) - 0.5])
+            return np.array([-0.5, len(self.data.to_dataframe().index) - 0.5])
         elif not categorical:
             return _infer_interval_breaks(Xlim.array.fget(self))
         return super(BarXlim, self).array
 
     def _round_min_max(self, *args, **kwargs):
         if not self.categorical.is_categorical:
             return Xlim._round_min_max(self, *args, **kwargs)
@@ -2801,84 +2971,90 @@
 
 class Xlim2D(Xlim):
     __doc__ = Xlim.__doc__
 
     @property
     def array(self):
         xcoord = self.transpose.get_x(self.data)
-        func = 'get_x' if not self.transpose.value else 'get_y'
+        func = "get_x" if not self.transpose.value else "get_y"
         data = next(self.iter_data)
-        if xcoord.name == getattr(self.decoder, func)(data).name:
+        decoder_coord = getattr(self.decoder, func)(data)
+        if decoder_coord is not None and xcoord.name == decoder_coord.name:
             bounds = self.decoder.get_cell_node_coord(
-                data, axis='x', coords=data.coords)
+                data, axis="x", coords=data.coords
+            )
             if bounds is None:
                 bounds = xcoord
             bounds = self.convert_coordinate(bounds, xcoord)
             return bounds.values.ravel()
         return self.decoder.get_plotbounds(xcoord)
 
 
 class Ylim2D(Ylim):
     __doc__ = Ylim.__doc__
 
     @property
     def array(self):
         ycoord = self.transpose.get_y(self.data)
-        func = 'get_x' if self.transpose.value else 'get_y'
+        func = "get_x" if self.transpose.value else "get_y"
         data = next(self.iter_data)
-        if ycoord.name == getattr(self.decoder, func)(data).name:
+        decoder_coord = getattr(self.decoder, func)(data)
+        if decoder_coord is not None and ycoord.name == decoder_coord.name:
             bounds = self.decoder.get_cell_node_coord(
-                data, axis='y', coords=data.coords)
+                data, axis="y", coords=data.coords
+            )
             if bounds is None:
                 bounds = ycoord
             bounds = self.convert_coordinate(bounds, ycoord)
             return bounds.values.ravel()
         return self.decoder.get_plotbounds(self.transpose.get_y(self.data))
 
 
 class ViolinYlim(Ylim):
     # Ylim class for ViolinPlotter
     __doc__ = Ylim.__doc__
 
     @property
     def array(self):
         if self.transpose.value:
-            return np.array(
-                [-0.5, len(list(self.iter_data)) - 0.5])
+            return np.array([-0.5, len(list(self.iter_data)) - 0.5])
         return super(ViolinYlim, self).array
 
     def _round_min_max(self, *args, **kwargs):
         if self.transpose.value:
             return self.array
         return super(ViolinYlim, self)._round_min_max(*args, **kwargs)
 
 
 class BarYlim(ViolinYlim):
     # ylim class for bar plotter
     __doc__ = Ylim.__doc__
 
-    dependencies = ViolinYlim.dependencies + ['categorical']
+    dependencies = ViolinYlim.dependencies + ["categorical"]
 
     @property
     def array(self):
         def select_array(arr):
             if arr.ndim > 1:
                 return arr.psy[0]
             return arr
+
         categorical = self.categorical.is_categorical
-        if not self.transpose.value and 'stacked' in slist(self.plot.value):
-            data = list(getattr(self.plot, 'plotted_data',
-                                self.iter_data)) or self.iter_data
+        if not self.transpose.value and "stacked" in slist(self.plot.value):
+            data = (
+                list(getattr(self.plot, "plotted_data", self.iter_data))
+                or self.iter_data
+            )
             df = InteractiveList(map(select_array, data)).to_dataframe()
             summed = df.sum(axis=1).values
             return np.concatenate(
-                [[min(summed.min(), 0)], df.sum(axis=1).values])
+                [[min(summed.min(), 0)], df.sum(axis=1).values]
+            )
         elif categorical and self.transpose.value:
-            return np.array(
-                [-0.5, len(self.data.to_dataframe().index) - 0.5])
+            return np.array([-0.5, len(self.data.to_dataframe().index) - 0.5])
         elif not categorical and self.transpose.value:
             return _infer_interval_breaks(Ylim.array.fget(self))
         elif not categorical:
             return Ylim.array.fget(self)
         return super(BarYlim, self).array
 
     def _round_min_max(self, *args, **kwargs):
@@ -2897,22 +3073,22 @@
     float
         The rotation angle in degrees
 
     See Also
     --------
     yrotation"""
 
-    group = 'ticks'
+    group = "ticks"
 
-    children = ['yticklabels']
+    children = ["yticklabels"]
 
-    name = 'Rotate x-ticklabels'
+    name = "Rotate x-ticklabels"
 
     def update(self, value):
-        for text in self.ax.get_xticklabels(which='both'):
+        for text in self.ax.get_xticklabels(which="both"):
             text.set_rotation(value)
 
 
 class YRotation(Formatoption):
     """
     Rotate the y-axis ticks
 
@@ -2921,22 +3097,22 @@
     float
         The rotation angle in degrees
 
     See Also
     --------
     xrotation"""
 
-    group = 'ticks'
+    group = "ticks"
 
-    children = ['yticklabels']
+    children = ["yticklabels"]
 
-    name = 'Rotate y-ticklabels'
+    name = "Rotate y-ticklabels"
 
     def update(self, value):
-        for text in self.ax.get_yticklabels(which='both'):
+        for text in self.ax.get_yticklabels(which="both"):
             text.set_rotation(value)
 
 
 class CMap(Formatoption):
     """
     Specify the color map
 
@@ -2950,21 +3126,21 @@
     matplotlib.colors.Colormap
         The colormap instance to use
 
     See Also
     --------
     bounds: specifies the boundaries of the colormap"""
 
-    group = 'colors'
+    group = "colors"
 
     priority = BEFOREPLOTTING
 
-    name = 'Colormap'
+    name = "Colormap"
 
-    connections = ['bounds', 'cbar']  # necessary for get_fmt_widget
+    connections = ["bounds", "cbar"]  # necessary for get_fmt_widget
 
     def get_cmap(self, arr=None, cmap=None, N=None):
         """Get the :class:`matplotlib.colors.Colormap` for plotting
 
         Parameters
         ----------
         arr: np.ndarray
@@ -2996,66 +3172,70 @@
 
     def update(self, value):
         pass  # the colormap is set when plotting
 
     def get_fmt_widget(self, parent, project):
         """Open a :class:`psy_simple.widget.CMapFmtWidget`"""
         from psy_simple.widgets.colors import CMapFmtWidget
+
         return CMapFmtWidget(parent, self, project)
 
 
 class MissColor(Formatoption):
     """
     Set the color for missing values
 
     Possible types
     --------------
     None
         Use the default from the colormap
     string, tuple.
         Defines the color of the grid."""
 
-    group = 'colors'
+    group = "colors"
 
     priority = END
 
-    dependencies = ['plot']
+    dependencies = ["plot"]
 
-    connections = ['transform']
+    connections = ["transform"]
 
-    name = 'Color of missing values'
+    name = "Color of missing values"
 
     update_after_plot = True
 
     def update(self, value):
         if self.plotter.replot:
             self.remove()
         if self.plot.value is None:
             return
-        elif value is not None and self.plot.value == 'contourf':
-            warn('[%s] - The miss_color formatoption is not supported for '
-                 'filled contour plots!' % self.logger.name)
+        elif value is not None and self.plot.value == "contourf":
+            warn(
+                "[%s] - The miss_color formatoption is not supported for "
+                "filled contour plots!" % self.logger.name
+            )
         mappable = self.plot.mappable
         if value is not None:
             mappable.get_cmap().set_bad(value)
         else:
             mappable.get_cmap().set_bad(alpha=0)
         mappable.changed()
 
     def remove(self):
-        if hasattr(self, '_miss_color_plot'):
+        if hasattr(self, "_miss_color_plot"):
             try:
                 self._miss_color_plot.remove()
                 del self._miss_color_plot
             except ValueError:
                 pass
 
 
-@docstrings.get_sections(base='Bounds', sections=['Possible types', 'Examples',
-                                              'See Also'])
+@docstrings.get_sections(
+    base="Bounds", sections=["Possible types", "Examples", "See Also"]
+)
 class Bounds(DataTicksCalculator):
     """
     Specify the boundaries of the colorbar
 
     Possible types
     --------------
     None
@@ -3105,21 +3285,21 @@
           >>> plotter.update(bounds=LogNorm())
 
 
     See Also
     --------
     cmap: Specifies the colormap"""
 
-    group = 'colors'
+    group = "colors"
 
     priority = BEFOREPLOTTING
 
-    name = 'Boundaries of the color map'
+    name = "Boundaries of the color map"
 
-    connections = ['cmap', 'cbar']  # necessary for get_fmt_widget
+    connections = ["cmap", "cbar"]  # necessary for get_fmt_widget
 
     @property
     def value2share(self):
         """The normalization instance"""
         if len(self.bounds) > 1:
             return list(self.bounds)
         return self.norm
@@ -3131,20 +3311,20 @@
         else:
             if isinstance(value[0], six.string_types):
                 value = self.calc_funcs[value[0]](*value[1:])
             if value[0] == value[-1]:
                 # make sure we have a small difference between the values
                 value[-1] += value[-1] * 0.5
             self.bounds = value
-            self.norm = mpl.colors.BoundaryNorm(
-                value, len(value) - 1)
+            self.norm = mpl.colors.BoundaryNorm(value, len(value) - 1)
 
     def get_fmt_widget(self, parent, project):
         """Open a :class:`psy_simple.widget.CMapFmtWidget`"""
         from psy_simple.widgets.colors import BoundsFmtWidget
+
         return BoundsFmtWidget(parent, self, project)
 
 
 def format_coord_func(ax, ref):
     """Create a function that can replace the
     :func:`matplotlib.axes.Axes.format_coord`
 
@@ -3167,15 +3347,16 @@
         fmto = ref()
         if fmto is None:
             return orig_s
         try:
             orig_s += fmto.add2format_coord(x, y)
         except Exception:
             fmto.logger.debug(
-                'Failed to get plot informations for status bar!', exc_info=1)
+                "Failed to get plot informations for status bar!", exc_info=1
+            )
         return orig_s
 
     return func
 
 
 class InterpolateBounds(Formatoption):
     """
@@ -3200,15 +3381,15 @@
 
     priority = BEFOREPLOTTING
 
     def update(self, value):
         pass
 
 
-@docstrings.get_sections(base='Plot2D')
+@docstrings.get_sections(base="Plot2D")
 class Plot2D(Formatoption):
     """
     Choose how to visualize a 2-dimensional scalar data field
 
     Possible types
     --------------
     None
@@ -3227,23 +3408,23 @@
     'contour'
         Same a ``'contourf'``, but does not make a filled contour plot, only
         lines.
     """
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
     priority = BEFOREPLOTTING
 
-    name = '2D plot type'
+    name = "2D plot type"
 
-    children = ['cmap', 'bounds']
+    children = ["cmap", "bounds"]
 
-    dependencies = ['levels', 'interp_bounds']
+    dependencies = ["levels", "interp_bounds"]
 
     @property
     def array(self):
         """The (masked) data array that is plotted"""
         arr = self.data.values
         return np.ma.masked_array(arr, mask=np.isnan(arr))
 
@@ -3286,82 +3467,93 @@
     def format_coord(self):
         """The function that can replace the axes.format_coord method"""
         return format_coord_func(self.ax, weakref.ref(self))
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._plot_funcs = {
-            'mesh': self._pcolormesh,
-            'contourf': self._contourf,
-            'contour': self._contourf,
-            'poly': self._polycolor,
+            "mesh": self._pcolormesh,
+            "contourf": self._contourf,
+            "contour": self._contourf,
+            "poly": self._polycolor,
         }
         self._orig_format_coord = None
         self._kwargs = {}
 
     def update(self, value):
         # the real plot making is done by make_plot
         pass
 
     def make_plot(self):
         # remove the plot if it shall be replotted or any of the dependencies
         # changed
         if self.plotter.replot or any(
-                self.plotter.has_changed(key) for key in chain(
-                    self.connections, self.dependencies, [self.key])):
+            self.plotter.has_changed(key)
+            for key in chain(self.connections, self.dependencies, [self.key])
+        ):
             self.remove()
         if self.value is not None:
-            if self.value == 'tri':
-                warn("The 'tri' value is depreceated and will be removed "
-                     "in the future. Use 'poly' instead!",
-                     DeprecationWarning)
+            if self.value == "tri":
+                warn(
+                    "The 'tri' value is depreceated and will be removed "
+                    "in the future. Use 'poly' instead!",
+                    DeprecationWarning,
+                )
             self._plot_funcs[self.value]()
             if self._orig_format_coord is None:
                 self._orig_format_coord = self.ax.format_coord
                 self.ax.format_coord = self.format_coord
 
     def _pcolormesh(self):
         if self.decoder.is_unstructured(self.raw_data):
             return self._polycolor()
         arr = self.array
         cmap = self.cmap.get_cmap(arr)
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             self._plot.update(dict(cmap=cmap, norm=self.bounds.norm))
             # for cartopy, we have to consider the wrapped collection if the
             # data has to be transformed
             try:
                 coll = self._plot._wrapped_collection_fix
             except AttributeError:
                 pass
             else:
                 coll.update(dict(cmap=cmap, norm=self.bounds.norm))
         else:
             x, y = self._get_xy_pcolormesh()
             self._plot = self.ax.pcolormesh(
-                x, y, arr, norm=self.bounds.norm,
-                cmap=cmap, rasterized=True, **self._kwargs)
+                x,
+                y,
+                arr,
+                norm=self.bounds.norm,
+                cmap=cmap,
+                rasterized=True,
+                **self._kwargs,
+            )
 
     def _get_xy_pcolormesh(self):
         interp_bounds = self.interp_bounds.value
         if interp_bounds is None and not self.decoder.is_circumpolar(
-                self.raw_data):
+            self.raw_data
+        ):
             interp_bounds = True
         if interp_bounds:
             return self.xbounds, self.ybounds
         else:
             return self.xcoord.values, self.ycoord.values
 
     def _contourf(self):
-        if hasattr(self, '_plot') and self.plotter.has_changed(
-                self.levels.key):
+        if hasattr(self, "_plot") and self.plotter.has_changed(
+            self.levels.key
+        ):
             self.remove()
         arr = self.array
         cmap = self.cmap.get_cmap(arr)
-        filled = self.value != 'contour'
-        if hasattr(self, '_plot'):
+        filled = self.value != "contour"
+        if hasattr(self, "_plot"):
             self._plot.set_cmap(cmap)
             self._plot.set_norm(self.bounds.norm)
         else:
             levels = self.levels.norm.boundaries
             xcoord = self.convert_coordinate(self.xcoord)
             ycoord = self.convert_coordinate(self.ycoord)
             if self.decoder.is_unstructured(self.raw_data):
@@ -3371,115 +3563,138 @@
                 y = ycoord.values[mask]
                 arr = arr[mask]
             else:
                 pm = self.ax.contourf if filled else self.ax.contour
                 x = xcoord.values
                 y = ycoord.values
             self._plot = pm(
-                x, y, arr, levels, norm=self.bounds.norm,
-                cmap=cmap, **self._kwargs)
+                x,
+                y,
+                arr,
+                levels,
+                norm=self.bounds.norm,
+                cmap=cmap,
+                **self._kwargs,
+            )
 
     @property
     def cell_nodes_x(self):
         """The unstructured x-boundaries with shape (N, m) where m > 2"""
         decoder = self.decoder
         xcoord = self.xcoord
         data = self.data
         xbounds = decoder.get_cell_node_coord(
-            data, coords=data.coords, axis='x')
+            data, coords=data.coords, axis="x"
+        )
         xbounds = self.convert_coordinate(xbounds, xcoord)
         return xbounds.values
 
     @property
     def cell_nodes_y(self):
         """The unstructured y-boundaries with shape (N, m) where m > 2"""
         decoder = self.decoder
         ycoord = self.ycoord
         data = self.data
         ybounds = decoder.get_cell_node_coord(
-            data, coords=data.coords, axis='y')
+            data, coords=data.coords, axis="y"
+        )
         ybounds = self.convert_coordinate(ybounds, ycoord)
         return ybounds.values
 
     def _polycolor(self):
         from matplotlib.collections import PolyCollection
-        self.logger.debug('Retrieving bounds')
+
+        self.logger.debug("Retrieving bounds")
         xbounds = self.cell_nodes_x
         ybounds = self.cell_nodes_y
-        self.logger.debug('Retrieving data')
+        self.logger.debug("Retrieving data")
         arr = self.array
         cmap = self.cmap.get_cmap(arr)
-        if hasattr(self, '_plot'):
-            self.logger.debug('Updating plot')
+        if hasattr(self, "_plot"):
+            self.logger.debug("Updating plot")
             self._plot.update(dict(cmap=cmap, norm=self.bounds.norm))
         else:
-            self.logger.debug('Making plot with %i cells', arr.size)
+            self.logger.debug("Making plot with %i cells", arr.size)
             if xbounds.ndim > 2:
                 xbounds = xbounds.reshape((-1, xbounds.shape[-1]))
                 ybounds = ybounds.reshape((-1, ybounds.shape[-1]))
             self._plot = PolyCollection(
-                np.dstack([xbounds, ybounds]), array=arr.ravel(),
-                norm=self.bounds.norm, rasterized=True, cmap=cmap,
-                edgecolors='none', antialiaseds=False, **self._kwargs)
-            self.logger.debug('Adding collection to axes')
+                np.dstack([xbounds, ybounds]),
+                array=arr.ravel(),
+                norm=self.bounds.norm,
+                rasterized=True,
+                cmap=cmap,
+                edgecolors="none",
+                antialiaseds=False,
+                **self._kwargs,
+            )
+            self.logger.debug("Adding collection to axes")
             self.ax.add_collection(self._plot, autolim=False)
-        self.logger.debug('Done.')
+        self.logger.debug("Done.")
 
     def remove(self):
-        if hasattr(self, '_plot'):
+        if hasattr(self, "_plot"):
             try:
                 self._plot.remove()
             except AttributeError:  # contour plot
                 for artist in self._plot.collections[:]:
                     try:
                         artist.remove()
                     except ValueError:
                         pass
             del self._plot
 
     def add2format_coord(self, x, y):
         """Additional information for the :meth:`format_coord`"""
         if self.value is None:
-            return ''
+            return ""
         data = self.data
         xcoord = self.xcoord
         ycoord = self.ycoord
         if self.decoder.is_unstructured(self.raw_data):
             x, y, z = self.get_xyz_tri(xcoord, x, ycoord, y, data)
         elif xcoord.ndim == 1:
             x, y, z = self.get_xyz_1d(xcoord, x, ycoord, y, data)
         elif xcoord.ndim == 2:
             x, y, z = self.get_xyz_2d(xcoord, x, ycoord, y, data)
         if z is None:
-            return ''
-        xunit = xcoord.attrs.get('units', '')
+            return ""
+        xunit = xcoord.attrs.get("units", "")
         if xunit:
-            xunit = ' ' + xunit
-        yunit = ycoord.attrs.get('units', '')
+            xunit = " " + xunit
+        yunit = ycoord.attrs.get("units", "")
         if yunit:
-            yunit = ' ' + yunit
-        zunit = data.attrs.get('units', '')
+            yunit = " " + yunit
+        zunit = data.attrs.get("units", "")
         if zunit:
-            zunit = ' ' + zunit
-        return ', data: %s: %.4g%s, %s: %.4g%s, %s: %.4g%s' % (
-            xcoord.name, x, xunit, ycoord.name, y, yunit,
-            data.name, z, zunit)
+            zunit = " " + zunit
+        return ", data: %s: %.4g%s, %s: %.4g%s, %s: %.4g%s" % (
+            xcoord.name,
+            x,
+            xunit,
+            ycoord.name,
+            y,
+            yunit,
+            data.name,
+            z,
+            zunit,
+        )
 
     def get_xyz_tri(self, xcoord, x, ycoord, y, data):
         """Get closest x, y and z for the given `x` and `y` in `data` for
         1d coords"""
         return self.get_xyz_2d(xcoord, x, ycoord, y, data)
 
     def get_xyz_1d(self, xcoord, x, ycoord, y, data):
         """Get closest x, y and z for the given `x` and `y` in `data` for
         1d coords"""
         x_idx = xcoord.indexes[xcoord.name]
         y_idx = ycoord.indexes[ycoord.name]
-        xclose = x_idx.get_loc(x, method='nearest')
-        yclose = y_idx.get_loc(y, method='nearest')
+        xclose = x_idx.get_loc(x, method="nearest")
+        yclose = y_idx.get_loc(y, method="nearest")
         dx_max = np.diff(x_idx.sort_values()).max()
         dy_max = np.diff(y_idx.sort_values()).max()
 
         x_data = xcoord[xclose].values
         y_data = ycoord[yclose].values
         if abs(x_data - x) > dx_max or abs(y_data - y) > dy_max:
             val = None
@@ -3492,19 +3707,19 @@
         2d coords"""
         xy = xcoord.values.ravel() + 1j * ycoord.values.ravel()
         dist = np.abs(xy - (x + 1j * y))
         imin = np.nanargmin(dist)
         xy_min = xy[imin]
 
         xb = self.decoder.get_cell_node_coord(
-            data, {xcoord.name: xcoord, ycoord.name: ycoord},
-            axis='x')
+            data, {xcoord.name: xcoord, ycoord.name: ycoord}, axis="x"
+        )
         yb = self.decoder.get_cell_node_coord(
-            data, {xcoord.name: xcoord, ycoord.name: ycoord},
-            axis='y')
+            data, {xcoord.name: xcoord, ycoord.name: ycoord}, axis="y"
+        )
 
         dx_max = np.diff(xb).max()
         dy_max = np.diff(yb).max()
 
         x_data = xy_min.real
         y_data = xy_min.imag
 
@@ -3512,16 +3727,20 @@
             val = None
         else:
             val = data.values.ravel()[imin]
 
         return x_data, y_data, val
 
 
-docstrings.delete_types('Bounds.possible_types', 'no_norm|None',
-                        'None', 'matplotlib.colors.Normalize')
+docstrings.delete_types(
+    "Bounds.possible_types",
+    "no_norm|None",
+    "None",
+    "matplotlib.colors.Normalize",
+)
 
 
 class ContourLevels(Bounds):
     """
     The levels for the contour plot
 
     This formatoption sets the levels for the filled contour plot and only has
@@ -3531,26 +3750,26 @@
     --------------
     None
         Use the settings from the :attr:`bounds` formatoption and if this
         does not specify boundaries, use 11
     %(Bounds.possible_types.no_norm|None)s
     """
 
-    dependencies = ['cbounds']
+    dependencies = ["cbounds"]
 
     priority = BEFOREPLOTTING
 
-    name = 'Levels for the filled contour plot'
+    name = "Levels for the filled contour plot"
 
     def update(self, value):
         if value is None:
             try:
                 value = self.cbounds.norm.boundaries
             except AttributeError:
-                value = ['rounded', 11]
+                value = ["rounded", 11]
         super(ContourLevels, self).update(value)
 
 
 class MaskDataGrid(Formatoption):
     """Mask the datagrid where the array is NaN
 
     This boolean formatoption enables to mask the grid of the :attr:`datagrid`
@@ -3566,15 +3785,14 @@
     datagrid"""
 
     def update(self, value):
         """dummy, since this fmt is considered in the :class:`DataGrid ` fmt"""
         pass
 
 
-
 class DataGrid(Formatoption):
     """
     Show the grid of the data
 
     This formatoption shows the grid of the data (without labels)
 
     Possible types
@@ -3589,21 +3807,23 @@
         :func:`matplotlib.pyplot.triplot` for unstructured grids and
         :func:`matplotlib.pyplot.hlines` for rectilinear grids)
 
     See Also
     --------
     mask_datagrid: To display cells with NaN"""
 
-    children = ['transform']
+    children = ["transform"]
+
+    dependencies = ["mask_datagrid"]
 
-    dependencies = ['mask_datagrid']
+    connections = ["plot"]
 
-    connections = ['plot']
+    name = "Grid of the data"
 
-    name = 'Grid of the data'
+    data_dependent = True
 
     @property
     def xcoord(self):
         """The x coordinate :class:`xarray.Variable`"""
         return self.decoder.get_x(self.data, coords=self.data.coords)
 
     @property
@@ -3624,28 +3844,34 @@
     @property
     def cell_nodes_x(self):
         """The unstructured x-boundaries with shape (N, m) where m > 2"""
         decoder = self.decoder
         xcoord = self.xcoord
         data = self.data
         xbounds = decoder.get_cell_node_coord(
-            data, coords=data.coords, axis='x',
-            nans='skip' if self.mask_datagrid.value else None)
+            data,
+            coords=data.coords,
+            axis="x",
+            nans="skip" if self.mask_datagrid.value else None,
+        )
         xbounds = self.convert_coordinate(xbounds, xcoord)
         return xbounds.values
 
     @property
     def cell_nodes_y(self):
         """The unstructured y-boundaries with shape (N, m) where m > 2"""
         decoder = self.decoder
         ycoord = self.ycoord
         data = self.data
         ybounds = decoder.get_cell_node_coord(
-            data, coords=data.coords, axis='y',
-            nans='skip' if self.mask_datagrid.value else None)
+            data,
+            coords=data.coords,
+            axis="y",
+            nans="skip" if self.mask_datagrid.value else None,
+        )
         ybounds = self.convert_coordinate(ybounds, ycoord, ybounds)
         return ybounds.values
 
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
@@ -3666,23 +3892,22 @@
             yb = np.c_[yb, yb[:, :1], [[np.nan]] * n].ravel()
             if isinstance(value, dict):
                 self._artists = self.ax.plot(xb, yb, **value)
             else:
                 self._artists = self.ax.plot(xb, yb, value)
 
     def remove(self):
-        if not hasattr(self, '_artists'):
+        if not hasattr(self, "_artists"):
             return
         for artist in self._artists:
             artist.remove()
         del self._artists
 
 
 class VectorDataGrid(DataGrid):
-
     @property
     def data(self):
         return super().data[0]
 
 
 class SimplePlot2D(Plot2D):
     """
@@ -3692,32 +3917,30 @@
     --------------
     None
         Don't make any plotting
     'mesh'
         Use the :func:`matplotlib.pyplot.pcolormesh` function to make the plot
     """
 
-    dependencies = Plot2D.dependencies + ['transpose']
+    dependencies = Plot2D.dependencies + ["transpose"]
 
     @property
     def array(self):
         if self.transpose.value:
             return super(SimplePlot2D, self).array.T
         else:
             return super(SimplePlot2D, self).array
 
     @property
     def xbounds(self):
-        return self.decoder.get_plotbounds(self.transpose.get_x(
-            self.data))
+        return self.decoder.get_plotbounds(self.transpose.get_x(self.data))
 
     @property
     def ybounds(self):
-        return self.decoder.get_plotbounds(self.transpose.get_y(
-            self.data))
+        return self.decoder.get_plotbounds(self.transpose.get_y(self.data))
 
     @property
     def xcoord(self):
         if self.transpose.value:
             return super(SimplePlot2D, self).ycoord
         return super(SimplePlot2D, self).xcoord
 
@@ -3737,15 +3960,14 @@
     def cell_nodes_y(self):
         if self.transpose.value:
             return super(SimplePlot2D, self).cell_nodes_x
         return super(SimplePlot2D, self).cell_nodes_y
 
 
 class XTicks2D(XTicks):
-
     __doc__ = XTicks.__doc__
 
     @property
     def data(self):
         data = []
         plot_data = super(XTicks, self).data
         if not isinstance(plot_data, InteractiveList):
@@ -3754,21 +3976,21 @@
             data.append(self.transpose.get_x(da))
         if len(data) == 1:
             return data[0]
         try:
             return xr.concat(data)
         except Exception:
             self.logger.debug(
-                'Failed to concatenate the data, returning first object!',
-                exc_info=True)
+                "Failed to concatenate the data, returning first object!",
+                exc_info=True,
+            )
             return data[0]
 
 
 class YTicks2D(YTicks):
-
     __doc__ = YTicks.__doc__
 
     @property
     def data(self):
         data = []
         plot_data = super(YTicks, self).data
         if not isinstance(plot_data, InteractiveList):
@@ -3778,40 +4000,43 @@
                 data.append(self.transpose.get_y(da))
         if len(data) == 1:
             return data[0]
         try:
             return xr.concat(data)
         except Exception:
             self.logger.debug(
-                'Failed to concatenate the data, returning first object!',
-                exc_info=True)
+                "Failed to concatenate the data, returning first object!",
+                exc_info=True,
+            )
             return data[0]
 
 
 class Extend(Formatoption):
     """
     Draw arrows at the side of the colorbar
 
     Possible types
     --------------
     str {'neither', 'both', 'min' or 'max'}
         If not 'neither', make pointed end(s) for out-of-range values
     """
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Ends of the colorbar'
+    name = "Ends of the colorbar"
 
-    connections = ['plot']
+    connections = ["plot"]
 
     def update(self, value):
         # nothing to do here because the extend is set by the Cbar formatoption
-        if self.plot.value == 'contourf' and value != 'neither':
-            warn('[%s] - Extend keyword is not implemented for contour '
-                 'plots' % self.logger.name)
+        if self.plot.value == "contourf" and value != "neither":
+            warn(
+                "[%s] - Extend keyword is not implemented for contour "
+                "plots" % self.logger.name
+            )
         else:
             if self.plot.value is not None:
                 self.plot.mappable.norm.extend = value
 
 
 class CbarSpacing(Formatoption):
     """
@@ -3820,25 +4045,25 @@
     Possible types
     --------------
     str {'uniform', 'proportional'}
         if ``'uniform'``, every color has exactly the same width in the
         colorbar, if ``'proportional'``, the size is chosen according to the
         data"""
 
-    group = 'colors'
+    group = "colors"
 
-    connections = ['cbar']
+    connections = ["cbar"]
 
-    name = 'Spacing of the colorbar'
+    name = "Spacing of the colorbar"
 
     def update(self, value):
-        self.cbar._kwargs['spacing'] = value
+        self.cbar._kwargs["spacing"] = value
 
 
-@docstrings.get_sections(base='Cbar')
+@docstrings.get_sections(base="Cbar")
 class Cbar(Formatoption):
     """
     Specify the position of the colorbars
 
     Possible types
     --------------
     bool
@@ -3858,42 +4083,52 @@
 
     Examples
     --------
     Draw a colorbar at the bottom and left of the axes::
 
     >>> plotter.update(cbar='bl')"""
 
-    dependencies = ['plot', 'cmap', 'bounds', 'extend', 'cbarspacing',
-                    'levels']
+    dependencies = [
+        "plot",
+        "cmap",
+        "bounds",
+        "extend",
+        "cbarspacing",
+        "levels",
+    ]
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Position of the colorbar'
+    name = "Position of the colorbar"
 
     priority = END + 0.1
 
-    figure_positions = {'fr', 'fb', 'fl', 'ft', 'b', 'r', 'l', 't'}
+    figure_positions = {"fr", "fb", "fl", "ft", "b", "r", "l", "t"}
 
     original_position = None
 
     @property
     def init_kwargs(self):
-        return dict(chain(six.iteritems(super(Cbar, self).init_kwargs),
-                          [('other_cbars', self.other_cbars)]))
+        return dict(
+            chain(
+                six.iteritems(super(Cbar, self).init_kwargs),
+                [("other_cbars", self.other_cbars)],
+            )
+        )
 
     @docstrings.dedent
     def __init__(self, *args, **kwargs):
         """
         Parameters
         ----------
         %(Formatoption.parameters)s
         other_cbars: list of str
             List of other colorbar formatoption keys (necessary for a
             sufficient resizing of the axes)"""
-        self.other_cbars = kwargs.pop('other_cbars', [])
+        self.other_cbars = kwargs.pop("other_cbars", [])
         super(Cbar, self).__init__(*args, **kwargs)
         self._kwargs = {}
         self._just_drawn = set()
 
     def initialize_plot(self, value):
         self._set_original_position()
         self.cbars = {}
@@ -3905,52 +4140,56 @@
         # although the figure has not been drawn so far
         for key in self.other_cbars:
             fmto = getattr(self.plotter, key, None)
             if fmto is not None and fmto.original_position:
                 self.original_position = fmto.original_position
                 return
         ax = self.ax
-        if ax._adjustable in ['box', 'box-forced']:
+        if ax._adjustable in ["box", "box-forced"]:
             figW, figH = ax.get_figure().get_size_inches()
             fig_aspect = figH / figW
             position = ax.get_position(True)
             pb = position.frozen()
             box_aspect = ax.get_data_ratio()
             pb1 = pb.shrunk_to_aspect(box_aspect, pb, fig_aspect)
             self.original_position = pb1.anchored(ax.get_anchor(), pb)
         else:
             self.original_position = ax.get_position(True)
 
     @property
     def value2share(self):
         """Those colorbar positions that are directly at the axes"""
-        return self.value.intersection(['r', 'b', 'l', 't'])
+        return self.value.intersection(["r", "b", "l", "t"])
 
     def update(self, value):
         """
         Updates the colorbar
 
         Parameters
         ----------
         value
             The value to update (see possible types)
         no_fig_cbars
             Does not update the colorbars that are not in the axes of this
             plot"""
         plotter = self.plotter
         if plotter.replot or any(
-                plotter.has_changed(key, False) for key in self.dependencies
-                if getattr(self, key, None) is not None and key not in [
-                        self._child_mapping['cmap'], self._child_mapping[
-                            'bounds']]):
+            plotter.has_changed(key, False)
+            for key in self.dependencies
+            if getattr(self, key, None) is not None
+            and key
+            not in [self._child_mapping["cmap"], self._child_mapping["bounds"]]
+        ):
             cbars2delete = set(self.cbars)
         else:
             changed_bounds = plotter.has_changed(self.bounds.key)
-            if changed_bounds and (type(changed_bounds[0]) is not
-                                   type(changed_bounds[1])):
+            if changed_bounds and (
+                type(changed_bounds[0])
+                is not type(changed_bounds[1])  # noqa: E721
+            ):
                 cbars2delete = set(self.cbars)
             else:
                 cbars2delete = set(self.cbars).difference(value)
         if cbars2delete:
             # if the colorbars are in the figure of the axes, we have to first
             # remove all the colorbars and then redraw it in order to make
             # sure that the axes gets the right position
@@ -3969,168 +4208,187 @@
                 self.remove(positions=cbars2delete)
         for pos in value.intersection(self.cbars):
             if self.plot.value is not None:
                 self.update_colorbar(pos)
         for pos in sorted(value.difference(self.cbars)):
             if self.plot.value is not None:
                 self.draw_colorbar(pos)
-        plotter._figs2draw.update(map(lambda cbar: cbar.ax.get_figure(),
-                                      six.itervalues(self.cbars)))
+        plotter._figs2draw.update(
+            map(lambda cbar: cbar.ax.get_figure(), six.itervalues(self.cbars))
+        )
 
     def update_colorbar(self, pos):
         cbar = self.cbars[pos]
         mappable = self.plot.mappable
-        if mpl.__version__ < '3.1':
+        if mpl.__version__ < "3.1":
             cbar.set_norm(self.plot.mappable.norm)
             cbar.set_cmap(self.plot.mappable.cmap)
         else:  # change the colorbar and reconnect signals
             old = cbar.mappable
             cbar.update_normal(mappable)
-            if not getattr(mappable, 'colorbar_cid', False):
-                if getattr(old, 'colorbar_cid', False):
+            if not getattr(mappable, "colorbar_cid", False):
+                if getattr(old, "colorbar_cid", False):
                     old.callbacksSM.disconnect(old.colorbar_cid)
                     old.colorbar = None
                     old.colorbar_cid = None
                 if mpl.__version__ < "3.3":
                     cid = mappable.callbacksSM.connect(
-                        'changed', cbar.on_mappable_changed
+                        "changed", cbar.on_mappable_changed
                     )
-                else:
+                elif mpl.__version__ < "3.5":
                     cid = mappable.callbacksSM.connect(
-                        'changed', cbar.update_normal
+                        "changed", cbar.update_normal
+                    )
+                else:
+                    cid = mappable.callbacks.connect(
+                        "changed", cbar.update_normal
                     )
                 mappable.colorbar = cbar
                 mappable.colorbar_cid = cid
             cbar.update_normal(cbar.mappable)
-        cbar.draw_all()
+        if mpl_version <= 3.5:
+            cbar.draw_all()
 
-    def remove(self, positions='all'):
+    def remove(self, positions="all"):
         import matplotlib.pyplot as plt
 
         def try2remove(cbar):
             try:
                 cbar.remove()
             except KeyError:
                 # the colorbar has been removed already from some other
                 # Cbar instance
                 pass
-        if positions == 'all':
+
+        if positions == "all":
             positions = self.cbars.keys()
         positions = set(positions).intersection(self.cbars.keys())
         if not positions:
             return
         adjustment = {}
-        to_adjust = {'fr': 'right', 'fl': 'left', 'ft': 'top', 'fb': 'bottom'}
+        to_adjust = {"fr": "right", "fl": "left", "ft": "top", "fb": "bottom"}
         for pos in positions:
             cbar = self.cbars.pop(pos)
-            if pos in ['sh', 'sv']:
+            if pos in ["sh", "sv"]:
                 plt.close(cbar.ax.get_figure())
             else:
                 # set the axes for the mappable if this has been removed
                 mappable = cbar.mappable
-                delaxes = not hasattr(mappable, 'axes')
-                if getattr(mappable, 'axes', None) is None:
+                delaxes = not hasattr(mappable, "axes")
+                if getattr(mappable, "axes", None) is None:
                     mappable.axes = self.plotter.ax
                     try2remove(cbar)
                     if delaxes:
                         del mappable.axes
                     else:
                         mappable.axes = None
                 else:
                     try2remove(cbar)
                 if pos in to_adjust:
                     adjustment[to_adjust[pos]] = mpl.rcParams[
-                        'figure.subplot.' + to_adjust[pos]]
+                        "figure.subplot." + to_adjust[pos]
+                    ]
         if adjustment:
             self.ax.get_figure().subplots_adjust(**adjustment)
         if self.figure_positions.intersection(positions):
             self.ax.set_position(self.original_position)
         return
 
     def draw_colorbar(self, pos):
         import matplotlib.pyplot as plt
+
         # TODO: Manage to draw colorbars left and top (gridspec does not work)
         orientations = {
             # 'b': 'bottom', 'r': 'right', 'l': 'left', 't': 'top',
-            'b': 'horizontal', 'r': 'vertical',
-            'fr': 'vertical', 'fl': 'vertical', 'sv': 'vertical',
-            'ft': 'horizontal', 'fb': 'horizontal', 'sh': 'horizontal'}
+            "b": "horizontal",
+            "r": "vertical",
+            "fr": "vertical",
+            "fl": "vertical",
+            "sv": "vertical",
+            "ft": "horizontal",
+            "fb": "horizontal",
+            "sh": "horizontal",
+        }
 
         orientation = orientations[pos]
         kwargs = self._kwargs.copy()
-        if pos in ['b', 'r', 'l', 't']:
+        if pos in ["b", "r", "l", "t"]:
             fig = self.ax.get_figure()
             # kwargs = {'ax': self.ax, 'location': orientation}
-            kwargs.update({'ax': self.ax, 'orientation': orientation})
-        elif pos == 'sh':
+            kwargs.update({"ax": self.ax, "orientation": orientation})
+        elif pos == "sh":
             fig = plt.figure(figsize=(8, 1))
-            kwargs.update({'cax': fig.add_axes([0.05, 0.5, 0.9, 0.3])})
+            kwargs.update({"cax": fig.add_axes([0.05, 0.5, 0.9, 0.3])})
             self.plotter._figs2draw.add(fig)  # add figure for drawing
-        elif pos == 'sv':
+        elif pos == "sv":
             fig = plt.figure(figsize=(1, 8))
-            kwargs.update({'cax': fig.add_axes([0.3, 0.05, 0.3, 0.9])})
+            kwargs.update({"cax": fig.add_axes([0.3, 0.05, 0.3, 0.9])})
             self.plotter._figs2draw.add(fig)  # add figure for drawing
         else:
             fig = self.ax.get_figure()
-            if pos == 'fb':
+            if pos == "fb":
                 fig.subplots_adjust(bottom=0.2)
-                kwargs['cax'] = fig.add_axes(
+                kwargs["cax"] = fig.add_axes(
                     [0.125, 0.135, 0.775, 0.05],
-                    label=self.raw_data.psy.arr_name + '_fb')
-            elif pos == 'fr':
+                    label=self.raw_data.psy.arr_name + "_fb",
+                )
+            elif pos == "fr":
                 fig.subplots_adjust(right=0.8)
-                kwargs['cax'] = fig.add_axes(
+                kwargs["cax"] = fig.add_axes(
                     [0.825, 0.25, 0.035, 0.6],
-                    label=self.raw_data.psy.arr_name + '_fr')
-            elif pos == 'fl':
+                    label=self.raw_data.psy.arr_name + "_fr",
+                )
+            elif pos == "fl":
                 fig.subplots_adjust(left=0.225)
-                kwargs['cax'] = fig.add_axes(
+                kwargs["cax"] = fig.add_axes(
                     [0.075, 0.25, 0.035, 0.6],
-                    label=self.raw_data.psy.arr_name + '_fl')
-            elif pos == 'ft':
+                    label=self.raw_data.psy.arr_name + "_fl",
+                )
+            elif pos == "ft":
                 fig.subplots_adjust(top=0.75)
-                kwargs['cax'] = fig.add_axes(
+                kwargs["cax"] = fig.add_axes(
                     [0.125, 0.825, 0.775, 0.05],
-                    label=self.raw_data.psy.arr_name + '_ft')
-        if float('.'.join(mpl.__version__.split('.')[:2])) <= 3.2:
-            kwargs['extend'] = self.extend.value
-        if 'location' not in kwargs:
-            kwargs['orientation'] = orientation
+                    label=self.raw_data.psy.arr_name + "_ft",
+                )
+        if float(".".join(mpl.__version__.split(".")[:2])) <= 3.2:
+            kwargs["extend"] = self.extend.value
+        if "location" not in kwargs:
+            kwargs["orientation"] = orientation
         if mpl.__version__.startswith("3.5.0"):
             from matplotlib.contour import ContourSet
-            if (
-                kwargs.get("orientation") == "horizontal" and
-                isinstance(self.plot.mappable, ContourSet)
+
+            if kwargs.get("orientation") == "horizontal" and isinstance(
+                self.plot.mappable, ContourSet
             ):
                 warn(
                     "Horizontal colorbars are not possible for contour plots "
                     "with matplotlib 3.5.0, see "
                     "https://github.com/matplotlib/matplotlib/issues/21683"
                 )
                 kwargs.pop("orientation")
         self.cbars[pos] = cbar = fig.colorbar(self.plot.mappable, **kwargs)
         self._just_drawn.add(cbar)
         self.set_label_pos(pos)
 
     def set_label_pos(self, pos):
         ax = self.cbars[pos].ax
-        if pos == 'fl':
+        if pos == "fl":
             # draw tick labels left
-            ax.tick_params('y', labelleft=True, labelright=False)
-            ax.yaxis.set_label_position('left')
+            ax.tick_params("y", labelleft=True, labelright=False)
+            ax.yaxis.set_label_position("left")
             ax.yaxis.tick_left()
-        elif pos == 'ft':
+        elif pos == "ft":
             # draw ticklabels at the top
-            ax.tick_params('x', labeltop=True, labelbottom=False)
-            ax.xaxis.set_label_position('top')
+            ax.tick_params("x", labeltop=True, labelbottom=False)
+            ax.xaxis.set_label_position("top")
             ax.xaxis.tick_top()
-        elif pos == 'r':
+        elif pos == "r":
             # draw ticklabels on the right
-            ax.tick_params('y', labelleft=False, labelright=True)
-            ax.yaxis.set_label_position('right')
+            ax.tick_params("y", labelleft=False, labelright=True)
+            ax.yaxis.set_label_position("right")
             ax.yaxis.tick_right()
 
     def finish_update(self):
         # Set the label position again in case this has been changed
         for pos, cbar in self.cbars.items():
             self.set_label_pos(pos)
         self._just_drawn.clear()
@@ -4149,37 +4407,47 @@
         The title for the :meth:`~matplotlib.colorbar.Colorbar.set_label`
         method.
 
     See Also
     --------
     clabelsize, clabelweight, clabelprops"""
 
-    children = ['plot']
+    children = ["plot"]
 
-    dependencies = ['cbar']
+    dependencies = ["cbar"]
 
-    name = 'Colorbar label'
+    name = "Colorbar label"
 
     data_dependent = True
 
-    group = 'labels'
+    group = "labels"
 
     axis_locations = {
-            'b': 'x', 'r': 'y', 'l': 'y', 't': 'x',  # axes locations
-            'fr': 'y', 'fl': 'y', 'sv': 'y',         # vertical figure cbars
-            'ft': 'x', 'fb': 'x', 'sh': 'x'}         # horizontal figure cbars
+        "b": "x",
+        "r": "y",
+        "l": "y",
+        "t": "x",  # axes locations
+        "fr": "y",
+        "fl": "y",
+        "sv": "y",  # vertical figure cbars
+        "ft": "x",
+        "fb": "x",
+        "sh": "x",
+    }  # horizontal figure cbars
 
     def update(self, value):
         arr = self.plot.data
         self.texts = []
         for pos, cbar in six.iteritems(self.cbar.cbars):
-            cbar.set_label(self.replace(
-                    value, arr, attrs=self.get_enhanced_attrs(arr)))
-            self.texts.append(getattr(
-                cbar.ax, self.axis_locations[pos] + 'axis').get_label())
+            cbar.set_label(
+                self.replace(value, arr, attrs=self.get_enhanced_attrs(arr))
+            )
+            self.texts.append(
+                getattr(cbar.ax, self.axis_locations[pos] + "axis").get_label()
+            )
 
 
 class VCLabel(CLabel):
     """
     Show the colorbar label of the vector plot
 
     Set the label of the colorbar.
@@ -4190,25 +4458,26 @@
     str
         The title for the :meth:`~matplotlib.colorbar.Colorbar.set_label`
         method.
 
     See Also
     --------
     vclabelsize, vclabelweight, vclabelprops"""
+
     pass
 
 
 class CbarOptions(Formatoption):
     """Base class for colorbar formatoptions"""
 
-    which = 'major'
+    which = "major"
 
-    children = ['plot']
+    children = ["plot"]
 
-    dependencies = ['cbar']
+    dependencies = ["cbar"]
 
     @property
     def colorbar(self):
         try:
             return self._colorbar
         except AttributeError:
             try:
@@ -4224,15 +4493,16 @@
         self._colorbar = cbar
 
     @property
     def axis(self):
         """axis of the colorbar with the ticks. Will be overwritten during
         update process."""
         return getattr(
-            self.colorbar.ax, self.axis_locations[self.position] + 'axis')
+            self.colorbar.ax, self.axis_locations[self.position] + "axis"
+        )
 
     @property
     def axisname(self):
         return self.axis_locations[self.position]
 
     @property
     def data(self):
@@ -4246,15 +4516,15 @@
     def update(self, value):
         for pos, cbar in six.iteritems(self.cbar.cbars):
             self.colorbar = cbar
             self.position = pos
             self.update_axis(value)
 
 
-@docstrings.get_sections(base='CTicks')
+@docstrings.get_sections(base="CTicks")
 class CTicks(CbarOptions, TicksBase):
     """
     Specify the tick locations of the colorbar
 
     Possible types
     --------------
     None
@@ -4271,19 +4541,19 @@
         integer ``i``, then this is the same as ``['bounds', i]``.
 
     See Also
     --------
     cticklabels
     """
 
-    dependencies = CbarOptions.dependencies + ['bounds']
+    dependencies = CbarOptions.dependencies + ["bounds"]
 
-    connections = CbarOptions.connections + ['cmap']
+    connections = CbarOptions.connections + ["cmap"]
 
-    name = 'Colorbar ticks'
+    name = "Colorbar ticks"
 
     _default_locator = None
 
     @property
     def default_locator(self):
         """Default locator of the axis of the colorbars"""
         if self._default_locator is None:
@@ -4292,16 +4562,16 @@
 
     @default_locator.setter
     def default_locator(self, locator):
         self._default_locator = locator
 
     def __init__(self, *args, **kwargs):
         super(CTicks, self).__init__(*args, **kwargs)
-        self.calc_funcs['bounds'] = self._bounds_ticks
-        self.calc_funcs['midbounds'] = self._mid_bounds_ticks
+        self.calc_funcs["bounds"] = self._bounds_ticks
+        self.calc_funcs["midbounds"] = self._mid_bounds_ticks
 
     def set_ticks(self, value):
         self.ticks = value
         self.colorbar.set_ticks(value)
 
     def _bounds_ticks(self, step=None, *args, **kwargs):
         step = step or 1
@@ -4311,15 +4581,16 @@
         step = step or 1
         ret = 0.5 * (self.bounds.bounds[1:] + self.bounds.bounds[:-1])
         return ret[::step]
 
     def update(self, value):
         # reset the locators if the colorbar has been drawn from scratch
         if self.cbar._just_drawn or (
-                not self.plotter.has_changed(self.key) and self.value is None):
+            not self.plotter.has_changed(self.key) and self.value is None
+        ):
             if self.cbar.cbars:
                 try:
                     del self._colorbar
                 except AttributeError:
                     pass
                 self.set_default_locators()
         super(CTicks, self).update(value)
@@ -4341,14 +4612,15 @@
         else:
             self.default_locator = cbar.locator
             self.default_formatter = cbar.formatter
 
     def get_fmt_widget(self, parent, project):
         """Open a :class:`psy_simple.widget.CMapFmtWidget`"""
         from psy_simple.widgets.colors import CTicksFmtWidget
+
         return CTicksFmtWidget(parent, self, project)
 
 
 class VectorCTicks(CTicks):
     """
     Specify the tick locations of the vector colorbar
 
@@ -4357,15 +4629,15 @@
     %(CTicks.possible_types)s
 
     See Also
     --------
     cticklabels, vcticklabels
     """
 
-    dependencies = CTicks.dependencies + ['color']
+    dependencies = CTicks.dependencies + ["color"]
 
     @property
     def array(self):
         arr = self.color._color_array
         return arr[~np.isnan(arr)]
 
 
@@ -4379,15 +4651,15 @@
 
     See Also
     --------
     cticks, cticksize, ctickweight, ctickprops
     vcticks, vcticksize, vctickweight, vctickprops
     """
 
-    name = 'Colorbar ticklabels'
+    name = "Colorbar ticklabels"
 
     @property
     def default_formatters(self):
         """Default locator of the axis of the colorbars"""
         if self._default_formatters:
             return self._default_formatters
         else:
@@ -4417,19 +4689,19 @@
     %(fontsizes)s
 
     See Also
     --------
     ctickweight, ctickprops, cticklabels, cticks
     vctickweight, vctickprops, vcticklabels, vcticks"""
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Font size of the colorbar ticklabels'
+    name = "Font size of the colorbar ticklabels"
 
-    dependencies = CbarOptions.dependencies + ['ctickprops']
+    dependencies = CbarOptions.dependencies + ["ctickprops"]
 
 
 class CTickWeight(CbarOptions, TickWeightBase):
     """
     Specify the fontweight of the colorbar ticklabels
 
     Possible types
@@ -4437,19 +4709,19 @@
     %(fontweights)s
 
     See Also
     --------
     cticksize, ctickprops, cticklabels, cticks
     vcticksize, vctickprops, vcticklabels, vcticks"""
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Font weight of the colorbar ticklabels'
+    name = "Font weight of the colorbar ticklabels"
 
-    dependencies = CbarOptions.dependencies + ['ctickprops']
+    dependencies = CbarOptions.dependencies + ["ctickprops"]
 
 
 class CTickProps(CbarOptions, TickPropsBase):
     """
     Specify the font properties of the colorbar ticklabels
 
     Possible types
@@ -4459,39 +4731,50 @@
     See Also
     --------
     cticksize, ctickweight, cticklabels, cticks
     vcticksize, vctickweight, vcticklabels, vcticks"""
 
     children = CbarOptions.children + TickPropsBase.children
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Font properties of the colorbar ticklabels'
+    name = "Font properties of the colorbar ticklabels"
 
     def update_axis(self, value):
         value = value.copy()
         default = self.default
-        if 'major' in default or 'minor' in default:
+        if "major" in default or "minor" in default:
             default = default.get(self.which, {})
         for key, val in chain(
-                default.items(), mpl.rcParams.find_all(
-                    self.axisname + 'tick\.%s\.\w' % self.which).items()):
-            value.setdefault(key.split('.')[-1], val)
-
-        if float('.'.join(mpl.__version__.split('.')[:2])) >= 1.5:
-            value.pop('visible', None)
-        posnames = ['top', 'bottom'] if self.axisname == 'x' else [
-            'left', 'right']
-        label_positions = dict(zip(
-            map('label{}'.format, posnames),
-            [True, False] if self.position in ['t', 'ft', 'l', 'fl'] else
-            [False, True]))
+            default.items(),
+            mpl.rcParams.find_all(
+                self.axisname + r"tick\.%s\.\w" % self.which
+            ).items(),
+        ):
+            value.setdefault(key.split(".")[-1], val)
+
+        if float(".".join(mpl.__version__.split(".")[:2])) >= 1.5:
+            value.pop("visible", None)
+        posnames = (
+            ["top", "bottom"] if self.axisname == "x" else ["left", "right"]
+        )
+        label_positions = dict(
+            zip(
+                map("label{}".format, posnames),
+                (
+                    [True, False]
+                    if self.position in ["t", "ft", "l", "fl"]
+                    else [False, True]
+                ),
+            )
+        )
         label_positions.update(**value)
         self.colorbar.ax.tick_params(
-            self.axisname, which=self.which, reset=True, **label_positions)
+            self.axisname, which=self.which, reset=True, **label_positions
+        )
 
 
 class ArrowSize(Formatoption):
     """
     Change the size of the arrows
 
     Possible types
@@ -4501,30 +4784,30 @@
     float
         Factor scaling the size of the arrows
 
     See Also
     --------
     arrowstyle, linewidth, density, color"""
 
-    group = 'vector'
+    group = "vector"
 
     priority = BEFOREPLOTTING
 
-    dependencies = ['plot']
+    dependencies = ["plot"]
 
-    name = 'Size of the arrows'
+    name = "Size of the arrows"
 
     def update(self, value):
         kwargs = self.plot._kwargs
-        if self.plot.value == 'stream':
-            kwargs.pop('scale', None)
-            kwargs['arrowsize'] = value or 1.0
+        if self.plot.value == "stream":
+            kwargs.pop("scale", None)
+            kwargs["arrowsize"] = value or 1.0
         else:
-            kwargs.pop('arrowsize', None)
-            kwargs['scale'] = value
+            kwargs.pop("arrowsize", None)
+            kwargs["scale"] = value
 
 
 class ArrowStyle(Formatoption):
     """Change the style of the arrows
 
     Possible types
     --------------
@@ -4536,30 +4819,30 @@
     -----
     This formatoption only has an effect for stream plots
 
     See Also
     --------
     arrowsize, linewidth, density, color"""
 
-    group = 'vector'
+    group = "vector"
 
     priority = BEFOREPLOTTING
 
-    dependencies = ['plot']
+    dependencies = ["plot"]
 
-    name = 'Style of the arrows'
+    name = "Style of the arrows"
 
     def update(self, value):
-        if self.plot.value == 'stream':
-            self.plot._kwargs['arrowstyle'] = value
+        if self.plot.value == "stream":
+            self.plot._kwargs["arrowstyle"] = value
         else:
-            self.plot._kwargs.pop('arrowstyle', None)
+            self.plot._kwargs.pop("arrowstyle", None)
 
 
-@docstrings.get_sections(base='WindCalculator')
+@docstrings.get_sections(base="WindCalculator")
 class VectorCalculator(Formatoption):
     """
     Abstract formatoption that provides calculation functions for speed, etc.
 
     Possible types
     --------------
     string {'absolute', 'u', 'v'}
@@ -4567,39 +4850,46 @@
         are
 
         - **absolute**: for the absolute wind speed
         - **u**: for the u component
         - **v**: for the v component
     """
 
-    dependencies = ['plot', 'transpose']
+    dependencies = ["plot", "transpose"]
 
     priority = BEFOREPLOTTING
 
     data_dependent = True
 
     def __init__(self, *args, **kwargs):
         super(VectorCalculator, self).__init__(*args, **kwargs)
         self._calc_funcs = {
-            'absolute': self._calc_speed,
-            'u': self._get_u,
-            'v': self._get_v}
+            "absolute": self._calc_speed,
+            "u": self._get_u,
+            "v": self._get_v,
+        }
 
     def _maybe_ravel(self, arr):
-        if (getattr(self, 'transpose', None) is not None and
-                self.transpose.value):
+        if (
+            getattr(self, "transpose", None) is not None
+            and self.transpose.value
+        ):
             arr = arr.T
-        if self.plot.value == 'quiver':
+        if self.plot.value == "quiver":
             return np.ravel(arr)
         return np.asarray(arr)
 
     def _calc_speed(self, scale=1.0):
         data = self.plot.data
-        return self._maybe_ravel(
-            np.sqrt(data[0].values**2 + data[1].values**2)) * scale
+        return (
+            self._maybe_ravel(
+                np.sqrt(data[0].values ** 2 + data[1].values ** 2)
+            )
+            * scale
+        )
 
     def _get_u(self, scale=1.0):
         return self._maybe_ravel(self.plot.data[0].values) * scale
 
     def _get_v(self, scale=1.0):
         return self._maybe_ravel(self.plot.data[1].values) * scale
 
@@ -4620,25 +4910,27 @@
         The values determine the linewidth for each plotted arrow. Note that
         the shape has to match the one of u and v.
 
     See Also
     --------
     arrowsize, arrowstyle, density, color"""
 
-    name = 'Linewidth of the arrows'
+    name = "Linewidth of the arrows"
 
     def update(self, value):
         if value is None:
-            self.plot._kwargs['linewidth'] = 0 if self.plot.value == 'quiver' \
-                else None
+            self.plot._kwargs["linewidth"] = (
+                0 if self.plot.value == "quiver" else None
+            )
         elif np.asarray(value).ndim and isinstance(value[0], six.string_types):
-            self.plot._kwargs['linewidth'] = self._calc_funcs[value[0]](
-                *value[1:])
+            self.plot._kwargs["linewidth"] = self._calc_funcs[value[0]](
+                *value[1:]
+            )
         else:
-            self.plot._kwargs['linewidth'] = self._maybe_ravel(value)
+            self.plot._kwargs["linewidth"] = self._maybe_ravel(value)
 
 
 class VectorColor(VectorCalculator):
     """
     Set the color for the arrows
 
     This formatoption can be used to set a single color for the vectors or
@@ -4658,62 +4950,65 @@
         The values determine the color for each plotted arrow. Note that
         the shape has to match the one of u and v.
 
     See Also
     --------
     arrowsize, arrowstyle, density, linewidth"""
 
-    dependencies = VectorCalculator.dependencies + ['cmap', 'bounds']
+    dependencies = VectorCalculator.dependencies + ["cmap", "bounds"]
 
-    group = 'colors'
+    group = "colors"
 
-    name = 'Color of the arrows'
+    name = "Color of the arrows"
 
     def update(self, value):
         try:
             value = validate_color(value)
             self.colored = False
         except ValueError:
-            if (isinstance(value, six.string_types) and
-                    value in self._calc_funcs):
+            if (
+                isinstance(value, six.string_types)
+                and value in self._calc_funcs
+            ):
                 value = self._calc_funcs[value]()
                 self.colored = True
                 self._color_array = value
             else:
                 try:
                     value = validate_float(value)
                     self.colored = False
                 except ValueError:
                     value = self._maybe_ravel(value)
                     self.colored = True
                     self._color_array = value
-        if self.plot.value == 'quiver' and self.colored:
+        if self.plot.value == "quiver" and self.colored:
             self.plot._args = [value]
-            self.plot._kwargs.pop('color', None)
+            self.plot._kwargs.pop("color", None)
         else:
             self.plot._args = []
-            self.plot._kwargs['color'] = value
+            self.plot._kwargs["color"] = value
         if self.colored:
             self._set_cmap()
         else:
             self._delete_cmap()
 
     def _set_cmap(self):
         if self.plotter.has_changed(self.key) or self.plotter._initializing:
             self.bounds.update(self.bounds.value)
-        self.plot._kwargs['cmap'] = get_cmap(
-            self.cmap.value, len(self.bounds.bounds) - 1 or None)
-        self.plot._kwargs['norm'] = self.bounds.norm
+        self.plot._kwargs["cmap"] = get_cmap(
+            self.cmap.value, len(self.bounds.bounds) - 1 or None
+        )
+        self.plot._kwargs["norm"] = self.bounds.norm
 
     def _delete_cmap(self):
-        self.plot._kwargs.pop('cmap', None)
-        self.plot._kwargs.pop('norm', None)
+        self.plot._kwargs.pop("cmap", None)
+        self.plot._kwargs.pop("norm", None)
 
 
-@docstrings.get_sections(base='Density')
+@docstrings.get_sections(base="Density")
 class Density(Formatoption):
     """
     Change the density of the arrows
 
     Possible types
     --------------
     float
@@ -4723,56 +5018,60 @@
         Defines the scaling in x- and y-direction manually
 
     Notes
     -----
     quiver plots do not support density scaling
     """
 
-    dependencies = ['plot']
+    dependencies = ["plot"]
 
-    group = 'vector'
+    group = "vector"
 
-    name = 'Density of the arrows'
+    name = "Density of the arrows"
 
     priority = BEFOREPLOTTING
 
     data_dependent = True
 
     def __init__(self, *args, **kwargs):
         super(Density, self).__init__(*args, **kwargs)
         self._density_funcs = {
-            'stream': self._set_stream_density,
-            'quiver': self._set_quiver_density}
+            "stream": self._set_stream_density,
+            "quiver": self._set_quiver_density,
+        }
         self._remove_funcs = {
-            'stream': self._unset_stream_density,
-            'quiver': self._unset_quiver_density}
+            "stream": self._unset_stream_density,
+            "quiver": self._unset_quiver_density,
+        }
 
     def update(self, value):
         has_changed = self.plotter.has_changed(self.plot.key)
         if has_changed:
             self.remove(has_changed[0])
         try:
             value = tuple(value)
         except TypeError:
             value = [value, value]
         if self.plot.value:
             self._density_funcs[self.plot.value](value)
 
     def _set_stream_density(self, value):
         return
-        self.plot._kwargs['density'] = value
+        self.plot._kwargs["density"] = value
 
     def _set_quiver_density(self, value):
         if any(val != 1.0 for val in value):
-            warn("[%s] - Quiver plot does not support the density "
-                 "keyword!" % self.logger.name,
-                 RuntimeWarning)
+            warn(
+                "[%s] - Quiver plot does not support the density "
+                "keyword!" % self.logger.name,
+                RuntimeWarning,
+            )
 
     def _unset_stream_density(self):
-        self.plot._kwargs.pop('density', None)
+        self.plot._kwargs.pop("density", None)
 
     def _unset_quiver_density(self):
         pass
 
     def remove(self, plot_type=None):
         plot_type = plot_type or self.plot.value
         self._remove_funcs[plot_type]()
@@ -4790,34 +5089,41 @@
         quiver
             to make a quiver plot
         stream
             to make a stream plot"""
 
     plot_fmt = True
 
-    group = 'plotting'
+    group = "plotting"
 
-    name = 'Plot type of the arrows'
+    name = "Plot type of the arrows"
 
     priority = BEFOREPLOTTING
 
-    children = ['cmap', 'bounds']
+    children = ["cmap", "bounds"]
 
-    connections = ['transpose', 'transform', 'arrowsize', 'arrowstyle',
-                   'density', 'linewidth', 'color']
+    connections = [
+        "transpose",
+        "transform",
+        "arrowsize",
+        "arrowstyle",
+        "density",
+        "linewidth",
+        "color",
+    ]
 
     @property
     def format_coord(self):
         """The function that can replace the axes.format_coord method"""
         return format_coord_func(self.ax, weakref.ref(self))
 
     @property
     def mappable(self):
         """The mappable, i.e. the container of the plot"""
-        if self.value == 'stream':
+        if self.value == "stream":
             return self._plot.lines
         else:
             return self._plot
 
     @property
     def xcoord(self):
         """The x coordinate :class:`xarray.Variable`"""
@@ -4829,16 +5135,17 @@
         """The y coordinate :class:`xarray.Variable`"""
         v = next(self.raw_data.psy.iter_base_variables)
         return self.decoder.get_y(v, coords=self.data.coords)
 
     def __init__(self, *args, **kwargs):
         Formatoption.__init__(self, *args, **kwargs)
         self._plot_funcs = {
-            'quiver': self._quiver_plot,
-            'stream': self._stream_plot}
+            "quiver": self._quiver_plot,
+            "stream": self._stream_plot,
+        }
         self._orig_format_coord = None
         self._args = []
         self._kwargs = {}
 
     @property
     def array(self):
         return self.data.values
@@ -4847,28 +5154,35 @@
         pass
         # the real plot making is done by make_plot but we store the value here
         # in case it is shared
 
     def make_plot(self):
         # remove the plot if it shall be replotted or any of the dependencies
         # changed. Otherwise there is nothing to change
-        if hasattr(self, '_plot') and (self.plotter.replot or any(
-                self.plotter.has_changed(key) for key in chain(
-                    self.connections, self.dependencies, [self.key]))):
+        if hasattr(self, "_plot") and (
+            self.plotter.replot
+            or any(
+                self.plotter.has_changed(key)
+                for key in chain(
+                    self.connections, self.dependencies, [self.key]
+                )
+            )
+        ):
             self.remove()
         if not hasattr(self, "_plot") and self.value is not None:
             self._plot_funcs[self.value]()
             if self._orig_format_coord is None:
                 self._orig_format_coord = self.ax.format_coord
                 self.ax.format_coord = self.format_coord
 
     def _quiver_plot(self):
         x, y, u, v = self._get_data()
-        self._plot = self.ax.quiver(x, y, u, v, *self._args, rasterized=True,
-                                    **self._kwargs)
+        self._plot = self.ax.quiver(
+            x, y, u, v, *self._args, rasterized=True, **self._kwargs
+        )
 
     def _stream_plot(self):
         x, y, u, v = self._get_data()
         dx = (x[-1] - x[0]) / (len(x) - 1)
         dy = (y[-1] - y[0]) / (len(y) - 1)
         if not np.allclose(np.diff(x), dx):
             warn("Rescaling x to be equally spaced!", PsyPlotRuntimeWarning)
@@ -4896,129 +5210,149 @@
         else:
             u, v = data.values
         x = self.transpose.get_x(data)
         y = self.transpose.get_y(data)
         return np.asarray(x), np.asarray(y), u, v
 
     def remove(self):
-
         def keep(x):
             return not isinstance(x, mpl.patches.FancyArrowPatch)
 
-        if not hasattr(self, '_plot'):
+        if not hasattr(self, "_plot"):
             return
         if isinstance(self._plot, mpl.streamplot.StreamplotSet):
             try:
                 self._plot.lines.remove()
             except ValueError:
                 pass
             # remove arrows
             for patch in list(self.ax.patches):
                 if not keep(patch):
-                    self.ax.patches.remove(patch)
+                    patch.remove()
         else:
             try:
                 self._plot.remove()
             except ValueError:  # the artist has already been removed
                 pass
         del self._plot
 
     def add2format_coord(self, x, y):
         """Additional information for the :meth:`format_coord`"""
         u, v = self.data
-        uname, vname = self.data.coords['variable'].values
+        uname, vname = self.data.coords["variable"].values
         xcoord = self.xcoord
         ycoord = self.ycoord
         if self.decoder.is_unstructured(self.raw_data[0]):
             x, y, z1, z2 = self.get_xyz_tri(xcoord, x, ycoord, y, u, v)
         elif xcoord.ndim == 1:
             x, y, z1, z2 = self.get_xyz_1d(xcoord, x, ycoord, y, u, v)
         elif xcoord.ndim == 2:
             x, y, z1, z2 = self.get_xyz_2d(xcoord, x, ycoord, y, u, v)
-        speed = (z1**2 + z2**2)**0.5
-        xunit = xcoord.attrs.get('units', '')
+        speed = (z1**2 + z2**2) ** 0.5
+        xunit = xcoord.attrs.get("units", "")
         if xunit:
-            xunit = ' ' + xunit
-        yunit = ycoord.attrs.get('units', '')
+            xunit = " " + xunit
+        yunit = ycoord.attrs.get("units", "")
         if yunit:
-            yunit = ' ' + yunit
-        zunit = u.attrs.get('units', '')
+            yunit = " " + yunit
+        zunit = u.attrs.get("units", "")
         if zunit:
-            zunit = ' ' + zunit
-        return (', vector data: %s: %.4g%s, %s: %.4g%s, %s: %.4g%s, '
-                '%s: %.4g%s, absolute: %.4g%s') % (
-                    xcoord.name, x, xunit, ycoord.name, y, yunit,
-                    uname, z1, zunit, vname, z2, zunit,
-                    speed, zunit)
+            zunit = " " + zunit
+        return (
+            ", vector data: %s: %.4g%s, %s: %.4g%s, %s: %.4g%s, "
+            "%s: %.4g%s, absolute: %.4g%s"
+        ) % (
+            xcoord.name,
+            x,
+            xunit,
+            ycoord.name,
+            y,
+            yunit,
+            uname,
+            z1,
+            zunit,
+            vname,
+            z2,
+            zunit,
+            speed,
+            zunit,
+        )
 
     def get_xyz_tri(self, xcoord, x, ycoord, y, u, v):
         """Get closest x, y and z for the given `x` and `y` in `data` for
         1d coords"""
         return self.get_xyz_2d(xcoord, x, ycoord, y, u, v)
 
     def get_xyz_1d(self, xcoord, x, ycoord, y, u, v):
         """Get closest x, y and z for the given `x` and `y` in `data` for
         1d coords"""
-        xclose = xcoord.indexes[xcoord.name].get_loc(x, method='nearest')
-        yclose = ycoord.indexes[ycoord.name].get_loc(y, method='nearest')
+        xclose = xcoord.indexes[xcoord.name].get_loc(x, method="nearest")
+        yclose = ycoord.indexes[ycoord.name].get_loc(y, method="nearest")
         uval = u[yclose, xclose].values
         vval = v[yclose, xclose].values
         return xcoord[xclose].values, ycoord[yclose].values, uval, vval
 
     def get_xyz_2d(self, xcoord, x, ycoord, y, u, v):
         """Get closest x, y and z for the given `x` and `y` in `data` for
         2d coords"""
         xy = xcoord.values.ravel() + 1j * ycoord.values.ravel()
         dist = np.abs(xy - (x + 1j * y))
         imin = np.nanargmin(dist)
         xy_min = xy[imin]
-        return (xy_min.real, xy_min.imag, u.values.ravel()[imin],
-                v.values.ravel()[imin])
+        return (
+            xy_min.real,
+            xy_min.imag,
+            u.values.ravel()[imin],
+            v.values.ravel()[imin],
+        )
 
 
 class SimpleVectorPlot(VectorPlot):
     # disable the stream plot for unstructured grids because it is not supported
     # for 1d arrays and for circumpolar grids because 2d coordinates are not
     # supported
 
     __doc__ = VectorPlot.__doc__
 
     def set_value(self, value, *args, **kwargs):
-        if value == 'stream' and self.raw_data is not None:
+        if value == "stream" and self.raw_data is not None:
             u = self.raw_data[0]
             if u.psy.decoder.is_unstructured(u):
-                warn('[%s] - Streamplot is not supported for unstructured '
-                     'grids!' % self.logger.name)
-                value = 'quiver'
+                warn(
+                    "[%s] - Streamplot is not supported for unstructured "
+                    "grids!" % self.logger.name
+                )
+                value = "quiver"
             elif u.psy.decoder.is_circumpolar(u):
-                warn('[%s] - Streamplot is not supported for circumpolar '
-                     'grids!' % self.logger.name)
-                value = 'quiver'
+                warn(
+                    "[%s] - Streamplot is not supported for circumpolar "
+                    "grids!" % self.logger.name
+                )
+                value = "quiver"
         super(SimpleVectorPlot, self).set_value(value, *args, **kwargs)
 
 
 class CombinedVectorPlot(VectorPlot):
-
     __doc__ = VectorPlot.__doc__
 
     def update(self, *args, **kwargs):
-        self._kwargs['zorder'] = 2
+        self._kwargs["zorder"] = 2
         super(CombinedVectorPlot, self).update(*args, **kwargs)
 
 
 class VectorCbar(Cbar):
     """
     Specify the position of the vector plot colorbars
 
     Possible types
     --------------
     %(Cbar.possible_types)s
     """
 
-    dependencies = Cbar.dependencies + ['color']
+    dependencies = Cbar.dependencies + ["color"]
 
     priority = END
 
     def update(self, *args, **kwargs):
         if self.color.colored:
             super(VectorCbar, self).update(*args, **kwargs)
         else:
@@ -5037,15 +5371,15 @@
     --------
     %(Bounds.examples)s
 
     See Also
     --------
     %(Bounds.see_also)s"""
 
-    parents = ['color']
+    parents = ["color"]
 
     @property
     def array(self):
         arr = self.color._color_array
         return arr[~np.isnan(arr)]
 
     def update(self, *args, **kwargs):
@@ -5070,31 +5404,38 @@
 
     See Also
     --------
     legend"""
 
     data_dependent = True
 
-    name = 'Labels in the legend'
+    name = "Labels in the legend"
 
     def update(self, value):
         def get1d(arr):
             if arr.ndim > 1:
                 return arr[0]
             return arr
+
         if isinstance(value, six.string_types):
             self.labels = [
-                self.replace(value, arr, self.get_enhanced_attrs(
-                    get1d(arr), replot=True))
-                for arr in self.iter_data]
+                self.replace(
+                    value,
+                    arr,
+                    self.get_enhanced_attrs(get1d(arr), replot=True),
+                )
+                for arr in self.iter_data
+            ]
         else:
             self.labels = [
-                self.replace(val, arr, self.get_enhanced_attrs(
-                    get1d(arr), replot=True)) for val, arr in zip(
-                        value, self.iter_data)]
+                self.replace(
+                    val, arr, self.get_enhanced_attrs(get1d(arr), replot=True)
+                )
+                for val, arr in zip(value, self.iter_data)
+            ]
 
 
 class Legend(DictFormatoption):
     """
     Draw a legend
 
     This formatoption determines where and if to draw the legend. It uses the
@@ -5109,45 +5450,48 @@
     dict
         Give the keywords for the :func:`matplotlib.pyplot.legend` function
 
     See Also
     --------
     labels"""
 
-    dependencies = ['legendlabels', 'plot', 'color', 'marker']
+    dependencies = ["legendlabels", "plot", "color", "marker"]
 
-    name = 'Properties of the legend'
+    name = "Properties of the legend"
 
     def update(self, value):
         self.remove()
         shared_by = self.shared_by
         if shared_by is not None:
             # update the legend of the other formatoption instead of this one
             if not shared_by.plotter._updating:
                 shared_by.update(shared_by.value)
             return
-        if not value.get('loc'):
+        if not value.get("loc"):
             return
         artists = []
         labels = []
         for fmto in self.shared.union([self]):
-            if hasattr(fmto.plot, '_plot'):
+            if hasattr(fmto.plot, "_plot"):
                 this_artists, this_labels = fmto.get_artists_and_labels()
                 artists.extend(this_artists)
                 labels.extend(this_labels)
         self.legend = self.ax.legend(artists, labels, **value)
 
     def get_artists_and_labels(self):
         return self.plot._plot, [
-            l for l, ls in zip(self.legendlabels.labels,
-                               cycle(slist(self.plot.value)))
-            if ls is not None]
+            label
+            for label, ls in zip(
+                self.legendlabels.labels, cycle(slist(self.plot.value))
+            )
+            if ls is not None
+        ]
 
     def remove(self):
-        if hasattr(self, 'legend'):
+        if hasattr(self, "legend"):
             self.legend.remove()
 
 
 class MeanCalculator(Formatoption):
     """
     Determine how the error is visualized
 
@@ -5163,27 +5507,27 @@
     See Also
     --------
     err_calc: Determines how to calculate the error
     """
 
     priority = START
 
-    name = 'Mean calculation'
+    name = "Mean calculation"
 
-    group = 'data'
+    group = "data"
 
     data_dependent = True
 
     requires_replot = True
 
     def update(self, value):
         for i, arr in enumerate(self.iter_data):
-            if value == 'mean':
+            if value == "mean":
                 data = arr.psy.fldmean()
-            elif value == 'median':
+            elif value == "median":
                 data = arr.psy.fldpctl(50)
             else:
                 data = arr.psy.fldpctl(value)
             data.psy.arr_name = arr.psy.arr_name
             self.set_data(data, i)
 
 
@@ -5212,56 +5556,57 @@
     See Also
     --------
     mean: Determines how the line is calculated
     """
 
     priority = START
 
-    name = 'Mean calculation'
+    name = "Mean calculation"
 
-    group = 'data'
+    group = "data"
 
-    children = ['mean']
+    children = ["mean"]
 
     data_dependent = True
 
     requires_replot = True
 
     def update(self, value):
         if value is None:
             return
         if isstring(value):
             use_std = True
-            m = re.search(r'\d+\.?\d*', value)
+            m = re.search(r"\d+\.?\d*", value)
             if m:
                 multiplier = float(m.group())
             else:
                 multiplier = 1
         else:
             use_std = False
-        for i, (arr, mean) in enumerate(zip(self.iter_raw_data,
-                                            self.iter_data)):
+        for i, (arr, mean) in enumerate(
+            zip(self.iter_raw_data, self.iter_data)
+        ):
             mean = mean.to_dataset()
             if use_std:
                 err = multiplier * arr.psy.fldstd()
                 mean[value] = err.variable
                 data = mean[[arr.name, value]].psy.to_array()
             else:
                 err = arr.psy.fldpctl(value)
-                names = list(map('pctl{:1.3g}'.format, value))
+                names = list(map("pctl{:1.3g}".format, value))
                 mean[names[0]] = err.variable[0]
                 mean[names[1]] = err.variable[1]
                 data = mean[[arr.name] + names].psy.to_array()
             data.psy.arr_name = arr.psy.arr_name
             data.attrs.update(arr.attrs)
             data.name = arr.name
             self.set_data(data, i)
 
 
-docstrings.delete_types('LimitBase.possible_types', 'no_None', 'None')
+docstrings.delete_types("LimitBase.possible_types", "no_None", "None")
 
 
 class Hist2DXRange(LimitBase):
     """
     Specify the range of the histogram for the x-dimension
 
     This formatoption specifies the minimum and maximum of the histogram
@@ -5278,29 +5623,30 @@
 
     See also
     --------
     yrange"""
 
     priority = START
 
-    group = 'data'
+    group = "data"
 
-    name = 'Range of the histogram in x-direction'
+    name = "Range of the histogram in x-direction"
 
     data_dependent = True
 
-    dependencies = ['coord']
+    dependencies = ["coord"]
 
     @property
     def array(self):
         # We don't use the :attr:`data` attribute because this fails if the
         # formatoption is shared and the ``coord`` formatoption is not None
         if self.coord.value is not None:
             coord = self.coord.get_alternative_coord(
-                self.raw_data, self.index_in_list or 0)[1].values
+                self.raw_data, self.index_in_list or 0
+            )[1].values
         else:
             da = self.raw_data
             coord = da.coords[da.dims[0]].values
         ret = coord[~np.isnan(coord)]
         return ret
 
     def set_limit(self, *args):
@@ -5323,15 +5669,15 @@
     This formatoption always acts on the DataArray, no matter what the
     value of the :attr:`transpose` formatoption is
 
     See Also
     --------
     xrange"""
 
-    name = 'Range of the histogram in y-direction'
+    name = "Range of the histogram in y-direction"
 
     data_dependent = True
 
     @property
     def array(self):
         return np.asarray(self.raw_data)[np.asarray(self.raw_data.notnull())]
 
@@ -5352,33 +5698,35 @@
     str
         One of ``{'scott' | 'silverman'}``. This uses the statsmodels package
         to estimate the bandwidth of the data that is then used in the
         histogram or KDE plot"""
 
     priority = START
 
-    dependencies = ['xrange', 'yrange']
+    dependencies = ["xrange", "yrange"]
 
-    connections = ['density']
+    connections = ["density"]
 
-    group = 'data'
+    group = "data"
 
-    name = 'Precision of the visualized data'
+    name = "Precision of the visualized data"
 
     data_dependent = True
 
     def estimate_bw(self, method, values, data_range=None):
         import statsmodels.nonparametric.api as smnp
+
         bw_func = getattr(smnp.bandwidths, "bw_" + method)
         if data_range is not None:
             vmin, vmax = sorted(data_range)
             values = values[(values >= vmin) & (values <= vmax)]
         if not len(values):
-            raise ValueError("No values found within the given range of "
-                             f"{data_range}!")
+            raise ValueError(
+                "No values found within the given range of " f"{data_range}!"
+            )
         return bw_func(values)
 
     def update(self, value):
         self.bins = [0, 0]
         value = slist(value)
         if len(value) == 1:
             value = [value[0], value[0]]
@@ -5421,31 +5769,31 @@
         otherwise the number of bins to use
     tuple (x, y) of int
         The bins for x and y explicitly
     """
 
     priority = START
 
-    dependencies = ['precision']
+    dependencies = ["precision"]
 
-    group = 'data'
+    group = "data"
 
-    name = 'Number of bins of the histogram'
+    name = "Number of bins of the histogram"
 
     data_dependent = True
 
     def update(self, value):
         self.bins = [0, 0]
         try:
             value = tuple(value)
         except TypeError:
             value = [value, value]
         for i, (bins, bins_prec) in enumerate(zip(value, self.precision.bins)):
             if bins == 0 and bins_prec == 0:
-                raise ValueError('precision and bins must not both be 0!')
+                raise ValueError("precision and bins must not both be 0!")
             elif bins == 0:
                 self.bins[i] = bins_prec
             elif bins_prec == 0:
                 self.bins[i] = bins
             else:
                 self.bins[i] = min(bins, bins_prec)
 
@@ -5477,46 +5825,49 @@
     See Also
     --------
     density
     """
 
     priority = START
 
-    name = 'Specify how to normalize the histogram'
+    name = "Specify how to normalize the histogram"
 
-    group = 'data'
+    group = "data"
 
-    name = 'Normalize the histogram'
+    name = "Normalize the histogram"
 
     data_dependent = True
 
     def update(self, value):
         pass  # nothing to do here
 
     def hist2d(self, da, **kwargs):
         """Make the two dimensional histogram
 
         Parameters
         ----------
         da: xarray.DataArray
             The data source"""
-        if self.value is None or self.value == 'counts':
+        if self.value is None or self.value == "counts":
             normed = False
         else:
             normed = True
         y = da.values
         x = da.coords[da.dims[0]].values
-        counts, xedges, yedges = np.histogram2d(
-            x, y, normed=normed, **kwargs)
-        if self.value == 'counts':  # normalize such that all values sum to one
+        if mpl_version < 3.3:
+            kwargs["normed"] = normed
+        else:
+            kwargs["density"] = normed
+        counts, xedges, yedges = np.histogram2d(x, y, **kwargs)
+        if self.value == "counts":  # normalize such that all values sum to one
             counts = counts / counts.sum().astype(float)
-        elif self.value in ['x', 'col', 'column', 'columns']:
+        elif self.value in ["x", "col", "column", "columns"]:
             # normalize such that every column sums to one
             counts = counts / counts.sum(axis=1, keepdims=True).astype(float)
-        elif self.value in ['y', 'row', 'rows']:
+        elif self.value in ["y", "row", "rows"]:
             # normalize such that every row sums to one
             counts = counts / counts.sum(axis=1, keepdims=True).astype(float)
         return counts, xedges, yedges
 
 
 class PointDensity(Formatoption):
     """
@@ -5533,68 +5884,75 @@
         kde
             Fit a bivariate kernel density estimate to the data. Note that
             this choice requires pythons [statsmodels]_ module to be
             installed
 
     References
     ----------
-    .. [statsmodels] http://statsmodels.sourceforge.net/
+    .. [statsmodels] https://www.statsmodels.org
     """
 
     priority = START
 
-    name = 'Type of the density plot'
+    name = "Type of the density plot"
 
-    dependencies = ['normed', 'bins', 'xrange', 'yrange', 'precision', 'coord']
+    dependencies = ["normed", "bins", "xrange", "yrange", "precision", "coord"]
 
-    group = 'data'
+    group = "data"
 
-    name = 'Calculation of the point density'
+    name = "Calculation of the point density"
 
     data_dependent = True
 
     def update(self, value):
-        if value == 'hist':
+        if value == "hist":
             self._hist()
         else:
             self._kde()
 
     def _kde(self):
         if self.coord.value is None:
             raw_da = self.raw_data
         else:
             raw_da = self.coord.replace_coord(0)
         xyranges = [self.xrange.range, self.yrange.range]
         bws = self.precision.prec
         grid = self.bins.bins
         for i, bw in enumerate(bws):
             if bw == 0:
-                bws[i] = 'scott'
+                bws[i] = "scott"
         coord = raw_da.coords[raw_da.dims[0]]
         xname = coord.name
         yname = raw_da.name
         x, y, z = self._statsmodels_bivariate_kde(
-            raw_da.coords[raw_da.dims[0]].values, raw_da.values, bws,
-            grid[0], grid[1], xyranges)
-        xcent = xr.Variable((xname, ), x, attrs=coord.attrs.copy())
-        ycent = xr.Variable((yname, ), y, attrs=raw_da.attrs.copy())
-        var = xr.Variable((yname, xname), z,
-                          attrs=raw_da.psy.base.attrs.copy())
-        ds = xr.Dataset({'counts': var}, {xname: xcent, yname: ycent})
+            raw_da.coords[raw_da.dims[0]].values,
+            raw_da.values,
+            bws,
+            grid[0],
+            grid[1],
+            xyranges,
+        )
+        xcent = xr.Variable((xname,), x, attrs=coord.attrs.copy())
+        ycent = xr.Variable((yname,), y, attrs=raw_da.attrs.copy())
+        var = xr.Variable(
+            (yname, xname), z, attrs=raw_da.psy.base.attrs.copy()
+        )
+        ds = xr.Dataset({"counts": var}, {xname: xcent, yname: ycent})
         ds = ds.assign_coords(**self._get_other_coords(raw_da))
         self.decoder = CFDecoder(ds)
         arr = ds.counts
         arr.psy.init_accessor(base=ds, decoder=self.decoder)
         self.data = arr
 
     def _statsmodels_bivariate_kde(self, x, y, bws, xsize, ysize, xyranges):
         """Compute a bivariate kde using statsmodels.
         This function is mainly motivated through
         seaborn.distributions._statsmodels_bivariate_kde"""
         import statsmodels.nonparametric.api as smnp
+
         for i, (coord, bw) in enumerate(zip([x, y], bws)):
             if isinstance(bw, six.string_types):
                 bw_func = getattr(smnp.bandwidths, "bw_" + bw)
                 bws[i] = bw_func(coord)
         kde = smnp.KDEMultivariate([x, y], "cc", bws)
         x_support = np.linspace(xyranges[0][0], xyranges[0][1], xsize)
         y_support = np.linspace(xyranges[1][0], xyranges[1][1], ysize)
@@ -5610,109 +5968,123 @@
         bins = self.bins.bins
         range_ = [self.xrange.range, self.yrange.range]
         z, x, y = self.normed.hist2d(raw_da, bins=bins, range=range_)
         coord = raw_da.coords[raw_da.dims[0]]
         xname = coord.name
         yname = raw_da.name
         # calculate the centers
-        xcent = xr.Variable((xname, ), np.c_[[x[:-1], x[1:]]].mean(axis=0),
-                            attrs=coord.attrs.copy())
-        ycent = xr.Variable((yname, ), np.c_[[y[:-1], y[1:]]].mean(axis=0),
-                            attrs=raw_da.attrs.copy())
-        xbounds = xr.Variable((xname, 'bnds'), np.c_[[x[:-1], x[1:]]].T)
-        ybounds = xr.Variable((yname, 'bnds'), np.c_[[y[:-1], y[1:]]].T)
-        xcent.attrs['bounds'] = xname + '_bnds'
-        ycent.attrs['bounds'] = yname + '_bnds'
-        var = xr.Variable((yname, xname), z.T,
-                          attrs=raw_da.psy.base.attrs.copy())
-        variables = {'counts': var}
-        coords = {xname: xcent, yname: ycent,
-                  xname + '_bnds': xbounds, yname + '_bnds': ybounds}
+        xcent = xr.Variable(
+            (xname,),
+            np.c_[[x[:-1], x[1:]]].mean(axis=0),
+            attrs=coord.attrs.copy(),
+        )
+        ycent = xr.Variable(
+            (yname,),
+            np.c_[[y[:-1], y[1:]]].mean(axis=0),
+            attrs=raw_da.attrs.copy(),
+        )
+        xbounds = xr.Variable((xname, "bnds"), np.c_[[x[:-1], x[1:]]].T)
+        ybounds = xr.Variable((yname, "bnds"), np.c_[[y[:-1], y[1:]]].T)
+        xcent.attrs["bounds"] = xname + "_bnds"
+        ycent.attrs["bounds"] = yname + "_bnds"
+        var = xr.Variable(
+            (yname, xname), z.T, attrs=raw_da.psy.base.attrs.copy()
+        )
+        variables = {"counts": var}
+        coords = {
+            xname: xcent,
+            yname: ycent,
+            xname + "_bnds": xbounds,
+            yname + "_bnds": ybounds,
+        }
         ds = xr.Dataset(variables, coords)
         ds = ds.assign_coords(**self._get_other_coords(raw_da))
         self.decoder = CFDecoder(ds)
         arr = ds.counts
         arr.psy.init_accessor(base=ds, decoder=self.decoder)
         self.data = arr
 
     def _get_other_coords(self, raw_da):
-        return {key: raw_da.coords[key]
-                for key in set(raw_da.coords).difference(raw_da.dims)}
+        return {
+            key: raw_da.coords[key]
+            for key in set(raw_da.coords).difference(raw_da.dims)
+        }
 
 
 class XYTickPlotter(Plotter):
-    """Plotter class for x- and y-ticks and x- and y- ticklabels
-    """
-    _rcparams_string = ['plotter.simple.']
+    """Plotter class for x- and y-ticks and x- and y- ticklabels"""
 
-    transpose = Transpose('transpose')
-    xticks = XTicks('xticks')
-    xticklabels = XTickLabels('xticklabels')
-    yticks = YTicks('yticks')
-    yticklabels = YTickLabels('yticklabels')
-    ticksize = TickSize('ticksize')
-    tickweight = TickWeight('tickweight')
-    xtickprops = XTickProps('xtickprops')
-    ytickprops = YTickProps('ytickprops')
-    xlabel = Xlabel('xlabel')
-    ylabel = Ylabel('ylabel')
-    labelsize = LabelSize('labelsize')
-    labelweight = LabelWeight('labelweight')
-    labelprops = LabelProps('labelprops')
-    xrotation = XRotation('xrotation')
-    yrotation = YRotation('yrotation')
+    _rcparams_string = ["plotter.simple."]
+
+    transpose = Transpose("transpose")
+    xticks = XTicks("xticks")
+    xticklabels = XTickLabels("xticklabels")
+    yticks = YTicks("yticks")
+    yticklabels = YTickLabels("yticklabels")
+    ticksize = TickSize("ticksize")
+    tickweight = TickWeight("tickweight")
+    xtickprops = XTickProps("xtickprops")
+    ytickprops = YTickProps("ytickprops")
+    xlabel = Xlabel("xlabel")
+    ylabel = Ylabel("ylabel")
+    labelsize = LabelSize("labelsize")
+    labelweight = LabelWeight("labelweight")
+    labelprops = LabelProps("labelprops")
+    xrotation = XRotation("xrotation")
+    yrotation = YRotation("yrotation")
 
 
 class Base2D(Plotter):
-    """Base plotter for 2-dimensional plots
-    """
+    """Base plotter for 2-dimensional plots"""
 
-    _rcparams_string = ['plotter.plot2d.']
+    _rcparams_string = ["plotter.plot2d."]
 
-    cmap = CMap('cmap')
-    bounds = Bounds('bounds')
-    extend = Extend('extend')
-    cbar = Cbar('cbar')
+    cmap = CMap("cmap")
+    bounds = Bounds("bounds")
+    extend = Extend("extend")
+    cbar = Cbar("cbar")
     plot = None
-    clabel = CLabel('clabel')
-    clabelsize = label_size(clabel, 'Colorbar label', dependencies=['clabel'])
-    clabelweight = label_weight(clabel, 'Colorbar label',
-                                dependencies=['clabel'])
-    cbarspacing = CbarSpacing('cbarspacing')
-    clabelprops = label_props(clabel, 'Colorbar label',
-                              dependencies=['clabel'])
-    cticks = CTicks('cticks')
-    cticklabels = CTickLabels('cticklabels')
-    cticksize = CTickSize('cticksize')
-    ctickweight = CTickWeight('ctickweight')
-    ctickprops = CTickProps('ctickprops')
-    mask_datagrid = MaskDataGrid('mask_datagrid')
-    datagrid = DataGrid('datagrid', index_in_list=0)
+    clabel = CLabel("clabel")
+    clabelsize = label_size(clabel, "Colorbar label", dependencies=["clabel"])
+    clabelweight = label_weight(
+        clabel, "Colorbar label", dependencies=["clabel"]
+    )
+    cbarspacing = CbarSpacing("cbarspacing")
+    clabelprops = label_props(
+        clabel, "Colorbar label", dependencies=["clabel"]
+    )
+    cticks = CTicks("cticks")
+    cticklabels = CTickLabels("cticklabels")
+    cticksize = CTickSize("cticksize")
+    ctickweight = CTickWeight("ctickweight")
+    ctickprops = CTickProps("ctickprops")
+    mask_datagrid = MaskDataGrid("mask_datagrid")
+    datagrid = DataGrid("datagrid", index_in_list=0)
 
 
 class SimplePlotterBase(BasePlotter, XYTickPlotter):
     """Base class for all simple plotters"""
 
     #: The number variables that one data array visualized by this plotter
     #: might have.
     allowed_vars = 1
 
     #: The number of allowed dimensions in the for the visualization. If
     #: the array is unstructured, one dimension will be subtracted
     allowed_dims = 1
 
-    transpose = Transpose('transpose')
-    axiscolor = AxisColor('axiscolor')
-    grid = Grid('grid')
-    color = LineColors('color')
-    xlim = Xlim('xlim')
-    ylim = Ylim('ylim')
-    sym_lims = SymmetricLimits('sym_lims')
-    legendlabels = LegendLabels('legendlabels')
-    legend = Legend('legend')
+    transpose = Transpose("transpose")
+    axiscolor = AxisColor("axiscolor")
+    grid = Grid("grid")
+    color = LineColors("color")
+    xlim = Xlim("xlim")
+    ylim = Ylim("ylim")
+    sym_lims = SymmetricLimits("sym_lims")
+    legendlabels = LegendLabels("legendlabels")
+    legend = Legend("legend")
 
     @classmethod
     @docstrings.dedent
     def check_data(cls, name, dims, is_unstructured=None):
         """
         A validation method for the data shape
 
@@ -5733,99 +6105,103 @@
         """
         if isinstance(name, six.string_types) or not is_iterable(name):
             name = [name]
             dims = [dims]
         N = len(name)
         if len(dims) != N:
             return [False] * N, [
-                'Number of provided names (%i) and dimensions '
-                '%(i) are not the same' % (N, len(dims))] * N
+                "Number of provided names (%i) and dimensions "
+                "(%i) are not the same" % (N, len(dims))
+            ] * N
         checks = [True] * N
-        messages = [''] * N
+        messages = [""] * N
         for i, (n, d) in enumerate(zip(name, dims)):
             if n != 0 and not n:
                 checks[i] = False
-                messages[i] = 'At least one variable name is required!'
-            elif ((not isstring(n) and is_iterable(n) and
-                   len(n) > cls.allowed_vars) and
-                  len(d) != (cls.allowed_dims - len(slist(n)))):
+                messages[i] = "At least one variable name is required!"
+            elif (
+                not isstring(n)
+                and is_iterable(n)
+                and len(n) > cls.allowed_vars
+            ) and len(d) != (cls.allowed_dims - len(slist(n))):
                 checks[i] = False
-                messages[i] = 'Only %i names are allowed per array!' % (
-                    cls.allowed_vars)
+                messages[i] = "Only %i names are allowed per array!" % (
+                    cls.allowed_vars
+                )
             elif len(d) != cls.allowed_dims:
                 checks[i] = False
-                messages[i] = 'Only %i-dimensional arrays are allowed!' % (
-                    cls.allowed_dims)
+                messages[i] = "Only %i-dimensional arrays are allowed!" % (
+                    cls.allowed_dims
+                )
         return checks, messages
 
 
 class LinePlotter(SimplePlotterBase):
-    """Plotter for simple one-dimensional line plots
-    """
+    """Plotter for simple one-dimensional line plots"""
 
-    _rcparams_string = ['plotter.line.']
+    _rcparams_string = ["plotter.line."]
 
     #: The number variables that one data array visualized by this plotter
     #: might have. We allow up to 3 variableswhere the second and third
     #: variable might be the errors (see the :attr:`error` formatoption)
     allowed_vars = 3
 
-    coord = AlternativeXCoord('coord')
-    marker = Marker('marker')
-    markersize = MarkerSize('markersize')
-    linewidth = LineWidth('linewidth')
-    plot = LinePlot('plot')
-    error = ErrorPlot('error')
-    erroralpha = ErrorAlpha('erroralpha')
+    coord = AlternativeXCoord("coord")
+    marker = Marker("marker")
+    markersize = MarkerSize("markersize")
+    linewidth = LineWidth("linewidth")
+    plot = LinePlot("plot")
+    error = ErrorPlot("error")
+    erroralpha = ErrorAlpha("erroralpha")
 
 
 class ViolinPlotter(SimplePlotterBase):
     """Plotter for making violin plots"""
 
-    _rcparams_string = ['plotter.violin.']
+    _rcparams_string = ["plotter.violin."]
 
-    plot = ViolinPlot('plot')
-    xlim = ViolinXlim('xlim')
-    ylim = ViolinYlim('ylim')
-    xticks = ViolinXTicks('xticks')
-    xticklabels = ViolinXTickLabels('xticklabels')
-    yticks = ViolinYTicks('yticks')
-    yticklabels = ViolinYTickLabels('yticklabels')
+    plot = ViolinPlot("plot")
+    xlim = ViolinXlim("xlim")
+    ylim = ViolinYlim("ylim")
+    xticks = ViolinXTicks("xticks")
+    xticklabels = ViolinXTickLabels("xticklabels")
+    yticks = ViolinYTicks("yticks")
+    yticklabels = ViolinYTickLabels("yticklabels")
 
 
 class BarPlotter(SimplePlotterBase):
     """Plotter for making bar plots"""
 
-    _rcparams_string = ['plotter.bar.']
+    _rcparams_string = ["plotter.bar."]
 
-    coord = AlternativeXCoord('coord')
-    widths = BarWidths('widths')
-    alpha = BarAlpha('alpha')
-    categorical = CategoricalBars('categorical')
-    plot = BarPlot('plot')
-    xlim = BarXlim('xlim')
-    ylim = BarYlim('ylim')
-    xticks = BarXTicks('xticks')
-    yticks = BarYTicks('yticks')
-    xticklabels = BarXTickLabels('xticklabels')
-    yticklabels = BarYTickLabels('yticklabels')
-    xlabel = BarXlabel('xlabel')
-    ylabel = BarYlabel('ylabel')
+    coord = AlternativeXCoord("coord")
+    widths = BarWidths("widths")
+    alpha = BarAlpha("alpha")
+    categorical = CategoricalBars("categorical")
+    plot = BarPlot("plot")
+    xlim = BarXlim("xlim")
+    ylim = BarYlim("ylim")
+    xticks = BarXTicks("xticks")
+    yticks = BarYTicks("yticks")
+    xticklabels = BarXTickLabels("xticklabels")
+    yticklabels = BarYTickLabels("yticklabels")
+    xlabel = BarXlabel("xlabel")
+    ylabel = BarYlabel("ylabel")
 
 
 class Simple2DBase(Base2D):
     """Base class for :class:`Simple2DPlotter` and
     :class:`psyplot.plotter.maps.FieldPlotter` that defines the data
     management"""
 
     #: The number of allowed dimensions in the for the visualization. If
     #: the array is unstructured, one dimension will be subtracted
     allowed_dims = 2
 
-    miss_color = MissColor('miss_color', index_in_list=0)
+    miss_color = MissColor("miss_color", index_in_list=0)
 
     @classmethod
     @docstrings.dedent
     def check_data(cls, name, dims, is_unstructured):
         """
         A validation method for the data shape
 
@@ -5845,112 +6221,123 @@
         if isinstance(name, six.string_types) or not is_iterable(name):
             name = [name]
             dims = [dims]
             is_unstructured = [is_unstructured]
         N = len(name)
         if N != 1:
             return [False] * N, [
-                'Number of provided names (%i) must equal 1!' % (N)] * N
+                "Number of provided names (%i) must equal 1!" % (N)
+            ] * N
         elif len(dims) != 1:
             return [False], [
-                'Number of provided dimension lists (%i) must equal 1!' % (
-                    len(dims))]
+                "Number of provided dimension lists (%i) must equal 1!"
+                % (len(dims))
+            ]
         elif len(is_unstructured) != 1:
             return [False], [
-                ('Number of provided unstructured information (%i) must '
-                 'equal 1!') % (len(is_unstructured))]
+                (
+                    "Number of provided unstructured information (%i) must "
+                    "equal 1!"
+                )
+                % (len(is_unstructured))
+            ]
         if name[0] != 0 and not name[0]:
-            return [False], ['At least one variable name must be provided!']
+            return [False], ["At least one variable name must be provided!"]
         # unstructured arrays have only 1 dimension
         dimlen = cls.allowed_dims
         if is_unstructured[0]:
             dimlen -= 1
         # Check that the array is two-dimensional
         #
         # if more than one array name is provided, the dimensions should be
         # one les than dimlen to have a 2D array
-        if (not isstring(name[0]) and not is_iterable(name[0])
-                and len(name[0]) != 1 and len(dims[0]) != dimlen - 1):
-            return [False], ['Only one name is allowed per array!']
+        if (
+            not isstring(name[0])
+            and not is_iterable(name[0])
+            and len(name[0]) != 1
+            and len(dims[0]) != dimlen - 1
+        ):
+            return [False], ["Only one name is allowed per array!"]
         # otherwise the number of dimensions must equal dimlen
         if len(dims[0]) != dimlen:
             return [False], [
-                'An array with dimension %i is required, not %i' % (
-                    dimlen, len(dims[0]))]
-        return [True], ['']
+                "An array with dimension %i is required, not %i"
+                % (dimlen, len(dims[0]))
+            ]
+        return [True], [""]
 
     def _set_data(self, *args, **kwargs):
         Plotter._set_data(self, *args, **kwargs)
         if isinstance(self.data, InteractiveList):
             data = self.data[0]
         else:
             data = self.data
         ndims = self.allowed_dims
         if data.psy.decoder.is_unstructured(data):
             ndims -= 1
         if data.ndim != ndims:
-            raise ValueError(f"Can only plot {self.allowed_dims}-dimensional "
-                             "data!")
+            raise ValueError(
+                f"Can only plot {self.allowed_dims}-dimensional " "data!"
+            )
 
 
 class Simple2DPlotter(Simple2DBase, SimplePlotterBase):
     """Plotter for visualizing 2-dimensional data.
 
     See Also
     --------
     psyplot.plotter.maps.FieldPlotter"""
 
-    transpose = Transpose('transpose')
-    interp_bounds = InterpolateBounds('interp_bounds')
-    plot = SimplePlot2D('plot')
-    xticks = XTicks2D('xticks')
-    yticks = YTicks2D('yticks')
-    xlim = Xlim2D('xlim')
-    ylim = Ylim2D('ylim')
-    levels = ContourLevels('levels', cbounds='bounds')
+    transpose = Transpose("transpose")
+    interp_bounds = InterpolateBounds("interp_bounds")
+    plot = SimplePlot2D("plot")
+    xticks = XTicks2D("xticks")
+    yticks = YTicks2D("yticks")
+    xlim = Xlim2D("xlim")
+    ylim = Ylim2D("ylim")
+    levels = ContourLevels("levels", cbounds="bounds")
     legend = None
     legendlabels = None
     color = None  # no need for this formatoption
 
 
 class DensityPlotter(Simple2DPlotter):
     """A plotter to visualize the density of points in a 2-dimensional grid"""
 
     allowed_vars = 1
 
     allowed_dims = 1
 
-    _rcparams_string = ['plotter.density.']
+    _rcparams_string = ["plotter.density."]
 
-    coord = AlternativeXCoord('coord')
-    xrange = Hist2DXRange('xrange')
-    yrange = Hist2DYRange('yrange')
-    precision = DataPrecision('precision')
-    bins = HistBins('bins')
-    normed = NormedHist2D('normed')
-    density = PointDensity('density')
+    coord = AlternativeXCoord("coord")
+    xrange = Hist2DXRange("xrange")
+    yrange = Hist2DYRange("yrange")
+    precision = DataPrecision("precision")
+    bins = HistBins("bins")
+    normed = NormedHist2D("normed")
+    density = PointDensity("density")
 
 
 class BaseVectorPlotter(Base2D):
-    """Base plotter for vector plots
-    """
+    """Base plotter for vector plots"""
 
     _rcparams_string = ["plotter.vector."]
 
     allowed_dims = 3
 
-    arrowsize = ArrowSize('arrowsize')
-    arrowstyle = ArrowStyle('arrowstyle')
-    density = Density('density')
-    color = VectorColor('color')
-    linewidth = VectorLineWidth('linewidth')
-    cbar = VectorCbar('cbar')
-    bounds = VectorBounds('bounds')
-    cticks = VectorCTicks('cticks')
-    datagrid = VectorDataGrid('datagrid')
+    arrowsize = ArrowSize("arrowsize")
+    arrowstyle = ArrowStyle("arrowstyle")
+    density = Density("density")
+    color = VectorColor("color")
+    linewidth = VectorLineWidth("linewidth")
+    cbar = VectorCbar("cbar")
+    bounds = VectorBounds("bounds")
+    cticks = VectorCTicks("cticks")
+    datagrid = VectorDataGrid("datagrid")
 
     @classmethod
     @docstrings.dedent
     def check_data(cls, name, dims, is_unstructured):
         """
         A validation method for the data shape
 
@@ -5972,127 +6359,159 @@
         if isinstance(name, six.string_types) or not is_iterable(name):
             name = [name]
             dims = [dims]
             is_unstructured = [is_unstructured]
         N = len(name)
         if N != 1:
             return [False] * N, [
-                'Number of provided names (%i) must equal 1!' % (N)] * N
+                "Number of provided names (%i) must equal 1!" % (N)
+            ] * N
         elif len(dims) != 1:
             return [False], [
-                'Number of provided dimension lists (%i) must equal 1!' % (
-                    len(dims))]
+                "Number of provided dimension lists (%i) must equal 1!"
+                % (len(dims))
+            ]
         elif len(is_unstructured) != 1:
             return [False], [
-                ('Number of provided unstructured information (%i) must '
-                 'equal 1!') % (len(is_unstructured))]
+                (
+                    "Number of provided unstructured information (%i) must "
+                    "equal 1!"
+                )
+                % (len(is_unstructured))
+            ]
         if name[0] != 0 and not name[0]:
-            return [False], ['Two variable names must be provided!']
+            return [False], ["Two variable names must be provided!"]
         # unstructured arrays have only 1 dimension
         dimlen = 1 if is_unstructured[0] else 2
         # Check that the array is two-dimensional
         #
         # if more than one array name is provided, the dimensions should be
         # one les than dimlen to have a 2D array
-        if (((isstring(name[0] or not is_iterable(name[0])) or
-              len(name[0]) == 1) and len(dims[0]) != dimlen + 1) or
-                len(name[0]) > 2):
+        if (
+            (
+                isstring(name[0] or not is_iterable(name[0]))
+                or len(name[0]) == 1
+            )
+            and len(dims[0]) != dimlen + 1
+        ) or len(name[0]) > 2:
             return [False], [
-                ('Two variables (one for x- and one for y-direction) are '
-                 'required!')]
-        elif ((isstring(name[0]) or len(name[0]) == 1) and
-              len(dims[0]) == dimlen + 1):
+                (
+                    "Two variables (one for x- and one for y-direction) are "
+                    "required!"
+                )
+            ]
+        elif (isstring(name[0]) or len(name[0]) == 1) and len(
+            dims[0]
+        ) == dimlen + 1:
             dimlen += 1
         # otherwise the number of dimensions must equal dimlen
         if len(dims[0]) != dimlen:
             return [False], [
-                'An array with dimension %i is required, not %i' % (
-                    dimlen, len(dims[0]))]
-        return [True], ['']
+                "An array with dimension %i is required, not %i"
+                % (dimlen, len(dims[0]))
+            ]
+        return [True], [""]
 
     def _set_data(self, *args, **kwargs):
         Plotter._set_data(self, *args, **kwargs)
         if isinstance(self.data, InteractiveList):
             data = self.data[0]
         else:
             data = self.data
         ndims = self.allowed_dims
         if data.psy.decoder.is_unstructured(data):
             ndims -= 1
         if data.ndim != ndims:
-            raise ValueError(f"Can only plot {self.allowed_dims}-dimensional "
-                             "data!")
+            raise ValueError(
+                f"Can only plot {self.allowed_dims}-dimensional " "data!"
+            )
 
 
 class SimpleVectorPlotter(BaseVectorPlotter, SimplePlotterBase):
     """Plotter for visualizing 2-dimensional vector data
 
     See Also
     --------
     psyplot.plotter.maps.VectorPlotter"""
 
-    plot = SimpleVectorPlot('plot')
-    xticks = XTicks2D('xticks')
-    yticks = YTicks2D('yticks')
-    xlim = Xlim2D('xlim')
-    ylim = Ylim2D('ylim')
+    plot = SimpleVectorPlot("plot")
+    xticks = XTicks2D("xticks")
+    yticks = YTicks2D("yticks")
+    xlim = Xlim2D("xlim")
+    ylim = Ylim2D("ylim")
     legend = None
     legendlabels = None
 
 
 class ScalarCombinedBase(Plotter):
     """Base plotter for combined 2-dimensional scalar field with any other
     plotter"""
 
     _rcparams_string = ["plotter.combinedsimple."]
 
     # scalar plot formatoptions
-    cbar = Cbar('cbar', other_cbars=['vcbar'])
-    cticks = CTicks('cticks')
-    bounds = Bounds('bounds', index_in_list=0)
+    cbar = Cbar("cbar", other_cbars=["vcbar"])
+    cticks = CTicks("cticks")
+    bounds = Bounds("bounds", index_in_list=0)
 
     # make sure that masking options only affect the scalar field
-    maskless = MaskLess('maskless', index_in_list=0)
-    maskleq = MaskLeq('maskleq', index_in_list=0)
-    maskgreater = MaskGreater('maskgreater', index_in_list=0)
-    maskgeq = MaskGeq('maskgeq', index_in_list=0)
-    maskbetween = MaskBetween('maskbetween', index_in_list=0)
+    maskless = MaskLess("maskless", index_in_list=0)
+    maskleq = MaskLeq("maskleq", index_in_list=0)
+    maskgreater = MaskGreater("maskgreater", index_in_list=0)
+    maskgeq = MaskGeq("maskgeq", index_in_list=0)
+    maskbetween = MaskBetween("maskbetween", index_in_list=0)
 
 
 class CombinedBase(ScalarCombinedBase):
     """Base plotter for combined 2-dimensional scalar and vector plot"""
 
     # vector plot formatoptions
-    color = VectorColor('color', plot='vplot', cmap='vcmap', bounds='vbounds',
-                        index_in_list=1)
-    linewidth = VectorLineWidth('linewidth', plot='vplot', index_in_list=1)
-    arrowsize = ArrowSize('arrowsize', plot='vplot', index_in_list=1)
-    arrowstyle = ArrowStyle('arrowstyle', plot='vplot', index_in_list=1)
-    vcbar = VectorCbar('vcbar', plot='vplot', cmap='vcmap', bounds='vbounds',
-                       cbarspacing='vcbarspacing', other_cbars=['cbar'],
-                       index_in_list=1)
-    vcbarspacing = CbarSpacing('vcbarspacing', cbar='vcbar', index_in_list=1)
-    vclabel = VCLabel('vclabel', plot='vplot', cbar='vcbar', index_in_list=1)
-    vclabelsize = label_size(vclabel, 'Vector colorbar label',
-                             dependencies=['vclabel'])
-    vclabelweight = label_weight(vclabel, 'Vector colorbar label',
-                                 dependencies=['vclabel'])
-    vclabelprops = label_props(vclabel, 'Vector colorbar label',
-                               dependencies=['vclabel'])
-    vcmap = CMap('vcmap', index_in_list=1, bounds='vbounds', cbar='vcbar')
-    vbounds = VectorBounds('vbounds', index_in_list=1, cmap='vcmap',
-                           cbar='vcbar')
-    vcticks = VectorCTicks('vcticks', cbar='vcbar', plot='vplot',
-                           bounds='vbounds', index_in_list=1)
-    vcticklabels = CTickLabels('vcticklabels', cbar='vcbar', index_in_list=1)
-    vcticksize = CTickSize('vcticksize', cbar='vcbar', index_in_list=1,
-                           ctickprops='vctickprops')
-    vctickweight = CTickWeight('vctickweight', cbar='vcbar', index_in_list=1)
-    vctickprops = CTickProps('vctickprops', cbar='vcbar',
-                             index_in_list=1)
+    color = VectorColor(
+        "color", plot="vplot", cmap="vcmap", bounds="vbounds", index_in_list=1
+    )
+    linewidth = VectorLineWidth("linewidth", plot="vplot", index_in_list=1)
+    arrowsize = ArrowSize("arrowsize", plot="vplot", index_in_list=1)
+    arrowstyle = ArrowStyle("arrowstyle", plot="vplot", index_in_list=1)
+    vcbar = VectorCbar(
+        "vcbar",
+        plot="vplot",
+        cmap="vcmap",
+        bounds="vbounds",
+        cbarspacing="vcbarspacing",
+        other_cbars=["cbar"],
+        index_in_list=1,
+    )
+    vcbarspacing = CbarSpacing("vcbarspacing", cbar="vcbar", index_in_list=1)
+    vclabel = VCLabel("vclabel", plot="vplot", cbar="vcbar", index_in_list=1)
+    vclabelsize = label_size(
+        vclabel, "Vector colorbar label", dependencies=["vclabel"]
+    )
+    vclabelweight = label_weight(
+        vclabel, "Vector colorbar label", dependencies=["vclabel"]
+    )
+    vclabelprops = label_props(
+        vclabel, "Vector colorbar label", dependencies=["vclabel"]
+    )
+    vcmap = CMap("vcmap", index_in_list=1, bounds="vbounds", cbar="vcbar")
+    vbounds = VectorBounds(
+        "vbounds", index_in_list=1, cmap="vcmap", cbar="vcbar"
+    )
+    vcticks = VectorCTicks(
+        "vcticks",
+        cbar="vcbar",
+        plot="vplot",
+        bounds="vbounds",
+        index_in_list=1,
+    )
+    vcticklabels = CTickLabels("vcticklabels", cbar="vcbar", index_in_list=1)
+    vcticksize = CTickSize(
+        "vcticksize", cbar="vcbar", index_in_list=1, ctickprops="vctickprops"
+    )
+    vctickweight = CTickWeight("vctickweight", cbar="vcbar", index_in_list=1)
+    vctickprops = CTickProps("vctickprops", cbar="vcbar", index_in_list=1)
 
     @classmethod
     @docstrings.dedent
     def check_data(cls, name, dims, is_unstructured):
         """
         A validation method for the data shape
 
@@ -6110,65 +6529,72 @@
         -------
         %(Plotter.check_data.returns)s
         """
         if isinstance(name, six.string_types) or not is_iterable(name):
             name = [name]
             dims = [dims]
             is_unstructured = [is_unstructured]
-        msg = ('Two arrays are required (one for the scalar and '
-               'one for the vector field)')
+        msg = (
+            "Two arrays are required (one for the scalar and "
+            "one for the vector field)"
+        )
         if len(name) < 2:
             return [None], [msg]
         elif len(name) > 2:
             return [False], [msg]
-        valid1, msg1 = Simple2DBase.check_data(name[:1], dims[0:1],
-                                               is_unstructured[:1])
-        valid2, msg2 = BaseVectorPlotter.check_data(name[1:], dims[1:],
-                                                    is_unstructured[1:])
+        valid1, msg1 = Simple2DBase.check_data(
+            name[:1], dims[0:1], is_unstructured[:1]
+        )
+        valid2, msg2 = BaseVectorPlotter.check_data(
+            name[1:], dims[1:], is_unstructured[1:]
+        )
         return valid1 + valid2, msg1 + msg2
 
     def _set_data(self, *args, **kwargs):
         super(CombinedBase, self)._set_data(*args, **kwargs)
         # implement 2 simple checks to make sure that we get the right data
         if not isinstance(self.plot_data, InteractiveList):
             raise ValueError(
                 "Combined plots must be lists of one scalar field and a"
-                "vector field. Got one %s instead" % str(type(
-                    self.plot_data)))
+                "vector field. Got one %s instead" % str(type(self.plot_data))
+            )
         elif len(self.plot_data) < 2:
             raise ValueError(
                 "Combined plots must be lists of one scalar field and a"
-                "vector field. Got a list of length %i instead!" % len(
-                    self.plot_data))
+                "vector field. Got a list of length %i instead!"
+                % len(self.plot_data)
+            )
 
 
-class CombinedSimplePlotter(CombinedBase, Simple2DPlotter,
-                            SimpleVectorPlotter):
+class CombinedSimplePlotter(
+    CombinedBase, Simple2DPlotter, SimpleVectorPlotter
+):
     """Combined 2D plotter and vector plotter
 
     See Also
     --------
     psyplot.plotter.maps.CombinedPlotter: for visualizing the data on a map"""
-    plot = Plot2D('plot', index_in_list=0)
-    vplot = CombinedVectorPlot('vplot', index_in_list=1, cmap='vcmap',
-                               bounds='vbounds')
-    density = Density('density', plot='vplot', index_in_list=1)
+
+    plot = Plot2D("plot", index_in_list=0)
+    vplot = CombinedVectorPlot(
+        "vplot", index_in_list=1, cmap="vcmap", bounds="vbounds"
+    )
+    density = Density("density", plot="vplot", index_in_list=1)
 
 
 class FldmeanPlotter(LinePlotter):
-
     _rcparams_string = ["plotter.fldmean."]
 
     allowed_dims = 3
 
-    err_calc = ErrorCalculator('err_calc')
-    mean = MeanCalculator('mean')
+    err_calc = ErrorCalculator("err_calc")
+    mean = MeanCalculator("mean")
 
     # We reimplement the masking formatoption to make sure, that they are
     # called after the mean calculation
-    maskgeq = MaskGeq('maskgeq', additional_children=['err_calc'])
-    maskleq = MaskLeq('maskleq', additional_children=['err_calc'])
-    maskgreater = MaskGreater('maskgreater', additional_children=['err_calc'])
-    maskless = MaskLess('maskless', additional_children=['err_calc'])
-    maskbetween = MaskBetween('maskbetween', additional_children=['err_calc'])
-    mask = Mask('mask', additional_children=['err_calc'])
-    coord = AlternativeXCoordPost('coord', additional_children=['err_calc'])
+    maskgeq = MaskGeq("maskgeq", additional_children=["err_calc"])
+    maskleq = MaskLeq("maskleq", additional_children=["err_calc"])
+    maskgreater = MaskGreater("maskgreater", additional_children=["err_calc"])
+    maskless = MaskLess("maskless", additional_children=["err_calc"])
+    maskbetween = MaskBetween("maskbetween", additional_children=["err_calc"])
+    mask = Mask("mask", additional_children=["err_calc"])
+    coord = AlternativeXCoordPost("coord", additional_children=["err_calc"])
```

### Comparing `psy-simple-1.4.1/psy_simple/plugin.py` & `psy-simple-1.5.0/psy_simple/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,135 @@
 """psy-simple psyplot plugin
 
 This module defines the rcParams for the psy-simple plugin.
 """
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-simple and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum Hereon
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
+
+import dataclasses
+import enum
 import re
+from itertools import repeat
+from warnings import warn
+
 import matplotlib as mpl
-import dataclasses
 import numpy as np
-import enum
+import six
+import xarray as xr
 from matplotlib.patches import ArrowStyle
-from warnings import warn
-from itertools import repeat
-from psyplot.config.rcsetup import (
-    RcParams, safe_list, SubDict, validate_dict, validate_stringlist,
-    validate_stringset)
 from matplotlib.rcsetup import (
-    validate_bool, validate_color, validate_fontsize,
-    ValidateInStrings, validate_int, validate_colorlist
+    ValidateInStrings,
+    validate_bool,
+    validate_color,
+    validate_colorlist,
+    validate_fontsize,
+    validate_int,
+)
+from psyplot.config.rcsetup import (
+    RcParams,
+    SubDict,
+    safe_list,
+    validate_dict,
+    validate_stringlist,
+    validate_stringset,
 )
+
 from psy_simple import __version__ as plugin_version
-import xarray as xr
 
 
 def get_versions(requirements=True):
-    return {'version': plugin_version}
+    return {"version": plugin_version}
 
 
 def patch_prior_1_0(plotter_d, versions):
     """Patch psy_simple plotters for versions smaller than 1.0
 
     Before psyplot 1.0.0, the plotters in the psy_simple package where part of
     the psyplot.plotter.simple module. This has to be corrected"""
-    plotter_d['cls'] = ('psy_simple.plotters', plotter_d['cls'][1])
+    plotter_d["cls"] = ("psy_simple.plotters", plotter_d["cls"][1])
 
 
 #: patches to apply when loading a project
 patches = {
-    ('psyplot.plotter.simple', 'LinRegPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'DensityRegPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'ViolinPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'Simple2DPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'SimpleVectorPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'BarPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'CombinedSimplePlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'DensityPlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'LinePlotter'): patch_prior_1_0,
-    ('psyplot.plotter.simple', 'SimplePlotterBase'): patch_prior_1_0,
-    }
-
-
-bound_strings = ['data', 'mid', 'rounded', 'roundedsym', 'minmax', 'sym',
-                 'log', 'symlog']
+    ("psyplot.plotter.simple", "LinRegPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "DensityRegPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "ViolinPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "Simple2DPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "SimpleVectorPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "BarPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "CombinedSimplePlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "DensityPlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "LinePlotter"): patch_prior_1_0,
+    ("psyplot.plotter.simple", "SimplePlotterBase"): patch_prior_1_0,
+}
+
+
+bound_strings = [
+    "data",
+    "mid",
+    "rounded",
+    "roundedsym",
+    "minmax",
+    "sym",
+    "log",
+    "symlog",
+]
 
-tick_strings = bound_strings + ['hour', 'day', 'week', 'month', 'monthend',
-                                'monthbegin', 'year', 'yearend', 'yearbegin']
+tick_strings = bound_strings + [
+    "hour",
+    "day",
+    "week",
+    "month",
+    "monthend",
+    "monthbegin",
+    "year",
+    "yearend",
+    "yearbegin",
+]
 
 
 class strEnum(str, enum.Enum):
     pass
 
 
 BoundsMethod = strEnum(
-    'BoundsMethod', zip(bound_strings, bound_strings), module=__name__)
+    "BoundsMethod", zip(bound_strings, bound_strings), module=__name__
+)
 
 
-cticks_strings = bound_strings + ['bounds', 'midbounds']
+cticks_strings = bound_strings + ["bounds", "midbounds"]
 
 
 CTicksMethod = strEnum(
-    'CTicksMethod', zip(cticks_strings, cticks_strings), module=__name__)
+    "CTicksMethod", zip(cticks_strings, cticks_strings), module=__name__
+)
 
 TicksMethod = strEnum(
-    'TicksMethod', zip(tick_strings, tick_strings), module=__name__)
+    "TicksMethod", zip(tick_strings, tick_strings), module=__name__
+)
 
 
 @dataclasses.dataclass
 class BoundsType:
     method: BoundsMethod
     N: int = None
     percmin: float = 0
     percmax: float = 100
     vmin: float = None
     vmax: float = None
 
     def __post_init__(self):
         for field, val in zip(dataclasses.fields(self), self):
-            if val is not None or field.name == 'method':
+            if val is not None or field.name == "method":
                 val = field.type(val)
                 setattr(self, field.name, val)
 
     def __iter__(self):
         return iter(dataclasses.astuple(self))
 
 
@@ -134,22 +150,24 @@
     ----------
     ``*funcs``
         Validation functions to test
 
     Returns
     -------
     function"""
+
     def validate(value):
         exc = None
         for func in funcs:
             try:
                 return func(value)
             except (ValueError, TypeError) as e:
                 exc = e
         raise exc
+
     return validate
 
 
 # -----------------------------------------------------------------------------
 # ------------------------- validation functions ------------------------------
 # -----------------------------------------------------------------------------
 
@@ -195,69 +213,83 @@
     Parameters
     ----------
     value: see :attr:`psyplot.plotter.labelplotter.text`
 
     Raises
     ------
     ValueError"""
-    possible_transform = ['axes', 'fig', 'data']
-    validate_transform = ValidateInStrings('transform', possible_transform,
-                                           True)
-    tests = [validate_float, validate_float, validate_str,
-             validate_transform, dict]
+    possible_transform = ["axes", "fig", "data"]
+    validate_transform = ValidateInStrings(
+        "transform", possible_transform, True
+    )
+    tests = [
+        validate_float,
+        validate_float,
+        validate_str,
+        validate_transform,
+        dict,
+    ]
     if isinstance(value, six.string_types):
-        xpos, ypos = rcParams['texts.default_position']
-        return [(xpos, ypos, value, 'axes', {'ha': 'right'})]
+        xpos, ypos = rcParams["texts.default_position"]
+        return [(xpos, ypos, value, "axes", {"ha": "right"})]
     elif isinstance(value, tuple):
         value = [value]
     try:
         value = list(value)[:]
     except TypeError:
         raise ValueError("Value must be string or list of tuples!")
     for i, val in enumerate(value):
         try:
             val = tuple(val)
         except TypeError:
             raise ValueError(
                 "Text must be an iterable of the form "
-                "(x, y, s[, trans, params])!")
+                "(x, y, s[, trans, params])!"
+            )
         if len(val) < 3:
             raise ValueError(
                 "Text tuple must at least be like [x, y, s], with floats x, "
-                "y and string s!")
+                "y and string s!"
+            )
         elif len(val) == 3 or isinstance(val[3], dict):
             val = list(val)
-            val.insert(3, 'data')
+            val.insert(3, "data")
             if len(val) == 4:
                 val += [{}]
             val = tuple(val)
         if len(val) > 5:
             raise ValueError(
                 "Text tuple must not be longer then length 5. It can be "
-                "like (x, y, s[, trans, params])!")
+                "like (x, y, s[, trans, params])!"
+            )
         value[i] = (validate(x) for validate, x in zip(tests, val))
     return value
 
 
 def validate_fontweight(value):
     if value is None:
         return None
     elif isinstance(value, six.string_types):
         return six.text_type(value)
-    elif mpl.__version__ >= '1.5':
+    elif mpl.__version__ >= "1.5":
         return validate_float(value)
     raise ValueError("Font weights must be None or a string!")
 
 
 def validate_limits(value):
     if value is None or isinstance(value, six.string_types):
         return (value, value)
     if not len(value) == 2:
         raise ValueError("Limits must have length 2!")
-    return tuple(value)
+    ret = tuple(value)
+    if all(isinstance(v, float) for v in ret):
+        # make sure, we do not have numpy floats in here because this can
+        # easily break the diff of the formatoption
+        ret = tuple(float(v) for v in ret)
+    return ret
 
 
 def validate_none(b):
     """Validate that None is given
 
     Parameters
     ----------
@@ -269,15 +301,15 @@
     None
 
     Raises
     ------
     ValueError"""
     if isinstance(b, six.string_types):
         b = b.lower()
-    if b is None or b == 'none':
+    if b is None or b == "none":
         return None
     else:
         raise ValueError('Could not convert "%s" to None' % b)
 
 
 validate_bool_maybe_none = try_and_error(validate_none, validate_bool)
 
@@ -294,23 +326,23 @@
     -------
     dict
 
     Raises
     ------
     ValueError"""
     validate = try_and_error(validate_none, validate_color)
-    possible_keys = {'right', 'left', 'top', 'bottom'}
+    possible_keys = {"right", "left", "top", "bottom"}
     try:
         value = dict(value)
         false_keys = set(value) - possible_keys
         if false_keys:
-            raise ValueError("Wrong keys (%s)!" % (', '.join(false_keys)))
+            raise ValueError("Wrong keys (%s)!" % (", ".join(false_keys)))
         for key, val in value.items():
             value[key] = validate(val)
-    except:
+    except Exception:
         value = dict(zip(possible_keys, repeat(validate(value))))
     return value
 
 
 def validate_dataarray(val):
     if not isinstance(val, xr.DataArray):
         raise ValueError("Require xarray.DataArray, not %r" % type(val))
@@ -323,18 +355,18 @@
     if val is None:
         return None
     else:
         return safe_list(val)
 
 
 def validate_alpha(val):
-    '''Validate an alpha value between 0 and 1'''
+    """Validate an alpha value between 0 and 1"""
     val = validate_float(val)
     if val < 0 or val > 1:
-        raise ValueError('Alpha values must lay between 0 and 1!')
+        raise ValueError("Alpha values must lay between 0 and 1!")
     return val
 
 
 def validate_iter(value):
     """Validate that the given value is an iterable"""
     try:
         iter(value)
@@ -356,27 +388,26 @@
     -------
     list
         list of strings with possible colorbar positions
 
     Raises
     ------
     ValueError"""
-    patt = 'sh|sv|fl|fr|ft|fb|b|r'
+    patt = "sh|sv|fl|fr|ft|fb|b|r"
     if value is True:
-        value = {'b'}
+        value = {"b"}
     elif not value:
         value = set()
     elif isinstance(value, six.string_types):
-        for s in re.finditer('[^%s]+' % patt, value):
+        for s in re.finditer("[^%s]+" % patt, value):
             warn("Unknown colorbar position %s!" % s.group(), RuntimeWarning)
         value = set(re.findall(patt, value))
     else:
         value = validate_stringset(value)
-        for s in (s for s in value
-                  if not re.match(patt, s)):
+        for s in (s for s in value if not re.match(patt, s)):
             warn("Unknown colorbar position %s!" % s)
             value.remove(s)
     return value
 
 
 def validate_cmap(val):
     """Validate a colormap
@@ -389,20 +420,20 @@
     -------
     str or :class:`mpl.colors.Colormap`
 
     Raises
     ------
     ValueError"""
     from matplotlib.colors import Colormap
+
     try:
         return validate_str(val)
     except ValueError:
         if not isinstance(val, Colormap):
-            raise ValueError(
-                "Could not find a valid colormap!")
+            raise ValueError("Could not find a valid colormap!")
         return val
 
 
 def validate_cmaps(cmaps):
     """Validate a dictionary of color lists
 
     Parameters
@@ -417,53 +448,62 @@
 
     Notes
     -----
     For all items (listname, list) in `cmaps`, the reversed list is
     automatically inserted with the ``listname + '_r'`` key."""
     cmaps = {validate_str(key): validate_colorlist(val) for key, val in cmaps}
     for key, val in six.iteritems(cmaps):
-        cmaps.setdefault(key + '_r', val[::-1])
+        cmaps.setdefault(key + "_r", val[::-1])
     return cmaps
 
 
 def validate_sym_lims(val):
-    validator = try_and_error(validate_none, ValidateInStrings(
-        'sym_links', ['min', 'max'], True))
+    validator = try_and_error(
+        validate_none, ValidateInStrings("sym_links", ["min", "max"], True)
+    )
     val = safe_list(val)
     if len(val) != 2:
         val = val + val
     if not len(val) == 2:
-        raise ValueError("Need two values for the symmetric limits, not %i" % (
-            len(val)))
+        raise ValueError(
+            "Need two values for the symmetric limits, not %i" % (len(val))
+        )
     return list(map(validator, val))
 
 
 valid_legend_locs = [
     "best",
-    "upper right", "upper left", "lower left", "lower right", "right",
-    "center left", "center right", "lower center", "upper center",
-    "center"
+    "upper right",
+    "upper left",
+    "lower left",
+    "lower right",
+    "right",
+    "center left",
+    "center right",
+    "lower center",
+    "upper center",
+    "center",
 ]
 
 validate_legend_loc = ValidateInStrings("legend_loc", valid_legend_locs, True)
 
 
 def validate_legend(value):
     if isinstance(value, dict):
         return value
     try:
-        return {'loc': validate_int(value)}
-    except (ValueError, TypeError) as e:
+        return {"loc": validate_int(value)}
+    except (ValueError, TypeError):
         pass
     try:
-        return {'loc': validate_legend_loc(value)}
-    except (ValueError, TypeError) as e:
+        return {"loc": validate_legend_loc(value)}
+    except (ValueError, TypeError):
         pass
     value = validate_bool(value)
-    return {'loc': 'best' if value else False}
+    return {"loc": "best" if value else False}
 
 
 def validate_lineplot(value):
     """Validate the value for the LinePlotter.plot formatoption
 
     Parameters
     ----------
@@ -477,28 +517,29 @@
         value = list(value)
         for i, v in enumerate(value):
             if v is None:
                 pass
             elif isinstance(v, six.string_types):
                 value[i] = six.text_type(v)
             else:
-                raise ValueError('Expected None or string, found %s' % (v, ))
+                raise ValueError("Expected None or string, found %s" % (v,))
     return value
 
 
-validate_ticklabels = try_and_error(validate_none, validate_str,
-                                    validate_stringlist)
+validate_ticklabels = try_and_error(
+    validate_none, validate_str, validate_stringlist
+)
 
-validate_extend = ValidateInStrings('extend',
-                                    ['neither', 'both', 'min', 'max'])
+validate_extend = ValidateInStrings(
+    "extend", ["neither", "both", "min", "max"]
+)
 
 
 class ValidateList(object):
-    """Validate a list of the specified `dtype`
-    """
+    """Validate a list of the specified `dtype`"""
 
     def __init__(self, dtype=None, length=None, listtype=list):
         """
         Parameters
         ----------
         dtype: object
             A datatype (e.g. :class:`float`) that shall be used for the
@@ -509,15 +550,15 @@
             The type to use for creating the list. Should accept any iterable
         """
         #: data type (e.g. :class:`float`) used for the conversion
         self.dtype = dtype
         self.length = length
         self.listtype = list
 
-    def __call__(self, l):
+    def __call__(self, sequence):
         """Validate whether `l` is a list with contents of :attr:`dtype`
 
         Parameters
         ----------
         l: list-like
 
         Returns
@@ -526,84 +567,92 @@
             list with values of dtype :attr:`dtype`
 
         Raises
         ------
         ValueError"""
         try:
             if self.dtype is None:
-                validated = self.listtype(l)
+                validated = self.listtype(sequence)
             else:
                 try:
                     len(self.dtype)
                 except TypeError:
-                    validated = self.listtype(map(self.dtype, l))
+                    validated = self.listtype(map(self.dtype, sequence))
                 else:
                     validated = self.listtype()
-                    for val in l:
+                    for val in sequence:
                         valid = False
                         for dtype in self.dtype:
                             try:
                                 validated.append(dtype(val))
                             except (TypeError, ValueError):
                                 pass
                             else:
                                 valid = True
                                 break
                         if not valid:
                             raise ValueError(
                                 f"{val} cannot be converted to any of the "
-                                f"given data types: {self.dtype}!")
+                                f"given data types: {self.dtype}!"
+                            )
 
         except TypeError:
             if self.dtype is None:
                 raise ValueError("Could not convert to list!")
             else:
                 raise ValueError(
-                    "Could not convert to list of type %s!" % str(self.dtype))
+                    "Could not convert to list of type %s!" % str(self.dtype)
+                )
         if self.length is not None and len(validated) != self.length:
-            raise ValueError('List with length %i is required! Not %i!' % (
-                self.length, len(validated)))
+            raise ValueError(
+                "List with length %i is required! Not %i!"
+                % (self.length, len(validated))
+            )
         return validated
 
 
 def validate_err_calc(val):
     """Validation function for the
     :attr:`psy_simple.plotter.FldmeanPlotter.err_calc` formatoption"""
     try:
         val = validate_float(val)
     except (ValueError, TypeError):
         pass
     else:
         if val <= 100 and val >= 0:
             return val
-        raise ValueError("Percentiles for the error calculation must lie "
-                         "between 0 and 100, not %s" % val)
+        raise ValueError(
+            "Percentiles for the error calculation must lie "
+            "between 0 and 100, not %s" % val
+        )
     try:
         val = ValidateList(float, 2)(val)
     except (ValueError, TypeError):
         pass
     else:
         if all((v <= 100 and v >= 0) for v in val):
             return val
-        raise ValueError("Percentiles for the error calculation must lie "
-                         "between 0 and 100, not %s" % val)
+        raise ValueError(
+            "Percentiles for the error calculation must lie "
+            "between 0 and 100, not %s" % val
+        )
     try:
         val = validate_str(val)
     except ValueError:
         pass
     else:
-        if 'std' not in val:
+        if "std" not in val:
             raise ValueError(
-                'A string for the error calculation must contain std!')
+                "A string for the error calculation must contain std!"
+            )
     return val
 
 
 class DictValValidator(object):
-    """A validation class for formatoptions that expect dictionaries as values
-    """
+    """A validation class for formatoptions that expect dictionaries as values"""
 
     def __init__(self, key, valid, validators, default, ignorecase=False):
         """
         Parameters
         ----------
         key: str
             The name of the formatoption (will be used for error handling)
@@ -620,16 +669,19 @@
         self.key = key
         self.valid = valid
         self.key_validator = ValidateInStrings(key, valid, ignorecase)
         self.default = default
         self.validate = validators
 
     def __call__(self, value):
-        if isinstance(value, dict) and value and all(
-                isinstance(key, six.string_types) for key in value):
+        if (
+            isinstance(value, dict)
+            and value
+            and all(isinstance(key, six.string_types) for key in value)
+        ):
             failed_key = False
             for key, val in list(six.iteritems(value)):
                 try:
                     new_key = self.key_validator(key)
                 except ValueError:
                     failed_key = True
                     break
@@ -646,36 +698,37 @@
             value = dict(zip(self.valid, repeat(value)))
         else:
             value = {self.default: self.validate(value)}
         return value
 
 
 class TicksValidator(ValidateInStrings):
-
     def __call__(self, val):
         # validate the ticks
         # if None, int or tuple (defining min- and max-range), pass
-        if val is None or isinstance(val, int) or (
-                isinstance(val, tuple) and len(val) <= 3):
+        if (
+            val is None
+            or isinstance(val, int)
+            or (isinstance(val, tuple) and len(val) <= 3)
+        ):
             return val
         # strings must be in the given list
         elif isinstance(val, six.string_types):
             return list(TicksType(val))
         elif isinstance(val, dict):
             return list(TicksType(**val))
         elif len(val) and isinstance(val[0], six.string_types):
             return list(TicksType(*val))
         # otherwise we assume an array
         else:
             return ValidateList()(val)
 
 
 class BoundsValidator:
-
-    def __init__(self, type, default='rounded', possible_instances=None):
+    def __init__(self, type, default="rounded", possible_instances=None):
         """
         For parameter description see
         :class:`matplotlib.rcsetup.ValidateInStrings`.
 
         Other Parameters
         ----------------
         inis: tuple
@@ -704,478 +757,791 @@
             return list(self.type(*val))
         # otherwise we assume an array
         else:
             return ValidateList(float)(val)
 
 
 class LineWidthValidator(ValidateInStrings):
-
     def __call__(self, val):
         if val is None:
             return val
         elif isinstance(val, six.string_types):
             return [ValidateInStrings.__call__(self, val), 1.0]
         elif np.asarray(val).ndim and isinstance(val[0], six.string_types):
             return [ValidateInStrings.__call__(self, val[0])] + list(val[1:])
         # otherwise we assume an array
         else:
             return np.asarray(val, float)
 
 
 def validate_plot(val):
     validator = ValidateInStrings(
-        '2d plot', ['mesh', 'contourf', 'contour', 'poly'], True)
+        "2d plot", ["mesh", "contourf", "contour", "poly"], True
+    )
 
     val = validator(val)
     return val
 
 
 # -----------------------------------------------------------------------------
 # ------------------------------ rcParams -------------------------------------
 # -----------------------------------------------------------------------------
 
 
 #: the :class:`~psyplot.config.rcsetup.RcParams` for the psy-simple plugin
-rcParams = RcParams(defaultParams={
-
-    # -------------------------------------------------------------------------
-    # ----------------------- Registered plotters -----------------------------
-    # -------------------------------------------------------------------------
-
-    'project.plotters': [
-        {'simple': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'SimplePlotterBase',
-             'plot_func': False,
-             'summary': ('All plotters that are visualized by the psy-simple '
-                         'package')},
-         'lineplot': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'LinePlotter',
-             'prefer_list': True,
-             'default_slice': None,
-             'summary': 'Make a line plot of one-dimensional data'},
-         'fldmean': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'FldmeanPlotter',
-             'prefer_list': True,
-             'default_slice': None,
-             'summary': 'Calculate and plot the mean over x- and y-dimensions'
-             },
-         'density': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'DensityPlotter',
-             'prefer_list': False,
-             'default_slice': None,
-             'summary': 'Make a density plot of point data'},
-         'barplot': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'BarPlotter',
-             'prefer_list': True,
-             'default_slice': None,
-             'summary': 'Make a bar plot of one-dimensional data'},
-         'violinplot': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'ViolinPlotter',
-             'prefer_list': True,
-             'default_slice': None,
-             'summary': 'Make a violin plot of your data'},
-         'plot2d': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'Simple2DPlotter',
-             'prefer_list': False,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': 'Make a simple plot of a 2D scalar field'},
-         'vector': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'SimpleVectorPlotter',
-             'prefer_list': False,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': 'Make a simple plot of a 2D vector field',
-             'example_call': "filename, name=[['u_var', 'v_var']], ..."},
-         'combined': {
-             'module': 'psy_simple.plotters',
-             'plotter_name': 'CombinedSimplePlotter',
-             'prefer_list': True,
-             'default_slice': 0,
-             'default_dims': {'x': slice(None), 'y': slice(None)},
-             'summary': ('Plot a 2D scalar field with an overlying vector '
-                         'field'),
-             'example_call': (
-                 "filename, name=[['my_variable', ['u_var', 'v_var']]], ...")},
-         },
-        validate_dict],
-
-    # -------------------------------------------------------------------------
-    # --------------------- Default formatoptions -----------------------------
-    # -------------------------------------------------------------------------
-
-    'plotter.baseplotter.tight': [False, validate_bool,
-                                  'fmt key for tight layout of the plots'],
-    'plotter.simple.grid': [
-        False, try_and_error(validate_bool_maybe_none, validate_color),
-        'fmt key to visualize the grid on simple plots (i.e. without '
-        'projection)'],
-
-    # labels
-    'plotter.baseplotter.title': [
-        '', six.text_type, 'fmt key to control the title of the axes'],
-    'plotter.baseplotter.figtitle': [
-        '', six.text_type, 'fmt key to control the title of the axes'],
-    'plotter.baseplotter.text': [
-        [], validate_text, 'fmt key to show text anywhere on the plot'],
-    'plotter.simple.ylabel': [
-        '', six.text_type, 'fmt key to modify the y-axis label for simple'
-        'plot (i.e. plots withouth projection)'],
-    'plotter.simple.xlabel': [
-        '', six.text_type, 'fmt key to modify the y-axis label for simple'
-        'plot (i.e. plots withouth projection)'],
-    'plotter.plot2d.clabel': [
-        '', six.text_type, 'fmt key to modify the colorbar label for 2D'
-        'plots'],
-
-    # text sizes
-    'plotter.baseplotter.titlesize': [
-        'large', validate_fontsize,
-        'fmt key for the fontsize of the axes title'],
-    'plotter.baseplotter.figtitlesize': [
-        12, validate_fontsize, 'fmt key for the fontsize of the figure title'],
-    'plotter.simple.labelsize': [
-        'medium', DictValValidator(
-            'labelsize', ['x', 'y'], validate_fontsize, None, True),
-        'fmt key for the fontsize of the x- and y-l abel of simple plots '
-        '(i.e. without projection)'],
-    'plotter.simple.ticksize': [
-        'medium', DictValValidator(
-            'ticksize', ['major', 'minor'], validate_fontsize, 'major', True),
-        'fmt key for the fontsize of the ticklabels of x- and y-axis of '
-        'simple plots (i.e. without projection)'],
-    'plotter.plot2d.cticksize': [
-        'medium', validate_fontsize,
-        'fmt key for the fontsize of the ticklabels of the colorbar of 2D '
-        'plots'],
-    'plotter.plot2d.clabelsize': [
-        'medium', validate_fontsize,
-        'fmt key for the fontsize of the colorbar label'],
-
-    # text weights
-    'plotter.baseplotter.titleweight': [
-        None, validate_fontweight,
-        'fmt key for the fontweight of the axes title'],
-    'plotter.baseplotter.figtitleweight': [
-        None, validate_fontweight,
-        'fmt key for the fontweight of the figure title'],
-    'plotter.simple.labelweight': [
-        None, DictValValidator(
-            'labelweight', ['x', 'y'], validate_fontweight, None, True),
-        'fmt key for the fontweight of the x- and y-l abel of simple plots '
-        '(i.e. without projection)'],
-    'plotter.simple.tickweight': [None, DictValValidator(
-        'tickweight', ['major', 'minor'], validate_fontweight, 'major', True),
-        'fmt key for the fontweight of the ticklabels of x- and y-axis of '
-        'simple plots (i.e. without projection)'],
-    'plotter.plot2d.ctickweight': [
-        None, validate_fontweight,
-        'fmt key for the fontweight of the ticklabels of the colorbar of 2D '
-        'plots'],
-    'plotter.plot2d.clabelweight': [
-        None, validate_fontweight,
-        'fmt key for the fontweight of the colorbar label'],
-
-    # text properties
-    'plotter.baseplotter.titleprops': [
-        {}, validate_dict, 'fmt key for the additional properties of the title'
-        ],
-    'plotter.baseplotter.figtitleprops': [
-        {}, validate_dict,
-        'fmt key for the additional properties of the figure title'],
-    'plotter.simple.labelprops': [{}, DictValValidator(
-        'labelprops', ['x', 'y'], validate_dict, None, True),
-        'fmt key for the additional properties of the x- and y-label'],
-    'plotter.simple.xtickprops': [
-        {'major': {}, 'minor': {}}, DictValValidator(
-            'xtickprops', ['major', 'minor'], validate_dict, 'major', True),
-        'fmt key for the additional properties of the ticklabels of x-axis'],
-    'plotter.simple.ytickprops': [
-        {'major': {}, 'minor': {}}, DictValValidator(
-            'ytickprops', ['major', 'minor'], validate_dict, 'major', True),
-        'fmt key for the additional properties of the ticklabels of y-axis'],
-    'plotter.plot2d.clabelprops': [
-        {}, validate_dict,
-        'fmt key for the additional properties of the colorbar label'],
-    'plotter.plot2d.ctickprops': [
-        {}, validate_dict,
-        'fmt key for the additional properties of the colorbar ticklabels'],
-
-    # mask formatoptions
-    'plotter.baseplotter.background': [
-        'rc', try_and_error(ValidateInStrings('background', ['rc']),
-                            validate_none, validate_color),
-        "The background color for the plot"],
-    'plotter.baseplotter.mask': [
-        None, try_and_error(validate_none, validate_str, validate_dataarray)],
-    'plotter.baseplotter.maskleq': [
-        None, try_and_error(validate_none, validate_float),
-        'fmt key to mask values less or equal than a certain threshold'],
-    'plotter.baseplotter.maskless': [
-        None, try_and_error(validate_none, validate_float),
-        'fmt key to mask values less than a certain threshold'],
-    'plotter.baseplotter.maskgreater': [
-        None, try_and_error(validate_none, validate_float),
-        'fmt key to mask values greater than a certain threshold'],
-    'plotter.baseplotter.maskgeq': [
-        None, try_and_error(validate_none, validate_float),
-        'fmt key to mask values greater than or equal to a certain threshold'],
-    'plotter.baseplotter.maskbetween': [
-        None, try_and_error(validate_none, ValidateList(float, 2)),
-        'fmt key to mask values between a certain range'],
-
-    # density plotter
-    'plotter.density.coord': [
-        None, try_and_error(validate_none, validate_dataarray,
-                            validate_str, validate_stringlist),
-        'Alternative x-coordinate to use for DensityPlotter'],
-    'plotter.density.xrange': [
-        'minmax', validate_limits, 'The histogram limits of the density plot'],
-    'plotter.density.yrange': [
-        'minmax', validate_limits, 'The histogram limits of the density plot'],
-    'plotter.density.precision': [
-        0, try_and_error(validate_float, ValidateList((float, str), 2),
-                         validate_str),
-        'The precision of the data to make sure that the bin width is not '
-        'below this value'],
-    'plotter.density.bins': [
-        10, try_and_error(validate_int, ValidateList(int, 2)),
-        'The bins in x- and y-direction of the density plot'],
-    'plotter.density.normed': [
-        None, try_and_error(validate_none, ValidateInStrings(
-            'normed', ['area', 'counts', 'x', 'y', 'col', 'column', 'columns',
-                       'row', 'rows'], True)),
-        'The normalization of the density histogram'],
-    'plotter.density.density': [
-        'hist', ValidateInStrings('density', ['hist', 'kde'], True)],
-
-    # axis color
-    'plotter.simple.axiscolor': [
-        None, validate_axiscolor, 'fmt key to modify the color of the spines'],
-
-    # SimplePlot
-    'plotter.line.coord': [
-        None, try_and_error(validate_none, validate_dataarray,
-                            validate_str, validate_stringlist),
-        'Alternative x-coordinate to use for LinePlotter'],
-    'plotter.line.plot': [
-        '-', validate_lineplot,
-        'fmt key to modify the line style'],
-    'plotter.line.error': [
-        'fill', try_and_error(ValidateInStrings('error', ['fill'], True),
-                              validate_none),
-        'The visualization type of the errors for line plots'],
-    'plotter.line.marker': [
-        None, validate_marker, 'The symbol of the marker'],
-    'plotter.line.markersize': [
-        None, try_and_error(validate_none, validate_float),
-        'The size of the marker'],
-    'plotter.line.linewidth': [
-        None, try_and_error(validate_none, validate_float),
-        'The widths of the lines'],
-    'plotter.line.erroralpha': [
-        0.15, validate_alpha, 'The alpha value of the error range'],
-    'plotter.bar.coord': [
-        None, try_and_error(validate_none, validate_dataarray,
-                            validate_str, validate_stringlist),
-        'Alternative x-coordinate to use for BarPlotter'],
-    'plotter.bar.widths': [
-        'equal', try_and_error(
-            validate_float, ValidateInStrings(
-                'widths', ['equal', 'data'], True)),
-        'fmt key to change between equal and data given width of the bars'],
-    'plotter.bar.categorical': [
-        None, validate_bool_maybe_none,
-        'fmt key to change between categorical and non-categorical plotting'],
-    'plotter.bar.alpha': [
-        1.0, validate_float,
-        'fmt key to control the transparency for the bar plots'],
-    'plotter.bar.plot': [
-        'bar', validate_lineplot,
-        'fmt key to modify whether bar plots shall be stacked or not'],
-    'plotter.violin.plot': [
-        True, validate_bool_maybe_none,
-        'fmt key to modify whether violin plots shall be drawn'],
-    'plotter.simple.transpose': [
-        False, validate_bool, 'fmt key to switch x- and y-axis'],
-    'plotter.simple.color': [
-        None, try_and_error(validate_none, validate_cmap, validate_iter),
-        'fmt key to modify the color cycle simple plots'],
-    'plotter.simple.ylim': [
-        'rounded', validate_limits, 'fmt key to specify the y-axis limits'],
-    'plotter.simple.xlim': [
-        'rounded', validate_limits, 'fmt key to specify the x-axis limits'],
-    'plotter.simple.sym_lims': [
-        None, validate_sym_lims,
-        'fmt key to make symmetric x- and y-axis limits'],
-    'plotter.simple.xticks': [
-        {'major': None, 'minor': None}, DictValValidator(
-            'xticks', ['major', 'minor'], TicksValidator(
-                'xticks', tick_strings, True), 'major', True),
-        'fmt key to modify the x-axis ticks'],
-    'plotter.simple.yticks': [
-        {'major': None, 'minor': None}, DictValValidator(
-            'yticks', ['major', 'minor'], TicksValidator(
-                'yticks', tick_strings, True), 'major', True),
-        'fmt key to modify the y-axis ticks'],
-    'plotter.simple.xticklabels': [
-        None, DictValValidator('xticklabels', ['major', 'minor'],
-                               validate_ticklabels, 'major', True),
-        'fmt key to modify the x-axis ticklabels'],
-    'plotter.simple.yticklabels': [
-        None, DictValValidator('yticklabels', ['major', 'minor'],
-                               validate_ticklabels, 'major', True),
-        'fmt key to modify the y-axis ticklabels'],
-    'plotter.simple.xrotation': [
-        0, validate_float,
-        'fmt key to modify the rotation of the x-axis ticklabels'],
-    'plotter.simple.yrotation': [
-        0, validate_float,
-        'fmt key to modify the rotation of the x-axis ticklabels'],
-    'plotter.simple.legendlabels': [
-        '%(arr_name)s', try_and_error(
-            validate_str, ValidateList(six.text_type)),
-        'fmt key to modify the legend labels'],
-    'plotter.simple.legend': [
-        True, validate_legend, 'fmt key to draw a legend'],
-
-    # FldmeanPlotter
-    'plotter.fldmean.mean': [
-        'mean', try_and_error(
-            ValidateInStrings('mean', ['mean', 'median'], True),
-            validate_float),
-        "The calculation result, either the 'mean', 'median' or a percentile"],
-    'plotter.fldmean.err_calc': [
-        'std', validate_err_calc,
-        "The error calculation method, either the 'std' or a minimum "
-        "and maximum percentile"],
-
-    # Plot2D
-    'plotter.plot2d.interp_bounds': [
-        None, validate_bool_maybe_none,
-        'Switch to interpolate the bounds for 2D plots'],
-    'plotter.plot2d.plot': [
-        'mesh', try_and_error(validate_none, validate_plot),
-        'fmt key to specify the plot type of 2D scalar plots'],
-    'plotter.plot2d.plot.min_circle_ratio': [
-        0.05, validate_float,
-        'fmt key to specify the min_circle_ratio that is used to mask very '
-        ' flat triangles in a triangular plot'],
-    'plotter.plot2d.cbar': [
-        ['b'], validate_cbarpos,
-        'fmt key to specify the position of the colorbar'],
-    'plotter.plot2d.cbarspacing': [
-        'uniform', validate_str,
-        'fmt key to specify the spacing of the colorbar'],
-    'plotter.plot2d.miss_color': [
-        None, try_and_error(validate_none, validate_color),
-        'fmt key to specify the color of missing values'],
-    'plotter.plot2d.cmap': [
-        'white_blue_red', validate_cmap, 'fmt key to specify the colormap'],
-    'plotter.plot2d.cticks': [
-        None, try_and_error(validate_none, BoundsValidator(
-            CTicksType, default='bounds')),
-        'fmt key to specify the ticks of the colorbar'],
-    'plotter.plot2d.cticklabels': [
-        None, validate_ticklabels,
-        'fmt key to specify the ticklabels of the colorbar'],
-    'plotter.plot2d.extend': [
-        'neither', validate_extend,
-        'fmt key to specify the style of the colorbar on minimum and maximum'],
-    'plotter.plot2d.bounds': [
-        'rounded', BoundsValidator(BoundsType, 'bounds', mpl.colors.Normalize),
-        'fmt key to specify bounds and norm of the colorbar'],
-    'plotter.plot2d.levels': [
-        None, BoundsValidator(BoundsType),
-        'fmt key to specify the levels for a contour plot'],
-    # TODO: Implement opacity
-    # 'plotter.plot2d.opacity': [None, try_and_error(validate_none,
-    #                                                validate_opacity)],
-    'plotter.plot2d.datagrid': [
-        None, try_and_error(validate_none, validate_dict, validate_str),
-        'fmt key to plot the lines of the data grid'],
-    'plotter.plot2d.mask_datagrid': [
-        True, validate_bool,
-        'fmt key to mask cells with NaN when plotting the data grid'],
-
-    # VectorPlot
-    'plotter.vector.plot': [
-        'quiver', try_and_error(validate_none, ValidateInStrings(
-            '2d plot', ['quiver', 'stream'], True)),
-        'fmt key for the plot type of vector plots'],
-    'plotter.vector.arrowsize': [
-        None, try_and_error(validate_none, validate_float),
-        'fmt key for the size of the arrows on vector plots'],
-    'plotter.vector.arrowstyle': [
-        '-|>', ValidateInStrings('arrowstyle', ArrowStyle._style_list),
-        'fmt key for the style of the arrows on stream plots'],
-    'plotter.vector.density': [
-        1.0, try_and_error(validate_float, ValidateList(float, 2)),
-        'fmt key for the density of arrows on a vector plot'],
-    'plotter.vector.linewidth': [
-        None, LineWidthValidator('linewidth', ['absolute', 'u', 'v'], True),
-        'fmt key for the linewidths of the arrows'],
-    'plotter.vector.color': [
-        'k', try_and_error(validate_float, validate_color, ValidateInStrings(
-            'color', ['absolute', 'u', 'v'], True)),
-        'fmt key for the colors of the arrows'],
-
-    # default texts
-    'texts.labels': [{'tinfo': '%H:%M',
-                      'dtinfo': '%B %d, %Y. %H:%M',
-                      'dinfo': '%B %d, %Y',
-                      'desc': '%(long_name)s [%(units)s]',
-                      'sdesc': '%(name)s [%(units)s]'}, validate_dict,
-                     'labels that shall be replaced in TextBase formatoptions',
-                     ' (e.g. the title formatoption) when inserted within '
-                     'curly braces ({}))'],
-    'texts.default_position': [(1., 1.), ValidateList(float, 2),
-                               'default position for the text fmt key'],
-    'texts.delimiter': [', ', validate_str,
-                        'default delimiter to separate netCDF meta attributes '
-                        'when displayed on the plot'],
-
-    # -------------------------------------------------------------------------
-    # ---------------------------- Miscallaneous ------------------------------
-    # -------------------------------------------------------------------------
-
-    # color lists for user-defined colormaps (see for example
-    # psy_simple.colors._cmapnames)
-    'colors.cmaps': [
-        {}, validate_cmaps,
-        'User defined color lists that shall be accessible through the '
-        ':meth:`psyplot.plotter.colors.get_cmap` function'],
-
-    'widgets.colors.cmaps': [
-        ["viridis", "Reds", "Blues", "Greens", "binary", "RdBu", "coolwarm",
-         "red_white_blue", "winter", "jet", "white_blue_red", "gist_ncar",
-         "gist_earth", "Paired", "gnuplot", "gnuplot2"],
-        validate_stringlist,
-        'Colormaps that should be listed in the context menu of the cmap '
-        'button'],
-
-    'ticks.which': ['major', ValidateInStrings(
-        'ticks.which', ['major', 'minor'], True),
-        'default tick that is used when using a x- or y-tick formatoption'],
-    })
+rcParams = RcParams(
+    defaultParams={
+        # -------------------------------------------------------------------------
+        # ----------------------- Registered plotters -----------------------------
+        # -------------------------------------------------------------------------
+        "project.plotters": [
+            {
+                "simple": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "SimplePlotterBase",
+                    "plot_func": False,
+                    "summary": (
+                        "All plotters that are visualized by the psy-simple "
+                        "package"
+                    ),
+                },
+                "lineplot": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "LinePlotter",
+                    "prefer_list": True,
+                    "default_slice": None,
+                    "summary": "Make a line plot of one-dimensional data",
+                },
+                "fldmean": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "FldmeanPlotter",
+                    "prefer_list": True,
+                    "default_slice": None,
+                    "summary": "Calculate and plot the mean over x- and y-dimensions",
+                },
+                "density": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "DensityPlotter",
+                    "prefer_list": False,
+                    "default_slice": None,
+                    "summary": "Make a density plot of point data",
+                },
+                "barplot": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "BarPlotter",
+                    "prefer_list": True,
+                    "default_slice": None,
+                    "summary": "Make a bar plot of one-dimensional data",
+                },
+                "violinplot": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "ViolinPlotter",
+                    "prefer_list": True,
+                    "default_slice": None,
+                    "summary": "Make a violin plot of your data",
+                },
+                "plot2d": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "Simple2DPlotter",
+                    "prefer_list": False,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": "Make a simple plot of a 2D scalar field",
+                },
+                "vector": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "SimpleVectorPlotter",
+                    "prefer_list": False,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": "Make a simple plot of a 2D vector field",
+                    "example_call": "filename, name=[['u_var', 'v_var']], ...",
+                },
+                "combined": {
+                    "module": "psy_simple.plotters",
+                    "plotter_name": "CombinedSimplePlotter",
+                    "prefer_list": True,
+                    "default_slice": 0,
+                    "default_dims": {"x": slice(None), "y": slice(None)},
+                    "summary": (
+                        "Plot a 2D scalar field with an overlying vector "
+                        "field"
+                    ),
+                    "example_call": (
+                        "filename, name=[['my_variable', ['u_var', 'v_var']]], ..."
+                    ),
+                },
+            },
+            validate_dict,
+        ],
+        # -------------------------------------------------------------------------
+        # --------------------- Default formatoptions -----------------------------
+        # -------------------------------------------------------------------------
+        "plotter.baseplotter.tight": [
+            False,
+            validate_bool,
+            "fmt key for tight layout of the plots",
+        ],
+        "plotter.simple.grid": [
+            False,
+            try_and_error(validate_bool_maybe_none, validate_color),
+            "fmt key to visualize the grid on simple plots (i.e. without "
+            "projection)",
+        ],
+        # labels
+        "plotter.baseplotter.title": [
+            "",
+            six.text_type,
+            "fmt key to control the title of the axes",
+        ],
+        "plotter.baseplotter.figtitle": [
+            "",
+            six.text_type,
+            "fmt key to control the title of the axes",
+        ],
+        "plotter.baseplotter.text": [
+            [],
+            validate_text,
+            "fmt key to show text anywhere on the plot",
+        ],
+        "plotter.simple.ylabel": [
+            "",
+            six.text_type,
+            "fmt key to modify the y-axis label for simple"
+            "plot (i.e. plots withouth projection)",
+        ],
+        "plotter.simple.xlabel": [
+            "",
+            six.text_type,
+            "fmt key to modify the y-axis label for simple"
+            "plot (i.e. plots withouth projection)",
+        ],
+        "plotter.plot2d.clabel": [
+            "",
+            six.text_type,
+            "fmt key to modify the colorbar label for 2D" "plots",
+        ],
+        # text sizes
+        "plotter.baseplotter.titlesize": [
+            "large",
+            validate_fontsize,
+            "fmt key for the fontsize of the axes title",
+        ],
+        "plotter.baseplotter.figtitlesize": [
+            12,
+            validate_fontsize,
+            "fmt key for the fontsize of the figure title",
+        ],
+        "plotter.simple.labelsize": [
+            "medium",
+            DictValValidator(
+                "labelsize", ["x", "y"], validate_fontsize, None, True
+            ),
+            "fmt key for the fontsize of the x- and y-l abel of simple plots "
+            "(i.e. without projection)",
+        ],
+        "plotter.simple.ticksize": [
+            "medium",
+            DictValValidator(
+                "ticksize",
+                ["major", "minor"],
+                validate_fontsize,
+                "major",
+                True,
+            ),
+            "fmt key for the fontsize of the ticklabels of x- and y-axis of "
+            "simple plots (i.e. without projection)",
+        ],
+        "plotter.plot2d.cticksize": [
+            "medium",
+            validate_fontsize,
+            "fmt key for the fontsize of the ticklabels of the colorbar of 2D "
+            "plots",
+        ],
+        "plotter.plot2d.clabelsize": [
+            "medium",
+            validate_fontsize,
+            "fmt key for the fontsize of the colorbar label",
+        ],
+        # text weights
+        "plotter.baseplotter.titleweight": [
+            None,
+            validate_fontweight,
+            "fmt key for the fontweight of the axes title",
+        ],
+        "plotter.baseplotter.figtitleweight": [
+            None,
+            validate_fontweight,
+            "fmt key for the fontweight of the figure title",
+        ],
+        "plotter.simple.labelweight": [
+            None,
+            DictValValidator(
+                "labelweight", ["x", "y"], validate_fontweight, None, True
+            ),
+            "fmt key for the fontweight of the x- and y-l abel of simple plots "
+            "(i.e. without projection)",
+        ],
+        "plotter.simple.tickweight": [
+            None,
+            DictValValidator(
+                "tickweight",
+                ["major", "minor"],
+                validate_fontweight,
+                "major",
+                True,
+            ),
+            "fmt key for the fontweight of the ticklabels of x- and y-axis of "
+            "simple plots (i.e. without projection)",
+        ],
+        "plotter.plot2d.ctickweight": [
+            None,
+            validate_fontweight,
+            "fmt key for the fontweight of the ticklabels of the colorbar of 2D "
+            "plots",
+        ],
+        "plotter.plot2d.clabelweight": [
+            None,
+            validate_fontweight,
+            "fmt key for the fontweight of the colorbar label",
+        ],
+        # text properties
+        "plotter.baseplotter.titleprops": [
+            {},
+            validate_dict,
+            "fmt key for the additional properties of the title",
+        ],
+        "plotter.baseplotter.figtitleprops": [
+            {},
+            validate_dict,
+            "fmt key for the additional properties of the figure title",
+        ],
+        "plotter.simple.labelprops": [
+            {},
+            DictValValidator(
+                "labelprops", ["x", "y"], validate_dict, None, True
+            ),
+            "fmt key for the additional properties of the x- and y-label",
+        ],
+        "plotter.simple.xtickprops": [
+            {"major": {}, "minor": {}},
+            DictValValidator(
+                "xtickprops", ["major", "minor"], validate_dict, "major", True
+            ),
+            "fmt key for the additional properties of the ticklabels of x-axis",
+        ],
+        "plotter.simple.ytickprops": [
+            {"major": {}, "minor": {}},
+            DictValValidator(
+                "ytickprops", ["major", "minor"], validate_dict, "major", True
+            ),
+            "fmt key for the additional properties of the ticklabels of y-axis",
+        ],
+        "plotter.plot2d.clabelprops": [
+            {},
+            validate_dict,
+            "fmt key for the additional properties of the colorbar label",
+        ],
+        "plotter.plot2d.ctickprops": [
+            {},
+            validate_dict,
+            "fmt key for the additional properties of the colorbar ticklabels",
+        ],
+        # mask formatoptions
+        "plotter.baseplotter.background": [
+            "rc",
+            try_and_error(
+                ValidateInStrings("background", ["rc"]),
+                validate_none,
+                validate_color,
+            ),
+            "The background color for the plot",
+        ],
+        "plotter.baseplotter.mask": [
+            None,
+            try_and_error(validate_none, validate_str, validate_dataarray),
+        ],
+        "plotter.baseplotter.maskleq": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "fmt key to mask values less or equal than a certain threshold",
+        ],
+        "plotter.baseplotter.maskless": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "fmt key to mask values less than a certain threshold",
+        ],
+        "plotter.baseplotter.maskgreater": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "fmt key to mask values greater than a certain threshold",
+        ],
+        "plotter.baseplotter.maskgeq": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "fmt key to mask values greater than or equal to a certain threshold",
+        ],
+        "plotter.baseplotter.maskbetween": [
+            None,
+            try_and_error(validate_none, ValidateList(float, 2)),
+            "fmt key to mask values between a certain range",
+        ],
+        # density plotter
+        "plotter.density.coord": [
+            None,
+            try_and_error(
+                validate_none,
+                validate_dataarray,
+                validate_str,
+                validate_stringlist,
+            ),
+            "Alternative x-coordinate to use for DensityPlotter",
+        ],
+        "plotter.density.xrange": [
+            "minmax",
+            validate_limits,
+            "The histogram limits of the density plot",
+        ],
+        "plotter.density.yrange": [
+            "minmax",
+            validate_limits,
+            "The histogram limits of the density plot",
+        ],
+        "plotter.density.precision": [
+            0,
+            try_and_error(
+                validate_float, ValidateList((float, str), 2), validate_str
+            ),
+            "The precision of the data to make sure that the bin width is not "
+            "below this value",
+        ],
+        "plotter.density.bins": [
+            10,
+            try_and_error(validate_int, ValidateList(int, 2)),
+            "The bins in x- and y-direction of the density plot",
+        ],
+        "plotter.density.normed": [
+            None,
+            try_and_error(
+                validate_none,
+                ValidateInStrings(
+                    "normed",
+                    [
+                        "area",
+                        "counts",
+                        "x",
+                        "y",
+                        "col",
+                        "column",
+                        "columns",
+                        "row",
+                        "rows",
+                    ],
+                    True,
+                ),
+            ),
+            "The normalization of the density histogram",
+        ],
+        "plotter.density.density": [
+            "hist",
+            ValidateInStrings("density", ["hist", "kde"], True),
+        ],
+        # axis color
+        "plotter.simple.axiscolor": [
+            None,
+            validate_axiscolor,
+            "fmt key to modify the color of the spines",
+        ],
+        # SimplePlot
+        "plotter.line.coord": [
+            None,
+            try_and_error(
+                validate_none,
+                validate_dataarray,
+                validate_str,
+                validate_stringlist,
+            ),
+            "Alternative x-coordinate to use for LinePlotter",
+        ],
+        "plotter.line.plot": [
+            "-",
+            validate_lineplot,
+            "fmt key to modify the line style",
+        ],
+        "plotter.line.error": [
+            "fill",
+            try_and_error(
+                ValidateInStrings("error", ["fill"], True), validate_none
+            ),
+            "The visualization type of the errors for line plots",
+        ],
+        "plotter.line.marker": [
+            None,
+            validate_marker,
+            "The symbol of the marker",
+        ],
+        "plotter.line.markersize": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "The size of the marker",
+        ],
+        "plotter.line.linewidth": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "The widths of the lines",
+        ],
+        "plotter.line.erroralpha": [
+            0.15,
+            validate_alpha,
+            "The alpha value of the error range",
+        ],
+        "plotter.bar.coord": [
+            None,
+            try_and_error(
+                validate_none,
+                validate_dataarray,
+                validate_str,
+                validate_stringlist,
+            ),
+            "Alternative x-coordinate to use for BarPlotter",
+        ],
+        "plotter.bar.widths": [
+            "equal",
+            try_and_error(
+                validate_float,
+                ValidateInStrings("widths", ["equal", "data"], True),
+            ),
+            "fmt key to change between equal and data given width of the bars",
+        ],
+        "plotter.bar.categorical": [
+            None,
+            validate_bool_maybe_none,
+            "fmt key to change between categorical and non-categorical plotting",
+        ],
+        "plotter.bar.alpha": [
+            1.0,
+            validate_float,
+            "fmt key to control the transparency for the bar plots",
+        ],
+        "plotter.bar.plot": [
+            "bar",
+            validate_lineplot,
+            "fmt key to modify whether bar plots shall be stacked or not",
+        ],
+        "plotter.violin.plot": [
+            True,
+            validate_bool_maybe_none,
+            "fmt key to modify whether violin plots shall be drawn",
+        ],
+        "plotter.simple.transpose": [
+            False,
+            validate_bool,
+            "fmt key to switch x- and y-axis",
+        ],
+        "plotter.simple.color": [
+            None,
+            try_and_error(validate_none, validate_cmap, validate_iter),
+            "fmt key to modify the color cycle simple plots",
+        ],
+        "plotter.simple.ylim": [
+            "rounded",
+            validate_limits,
+            "fmt key to specify the y-axis limits",
+        ],
+        "plotter.simple.xlim": [
+            "rounded",
+            validate_limits,
+            "fmt key to specify the x-axis limits",
+        ],
+        "plotter.simple.sym_lims": [
+            None,
+            validate_sym_lims,
+            "fmt key to make symmetric x- and y-axis limits",
+        ],
+        "plotter.simple.xticks": [
+            {"major": None, "minor": None},
+            DictValValidator(
+                "xticks",
+                ["major", "minor"],
+                TicksValidator("xticks", tick_strings, True),
+                "major",
+                True,
+            ),
+            "fmt key to modify the x-axis ticks",
+        ],
+        "plotter.simple.yticks": [
+            {"major": None, "minor": None},
+            DictValValidator(
+                "yticks",
+                ["major", "minor"],
+                TicksValidator("yticks", tick_strings, True),
+                "major",
+                True,
+            ),
+            "fmt key to modify the y-axis ticks",
+        ],
+        "plotter.simple.xticklabels": [
+            None,
+            DictValValidator(
+                "xticklabels",
+                ["major", "minor"],
+                validate_ticklabels,
+                "major",
+                True,
+            ),
+            "fmt key to modify the x-axis ticklabels",
+        ],
+        "plotter.simple.yticklabels": [
+            None,
+            DictValValidator(
+                "yticklabels",
+                ["major", "minor"],
+                validate_ticklabels,
+                "major",
+                True,
+            ),
+            "fmt key to modify the y-axis ticklabels",
+        ],
+        "plotter.simple.xrotation": [
+            0,
+            validate_float,
+            "fmt key to modify the rotation of the x-axis ticklabels",
+        ],
+        "plotter.simple.yrotation": [
+            0,
+            validate_float,
+            "fmt key to modify the rotation of the x-axis ticklabels",
+        ],
+        "plotter.simple.legendlabels": [
+            "%(arr_name)s",
+            try_and_error(validate_str, ValidateList(six.text_type)),
+            "fmt key to modify the legend labels",
+        ],
+        "plotter.simple.legend": [
+            True,
+            validate_legend,
+            "fmt key to draw a legend",
+        ],
+        # FldmeanPlotter
+        "plotter.fldmean.mean": [
+            "mean",
+            try_and_error(
+                ValidateInStrings("mean", ["mean", "median"], True),
+                validate_float,
+            ),
+            "The calculation result, either the 'mean', 'median' or a percentile",
+        ],
+        "plotter.fldmean.err_calc": [
+            "std",
+            validate_err_calc,
+            "The error calculation method, either the 'std' or a minimum "
+            "and maximum percentile",
+        ],
+        # Plot2D
+        "plotter.plot2d.interp_bounds": [
+            None,
+            validate_bool_maybe_none,
+            "Switch to interpolate the bounds for 2D plots",
+        ],
+        "plotter.plot2d.plot": [
+            "mesh",
+            try_and_error(validate_none, validate_plot),
+            "fmt key to specify the plot type of 2D scalar plots",
+        ],
+        "plotter.plot2d.plot.min_circle_ratio": [
+            0.05,
+            validate_float,
+            "fmt key to specify the min_circle_ratio that is used to mask very "
+            " flat triangles in a triangular plot",
+        ],
+        "plotter.plot2d.cbar": [
+            ["b"],
+            validate_cbarpos,
+            "fmt key to specify the position of the colorbar",
+        ],
+        "plotter.plot2d.cbarspacing": [
+            "uniform",
+            validate_str,
+            "fmt key to specify the spacing of the colorbar",
+        ],
+        "plotter.plot2d.miss_color": [
+            None,
+            try_and_error(validate_none, validate_color),
+            "fmt key to specify the color of missing values",
+        ],
+        "plotter.plot2d.cmap": [
+            "white_blue_red",
+            validate_cmap,
+            "fmt key to specify the colormap",
+        ],
+        "plotter.plot2d.cticks": [
+            None,
+            try_and_error(
+                validate_none, BoundsValidator(CTicksType, default="bounds")
+            ),
+            "fmt key to specify the ticks of the colorbar",
+        ],
+        "plotter.plot2d.cticklabels": [
+            None,
+            validate_ticklabels,
+            "fmt key to specify the ticklabels of the colorbar",
+        ],
+        "plotter.plot2d.extend": [
+            "neither",
+            validate_extend,
+            "fmt key to specify the style of the colorbar on minimum and maximum",
+        ],
+        "plotter.plot2d.bounds": [
+            "rounded",
+            BoundsValidator(BoundsType, "bounds", mpl.colors.Normalize),
+            "fmt key to specify bounds and norm of the colorbar",
+        ],
+        "plotter.plot2d.levels": [
+            None,
+            BoundsValidator(BoundsType),
+            "fmt key to specify the levels for a contour plot",
+        ],
+        # TODO: Implement opacity
+        # 'plotter.plot2d.opacity': [None, try_and_error(validate_none,
+        #                                                validate_opacity)],
+        "plotter.plot2d.datagrid": [
+            None,
+            try_and_error(validate_none, validate_dict, validate_str),
+            "fmt key to plot the lines of the data grid",
+        ],
+        "plotter.plot2d.mask_datagrid": [
+            True,
+            validate_bool,
+            "fmt key to mask cells with NaN when plotting the data grid",
+        ],
+        # VectorPlot
+        "plotter.vector.plot": [
+            "quiver",
+            try_and_error(
+                validate_none,
+                ValidateInStrings("2d plot", ["quiver", "stream"], True),
+            ),
+            "fmt key for the plot type of vector plots",
+        ],
+        "plotter.vector.arrowsize": [
+            None,
+            try_and_error(validate_none, validate_float),
+            "fmt key for the size of the arrows on vector plots",
+        ],
+        "plotter.vector.arrowstyle": [
+            "-|>",
+            ValidateInStrings("arrowstyle", ArrowStyle._style_list),
+            "fmt key for the style of the arrows on stream plots",
+        ],
+        "plotter.vector.density": [
+            1.0,
+            try_and_error(validate_float, ValidateList(float, 2)),
+            "fmt key for the density of arrows on a vector plot",
+        ],
+        "plotter.vector.linewidth": [
+            None,
+            LineWidthValidator("linewidth", ["absolute", "u", "v"], True),
+            "fmt key for the linewidths of the arrows",
+        ],
+        "plotter.vector.color": [
+            "k",
+            try_and_error(
+                validate_float,
+                validate_color,
+                ValidateInStrings("color", ["absolute", "u", "v"], True),
+            ),
+            "fmt key for the colors of the arrows",
+        ],
+        # default texts
+        "texts.labels": [
+            {
+                "tinfo": "%H:%M",
+                "dtinfo": "%B %d, %Y. %H:%M",
+                "dinfo": "%B %d, %Y",
+                "desc": "%(long_name)s [%(units)s]",
+                "sdesc": "%(name)s [%(units)s]",
+            },
+            validate_dict,
+            "labels that shall be replaced in TextBase formatoptions",
+            " (e.g. the title formatoption) when inserted within "
+            "curly braces ({}))",
+        ],
+        "texts.default_position": [
+            (1.0, 1.0),
+            ValidateList(float, 2),
+            "default position for the text fmt key",
+        ],
+        "texts.delimiter": [
+            ", ",
+            validate_str,
+            "default delimiter to separate netCDF meta attributes "
+            "when displayed on the plot",
+        ],
+        # -------------------------------------------------------------------------
+        # ---------------------------- Miscallaneous ------------------------------
+        # -------------------------------------------------------------------------
+        # color lists for user-defined colormaps (see for example
+        # psy_simple.colors._cmapnames)
+        "colors.cmaps": [
+            {},
+            validate_cmaps,
+            "User defined color lists that shall be accessible through the "
+            ":meth:`psyplot.plotter.colors.get_cmap` function",
+        ],
+        "widgets.colors.cmaps": [
+            [
+                "viridis",
+                "Reds",
+                "Blues",
+                "Greens",
+                "binary",
+                "RdBu",
+                "coolwarm",
+                "red_white_blue",
+                "winter",
+                "jet",
+                "white_blue_red",
+                "gist_ncar",
+                "gist_earth",
+                "Paired",
+                "gnuplot",
+                "gnuplot2",
+            ],
+            validate_stringlist,
+            "Colormaps that should be listed in the context menu of the cmap "
+            "button",
+        ],
+        "ticks.which": [
+            "major",
+            ValidateInStrings("ticks.which", ["major", "minor"], True),
+            "default tick that is used when using a x- or y-tick formatoption",
+        ],
+    }
+)
 
 
 # add combinedplotter strings for vectorplot
-_subd = SubDict(rcParams.defaultParams, ['plotter.vector.', 'plotter.plot2d.'])
-for _key in ['plot', 'cbar', 'cmap', 'bounds', 'cticksize', 'cbarspacing',
-             'ctickweight', 'ctickprops', 'clabel', 'cticks', 'cticklabels',
-             'clabelsize', 'clabelprops', 'clabelweight']:
-    rcParams.defaultParams['plotter.combinedsimple.v%s' % _key] = _subd[_key]
-rcParams.defaultParams['plotter.combinedsimple.plot'] = rcParams.defaultParams[
-    'plotter.plot2d.plot']
+_subd = SubDict(rcParams.defaultParams, ["plotter.vector.", "plotter.plot2d."])
+for _key in [
+    "plot",
+    "cbar",
+    "cmap",
+    "bounds",
+    "cticksize",
+    "cbarspacing",
+    "ctickweight",
+    "ctickprops",
+    "clabel",
+    "cticks",
+    "cticklabels",
+    "clabelsize",
+    "clabelprops",
+    "clabelweight",
+]:
+    rcParams.defaultParams["plotter.combinedsimple.v%s" % _key] = _subd[_key]
+rcParams.defaultParams["plotter.combinedsimple.plot"] = rcParams.defaultParams[
+    "plotter.plot2d.plot"
+]
 del _key, _subd
 
 
 rcParams.update_from_defaultParams()
```

### Comparing `psy-simple-1.4.1/psy_simple/widgets/colors.py` & `psy-simple-1.5.0/psy_simple/widgets/colors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,50 @@
 """Module for color specific widgets
 
 This module corresponds to the :mod:`psy_simple.colors` module as a version for
 the usage in the psyplot GUI.
 """
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-simple and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum Hereon
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-import six
+
+import contextlib
 import os.path as osp
-from itertools import chain
 from functools import partial
-import contextlib
-from psyplot.data import safe_list, rcParams
-from psy_simple.widgets import Switch2FmtButton, get_icon
-import psy_simple.colors as psc
-from psy_simple.plugin import BoundsType, CTicksType
-from psyplot.docstring import docstrings
-import numpy as np
-import xarray as xr
+from itertools import chain
+
 import matplotlib as mpl
 import matplotlib.colors as mcol
-from PyQt5 import QtWidgets, QtCore, QtGui
+import numpy as np
+import six
+import xarray as xr
+from psyplot.data import rcParams, safe_list
+from psyplot.docstring import docstrings
+from PyQt5 import QtCore, QtGui, QtWidgets
 from PyQt5.QtCore import Qt
 
+import psy_simple.colors as psc
+from psy_simple.plugin import BoundsType, CTicksType
+from psy_simple.widgets import Switch2FmtButton, get_icon
 
-mpl_version = tuple(map(int, mpl.__version__.split('.')[:2]))
+mpl_version = tuple(map(int, mpl.__version__.split(".")[:2]))
 
 
-docstrings.delete_params('show_colormaps.parameters', 'show', 'use_qt')
+docstrings.delete_params("show_colormaps.parameters", "show", "use_qt")
 
 
 class ColormapModel(QtCore.QAbstractTableModel):
     """A model for displaying colormaps"""
 
-    @docstrings.get_sections(base='ColormapModel')
+    @docstrings.get_sections(base="ColormapModel")
     @docstrings.with_indent(8)
     def __init__(self, names=[], N=10, *args, **kwargs):
         """
         Parameters
         ----------
         %(show_colormaps.parameters.no_show|use_qt)s
 
@@ -73,47 +59,51 @@
 
     def set_colors(self, N=None, names=None):
         self.names = names = names or self.names
         self.N = N = N or self.N
 
         colors = np.zeros((len(names), N, 4))
         a = np.linspace(0, 1, N)
-        for i, cmap in enumerate(map(lambda name: psc.get_cmap(name, N),
-                                     names)):
+        for i, cmap in enumerate(
+            map(lambda name: psc.get_cmap(name, N), names)
+        ):
             colors[i, :, :] = cmap(a)
 
         self.color_da = xr.DataArray(
-            colors, coords={'cmap': list(map(str, names))},
-            dims=('cmap', 'color', 'rgba'))
+            colors,
+            coords={"cmap": list(map(str, names))},
+            dims=("cmap", "color", "rgba"),
+        )
 
     def rowCount(self, index=QtCore.QModelIndex()):
         return self.color_da.shape[0]
 
     def columnCount(self, index=QtCore.QModelIndex()):
         return self.color_da.shape[1]
 
     def data(self, index, role=Qt.DisplayRole):
         """Cell content"""
         if not index.isValid():
             return None
         if role == Qt.DisplayRole or role == Qt.EditRole:
-            return ' '
+            return " "
         if role == Qt.BackgroundColorRole:
             color = self.color_da[index.row(), index.column()].values
             return QtGui.QColor.fromRgbF(*color)
         return None
 
     def headerData(self, section, orientation, role=Qt.DisplayRole):
         """Set header data"""
         if role != Qt.DisplayRole:
             return None
         if orientation == Qt.Vertical:
             return six.text_type(self.color_da.cmap[section].values)
-        return super(ColormapModel, self).headerData(section, orientation,
-                                                     role)
+        return super(ColormapModel, self).headerData(
+            section, orientation, role
+        )
 
     def reset(self):
         self.beginResetModel()
         self.endResetModel()
 
 
 class ColormapTable(QtWidgets.QTableView):
@@ -170,15 +160,16 @@
         model = self.model()
         name = six.text_type(self.orig_color_da.cmap[row].values)
         colors = model.color_da[row].values
         orig_colors = self.orig_color_da[row].values
         if np.allclose(colors, orig_colors):
             return model.names[row]
         return mcol.LinearSegmentedColormap.from_list(
-            name, colors, N=self.columnCount())
+            name, colors, N=self.columnCount()
+        )
 
 
 class ColormapDialog(QtWidgets.QDialog):
     """A widget for selecting a colormap"""
 
     @docstrings.with_indent(8)
     def __init__(self, names=[], N=10, editable=True, *args, **kwargs):
@@ -199,18 +190,26 @@
             vbox.addWidget(QtWidgets.QLabel("Double-click a color to edit"))
         vbox.addWidget(self.table)
         self.setLayout(vbox)
         col_width = self.table.columnWidth(0)
         header_width = self.table.verticalHeader().width()
         row_height = self.table.rowHeight(0)
         available = QtWidgets.QDesktopWidget().availableGeometry()
-        height = int(min(row_height * (self.table.rowCount() + 1),
-                         2. * available.height() / 3.))
-        width = int(min(header_width + col_width * N + 0.5 * col_width,
-                        2. * available.width() / 3.))
+        height = int(
+            min(
+                row_height * (self.table.rowCount() + 1),
+                2.0 * available.height() / 3.0,
+            )
+        )
+        width = int(
+            min(
+                header_width + col_width * N + 0.5 * col_width,
+                2.0 * available.width() / 3.0,
+            )
+        )
         self.resize(QtCore.QSize(width, height))
 
     @classmethod
     @docstrings.with_indent(8)
     def get_colormap(cls, names=[], N=10, *args, **kwargs):
         """Open a :class:`ColormapDialog` and get a colormap
 
@@ -229,68 +228,74 @@
             Either the name of a standard colormap available via
             :func:`psy_simple.colors.get_cmap` or a colormap
         """
         names = safe_list(names)
         obj = cls(names, N, *args, **kwargs)
         vbox = obj.layout()
         buttons = QtWidgets.QDialogButtonBox(
-            QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel, parent=obj)
+            QtWidgets.QDialogButtonBox.Ok | QtWidgets.QDialogButtonBox.Cancel,
+            parent=obj,
+        )
         buttons.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(False)
         vbox.addWidget(buttons)
         buttons.accepted.connect(obj.accept)
         buttons.rejected.connect(obj.reject)
 
         obj.table.selectionModel().selectionChanged.connect(
-            lambda indices: buttons.button(QtWidgets.QDialogButtonBox.Ok).setEnabled(
-                bool(indices)))
+            lambda indices: buttons.button(
+                QtWidgets.QDialogButtonBox.Ok
+            ).setEnabled(bool(indices))
+        )
         accepted = obj.exec_()
         if accepted:
             return obj.table.chosen_colormap
 
-    docstrings.delete_params('show_colormaps.parameters', 'use_qt')
+    docstrings.delete_params("show_colormaps.parameters", "use_qt")
 
     @classmethod
     @docstrings.with_indent(8)
     def show_colormap(cls, names=[], N=10, show=True, *args, **kwargs):
         """Show a colormap dialog
 
         Parameters
         ----------
         %(show_colormaps.parameters.no_use_qt)s"""
         names = safe_list(names)
         obj = cls(names, N, *args, **kwargs)
         vbox = obj.layout()
-        buttons = QtWidgets.QDialogButtonBox(QtWidgets.QDialogButtonBox.Close, parent=obj)
+        buttons = QtWidgets.QDialogButtonBox(
+            QtWidgets.QDialogButtonBox.Close, parent=obj
+        )
         buttons.rejected.connect(obj.close)
         vbox.addWidget(buttons)
         if show:
             obj.show()
         return obj
 
 
 def create_cmap_thumb(cmap, output=None):
-    from matplotlib.figure import Figure
     from matplotlib.cm import ScalarMappable
+    from matplotlib.figure import Figure
 
-    fig = Figure(figsize=(4., 0.2))
+    fig = Figure(figsize=(4.0, 0.2))
     cax = fig.add_axes([0, 0, 1, 1])
     _cmap = psc.get_cmap(cmap)
     mappable = ScalarMappable(cmap=_cmap)
     mappable.set_array([])
-    fig.colorbar(mappable, cmap=_cmap, cax=cax, orientation='horizontal')
+    fig.colorbar(mappable, cmap=_cmap, cax=cax, orientation="horizontal")
     if output:
         fig.savefig(output, dpi=72)
     return fig
 
 
 class HighlightWidget(QtWidgets.QWidget):
-
     def set_highlighted(self, b):
-        self.setBackgroundRole(QtGui.QPalette.Highlight if b else
-                               QtGui.QPalette.Window)
+        self.setBackgroundRole(
+            QtGui.QPalette.Highlight if b else QtGui.QPalette.Window
+        )
         self.setAutoFillBackground(b)
 
     def enterEvent(self, event):
         self.set_highlighted(True)
 
     def leaveEvent(self, event):
         self.set_highlighted(False)
@@ -302,30 +307,30 @@
     # a signal that is triggered if the colormap has been changed
     colormap_changed = QtCore.pyqtSignal([str], [mcol.Colormap])
 
     def __init__(self, cmaps=None, current=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         if cmaps is None:
-            cmaps = list(rcParams['widgets.colors.cmaps'])
+            cmaps = list(rcParams["widgets.colors.cmaps"])
 
         self.cmaps = cmaps
 
         self.setText(current or cmaps[0])
         self.cmap_menu = self.setup_cmap_menu()
         self.setMenu(self.cmap_menu)
 
         max_width = max(map(self.fontMetrics().width, cmaps)) * 2
         self.setMinimumWidth(max_width)
         self.setPopupMode(QtWidgets.QToolButton.InstantPopup)
 
     def setup_cmap_menu(self):
         menu = QtWidgets.QMenu()
         for cmap in self.cmaps:
-            icon = get_icon(osp.join('cmaps', cmap))
+            icon = get_icon(osp.join("cmaps", cmap))
             if osp.exists(icon):
                 action = QtWidgets.QWidgetAction(menu)
                 w = HighlightWidget()
                 hbox = QtWidgets.QVBoxLayout()
                 label = QtWidgets.QLabel()
                 label.setPixmap(QtGui.QPixmap(icon))
                 hbox.addWidget(label)
@@ -340,15 +345,15 @@
         return menu
 
     def set_cmap(self, cmap):
         if isinstance(cmap, str):
             self.setText(str(cmap))
             self.colormap_changed[str].emit(cmap)
         else:
-            self.setText('Custom')
+            self.setText("Custom")
             self.colormap_changed[mcol.Colormap].emit(cmap)
 
     def open_cmap_dialog(self, N=10):
         cmap = ColormapDialog.get_colormap(N=N)
         if cmap is not None:
             self.set_cmap(cmap)
 
@@ -358,48 +363,51 @@
 
     #: a signal that is emitted with an rgba color if the chosen color changes
     color_changed = QtCore.pyqtSignal(QtGui.QColor)
 
     #: QtCore.QColor. The current color that is displayed
     color = None
 
-    def __init__(self, color='w', *args, **kwargs):
+    def __init__(self, color="w", *args, **kwargs):
         """The color to display
 
         Parameters
         ----------
         color: object
             Either a QtGui.QColor object or a color that can be converted
             to RGBA using the :func:`matplotlib.colors.to_rgba` function"""
         super(ColorLabel, self).__init__(*args, **kwargs)
         self.setColumnCount(1)
         self.setRowCount(1)
         self.setVerticalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.setHorizontalScrollBarPolicy(Qt.ScrollBarAlwaysOff)
         self.horizontalHeader().setHidden(True)
         self.horizontalHeader().setSectionResizeMode(
-            QtWidgets.QHeaderView.Stretch)
+            QtWidgets.QHeaderView.Stretch
+        )
         self.verticalHeader().setHidden(True)
-        self.verticalHeader().setSectionResizeMode(QtWidgets.QHeaderView.Stretch)
+        self.verticalHeader().setSectionResizeMode(
+            QtWidgets.QHeaderView.Stretch
+        )
         self.setEditTriggers(QtWidgets.QTableWidget.NoEditTriggers)
         self.setSelectionMode(QtWidgets.QTableWidget.NoSelection)
         self.itemClicked.connect(self.select_color)
         self.color_item = QtWidgets.QTableWidgetItem()
         self.setItem(0, 0, self.color_item)
         self.adjust_height()
         self.set_color(color)
         self.orig_color = self.color
 
         self.setMaximumWidth(80)
 
     def select_color(self, *args):
-        """Select a color using :meth:`PyQt5.QtWidgets.QColorDialog.getColor`
-        """
+        """Select a color using :meth:`PyQt5.QtWidgets.QColorDialog.getColor`"""
         color = QtWidgets.QColorDialog.getColor(
-            self.color_item.background().color())
+            self.color_item.background().color()
+        )
         if color.isValid():
             self.set_color(color)
 
     def set_color(self, color):
         """Set the color of the label
 
         This method sets the given `color` as background color for the cell
@@ -412,24 +420,25 @@
             to RGBA using the :func:`matplotlib.colors.to_rgba` function"""
         color = self._set_color(color)
         self.color_changed.emit(color)
 
     def setEnabled(self, b):
         if not b:
             orig_color = self.color
-            self._set_color('0.75')
+            self._set_color("0.75")
             self.color = orig_color
         else:
             self._set_color(self.color)
         super().setEnabled(b)
 
     def _set_color(self, color):
         if not isinstance(color, QtGui.QColor):
             color = QtGui.QColor(
-                *map(int, np.round(np.array(mcol.to_rgba(color)) * 255)))
+                *map(int, np.round(np.array(mcol.to_rgba(color)) * 255))
+            )
         self.color_item.setBackground(color)
         self.color = color
         return color
 
     def adjust_height(self):
         """Adjust the height to match the row height"""
         h = self.rowHeight(0) * self.rowCount()
@@ -444,29 +453,29 @@
 
 class BackGroundColorWidget(QtWidgets.QWidget):
     """The widget to select the axes background color"""
 
     def __init__(self, parent, fmto, project):
         super().__init__()
         ax = fmto.ax
-        self.cb_enable = QtWidgets.QCheckBox('transparent')
+        self.cb_enable = QtWidgets.QCheckBox("transparent")
         self.color_label = ColorLabel(ax.patch.get_facecolor())
         self.editor = parent
 
         self.cb_enable.setChecked(fmto.value is None)
 
         self.toggle_color_button()
 
         self.color_label.color_changed.connect(self.set_color)
 
         self.cb_enable.stateChanged.connect(self.toggle_color_button)
         self.cb_enable.stateChanged.connect(self.set_transparent)
 
         layout = QtWidgets.QHBoxLayout()
-        layout.addWidget(QtWidgets.QLabel('Select color:'))
+        layout.addWidget(QtWidgets.QLabel("Select color:"))
         layout.addWidget(self.color_label)
         layout.addWidget(self.cb_enable)
         layout.addStretch(0)
         self.setLayout(layout)
 
     def set_transparent(self):
         if self.cb_enable.isChecked():
@@ -494,33 +503,34 @@
 
         # add a select colormap button
         self.btn_choose = button = CmapButton()
         button.colormap_changed.connect(self.set_obj)
         button.colormap_changed[mcol.Colormap].connect(self.set_obj)
         self.btn_choose.cmap_menu.addSeparator()
         self.btn_choose.cmap_menu.addAction(
-            'More...', partial(self.choose_cmap, None))
+            "More...", partial(self.choose_cmap, None)
+        )
 
         if isinstance(fmto.value, str):
             self.btn_choose.setText(fmto.value)
         else:
             self.btn_choose.setText("Custom")
 
         hbox.addWidget(button)
 
         # add a show colormap button
-        self.btn_show = button = QtWidgets.QPushButton('Edit...')
+        self.btn_show = button = QtWidgets.QPushButton("Edit...")
         button.clicked.connect(self.edit_cmap)
         hbox.addWidget(button)
 
         # add a checkbox to invert the colormap
         self.cb_invert = QtWidgets.QCheckBox("Inverted")
         self.cb_invert.setEnabled(isinstance(fmto.value, str))
         if isinstance(fmto.value, str):
-            self.cb_invert.setChecked(fmto.value.endswith('_r'))
+            self.cb_invert.setChecked(fmto.value.endswith("_r"))
         self.cb_invert.stateChanged.connect(self.invert_cmap)
         hbox.addWidget(self.cb_invert)
 
         hbox.addStretch(0)
 
         if properties:
             hbox.addWidget(Switch2FmtButton(parent, fmto.bounds, fmto.cbar))
@@ -534,48 +544,50 @@
     def invert_cmap(self):
         try:
             value = self.editor.get_obj()
         except Exception:
             return
         if isinstance(value, str):
             self.cb_invert.setEnabled(True)
-            if self.cb_invert.isChecked() and not value.endswith('_r'):
-                self.editor.set_obj(value + '_r')
-            elif value.endswith('_r'):
+            if self.cb_invert.isChecked() and not value.endswith("_r"):
+                self.editor.set_obj(value + "_r")
+            elif value.endswith("_r"):
                 self.editor.set_obj(value[:-2])
         else:
             self.refresh_cb_invert(value)
 
     def refresh_cb_invert(self, obj):
         try:
             self.cb_invert.blockSignals(True)
             if isinstance(obj, str):
                 self.cb_invert.setEnabled(True)
-                self.cb_invert.setChecked(obj.endswith('_r'))
+                self.cb_invert.setChecked(obj.endswith("_r"))
             else:
                 self.cb_invert.setEnabled(False)
                 self.cb_invert.setChecked(False)
         finally:
             self.cb_invert.blockSignals(False)
 
     def choose_cmap(self, cmap=None):
         if cmap is None:
             editor = self.editor
-            N = getattr(editor.fmto.bounds.norm, 'Ncmap', 10)
+            N = getattr(editor.fmto.bounds.norm, "Ncmap", 10)
             self.btn_choose.open_cmap_dialog(N)
         else:
             self.set_obj(cmap)
 
     def edit_cmap(self):
         editor = self.editor
         cmap = editor.get_obj()
         if cmap is not None:
             cmap = ColormapDialog.get_colormap(
-                cmap, N=getattr(editor.fmto.bounds.norm, 'Ncmap', 10),
-                parent=self)
+                cmap,
+                N=getattr(editor.fmto.bounds.norm, "Ncmap", 10),
+                parent=self,
+            )
             if cmap is not None:
                 editor.set_obj(cmap)
 
 
 class DataTicksCalculatorFmtWidget(QtWidgets.QWidget):
     """Fmt widget for :class:`psy_simple.plotters.DataTicksCalculator`
 
@@ -589,60 +601,65 @@
         QtWidgets.QWidget.__init__(self, parent)
 
         self.method = method
 
         hbox = QtWidgets.QHBoxLayout()
 
         self.sb_N = QtWidgets.QSpinBox()
-        self.sb_N.setSpecialValueText('auto')
+        self.sb_N.setSpecialValueText("auto")
         self.sb_N.setMinimum(0)
         hbox.addWidget(self.sb_N)
 
         self.txt_min_pctl = QtWidgets.QLineEdit()
-        self.txt_min_pctl.setValidator(QtGui.QDoubleValidator(0., 100., 10))
-
+        self.txt_min_pctl.setValidator(QtGui.QDoubleValidator(0.0, 100.0, 10))
 
-        hbox.addWidget(QtWidgets.QLabel('Min.:'))
+        hbox.addWidget(QtWidgets.QLabel("Min.:"))
 
         self.combo_min = QtWidgets.QComboBox()
-        self.combo_min.addItems(['absolute', 'percentile'])
+        self.combo_min.addItems(["absolute", "percentile"])
         hbox.addWidget(self.combo_min)
 
         hbox.addWidget(self.txt_min_pctl)
 
         self.txt_max_pctl = QtWidgets.QLineEdit()
-        self.txt_max_pctl.setValidator(QtGui.QDoubleValidator(0., 100., 10))
-        hbox.addWidget(QtWidgets.QLabel('Max.:'))
+        self.txt_max_pctl.setValidator(QtGui.QDoubleValidator(0.0, 100.0, 10))
+        hbox.addWidget(QtWidgets.QLabel("Max.:"))
 
         self.combo_max = QtWidgets.QComboBox()
-        self.combo_max.addItems(['absolute', 'percentile'])
+        self.combo_max.addItems(["absolute", "percentile"])
         hbox.addWidget(self.combo_max)
 
         hbox.addWidget(self.txt_max_pctl)
 
         self.sb_N.valueChanged.connect(self.set_obj)
         self.combo_min.currentIndexChanged.connect(self.set_obj)
         self.combo_max.currentIndexChanged.connect(self.set_obj)
         self.txt_min_pctl.textChanged.connect(self.set_obj)
         self.txt_max_pctl.textChanged.connect(self.set_obj)
 
         self.setLayout(hbox)
 
     def set_obj(self):
         obj = {
-            'method': self.method,
-            'N': self.sb_N.value() or None,
-            }
+            "method": self.method,
+            "N": self.sb_N.value() or None,
+        }
         if self.txt_min_pctl.text().strip():
-            key = 'vmin' if self.combo_min.currentText() == 'absolute' else \
-                'percmin'
+            key = (
+                "vmin"
+                if self.combo_min.currentText() == "absolute"
+                else "percmin"
+            )
             obj[key] = float(self.txt_min_pctl.text().strip())
         if self.txt_max_pctl.text().strip():
-            key = 'vmax' if self.combo_max.currentText() == 'absolute' else \
-                'percmax'
+            key = (
+                "vmax"
+                if self.combo_max.currentText() == "absolute"
+                else "percmax"
+            )
             obj[key] = float(self.txt_max_pctl.text().strip())
         val = list(self.methods_type(**obj))
         try:
             val[0] = val[0].name
         except AttributeError:
             pass
         self.parent().set_obj(val)
@@ -654,40 +671,40 @@
         try:
             value = self.methods_type(*value)
         except (ValueError, TypeError):
             pass
         else:
             self.sb_N.setValue(value.N or 0)
 
-            bounds_val = value.method.name in ['bounds', 'midbounds']
+            bounds_val = value.method.name in ["bounds", "midbounds"]
             self.txt_min_pctl.setEnabled(not bounds_val)
             self.txt_max_pctl.setEnabled(not bounds_val)
             self.combo_min.setEnabled(not bounds_val)
             self.combo_max.setEnabled(not bounds_val)
 
             decimals = None
             if value.vmin is not None and value.vmax is not None:
                 decimals = self.get_decimals(value.vmin, value.vmax)
             if value.vmin is not None:
                 if decimals is None:
                     decimals = -np.floor(np.log10(value.vmin)) + 4
                 self.txt_min_pctl.setText(str(np.round(value.vmin, decimals)))
-                self.combo_min.setCurrentText('absolute')
+                self.combo_min.setCurrentText("absolute")
             elif value.percmin != 0:
-                self.txt_min_pctl.setText('%1.6g' % value.percmin)
-                self.combo_min.setCurrentText('percentile')
+                self.txt_min_pctl.setText("%1.6g" % value.percmin)
+                self.combo_min.setCurrentText("percentile")
 
             if value.vmax is not None:
                 if decimals is None:
                     decimals = -np.floor(np.log10(value.vmax)) + 4
                 self.txt_max_pctl.setText(str(np.round(value.vmax, decimals)))
-                self.combo_max.setCurrentText('absolute')
+                self.combo_max.setCurrentText("absolute")
             elif value.percmax != 100:
-                self.txt_max_pctl.setText('%1.6g' % value.percmax)
-                self.combo_max.setCurrentText('percentile')
+                self.txt_max_pctl.setText("%1.6g" % value.percmax)
+                self.combo_max.setCurrentText("percentile")
 
     @staticmethod
     def get_decimals(vmin, vmax):
         if vmin == vmax:
             decimals = 4
         else:
             decimals = -np.floor(np.log10(abs(vmax - vmin))) + 4
@@ -708,50 +725,50 @@
         self.txt_min.setValidator(QtGui.QDoubleValidator())
         self.txt_max = QtWidgets.QLineEdit()
         self.txt_max.setValidator(QtGui.QDoubleValidator())
         self.txt_step = QtWidgets.QLineEdit()
         self.txt_step.setValidator(QtGui.QDoubleValidator(1e-10, 1e10, 10))
         self.sb_nsteps = QtWidgets.QSpinBox()
         self.step_inc_combo = combo = QtWidgets.QComboBox()
-        combo.addItems(['Step', '# Steps'])
+        combo.addItems(["Step", "# Steps"])
 
         if array is not None:
             vmin, vmax = array.min(), array.max()
             decimals = self.get_decimals(vmin, vmax)
 
-            self.txt_min.setText(f'%1.{decimals}g' % vmin)
-            self.txt_max.setText(f'%1.{decimals}g' % vmax)
+            self.txt_min.setText(f"%1.{decimals}g" % vmin)
+            self.txt_max.setText(f"%1.{decimals}g" % vmax)
             steps = np.diff(array)
             if len(steps) == 1 or np.diff(steps).max() < 1e-5:
-                self.txt_step.setText(f'%1.{decimals}g' % steps[0])
+                self.txt_step.setText(f"%1.{decimals}g" % steps[0])
                 combo.setCurrentIndex(0)
             else:
                 combo.setCurrentIndex(1)
             self.sb_nsteps.setValue(len(array))
 
         self.toggle_txt_step(combo.currentText())
 
         hbox = QtWidgets.QHBoxLayout()
-        hbox.addWidget(QtWidgets.QLabel('Min.'))
+        hbox.addWidget(QtWidgets.QLabel("Min."))
         hbox.addWidget(self.txt_min)
-        hbox.addWidget(QtWidgets.QLabel('Max.'))
+        hbox.addWidget(QtWidgets.QLabel("Max."))
         hbox.addWidget(self.txt_max)
         hbox.addWidget(combo)
         hbox.addWidget(self.txt_step)
         hbox.addWidget(self.sb_nsteps)
         self.setLayout(hbox)
 
         for w in [self.txt_min, self.txt_max, self.txt_step]:
             w.textChanged.connect(self.set_array)
         self.sb_nsteps.valueChanged.connect(self.set_array)
 
         combo.currentTextChanged.connect(self.toggle_txt_step)
 
     def toggle_txt_step(self, s):
-        show_step = s == 'Step'
+        show_step = s == "Step"
         self.txt_step.setVisible(show_step)
         self.sb_nsteps.setVisible(not show_step)
         self.txt_step.setEnabled(show_step)
         self.sb_nsteps.setEnabled(not show_step)
         self.set_array()
 
     @staticmethod
@@ -776,15 +793,16 @@
                 step = float(self.txt_step.text().strip())
             except (ValueError, TypeError):
                 return
             arr = np.arange(vmin, vmax + 0.05 * step, step)
         else:
             arr = np.linspace(vmin, vmax, self.sb_nsteps.value())
         self.parent().set_obj(
-            np.round(arr, self.get_decimals(vmin, vmax)).tolist())
+            np.round(arr, self.get_decimals(vmin, vmax)).tolist()
+        )
 
     def set_obj(self):
         self.set_array()
 
 
 class NormalizationWidget(QtWidgets.QWidget):
     """A simple widget representing a boundary norm"""
@@ -795,32 +813,33 @@
 
         validator = QtGui.QDoubleValidator()
         self.txt_min = QtWidgets.QLineEdit()
         self.txt_min.setValidator(validator)
         self.txt_max = QtWidgets.QLineEdit()
         self.txt_max.setValidator(validator)
 
-        self.lbl_linthresh = QtWidgets.QLabel('linthresh:')
+        self.lbl_linthresh = QtWidgets.QLabel("linthresh:")
         self.txt_linthresh = QtWidgets.QLineEdit()  # linthresh for SymLogNorm
         self.txt_linthresh.setValidator(validator)
         self.txt_linthresh.setToolTip(
-            'The threshold for linear scaling. Within this distance from 0, '
-            'the scaling will be linear, not logarithmic.')
+            "The threshold for linear scaling. Within this distance from 0, "
+            "the scaling will be linear, not logarithmic."
+        )
 
-        self.lbl_gamma = QtWidgets.QLabel('gamma:')
+        self.lbl_gamma = QtWidgets.QLabel("gamma:")
         self.txt_gamma = QtWidgets.QLineEdit()  # gamma for PowerNorm
         self.txt_gamma.setValidator(validator)
-        self.txt_gamma.setToolTip('The power value for the PowerNorm')
+        self.txt_gamma.setToolTip("The power value for the PowerNorm")
 
         self.fill_from_norm()
 
         hbox = QtWidgets.QHBoxLayout()
-        hbox.addWidget(QtWidgets.QLabel('Min.:'))
+        hbox.addWidget(QtWidgets.QLabel("Min.:"))
         hbox.addWidget(self.txt_min)
-        hbox.addWidget(QtWidgets.QLabel('Max.:'))
+        hbox.addWidget(QtWidgets.QLabel("Max.:"))
         hbox.addWidget(self.txt_max)
         hbox.addWidget(self.lbl_linthresh)
         hbox.addWidget(self.txt_linthresh)
         hbox.addWidget(self.lbl_gamma)
         hbox.addWidget(self.txt_gamma)
         self.setLayout(hbox)
 
@@ -828,31 +847,31 @@
         self.txt_max.textChanged.connect(self.set_obj)
         self.txt_linthresh.textChanged.connect(self.set_obj)
         self.txt_gamma.textChanged.connect(self.set_obj)
 
     def fill_from_norm(self):
         norm = self.norm
         if norm.vmin is not None:
-            self.txt_min.setText('%1.6g' % norm.vmin)
+            self.txt_min.setText("%1.6g" % norm.vmin)
         if norm.vmax is not None:
-            self.txt_max.setText('%1.6g' % norm.vmax)
+            self.txt_max.setText("%1.6g" % norm.vmax)
         if isinstance(self.norm, mcol.SymLogNorm):
             self.txt_linthresh.setVisible(True)
             self.txt_linthresh.setEnabled(True)
             self.lbl_linthresh.setVisible(True)
-            self.txt_linthresh.setText('%1.6g' % norm.linthresh)
+            self.txt_linthresh.setText("%1.6g" % norm.linthresh)
         else:
             self.txt_linthresh.setVisible(False)
             self.txt_linthresh.setEnabled(False)
             self.lbl_linthresh.setVisible(False)
         if isinstance(norm, mcol.PowerNorm):
             self.txt_gamma.setVisible(True)
             self.txt_gamma.setEnabled(True)
             self.lbl_gamma.setVisible(True)
-            self.txt_gamma.setText('%1.6g' % norm.gamma)
+            self.txt_gamma.setText("%1.6g" % norm.gamma)
         else:
             self.txt_gamma.setVisible(False)
             self.txt_gamma.setEnabled(False)
             self.lbl_gamma.setVisible(False)
 
     def set_obj(self):
         cls = self.norm.__class__
@@ -888,85 +907,83 @@
     _norm_widget = None
 
     current_widget = None
 
     methods_type = BoundsType
 
     norm_map = {
-        'No normalization': mcol.Normalize,
-        'log': mcol.LogNorm,
-        'symlog': mcol.SymLogNorm,
-        'power-law': mcol.PowerNorm,
-        }
+        "No normalization": mcol.Normalize,
+        "log": mcol.LogNorm,
+        "symlog": mcol.SymLogNorm,
+        "power-law": mcol.PowerNorm,
+    }
 
-    default_args = {
-        'symlog': [1e-3],  # linthresh
-        'power-law': [1.0]  # gamma
-        }
+    default_args = {"symlog": [1e-3], "power-law": [1.0]}  # linthresh  # gamma
 
-    default_kws = {
-        "symlog": {"base": 10} if mpl_version >= (3, 2) else {}
-    }
+    default_kws = {"symlog": {"base": 10} if mpl_version >= (3, 2) else {}}
 
-    methods = ['Discrete', 'Continuous']
+    methods = ["Discrete", "Continuous"]
 
     def __init__(self, parent, fmto, project, properties=True):
         QtWidgets.QWidget.__init__(self, parent)
         self._editor = parent
         hbox = QtWidgets.QHBoxLayout()
 
         self.type_combo = QtWidgets.QComboBox(self)
         self.type_combo.addItems(self.methods)
 
         self.method_combo = QtWidgets.QComboBox(self)
 
-        self.discrete_items = sorted(fmto.calc_funcs) + ['Custom']
+        self.discrete_items = sorted(fmto.calc_funcs) + ["Custom"]
 
         hbox.addWidget(self.type_combo)
         hbox.addWidget(self.method_combo)
         hbox.addStretch(0)
 
         self.type_combo.currentTextChanged.connect(self.refresh_methods)
         self.method_combo.currentTextChanged.connect(
-            self.refresh_current_widget)
+            self.refresh_current_widget
+        )
 
         # add a button to select other formatoptions
         if properties:
             hbox.addWidget(Switch2FmtButton(parent, fmto.cmap, fmto.cbar))
         self.setLayout(hbox)
 
         self.set_value(fmto.value)
 
     def set_value(self, value):
         with self.block_widgets(self.method_combo, self.type_combo):
             if value is None:
-                self.type_combo.setCurrentText('Continuous')
-                self.refresh_methods('Continuous')
-                self.method_combo.setCurrentText('No normalization')
+                self.type_combo.setCurrentText("Continuous")
+                self.refresh_methods("Continuous")
+                self.method_combo.setCurrentText("No normalization")
             elif isinstance(value, mcol.Normalize) and not hasattr(
-                    value, 'boundaries'):
-                self.type_combo.setCurrentText('Continuous')
-                self.refresh_methods('Continuous')
+                value, "boundaries"
+            ):
+                self.type_combo.setCurrentText("Continuous")
+                self.refresh_methods("Continuous")
 
                 if isinstance(value, mcol.LogNorm):
-                    self.method_combo.setCurrentText('log')
+                    self.method_combo.setCurrentText("log")
                 elif isinstance(value, mcol.SymLogNorm):
-                    self.method_combo.setCurrentText('symlog')
+                    self.method_combo.setCurrentText("symlog")
                 elif isinstance(value, mcol.PowerNorm):
-                    self.method_combo.setCurrentText('power-law')
+                    self.method_combo.setCurrentText("power-law")
                 else:
-                    self.method_combo.setCurrentText('Custom')
+                    self.method_combo.setCurrentText("Custom")
             else:
-                self.type_combo.setCurrentText('Discrete')
-                self.refresh_methods('Discrete')
+                self.type_combo.setCurrentText("Discrete")
+                self.refresh_methods("Discrete")
                 if not isinstance(value, mcol.Normalize) and isinstance(
-                        value[0], six.string_types):
+                    value[0], six.string_types
+                ):
                     self.method_combo.setCurrentText(value[0])
                 else:
-                    self.method_combo.setCurrentText('Custom')
+                    self.method_combo.setCurrentText("Custom")
 
         self.refresh_methods(self.type_combo.currentText())
 
     @contextlib.contextmanager
     def block_widgets(self, *widgets):
         for w in widgets:
             w.blockSignals(True)
@@ -974,69 +991,70 @@
         for w in widgets:
             w.blockSignals(False)
 
     def refresh_methods(self, text):
         current = self.method_combo.currentText()
         with self.block_widgets(self.method_combo):
             self.method_combo.clear()
-            if text == 'Discrete':
+            if text == "Discrete":
                 items = self.discrete_items
                 self.method_combo.addItems(items)
                 if current in items:
                     self.method_combo.setCurrentText(current)
-                elif current == 'No normalization' and 'rounded' in items:
-                    self.method_combo.setCurrentText('rounded')
+                elif current == "No normalization" and "rounded" in items:
+                    self.method_combo.setCurrentText("rounded")
             else:
                 self.method_combo.addItems(list(self.norm_map))
                 if current in self.norm_map:
                     self.method_combo.setCurrentText(current)
                 else:
-                    self.method_combo.setCurrentText('No normalization')
+                    self.method_combo.setCurrentText("No normalization")
 
         self.refresh_current_widget()
 
     def refresh_current_widget(self):
         if self.current_widget is not None:
             self.current_widget.setVisible(False)
-        if self.type_combo.currentText() == 'Continuous':
+        if self.type_combo.currentText() == "Continuous":
             s = self.method_combo.currentText()
-            norm = self.norm_map[s](*self.default_args.get(s, []),
-                                    **self.default_kws.get(s, {}))
+            norm = self.norm_map[s](
+                *self.default_args.get(s, []), **self.default_kws.get(s, {})
+            )
             self.current_widget = self.get_norm_widget(norm)
         else:
-            if self.method_combo.currentText() != 'Custom':
+            if self.method_combo.currentText() != "Custom":
                 self.current_widget = self.get_auto_discrete_array_widget()
             else:
                 self.current_widget = self.get_discrete_array_widget()
         if self.current_widget is not None:
             self.current_widget.setVisible(True)
             self.current_widget.set_obj()
 
     def get_auto_discrete_array_widget(self):
         method = self.method_combo.currentText()
         if self._auto_array_widget is not None:
             self._auto_array_widget.method = method
         else:
             self._auto_array_widget = DataTicksCalculatorFmtWidget(
-                self._editor, method, self.methods_type)
+                self._editor, method, self.methods_type
+            )
             self.layout().insertWidget(3, self._auto_array_widget)
 
         fmto = self._editor.fmto
-        self._auto_array_widget.refresh(
-            self.method_combo.currentText(), fmto)
+        self._auto_array_widget.refresh(self.method_combo.currentText(), fmto)
         return self._auto_array_widget
 
     def get_discrete_array_widget(self):
         if self._array_widget is not None:
             return self._array_widget
         fmto = self._editor.fmto
         try:
             arr = fmto.norm.boundaries
         except AttributeError:
-            arr = fmto.calc_funcs['rounded']()
+            arr = fmto.calc_funcs["rounded"]()
         self._array_widget = ArrayFmtWidget(self._editor, arr)
         self.layout().insertWidget(3, self._array_widget)
         return self._array_widget
 
     def get_norm_widget(self, norm):
         if self._norm_widget is not None:
             if norm.__class__ is not self._norm_widget.norm.__class__:
@@ -1051,51 +1069,53 @@
     def set_obj(self, obj):
         self._editor.set_obj(obj)
 
 
 class CTicksFmtWidget(BoundsFmtWidget):
     """The formatoptions widget for the colorbar ticks."""
 
-    methods = ['Discrete', 'Auto']
+    methods = ["Discrete", "Auto"]
 
     norm_map = {}
 
     methods_type = CTicksType
 
     auto_val = None
 
     def set_value(self, value):
         if value is self.auto_val:
             with self.block_widgets(self.method_combo, self.type_combo):
-                self.type_combo.setCurrentText('Auto')
-            self.refresh_methods('Auto')
+                self.type_combo.setCurrentText("Auto")
+            self.refresh_methods("Auto")
         else:
             super().set_value(value)
 
     def refresh_methods(self, text):
-        if text == 'Auto':
+        if text == "Auto":
             with self.block_widgets(self.method_combo):
                 self.method_combo.clear()
             self.set_obj(self.auto_val)
             self.refresh_current_widget()
         else:
             super().refresh_methods(text)
 
     def refresh_current_widget(self):
         w = self.current_widget
-        auto_ticks = self.type_combo.currentText() == 'Auto'
+        auto_ticks = self.type_combo.currentText() == "Auto"
         if auto_ticks and w is not None:
             w.setVisible(False)
             self.current_widget = None
         if not auto_ticks:
             super().refresh_current_widget()
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     # build colormap thumbnails
     import matplotlib.pyplot as plt
+
     available_cmaps = set(
-        chain(plt.cm.cmap_d, psc._cmapnames, rcParams['colors.cmaps']))
+        chain(plt.cm.cmap_d, psc._cmapnames, rcParams["colors.cmaps"])
+    )
     N = len(available_cmaps)
     for i, cmap in enumerate(available_cmaps, 1):
         print("%i of %i: Generating thumb %s" % (i, N, cmap))
-        create_cmap_thumb(cmap, get_icon(osp.join('cmaps', cmap)))
+        create_cmap_thumb(cmap, get_icon(osp.join("cmaps", cmap)))
```

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Blues.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Blues.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Blues_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Blues_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BrBG.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BrBG.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BrBG_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BrBG_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuGn.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuGn.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuGn_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuGn_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuPu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuPu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/BuPu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/BuPu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/CMRmap.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/CMRmap.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/CMRmap_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/CMRmap_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/GnBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/GnBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/GnBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/GnBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greens.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greens.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Greens_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Greens_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/OrRd.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/OrRd.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/OrRd_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/OrRd_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Oranges.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Oranges.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Oranges_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Oranges_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PRGn.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PRGn.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PRGn_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PRGn_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PiYG.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PiYG.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PiYG_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PiYG_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBuGn.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBuGn_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBuGn_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuOr.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuOr.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuOr_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuOr_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuRd.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuRd.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/PuRd_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/PuRd_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Purples.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Purples.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Purples_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Purples_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdGy.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdGy.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdGy_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdGy_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdPu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdPu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdPu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdPu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlGn.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlGn.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/RdYlGn_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/RdYlGn_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Reds.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Reds.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Reds_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Reds_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Spectral.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Spectral.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/Spectral_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/Spectral_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGn.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGn.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGnBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGnBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGnBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlGn_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlGn_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrBr.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrBr_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrBr_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrRd.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/YlOrRd_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/YlOrRd_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/bone_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/bone_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cividis.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cividis.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cividis_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cividis_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/coolwarm.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/coolwarm.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/coolwarm_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/coolwarm_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cubehelix.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cubehelix.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/cubehelix_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/cubehelix_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/flag.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/flag.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/flag_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/flag_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_earth.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_earth.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_earth_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_earth_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_ncar.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_ncar.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gist_ncar_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gist_ncar_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/gnuplot_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/gnuplot_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/inferno.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/inferno.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/inferno_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/inferno_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/jet.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/jet.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/jet_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/jet_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/magma.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/magma.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/magma_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/magma_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/nipy_spectral.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/nipy_spectral.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/nipy_spectral_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/nipy_spectral_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/pink.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/pink.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/pink_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/pink_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/plasma.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/plasma.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/plasma_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/plasma_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/prism.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/prism.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/prism_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/prism_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rainbow.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rainbow.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/rainbow_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/rainbow_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/terrain.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/terrain.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/terrain_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/terrain_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_shifted.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_shifted.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/twilight_shifted_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/twilight_shifted_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/viridis.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/viridis.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/viridis_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/viridis_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Blues.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Blues.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Greens.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Greens.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_RdBu.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_RdBu.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_RdBu_r.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_RdBu_r.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/icons/cmaps/w_Reds.png` & `psy-simple-1.5.0/psy_simple/widgets/icons/cmaps/w_Reds.png`

 * *Files identical despite different names*

### Comparing `psy-simple-1.4.1/psy_simple/widgets/texts.py` & `psy-simple-1.5.0/psy_simple/widgets/texts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,95 +1,96 @@
 # -*- coding: utf-8 -*-
 """Psyplot GUI widgets for modifying label formatoptions
 
 This module contains PyQt widgets that can be used to modify label
 formatoptions (e.g. title, xlabel, titleprops, etc.) in the psyplot GUI.
 """
 
-# Disclaimer
-# ----------
-#
-# Copyright (C) 2021 Helmholtz-Zentrum Hereon
-# Copyright (C) 2020-2021 Helmholtz-Zentrum Geesthacht
-# Copyright (C) 2016-2021 University of Lausanne
-#
-# This file is part of psy-simple and is released under the GNU LGPL-3.O license.
-# See COPYING and COPYING.LESSER in the root of the repository for full
-# licensing details.
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License version 3.0 as
-# published by the Free Software Foundation.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU LGPL-3.0 license for more details.
+
+# SPDX-FileCopyrightText: 2021-2024 Helmholtz-Zentrum Hereon
+# SPDX-FileCopyrightText: 2020-2021 Helmholtz-Zentrum Geesthacht
+# SPDX-FileCopyrightText: 2016-2024 University of Lausanne
 #
-# You should have received a copy of the GNU LGPL-3.0 license
-# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+# SPDX-License-Identifier: LGPL-3.0-only
 
-from psyplot_gui.compat.qtcompat import (
-    QWidget, QComboBox, QHBoxLayout, QPushButton, QLabel, QtGui, with_qt5,
-    QToolButton, QIcon, Qt)
-from psy_simple.widgets import get_icon, Switch2FmtButton
+
+from functools import partial
 from warnings import warn
+
 import matplotlib as mpl
 import matplotlib.colors as mcol
-from psyplot.compat.pycompat import OrderedDict
-from psyplot.docstring import docstrings
 from psyplot import utils
-from functools import partial
+from psyplot.docstring import docstrings
+from psyplot_gui.compat.qtcompat import (
+    QComboBox,
+    QHBoxLayout,
+    QIcon,
+    QLabel,
+    QPushButton,
+    Qt,
+    QtGui,
+    QToolButton,
+    QWidget,
+    with_qt5,
+)
 
+from psy_simple.widgets import Switch2FmtButton, get_icon
 
 if with_qt5:
-    from PyQt5.QtWidgets import QSpinBox, QFontDialog, QColorDialog
+    from PyQt5.QtWidgets import QColorDialog, QFontDialog, QSpinBox
 else:
-    from PyQt4.QtGui import QSpinBox, QFontDialog, QColorDialog
+    from PyQt4.QtGui import QColorDialog, QFontDialog, QSpinBox
 
 
 if with_qt5:
-    weights_mpl2qt = OrderedDict([
-        ('ultralight', QtGui.QFont.ExtraLight),
-        ('light', QtGui.QFont.Light),
-        ('normal', QtGui.QFont.Normal),
-        ('regular', QtGui.QFont.Normal),
-        ('book', QtGui.QFont.Normal),
-        ('medium', QtGui.QFont.Medium),
-        ('roman', QtGui.QFont.Medium),
-        ('semibold', QtGui.QFont.DemiBold),
-        ('demibold', QtGui.QFont.DemiBold),
-        ('demi', QtGui.QFont.DemiBold),
-        ('bold', QtGui.QFont.Bold),
-        ('heavy', QtGui.QFont.Bold),
-        ('extra bold', QtGui.QFont.ExtraBold),
-        ('black', QtGui.QFont.Black),
-        ])
+    weights_mpl2qt = dict(
+        [
+            ("ultralight", QtGui.QFont.ExtraLight),
+            ("light", QtGui.QFont.Light),
+            ("normal", QtGui.QFont.Normal),
+            ("regular", QtGui.QFont.Normal),
+            ("book", QtGui.QFont.Normal),
+            ("medium", QtGui.QFont.Medium),
+            ("roman", QtGui.QFont.Medium),
+            ("semibold", QtGui.QFont.DemiBold),
+            ("demibold", QtGui.QFont.DemiBold),
+            ("demi", QtGui.QFont.DemiBold),
+            ("bold", QtGui.QFont.Bold),
+            ("heavy", QtGui.QFont.Bold),
+            ("extra bold", QtGui.QFont.ExtraBold),
+            ("black", QtGui.QFont.Black),
+        ]
+    )
 else:
-    weights_mpl2qt = OrderedDict([
-        ('ultralight', QtGui.QFont.Light),
-        ('light', QtGui.QFont.Light),
-        ('normal', QtGui.QFont.Normal),
-        ('regular', QtGui.QFont.Normal),
-        ('book', QtGui.QFont.Normal),
-        ('medium', QtGui.QFont.Normal),
-        ('roman', QtGui.QFont.Normal),
-        ('semibold', QtGui.QFont.DemiBold),
-        ('demibold', QtGui.QFont.DemiBold),
-        ('demi', QtGui.QFont.DemiBold),
-        ('bold', QtGui.QFont.Bold),
-        ('heavy', QtGui.QFont.Bold),
-        ('extra bold', QtGui.QFont.Black),
-        ('black', QtGui.QFont.Black),
-        ])
-
-
-weights_qt2mpl = OrderedDict(
-    map(reversed, utils.unique_everseen(weights_mpl2qt.items(),
-                                        key=lambda t: t[1])))
+    weights_mpl2qt = dict(
+        [
+            ("ultralight", QtGui.QFont.Light),
+            ("light", QtGui.QFont.Light),
+            ("normal", QtGui.QFont.Normal),
+            ("regular", QtGui.QFont.Normal),
+            ("book", QtGui.QFont.Normal),
+            ("medium", QtGui.QFont.Normal),
+            ("roman", QtGui.QFont.Normal),
+            ("semibold", QtGui.QFont.DemiBold),
+            ("demibold", QtGui.QFont.DemiBold),
+            ("demi", QtGui.QFont.DemiBold),
+            ("bold", QtGui.QFont.Bold),
+            ("heavy", QtGui.QFont.Bold),
+            ("extra bold", QtGui.QFont.Black),
+            ("black", QtGui.QFont.Black),
+        ]
+    )
+
+
+weights_qt2mpl = dict(
+    map(
+        reversed,
+        utils.unique_everseen(weights_mpl2qt.items(), key=lambda t: t[1]),
+    )
+)
 
 
 def mpl_weight2qt(weight):
     """Convert a weight from matplotlib definition to a Qt weight
 
     Parameters
     ----------
@@ -106,115 +107,124 @@
     except KeyError:
         try:
             weight = float(weight) / 10
         except (ValueError, TypeError):
             weight = QtGui.QFont.Normal
         else:
             try:
-                weight = min(filter(lambda w: w >= weight, weights_qt2mpl),
-                             key=lambda w: abs(w - weight))
+                weight = min(
+                    filter(lambda w: w >= weight, weights_qt2mpl),
+                    key=lambda w: abs(w - weight),
+                )
             except ValueError:
                 weight = QtGui.QFont.Normal
     return weight
 
 
 class DictCombo(QComboBox):
     """A combobox that inserts keys into the formatoption"""
 
     def __init__(self, attrs, fmt_widget, modulo_style=True):
         QComboBox.__init__(self)
         self.fmt_widget = fmt_widget
         self.addItems(
-            [''] +
-            [(key + ': ' + str(val))[:40] for key, val in attrs.items()])
+            [""] + [(key + ": " + str(val))[:40] for key, val in attrs.items()]
+        )
         func = self.insert_modulo if modulo_style else self.insert_bracketed
         self.currentTextChanged.connect(func)
 
     def insert_modulo(self, s):
         self.fmt_widget.insert_obj(
-            ('%(' + s.split(':')[0] + ')s') if s else '')
+            ("%(" + s.split(":")[0] + ")s") if s else ""
+        )
 
     def insert_bracketed(self, s):
-        self.fmt_widget.insert_obj(
-                ('{' + s.split(':')[0] + '}') if s else '')
+        self.fmt_widget.insert_obj(("{" + s.split(":")[0] + "}") if s else "")
 
 
 class LabelWidget(QWidget):
     """A widget to modify a text label (title, xlabel, etc.)
 
     This widget contains one combobox for the ``'labels'`` key in the
     :attr:`psyplot.rcParams` dictionary, and a second combobox for the
     enhanced attributes of the corresponding formatoption object `fmto`.
 
     Additionally, it provides buttons to switch to the formatoption options
     of the corresponding fontsize, fontweight and fontproperties of this
     label"""
 
-    @docstrings.get_sections(base='LabelWidget')
+    @docstrings.get_sections(base="LabelWidget")
     def __init__(self, parent, fmto, project, properties=True):
         """
         Parameters
         ----------
         parent: psyplot_gui.fmt_widget.FormatoptionWidget
             The formatoption widget where this widget is inserted
         fmto: psyplot.plotter.Formatoption
             The formatoption that is represented by this widget
         project: psyplot.project.Project
             The current psyplot subproject"""
         QWidget.__init__(self, parent)
         hbox = QHBoxLayout()
 
         # Create a combo box for the rcParams 'labels' key
-        label_combo = DictCombo(fmto.rc['labels'], parent, modulo_style=False)
+        label_combo = DictCombo(fmto.rc["labels"], parent, modulo_style=False)
         hbox.addWidget(label_combo)
 
         # Create a combo for the :attr:`enhanced_attrs`
-        attrs = OrderedDict(sorted(utils.join_dicts(
-            [getattr(plotter, fmto.key).enhanced_attrs
-             for plotter in project.plotters],
-            delimiter=', ').items()))
+        attrs = dict(
+            sorted(
+                utils.join_dicts(
+                    [
+                        getattr(plotter, fmto.key).enhanced_attrs
+                        for plotter in project.plotters
+                    ],
+                    delimiter=", ",
+                ).items()
+            )
+        )
         attr_combo = DictCombo(attrs, parent)
         hbox.addWidget(attr_combo)
 
         fmtos = [
             # add a button to change to the properties formatoption
-            getattr(fmto.plotter, fmto.key + 'props', None),
-            getattr(fmto.plotter, fmto.key + 'size', None),
-            getattr(fmto.plotter, fmto.key + 'weight', None)
-            ]
+            getattr(fmto.plotter, fmto.key + "props", None),
+            getattr(fmto.plotter, fmto.key + "size", None),
+            getattr(fmto.plotter, fmto.key + "weight", None),
+        ]
         fmtos = list(filter(None, fmtos))
         if fmtos and properties:
             hbox.addWidget(Switch2FmtButton(parent, *fmtos))
 
         self.setLayout(hbox)
 
 
-docstrings.keep_params('LabelWidget.parameters', 'parent', 'fmto')
+docstrings.keep_params("LabelWidget.parameters", "parent", "fmto")
 
 
 class FontWeightWidget(QWidget):
     """A widget for modifying the fontweight of a label"""
 
-    @docstrings.get_sections(base='FontWeightWidget')
+    @docstrings.get_sections(base="FontWeightWidget")
     @docstrings.with_indent(8)
     def __init__(self, parent, fmto, artist=None, base=None):
         """
         Parameters
         ----------
         %(LabelWidget.parameters.parent|fmto)s
         artist: matplotlib.text.Text
             The text instance this formatoption is modifying
         base: psyplot.plotter.Formatoption
             The original formatoption of the label the given `fmto` belongs to
         """
         QWidget.__init__(self, parent)
         hbox = QHBoxLayout()
-        hbox.addWidget(QLabel('Font weights:'))
+        hbox.addWidget(QLabel("Font weights:"))
         if artist is None:
-            weight = 'normal'
+            weight = "normal"
         else:
             weight = artist.get_weight()
 
         self.spin_box = spin_box = QSpinBox(self)
         spin_box.setRange(1, 1000)
         try:
             weight = int(weight)
@@ -234,17 +244,17 @@
         combo.currentTextChanged.connect(parent.set_obj)
         hbox.addWidget(combo)
 
         # add a button to change to the properties formatoption
         if base is not None:
             fmtos = [
                 base,
-                getattr(fmto.plotter, base.key + 'props', None),
-                getattr(fmto.plotter, base.key + 'size', None),
-                ]
+                getattr(fmto.plotter, base.key + "props", None),
+                getattr(fmto.plotter, base.key + "size", None),
+            ]
             fmtos = list(filter(None, fmtos))
             hbox.addWidget(Switch2FmtButton(parent, *fmtos))
 
         self.setLayout(hbox)
 
 
 class FontSizeWidget(QWidget):
@@ -255,37 +265,46 @@
         """
         Parameters
         ----------
         %(FontWeightWidget.parameters)s
         """
         QWidget.__init__(self, parent)
         hbox = QHBoxLayout()
-        hbox.addWidget(QLabel('Font sizes:'))
+        hbox.addWidget(QLabel("Font sizes:"))
 
         self.spin_box = spin_box = QSpinBox(self)
         spin_box.setRange(1, int(1e9))
         if artist is not None:
             spin_box.setValue(int(artist.get_size()))
 
         spin_box.valueChanged.connect(parent.set_obj)
         hbox.addWidget(spin_box)
 
         combo = QComboBox()
-        combo.addItems(['xx-small', 'x-small', 'small', 'medium', 'large',
-                        'x-large', 'xx-large'])
+        combo.addItems(
+            [
+                "xx-small",
+                "x-small",
+                "small",
+                "medium",
+                "large",
+                "x-large",
+                "xx-large",
+            ]
+        )
         combo.currentTextChanged.connect(parent.set_obj)
         hbox.addWidget(combo)
 
         # add a button to change to the properties formatoption
         if base is not None:
             fmtos = [
                 base,
-                getattr(fmto.plotter, base.key + 'props', None),
-                getattr(fmto.plotter, base.key + 'weight', None),
-                ]
+                getattr(fmto.plotter, base.key + "props", None),
+                getattr(fmto.plotter, base.key + "weight", None),
+            ]
             fmtos = list(filter(None, fmtos))
             hbox.addWidget(Switch2FmtButton(parent, *fmtos))
 
         self.setLayout(hbox)
 
 
 class FontPropertiesWidget(QWidget):
@@ -302,63 +321,64 @@
         %(FontWeightWidget.parameters)s
         """
         QWidget.__init__(self, parent)
         hbox = QHBoxLayout()
         if artist is not None:
             self.current_font = self.artist_to_qfont(artist)
             self.current_color = QtGui.QColor.fromRgbF(
-                *mcol.to_rgba(artist.get_color()))
+                *mcol.to_rgba(artist.get_color())
+            )
         else:
             self.current_color = QtGui.QColor(Qt.black)
         self.fmto_name = fmto.name or fmto.key
 
         # choose font button
-        button = QPushButton('Choose font')
+        button = QPushButton("Choose font")
         button.clicked.connect(partial(self.choose_font, None))
         hbox.addWidget(button)
 
         # font size spin box
         self.spin_box = spin_box = QSpinBox(self)
         spin_box.setRange(1, int(1e9))
         if artist is not None:
             spin_box.setValue(int(artist.get_size()))
         spin_box.valueChanged.connect(self.modify_size)
         hbox.addWidget(spin_box)
 
         # font color button
         self.btn_font_color = button = QToolButton(self)
-        button.setIcon(QIcon(get_icon('font_color')))
+        button.setIcon(QIcon(get_icon("font_color")))
         button.clicked.connect(partial(self.choose_color, None))
         hbox.addWidget(button)
 
         # bold button
         self.btn_bold = button = QToolButton(self)
-        button.setIcon(QIcon(get_icon('bold')))
+        button.setIcon(QIcon(get_icon("bold")))
         button.clicked.connect(self.toggle_bold)
         button.setCheckable(True)
         if artist is not None:
             button.setChecked(self.current_font.weight() > 50)
         hbox.addWidget(button)
 
         # italic button
         self.btn_italic = button = QToolButton(self)
-        button.setIcon(QIcon(get_icon('italic')))
+        button.setIcon(QIcon(get_icon("italic")))
         button.clicked.connect(self.toggle_italic)
         button.setCheckable(True)
         if artist is not None:
             button.setChecked(self.current_font.italic())
         hbox.addWidget(button)
 
         if base is not None:
             # add a button to change to the base formatoption
             fmtos = [
                 base,
-                getattr(fmto.plotter, base.key + 'size', None),
-                getattr(fmto.plotter, base.key + 'weight', None),
-                ]
+                getattr(fmto.plotter, base.key + "size", None),
+                getattr(fmto.plotter, base.key + "weight", None),
+            ]
             fmtos = list(filter(None, fmtos))
             hbox.addWidget(Switch2FmtButton(parent, *fmtos))
 
         self.setLayout(hbox)
 
     @staticmethod
     def artist_to_qfont(artist):
@@ -371,71 +391,75 @@
 
         Returns
         -------
         PyQt5.QtGui.QFont
             The QFont object"""
         size = int(artist.get_size())
         weight = mpl_weight2qt(artist.get_weight())
-        italic = artist.get_style() == 'italic'
+        italic = artist.get_style() == "italic"
         for family in artist.get_family():
-            if family in ['sans-serif', 'cursive', 'monospace', 'serif']:
-                for name in mpl.rcParams['font.' + family]:
+            if family in ["sans-serif", "cursive", "monospace", "serif"]:
+                for name in mpl.rcParams["font." + family]:
                     font = QtGui.QFont(name, size, weight, italic)
                     if font.exactMatch():
                         break
             else:
                 font = QtGui.QFont(family, size, weight, italic)
         return font
 
     @staticmethod
     def qfont_to_artist_props(font):
         properties = {
-            'family': font.family(),
-            'size': font.pointSize(),
-            'weight': weights_qt2mpl[font.weight()],
-            'style': 'italic' if font.italic() else 'normal'}
+            "family": font.family(),
+            "size": font.pointSize(),
+            "weight": weights_qt2mpl[font.weight()],
+            "style": "italic" if font.italic() else "normal",
+        }
         if font.underline():
-            warn("Underline is ignored! Use LaTeX syntax: $\\underline{text}$!"
-                 )
+            warn(
+                "Underline is ignored! Use LaTeX syntax: $\\underline{text}$!"
+            )
         if font.strikeOut():
             warn("StrikeOut is ignored! Use LaTeX syntax: $\\sout{text}$!")
         return properties
 
     def modify_size(self, val):
         properties = self.load_properties()
-        properties['fontsize' if 'fontsize' in properties else 'size'] = val
+        properties["fontsize" if "fontsize" in properties else "size"] = val
         self.current_font.setPointSize(val)
         self.parent().set_obj(properties)
 
     def toggle_bold(self):
         properties = self.load_properties()
         bold = self.btn_bold.isChecked()
-        properties['weight'] = 'bold' if bold else 'normal'
+        properties["weight"] = "bold" if bold else "normal"
         self.current_font.setBold(bold)
         self.parent().set_obj(properties)
 
     def toggle_italic(self):
         properties = self.load_properties()
         italic = self.btn_italic.isChecked()
-        properties['style'] = 'italic' if italic else 'normal'
+        properties["style"] = "italic" if italic else "normal"
         self.current_font.setItalic(italic)
         self.parent().set_obj(properties)
 
     def load_properties(self):
         return dict(self.parent().get_obj() or {})
 
     def choose_font(self, font=None):
         """Choose a font for the label through a dialog"""
         fmt_widget = self.parent()
         if font is None:
             if self.current_font:
                 font, ok = QFontDialog.getFont(
-                    self.current_font, fmt_widget,
-                    'Select %s font' % self.fmto_name,
-                    QFontDialog.DontUseNativeDialog)
+                    self.current_font,
+                    fmt_widget,
+                    "Select %s font" % self.fmto_name,
+                    QFontDialog.DontUseNativeDialog,
+                )
             else:
                 font, ok = QFontDialog.getFont(fmt_widget)
             if not ok:
                 return
         self.current_font = font
         properties = self.load_properties()
         properties.update(self.qfont_to_artist_props(font))
@@ -461,15 +485,17 @@
         self.spin_box.setValue(font.pointSize())
         self.spin_box.blockSignals(False)
 
     def choose_color(self, color=None):
         fmt_widget = self.parent()
         if color is None:
             color = QColorDialog.getColor(
-                self.current_color, fmt_widget,
-                'Select %s color' % self.fmto_name)
+                self.current_color,
+                fmt_widget,
+                "Select %s color" % self.fmto_name,
+            )
         if not color.isValid():
             return
         self.current_color = color
         properties = self.load_properties()
-        properties['color'] = color.getRgbF()
+        properties["color"] = color.getRgbF()
         fmt_widget.set_obj(properties)
```

### Comparing `psy-simple-1.4.1/psy_simple.egg-info/SOURCES.txt` & `psy-simple-1.5.0/psy_simple.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-COPYING
-COPYING.LESSER
 MANIFEST.in
 README.rst
-setup.cfg
+pyproject.toml
 setup.py
-versioneer.py
+LICENSES/CC-BY-4.0.txt
+LICENSES/CC0-1.0.txt
+LICENSES/LGPL-3.0-only.txt
 psy_simple/__init__.py
 psy_simple/_version.py
 psy_simple/base.py
 psy_simple/colors.py
 psy_simple/plotters.py
 psy_simple/plugin.py
 psy_simple.egg-info/PKG-INFO
@@ -202,8 +202,31 @@
 psy_simple/widgets/icons/cmaps/white_blue_red.png
 psy_simple/widgets/icons/cmaps/white_blue_red_r.png
 psy_simple/widgets/icons/cmaps/white_red_blue.png
 psy_simple/widgets/icons/cmaps/white_red_blue_r.png
 psy_simple/widgets/icons/cmaps/winter.png
 psy_simple/widgets/icons/cmaps/winter_r.png
 psy_simple/widgets/icons/cmaps/wrb.png
-psy_simple/widgets/icons/cmaps/wrb_r.png
+psy_simple/widgets/icons/cmaps/wrb_r.png
+tests/test_barplot.py
+tests/test_barplot_data.py
+tests/test_barplot_single.py
+tests/test_base.py
+tests/test_colors.py
+tests/test_combined.py
+tests/test_combined_icon.py
+tests/test_density.py
+tests/test_density_kde.py
+tests/test_fldmean.py
+tests/test_fldmean_icon.py
+tests/test_lineplot.py
+tests/test_lineplot_single.py
+tests/test_plot2d.py
+tests/test_plot2d_contour.py
+tests/test_plot2d_icon.py
+tests/test_plot2d_icon_contour.py
+tests/test_plot2d_icon_edge.py
+tests/test_vector.py
+tests/test_vector_icon.py
+tests/test_vector_stream.py
+tests/test_violin.py
+tests/test_violin_single.py
```

