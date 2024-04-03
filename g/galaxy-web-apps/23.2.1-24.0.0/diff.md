# Comparing `tmp/galaxy-web-apps-23.2.1.tar.gz` & `tmp/galaxy-web-apps-24.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_apps/dist/.tmp-lz06dv5k/galaxy-web-apps-23.2.1.tar", last modified: Thu Feb 22 03:57:10 2024, max compression
+gzip compressed data, was "galaxy-web-apps-24.0.0.tar", last modified: Wed Apr  3 02:46:50 2024, max compression
```

## Comparing `galaxy-web-apps-23.2.1.tar` & `galaxy-web-apps-24.0.0.tar`

### file list

```diff
@@ -1,522 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    21524 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22878 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/biom/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/icn3d/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bb.xml
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/wig.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/gff.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/image/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/image/avivator.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/intermine/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/iobio/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/iobio/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/minerva/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8012 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    63340 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/erricon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    20770 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/formatHelp.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/delete.gif
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/delete_tag_icon_gray.png
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/dw.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      516 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/application-dock-270.png
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-090.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-circle.png
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090.png
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-split.png
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/block--plus-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/block--plus.png
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bookmarks.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bug.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/chart.png
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      490 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/chevron-expand.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/chevron.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/control-270.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-button.png
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-circle.png
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-small-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross.png
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/disk--arrow.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/disk.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/exclamation.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/external.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/eye.png
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/gear-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/gear.png
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/globe-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/globe.png
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/hammer-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      575 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/hammer.png
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/information-white.png
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layer-transparent.png
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layers-stack.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-left.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/navigation.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      309 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/pencil-small.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/pencil.png
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-button-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-button.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-circle.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/sticky-note-text.png
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tag--plus.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tag-label.png
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tags.png
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-bw.png
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-expand.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     1243 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toolbox-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toolbox.png
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/ui-slider-050.png
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/hatch-fade-023858.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/delete_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/eye_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_grey.png
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_grey.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/data_empty.png
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/data_error.png
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/data_ok.png
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/data_queued.png
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history.gif
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history_down_arrow.gif
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history_up_arrow.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_error_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_error_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_info_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_info_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_success_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_success_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_warning_lrg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_warning_sml.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/loading_large_white_bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/loading_small_white_bg.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/maf_icons/
--rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/maf_icons/interval2maf.png
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/openid-16x16.gif
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/square_empty.gif
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/square_error.gif
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/square_ok.gif
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/square_queued.gif
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/square_running.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/star.gif
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tool_menu_down_arrow.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/
--rw-r--r--   0 runner    (1001) docker     (127)   257713 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg
--rw-r--r--   0 runner    (1001) docker     (127)    81633 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg
--rw-r--r--   0 runner    (1001) docker     (127)    72821 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg
--rw-r--r--   0 runner    (1001) docker     (127)    92949 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg
--rw-r--r--   0 runner    (1001) docker     (127)   108978 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg
--rw-r--r--   0 runner    (1001) docker     (127)   109459 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/lda/
--rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png
--rw-r--r--   0 runner    (1001) docker     (127)    23673 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/block.png
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/close_btn.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/diag_bg.gif
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/go_btn.gif
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/handle-left.gif
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/handle-right.gif
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/pan_left.gif
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/pan_right.gif
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/show_history.gif
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/zoom_in.gif
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/zoom_in_full.gif
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/zoom_out.gif
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/zoom_out_full.gif
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/up.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/draggable_horizontal.png
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/draggable_vertical.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/strand_left.png
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/strand_left_inv.png
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/strand_right.png
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/visualization/strand_right_inv.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/yui/
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/incompatible-browser.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/patmat/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/patmat/findcluster.png
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/circster.css
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/data_running.gif
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/data_upload.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4046 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/icons.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/loading.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)     9902 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css
--rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif
--rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/vline.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/embed_item.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/history.css
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/info_icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery.rating.css
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/library.css
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/masthead.css
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/ok_small.png
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/question-octagon-frame.png
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/reports.css
--rw-r--r--   0 runner    (1001) docker     (127)    31536 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-fugue.png
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-history-buttons.png
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-history-states.png
--rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/trackster.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-model.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/test-file.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-model.js
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/user_disabled.html
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/static/welcome.html.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/base/
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/base/base_panels.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/display_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/display_common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/embed_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/galaxy_client_app.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/js-app.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/legacy/grid_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/legacy/grid_base_async.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/message.mako
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/no_access.mako
--rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/page_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/refresh_frames.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/slug_editing_js.mako
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/sorting_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/spark_base.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/tagging_common.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/tool_shed_rating.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/history/
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/history/as_xml.mako
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/history/list_as_xml.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/root/
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)    10235 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/phyloviz.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/sweepster.mako
--rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/base_panels.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/index.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/job_info.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/run_stats.mako
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/system.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/common/
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/
--rw-r--r--   0 runner    (1001) docker     (127)    57351 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako
--rw-r--r--   0 runner    (1001) docker     (127)    50772 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/base/webapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/
--rw-r--r--   0 runner    (1001) docker     (127)    18364 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/cloudauthz.py
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4444 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/container_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    17538 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/drs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/dynamic_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/extended_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/genomes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    24342 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    40610 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)    21594 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7392 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)    22973 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/library_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    38872 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/library_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/page_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/roles.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4089 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/sanitize_allow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/short_term_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    22648 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_shed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    24008 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/toolshed.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tours.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/trs_consumer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/trs_search.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/uploads.py
--rw-r--r--   0 runner    (1001) docker     (127)    49338 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    16198 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    64629 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)    43371 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/buildapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74542 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/admin_toolshed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/async.py
--rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/authnz.py
--rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    52736 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13895 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    35404 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/history.py
--rw-r--r--   0 runner    (1001) docker     (127)    23206 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/shed_tool_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/tool_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    17605 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    35495 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    26314 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/fast_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/fast_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8801 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/_fetch_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11681 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    37884 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    33801 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    66380 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/invocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15473 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/library_folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/library_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)    11779 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6179 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     6492 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/quotas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/storage_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/tool_shed_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    12897 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9990 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/workers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/openapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/openapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22450 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/openapi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4129 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/buildapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/home.py
--rw-r--r--   0 runner    (1001) docker     (127)    46718 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/fast_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/reports/fast_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/galaxy/webapps/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22878 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24617 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-02-22 03:57:10.000000 galaxy-web-apps-23.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-22 03:50:43.000000 galaxy-web-apps-23.2.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    31959 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    34337 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.916463 galaxy-web-apps-24.0.0/galaxy/datatypes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.916463 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/biom/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/biom/biom_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/icn3d/icn3d_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.928464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/image/avivator.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/intermine/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/intermine/intermine_simple.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/iobio/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/minerva/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/minerva/tabular.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.932464 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/trackhub.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63303 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.936464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/erricon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    20770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/formatHelp.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.940464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      752 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete_tag_icon_gray.png
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/dw.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.944464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   134808 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   165742 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   444379 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   165548 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    98024 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    77160 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.956464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      516 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      553 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-090.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      403 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bug.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      436 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chart.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      490 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      493 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      375 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/control-270.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      555 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-small-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      476 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      603 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      613 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/exclamation.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      621 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/external.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      536 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/eye.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      721 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer.png
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/information-white.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      566 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      664 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-left.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      736 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      758 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/navigation.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      309 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/pencil-small.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-circle.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/sticky-note-text.png
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag--plus.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      714 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag-label.png
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tags.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-bw.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      448 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1243 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      454 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050.png
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/hatch-fade-023858.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_grey.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_grey.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_error.png
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_ok.png
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_queued.png
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history_down_arrow.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history_up_arrow.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_lrg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_sml.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_large_white_bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_small_white_bg.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.960464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    11787 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/interval2maf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/openid-16x16.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_empty.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_error.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_ok.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_queued.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/square_running.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      815 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/star.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tool_menu_down_arrow.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/
+-rw-r--r--   0 runner    (1001) docker     (127)   257713 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    81633 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    72821 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    92949 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   108978 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   109459 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/
+-rw-r--r--   0 runner    (1001) docker     (127)    33141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23673 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.964464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/block.png
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/close_btn.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/diag_bg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/go_btn.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/handle-left.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/handle-right.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/pan_left.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/pan_right.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/show_history.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_in.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_in_full.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_out.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/zoom_out_full.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/up.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/draggable_horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/draggable_vertical.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_left.png
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_left_inv.png
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_right.png
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/visualization/strand_right_inv.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/incompatible-browser.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.968464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/findcluster.png
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/circster.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_running.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_upload.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4046 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4041 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      570 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/loading.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9902 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)      842 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)      844 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/embed_item.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/history.css
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/info_icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.972464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_flat_75_ffffff_40x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      144 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      111 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      119 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5355 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4369 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20147 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery.rating.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/library.css
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/masthead.css
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/ok_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/question-octagon-frame.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/reports.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31536 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-fugue.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-buttons.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-states.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/trackster.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.920464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-model.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/test-file.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.976464 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-model.js
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/user_disabled.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/static/welcome.html.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/base_panels.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/embed_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/galaxy_client_app.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/js-app.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)     8033 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base_async.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/message.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/no_access.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     8698 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/page_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/refresh_frames.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/slug_editing_js.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/sorting_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/spark_base.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tagging_common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tool_shed_rating.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.980464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/base_panels.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     8219 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/index.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/job_info.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4641 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/run_stats.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/system.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.924464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/
+-rw-r--r--   0 runner    (1001) docker     (127)    57351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako
+-rw-r--r--   0 runner    (1001) docker     (127)    51314 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/base/webapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:49.988464 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.004465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cbv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12759 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloudauthz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4936 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18059 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dynamic_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/extended_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/genomes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28672 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39822 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22023 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22961 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38850 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10414 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10566 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/roles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4090 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/sanitize_allow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_shed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23930 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/toolshed.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49922 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16087 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71507 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41693 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/buildapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.008465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51510 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin_toolshed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10677 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/authnz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10622 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52721 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15655 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/shed_tool_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tool_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17575 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20164 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/_fetch_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39171 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34805 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66849 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11086 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/invocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15421 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12572 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11795 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/quotas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/storage_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tool_shed_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12829 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11225 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/workers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/openapi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.012465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/buildapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4387 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/home.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46704 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9351 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9583 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17898 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/galaxy/webapps/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    34337 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24368 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:46:49.000000 galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-03 02:46:50.016465 galaxy-web-apps-24.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 02:43:42.000000 galaxy-web-apps-24.0.0/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `galaxy-web-apps-23.2.1/HISTORY.rst` & `galaxy-web-apps-24.0.0/HISTORY.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,92 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* tus wants a json response from v2.0.0 by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17246 <https://github.com/galaxyproject/galaxy/pull/17246>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Associate default history with session when creating a new session by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17557 <https://github.com/galaxyproject/galaxy/pull/17557>`_
+* Fix tool shed webapp by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17597 <https://github.com/galaxyproject/galaxy/pull/17597>`_
+* Don't call ``get_or_create_default_history()`` twice for invalidated sessions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17613 <https://github.com/galaxyproject/galaxy/pull/17613>`_
+* Fix tool panel workflow and favorites button bugs by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17634 <https://github.com/galaxyproject/galaxy/pull/17634>`_
+* Fix DataResult type by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17639 <https://github.com/galaxyproject/galaxy/pull/17639>`_
+* Prevent 500 for anon /api/invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17640 <https://github.com/galaxyproject/galaxy/pull/17640>`_
+* Don't fail for anon /api/users request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17645 <https://github.com/galaxyproject/galaxy/pull/17645>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Handle missing indexer for a dataset by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17736 <https://github.com/galaxyproject/galaxy/pull/17736>`_
+* Don't require history to calculate anon disk usage by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17765 <https://github.com/galaxyproject/galaxy/pull/17765>`_
+* Fix anon user values again by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17772 <https://github.com/galaxyproject/galaxy/pull/17772>`_
+* Fix new default history creation when in remote or single user mode by `@dannon <https://github.com/dannon>`_ in `#17796 <https://github.com/galaxyproject/galaxy/pull/17796>`_
+* Return published histories first in display_by_username_and_slug by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17808 <https://github.com/galaxyproject/galaxy/pull/17808>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Migrate dataset extra files store to Pinia by `@davelopez <https://github.com/davelopez>`_ in `#17145 <https://github.com/galaxyproject/galaxy/pull/17145>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Remove legacy tool versions list from admin panel by `@guerler <https://github.com/guerler>`_ in `#17155 <https://github.com/galaxyproject/galaxy/pull/17155>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Drop fastapi-utils.InferringRouter in favor of fastapi.APIRouter  by `@jdavcs <https://github.com/jdavcs>`_ in `#17184 <https://github.com/galaxyproject/galaxy/pull/17184>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Refactor two of the missing invocation routes to FastAPI by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17237 <https://github.com/galaxyproject/galaxy/pull/17237>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Fix any type for tool_data_file_path by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17293 <https://github.com/galaxyproject/galaxy/pull/17293>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Replaces Trackster Grids with Data Dialog, Removes Phyloviz, Circster and Sweepster by `@guerler <https://github.com/guerler>`_ in `#17415 <https://github.com/galaxyproject/galaxy/pull/17415>`_
+* Removes outdated Grid controller and backbone modules by `@guerler <https://github.com/guerler>`_ in `#17434 <https://github.com/galaxyproject/galaxy/pull/17434>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Modernize bits and pieces of storage display by `@jmchilton <https://github.com/jmchilton>`_ in `#17436 <https://github.com/galaxyproject/galaxy/pull/17436>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* Removes legacy history xml makos by `@guerler <https://github.com/guerler>`_ in `#17505 <https://github.com/galaxyproject/galaxy/pull/17505>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Links to individual invocations. by `@jmchilton <https://github.com/jmchilton>`_ in `#17566 <https://github.com/galaxyproject/galaxy/pull/17566>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-23.2.1/LICENSE` & `galaxy-web-apps-24.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/PKG-INFO` & `galaxy-web-apps-24.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-web-apps
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web apps
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-app
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-job-execution
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util[jstree,template]
+Requires-Dist: galaxy-web-framework
+Requires-Dist: galaxy-web-stack
+Requires-Dist: a2wsgi
+Requires-Dist: apispec
+Requires-Dist: Babel
+Requires-Dist: Cheetah3
+Requires-Dist: fastapi>=0.101.0
+Requires-Dist: gunicorn
+Requires-Dist: gxformat2
+Requires-Dist: importlib-resources; python_version < "3.9"
+Requires-Dist: Mako
+Requires-Dist: MarkupSafe
+Requires-Dist: mercurial
+Requires-Dist: Paste
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: PyJWT
+Requires-Dist: python-dateutil
+Requires-Dist: python-multipart
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: Routes
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: sqlalchemy-migrate
+Requires-Dist: starlette
+Requires-Dist: starlette-context
+Requires-Dist: tuswsgi
+Requires-Dist: typing-extensions
+Requires-Dist: uvicorn
+Requires-Dist: uvloop
+Requires-Dist: WebOb
+Requires-Dist: Whoosh
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-apps.svg
    :target: https://pypi.python.org/pypi/galaxy-web-apps/
 
 
 Overview
@@ -42,14 +78,93 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* tus wants a json response from v2.0.0 by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17246 <https://github.com/galaxyproject/galaxy/pull/17246>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Associate default history with session when creating a new session by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17557 <https://github.com/galaxyproject/galaxy/pull/17557>`_
+* Fix tool shed webapp by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17597 <https://github.com/galaxyproject/galaxy/pull/17597>`_
+* Don't call ``get_or_create_default_history()`` twice for invalidated sessions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17613 <https://github.com/galaxyproject/galaxy/pull/17613>`_
+* Fix tool panel workflow and favorites button bugs by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17634 <https://github.com/galaxyproject/galaxy/pull/17634>`_
+* Fix DataResult type by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17639 <https://github.com/galaxyproject/galaxy/pull/17639>`_
+* Prevent 500 for anon /api/invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17640 <https://github.com/galaxyproject/galaxy/pull/17640>`_
+* Don't fail for anon /api/users request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17645 <https://github.com/galaxyproject/galaxy/pull/17645>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Handle missing indexer for a dataset by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17736 <https://github.com/galaxyproject/galaxy/pull/17736>`_
+* Don't require history to calculate anon disk usage by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17765 <https://github.com/galaxyproject/galaxy/pull/17765>`_
+* Fix anon user values again by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17772 <https://github.com/galaxyproject/galaxy/pull/17772>`_
+* Fix new default history creation when in remote or single user mode by `@dannon <https://github.com/dannon>`_ in `#17796 <https://github.com/galaxyproject/galaxy/pull/17796>`_
+* Return published histories first in display_by_username_and_slug by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17808 <https://github.com/galaxyproject/galaxy/pull/17808>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Migrate dataset extra files store to Pinia by `@davelopez <https://github.com/davelopez>`_ in `#17145 <https://github.com/galaxyproject/galaxy/pull/17145>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Remove legacy tool versions list from admin panel by `@guerler <https://github.com/guerler>`_ in `#17155 <https://github.com/galaxyproject/galaxy/pull/17155>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Drop fastapi-utils.InferringRouter in favor of fastapi.APIRouter  by `@jdavcs <https://github.com/jdavcs>`_ in `#17184 <https://github.com/galaxyproject/galaxy/pull/17184>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Refactor two of the missing invocation routes to FastAPI by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17237 <https://github.com/galaxyproject/galaxy/pull/17237>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Fix any type for tool_data_file_path by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17293 <https://github.com/galaxyproject/galaxy/pull/17293>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Replaces Trackster Grids with Data Dialog, Removes Phyloviz, Circster and Sweepster by `@guerler <https://github.com/guerler>`_ in `#17415 <https://github.com/galaxyproject/galaxy/pull/17415>`_
+* Removes outdated Grid controller and backbone modules by `@guerler <https://github.com/guerler>`_ in `#17434 <https://github.com/galaxyproject/galaxy/pull/17434>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Modernize bits and pieces of storage display by `@jmchilton <https://github.com/jmchilton>`_ in `#17436 <https://github.com/galaxyproject/galaxy/pull/17436>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* Removes legacy history xml makos by `@guerler <https://github.com/guerler>`_ in `#17505 <https://github.com/galaxyproject/galaxy/pull/17505>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Links to individual invocations. by `@jmchilton <https://github.com/jmchilton>`_ in `#17566 <https://github.com/galaxyproject/galaxy/pull/17566>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ensembl/ensembl_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/gbrowse/gbrowse_wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bam.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bb.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bb.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bedgraph.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/bigwig.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/gtf.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/gtf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igb/wig.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igb/wig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/bam.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/bigwig.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/genbank.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genbank.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/genome_fasta.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/gff.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/gff.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/igv/vcf.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/igv/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/rviewer/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bam.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bam.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigbed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/bigwig.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/interval_as_bed.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/maf_customtrack.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml` & `galaxy-web-apps-24.0.0/galaxy/datatypes/display_applications/configs/ucsc/vcf.xml`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/api.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,19 +15,17 @@
     FileResponse,
     Response,
 )
 from starlette_context.middleware import RawContextMiddleware
 from starlette_context.plugins import RequestIdPlugin
 
 from galaxy.exceptions import MessageException
+from galaxy.exceptions.utils import api_error_to_dict
 from galaxy.web.framework.base import walk_controller_modules
-from galaxy.web.framework.decorators import (
-    api_error_message,
-    validation_error_to_message_exception,
-)
+from galaxy.web.framework.decorators import validation_error_to_message_exception
 
 if typing.TYPE_CHECKING:
     from starlette.background import BackgroundTask
     from starlette.types import (
         Receive,
         Scope,
         Send,
@@ -57,15 +55,14 @@
 class GalaxyFileResponse(FileResponse):
     """
     Augments starlette FileResponse with x-accel-redirect/x-sendfile and byte-range handling.
     """
 
     nginx_x_accel_redirect_base: typing.Optional[str] = None
     apache_xsendfile: typing.Optional[bool] = None
-    send_header_only: bool
 
     def __init__(
         self,
         path: typing.Union[str, "os.PathLike[str]"],
         status_code: int = 200,
         headers: typing.Optional[typing.Mapping[str, str]] = None,
         media_type: typing.Optional[str] = None,
@@ -75,40 +72,42 @@
         method: typing.Optional[str] = None,
         content_disposition_type: str = "attachment",
     ) -> None:
         super().__init__(
             path, status_code, headers, media_type, background, filename, stat_result, method, content_disposition_type
         )
         self.headers["accept-ranges"] = "bytes"
-        send_header_only = self.nginx_x_accel_redirect_base or self.apache_xsendfile
+        self.xsendfile = self.nginx_x_accel_redirect_base or self.apache_xsendfile
         if self.nginx_x_accel_redirect_base:
             self.headers["x-accel-redirect"] = self.nginx_x_accel_redirect_base + os.path.abspath(path)
         elif self.apache_xsendfile:
             self.headers["x-sendfile"] = os.path.abspath(path)
-        if not self.send_header_only and send_header_only:
-            # Not a head request, but nginx_x_accel_redirect_base / send_header_only, we don't send a body
-            self.send_header_only = True
-            self.headers["content-length"] = "0"
 
     async def __call__(self, scope: "Scope", receive: "Receive", send: "Send") -> None:
         if self.stat_result is None:
             try:
                 stat_result = await anyio.to_thread.run_sync(os.stat, self.path)
                 self.set_stat_headers(stat_result)
             except FileNotFoundError:
                 raise RuntimeError(f"File at path {self.path} does not exist.")
             else:
                 mode = stat_result.st_mode
                 if not stat.S_ISREG(mode):
                     raise RuntimeError(f"File at path {self.path} is not a file.")
 
         # This is where we diverge from the superclass, this adds support for byte range requests
+        is_head_request = scope["method"].upper() == "HEAD"
+        if not is_head_request and self.xsendfile:
+            # Not a head request, but nginx_x_accel_redirect_base / send_header_only, we don't send a body
+            self.headers["content-length"] = "0"
+        send_header_only = self.xsendfile or is_head_request
+
         start = 0
         end = stat_result.st_size - 1
-        if not self.send_header_only:
+        if not send_header_only:
             http_range = ""
             for key, value in scope["headers"]:
                 if key == b"range":
                     http_range = value.decode("latin-1")
                     start, end = _get_range_header(http_range, stat_result.st_size)
                     self.headers["content-length"] = str(end - start + 1)
                     self.headers["content-range"] = f"bytes {start}-{end}/{stat_result.st_size}"
@@ -118,15 +117,15 @@
         await send(
             {
                 "type": "http.response.start",
                 "status": self.status_code,
                 "headers": self.raw_headers,
             }
         )
-        if self.send_header_only:
+        if send_header_only:
             await send({"type": "http.response.body", "body": b"", "more_body": False})
         else:
             # This also diverges from the superclass by seeking to start and limiting to end if handling byte range requests
             async with await anyio.open_file(self.path, mode="rb") as file:
                 more_body = True
                 if start:
                     await file.seek(start)
@@ -155,18 +154,17 @@
 def add_sentry_middleware(app: FastAPI) -> None:
     from sentry_sdk.integrations.asgi import SentryAsgiMiddleware
 
     app.add_middleware(SentryAsgiMiddleware)
 
 
 def get_error_response_for_request(request: Request, exc: MessageException) -> JSONResponse:
-    error_dict = api_error_message(None, exception=exc)
+    error_dict = api_error_to_dict(exception=exc)
     status_code = exc.status_code
-    path = request.url.path
-    if "ga4gh" in path:
+    if "ga4gh" in (path := request.url.path):
         # When serving GA4GH APIs use limited exceptions to conform their expected
         # error schema. Tailored to DRS currently.
         message = error_dict["err_msg"]
         if "drs" in path:
             content = {"status_code": status_code, "msg": message}
         elif "trs" in path:
             content = {"code": status_code, "message": message}
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/controller.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Contains functionality needed in every web interface
 """
+
 import logging
 from typing import (
     Any,
     Callable,
     Optional,
 )
 
@@ -221,16 +222,15 @@
         keys = kwd.get("keys")
         if isinstance(keys, str):
             keys = keys.split(",")
         return dict(view=view, keys=keys, default_view=default_view)
 
     # TODO: this will be replaced by lib.galaxy.schema.FilterQueryParams.build_order_by
     def _parse_order_by(self, manager, order_by_string):
-        ORDER_BY_SEP_CHAR = ","
-        if ORDER_BY_SEP_CHAR in order_by_string:
+        if (ORDER_BY_SEP_CHAR := ",") in order_by_string:
             return [manager.parse_order_by(o) for o in order_by_string.split(ORDER_BY_SEP_CHAR)]
         return manager.parse_order_by(order_by_string)
 
 
 class JSAppLauncher(BaseUIController):
     """
     A controller that launches JavaScript web applications.
@@ -1065,16 +1065,15 @@
         query_dbkey = dataset.dbkey
         if query_dbkey == "?":
             query_dbkey = dbkey
         chroms_info = self.app.genomes.chroms(trans, dbkey=query_dbkey)
 
         # If there are no messages (messages indicate data is not ready/available), get data.
         messages_list = [data_source_dict["message"] for data_source_dict in data_sources.values()]
-        message = self._get_highest_priority_msg(messages_list)
-        if message:
+        if message := self._get_highest_priority_msg(messages_list):
             rval = message
         else:
             # HACK: chromatin interactions tracks use data as source.
             source = "index"
             if isinstance(dataset.datatype, ChromatinInteractions):
                 source = "data"
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/erricon.ico` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/erricon.ico`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/favicon.ico` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/favicon.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/favicon.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/formatHelp.html` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/formatHelp.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/delete.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/delete.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/dw.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/dw.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/FontAwesome.otf` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/application-dock-270.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/application-dock-270.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-000-small-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-090.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-090.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-circle.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-resize-090-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-split.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-split.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-270-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/arrow-transition-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/block--plus-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/block--plus.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/block--plus.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bookmarks.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bookmarks.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/bug.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/bug.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/chevron-expand-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-button.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-button.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-circle.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/cross-small-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/cross-small-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/disk--arrow.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/disk--arrow.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/exclamation.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/exclamation.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/external.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/external.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/eye.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/eye.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/gear-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/gear.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/gear.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/globe-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/globe.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/globe.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/hammer-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/hammer.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/hammer.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/information-white.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/information-white.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layer-transparent.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layer-transparent.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/layers-stack.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/layers-stack.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-left.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-left.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom-out.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/magnifier-zoom.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/navigation.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/navigation.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-button-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-button.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-button.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/plus-circle.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/plus-circle.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/sticky-note-text.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/sticky-note-text.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tag--plus.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag--plus.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tag-label.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tag-label.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/tags.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/tags.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toggle-expand.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toggle-expand.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/toolbox-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/toolbox-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/fugue/ui-slider-050-bw.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/delete_icon.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/delete_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/eye_icon.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/eye_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-buttons/pencil_icon_dark.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history-states/data_queued.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history-states/data_queued.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/history.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/history.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_error_lrg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_error_sml.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_error_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_info_lrg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_info_sml.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_info_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_success_lrg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_success_sml.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_success_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_warning_lrg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_lrg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/icon_warning_sml.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/icon_warning_sml.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/loading_large_white_bg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_large_white_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/loading_small_white_bg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/loading_small_white_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/maf_icons/interval2maf.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/interval2maf.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/maf_icons/stitchMaf.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/rgWebLogo3_test.jpg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/star.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/star.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/build_list.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_empty.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/filter_error.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/flatten.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/unzip.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/collection_ops/zip.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/first_matrix_generator_example_file.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tools/lda/second_matrix_generator_example_file.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/block.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/block.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/diag_bg.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/diag_bg.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/tracks/show_history.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/tracks/show_history.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/up.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/up.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/images/yui/rel_interstitial_loading.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/incompatible-browser.html` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/incompatible-browser.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/patmat/findcluster.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/patmat/findcluster.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/data_running.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_running.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/data_upload.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/data_upload.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons-rtl.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/icons.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/icons.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/loading.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/loading.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/ui.dynatree.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline-rtl.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/dynatree_skin/vline.gif` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/dynatree_skin/vline.gif`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/embed_item.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/embed_item.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/info_icon.svg` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/info_icon.svg`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery-ui/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/jquery.rating.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/jquery.rating.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/library.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/library.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/masthead.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/masthead.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/question-octagon-frame.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/question-octagon-frame.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/reports.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/reports.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-fugue.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-fugue.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-history-buttons.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-buttons.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/sprite-history-states.png` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/sprite-history-states.png`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/style/trackster.css` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/style/trackster.css`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-detail-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-list-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/mvc/groups/group-listrow-view.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/maps/toolshed.groups.js.map`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-detail-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-list-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/mvc/groups/group-listrow-view.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/toolshed/scripts/toolshed.groups.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/user_disabled.html` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/user_disabled.html`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/static/welcome.html.sample` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/static/welcome.html.sample`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/base/base_panels.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base/base_panels.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/display_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/display_common.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/display_common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/embed_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/embed_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/galaxy_client_app.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/galaxy_client_app.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/js-app.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/js-app.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/legacy/grid_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/legacy/grid_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/message.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/message.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/no_access.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/no_access.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/page_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/page_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/refresh_frames.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/refresh_frames.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/slug_editing_js.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/slug_editing_js.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/sorting_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/sorting_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/spark_base.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/spark_base.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/tagging_common.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tagging_common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/tool_shed_rating.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/tool_shed_rating.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
                         encoded_id = trans.security.encode_id(data.id)
                         input_id = "%s|%s" % ( data.history_content_type, encoded_id )
                         if input_id in source_content_ids:
                             checked = " checked='checked'"
                     %>
                     <div class="form-row">
                         <input type="checkbox" name="source_content_ids" id="${input_id}" value="${input_id}"${checked}/>
-                        <label for="${input_id}" style="display: inline;font-weight:normal;"> ${data.hid}: ${h.to_unicode(data.name) | h}</label>
+                        <label for="${input_id}" style="display: inline;font-weight:normal;"> ${data.hid}: ${util.unicodify(data.name) | h}</label>
                     </div>
                 %endfor
                 %if not has_source_contents:
                     <div class="form-row">This history has no datasets.</div>
                 %endif
             </div>
         </div>
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/base_panels.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/base_panels.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/dataset_info.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/history_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/index.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/index.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/job_info.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/job_info.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_errors_per_tool.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_by_user_and_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_month_in_error.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_tool.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_per_user_by_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_specified_month_in_error.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_tool_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/jobs_user_per_month_by_destination.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_date.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/registered_users_specified_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/run_stats.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/run_stats.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/system.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/system.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_error_messages.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tool_execution_time_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/tools_and_job_state_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_last_access_date.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/users_user_disk_usage.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_month_all.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_user.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_per_workflow.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/reports/workflows_user_per_month.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/common/common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/templates/webapps/tool_shed/repository/common.mako`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/base/webapp.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/base/webapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+
 import datetime
 import inspect
 import logging
 import os
 import re
 import socket
 import time
@@ -33,15 +34,18 @@
     MalformedId,
     MessageException,
     RequestParameterMissingException,
 )
 from galaxy.managers import context
 from galaxy.managers.session import GalaxySessionManager
 from galaxy.managers.users import UserManager
-from galaxy.model.base import transaction
+from galaxy.model.base import (
+    ensure_object_added_to_session,
+    transaction,
+)
 from galaxy.structured_app import (
     BasicSharedApp,
     MinimalApp,
 )
 from galaxy.util import (
     asbool,
     safe_makedirs,
@@ -305,16 +309,15 @@
         self._app = app
         self.webapp = webapp
         self.user_manager = app[UserManager]
         self.session_manager = app[GalaxySessionManager]
         super().__init__(environ)
         config = self.app.config
         self.debug = asbool(config.get("debug", False))
-        x_frame_options = getattr(config, "x_frame_options", None)
-        if x_frame_options:
+        if x_frame_options := getattr(config, "x_frame_options", None):
             self.response.headers["X-Frame-Options"] = x_frame_options
         # Flag indicating whether we are in workflow building mode (means
         # that the current history should not be used for parameter values
         # and such).
         self.workflow_building_mode = False
         self.__user = None
         self.galaxy_session = None
@@ -528,14 +531,18 @@
         if self.app.config.cookie_domain is not None:
             self.response.cookies[name]["domain"] = self.app.config.cookie_domain
 
     def _authenticate_api(self, session_cookie: str) -> Optional[str]:
         """
         Authenticate for the API via key or session (if available).
         """
+        oidc_access_token = self.request.headers.get("Authorization", None)
+        oidc_token_supplied = (
+            self.environ.get("is_api_request", False) and oidc_access_token and "Bearer " in oidc_access_token
+        )
         api_key = self.request.params.get("key", None) or self.request.headers.get("x-api-key", None)
         secure_id = self.get_cookie(name=session_cookie)
         api_key_supplied = self.environ.get("is_api_request", False) and api_key
         if api_key_supplied:
             # Sessionless API transaction, we just need to associate a user.
             try:
                 user = self.user_manager.by_api_key(api_key)
@@ -550,14 +557,22 @@
                 self._ensure_valid_session(session_cookie)
             except Exception:
                 log.exception(
                     "Exception during Session-based API authentication, this was most likely an attempt to use an anonymous cookie under remote authentication (so, no user), which we don't support."
                 )
                 self.user = None
                 self.galaxy_session = None
+        elif oidc_token_supplied:
+            # Sessionless API transaction with oidc token, we just need to associate a user.
+            oidc_access_token = oidc_access_token.replace("Bearer ", "")
+            try:
+                user = self.user_manager.by_oidc_access_token(oidc_access_token)
+            except AuthenticationFailed as e:
+                return str(e)
+            self.set_user(user)
         else:
             # Anonymous API interaction -- anything but @expose_api_anonymous will fail past here.
             self.user = None
             self.galaxy_session = None
         return None
 
     def _ensure_valid_session(self, session_cookie: str, create: bool = True) -> None:
@@ -649,27 +664,25 @@
         if galaxy_session is None:
             galaxy_session = self.__create_new_session(prev_galaxy_session, user_for_new_session)
             galaxy_session_requires_flush = True
             self.galaxy_session = galaxy_session
             self.__update_session_cookie(name=session_cookie)
         else:
             self.galaxy_session = galaxy_session
+            if self.webapp.name == "galaxy":
+                self.get_or_create_default_history()
         # Do we need to flush the session?
         if galaxy_session_requires_flush:
             self.sa_session.add(galaxy_session)
             # FIXME: If prev_session is a proper relation this would not
             #        be needed.
             if prev_galaxy_session:
                 self.sa_session.add(prev_galaxy_session)
             with transaction(self.sa_session):
                 self.sa_session.commit()
-        # If the old session was invalid, get a new (or existing default,
-        # unused) history with our new session
-        if invalidate_existing_session:
-            self.get_or_create_default_history()
 
     def _ensure_logged_in_user(self, session_cookie: str) -> None:
         # The value of session_cookie can be one of
         # 'galaxysession' or 'galaxycommunitysession'
         # Currently this method does nothing unless session_cookie is 'galaxysession'
         assert self.galaxy_session
         if session_cookie == "galaxysession" and self.galaxy_session.user is None:
@@ -797,18 +810,18 @@
         if (
             not history
             and users_last_session
             and users_last_session.current_history
             and not users_last_session.current_history.deleted
         ):
             history = users_last_session.current_history
-        elif not history:
-            history = self.get_history(create=True, most_recent=True)
         if history not in self.galaxy_session.histories:
             self.galaxy_session.add_history(history)
+        if not history:
+            history = self.new_history()
         if history.user is None:
             history.user = user
         self.galaxy_session.current_history = history
         if set_permissions:
             self.app.security_agent.history_set_default_permissions(
                 history, dataset=True, bypass_manage_permission=True
             )
@@ -911,40 +924,35 @@
 
     def get_or_create_default_history(self):
         """
         Gets or creates a default history and associates it with the current
         session.
         """
 
-        # There must be a user to fetch a default history.
-        if not self.galaxy_session.user:
-            return self.new_history()
-
-        # Look for default history that (a) has default name + is not deleted and
-        # (b) has no datasets. If suitable history found, use it; otherwise, create
-        # new history.
-        stmt = select(self.app.model.History).filter_by(
-            user=self.galaxy_session.user, name=self.app.model.History.default_name, deleted=False
-        )
-        unnamed_histories = self.sa_session.scalars(stmt)
-        default_history = None
-        for history in unnamed_histories:
-            if history.empty:
-                # Found suitable default history.
-                default_history = history
-                break
-
-        # Set or create history.
-        if default_history:
-            history = default_history
-            self.set_history(history)
-        else:
-            history = self.new_history()
+        # Just return the current history if one exists and is not deleted.
+        history = self.galaxy_session.current_history
+        if history and not history.deleted:
+            return history
 
-        return history
+        # Look for an existing history that has the default name, is not
+        # deleted, and is empty. If this exists, we associate it with the
+        # current session and return it.
+        user = self.galaxy_session.user
+        if user:
+            stmt = select(self.app.model.History).filter_by(
+                user=user, name=self.app.model.History.default_name, deleted=False
+            )
+            unnamed_histories = self.sa_session.scalars(stmt)
+            for history in unnamed_histories:
+                if history.empty:
+                    self.set_history(history)
+                    return history
+
+        # No suitable history found, create a new one.
+        return self.new_history()
 
     def get_most_recent_history(self):
         """
         Gets the most recently updated history.
         """
         # There must be a user to fetch histories, and without a user we have
         # no recent history.
@@ -1116,14 +1124,15 @@
     )
     if prev_galaxy_session:
         # Invalidated an existing session for some reason, keep track
         galaxy_session.prev_session_id = prev_galaxy_session.id
     if user_for_new_session:
         # The new session should be associated with the user
         galaxy_session.user = user_for_new_session
+        ensure_object_added_to_session(galaxy_session, object_in_session=user_for_new_session)
     return galaxy_session
 
 
 def default_url_path(path):
     return os.path.abspath(os.path.join(os.path.dirname(__file__), path))
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/__init__.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 """
 This module *does not* contain API routes. It exclusively contains dependencies to be used in FastAPI routes
 """
+
 import inspect
 from enum import Enum
 from string import Template
 from typing import (
     Any,
     AsyncGenerator,
     cast,
-    MutableMapping,
     NamedTuple,
     Optional,
     Tuple,
     Type,
     TypeVar,
 )
 from urllib.parse import (
     urlencode,
     urljoin,
 )
 
 from a2wsgi.wsgi import build_environ
+from a2wsgi.wsgi_typing import Environ
 from fastapi import (
+    APIRouter,
     Form,
     Header,
     Query,
     Request,
     Response,
     Security,
 )
 from fastapi.exceptions import RequestValidationError
 from fastapi.params import Depends
 from fastapi.routing import APIRoute
 from fastapi.security import (
     APIKeyCookie,
     APIKeyHeader,
     APIKeyQuery,
+    HTTPAuthorizationCredentials,
+    HTTPBearer,
 )
-from fastapi_utils.cbv import cbv
-from fastapi_utils.inferring_router import InferringRouter
 from pydantic import ValidationError
 from pydantic.main import BaseModel
 from routes import (
     Mapper,
     request_config,
 )
 from starlette.datastructures import Headers
@@ -71,23 +73,25 @@
 from galaxy.managers.users import UserManager
 from galaxy.model import User
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.structured_app import StructuredApp
 from galaxy.web.framework.decorators import require_admin_message
 from galaxy.webapps.base.controller import BaseAPIController
+from galaxy.webapps.galaxy.api.cbv import cbv
 from galaxy.work.context import (
     GalaxyAbstractRequest,
     GalaxyAbstractResponse,
     SessionRequestContext,
 )
 
 api_key_query = APIKeyQuery(name="key", auto_error=False)
 api_key_header = APIKeyHeader(name="x-api-key", auto_error=False)
 api_key_cookie = APIKeyCookie(name="galaxysession", auto_error=False)
+api_bearer_token = HTTPBearer(auto_error=False)
 
 
 def get_app() -> StructuredApp:
     return cast(StructuredApp, galaxy_app.app)
 
 
 async def get_app_with_request_session() -> AsyncGenerator[StructuredApp, None]:
@@ -139,27 +143,31 @@
     return None
 
 
 def get_api_user(
     user_manager: UserManager = depends(UserManager),
     key: str = Security(api_key_query),
     x_api_key: str = Security(api_key_header),
+    bearer_token: HTTPAuthorizationCredentials = Security(api_bearer_token),
     run_as: Optional[DecodedDatabaseIdField] = Header(
         default=None,
         title="Run as User",
         description=(
             "The user ID that will be used to effectively make this API call. "
             "Only admins and designated users can make API calls on behalf of other users."
         ),
     ),
 ) -> Optional[User]:
     api_key = key or x_api_key
-    if not api_key:
+    if api_key:
+        user = user_manager.by_api_key(api_key=api_key)
+    elif bearer_token:
+        user = user_manager.by_oidc_access_token(access_token=bearer_token.credentials)
+    else:
         return None
-    user = user_manager.by_api_key(api_key=api_key)
     if run_as:
         if user_manager.user_can_do_run_as(user):
             return user_manager.by_id(run_as)
         else:
             raise UserCannotRunAsException
     return user
 
@@ -205,35 +213,34 @@
     Implements the GalaxyAbstractRequest interface to provide access to some properties
     of the request commonly used."""
 
     __request: Request
 
     def __init__(self, request: Request):
         self.__request = request
-        self.__environ: Optional[MutableMapping[str, Any]] = None
+        self.__environ: Optional[Environ] = None
 
     @property
     def base(self) -> str:
         return str(self.__request.base_url)
 
     @property
     def url_path(self) -> str:
         scope = self.__request.scope
-        root_path = scope.get("root_path")
         url = self.base
-        if root_path:
+        if root_path := scope.get("root_path"):
             url = urljoin(url, root_path)
         return url
 
     @property
     def host(self) -> str:
         return self.__request.base_url.netloc
 
     @property
-    def environ(self) -> MutableMapping[str, Any]:
+    def environ(self) -> Environ:
         """
         Fallback WSGI environ.
 
         This is not a full environ, there is no body. This is only meant to make routes.url_for work.
         """
         if self.__environ is None:
             self.__environ = build_environ(self.__request.scope, None)  # type: ignore[arg-type]
@@ -325,16 +332,15 @@
     app: StructuredApp = DependsOnApp,
     user=cast(Optional[User], Depends(get_user)),
     galaxy_session=cast(Optional[model.GalaxySession], Depends(get_session)),
 ) -> SessionRequestContext:
     url_builder = UrlBuilder(request)
     galaxy_request = GalaxyASGIRequest(request)
     galaxy_response = GalaxyASGIResponse(response)
-    mapper = getattr(app, "legacy_mapper", None)
-    if mapper:
+    if mapper := getattr(app, "legacy_mapper", None):
         fix_url_for(mapper, galaxy_request)
     return SessionRequestContext(
         app=app,
         user=user,
         galaxy_session=galaxy_session,
         url_builder=url_builder,
         request=galaxy_request,
@@ -366,16 +372,16 @@
     post = "POST"
     put = "PUT"
     patch = "PATCH"
     delete = "DELETE"
     options = "OPTIONS"
 
 
-class FrameworkRouter(InferringRouter):
-    """A FastAPI Inferring Router tailored to Galaxy."""
+class FrameworkRouter(APIRouter):
+    """A FastAPI Router tailored to Galaxy."""
 
     admin_user_dependency: Any
 
     def wrap_with_alias(self, verb: RestVerb, *args, alias: Optional[str] = None, **kwd):
         """
         Wraps FastAPI methods with additional alias keyword and require_admin handling.
 
@@ -453,14 +459,20 @@
         require_admin = kwd.pop("require_admin", False)
         if require_admin:
             if "dependencies" in kwd:
                 kwd["dependencies"].append(self.admin_user_dependency)
             else:
                 kwd["dependencies"] = [self.admin_user_dependency]
 
+        public = kwd.pop("public", False)
+        openapi_extra = kwd.pop("openapi_extra", {})
+        if public:
+            openapi_extra["security"] = []
+        if openapi_extra:
+            kwd["openapi_extra"] = openapi_extra
         return kwd
 
     @property
     def cbv(self):
         """Short-hand for frequently used Galaxy-pattern of FastAPI class based views.
 
         Creates a class-based view for for this router, for more information see:
@@ -504,26 +516,26 @@
     Adds an as_form class method to decorated models. The as_form class method
     can be used with FastAPI endpoints.
 
     See https://github.com/tiangolo/fastapi/issues/2387#issuecomment-731662551
     """
     new_params = [
         inspect.Parameter(
-            field.alias,
+            field_name,
             inspect.Parameter.POSITIONAL_ONLY,
-            default=(Form(field.default) if not field.required else Form(...)),
+            default=(Form(field.default) if not field.is_required() else Form(...)),
         )
-        for field in cls.__fields__.values()
+        for field_name, field in cls.model_fields.items()
     ]
 
     async def _as_form(**data):
         try:
             return cls(**data)
         except ValidationError as e:
-            raise RequestValidationError(e.raw_errors)
+            raise RequestValidationError(e.errors())
 
     sig = inspect.signature(_as_form)
     sig = sig.replace(parameters=new_params)
     _as_form.__signature__ = sig  # type: ignore[attr-defined]
     cls.as_form = _as_form  # type: ignore[attr-defined]
     return cls
 
@@ -570,16 +582,15 @@
     tag: str
     description: str
     alias: Optional[str] = None
     admin_only: bool = False
 
     def as_markdown(self):
         desc = self.description
-        alias = self.alias
-        if alias:
+        if alias := self.alias:
             desc += f" (The tag `{alias}` can be used a short hand alias for this tag to filter on this attribute.)"
         if self.admin_only:
             desc += " This tag is only available for requests using admin keys and/or sessions."
         return f"`{self.tag}`\n: {desc}"
 
 
 def search_query_param(model_name: str, tags: list, free_text_fields: list) -> Optional[str]:
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/annotations.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/annotations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on annotations.
 """
+
 import logging
 from abc import abstractmethod
 
 from galaxy import (
     exceptions,
     managers,
 )
@@ -24,40 +25,37 @@
 
 class BaseAnnotationsController(BaseGalaxyAPIController, UsesStoredWorkflowMixin, UsesAnnotations):
     tagged_item_id: str
 
     @expose_api
     def index(self, trans: ProvidesHistoryContext, **kwd):
         idnum = kwd[self.tagged_item_id]
-        item = self._get_item_from_id(trans, idnum)
-        if item is not None:
+        if (item := self._get_item_from_id(trans, idnum)) is not None:
             return self.get_item_annotation_str(trans.sa_session, trans.user, item)
 
     @expose_api
     def create(self, trans: ProvidesHistoryContext, payload: dict, **kwd):
         if "text" not in payload:
             return ""
         idnum = kwd[self.tagged_item_id]
-        item = self._get_item_from_id(trans, idnum)
-        if item is not None:
+        if (item := self._get_item_from_id(trans, idnum)) is not None:
             new_annotation = payload.get("text")
             # TODO: sanitize on display not entry
             new_annotation = sanitize_html(new_annotation)
 
             self.add_item_annotation(trans.sa_session, trans.user, item, new_annotation)
             with transaction(trans.sa_session):
                 trans.sa_session.commit()
             return new_annotation
         return ""
 
     @expose_api
     def delete(self, trans: ProvidesHistoryContext, **kwd):
         idnum = kwd[self.tagged_item_id]
-        item = self._get_item_from_id(trans, idnum)
-        if item is not None:
+        if (item := self._get_item_from_id(trans, idnum)) is not None:
             return self.delete_item_annotation(trans.sa_session, trans.user, item)
 
     @expose_api
     def undelete(self, trans: ProvidesHistoryContext, **kwd):
         raise exceptions.NotImplemented()
 
     @abstractmethod
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/authenticate.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/authenticate.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 .. code-block:: json
 
     {
         "api_key": "baa4d6e3a156d3033f05736255f195f9"
     }
 
 """
+
 from fastapi import Request
 
 from galaxy.web import expose_api_anonymous_and_sessionless
 from galaxy.webapps.base.webapp import GalaxyWebTransaction
 from galaxy.webapps.galaxy.services.authenticate import (
     APIKeyResponse,
     AuthenticationService,
@@ -55,10 +56,11 @@
     authentication_service: AuthenticationService = depends(AuthenticationService)
 
     @router.get(
         "/api/authenticate/baseauth",
         summary="Returns returns an API key for authenticated user based on BaseAuth headers.",
     )
     def get_api_key(self, request: Request) -> APIKeyResponse:
+        # TODO: use fastapi.security mechanism
         authorization = request.headers.get("Authorization")
         auth = {"HTTP_AUTHORIZATION": authorization}
         return self.authentication_service.get_api_key(auth, request)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/cloud.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """
 API operations on Cloud-based storages, such as Amazon Simple Storage Service (S3).
 """
 
 import logging
 
-from fastapi import (
-    Body,
-    Response,
-    status,
-)
-from pydantic import Required
+from fastapi import Body
 
 from galaxy.managers.cloud import CloudManager
 from galaxy.managers.context import ProvidesHistoryContext
 from galaxy.managers.datasets import DatasetSerializer
 from galaxy.schema.cloud import (
     CloudDatasets,
     CloudDatasetsResponse,
     CloudObjects,
     DatasetSummaryList,
-    StatusCode,
 )
 from galaxy.webapps.galaxy.api import (
     depends,
     Router,
 )
 from . import DependsOnTrans
 
@@ -33,58 +27,45 @@
 
 
 @router.cbv
 class FastAPICloudController:
     cloud_manager: CloudManager = depends(CloudManager)
     datasets_serializer: DatasetSerializer = depends(DatasetSerializer)
 
-    @router.get(
-        "/api/cloud/storage",
-        summary="Lists cloud-based buckets (e.g., S3 bucket, Azure blob) user has defined. Is not yet implemented",
-        deprecated=True,
-    )
-    def index(
-        self,
-        response: Response,
-    ):
-        # TODO: This can be implemented leveraging PluggedMedia objects (part of the user-based object store project)
-        response.status_code = status.HTTP_501_NOT_IMPLEMENTED
-        return StatusCode(detail="Not yet implemented.", status=501)
-
     @router.post(
         "/api/cloud/storage/get",
         summary="Gets given objects from a given cloud-based bucket to a Galaxy history.",
         deprecated=True,
     )
     def get(
         self,
-        payload: CloudObjects = Body(default=Required),
+        payload: CloudObjects = Body(default=...),
         trans: ProvidesHistoryContext = DependsOnTrans,
     ) -> DatasetSummaryList:
         datasets = self.cloud_manager.get(
             trans=trans,
             history_id=payload.history_id,
             bucket_name=payload.bucket,
             objects=payload.objects,
             authz_id=payload.authz_id,
             input_args=payload.input_args,
         )
         rtv = []
         for dataset in datasets:
             rtv.append(self.datasets_serializer.serialize_to_view(dataset, view="summary"))
-        return DatasetSummaryList.construct(__root__=rtv)
+        return DatasetSummaryList.model_construct(root=rtv)
 
     @router.post(
         "/api/cloud/storage/send",
         summary="Sends given dataset(s) in a given history to a given cloud-based bucket.",
         deprecated=True,
     )
     def send(
         self,
-        payload: CloudDatasets = Body(default=Required),
+        payload: CloudDatasets = Body(default=...),
         trans: ProvidesHistoryContext = DependsOnTrans,
     ) -> CloudDatasetsResponse:
         log.info(
             msg="Received api/send request for `{}` datasets using authnz with id `{}`, and history `{}`."
             "".format(
                 "all the dataset in the given history" if not payload.dataset_ids else len(payload.dataset_ids),
                 payload.authz_id,
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/cloudauthz.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/cloudauthz.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/common.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,123 @@
 """This module contains utility functions shared across the api package."""
+
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Set,
 )
 
 from fastapi import (
+    Path,
     Query,
     Request,
 )
+from typing_extensions import Annotated
 
 from galaxy.schema import (
     FilterQueryParams,
     SerializationParams,
     ValueFilterQueryParams,
 )
+from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import UpdateDatasetPermissionsPayload
 from galaxy.util import listify
 
-SerializationViewQueryParam: Optional[str] = Query(
-    None,
-    title="View",
-    description="View to be passed to the serializer",
-)
+HistoryIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="History ID", description="The encoded database identifier of the History."),
+]
+
+HistoryDatasetIDPathParam = Annotated[
+    DecodedDatabaseIdField, Path(..., title="History Dataset ID", description="The ID of the History Dataset.")
+]
+
+
+HistoryItemIDPathParam = Annotated[
+    DecodedDatabaseIdField, Path(..., title="History Item ID", description="The ID of the item (`HDA`/`HDCA`)")
+]
+
+HistoryHDCAIDPathParam = Annotated[
+    DecodedDatabaseIdField, Path(..., title="History Dataset Collection ID", description="The ID of the `HDCA`.")
+]
+
+
+DatasetCollectionElementIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Dataset Collection Element ID", description="The encoded ID of the dataset collection element."),
+]
+
+
+UserIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="User ID", description="The ID of the user."),
+]
+
+
+GroupIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Group ID", description="The ID of the group."),
+]
+
+
+RoleIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Role ID", description="The ID of the role."),
+]
+
+
+LibraryIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Library ID", description="The ID of the Library."),
+]
+
+NotificationIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Notification ID", description="The ID of the Notification."),
+]
+
+
+PageIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Page ID", description="The ID of the Page."),
+]
+
+QuotaIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Quota ID", description="The ID of the Quota."),
+]
+
+SerializationViewQueryParam = Annotated[
+    Optional[str],
+    Query(
+        title="View",
+        description="View to be passed to the serializer",
+    ),
+]
 
 SerializationKeysQueryParam: Optional[str] = Query(
     None,
     title="Keys",
     description="Comma-separated list of keys to be passed to the serializer",
 )
 
 FilterQueryQueryParam: Optional[List[str]] = Query(
     default=None,
     title="Filter Query",
     description="Generally a property name to filter by followed by an (often optional) hyphen and operator string.",
-    example="create_time-gt",
+    examples=["create_time-gt"],
 )
 
 FilterValueQueryParam: Optional[List[str]] = Query(
     default=None,
     title="Filter Value",
     description="The value to filter by.",
-    example="2015-01-29",
+    examples=["2015-01-29"],
 )
 
 OffsetQueryParam: Optional[int] = Query(
     default=0,
     ge=0,
     title="Offset",
     description="Starts at the beginning skip the first ( offset - 1 ) items and begin returning at the Nth item",
@@ -80,15 +150,15 @@
     key_list = None
     if keys:
         key_list = keys.split(",")
     return SerializationParams(view=view, keys=key_list, default_view=default_view)
 
 
 def query_serialization_params(
-    view: Optional[str] = SerializationViewQueryParam,
+    view: SerializationViewQueryParam = None,
     keys: Optional[str] = SerializationKeysQueryParam,
 ) -> SerializationParams:
     return parse_serialization_params(view=view, keys=keys)
 
 
 def get_value_filter_query_params(
     q: Optional[List[str]] = FilterQueryQueryParam,
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/configuration.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/configuration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 API operations allowing clients to determine Galaxy instance's capabilities
 and configuration settings.
 """
+
 import logging
 from typing import (
     Any,
     Dict,
     List,
     Optional,
 )
 
 from fastapi import Path
 
 from galaxy.managers.configuration import ConfigurationManager
 from galaxy.managers.context import ProvidesUserContext
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.schema.schema import UserModel
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
 from galaxy.webapps.galaxy.api.common import (
@@ -34,14 +35,20 @@
 
 EncodedIdPathParam = Path(
     ...,
     title="Encoded id",
     description="Encoded id to be decoded",
 )
 
+DecodedIdPathParam = Path(
+    ...,
+    title="Decoded id",
+    description="Decoded id to be encoded",
+)
+
 
 @router.cbv
 class FastAPIConfiguration:
     configuration_manager: ConfigurationManager = depends(ConfigurationManager)
 
     @router.get(
         "/api/whoami",
@@ -56,28 +63,29 @@
         "/api/configuration",
         summary="Return an object containing exposable configuration settings",
         response_description="Object containing exposable configuration settings",
     )
     def index(
         self,
         trans: ProvidesUserContext = DependsOnTrans,
-        view: Optional[str] = SerializationViewQueryParam,
+        view: SerializationViewQueryParam = None,
         keys: Optional[str] = SerializationKeysQueryParam,
     ) -> Dict[str, Any]:
         """
         Return an object containing exposable configuration settings.
 
         A more complete list is returned if the user is an admin.
         Pass in `view` and a comma-seperated list of keys to control which
         configuration settings are returned.
         """
         return _index(self.configuration_manager, trans, view, keys)
 
     @router.get(
         "/api/version",
+        public=True,
         summary="Return Galaxy version information: major/minor version, optional extra info",
         response_description="Galaxy version information: major/minor version, optional extra info",
     )
     def version(self) -> Dict[str, Any]:
         """Return Galaxy version information: major/minor version, optional extra info."""
         return self.configuration_manager.version()
 
@@ -98,14 +106,24 @@
         response_description="Decoded id",
     )
     def decode_id(self, encoded_id: str = EncodedIdPathParam) -> Dict[str, int]:
         """Decode a given id."""
         return self.configuration_manager.decode_id(encoded_id)
 
     @router.get(
+        "/api/configuration/encode/{decoded_id}",
+        require_admin=True,
+        summary="Encode a given id",
+        response_description="Encoded id",
+    )
+    def encode_id(self, decoded_id: int = DecodedIdPathParam) -> Dict[str, str]:
+        """Decode a given id."""
+        return self.configuration_manager.encode_id(decoded_id)
+
+    @router.get(
         "/api/configuration/tool_lineages",
         require_admin=True,
         summary="Return tool lineages for tools that have them",
         response_description="Tool lineages for tools that have them",
     )
     def tool_lineages(self) -> List[Dict[str, Dict]]:
         """Return tool lineages for tools that have them."""
@@ -117,14 +135,16 @@
     def reload_toolbox(self):
         """Reload the Galaxy toolbox (but not individual tools)."""
         self.configuration_manager.reload_toolbox()
 
 
 def _user_to_model(user):
     if user:
-        return UserModel.construct(**user.to_dict(view="element", value_mapper={"id": DecodedDatabaseIdField.encode}))
+        return UserModel.model_construct(
+            **user.to_dict(view="element", value_mapper={"id": Security.security.encode_id})
+        )
     return None
 
 
 def _index(manager: ConfigurationManager, trans, view, keys):
     serialization_params = parse_serialization_params(view, keys, "all")
     return manager.get_configuration(trans, serialization_params)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/container_resolution.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/container_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations allowing clients to manage container resolution.
 """
+
 import logging
 
 import requests
 
 from galaxy.structured_app import StructuredApp
 from galaxy.tool_util.deps import views
 from galaxy.web import (
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/dataset_collections.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dataset_collections.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,48 +2,45 @@
 from typing import Optional
 
 from fastapi import (
     Body,
     Path,
     Query,
 )
+from typing_extensions import Annotated
 
 from galaxy.managers.context import ProvidesHistoryContext
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import (
     CreateNewCollectionPayload,
     DatasetCollectionInstanceType,
     DCESummary,
     HDCADetailed,
 )
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import (
+    DatasetCollectionElementIdPathParam,
+    HistoryHDCAIDPathParam,
+)
 from galaxy.webapps.galaxy.services.dataset_collections import (
     DatasetCollectionAttributesResult,
     DatasetCollectionContentElements,
     DatasetCollectionsService,
     SuitableConverters,
     UpdateCollectionAttributePayload,
 )
 
 log = getLogger(__name__)
 
 router = Router(tags=["dataset collections"])
 
-DatasetCollectionIdPathParam: DecodedDatabaseIdField = Path(
-    ..., description="The encoded identifier of the dataset collection."
-)
-
-
-DatasetCollectionElementIdPathParam: DecodedDatabaseIdField = Path(
-    ..., description="The encoded identifier of the dataset collection element."
-)
 
 InstanceTypeQueryParam: DatasetCollectionInstanceType = Query(
     default="history",
     description="The type of collection instance. Either `history` (default) or `library`.",
 )
 
 
@@ -64,69 +61,72 @@
 
     @router.post(
         "/api/dataset_collections/{id}/copy",
         summary="Copy the given collection datasets to a new collection using a new `dbkey` attribute.",
     )
     def copy(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = Path(..., description="The ID of the dataset collection to copy."),
         payload: UpdateCollectionAttributePayload = Body(...),
     ):
         self.service.copy(trans, id, payload)
 
     @router.get(
         "/api/dataset_collections/{id}/attributes",
         summary="Returns `dbkey`/`extension` attributes for all the collection elements.",
     )
     def attributes(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = DatasetCollectionIdPathParam,
         instance_type: DatasetCollectionInstanceType = InstanceTypeQueryParam,
     ) -> DatasetCollectionAttributesResult:
         return self.service.attributes(trans, id, instance_type)
 
     @router.get(
         "/api/dataset_collections/{id}/suitable_converters",
         summary="Returns a list of applicable converters for all datatypes in the given collection.",
     )
     def suitable_converters(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = DatasetCollectionIdPathParam,
         instance_type: DatasetCollectionInstanceType = InstanceTypeQueryParam,
     ) -> SuitableConverters:
         return self.service.suitable_converters(trans, id, instance_type)
 
     @router.get(
         "/api/dataset_collections/{id}",
         summary="Returns detailed information about the given collection.",
     )
     def show(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = DatasetCollectionIdPathParam,
         instance_type: DatasetCollectionInstanceType = InstanceTypeQueryParam,
     ) -> HDCADetailed:
         return self.service.show(trans, id, instance_type)
 
     @router.get(
         "/api/dataset_collections/{hdca_id}/contents/{parent_id}",
         name="contents_dataset_collection",
         summary="Returns direct child contents of indicated dataset collection parent ID.",
     )
     def contents(
         self,
+        hdca_id: HistoryHDCAIDPathParam,
+        parent_id: Annotated[
+            DecodedDatabaseIdField,
+            Path(
+                ...,
+                description="Parent collection ID describing what collection the contents belongs to.",
+            ),
+        ],
         trans: ProvidesHistoryContext = DependsOnTrans,
-        hdca_id: DecodedDatabaseIdField = DatasetCollectionIdPathParam,
-        parent_id: DecodedDatabaseIdField = Path(
-            ...,
-            description="Parent collection ID describing what collection the contents belongs to.",
-        ),
         instance_type: DatasetCollectionInstanceType = InstanceTypeQueryParam,
         limit: Optional[int] = Query(
             default=None,
             description="The maximum number of content elements to return.",
         ),
         offset: Optional[int] = Query(
             default=None,
@@ -134,11 +134,11 @@
         ),
     ) -> DatasetCollectionContentElements:
         return self.service.contents(trans, hdca_id, parent_id, instance_type, limit, offset)
 
     @router.get("/api/dataset_collection_element/{dce_id}")
     def content(
         self,
+        dce_id: DatasetCollectionElementIdPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        dce_id: DecodedDatabaseIdField = DatasetCollectionElementIdPathParam,
     ) -> DCESummary:
         return self.service.dce_content(trans, dce_id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/datasets.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on the contents of a history dataset.
 """
+
 import logging
 from io import (
     BytesIO,
     IOBase,
     StringIO,
 )
 from typing import (
@@ -22,14 +23,15 @@
     Query,
     Request,
 )
 from starlette.responses import (
     Response,
     StreamingResponse,
 )
+from typing_extensions import Annotated
 
 from galaxy.schema import (
     FilterQueryParams,
     SerializationParams,
 )
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import (
@@ -47,36 +49,40 @@
     DependsOnTrans,
     Router,
 )
 from galaxy.webapps.galaxy.api.common import (
     get_filter_query_params,
     get_query_parameters_from_request_excluding,
     get_update_permission_payload,
+    HistoryDatasetIDPathParam,
+    HistoryIDPathParam,
     query_serialization_params,
 )
 from galaxy.webapps.galaxy.services.datasets import (
     ComputeDatasetHashPayload,
     ConvertedDatasetsMap,
     DatasetContentType,
+    DatasetExtraFiles,
     DatasetInheritanceChain,
     DatasetsService,
     DatasetStorageDetails,
     DatasetTextContentDetails,
     DeleteDatasetBatchPayload,
     DeleteDatasetBatchResult,
     RequestDataType,
+    UpdateObjectStoreIdPayload,
 )
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["datasets"])
 
-DatasetIDPathParam: DecodedDatabaseIdField = Path(..., description="The encoded database identifier of the dataset.")
-
-HistoryIDPathParam: DecodedDatabaseIdField = Path(..., description="The encoded database identifier of the History.")
+DatasetIDPathParam = Annotated[
+    DecodedDatabaseIdField, Path(..., description="The encoded database identifier of the dataset.")
+]
 
 DatasetSourceQueryParam: DatasetSourceType = Query(
     default=DatasetSourceType.hda,
     description="Whether this dataset belongs to a history (HDA) or a library (LDDA).",
 )
 
 PreviewQueryParam = Query(
@@ -131,14 +137,15 @@
 @router.cbv
 class FastAPIDatasets:
     service: DatasetsService = depends(DatasetsService)
 
     @router.get(
         "/api/datasets",
         summary="Search datasets or collections using a query system.",
+        response_model_exclude_unset=True,
     )
     def index(
         self,
         trans=DependsOnTrans,
         history_id: Optional[DecodedDatabaseIdField] = Query(
             default=None,
             description="Optional identifier of a History. Use it to restrict the search within a particular History.",
@@ -150,52 +157,52 @@
 
     @router.get(
         "/api/datasets/{dataset_id}/storage",
         summary="Display user-facing storage details related to the objectstore a dataset resides in.",
     )
     def show_storage(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         hda_ldda: DatasetSourceType = DatasetSourceQueryParam,
     ) -> DatasetStorageDetails:
         return self.service.show_storage(trans, dataset_id, hda_ldda)
 
     @router.get(
         "/api/datasets/{dataset_id}/inheritance_chain",
         summary="For internal use, this endpoint may change without warning.",
         include_in_schema=True,  # Can be changed to False if we don't really want to expose this
     )
     def show_inheritance_chain(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         hda_ldda: DatasetSourceType = DatasetSourceQueryParam,
     ) -> DatasetInheritanceChain:
         return self.service.show_inheritance_chain(trans, dataset_id, hda_ldda)
 
     @router.get(
         "/api/datasets/{dataset_id}/get_content_as_text",
         summary="Returns dataset content as Text.",
     )
     def get_content_as_text(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
     ) -> DatasetTextContentDetails:
         return self.service.get_content_as_text(trans, dataset_id)
 
     @router.get(
         "/api/datasets/{dataset_id}/converted/{ext}",
         summary="Return information about datasets made by converting this dataset to a new format.",
     )
     def converted_ext(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         ext: str = Path(
             ...,
             description="File extension of the new format to convert this dataset to.",
         ),
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHDA:
         """
@@ -209,54 +216,65 @@
 
     @router.get(
         "/api/datasets/{dataset_id}/converted",
         summary=("Return a a map with all the existing converted datasets associated with this instance."),
     )
     def converted(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
     ) -> ConvertedDatasetsMap:
         """
         Return a map of `<converted extension> : <converted id>` containing all the *existing* converted datasets.
         """
         return self.service.converted(trans, dataset_id)
 
     @router.put(
         "/api/datasets/{dataset_id}/permissions",
         summary="Set permissions of the given history dataset to the given role ids.",
     )
     def update_permissions(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         # Using a generic Dict here as an attempt on supporting multiple aliases for the permissions params.
         payload: Dict[str, Any] = Body(
             default=...,
-            example=UpdateDatasetPermissionsPayload(),
+            examples=[UpdateDatasetPermissionsPayload()],
         ),
     ) -> DatasetAssociationRoles:
         """Set permissions of the given history dataset to the given role ids."""
         update_payload = get_update_permission_payload(payload)
         return self.service.update_permissions(trans, dataset_id, update_payload)
 
     @router.get(
         "/api/histories/{history_id}/contents/{history_content_id}/extra_files",
-        summary="Generate list of extra files.",
+        summary="Get the list of extra files/directories associated with a dataset.",
         tags=["histories"],
     )
-    def extra_files(
+    def extra_files_history(
         self,
+        history_id: HistoryIDPathParam,
+        history_content_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        history_content_id: DecodedDatabaseIdField = DatasetIDPathParam,
-    ):
+    ) -> DatasetExtraFiles:
         return self.service.extra_files(trans, history_content_id)
 
     @router.get(
+        "/api/datasets/{dataset_id}/extra_files",
+        summary="Get the list of extra files/directories associated with a dataset.",
+    )
+    def extra_files(
+        self,
+        dataset_id: DatasetIDPathParam,
+        trans=DependsOnTrans,
+    ) -> DatasetExtraFiles:
+        return self.service.extra_files(trans, dataset_id)
+
+    @router.get(
         "/api/histories/{history_id}/contents/{history_content_id}/display",
         name="history_contents_display",
         summary="Displays (preview) or downloads dataset content.",
         tags=["histories"],
         response_class=StreamingResponse,
     )
     @router.head(
@@ -264,19 +282,17 @@
         name="history_contents_display",
         summary="Check if dataset content can be previewed or downloaded.",
         tags=["histories"],
     )
     def display_history_content(
         self,
         request: Request,
+        history_content_id: HistoryDatasetIDPathParam,
+        history_id: Optional[HistoryIDPathParam] = None,
         trans=DependsOnTrans,
-        history_id: Optional[DecodedDatabaseIdField] = Path(
-            description="The encoded database identifier of the History.",
-        ),
-        history_content_id: DecodedDatabaseIdField = DatasetIDPathParam,
         preview: bool = PreviewQueryParam,
         filename: Optional[str] = FilenameQueryParam,
         to_ext: Optional[str] = ToExtQueryParam,
         raw: bool = RawQueryParam,
         offset: Optional[int] = DisplayOffsetQueryParam,
         ck_size: Optional[int] = DisplayChunkSizeQueryParam,
     ):
@@ -291,16 +307,16 @@
     @router.head(
         "/api/datasets/{history_content_id}/display",
         summary="Check if dataset content can be previewed or downloaded.",
     )
     def display(
         self,
         request: Request,
+        history_content_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        history_content_id: DecodedDatabaseIdField = DatasetIDPathParam,
         preview: bool = PreviewQueryParam,
         filename: Optional[str] = FilenameQueryParam,
         to_ext: Optional[str] = ToExtQueryParam,
         raw: bool = RawQueryParam,
         offset: Optional[int] = DisplayOffsetQueryParam,
         ck_size: Optional[int] = DisplayChunkSizeQueryParam,
     ):
@@ -351,19 +367,17 @@
         name="get_metadata_file",
         tags=["histories"],
         operation_id="history_contents__get_metadata_file",
         response_class=GalaxyFileResponse,
     )
     def get_metadata_file_history_content(
         self,
+        history_id: HistoryIDPathParam,
+        history_content_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        history_id: DecodedDatabaseIdField = Path(
-            description="The encoded database identifier of the History.",
-        ),
-        history_content_id: DecodedDatabaseIdField = DatasetIDPathParam,
         metadata_file: str = Query(
             ...,
             description="The name of the metadata file to retrieve.",
         ),
     ):
         return self._get_metadata_file(trans, history_content_id, metadata_file)
 
@@ -375,16 +389,16 @@
     )
     @router.head(
         "/api/datasets/{history_content_id}/metadata_file",
         summary="Check if metadata file can be downloaded.",
     )
     def get_metadata_file_datasets(
         self,
+        history_content_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        history_content_id: DecodedDatabaseIdField = DatasetIDPathParam,
         metadata_file: str = Query(
             ...,
             description="The name of the metadata file to retrieve.",
         ),
     ):
         return self._get_metadata_file(trans, history_content_id, metadata_file)
 
@@ -400,16 +414,16 @@
     @router.get(
         "/api/datasets/{dataset_id}",
         summary="Displays information about and/or content of a dataset.",
     )
     def show(
         self,
         request: Request,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         hda_ldda: DatasetSourceType = Query(
             default=DatasetSourceType.hda,
             description=("The type of information about the dataset to be requested."),
         ),
         data_type: Optional[RequestDataType] = Query(
             default=None,
             description=(
@@ -422,28 +436,28 @@
     ):
         """
         **Note**: Due to the multipurpose nature of this endpoint, which can receive a wild variety of parameters
         and return different kinds of responses, the documentation here will be limited.
         To get more information please check the source code.
         """
         exclude_params = {"hda_ldda", "data_type"}
-        exclude_params.update(SerializationParams.__fields__.keys())
+        exclude_params.update(SerializationParams.model_fields.keys())
         extra_params = get_query_parameters_from_request_excluding(request, exclude_params)
 
         return self.service.show(trans, dataset_id, hda_ldda, serialization_params, data_type, **extra_params)
 
     @router.get(
         "/api/datasets/{dataset_id}/content/{content_type}",
         summary="Retrieve information about the content of a dataset.",
     )
     def get_structured_content(
         self,
         request: Request,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         content_type: DatasetContentType = DatasetContentType.data,
     ):
         content, headers = self.service.get_structured_content(trans, dataset_id, content_type, **request.query_params)
         return Response(content=content, headers=headers)
 
     @router.delete(
         "/api/datasets",
@@ -463,13 +477,26 @@
 
     @router.put(
         "/api/datasets/{dataset_id}/hash",
         summary="Compute dataset hash for dataset and update model",
     )
     def compute_hash(
         self,
+        dataset_id: HistoryDatasetIDPathParam,
         trans=DependsOnTrans,
-        dataset_id: DecodedDatabaseIdField = DatasetIDPathParam,
         hda_ldda: DatasetSourceType = DatasetSourceQueryParam,
         payload: ComputeDatasetHashPayload = Body(...),
     ) -> AsyncTaskResultSummary:
         return self.service.compute_hash(trans, dataset_id, payload, hda_ldda=hda_ldda)
+
+    @router.put(
+        "/api/datasets/{dataset_id}/object_store_id",
+        summary="Update an object store ID for a dataset you own.",
+        operation_id="datasets__update_object_store_id",
+    )
+    def update_object_store_id(
+        self,
+        dataset_id: HistoryDatasetIDPathParam,
+        trans=DependsOnTrans,
+        payload: UpdateObjectStoreIdPayload = Body(...),
+    ) -> None:
+        self.service.update_object_store_id(trans, dataset_id, payload)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/datatypes.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/datatypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations allowing clients to determine datatype supported by Galaxy.
 """
+
 import logging
 from typing import (
     cast,
     Dict,
     List,
     Optional,
     Union,
@@ -56,36 +57,39 @@
 
 @router.cbv
 class FastAPIDatatypes:
     datatypes_registry: Registry = depends(Registry)
 
     @router.get(
         "/api/datatypes",
+        public=True,
         summary="Lists all available data types",
         response_description="List of data types",
     )
     async def index(
         self,
         extension_only: Optional[bool] = ExtensionOnlyQueryParam,
         upload_only: Optional[bool] = UploadOnlyQueryParam,
     ) -> Union[List[DatatypeDetails], List[str]]:
         """Gets the list of all available data types."""
         return view_index(self.datatypes_registry, extension_only, upload_only)
 
     @router.get(
         "/api/datatypes/mapping",
+        public=True,
         summary="Returns mappings for data types and their implementing classes",
         response_description="Dictionary to map data types with their classes",
     )
     async def mapping(self) -> DatatypesMap:
         """Gets mappings for data types."""
         return view_mapping(self.datatypes_registry)
 
     @router.get(
         "/api/datatypes/types_and_mapping",
+        public=True,
         summary="Returns all the data types extensions and their mappings",
         response_description="Dictionary to map data types with their classes",
     )
     async def types_and_mapping(
         self,
         extension_only: Optional[bool] = ExtensionOnlyQueryParam,
         upload_only: Optional[bool] = UploadOnlyQueryParam,
@@ -96,61 +100,67 @@
         return DatatypesCombinedMap(
             datatypes=view_index(self.datatypes_registry, extension_only, upload_only),
             datatypes_mapping=view_mapping(self.datatypes_registry),
         )
 
     @router.get(
         "/api/datatypes/sniffers",
+        public=True,
         summary="Returns the list of all installed sniffers",
         response_description="List of datatype sniffers",
     )
     async def sniffers(self) -> List[str]:
         """Gets the list of all installed data type sniffers."""
         return view_sniffers(self.datatypes_registry)
 
     @router.get(
         "/api/datatypes/converters",
+        public=True,
         summary="Returns the list of all installed converters",
         response_description="List of all datatype converters",
     )
     async def converters(self) -> DatatypeConverterList:
         """Gets the list of all installed converters."""
         return view_converters(self.datatypes_registry)
 
     @router.get(
         "/api/datatypes/edam_formats",
+        public=True,
         summary="Returns a dictionary/map of datatypes and EDAM formats",
         response_description="Dictionary/map of datatypes and EDAM formats",
     )
     async def edam_formats(self) -> Dict[str, str]:
         """Gets a map of datatypes and their corresponding EDAM formats."""
         return cast(Dict[str, str], view_edam_formats(self.datatypes_registry))
 
     @router.get(
         "/api/datatypes/edam_formats/detailed",
+        public=True,
         summary="Returns a dictionary of datatypes and EDAM format details",
         response_description="Dictionary of EDAM format details containing the EDAM iri, label, and definition",
         response_model=DatatypesEDAMDetailsDict,
     )
     async def edam_formats_detailed(self):
         """Gets a map of datatypes and their corresponding EDAM formats.
         EDAM formats contain the EDAM iri, label, and definition."""
         return view_edam_formats(self.datatypes_registry, True)
 
     @router.get(
         "/api/datatypes/edam_data",
+        public=True,
         summary="Returns a dictionary/map of datatypes and EDAM data",
         response_description="Dictionary/map of datatypes and EDAM data",
     )
     async def edam_data(self) -> Dict[str, str]:
         """Gets a map of datatypes and their corresponding EDAM data."""
         return cast(Dict[str, str], view_edam_data(self.datatypes_registry))
 
     @router.get(
         "/api/datatypes/edam_data/detailed",
+        public=True,
         summary="Returns a dictionary of datatypes and EDAM data details",
         response_description="Dictionary of EDAM data details containing the EDAM iri, label, and definition",
         response_model=DatatypesEDAMDetailsDict,
     )
     async def edam_data_detailed(self):
         """Gets a map of datatypes and their corresponding EDAM data.
         EDAM data contains the EDAM iri, label, and definition."""
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/display_applications.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/display_applications.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on annotations.
 """
+
 import logging
 from typing import (
     Dict,
     List,
     Optional,
 )
 
@@ -27,14 +28,15 @@
 
 @router.cbv
 class FastAPIDisplay:
     manager: DisplayApplicationsManager = depends(DisplayApplicationsManager)
 
     @router.get(
         "/api/display_applications",
+        public=True,
         summary="Returns the list of display applications.",
         name="display_applications_index",
     )
     def index(
         self,
     ) -> List[DisplayApplication]:
         """
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/drs.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/drs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Implement a DRS server for Galaxy dataset objects (experimental)."""
+
 import logging
 from io import IOBase
 from typing import cast
 
 from fastapi import (
     Path,
     Request,
@@ -10,19 +11,18 @@
 from starlette.responses import FileResponse
 
 from galaxy.config import GalaxyAppConfiguration
 from galaxy.exceptions import ObjectNotFound
 from galaxy.managers.context import ProvidesHistoryContext
 from galaxy.schema.drs import (
     DrsObject,
+    Organization,
     Service,
-    ServiceOrganization,
     ServiceType,
 )
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.version import VERSION
 from galaxy.webapps.galaxy.services.datasets import DatasetsService
 from . import (
     depends,
     DependsOnTrans,
     Router,
 )
@@ -39,73 +39,73 @@
 
 
 @router.cbv
 class DrsApi:
     service: DatasetsService = depends(DatasetsService)
     config: GalaxyAppConfiguration = depends(GalaxyAppConfiguration)
 
-    @router.get("/ga4gh/drs/v1/service-info")
+    @router.get("/ga4gh/drs/v1/service-info", public=True)
     def service_info(self, request: Request) -> Service:
         components = request.url.components
         hostname = components.hostname
         assert hostname
         default_organization_id = ".".join(reversed(hostname.split(".")))
         config = self.config
         organization_id = config.ga4gh_service_id or default_organization_id
         organization_name = config.organization_name or organization_id
         organization_url = config.organization_url or f"{components.scheme}://{components.netloc}"
 
-        organization = ServiceOrganization(
+        organization = Organization(
             url=organization_url,
             name=organization_name,
         )
         service_type = ServiceType(
             group="org.ga4gh",
             artifact="drs",
             version="1.2.0",
         )
-        environment = config.ga4gh_service_environment
         extra_kwds = {}
-        if environment:
+        if environment := config.ga4gh_service_environment:
             extra_kwds["environment"] = environment
         return Service(
             id=organization_id + ".drs",
             name=DRS_SERVICE_NAME,
             description=DRS_SERVICE_DESCRIPTION,
             organization=organization,
             type=service_type,
             version=VERSION,
             **extra_kwds,
         )
 
-    @router.get("/ga4gh/drs/v1/objects/{object_id}")
-    @router.post("/ga4gh/drs/v1/objects/{object_id}")  # spec specifies both get and post should work.
+    @router.get("/ga4gh/drs/v1/objects/{object_id}", public=True)
+    @router.post("/ga4gh/drs/v1/objects/{object_id}", public=True)  # spec specifies both get and post should work.
     def get_object(
         self,
         request: Request,
         trans: ProvidesHistoryContext = DependsOnTrans,
         object_id: str = ObjectIDParam,
     ) -> DrsObject:
         return self.service.get_drs_object(trans, object_id, request_url=request.url)
 
-    @router.get("/ga4gh/drs/v1/objects/{object_id}/access/{access_id}")
-    @router.post("/ga4gh/drs/v1/objects/{object_id}/access/{access_id}")
+    @router.get("/ga4gh/drs/v1/objects/{object_id}/access/{access_id}", public=True)
+    @router.post("/ga4gh/drs/v1/objects/{object_id}/access/{access_id}", public=True)
     def get_access_url(
         self,
         request: Request,
         trans: ProvidesHistoryContext = DependsOnTrans,
         object_id: str = ObjectIDParam,
         access_id: str = AccessIDParam,
     ):
         raise ObjectNotFound("Access IDs are not implemented for this DRS server")
 
     @router.get(
         "/api/drs_download/{object_id}",
+        public=True,
         response_class=FileResponse,
     )
     def download(self, trans: ProvidesHistoryContext = DependsOnTrans, object_id: str = ObjectIDParam):
         decoded_object_id, hda_ldda = self.service.drs_dataset_instance(object_id)
         display_data, headers = self.service.display(
-            trans, DecodedDatabaseIdField(decoded_object_id), hda_ldda=hda_ldda, filename=None, raw=True
+            trans, decoded_object_id, hda_ldda=hda_ldda, filename=None, raw=True
         )
         data_io = cast(IOBase, display_data)
         return FileResponse(getattr(data_io, "name", "unnamed_file"), headers=headers)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/dynamic_tools.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/dynamic_tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/extended_metadata.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/extended_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on annotations.
 """
+
 import logging
 from typing import (
     Generic,
     Optional,
     TypeVar,
 )
 
@@ -29,16 +30,15 @@
 
 
 class BaseExtendedMetadataController(
     BaseGalaxyAPIController, UsesExtendedMetadataMixin, UsesLibraryMixinItems, UsesStoredWorkflowMixin, Generic[T]
 ):
     exmeta_item_id: str
 
-    def _get_item_from_id(self, trans, idstr, check_writable=True) -> Optional[T]:
-        ...
+    def _get_item_from_id(self, trans, idstr, check_writable=True) -> Optional[T]: ...
 
     @web.expose_api
     def index(self, trans, **kwd):
         idnum = kwd[self.exmeta_item_id]
         item = self._get_item_from_id(trans, idnum, check_writable=False)
         if item is not None:
             ex_meta = self.get_item_extended_metadata_obj(trans, item)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/folder_contents.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folder_contents.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 API operations on the contents of a library folder.
 """
+
 import logging
 from typing import Optional
 
 from fastapi import (
     Body,
     Path,
     Query,
 )
+from typing_extensions import Annotated
 
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.schema.fields import LibraryFolderDatabaseIdField
 from galaxy.schema.schema import (
     CreateLibraryFilePayload,
     LibraryFolderContentsIndexQueryPayload,
     LibraryFolderContentsIndexResult,
@@ -25,17 +27,18 @@
 )
 from galaxy.webapps.galaxy.services.library_folder_contents import LibraryFolderContentsService
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["data libraries folders"])
 
-FolderIdPathParam: LibraryFolderDatabaseIdField = Path(
-    ..., title="Folder ID", description="The encoded identifier of the library folder."
-)
+FolderIdPathParam = Annotated[
+    LibraryFolderDatabaseIdField,
+    Path(..., title="Folder ID", description="The encoded identifier of the library folder."),
+]
 
 LimitQueryParam: int = Query(default=10, title="Limit", description="Maximum number of contents to return.")
 
 OffsetQueryParam: int = Query(
     default=0,
     title="Offset",
     description="Return contents from this specified position. For example, if ``limit`` is set to 100 and ``offset`` to 200, contents between position 200-299 will be returned.",
@@ -78,16 +81,16 @@
                 "description": "The contents of the folder that match the query parameters.",
                 "model": LibraryFolderContentsIndexResult,
             },
         },
     )
     def index(
         self,
+        folder_id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        folder_id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         limit: int = LimitQueryParam,
         offset: int = OffsetQueryParam,
         search_text: Optional[str] = SearchQueryParam,
         include_deleted: Optional[bool] = IncludeDeletedQueryParam,
         order_by: LibraryFolderContentsIndexSortByEnum = SortByQueryParam,
         sort_desc: Optional[bool] = SortDescQueryParam,
     ):
@@ -116,12 +119,12 @@
     @router.post(
         "/api/folders/{folder_id}/contents",
         name="add_history_datasets_to_library",
         summary="Creates a new library file from an existing HDA/HDCA.",
     )
     def create(
         self,
+        folder_id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        folder_id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         payload: CreateLibraryFilePayload = Body(...),
     ):
         return self.service.create(trans, folder_id, payload)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/folders.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/folders.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 API operations on library folders.
 """
+
 import logging
 from typing import (
     Optional,
     Union,
 )
 
 from fastapi import (
     Body,
     Path,
     Query,
 )
+from typing_extensions import Annotated
 
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.schema.fields import LibraryFolderDatabaseIdField
 from galaxy.schema.schema import (
     CreateLibraryFolderPayload,
     LibraryAvailablePermissions,
     LibraryFolderCurrentPermissions,
@@ -32,87 +34,88 @@
 )
 from galaxy.webapps.galaxy.services.library_folders import LibraryFoldersService
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["data libraries folders"])
 
-FolderIdPathParam: LibraryFolderDatabaseIdField = Path(
-    ..., title="Folder ID", description="The encoded identifier of the library folder."
-)
-
-UndeleteQueryParam: Optional[bool] = Query(
-    default=None, title="Undelete", description="Whether to restore a deleted library folder."
-)
+FolderIdPathParam = Annotated[
+    LibraryFolderDatabaseIdField,
+    Path(..., title="Folder ID", description="The encoded identifier of the library folder."),
+]
+
+UndeleteQueryParam = Annotated[
+    Optional[bool], Query(title="Undelete", description="Whether to restore a deleted library folder.")
+]
 
 
 @router.cbv
 class FastAPILibraryFolders:
     service: LibraryFoldersService = depends(LibraryFoldersService)
 
     @router.get(
         "/api/folders/{id}",
         summary="Displays information about a particular library folder.",
     )
     def show(
         self,
+        id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
     ) -> LibraryFolderDetails:
         """Returns detailed information about the library folder with the given ID."""
         return self.service.show(trans, id)
 
     @router.post(
         "/api/folders/{id}",
         summary="Create a new library folder underneath the one specified by the ID.",
     )
     def create(
         self,
+        id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         payload: CreateLibraryFolderPayload = Body(...),
     ) -> LibraryFolderDetails:
         """Returns detailed information about the newly created library folder."""
         return self.service.create(trans, id, payload)
 
     @router.put(
         "/api/folders/{id}",
         summary="Updates the information of an existing library folder.",
     )
     @router.patch("/api/folders/{id}")
     def update(
         self,
+        id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         payload: UpdateLibraryFolderPayload = Body(...),
     ) -> LibraryFolderDetails:
         """Updates the information of an existing library folder."""
         return self.service.update(trans, id, payload)
 
     @router.delete(
         "/api/folders/{id}",
         summary="Marks the specified library folder as deleted (or undeleted).",
     )
     def delete(
         self,
+        id: FolderIdPathParam,
+        undelete: UndeleteQueryParam = None,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
-        undelete: Optional[bool] = UndeleteQueryParam,
     ) -> LibraryFolderDetails:
         """Marks the specified library folder as deleted (or undeleted)."""
         return self.service.delete(trans, id, undelete)
 
     @router.get(
         "/api/folders/{id}/permissions",
         summary="Gets the current or available permissions of a particular library folder.",
     )
     def get_permissions(
         self,
+        id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         scope: Optional[LibraryPermissionScope] = Query(
             None,
             title="Scope",
             description="The scope of the permissions to retrieve. Either the `current` permissions or the `available`.",
         ),
         page: int = Query(
             default=1, title="Page", description="The page number to retrieve when paginating the available roles."
@@ -137,24 +140,24 @@
 
     @router.post(
         "/api/folders/{id}/permissions",
         summary="Sets the permissions to manage a library folder.",
     )
     def set_permissions(
         self,
+        id: FolderIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: LibraryFolderDatabaseIdField = FolderIdPathParam,
         action: Optional[LibraryFolderPermissionAction] = Query(
             default=None,
             title="Action",
             description=(
                 "Indicates what action should be performed on the Library. "
                 f"Currently only `{LibraryFolderPermissionAction.set_permissions.value}` is supported."
             ),
         ),
         payload: LibraryFolderPermissionsPayload = Body(...),
     ) -> LibraryFolderCurrentPermissions:
         """Sets the permissions to manage a library folder."""
-        payload_dict = payload.dict(by_alias=True)
+        payload_dict = payload.model_dump(by_alias=True)
         if isinstance(payload, LibraryFolderPermissionsPayload) and action is not None:
             payload_dict["action"] = action
         return self.service.set_permissions(trans, id, payload_dict)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/genomes.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     @router.get(
         "/api/genomes/{id}/indexes",
         summary="Return all available indexes for a genome id for provided type",
         response_description="Indexes for a genome id for provided type",
     )
     def indexes(
         self,
+        trans: ProvidesUserContext = DependsOnTrans,  # may want to get custom index in the future
         id: str = IdPathParam,
         type: str = IndexTypeQueryParam,
         format: str = FormatQueryParam,
     ) -> Any:
         id = get_id(id, format)
         rval = self.manager.get_indexes(id, type)
         return Response(rval)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/group_roles.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_roles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """
 API operations on Group objects.
 """
 
 import logging
 
-from fastapi import Path
-
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.managers.group_roles import GroupRolesManager
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.schema.schema import (
     GroupRoleListResponse,
     GroupRoleResponse,
 )
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import (
+    GroupIDPathParam,
+    RoleIDPathParam,
+)
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["group_roles"])
 
-GroupIDParam: DecodedDatabaseIdField = Path(..., title="GroupID", description="The ID of the group")
-
-RoleIDParam: DecodedDatabaseIdField = Path(..., title="RoleID", description="The ID of the role")
-
 
 def group_role_to_model(trans, group_id: int, role) -> GroupRoleResponse:
-    encoded_group_id = DecodedDatabaseIdField.encode(group_id)
-    encoded_role_id = DecodedDatabaseIdField.encode(role.id)
+    encoded_group_id = Security.security.encode_id(group_id)
+    encoded_role_id = Security.security.encode_id(role.id)
     url = trans.url_builder("group_role", group_id=encoded_group_id, role_id=encoded_role_id)
     return GroupRoleResponse(id=role.id, name=role.name, url=url)
 
 
 @router.cbv
 class FastAPIGroupRoles:
     manager: GroupRolesManager = depends(GroupRolesManager)
@@ -42,46 +40,48 @@
     @router.get(
         "/api/groups/{group_id}/roles",
         require_admin=True,
         summary="Displays a collection (list) of groups.",
         name="group_roles",
     )
     def index(
-        self, trans: ProvidesAppContext = DependsOnTrans, group_id: DecodedDatabaseIdField = GroupIDParam
+        self,
+        group_id: GroupIDPathParam,
+        trans: ProvidesAppContext = DependsOnTrans,
     ) -> GroupRoleListResponse:
         group_roles = self.manager.index(trans, group_id)
-        return GroupRoleListResponse(__root__=[group_role_to_model(trans, group_id, gr.role) for gr in group_roles])
+        return GroupRoleListResponse(root=[group_role_to_model(trans, group_id, gr.role) for gr in group_roles])
 
     @router.get(
         "/api/groups/{group_id}/roles/{role_id}",
         name="group_role",
         require_admin=True,
         summary="Displays information about a group role.",
     )
     def show(
         self,
+        group_id: GroupIDPathParam,
+        role_id: RoleIDPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        role_id: DecodedDatabaseIdField = RoleIDParam,
     ) -> GroupRoleResponse:
         role = self.manager.show(trans, role_id, group_id)
         return group_role_to_model(trans, group_id, role)
 
     @router.put("/api/groups/{group_id}/roles/{role_id}", require_admin=True, summary="Adds a role to a group")
     def update(
         self,
+        group_id: GroupIDPathParam,
+        role_id: RoleIDPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        role_id: DecodedDatabaseIdField = RoleIDParam,
     ) -> GroupRoleResponse:
         role = self.manager.update(trans, role_id, group_id)
         return group_role_to_model(trans, group_id, role)
 
     @router.delete("/api/groups/{group_id}/roles/{role_id}", require_admin=True, summary="Removes a role from a group")
     def delete(
         self,
+        group_id: GroupIDPathParam,
+        role_id: RoleIDPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        role_id: DecodedDatabaseIdField = RoleIDParam,
     ) -> GroupRoleResponse:
         role = self.manager.delete(trans, role_id, group_id)
         return group_role_to_model(trans, group_id, role)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/group_users.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/group_users.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 """
 API operations on Group objects.
 """
-import logging
 
-from fastapi import Path
+import logging
 
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.managers.group_users import GroupUsersManager
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.schema.schema import (
     GroupUserListResponse,
     GroupUserResponse,
 )
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import (
+    GroupIDPathParam,
+    UserIdPathParam,
+)
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["group_users"])
 
-GroupIDParam: DecodedDatabaseIdField = Path(..., title="GroupID", description="The ID of the group")
-
-UserIDParam: DecodedDatabaseIdField = Path(..., title="UserID", description="The ID of the user")
-
 
 def group_user_to_model(trans, group_id, user) -> GroupUserResponse:
-    encoded_group_id = DecodedDatabaseIdField.encode(group_id)
-    encoded_user_id = DecodedDatabaseIdField.encode(user.id)
+    encoded_group_id = Security.security.encode_id(group_id)
+    encoded_user_id = Security.security.encode_id(user.id)
     url = trans.url_builder("group_user", group_id=encoded_group_id, user_id=encoded_user_id)
     return GroupUserResponse(id=user.id, email=user.email, url=url)
 
 
 @router.cbv
 class FastAPIGroupUsers:
     manager: GroupUsersManager = depends(GroupUsersManager)
@@ -41,35 +40,37 @@
     @router.get(
         "/api/groups/{group_id}/users",
         require_admin=True,
         summary="Displays a collection (list) of groups.",
         name="group_users",
     )
     def index(
-        self, trans: ProvidesAppContext = DependsOnTrans, group_id: DecodedDatabaseIdField = GroupIDParam
+        self,
+        group_id: GroupIDPathParam,
+        trans: ProvidesAppContext = DependsOnTrans,
     ) -> GroupUserListResponse:
         """
         GET /api/groups/{encoded_group_id}/users
         Displays a collection (list) of groups.
         """
         group_users = self.manager.index(trans, group_id)
-        return GroupUserListResponse(__root__=[group_user_to_model(trans, group_id, gr) for gr in group_users])
+        return GroupUserListResponse(root=[group_user_to_model(trans, group_id, gr) for gr in group_users])
 
     @router.get(
         "/api/groups/{group_id}/user/{user_id}",
         alias="/api/groups/{group_id}/users/{user_id}",
         name="group_user",
         require_admin=True,
         summary="Displays information about a group user.",
     )
     def show(
         self,
+        group_id: GroupIDPathParam,
+        user_id: UserIdPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        user_id: DecodedDatabaseIdField = UserIDParam,
     ) -> GroupUserResponse:
         """
         Displays information about a group user.
         """
         user = self.manager.show(trans, user_id, group_id)
         return group_user_to_model(trans, group_id, user)
 
@@ -77,17 +78,17 @@
         "/api/groups/{group_id}/users/{user_id}",
         alias="/api/groups/{group_id}/user/{user_id}",
         require_admin=True,
         summary="Adds a user to a group",
     )
     def update(
         self,
+        group_id: GroupIDPathParam,
+        user_id: UserIdPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        user_id: DecodedDatabaseIdField = UserIDParam,
     ) -> GroupUserResponse:
         """
         PUT /api/groups/{encoded_group_id}/users/{encoded_user_id}
         Adds a user to a group
         """
         user = self.manager.update(trans, user_id, group_id)
         return group_user_to_model(trans, group_id, user)
@@ -96,17 +97,17 @@
         "/api/groups/{group_id}/user/{user_id}",
         alias="/api/groups/{group_id}/users/{user_id}",
         require_admin=True,
         summary="Removes a user from a group",
     )
     def delete(
         self,
+        group_id: GroupIDPathParam,
+        user_id: UserIdPathParam,
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = GroupIDParam,
-        user_id: DecodedDatabaseIdField = UserIDParam,
     ) -> GroupUserResponse:
         """
         DELETE /api/groups/{encoded_group_id}/users/{encoded_user_id}
         Removes a user from a group
         """
         user = self.manager.delete(trans, user_id, group_id)
         return group_user_to_model(trans, group_id, user)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/groups.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 API operations on Group objects.
 """
+
 import logging
 
 from fastapi import (
     Body,
     Path,
 )
+from typing_extensions import Annotated
 
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.managers.groups import GroupsManager
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.groups import (
     GroupCreatePayload,
     GroupListResponse,
@@ -47,38 +49,50 @@
         "/api/groups",
         summary="Creates a new group.",
         require_admin=True,
         response_model_exclude_unset=True,
     )
     def create(
         self,
+        payload: Annotated[GroupCreatePayload, Body(...)],
         trans: ProvidesAppContext = DependsOnTrans,
-        payload: GroupCreatePayload = Body(...),
     ) -> GroupListResponse:
         return self.manager.create(trans, payload)
 
     @router.get(
         "/api/groups/{group_id}",
         summary="Displays information about a group.",
         require_admin=True,
         name="show_group",
     )
     def show(
         self,
+        group_id: Annotated[DecodedDatabaseIdField, Path(...)],
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = Path(...),
     ) -> GroupResponse:
         return self.manager.show(trans, group_id)
 
     @router.put(
         "/api/groups/{group_id}",
         summary="Modifies a group.",
         require_admin=True,
         response_model_exclude_unset=True,
     )
     def update(
         self,
+        group_id: Annotated[DecodedDatabaseIdField, Path(...)],
         trans: ProvidesAppContext = DependsOnTrans,
-        group_id: DecodedDatabaseIdField = Path(...),
         payload: GroupCreatePayload = Body(...),
     ) -> GroupResponse:
         return self.manager.update(trans, group_id, payload)
+
+    @router.delete("/api/groups/{group_id}", require_admin=True)
+    def delete(self, group_id: DecodedDatabaseIdField, trans: ProvidesAppContext = DependsOnTrans):
+        self.manager.delete(trans, group_id)
+
+    @router.post("/api/groups/{group_id}/purge", require_admin=True)
+    def purge(self, group_id: DecodedDatabaseIdField, trans: ProvidesAppContext = DependsOnTrans):
+        self.manager.purge(trans, group_id)
+
+    @router.post("/api/groups/{group_id}/undelete", require_admin=True)
+    def undelete(self, group_id: DecodedDatabaseIdField, trans: ProvidesAppContext = DependsOnTrans):
+        self.manager.undelete(trans, group_id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/help.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/help.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import logging
 
 from fastapi import Query
 from typing_extensions import Annotated
 
+from galaxy.managers.context import ProvidesUserContext
 from galaxy.schema.help import HelpForumSearchResponse
 from galaxy.webapps.galaxy.services.help import HelpService
 from . import (
     depends,
+    DependsOnTrans,
     Router,
 )
 
 log = logging.getLogger(__name__)
 
 
 router = Router(tags=["help"])
@@ -23,13 +25,14 @@
     @router.get(
         "/api/help/forum/search",
         summary="Search the Galaxy Help forum.",
     )
     def search_forum(
         self,
         query: Annotated[str, Query(description="Search query to use for searching the Galaxy Help forum.")],
+        trans: ProvidesUserContext = DependsOnTrans,  # Require session or API key, don't make public
     ) -> HelpForumSearchResponse:
         """Search the Galaxy Help forum using the Discourse API.
 
         **Note**: This endpoint is for **INTERNAL USE ONLY** and is not part of the public Galaxy API.
         """
         return self.service.search_forum(query)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/histories.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/histories.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 API operations on a history.
 
 .. seealso:: :class:`galaxy.model.History`
 """
+
 import logging
 from typing import (
     Any,
     List,
     Optional,
     Union,
 )
@@ -18,24 +19,29 @@
     Path,
     Query,
     Response,
     status,
 )
 from pydantic.fields import Field
 from pydantic.main import BaseModel
+from typing_extensions import Annotated
 
 from galaxy.managers.context import (
     ProvidesHistoryContext,
     ProvidesUserContext,
 )
 from galaxy.schema import (
     FilterQueryParams,
     SerializationParams,
 )
 from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.history import (
+    HistoryIndexQueryPayload,
+    HistorySortByEnum,
+)
 from galaxy.schema.schema import (
     AnyArchivedHistoryView,
     AnyHistoryView,
     ArchiveHistoryRequestPayload,
     AsyncFile,
     AsyncTaskResultSummary,
     CreateHistoryFromStore,
@@ -43,113 +49,191 @@
     CustomBuildsMetadataResponse,
     ExportHistoryArchivePayload,
     ExportTaskListResponse,
     HistoryArchiveExportResult,
     JobExportHistoryArchiveListResponse,
     JobImportHistoryResponse,
     SetSlugPayload,
+    ShareHistoryWithStatus,
     ShareWithPayload,
-    ShareWithStatus,
     SharingStatus,
     StoreExportPayload,
     WriteStoreToPayload,
 )
 from galaxy.schema.types import LatestLiteral
 from galaxy.webapps.base.api import GalaxyFileResponse
 from galaxy.webapps.galaxy.api import (
     as_form,
     depends,
     DependsOnTrans,
+    IndexQueryTag,
     Router,
+    search_query_param,
     try_get_request_body_as_json,
 )
 from galaxy.webapps.galaxy.api.common import (
     get_filter_query_params,
     LimitQueryParam,
     OffsetQueryParam,
     query_serialization_params,
 )
 from galaxy.webapps.galaxy.services.histories import HistoriesService
+from .common import HistoryIDPathParam
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["histories"])
 
-HistoryIDPathParam: DecodedDatabaseIdField = Path(
-    ..., title="History ID", description="The encoded database identifier of the History."
+query_tags = [
+    IndexQueryTag("name", "The history's name."),
+    IndexQueryTag("annotation", "The history's annotation.", "a"),
+    IndexQueryTag("tag", "The history's tags.", "t"),
+]
+
+AllHistoriesQueryParam = Query(
+    default=False,
+    title="All Histories",
+    description=(
+        "Whether all histories from other users in this Galaxy should be included. "
+        "Only admins are allowed to query all histories."
+    ),
 )
 
 JehaIDPathParam: Union[DecodedDatabaseIdField, LatestLiteral] = Path(
     title="Job Export History ID",
     description=(
         "The ID of the specific Job Export History Association or "
         "`latest` (default) to download the last generated archive."
     ),
-    example="latest",
+    examples=["latest"],
 )
 
-AllHistoriesQueryParam = Query(
-    default=False,
-    title="All Histories",
-    description=(
-        "Whether all histories from other users in this Galaxy should be included. "
-        "Only admins are allowed to query all histories."
-    ),
+SearchQueryParam: Optional[str] = search_query_param(
+    model_name="History",
+    tags=query_tags,
+    free_text_fields=["title", "description", "slug", "tag"],
+)
+
+ShowOwnQueryParam: bool = Query(default=True, title="Show histories owned by user.", description="")
+
+ShowPublishedQueryParam: bool = Query(default=True, title="Include published histories.", description="")
+
+ShowSharedQueryParam: bool = Query(
+    default=False, title="Include histories shared with authenticated user.", description=""
+)
+
+ShowArchivedQueryParam: Optional[bool] = Query(
+    default=None,
+    title="Show Archived",
+    description="Whether to include archived histories.",
+)
+
+SortByQueryParam: HistorySortByEnum = Query(
+    default="update_time",
+    title="Sort attribute",
+    description="Sort index by this specified attribute",
+)
+
+SortDescQueryParam: bool = Query(
+    default=True,
+    title="Sort Descending",
+    description="Sort in descending order?",
 )
 
 
 class DeleteHistoryPayload(BaseModel):
     purge: bool = Field(
         default=False, title="Purge", description="Whether to definitely remove this history from disk."
     )
 
 
+class DeleteHistoriesPayload(BaseModel):
+    ids: Annotated[List[DecodedDatabaseIdField], Field(title="IDs", description="List of history IDs to be deleted.")]
+    purge: Annotated[
+        bool, Field(default=False, title="Purge", description="Whether to definitely remove this history from disk.")
+    ]
+
+
+class UndeleteHistoriesPayload(BaseModel):
+    ids: Annotated[List[DecodedDatabaseIdField], Field(title="IDs", description="List of history IDs to be undeleted.")]
+
+
 @as_form
 class CreateHistoryFormData(CreateHistoryPayload):
     """Uses Form data instead of JSON"""
 
 
 @router.cbv
 class FastAPIHistories:
     service: HistoriesService = depends(HistoriesService)
 
     @router.get(
         "/api/histories",
-        summary="Returns histories for the current user.",
+        summary="Returns histories available to the current user.",
+        response_model_exclude_unset=True,
     )
     def index(
         self,
+        response: Response,
         trans: ProvidesHistoryContext = DependsOnTrans,
+        limit: Optional[int] = LimitQueryParam,
+        offset: Optional[int] = OffsetQueryParam,
+        show_own: bool = ShowOwnQueryParam,
+        show_published: bool = ShowPublishedQueryParam,
+        show_shared: bool = ShowSharedQueryParam,
+        show_archived: Optional[bool] = ShowArchivedQueryParam,
+        sort_by: HistorySortByEnum = SortByQueryParam,
+        sort_desc: bool = SortDescQueryParam,
+        search: Optional[str] = SearchQueryParam,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         all: Optional[bool] = AllHistoriesQueryParam,
         deleted: Optional[bool] = Query(  # This is for backward compatibility but looks redundant
             default=False,
             title="Deleted Only",
             description="Whether to return only deleted items.",
             deprecated=True,  # Marked as deprecated as it seems just like '/api/histories/deleted'
         ),
     ) -> List[AnyHistoryView]:
-        return self.service.index(
-            trans, serialization_params, filter_query_params, deleted_only=deleted, all_histories=all
-        )
+        if search is None:
+            return self.service.index(
+                trans, serialization_params, filter_query_params, deleted_only=deleted, all_histories=all
+            )
+        else:
+            payload = HistoryIndexQueryPayload.model_construct(
+                show_own=show_own,
+                show_published=show_published,
+                show_shared=show_shared,
+                show_archived=show_archived,
+                sort_by=sort_by,
+                sort_desc=sort_desc,
+                limit=limit,
+                offset=offset,
+                search=search,
+            )
+            entries, total_matches = self.service.index_query(
+                trans, payload, serialization_params, include_total_count=True
+            )
+            response.headers["total_matches"] = str(total_matches)
+            return entries
 
     @router.get(
         "/api/histories/count",
         summary="Returns number of histories for the current user.",
     )
     def count(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
     ) -> int:
         return self.service.count(trans)
 
     @router.get(
         "/api/histories/deleted",
         summary="Returns deleted histories for the current user.",
+        response_model_exclude_unset=True,
     )
     def index_deleted(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         all: Optional[bool] = AllHistoriesQueryParam,
@@ -157,26 +241,28 @@
         return self.service.index(
             trans, serialization_params, filter_query_params, deleted_only=True, all_histories=all
         )
 
     @router.get(
         "/api/histories/published",
         summary="Return all histories that are published.",
+        response_model_exclude_unset=True,
     )
     def published(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> List[AnyHistoryView]:
         return self.service.published(trans, serialization_params, filter_query_params)
 
     @router.get(
         "/api/histories/shared_with_me",
         summary="Return all histories that are shared with the current user.",
+        response_model_exclude_unset=True,
     )
     def shared_with_me(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> List[AnyHistoryView]:
@@ -202,81 +288,84 @@
         )
         response.headers["total_matches"] = str(total_matches)
         return archived_histories
 
     @router.get(
         "/api/histories/most_recently_used",
         summary="Returns the most recently used history of the user.",
+        response_model_exclude_unset=True,
     )
     def show_recent(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryView:
         return self.service.show(trans, serialization_params)
 
     @router.get(
         "/api/histories/{history_id}",
         name="history",
         summary="Returns the history with the given ID.",
+        response_model_exclude_unset=True,
     )
     def show(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryView:
         return self.service.show(trans, serialization_params, history_id)
 
     @router.post(
         "/api/histories/{history_id}/prepare_store_download",
         summary="Return a short term storage token to monitor download of the history.",
     )
     def prepare_store_download(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: StoreExportPayload = Body(...),
     ) -> AsyncFile:
         return self.service.prepare_download(
             trans,
             history_id,
             payload=payload,
         )
 
     @router.post(
         "/api/histories/{history_id}/write_store",
         summary="Prepare history for export-style download and write to supplied URI.",
     )
     def write_store(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: WriteStoreToPayload = Body(...),
     ) -> AsyncTaskResultSummary:
         return self.service.write_store(
             trans,
             history_id,
             payload=payload,
         )
 
     @router.get(
         "/api/histories/{history_id}/citations",
         summary="Return all the citations for the tools used to produce the datasets in the history.",
     )
     def citations(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> List[Any]:
         return self.service.citations(trans, history_id)
 
     @router.post(
         "/api/histories",
         summary="Creates a new history.",
+        response_model_exclude_unset=True,
     )
     def create(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         payload: CreateHistoryPayload = Depends(CreateHistoryFormData.as_form),  # type: ignore[attr-defined]
         payload_as_json: Optional[Any] = Depends(try_get_request_body_as_json),
         serialization_params: SerializationParams = Depends(query_serialization_params),
@@ -285,64 +374,105 @@
         # This action needs to work both with json and x-www-form-urlencoded payloads.
         # The way to support different content types on the same path operation is reading
         # the request directly and parse it depending on the content type.
         # We will assume x-www-form-urlencoded (payload) by default to deal with possible file uploads
         # and if the content type is explicitly JSON, we will use payload_as_json instead.
         # See https://github.com/tiangolo/fastapi/issues/990#issuecomment-639615888
         if payload_as_json:
-            payload = CreateHistoryPayload.parse_obj(payload_as_json)
+            payload = CreateHistoryPayload.model_validate(payload_as_json)
         return self.service.create(trans, payload, serialization_params)
 
     @router.delete(
         "/api/histories/{history_id}",
         summary="Marks the history with the given ID as deleted.",
+        response_model_exclude_unset=True,
     )
     def delete(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         purge: bool = Query(default=False),
         payload: Optional[DeleteHistoryPayload] = Body(default=None),
     ) -> AnyHistoryView:
         if payload:
             purge = payload.purge
         return self.service.delete(trans, history_id, serialization_params, purge)
 
+    @router.put(
+        "/api/histories/batch/delete",
+        summary="Marks several histories with the given IDs as deleted.",
+        response_model_exclude_unset=True,
+    )
+    def batch_delete(
+        self,
+        trans: ProvidesHistoryContext = DependsOnTrans,
+        serialization_params: SerializationParams = Depends(query_serialization_params),
+        purge: bool = Query(default=False),
+        payload: DeleteHistoriesPayload = Body(...),
+    ) -> List[AnyHistoryView]:
+        if payload:
+            purge = payload.purge
+        results = []
+        for history_id in payload.ids:
+            result = self.service.delete(trans, history_id, serialization_params, purge)
+            results.append(result)
+        return results
+
     @router.post(
         "/api/histories/deleted/{history_id}/undelete",
         summary="Restores a deleted history with the given ID (that hasn't been purged).",
+        response_model_exclude_unset=True,
     )
     def undelete(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryView:
         return self.service.undelete(trans, history_id, serialization_params)
 
     @router.put(
+        "/api/histories/batch/undelete",
+        summary="Marks several histories with the given IDs as undeleted.",
+        response_model_exclude_unset=True,
+    )
+    def batch_undelete(
+        self,
+        trans: ProvidesHistoryContext = DependsOnTrans,
+        serialization_params: SerializationParams = Depends(query_serialization_params),
+        payload: UndeleteHistoriesPayload = Body(...),
+    ) -> List[AnyHistoryView]:
+        results = []
+        for history_id in payload.ids:
+            result = self.service.undelete(trans, history_id, serialization_params)
+            results.append(result)
+        return results
+
+    @router.put(
         "/api/histories/{history_id}",
         summary="Updates the values for the history with the given ID.",
+        response_model_exclude_unset=True,
     )
     def update(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: Any = Body(
             ...,
             description="Object containing any of the editable fields of the history.",
         ),
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryView:
         return self.service.update(trans, history_id, payload, serialization_params)
 
     @router.post(
         "/api/histories/from_store",
         summary="Create histories from a model store.",
+        response_model_exclude_unset=True,
     )
     def create_from_store(
         self,
         trans: ProvidesHistoryContext = DependsOnTrans,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: CreateHistoryFromStore = Body(...),
     ) -> AnyHistoryView:
@@ -364,41 +494,41 @@
         name="get_history_exports",
         summary=("Get previous history exports."),
         responses={
             200: {
                 "description": "A list of history exports",
                 "content": {
                     "application/json": {
-                        "schema": {"ref": "#/components/schemas/JobExportHistoryArchiveListResponse"},
+                        "schema": {"$ref": "#/components/schemas/JobExportHistoryArchiveListResponse"},
                     },
                     ExportTaskListResponse.__accept_type__: {
-                        "schema": {"ref": "#/components/schemas/ExportTaskListResponse"},
+                        "schema": {"$ref": "#/components/schemas/ExportTaskListResponse"},
                     },
                 },
             },
         },
     )
     def index_exports(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         limit: Optional[int] = LimitQueryParam,
         offset: Optional[int] = OffsetQueryParam,
         accept: str = Header(default="application/json", include_in_schema=False),
     ) -> Union[JobExportHistoryArchiveListResponse, ExportTaskListResponse]:
         """
         By default the legacy job-based history exports (jeha) are returned.
 
         Change the `accept` content type header to return the new task-based history exports.
         """
         use_tasks = accept == ExportTaskListResponse.__accept_type__
         exports = self.service.index_exports(trans, history_id, use_tasks, limit, offset)
         if use_tasks:
-            return ExportTaskListResponse(__root__=exports)
-        return JobExportHistoryArchiveListResponse(__root__=exports)
+            return ExportTaskListResponse(root=exports)
+        return JobExportHistoryArchiveListResponse(root=exports)
 
     @router.put(  # PUT instead of POST because multiple requests should just result in one object being created.
         "/api/histories/{history_id}/exports",
         summary=("Start job (if needed) to create history export for corresponding history."),
         responses={
             200: {
                 "description": "Object containing url to fetch export from.",
@@ -408,16 +538,16 @@
             },
         },
         deprecated=True,
     )
     def archive_export(
         self,
         response: Response,
+        history_id: HistoryIDPathParam,
         trans=DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: Optional[ExportHistoryArchivePayload] = Body(None),
     ) -> HistoryArchiveExportResult:
         """This will start a job to create a history export archive.
 
         Calling this endpoint multiple times will return the 202 status code until the archive
         has been completely generated and is ready to download. When ready, it will return
         the 200 status code along with the download link information.
@@ -444,16 +574,16 @@
                 "description": "The archive file containing the History.",
             }
         },
         deprecated=True,
     )
     def archive_download(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         jeha_id: Union[DecodedDatabaseIdField, LatestLiteral] = JehaIDPathParam,
     ):
         """
         See ``PUT /api/histories/{id}/exports`` to initiate the creation
         of the history export - when ready, that route will return 200 status
         code (instead of 202) and this route can be used to download the archive.
 
@@ -471,27 +601,27 @@
 
     @router.get(
         "/api/histories/{history_id}/custom_builds_metadata",
         summary="Returns meta data for custom builds.",
     )
     def get_custom_builds_metadata(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> CustomBuildsMetadataResponse:
         return self.service.get_custom_builds_metadata(trans, history_id)
 
     @router.post(
         "/api/histories/{history_id}/archive",
         summary="Archive a history.",
     )
     def archive_history(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: Optional[ArchiveHistoryRequestPayload] = Body(default=None),
     ) -> AnyArchivedHistoryView:
         """Marks the given history as 'archived' and returns the history.
 
         Archiving a history will remove it from the list of active histories of the user but it will still be
         accessible via the `/api/histories/{id}` or the `/api/histories/archived` endpoints.
 
@@ -506,19 +636,20 @@
         If the history was not purged after it was archived, you can restore it using the `/api/histories/{id}/archive/restore` endpoint.
         """
         return self.service.archive_history(trans, history_id, payload)
 
     @router.put(
         "/api/histories/{history_id}/archive/restore",
         summary="Restore an archived history.",
+        response_model_exclude_unset=True,
     )
     def restore_archived_history(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         force: Optional[bool] = Query(
             default=None,
             description="If true, the history will be un-archived even if it has an associated archive export record and was purged.",
         ),
     ) -> AnyHistoryView:
         """Restores an archived history and returns it.
 
@@ -532,88 +663,88 @@
 
     @router.get(
         "/api/histories/{history_id}/sharing",
         summary="Get the current sharing status of the given item.",
     )
     def sharing(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> SharingStatus:
         """Return the sharing status of the item."""
         return self.service.shareable_service.sharing(trans, history_id)
 
     @router.put(
         "/api/histories/{history_id}/enable_link_access",
         summary="Makes this item accessible by a URL link.",
     )
     def enable_link_access(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> SharingStatus:
         """Makes this item accessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.enable_link_access(trans, history_id)
 
     @router.put(
         "/api/histories/{history_id}/disable_link_access",
         summary="Makes this item inaccessible by a URL link.",
     )
     def disable_link_access(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> SharingStatus:
         """Makes this item inaccessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.disable_link_access(trans, history_id)
 
     @router.put(
         "/api/histories/{history_id}/publish",
         summary="Makes this item public and accessible by a URL link.",
     )
     def publish(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> SharingStatus:
         """Makes this item publicly available by a URL link and return the current sharing status."""
         return self.service.shareable_service.publish(trans, history_id)
 
     @router.put(
         "/api/histories/{history_id}/unpublish",
         summary="Removes this item from the published list.",
     )
     def unpublish(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
     ) -> SharingStatus:
         """Removes this item from the published list and return the current sharing status."""
         return self.service.shareable_service.unpublish(trans, history_id)
 
     @router.put(
         "/api/histories/{history_id}/share_with_users",
         summary="Share this item with specific users.",
     )
     def share_with_users(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: ShareWithPayload = Body(...),
-    ) -> ShareWithStatus:
+    ) -> ShareHistoryWithStatus:
         """Shares this item with specific users and return the current sharing status."""
         return self.service.shareable_service.share_with_users(trans, history_id, payload)
 
     @router.put(
         "/api/histories/{history_id}/slug",
         summary="Set a new slug for this shared item.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def set_slug(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         payload: SetSlugPayload = Body(...),
     ):
         """Sets a new slug to access this item by URL. The new slug must be unique."""
         self.service.shareable_service.set_slug(trans, history_id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/history_contents.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/history_contents.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on the contents of a history.
 """
+
 import logging
 from typing import (
     Any,
     Dict,
     List,
     Optional,
     Union,
@@ -13,15 +14,15 @@
 from fastapi import (
     Body,
     Depends,
     Header,
     Path,
     Query,
 )
-from pydantic.error_wrappers import ValidationError
+from pydantic import ValidationError
 from starlette import status
 from starlette.responses import (
     Response,
     StreamingResponse,
 )
 
 from galaxy import util
@@ -61,14 +62,17 @@
     DependsOnTrans,
     Router,
 )
 from galaxy.webapps.galaxy.api.common import (
     get_filter_query_params,
     get_update_permission_payload,
     get_value_filter_query_params,
+    HistoryHDCAIDPathParam,
+    HistoryIDPathParam,
+    HistoryItemIDPathParam,
     query_serialization_params,
 )
 from galaxy.webapps.galaxy.services.history_contents import (
     CreateHistoryContentFromStore,
     CreateHistoryContentPayload,
     HistoriesContentsService,
     HistoryContentsIndexJobsSummaryParams,
@@ -77,38 +81,28 @@
 )
 
 log = logging.getLogger(__name__)
 
 
 router = Router(tags=["histories"])
 
-HistoryIDPathParam: DecodedDatabaseIdField = Path(..., title="History ID", description="The ID of the History.")
-
-HistoryItemIDPathParam: DecodedDatabaseIdField = Path(
-    ..., title="History Item ID", description="The ID of the item (`HDA`/`HDCA`) contained in the history."
-)
-
-HistoryHDCAIDPathParam: DecodedDatabaseIdField = Path(
-    ..., title="History Dataset Collection ID", description="The ID of the `HDCA` contained in the history."
-)
-
 
 def ContentTypeQueryParam(default: Optional[HistoryContentType]):
     return Query(
         default=default,
         title="Content Type",
         description="The type of the target history element.",
-        example=HistoryContentType.dataset,
+        examples=[HistoryContentType.dataset],
     )
 
 
 ContentTypePathParam = Path(
     title="Content Type",
     description="The type of the target history element.",
-    example=HistoryContentType.dataset,
+    examples=[HistoryContentType.dataset],
 )
 
 FuzzyCountQueryParam = Query(
     default=None,
     title="Fuzzy Count",
     description=(
         "This value can be used to broadly restrict the magnitude "
@@ -165,15 +159,15 @@
     v: Optional[str] = Query(  # Should this be deprecated at some point and directly use the latest version by default?
         default=None,
         title="Version",
         description=(
             "Only `dev` value is allowed. Set it to use the latest version of this endpoint. "
             "**All parameters marked as `deprecated` will be ignored when this parameter is set.**"
         ),
-        example="dev",
+        examples=["dev"],
     ),
     dataset_details: Optional[str] = Query(
         default=None,
         alias="details",
         title="Dataset Details",
         description=(
             "A comma-separated list of encoded dataset IDs that will return additional (full) details "
@@ -386,19 +380,20 @@
 class FastAPIHistoryContents:
     service: HistoriesContentsService = depends(HistoriesContentsService)
 
     @router.get(
         "/api/histories/{history_id}/contents/{type}s",
         summary="Returns the contents of the given history filtered by type.",
         operation_id="history_contents__index_typed",
+        response_model_exclude_unset=True,
     )
     def index_typed(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         index_params: HistoryContentsIndexParams = Depends(get_index_query_params),
         type: HistoryContentType = ContentTypePathParam,
         legacy_params: LegacyHistoryContentsIndexParams = Depends(get_legacy_index_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         accept: str = Header(default="application/json", include_in_schema=False),
     ) -> Union[HistoryContentsResult, HistoryContentsWithStatsResult]:
@@ -428,31 +423,32 @@
         summary="Returns the contents of the given history.",
         responses={
             200: {
                 "description": ("The contents of the history that match the query."),
                 "content": {
                     "application/json": {
                         "schema": {  # HistoryContentsResult.schema(),
-                            "ref": "#/components/schemas/HistoryContentsResult"
+                            "$ref": "#/components/schemas/HistoryContentsResult"
                         },
                     },
                     HistoryContentsWithStatsResult.__accept_type__: {
                         "schema": {  # HistoryContentsWithStatsResult.schema(),
-                            "ref": "#/components/schemas/HistoryContentsWithStatsResult"
+                            "$ref": "#/components/schemas/HistoryContentsWithStatsResult"
                         },
                     },
                 },
             },
         },
         operation_id="history_contents__index",
+        response_model_exclude_unset=True,
     )
     def index(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         index_params: HistoryContentsIndexParams = Depends(get_index_query_params),
         type: Optional[str] = Query(default=None, include_in_schema=False, deprecated=True),
         legacy_params: LegacyHistoryContentsIndexParams = Depends(get_legacy_index_query_params),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
         accept: str = Header(default="application/json", include_in_schema=False),
     ) -> Union[HistoryContentsResult, HistoryContentsWithStatsResult]:
@@ -479,17 +475,17 @@
 
     @router.get(
         "/api/histories/{history_id}/contents/{type}s/{id}/jobs_summary",
         summary="Return detailed information about an `HDA` or `HDCAs` jobs.",
     )
     def show_jobs_summary(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
     ) -> AnyJobStateSummary:
         """Return detailed information about an `HDA` or `HDCAs` jobs.
 
         **Warning**: We allow anyone to fetch job state information about any object they
         can guess an encoded ID for - it isn't considered protected data. This keeps
         polling IDs as part of state calculation for large histories and collections as
@@ -498,20 +494,21 @@
         return self.service.show_jobs_summary(trans, id, contents_type=type)
 
     @router.get(
         "/api/histories/{history_id}/contents/{type}s/{id}",
         name="history_content_typed",
         summary="Return detailed information about a specific HDA or HDCA with the given `ID` within a history.",
         operation_id="history_contents__show",
+        response_model_exclude_unset=True,
     )
     def show(
         self,
+        id: HistoryItemIDPathParam,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         fuzzy_count: Optional[int] = FuzzyCountQueryParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryContentItem:
         """
         Return detailed information about an `HDA` or `HDCA` within a history.
 
@@ -527,21 +524,22 @@
 
     @router.get(
         "/api/histories/{history_id}/contents/{id}",
         name="history_content",
         summary="Return detailed information about an HDA within a history. ``/api/histories/{history_id}/contents/{type}s/{id}`` should be used instead.",
         deprecated=True,
         operation_id="history_contents__show_legacy",
+        response_model_exclude_unset=True,
     )
     def show_legacy(
         self,
+        id: HistoryItemIDPathParam,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         type: HistoryContentType = ContentTypeQueryParam(default=HistoryContentType.dataset),
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         fuzzy_count: Optional[int] = FuzzyCountQueryParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
     ) -> AnyHistoryContentItem:
         """
         Return detailed information about an `HDA` or `HDCA` within a history.
 
         **Note**: Anonymous users are allowed to get their current history contents.
@@ -556,17 +554,17 @@
 
     @router.post(
         "/api/histories/{history_id}/contents/{type}s/{id}/prepare_store_download",
         summary="Prepare a dataset or dataset collection for export-style download.",
     )
     def prepare_store_download(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         payload: StoreExportPayload = Body(...),
     ) -> AsyncFile:
         return self.service.prepare_store_download(
             trans,
             id,
             contents_type=type,
@@ -575,17 +573,17 @@
 
     @router.post(
         "/api/histories/{history_id}/contents/{type}s/{id}/write_store",
         summary="Prepare a dataset or dataset collection for export-style download and write to supplied URI.",
     )
     def write_store(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         payload: WriteStoreToPayload = Body(...),
     ) -> AsyncTaskResultSummary:
         return self.service.write_store(
             trans,
             id,
             contents_type=type,
@@ -594,16 +592,16 @@
 
     @router.get(
         "/api/histories/{history_id}/jobs_summary",
         summary="Return job state summary info for jobs, implicit groups jobs for collections or workflow invocations.",
     )
     def index_jobs_summary(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         params: HistoryContentsIndexJobsSummaryParams = Depends(get_index_jobs_summary_params),
     ) -> List[AnyJobStateSummary]:
         """Return job state summary info for jobs, implicit groups jobs for collections or workflow invocations.
 
         **Warning**: We allow anyone to fetch job state information about any object they
         can guess an encoded ID for - it isn't considered protected data. This keeps
         polling IDs as part of state calculation for large histories and collections as
@@ -615,19 +613,19 @@
         "/api/histories/{history_id}/contents/dataset_collections/{id}/download",
         summary="Download the content of a dataset collection as a `zip` archive.",
         response_class=StreamingResponse,
         operation_id="history_contents__download_collection",
     )
     def download_dataset_collection_history_content(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
         history_id: Optional[DecodedDatabaseIdField] = Path(
             description="The encoded database identifier of the History.",
         ),
-        id: DecodedDatabaseIdField = HistoryHDCAIDPathParam,
     ):
         """Download the content of a history dataset collection as a `zip` archive
         while maintaining approximate collection structure.
         """
         archive = self.service.get_dataset_collection_archive_for_download(trans, id)
         return StreamingResponse(archive.response(), headers=archive.get_headers())
 
@@ -636,16 +634,16 @@
         summary="Download the content of a dataset collection as a `zip` archive.",
         response_class=StreamingResponse,
         tags=["dataset collections"],
         operation_id="dataset_collections__download",
     )
     def download_dataset_collection(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = HistoryHDCAIDPathParam,
     ):
         """Download the content of a history dataset collection as a `zip` archive
         while maintaining approximate collection structure.
         """
         archive = self.service.get_dataset_collection_archive_for_download(trans, id)
         return StreamingResponse(archive.response(), headers=archive.get_headers())
 
@@ -663,49 +661,51 @@
             },
             501: {"description": "Required asynchronous tasks required for this operation not available."},
         },
         tags=["dataset collections"],
     )
     def prepare_collection_download(
         self,
+        id: HistoryHDCAIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = HistoryHDCAIDPathParam,
     ) -> AsyncFile:
         """The history dataset collection will be written as a `zip` archive to the
         returned short term storage object. Progress tracking this file's creation
         can be tracked with the short_term_storage API.
         """
         return self.service.prepare_collection_download(trans, id)
 
     @router.post(
         "/api/histories/{history_id}/contents/{type}s",
         summary="Create a new `HDA` or `HDCA` in the given History.",
         operation_id="history_contents__create_typed",
+        response_model_exclude_unset=True,
     )
     def create_typed(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: CreateHistoryContentPayload = Body(...),
     ) -> Union[AnyHistoryContentItem, List[AnyHistoryContentItem]]:
         """Create a new `HDA` or `HDCA` in the given History."""
         return self._create(trans, history_id, type, serialization_params, payload)
 
     @router.post(
         "/api/histories/{history_id}/contents",
         summary="Create a new `HDA` or `HDCA` in the given History.",
         deprecated=True,
         operation_id="history_contents__create",
+        response_model_exclude_unset=True,
     )
     def create(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         type: Optional[HistoryContentType] = ContentTypeQueryParam(default=None),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: CreateHistoryContentPayload = Body(...),
     ) -> Union[AnyHistoryContentItem, List[AnyHistoryContentItem]]:
         """Create a new `HDA` or `HDCA` in the given History."""
         return self._create(trans, history_id, type, serialization_params, payload)
 
@@ -723,54 +723,55 @@
 
     @router.put(
         "/api/histories/{history_id}/contents/{dataset_id}/permissions",
         summary="Set permissions of the given history dataset to the given role ids.",
     )
     def update_permissions(
         self,
+        history_id: HistoryIDPathParam,
+        dataset_id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        dataset_id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         # Using a generic Dict here as an attempt on supporting multiple aliases for the permissions params.
         payload: Dict[str, Any] = Body(
             default=...,
-            example=UpdateDatasetPermissionsPayload(),
+            examples=[UpdateDatasetPermissionsPayload().model_dump()],
         ),
     ) -> DatasetAssociationRoles:
         """Set permissions of the given history dataset to the given role ids."""
         update_payload = get_update_permission_payload(payload)
         return self.service.update_permissions(trans, dataset_id, update_payload)
 
     @router.put(
         "/api/histories/{history_id}/contents",
         summary="Batch update specific properties of a set items contained in the given History.",
+        response_model_exclude_unset=True,
     )
     def update_batch(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: UpdateHistoryContentsBatchPayload = Body(...),
     ) -> HistoryContentsResult:
         """Batch update specific properties of a set items contained in the given History.
 
         If you provide an invalid/unknown property key the request will not fail, but no changes
         will be made to the items.
         """
         result = self.service.update_batch(trans, history_id, payload, serialization_params)
-        return HistoryContentsResult.construct(__root__=result)
+        return HistoryContentsResult(root=result)
 
     @router.put(
         "/api/histories/{history_id}/contents/bulk",
         summary="Executes an operation on a set of items contained in the given History.",
     )
     def bulk_operation(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         filter_query_params: ValueFilterQueryParams = Depends(get_value_filter_query_params),
         payload: HistoryContentBulkOperationPayload = Body(...),
     ) -> HistoryContentBulkOperationResult:
         """Executes an operation on a set of items contained in the given History.
 
         The items to be processed can be explicitly set or determined by a dynamic query.
         """
@@ -778,72 +779,74 @@
 
     @router.put(
         "/api/histories/{history_id}/contents/{id}/validate",
         summary="Validates the metadata associated with a dataset within a History.",
     )
     def validate(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
     ) -> dict:  # TODO: define a response?
         """Validates the metadata associated with a dataset within a History."""
         return self.service.validate(trans, history_id, id)
 
     @router.put(
         "/api/histories/{history_id}/contents/{type}s/{id}",
         summary="Updates the values for the history content item with the given ``ID`` and path specified type.",
         operation_id="history_contents__update_typed",
+        response_model_exclude_unset=True,
     )
     def update_typed(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: UpdateHistoryContentsPayload = Body(...),
     ) -> AnyHistoryContentItem:
         """Updates the values for the history content item with the given ``ID``."""
         return self.service.update(
-            trans, history_id, id, payload.dict(exclude_unset=True), serialization_params, contents_type=type
+            trans, history_id, id, payload.model_dump(exclude_unset=True), serialization_params, contents_type=type
         )
 
     @router.put(
         "/api/histories/{history_id}/contents/{id}",
         summary="Updates the values for the history content item with the given ``ID`` and query specified type. ``/api/histories/{history_id}/contents/{type}s/{id}`` should be used instead.",
         deprecated=True,
         operation_id="history_contents__update_legacy",
+        response_model_exclude_unset=True,
     )
     def update_legacy(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypeQueryParam(default=HistoryContentType.dataset),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         payload: UpdateHistoryContentsPayload = Body(...),
     ) -> AnyHistoryContentItem:
         """Updates the values for the history content item with the given ``ID``."""
         return self.service.update(
-            trans, history_id, id, payload.dict(exclude_unset=True), serialization_params, contents_type=type
+            trans, history_id, id, payload.model_dump(exclude_unset=True), serialization_params, contents_type=type
         )
 
     @router.delete(
         "/api/histories/{history_id}/contents/{type}s/{id}",
         summary="Delete the history content with the given ``ID`` and path specified type.",
         responses=CONTENT_DELETE_RESPONSES,
         operation_id="history_contents__delete_typed",
     )
     def delete_typed(
         self,
         response: Response,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: str = Path(..., description="History ID or any string."),
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypePathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         purge: Optional[bool] = PurgeQueryParam,
         recursive: Optional[bool] = RecursiveQueryParam,
         stop_job: Optional[bool] = StopJobQueryParam,
         payload: DeleteHistoryContentPayload = Body(None),
     ):
@@ -869,17 +872,17 @@
         summary="Delete the history dataset with the given ``ID``.",
         responses=CONTENT_DELETE_RESPONSES,
         operation_id="history_contents__delete_legacy",
     )
     def delete_legacy(
         self,
         response: Response,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
         type: HistoryContentType = ContentTypeQueryParam(default=HistoryContentType.dataset),
         serialization_params: SerializationParams = Depends(query_serialization_params),
         purge: Optional[bool] = PurgeQueryParam,
         recursive: Optional[bool] = RecursiveQueryParam,
         stop_job: Optional[bool] = StopJobQueryParam,
         payload: DeleteHistoryContentPayload = Body(None),
     ):
@@ -933,16 +936,16 @@
     @router.get(
         "/api/histories/{history_id}/contents/archive/{filename}.{format}",
         summary="Build and return a compressed archive of the selected history contents.",
         operation_id="history_contents__archive_named",
     )
     def archive_named(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         filename: str = ArchiveFilenamePathParam,
         format: str = Path(
             description="Output format of the archive.",
             deprecated=True,  # Looks like is not really used?
         ),
         dry_run: Optional[bool] = DryRunQueryParam,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
@@ -958,33 +961,37 @@
     @router.get(
         "/api/histories/{history_id}/contents/archive",
         summary="Build and return a compressed archive of the selected history contents.",
         operation_id="history_contents__archive",
     )
     def archive(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         filename: Optional[str] = ArchiveFilenameQueryParam,
         dry_run: Optional[bool] = DryRunQueryParam,
         filter_query_params: FilterQueryParams = Depends(get_filter_query_params),
     ):
         """Build and return a compressed archive of the selected history contents.
 
         **Note**: this is a volatile endpoint and settings and behavior may change."""
         archive = self.service.archive(trans, history_id, filter_query_params, filename, dry_run)
         if isinstance(archive, HistoryContentsArchiveDryRunResult):
             return archive
         return StreamingResponse(archive.response(), headers=archive.get_headers())
 
-    @router.post("/api/histories/{history_id}/contents_from_store", summary="Create contents from store.")
+    @router.post(
+        "/api/histories/{history_id}/contents_from_store",
+        summary="Create contents from store.",
+        response_model_exclude_unset=True,
+    )
     def create_from_store(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         serialization_params: SerializationParams = Depends(query_serialization_params),
         create_payload: CreateHistoryContentFromStore = Body(...),
     ) -> List[AnyHistoryContentItem]:
         """
         Create history contents from model store.
         Input can be a tarfile created with build_objects script distributed
         with galaxy-data, from an exported history with files stripped out,
@@ -994,34 +1001,35 @@
 
     @router.post(
         "/api/histories/{history_id}/contents/datasets/{id}/materialize",
         summary="Materialize a deferred dataset into real, usable dataset.",
     )
     def materialize_dataset(
         self,
+        history_id: HistoryIDPathParam,
+        id: HistoryItemIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
-        id: DecodedDatabaseIdField = HistoryItemIDPathParam,
     ) -> AsyncTaskResultSummary:
-        materialize_request = MaterializeDatasetInstanceRequest.construct(
+        # values are already validated, use model_construct
+        materialize_request = MaterializeDatasetInstanceRequest.model_construct(
             history_id=history_id,
             source=DatasetSourceType.hda,
             content=id,
         )
         rval = self.service.materialize(trans, materialize_request)
         return rval
 
     @router.post(
         "/api/histories/{history_id}/materialize",
         summary="Materialize a deferred library or HDA dataset into real, usable dataset in specified history.",
     )
     def materialize_to_history(
         self,
+        history_id: HistoryIDPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        history_id: DecodedDatabaseIdField = HistoryIDPathParam,
         materialize_api_payload: MaterializeDatasetInstanceAPIRequest = Body(...),
     ) -> AsyncTaskResultSummary:
-        materialize_request: MaterializeDatasetInstanceRequest = MaterializeDatasetInstanceRequest.construct(
-            history_id=history_id, **materialize_api_payload.dict()
+        materialize_request: MaterializeDatasetInstanceRequest = MaterializeDatasetInstanceRequest.model_construct(
+            history_id=history_id, **materialize_api_payload.model_dump()
         )
         rval = self.service.materialize(trans, materialize_request)
         return rval
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/item_tags.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/item_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 API operations related to tagging items.
 """
+
 import logging
 
 from fastapi import (
     Body,
     Path,
 )
+from typing_extensions import Annotated
 
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.managers.item_tags import ItemTagsManager
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.item_tags import (
     ItemTagsCreatePayload,
     ItemTagsListResponse,
@@ -38,43 +40,43 @@
                 f"/api/{prefix}/{{{tagged_item_id}}}/tags",
                 tags=[api_docs_tag],
                 summary=f"Show tags based on {tagged_item_id}",
                 openapi_extra=extra_path_params,
             )
             def index(
                 self,
+                item_id: Annotated[DecodedDatabaseIdField, Path(..., title="Item ID", alias=tagged_item_id)],
                 trans: ProvidesAppContext = DependsOnTrans,
-                item_id: DecodedDatabaseIdField = Path(..., title="Item ID", alias=tagged_item_id),
             ) -> ItemTagsListResponse:
                 return self.manager.index(trans, tagged_item_class, item_id)
 
             @router.get(
                 f"/api/{prefix}/{{{tagged_item_id}}}/tags/{{tag_name}}",
                 tags=[api_docs_tag],
                 summary=f"Show tag based on {tagged_item_id}",
                 openapi_extra=extra_path_params,
             )
             def show(
                 self,
+                item_id: Annotated[DecodedDatabaseIdField, Path(..., title="Item ID", alias=tagged_item_id)],
                 trans: ProvidesAppContext = DependsOnTrans,
-                item_id: DecodedDatabaseIdField = Path(..., title="Item ID", alias=tagged_item_id),
                 tag_name: str = Path(..., title="Tag Name"),
             ) -> ItemTagsResponse:
                 return self.manager.show(trans, tagged_item_class, item_id, tag_name)
 
             @router.post(
                 f"/api/{prefix}/{{{tagged_item_id}}}/tags/{{tag_name}}",
                 tags=[api_docs_tag],
                 summary=f"Create tag based on {tagged_item_id}",
                 openapi_extra=extra_path_params,
             )
             def create(
                 self,
+                item_id: Annotated[DecodedDatabaseIdField, Path(..., title="Item ID", alias=tagged_item_id)],
                 trans: ProvidesAppContext = DependsOnTrans,
-                item_id: DecodedDatabaseIdField = Path(..., title="Item ID", alias=tagged_item_id),
                 tag_name: str = Path(..., title="Tag Name"),
                 payload: ItemTagsCreatePayload = Body(None),
             ) -> ItemTagsResponse:
                 if payload is None:
                     payload = ItemTagsCreatePayload()
                 return self.manager.create(trans, tagged_item_class, item_id, tag_name, payload)
 
@@ -82,31 +84,31 @@
                 f"/api/{prefix}/{{{tagged_item_id}}}/tags/{{tag_name}}",
                 tags=[api_docs_tag],
                 summary=f"Update tag based on {tagged_item_id}",
                 openapi_extra=extra_path_params,
             )
             def update(
                 self,
+                item_id: Annotated[DecodedDatabaseIdField, Path(..., title="Item ID", alias=tagged_item_id)],
                 trans: ProvidesAppContext = DependsOnTrans,
-                item_id: DecodedDatabaseIdField = Path(..., title="Item ID", alias=tagged_item_id),
                 tag_name: str = Path(..., title="Tag Name"),
                 payload: ItemTagsCreatePayload = Body(...),
             ) -> ItemTagsResponse:
                 return self.manager.create(trans, tagged_item_class, item_id, tag_name, payload)
 
             @router.delete(
                 f"/api/{prefix}/{{{tagged_item_id}}}/tags/{{tag_name}}",
                 tags=[api_docs_tag],
                 summary=f"Delete tag based on {tagged_item_id}",
                 openapi_extra=extra_path_params,
             )
             def delete(
                 self,
+                item_id: Annotated[DecodedDatabaseIdField, Path(..., title="Item ID", alias=tagged_item_id)],
                 trans: ProvidesAppContext = DependsOnTrans,
-                item_id: DecodedDatabaseIdField = Path(..., title="Item ID", alias=tagged_item_id),
                 tag_name: str = Path(..., title="Tag Name"),
             ) -> bool:
                 return self.manager.delete(trans, tagged_item_class, item_id, tag_name)
 
         return Temp
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_files.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_files.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """ API for asynchronous job running mechanisms can use to fetch or put files
 related to running and queued jobs.
 """
+
 import logging
 import os
+import re
 import shutil
 
 from galaxy import (
     exceptions,
     util,
 )
 from galaxy.model import Job
@@ -95,14 +97,26 @@
                 " nginx_upload_module but Galaxy is not"
                 " configured to recognize it"
             )
             assert file_path.startswith(
                 upload_store
             ), f"Filename provided by nginx ({file_path}) is not in correct directory ({upload_store})"
             input_file = open(file_path)
+        elif "session_id" in payload:
+            # code stolen from basic.py
+            session_id = payload["session_id"]
+            upload_store = (
+                trans.app.config.tus_upload_store_job_files
+                or trans.app.config.tus_upload_store
+                or trans.app.config.new_file_path
+            )
+            if re.match(r"^[\w-]+$", session_id) is None:
+                raise ValueError("Invalid session id format.")
+            local_filename = os.path.abspath(os.path.join(upload_store, session_id))
+            input_file = open(local_filename)
         else:
             input_file = payload.get("file", payload.get("__file", None)).file
         target_dir = os.path.dirname(path)
         util.safe_makedirs(target_dir)
         try:
             shutil.move(input_file.name, path)
         finally:
@@ -110,14 +124,55 @@
                 input_file.close()
             except OSError:
                 # Fails to close file if not using nginx upload because the
                 # tempfile has moved and Python wants to delete it.
                 pass
         return {"message": "ok"}
 
+    @expose_api_anonymous_and_sessionless
+    def tus_patch(self, trans, **kwds):
+        """
+        Exposed as PATCH /api/job_files/resumable_upload.
+
+        I think based on the docs, a separate tusd server is needed for job files if
+        also hosting one for use facing uploads.
+
+        Setting up tusd for job files should just look like (I think):
+
+        tusd -host localhost -port 1080 -upload-dir=<galaxy_root>/database/tmp
+
+        See more discussion of checking upload access, but we shouldn't need the
+        API key and session stuff the user upload tusd server should be configured with.
+
+        Also shouldn't need a hooks endpoint for this reason but if you want to add one
+        the target CLI entry would be -hooks-http=<galaxy_url>/api/job_files/tus_hooks
+        and the action is featured below.
+
+        I would love to check the job state with __authorize_job_access on the first
+        POST but it seems like TusMiddleware doesn't default to coming in here for that
+        initial POST the way it does for the subsequent PATCHes. Ultimately, the upload
+        is still authorized before the write done with POST /api/jobs/<job_id>/files
+        so I think there is no route here to mess with user data - the worst of the security
+        issues that can be caused is filling up the sever with needless files that aren't
+        acted on. Since this endpoint is not meant for public consumption - all the job
+        files stuff and the TUS server should be blocked to public IPs anyway and restricted
+        to your Pulsar servers and similar targeting could be accomplished with a user account
+        and the user facing upload endpoints.
+        """
+        return None
+
+    @expose_api_anonymous_and_sessionless
+    def tus_hooks(self, trans, **kwds):
+        """No-op but if hook specified the way we do for user upload it would hit this action.
+
+        Exposed as PATCH /api/job_files/tus_hooks and documented in the docstring for
+        tus_patch.
+        """
+        pass
+
     def __authorize_job_access(self, trans, encoded_job_id, **kwargs):
         for key in ["path", "job_key"]:
             if key not in kwargs:
                 error_message = f"Job files action requires a valid '{key}'."
                 raise exceptions.ObjectAttributeMissingException(error_message)
 
         job_id = trans.security.decode_id(encoded_job_id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_lock.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_lock.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_ports.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_ports.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ API for asynchronous job running mechanisms can use to fetch or put files
 related to running and queued jobs.
 """
+
 from galaxy.job_execution.ports import JobPortsView
 from galaxy.structured_app import StructuredApp
 from galaxy.web import expose_api_anonymous_and_sessionless
 from . import BaseGalaxyAPIController
 
 
 class JobPortsAPIController(BaseGalaxyAPIController):
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/job_tokens.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/job_tokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ API asynchronous job running mechanisms can use to get a fresh OIDC token.
 """
+
 import logging
 
 from fastapi import Query
 from fastapi.responses import PlainTextResponse
 
 from galaxy import (
     exceptions,
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/jobs.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/jobs.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,28 +6,25 @@
 
 import logging
 from datetime import (
     date,
     datetime,
 )
 from typing import (
-    Any,
-    Dict,
     List,
     Optional,
     Union,
 )
 
 from fastapi import (
     Body,
     Depends,
     Path,
     Query,
 )
-from pydantic import Required
 from typing_extensions import Annotated
 
 from galaxy import exceptions
 from galaxy.managers.context import (
     ProvidesHistoryContext,
     ProvidesUserContext,
 )
@@ -45,19 +42,21 @@
     JobDisplayParametersSummary,
     JobErrorSummary,
     JobInputAssociation,
     JobInputSummary,
     JobOutputAssociation,
     ReportJobErrorPayload,
     SearchJobsPayload,
+    ShowFullJobResponse,
 )
 from galaxy.schema.schema import (
     DatasetSourceType,
     JobIndexSortByEnum,
     JobMetric,
+    JobSummary,
 )
 from galaxy.schema.types import OffsetNaiveDatetime
 from galaxy.web import expose_api_anonymous
 from galaxy.webapps.base.controller import UsesVisualizationMixin
 from galaxy.webapps.galaxy.api import (
     BaseGalaxyAPIController,
     depends,
@@ -146,14 +145,20 @@
 
 InvocationIdQueryParam: Optional[DecodedDatabaseIdField] = Query(
     default=None,
     title="Invocation ID",
     description="Limit listing of jobs to those that match the specified workflow invocation ID. If none, jobs from any workflow invocation (or from no workflows) may be returned.",
 )
 
+ImplicitCollectionJobsIdQueryParam: Optional[DecodedDatabaseIdField] = Query(
+    default=None,
+    title="Implicit Collection Jobs ID",
+    description="Limit listing of jobs to those that match the specified implicit collection job ID. If none, jobs from any implicit collection execution (or from no implicit collection execution) may be returned.",
+)
+
 SortByQueryParam: JobIndexSortByEnum = Query(
     default=JobIndexSortByEnum.update_time,
     title="Sort By",
     description="Sort results by specified field.",
 )
 
 LimitQueryParam: int = Query(default=500, title="Limit", description="Maximum number of jobs to return.")
@@ -185,19 +190,19 @@
 )
 HdaLddaQueryParam: DatasetSourceType = Query(
     title="HDA or LDDA",
     description="Whether this dataset belongs to a history (HDA) or a library (LDDA).",
 )
 
 
-JobIdPathParam: DecodedDatabaseIdField = Path(title="Job ID", description="The ID of the job")
-DatasetIdPathParam: DecodedDatabaseIdField = Path(title="Dataset ID", description="The ID of the dataset")
+JobIdPathParam = Annotated[DecodedDatabaseIdField, Path(title="Job ID", description="The ID of the job")]
+DatasetIdPathParam = Annotated[DecodedDatabaseIdField, Path(title="Dataset ID", description="The ID of the dataset")]
 
-ReportErrorBody = Body(default=Required, title="Report error", description="The values to report an Error")
-SearchJobBody = Body(default=Required, title="Search job", description="The values to search an Job")
+ReportErrorBody = Body(default=..., title="Report error", description="The values to report an Error")
+SearchJobBody = Body(default=..., title="Search job", description="The values to search an Job")
 DeleteJobBody = Body(title="Delete/cancel job", description="The values to delete/cancel a job")
 
 
 @router.cbv
 class FastAPIJobs:
     service: JobsService = depends(JobsService)
 
@@ -212,46 +217,48 @@
         tool_ids: Optional[List[str]] = Depends(query_parameter_as_list(ToolIdQueryParam)),
         tool_ids_like: Optional[List[str]] = Depends(query_parameter_as_list(ToolIdLikeQueryParam)),
         date_range_min: Optional[Union[datetime, date]] = DateRangeMinQueryParam,
         date_range_max: Optional[Union[datetime, date]] = DateRangeMaxQueryParam,
         history_id: Optional[DecodedDatabaseIdField] = HistoryIdQueryParam,
         workflow_id: Optional[DecodedDatabaseIdField] = WorkflowIdQueryParam,
         invocation_id: Optional[DecodedDatabaseIdField] = InvocationIdQueryParam,
+        implicit_collection_jobs_id: Optional[DecodedDatabaseIdField] = ImplicitCollectionJobsIdQueryParam,
         order_by: JobIndexSortByEnum = SortByQueryParam,
         search: Optional[str] = SearchQueryParam,
         limit: int = LimitQueryParam,
         offset: int = OffsetQueryParam,
-    ) -> List[Dict[str, Any]]:
-        payload = JobIndexPayload.construct(
+    ) -> List[Union[ShowFullJobResponse, EncodedJobDetails, JobSummary]]:
+        payload = JobIndexPayload.model_construct(
             states=states,
             user_details=user_details,
             user_id=user_id,
             view=view,
             tool_ids=tool_ids,
             tool_ids_like=tool_ids_like,
             date_range_min=date_range_min,
             date_range_max=date_range_max,
             history_id=history_id,
             workflow_id=workflow_id,
             invocation_id=invocation_id,
+            implicit_collection_jobs_id=implicit_collection_jobs_id,
             order_by=order_by,
             search=search,
             limit=limit,
             offset=offset,
         )
         return self.service.index(trans, payload)
 
     @router.get(
         "/api/jobs/{job_id}/common_problems",
         name="check_common_problems",
         summary="Check inputs and job for common potential problems to aid in error reporting",
     )
     def common_problems(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> JobInputSummary:
         job = self.service.get_job(trans=trans, job_id=job_id)
         seen_ids = set()
         has_empty_inputs = False
         has_duplicate_inputs = False
         for job_input_assoc in job.input_datasets:
@@ -273,47 +280,48 @@
     @router.put(
         "/api/jobs/{job_id}/resume",
         name="resume_paused_job",
         summary="Resumes a paused job.",
     )
     def resume(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> List[JobOutputAssociation]:
         job = self.service.get_job(trans, job_id=job_id)
         if not job:
             raise exceptions.ObjectNotFound("Could not access job with the given id")
         if job.state == job.states.PAUSED:
             job.resume()
         else:
             exceptions.RequestParameterInvalidException(f"Job with id '{job.tool_id}' is not paused")
+        # Maybe just return 202 ? What's the point of this ?
         associations = self.service.dictify_associations(trans, job.output_datasets, job.output_library_datasets)
         output_associations = []
         for association in associations:
             output_associations.append(JobOutputAssociation(name=association.name, dataset=association.dataset))
         return output_associations
 
     @router.post(
         "/api/jobs/{job_id}/error",
         name="report_error",
         summary="Submits a bug report via the API.",
     )
     def error(
         self,
         payload: Annotated[ReportJobErrorPayload, ReportErrorBody],
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> JobErrorSummary:
         # Get dataset on which this error was triggered
         dataset_id = payload.dataset_id
         dataset = self.service.hda_manager.get_accessible(id=dataset_id, user=trans.user)
         # Get job
         job = self.service.get_job(trans, job_id)
-        if dataset.creating_job.id != job.id:
+        if not dataset.creating_job or dataset.creating_job.id != job.id:
             raise exceptions.RequestParameterInvalidException("dataset_id was not created by job_id")
         tool = trans.app.toolbox.get_tool(job.tool_id, tool_version=job.tool_version) or None
         email = payload.email
         if not email and not trans.anonymous:
             email = trans.user.email
         messages = trans.app.error_reports.default_error_plugin.submit_report(
             dataset=dataset,
@@ -329,15 +337,15 @@
     @router.get(
         "/api/jobs/{job_id}/inputs",
         name="get_inputs",
         summary="Returns input datasets created by a job.",
     )
     def inputs(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> List[JobInputAssociation]:
         job = self.service.get_job(trans=trans, job_id=job_id)
         associations = self.service.dictify_associations(trans, job.input_datasets, job.input_library_datasets)
         input_associations = []
         for association in associations:
             input_associations.append(JobInputAssociation(name=association.name, dataset=association.dataset))
@@ -346,15 +354,15 @@
     @router.get(
         "/api/jobs/{job_id}/outputs",
         name="get_outputs",
         summary="Returns output datasets created by a job.",
     )
     def outputs(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> List[JobOutputAssociation]:
         job = self.service.get_job(trans=trans, job_id=job_id)
         associations = self.service.dictify_associations(trans, job.output_datasets, job.output_library_datasets)
         output_associations = []
         for association in associations:
             output_associations.append(JobOutputAssociation(name=association.name, dataset=association.dataset))
@@ -363,15 +371,15 @@
     @router.get(
         "/api/jobs/{job_id}/parameters_display",
         name="resolve_parameters_display",
         summary="Resolve parameters as a list for nested display.",
     )
     def parameters_display_by_job(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         hda_ldda: Annotated[Optional[DatasetSourceType], DeprecatedHdaLddaQueryParam] = DatasetSourceType.hda,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> JobDisplayParametersSummary:
         """
         Resolve parameters as a list for nested display.
         This API endpoint is unstable and tied heavily to Galaxy's JS client code,
         this endpoint will change frequently.
@@ -384,15 +392,15 @@
         "/api/datasets/{dataset_id}/parameters_display",
         name="resolve_parameters_display",
         summary="Resolve parameters as a list for nested display.",
         deprecated=True,
     )
     def parameters_display_by_dataset(
         self,
-        dataset_id: Annotated[DecodedDatabaseIdField, DatasetIdPathParam],
+        dataset_id: DatasetIdPathParam,
         hda_ldda: Annotated[DatasetSourceType, HdaLddaQueryParam] = DatasetSourceType.hda,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> JobDisplayParametersSummary:
         """
         Resolve parameters as a list for nested display.
         This API endpoint is unstable and tied heavily to Galaxy's JS client code,
         this endpoint will change frequently.
@@ -403,15 +411,15 @@
     @router.get(
         "/api/jobs/{job_id}/metrics",
         name="get_metrics",
         summary="Return job metrics for specified job.",
     )
     def metrics_by_job(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         hda_ldda: Annotated[Optional[DatasetSourceType], DeprecatedHdaLddaQueryParam] = DatasetSourceType.hda,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> List[Optional[JobMetric]]:
         hda_ldda_str = hda_ldda or "hda"
         job = self.service.get_job(trans, job_id=job_id, hda_ldda=hda_ldda_str)
         return [JobMetric(**metric) for metric in summarize_job_metrics(trans, job)]
 
@@ -419,30 +427,30 @@
         "/api/datasets/{dataset_id}/metrics",
         name="get_metrics",
         summary="Return job metrics for specified job.",
         deprecated=True,
     )
     def metrics_by_dataset(
         self,
-        dataset_id: Annotated[DecodedDatabaseIdField, DatasetIdPathParam],
+        dataset_id: DatasetIdPathParam,
         hda_ldda: Annotated[DatasetSourceType, HdaLddaQueryParam] = DatasetSourceType.hda,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> List[Optional[JobMetric]]:
         job = self.service.get_job(trans, dataset_id=dataset_id, hda_ldda=hda_ldda)
         return [JobMetric(**metric) for metric in summarize_job_metrics(trans, job)]
 
     @router.get(
         "/api/jobs/{job_id}/destination_params",
         name="destination_params_job",
         summary="Return destination parameters for specified job.",
         require_admin=True,
     )
     def destination_params(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> JobDestinationParams:
         job = self.service.get_job(trans, job_id=job_id)
         return JobDestinationParams(**summarize_destination_params(trans, job))
 
     @router.post(
         "/api/jobs/search",
@@ -493,28 +501,31 @@
     @router.get(
         "/api/jobs/{job_id}",
         name="show_job",
         summary="Return dictionary containing description of job data.",
     )
     def show(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         full: Annotated[Optional[bool], FullShowQueryParam] = False,
         trans: ProvidesUserContext = DependsOnTrans,
-    ) -> Dict[str, Any]:
-        return self.service.show(trans, job_id, bool(full))
+    ) -> Union[ShowFullJobResponse, EncodedJobDetails]:
+        if full:
+            return ShowFullJobResponse(**self.service.show(trans, job_id, bool(full)))
+        else:
+            return EncodedJobDetails(**self.service.show(trans, job_id, bool(full)))
 
     @router.delete(
         "/api/jobs/{job_id}",
         name="cancel_job",
         summary="Cancels specified job",
     )
     def delete(
         self,
-        job_id: Annotated[DecodedDatabaseIdField, JobIdPathParam],
+        job_id: JobIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
         payload: Annotated[Optional[DeleteJobPayload], DeleteJobBody] = None,
     ) -> bool:
         job = self.service.get_job(trans=trans, job_id=job_id)
         if payload:
             message = payload.message
         else:
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/libraries.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/libraries.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """
 API operations on a data library.
 """
+
 import logging
 from typing import (
     List,
     Optional,
     Union,
 )
 
 from fastapi import (
     Body,
-    Path,
     Query,
 )
 
 from galaxy.managers.context import ProvidesUserContext
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import (
     CreateLibrariesFromStore,
     CreateLibraryPayload,
     DeleteLibraryPayload,
     LegacyLibraryPermissionsPayload,
     LibraryAvailablePermissions,
     LibraryCurrentPermissions,
@@ -32,28 +31,25 @@
     UpdateLibraryPayload,
 )
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import LibraryIdPathParam
 from galaxy.webapps.galaxy.services.libraries import LibrariesService
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["libraries"])
 
 DeletedQueryParam: Optional[bool] = Query(
     default=None, title="Display deleted", description="Whether to include deleted libraries in the result."
 )
 
-LibraryIdPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Library ID", description="The encoded identifier of the Library."
-)
-
 UndeleteQueryParam: Optional[bool] = Query(
     default=None, title="Undelete", description="Whether to restore a deleted library."
 )
 
 
 @router.cbv
 class FastAPILibraries:
@@ -84,16 +80,16 @@
 
     @router.get(
         "/api/libraries/{id}",
         summary="Returns summary information about a particular library.",
     )
     def show(
         self,
+        id: LibraryIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = LibraryIdPathParam,
     ) -> LibrarySummary:
         """Returns summary information about a particular library."""
         return self.service.show(trans, id)
 
     @router.post(
         "/api/libraries",
         summary="Creates a new library and returns its summary information.",
@@ -121,32 +117,32 @@
 
     @router.patch(
         "/api/libraries/{id}",
         summary="Updates the information of an existing library.",
     )
     def update(
         self,
+        id: LibraryIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = LibraryIdPathParam,
         payload: UpdateLibraryPayload = Body(...),
     ) -> LibrarySummary:
         """
         Updates the information of an existing library.
         """
         return self.service.update(trans, id, payload)
 
     @router.delete(
         "/api/libraries/{id}",
         summary="Marks the specified library as deleted (or undeleted).",
         require_admin=True,
     )
     def delete(
         self,
+        id: LibraryIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = LibraryIdPathParam,
         undelete: Optional[bool] = UndeleteQueryParam,
         payload: Optional[DeleteLibraryPayload] = Body(default=None),
     ) -> LibrarySummary:
         """Marks the specified library as deleted (or undeleted).
         Currently, only admin users can delete or restore libraries."""
         if payload:
             undelete = payload.undelete
@@ -154,16 +150,16 @@
 
     @router.get(
         "/api/libraries/{id}/permissions",
         summary="Gets the current or available permissions of a particular library.",
     )
     def get_permissions(
         self,
+        id: LibraryIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = LibraryIdPathParam,
         scope: Optional[LibraryPermissionScope] = Query(
             None,
             title="Scope",
             description="The scope of the permissions to retrieve. Either the `current` permissions or the `available`.",
         ),
         is_library_access: Optional[bool] = Query(
             None,
@@ -194,24 +190,24 @@
 
     @router.post(
         "/api/libraries/{id}/permissions",
         summary="Sets the permissions to access and manipulate a library.",
     )
     def set_permissions(
         self,
+        id: LibraryIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = LibraryIdPathParam,
         action: Optional[LibraryPermissionAction] = Query(
             default=None,
             title="Action",
             description="Indicates what action should be performed on the Library.",
         ),
         payload: Union[
             LibraryPermissionsPayload,
             LegacyLibraryPermissionsPayload,
         ] = Body(...),
     ) -> Union[LibraryLegacySummary, LibraryCurrentPermissions]:  # Old legacy response
         """Sets the permissions to access and manipulate a library."""
-        payload_dict = payload.dict(by_alias=True)
+        payload_dict = payload.model_dump(by_alias=True)
         if isinstance(payload, LibraryPermissionsPayload) and action is not None:
             payload_dict["action"] = action
         return self.service.set_permissions(trans, id, payload_dict)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/library_contents.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_contents.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on the contents of a data library.
 """
+
 import logging
 from typing import Optional
 
 from galaxy import (
     exceptions,
     managers,
     util,
@@ -328,27 +329,26 @@
         replace_dataset: Optional[LibraryDataset] = None
         upload_option = kwd.get("upload_option", "upload_file")
         dbkey = kwd.get("dbkey", "?")
         if isinstance(dbkey, list):
             last_used_build = dbkey[0]
         else:
             last_used_build = dbkey
-        roles = kwd.get("roles", "")
         is_admin = trans.user_is_admin
         current_user_roles = trans.get_current_user_roles()
         folder = trans.sa_session.get(LibraryFolder, folder_id)
         self._check_access(trans, is_admin, folder, current_user_roles)
         self._check_add(trans, is_admin, folder, current_user_roles)
         library = folder.parent_library
         if folder and last_used_build in ["None", None, "?"]:
             last_used_build = folder.genome_build
         error = False
         if upload_option == "upload_paths":
             validate_path_upload(trans)  # Duplicate check made in _upload_dataset.
-        elif roles:
+        elif roles := kwd.get("roles", ""):
             # Check to see if the user selected roles to associate with the DATASET_ACCESS permission
             # on the dataset that would cause accessibility issues.
             vars = dict(DATASET_ACCESS_in=roles)
             permissions, in_roles, error, message = trans.app.security_agent.derive_roles_from_access(
                 trans, library.id, "api", library=True, **vars
             )
         if error:
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/library_datasets.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/library_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """API operations on the library datasets."""
+
 import glob
 import logging
 import os
 import os.path
 import string
 from json import dumps
 
@@ -430,16 +431,15 @@
             kwd.update(payload)
         kwd["space_to_tab"] = False
         kwd["to_posix_lines"] = True
         kwd["dbkey"] = kwd.get("dbkey", "?")
         kwd["file_type"] = kwd.get("file_type", "auto")
         kwd["link_data_only"] = "link_to_files" if util.string_as_bool(kwd.get("link_data", False)) else "copy_files"
         kwd["tag_using_filenames"] = util.string_as_bool(kwd.get("tag_using_filenames", None))
-        encoded_folder_id = kwd.get("encoded_folder_id", None)
-        if encoded_folder_id is not None:
+        if (encoded_folder_id := kwd.get("encoded_folder_id", None)) is not None:
             folder_id = self.folder_manager.cut_and_decode(trans, encoded_folder_id)
         else:
             raise exceptions.RequestParameterMissingException("The required attribute encoded_folder_id is missing.")
         path = kwd.get("path", None)
         if path is None:
             raise exceptions.RequestParameterMissingException("The required attribute path is missing.")
         if not isinstance(path, str):
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/licenses.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/licenses.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,31 +13,35 @@
 
 router = Router(tags=["licenses"])
 
 LicenseIdPath: str = Path(
     ...,  # Mark this Path parameter as required
     title="SPDX license short ID",
     description="The [SPDX license short identifier](https://spdx.github.io/spdx-spec/appendix-I-SPDX-license-list/)",
-    example="Apache-2.0",
+    examples=["Apache-2.0"],
 )
 
 
 @router.cbv
 class FastAPILicenses:
     licenses_manager: LicensesManager = depends(LicensesManager)
 
     @router.get(
-        "/api/licenses", summary="Lists all available SPDX licenses", response_description="List of SPDX licenses"
+        "/api/licenses",
+        public=True,
+        summary="Lists all available SPDX licenses",
+        response_description="List of SPDX licenses",
     )
     async def index(self) -> List[LicenseMetadataModel]:
         """Returns an index with all the available [SPDX licenses](https://spdx.org/licenses/)."""
         return self.licenses_manager.get_licenses()
 
     @router.get(
         "/api/licenses/{id}",
+        public=True,
         summary="Gets the SPDX license metadata associated with the short identifier",
         response_description="SPDX license metadata",
     )
     async def get(self, id=LicenseIdPath) -> LicenseMetadataModel:
         """Returns the license metadata associated with the given
         [SPDX license short ID](https://spdx.github.io/spdx-spec/appendix-I-SPDX-license-list/)."""
         return self.licenses_manager.get_license_by_id(id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/metrics.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 API operations for for querying and recording user metrics from some client
 (typically a user's browser).
 """
+
 # TODO: facade or adapter to fluentd
 
 import logging
 from typing import Any
 
 from fastapi import Body
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/notifications.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/notifications.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 """
 
 import logging
 from typing import Optional
 
 from fastapi import (
     Body,
-    Path,
     Query,
     Response,
     status,
 )
 
 from galaxy.managers.context import ProvidesUserContext
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.notifications import (
     BroadcastNotificationCreateRequest,
     BroadcastNotificationListResponse,
     BroadcastNotificationResponse,
     NotificationBroadcastUpdateRequest,
     NotificationCreatedResponse,
     NotificationCreateRequest,
@@ -29,14 +27,15 @@
     UserNotificationListResponse,
     UserNotificationPreferences,
     UserNotificationResponse,
     UserNotificationsBatchUpdateRequest,
     UserNotificationUpdateRequest,
 )
 from galaxy.schema.types import OffsetNaiveDatetime
+from galaxy.webapps.galaxy.api.common import NotificationIdPathParam
 from galaxy.webapps.galaxy.services.notifications import NotificationService
 from . import (
     depends,
     DependsOnTrans,
     Router,
 )
 
@@ -106,16 +105,16 @@
 
     @router.get(
         "/api/notifications/broadcast/{notification_id}",
         summary="Returns the information of a specific broadcasted notification.",
     )
     def get_broadcasted(
         self,
+        notification_id: NotificationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        notification_id: DecodedDatabaseIdField = Path(),
     ) -> BroadcastNotificationResponse:
         """Only Admin users can access inactive notifications (scheduled or recently expired)."""
         return self.service.get_broadcasted_notification(trans, notification_id)
 
     @router.get(
         "/api/notifications/broadcast",
         summary="Returns all currently active broadcasted notifications.",
@@ -129,45 +128,45 @@
 
     @router.get(
         "/api/notifications/{notification_id}",
         summary="Displays information about a notification received by the user.",
     )
     def show_notification(
         self,
+        notification_id: NotificationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        notification_id: DecodedDatabaseIdField = Path(),
     ) -> UserNotificationResponse:
         user = self.service.get_authenticated_user(trans)
         return self.service.get_user_notification(user, notification_id)
 
     @router.put(
         "/api/notifications/broadcast/{notification_id}",
         summary="Updates the state of a broadcasted notification.",
         require_admin=True,
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def update_broadcasted_notification(
         self,
+        notification_id: NotificationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        notification_id: DecodedDatabaseIdField = Path(),
         payload: NotificationBroadcastUpdateRequest = Body(),
     ):
         """Only Admins can update broadcasted notifications. This is useful to reschedule, edit or expire broadcasted notifications."""
         self.service.update_broadcasted_notification(trans, notification_id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.put(
         "/api/notifications/{notification_id}",
         summary="Updates the state of a notification received by the user.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def update_user_notification(
         self,
+        notification_id: NotificationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        notification_id: DecodedDatabaseIdField = Path(),
         payload: UserNotificationUpdateRequest = Body(),
     ):
         self.service.update_user_notification(trans, notification_id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.put(
         "/api/notifications",
@@ -183,16 +182,16 @@
     @router.delete(
         "/api/notifications/{notification_id}",
         summary="Deletes a notification received by the user.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def delete_user_notification(
         self,
+        notification_id: NotificationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        notification_id: DecodedDatabaseIdField = Path(),
     ):
         """When a notification is deleted, it is not immediately removed from the database, but marked as deleted.
 
         - It will not be returned in the list of notifications, but admins can still access it as long as it is not expired.
         - It will be eventually removed from the database by a background task after the expiration time.
         - Deleted notifications will be permanently deleted when the expiration time is reached.
         """
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/object_store.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/object_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on Galaxy's object store.
 """
+
 import logging
 from typing import List
 
 from fastapi import (
     Path,
     Query,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/page_revisions.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/page_revisions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API for updating Galaxy Pages
 """
+
 import logging
 
 from galaxy.managers.base import get_object
 from galaxy.managers.pages import (
     get_page_revision,
     PageManager,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/pages.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/pages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 API for updating Galaxy Pages
 """
+
 import io
 import logging
 from typing import Optional
 
 from fastapi import (
     Body,
-    Path,
     Query,
     Response,
     status,
 )
 from starlette.responses import StreamingResponse
 
 from galaxy.managers.context import ProvidesUserContext
@@ -32,14 +32,15 @@
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     IndexQueryTag,
     Router,
     search_query_param,
 )
+from galaxy.webapps.galaxy.api.common import PageIdPathParam
 from galaxy.webapps.galaxy.services.pages import PagesService
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["pages"])
 
 DeletedQueryParam: bool = Query(
@@ -47,17 +48,15 @@
 )
 
 UserIdQueryParam: Optional[DecodedDatabaseIdField] = Query(
     default=None,
     title="Encoded user ID to restrict query to, must be own id if not an admin user",
 )
 
-PageIdPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Page ID", description="The encoded database identifier of the Page."  # Required
-)
+ShowOwnQueryParam: bool = Query(default=True, title="Show pages owned by user.", description="")
 
 ShowPublishedQueryParam: bool = Query(default=True, title="Include published pages.", description="")
 
 ShowSharedQueryParam: bool = Query(default=False, title="Include pages shared with authenticated user.", description="")
 
 
 SortByQueryParam: PageSortByEnum = Query(
@@ -104,34 +103,36 @@
         response_description="A list with summary page information.",
     )
     async def index(
         self,
         response: Response,
         trans: ProvidesUserContext = DependsOnTrans,
         deleted: bool = DeletedQueryParam,
-        user_id: Optional[DecodedDatabaseIdField] = UserIdQueryParam,
+        limit: int = LimitQueryParam,
+        offset: int = OffsetQueryParam,
+        search: Optional[str] = SearchQueryParam,
+        show_own: bool = ShowOwnQueryParam,
         show_published: bool = ShowPublishedQueryParam,
         show_shared: bool = ShowSharedQueryParam,
         sort_by: PageSortByEnum = SortByQueryParam,
         sort_desc: bool = SortDescQueryParam,
-        limit: int = LimitQueryParam,
-        offset: int = OffsetQueryParam,
-        search: Optional[str] = SearchQueryParam,
+        user_id: Optional[DecodedDatabaseIdField] = UserIdQueryParam,
     ) -> PageSummaryList:
         """Get a list with summary information of all Pages available to the user."""
-        payload = PageIndexQueryPayload.construct(
+        payload = PageIndexQueryPayload.model_construct(
             deleted=deleted,
-            user_id=user_id,
+            limit=limit,
+            offset=offset,
+            search=search,
+            show_own=show_own,
             show_published=show_published,
             show_shared=show_shared,
             sort_by=sort_by,
             sort_desc=sort_desc,
-            limit=limit,
-            offset=offset,
-            search=search,
+            user_id=user_id,
         )
         pages, total_matches = self.service.index(trans, payload, include_total_count=True)
         response.headers["total_matches"] = str(total_matches)
         return pages
 
     @router.post(
         "/api/pages",
@@ -149,37 +150,51 @@
     @router.delete(
         "/api/pages/{id}",
         summary="Marks the specific Page as deleted.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     async def delete(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ):
         """Marks the Page with the given ID as deleted."""
         self.service.delete(trans, id)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
+    @router.put(
+        "/api/pages/{id}/undelete",
+        summary="Undelete the specific Page.",
+        status_code=status.HTTP_204_NO_CONTENT,
+    )
+    async def undelete(
+        self,
+        id: PageIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ):
+        """Marks the Page with the given ID as undeleted."""
+        self.service.undelete(trans, id)
+        return Response(status_code=status.HTTP_204_NO_CONTENT)
+
     @router.get(
         "/api/pages/{id}.pdf",
         summary="Return a PDF document of the last revision of the Page.",
         response_class=StreamingResponse,
         responses={
             200: {
                 "description": "PDF document with the last revision of the page.",
                 "content": {"application/pdf": {}},
             },
             501: {"description": "PDF conversion service not available."},
         },
     )
     async def show_pdf(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ):
         """Return a PDF document of the last revision of the Page.
 
         This feature may not be available in this Galaxy.
         """
         pdf_bytes = self.service.show_pdf(trans, id)
         return StreamingResponse(io.BytesIO(pdf_bytes), media_type="application/pdf")
@@ -192,116 +207,116 @@
                 "description": "Short term storage reference for async monitoring of this download.",
             },
             501: {"description": "PDF conversion service not available."},
         },
     )
     async def prepare_pdf(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> AsyncFile:
         """Return a STS download link for this page to be downloaded as a PDF.
 
         This feature may not be available in this Galaxy.
         """
         return self.service.prepare_pdf(trans, id)
 
     @router.get(
         "/api/pages/{id}",
         summary="Return a page summary and the content of the last revision.",
         response_description="The page summary information.",
     )
     async def show(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> PageDetails:
         """Return summary information about a specific Page and the content of the last revision."""
         return self.service.show(trans, id)
 
     @router.get(
         "/api/pages/{id}/sharing",
         summary="Get the current sharing status of the given Page.",
     )
     def sharing(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> SharingStatus:
         """Return the sharing status of the item."""
         return self.service.shareable_service.sharing(trans, id)
 
     @router.put(
         "/api/pages/{id}/enable_link_access",
         summary="Makes this item accessible by a URL link.",
     )
     def enable_link_access(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> SharingStatus:
         """Makes this item accessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.enable_link_access(trans, id)
 
     @router.put(
         "/api/pages/{id}/disable_link_access",
         summary="Makes this item inaccessible by a URL link.",
     )
     def disable_link_access(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> SharingStatus:
         """Makes this item inaccessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.disable_link_access(trans, id)
 
     @router.put(
         "/api/pages/{id}/publish",
         summary="Makes this item public and accessible by a URL link.",
     )
     def publish(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> SharingStatus:
         """Makes this item publicly available by a URL link and return the current sharing status."""
         return self.service.shareable_service.publish(trans, id)
 
     @router.put(
         "/api/pages/{id}/unpublish",
         summary="Removes this item from the published list.",
     )
     def unpublish(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
     ) -> SharingStatus:
         """Removes this item from the published list and return the current sharing status."""
         return self.service.shareable_service.unpublish(trans, id)
 
     @router.put(
         "/api/pages/{id}/share_with_users",
         summary="Share this item with specific users.",
     )
     def share_with_users(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
         payload: ShareWithPayload = Body(...),
     ) -> ShareWithStatus:
         """Shares this item with specific users and return the current sharing status."""
         return self.service.shareable_service.share_with_users(trans, id, payload)
 
     @router.put(
         "/api/pages/{id}/slug",
         summary="Set a new slug for this shared item.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def set_slug(
         self,
+        id: PageIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = PageIdPathParam,
         payload: SetSlugPayload = Body(...),
     ):
         """Sets a new slug to access this item by URL. The new slug must be unique."""
         self.service.shareable_service.set_slug(trans, id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/plugins.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/plugins.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Plugins resource control over the API.
 """
+
 import logging
 
 from galaxy import exceptions
 from galaxy.managers import (
     hdas,
     histories,
 )
@@ -31,30 +32,28 @@
 
     @expose_api_anonymous_and_sessionless
     def index(self, trans, **kwargs):
         """
         GET /api/plugins:
         """
         registry = self._get_registry()
-        dataset_id = kwargs.get("dataset_id")
-        if dataset_id is not None:
+        if (dataset_id := kwargs.get("dataset_id")) is not None:
             hda = self.hda_manager.get_accessible(self.decode_id(dataset_id), trans.user)
             return registry.get_visualizations(trans, hda)
         else:
             embeddable = asbool(kwargs.get("embeddable"))
             return registry.get_plugins(embeddable=embeddable)
 
     @expose_api
     def show(self, trans, id, **kwargs):
         """
         GET /api/plugins/{id}:
         """
         registry = self._get_registry()
-        history_id = kwargs.get("history_id")
-        if history_id is not None:
+        if (history_id := kwargs.get("history_id")) is not None:
             history = self.history_manager.get_owned(
                 trans.security.decode_id(history_id), trans.user, current_history=trans.history
             )
             result = {"hdas": []}
             for hda in history.contents_iter(types=["dataset"], deleted=False, visible=True):
                 if registry.get_visualization(trans, id, hda):
                     result["hdas"].append({"id": trans.security.encode_id(hda.id), "name": hda.name})
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/provenance.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/provenance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations provenance
 """
+
 import logging
 
 from paste.httpexceptions import (
     HTTPBadRequest,
     HTTPNotImplemented,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/quotas.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/quotas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 """
 API operations on Quota objects.
 """
+
 import logging
 
-from fastapi import Path
 from fastapi.param_functions import Body
 
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.quota._schema import (
     CreateQuotaParams,
     CreateQuotaResult,
     DeleteQuotaPayload,
     QuotaDetails,
     QuotaSummaryList,
     UpdateQuotaParams,
 )
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.webapps.galaxy.api import (
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import QuotaIdPathParam
 from galaxy.webapps.galaxy.services.quotas import QuotasService
 
 log = logging.getLogger(__name__)
 
 
 router = Router(tags=["quotas"])
 
 
-QuotaIdPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Quota ID", description="The encoded identifier of the Quota."  # Required
-)
-
-
 @router.cbv
 class FastAPIQuota:
     service: QuotasService = depends(QuotasService)
 
     @router.get(
         "/api/quotas",
         summary="Displays a list with information of quotas that are currently active.",
@@ -65,29 +60,31 @@
     @router.get(
         "/api/quotas/{id}",
         name="quota",
         summary="Displays details on a particular active quota.",
         require_admin=True,
     )
     def show(
-        self, trans: ProvidesUserContext = DependsOnTrans, id: DecodedDatabaseIdField = QuotaIdPathParam
+        self,
+        id: QuotaIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
     ) -> QuotaDetails:
         """Displays details on a particular active quota."""
         return self.service.show(trans, id)
 
     @router.get(
         "/api/quotas/deleted/{id}",
         name="deleted_quota",
         summary="Displays details on a particular quota that has been deleted.",
         require_admin=True,
     )
     def show_deleted(
         self,
+        id: QuotaIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = QuotaIdPathParam,
     ) -> QuotaDetails:
         """Displays details on a particular quota that has been deleted."""
         return self.service.show(trans, id, deleted=True)
 
     @router.post(
         "/api/quotas",
         summary="Creates a new quota.",
@@ -104,40 +101,48 @@
     @router.put(
         "/api/quotas/{id}",
         summary="Updates an existing quota.",
         require_admin=True,
     )
     def update(
         self,
+        id: QuotaIdPathParam,
         payload: UpdateQuotaParams,
-        id: DecodedDatabaseIdField = QuotaIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> str:
         """Updates an existing quota."""
         return self.service.update(trans, id, payload)
 
     @router.delete(
         "/api/quotas/{id}",
         summary="Deletes an existing quota.",
         require_admin=True,
     )
     def delete(
         self,
-        id: DecodedDatabaseIdField = QuotaIdPathParam,
+        id: QuotaIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
         payload: DeleteQuotaPayload = Body(None),  # Optional
     ) -> str:
         """Deletes an existing quota."""
         return self.service.delete(trans, id, payload)
 
     @router.post(
+        "/api/quotas/{id}/purge",
+        summary="Purges a previously deleted quota.",
+        require_admin=True,
+    )
+    def purge(self, id: QuotaIdPathParam, trans: ProvidesUserContext = DependsOnTrans) -> str:
+        return self.service.purge(trans, id)
+
+    @router.post(
         "/api/quotas/deleted/{id}/undelete",
         summary="Restores a previously deleted quota.",
         require_admin=True,
     )
     def undelete(
         self,
-        id: DecodedDatabaseIdField = QuotaIdPathParam,
+        id: QuotaIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
     ) -> str:
         """Restores a previously deleted quota."""
         return self.service.undelete(trans, id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/remote_files.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/remote_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on remote files.
 """
+
 import logging
 from typing import (
     List,
     Optional,
 )
 
 from fastapi import Body
@@ -49,15 +50,15 @@
     ),
 )
 
 RecursiveQueryParam: Optional[bool] = Query(
     default=None,
     title="Recursive",
     description=(
-        "Wether to recursively lists all sub-directories." " This will be `True` by default depending on the `target`."
+        "Whether to recursively lists all sub-directories." " This will be `True` by default depending on the `target`."
     ),
 )
 
 DisableModeQueryParam: Optional[RemoteFilesDisableMode] = Query(
     default=None,
     title="Disable mode",
     description=(
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/roles.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/roles.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 API operations on Role objects.
 """
+
 import logging
 
 from fastapi import Body
 
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.managers.roles import RoleManager
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import (
+    DecodedDatabaseIdField,
+    Security,
+)
 from galaxy.schema.schema import (
     RoleDefinitionModel,
     RoleListResponse,
     RoleModelResponse,
 )
 from galaxy.webapps.base.controller import url_for
 from galaxy.webapps.galaxy.api import (
@@ -26,32 +30,50 @@
 # Empty paths (e.g. /api/roles) only work if a prefix is defined right here.
 # https://github.com/tiangolo/fastapi/pull/415/files
 router = Router(tags=["roles"])
 
 
 def role_to_model(role):
     item = role.to_dict(view="element")
-    role_id = DecodedDatabaseIdField.encode(role.id)
+    role_id = Security.security.encode_id(role.id)
     item["url"] = url_for("role", id=role_id)
     return RoleModelResponse(**item)
 
 
 @router.cbv
 class FastAPIRoles:
     role_manager: RoleManager = depends(RoleManager)
 
     @router.get("/api/roles")
     def index(self, trans: ProvidesUserContext = DependsOnTrans) -> RoleListResponse:
         roles = self.role_manager.list_displayable_roles(trans)
-        return RoleListResponse(__root__=[role_to_model(r) for r in roles])
+        return RoleListResponse(root=[role_to_model(r) for r in roles])
 
     @router.get("/api/roles/{id}")
     def show(self, id: DecodedDatabaseIdField, trans: ProvidesUserContext = DependsOnTrans) -> RoleModelResponse:
         role = self.role_manager.get(trans, id)
         return role_to_model(role)
 
     @router.post("/api/roles", require_admin=True)
     def create(
         self, trans: ProvidesUserContext = DependsOnTrans, role_definition_model: RoleDefinitionModel = Body(...)
     ) -> RoleModelResponse:
         role = self.role_manager.create_role(trans, role_definition_model)
         return role_to_model(role)
+
+    @router.delete("/api/roles/{id}", require_admin=True)
+    def delete(self, id: DecodedDatabaseIdField, trans: ProvidesUserContext = DependsOnTrans) -> RoleModelResponse:
+        role = self.role_manager.get(trans, id)
+        role = self.role_manager.delete(trans, role)
+        return role_to_model(role)
+
+    @router.post("/api/roles/{id}/purge", require_admin=True)
+    def purge(self, id: DecodedDatabaseIdField, trans: ProvidesUserContext = DependsOnTrans) -> RoleModelResponse:
+        role = self.role_manager.get(trans, id)
+        role = self.role_manager.purge(trans, role)
+        return role_to_model(role)
+
+    @router.post("/api/roles/{id}/undelete", require_admin=True)
+    def undelete(self, id: DecodedDatabaseIdField, trans: ProvidesUserContext = DependsOnTrans) -> RoleModelResponse:
+        role = self.role_manager.get(trans, id)
+        role = self.role_manager.undelete(trans, role)
+        return role_to_model(role)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/sanitize_allow.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/sanitize_allow.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations allowing clients to retrieve and modify the HTML sanitization allow list.
 """
+
 import logging
 from typing import (
     Any,
     Dict,
 )
 
 from galaxy import web
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/short_term_storage.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/short_term_storage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
-API operations around galaxy.web.short_term_storage infrastructure.
+API operations around galaxy.short_term_storage infrastructure.
 """
+
 from uuid import UUID
 
-from galaxy.web.short_term_storage import (
+from galaxy.short_term_storage import (
     ShortTermStorageMonitor,
     ShortTermStorageServeCancelledInformation,
     ShortTermStorageServeCompletedInformation,
 )
 from galaxy.webapps.base.api import GalaxyFileResponse
 from . import (
     depends,
@@ -21,21 +22,23 @@
 class FastAPIShortTermStorage:
     short_term_storage_monitor: ShortTermStorageMonitor = depends(ShortTermStorageMonitor)  # type: ignore[type-abstract]  # https://github.com/python/mypy/issues/4717
 
     @router.get(
         "/api/short_term_storage/{storage_request_id}/ready",
         summary="Determine if specified storage request ID is ready for download.",
         response_description="Boolean indicating if the storage is ready.",
+        public=True,
     )
     def is_ready(self, storage_request_id: UUID) -> bool:
         storage_target = self.short_term_storage_monitor.recover_target(storage_request_id)
         return self.short_term_storage_monitor.is_ready(storage_target)
 
     @router.get(
         "/api/short_term_storage/{storage_request_id}",
+        public=True,
         summary="Serve the staged download specified by request ID.",
         response_description="Raw contents of the file.",
         response_class=GalaxyFileResponse,
         responses={
             200: {
                 "description": "The archive file containing the History.",
             },
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/storage_cleaner.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/storage_cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on User storage management.
 """
+
 import logging
 from typing import (
     List,
     Optional,
 )
 
 from fastapi import (
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tags.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API Controller providing Galaxy Tags
 """
+
 import logging
 
 from fastapi import (
     Body,
     Response,
     status,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tasks.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API Controller providing experimental access to Celery Task State.
 """
+
 import logging
 from uuid import UUID
 
 from galaxy.managers.tasks import (
     AsyncTasksManager,
     TaskState,
 )
@@ -20,12 +21,13 @@
 
 @router.cbv
 class FastAPITasks:
     manager: AsyncTasksManager = depends(AsyncTasksManager)  # type: ignore[type-abstract]
 
     @router.get(
         "/api/tasks/{task_id}/state",
+        public=True,
         summary="Determine state of task ID",
         response_description="String indicating task state.",
     )
     def state(self, task_id: UUID) -> TaskState:
         return self.manager.get_state(task_id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_data.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 from fastapi import (
     Body,
     Path,
 )
 from pydantic import (
     BaseModel,
     Field,
@@ -28,15 +30,15 @@
 
 router = Router(tags=["tool data tables"])
 
 ToolDataTableName = Path(
     ...,  # Mark this field as required
     title="Data table name",
     description="The name of the tool data table",
-    example="all_fasta",
+    examples=["all_fasta"],
 )
 
 ToolDataTableFieldName = Path(
     ...,  # Mark this field as required
     title="Field name",
     description="The name of the tool data table field",
 )
@@ -50,30 +52,30 @@
 class FastAPIToolData:
     tool_data_manager: ToolDataManager = depends(ToolDataManager)
 
     @router.get(
         "/api/tool_data",
         summary="Lists all available data tables",
         response_description="A list with details on individual data tables.",
-        require_admin=True,
+        public=True,
     )
     async def index(self) -> ToolDataEntryList:
         """Get the list of all available data tables."""
         return self.tool_data_manager.index()
 
     @router.post(
         "/api/tool_data",
         summary="Import a data manager bundle",
         require_admin=True,
     )
     async def create(
-        self, tool_data_file_path=None, import_bundle_model: ImportToolDataBundle = Body(...)
+        self, tool_data_file_path: Optional[str] = None, import_bundle_model: ImportToolDataBundle = Body(...)
     ) -> AsyncTaskResultSummary:
         source = import_bundle_model.source
-        result = import_data_bundle.delay(tool_data_file_path=tool_data_file_path, **source.dict())
+        result = import_data_bundle.delay(tool_data_file_path=tool_data_file_path, **source.model_dump())
         summary = async_task_summary(result)
         return summary
 
     @router.get(
         "/api/tool_data/{table_name}",
         summary="Get details of a given data table",
         response_description="A description of the given data table and its content",
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_dependencies.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations allowing clients to manage tool dependencies.
 """
+
 import logging
 from typing import Optional
 
 from galaxy.managers.context import ProvidesAppContext
 from galaxy.structured_app import StructuredApp
 from galaxy.tool_util.deps import views
 from galaxy.web import (
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_entry_points.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_entry_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ API for asynchronous job running mechanisms can use to fetch or put files
 related to running and queued jobs.
 """
+
 import logging
 
 from galaxy import (
     exceptions,
     util,
 )
 from galaxy.managers.context import ProvidesUserContext
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tool_shed_repositories.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tool_shed_repositories.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Path,
     Query,
 )
 from paste.httpexceptions import (
     HTTPBadRequest,
     HTTPForbidden,
 )
+from typing_extensions import Annotated
 
 from galaxy import (
     exceptions,
     util,
 )
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.schema.fields import DecodedDatabaseIdField
@@ -138,17 +139,15 @@
         tool_shed_url, name, owner, changeset_revision = self.__parse_repository_from_payload(
             payload, include_changeset=True
         )
         self.__ensure_can_install_repos(trans)
         irm = InstallRepositoryManager(self.app)
         installed_tool_shed_repositories = irm.install(tool_shed_url, name, owner, changeset_revision, payload)
         if installed_tool_shed_repositories:
-            return InstalledToolShedRepositories(
-                __root__=list(map(self.service._show, installed_tool_shed_repositories))
-            )
+            return InstalledToolShedRepositories(root=list(map(self.service._show, installed_tool_shed_repositories)))
         message = "No repositories were installed, possibly because the selected repository has already been installed."
         return dict(status="ok", message=message)
 
     @require_admin
     @expose_api
     def install_repository_revisions(self, trans, payload, **kwd):
         """
@@ -240,16 +239,16 @@
                 shed_tool_conf=shed_tool_conf,
             )
             installed_tool_shed_repositories = self.install_repository_revision(trans, **current_payload)
             if isinstance(installed_tool_shed_repositories, dict):
                 # We encountered an error.
                 return installed_tool_shed_repositories
             elif isinstance(installed_tool_shed_repositories, InstalledToolShedRepositories):
-                all_installed_tool_shed_repositories.extend(installed_tool_shed_repositories.__root__)
-        return InstalledToolShedRepositories(__root__=all_installed_tool_shed_repositories)
+                all_installed_tool_shed_repositories.extend(installed_tool_shed_repositories.root)
+        return InstalledToolShedRepositories(root=all_installed_tool_shed_repositories)
 
     @require_admin
     @expose_api
     def uninstall_repository(self, trans, id=None, **kwd):
         """
         DELETE /api/tool_shed_repositories/id
         DELETE /api/tool_shed_repositories/
@@ -314,16 +313,15 @@
             raise HTTPBadRequest(detail="Missing required parameter 'changeset_revision'.")
 
         return tool_shed_url, name, owner, changeset_revision
 
     @require_admin
     @expose_api
     def reset_metadata_on_selected_installed_repositories(self, trans, **kwd):
-        repository_ids = util.listify(kwd.get("repository_ids"))
-        if repository_ids:
+        if repository_ids := util.listify(kwd.get("repository_ids")):
             irmm = InstalledRepositoryMetadataManager(self.app)
             failed = []
             successful = []
             for repository_id in repository_ids:
                 try:
                     repository = get_installed_tool_shed_repository(self.app, repository_id)
                     irmm.set_repository(repository)
@@ -381,19 +379,22 @@
                 results["unsuccessful_count"] += 1
             results["repository_status"].append(message)
         stop_time = strftime("%Y-%m-%d %H:%M:%S")
         results["stop_time"] = stop_time
         return json.dumps(results, sort_keys=True, indent=4)
 
 
-InstalledToolShedRepositoryIDPathParam: DecodedDatabaseIdField = Path(
-    ...,
-    title="Installed Tool Shed Repository ID",
-    description="The encoded database identifier of the installed Tool Shed Repository.",
-)
+InstalledToolShedRepositoryIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(
+        ...,
+        title="Installed Tool Shed Repository ID",
+        description="The encoded database identifier of the installed Tool Shed Repository.",
+    ),
+]
 
 NameQueryParam: Optional[str] = Query(default=None, title="Name", description="Filter by repository name.")
 
 OwnerQueryParam: Optional[str] = Query(default=None, title="Owner", description="Filter by repository owner.")
 
 ChangesetQueryParam: Optional[str] = Query(default=None, title="Changeset", description="Filter by changeset revision.")
 
@@ -408,14 +409,15 @@
 
 @router.cbv
 class FastAPIToolShedRepositories:
     service: ToolShedRepositoriesService = depends(ToolShedRepositoriesService)
 
     @router.get(
         "/api/tool_shed_repositories",
+        public=True,
         summary="Lists installed tool shed repositories.",
         response_description="A list of installed tool shed repository objects.",
     )
     def index(
         self,
         name: Optional[str] = NameQueryParam,
         owner: Optional[str] = OwnerQueryParam,
@@ -439,14 +441,15 @@
         require_admin=True,
     )
     def check_for_updates(self, id: Optional[DecodedDatabaseIdField] = None) -> CheckForUpdatesResponse:
         return self.service.check_for_updates(id and int(id))
 
     @router.get(
         "/api/tool_shed_repositories/{id}",
+        public=True,
         summary="Show installed tool shed repository.",
     )
     def show(
         self,
-        id: DecodedDatabaseIdField = InstalledToolShedRepositoryIDPathParam,
+        id: InstalledToolShedRepositoryIDPathParam,
     ) -> InstalledToolShedRepository:
         return self.service.show(id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tools.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,17 +234,16 @@
     def build(self, trans: GalaxyWebTransaction, id, **kwd):
         """
         GET /api/tools/{tool_id}/build
         Returns a tool model including dynamic parameters and updated values, repeats block etc.
         """
         kwd = _kwd_or_payload(kwd)
         tool_version = kwd.get("tool_version")
-        history_id = kwd.pop("history_id", None)
         history = None
-        if history_id:
+        if history_id := kwd.pop("history_id", None):
             history = self.history_manager.get_owned(
                 self.decode_id(history_id), trans.user, current_history=trans.history
             )
         tool = self.service._get_tool(trans, id, tool_version=tool_version, user=trans.user)
         return tool.to_json(trans, kwd.get("inputs", kwd), history=history)
 
     @web.require_admin
@@ -271,16 +270,15 @@
         GET /api/tools/{tool_id}/test_data_download?tool_version={tool_version}&filename={filename}
         """
         tool_version = kwd.get("tool_version", None)
         tool = self.service._get_tool(trans, id, tool_version=tool_version, user=trans.user)
         filename = kwd.get("filename")
         if filename is None:
             raise exceptions.ObjectNotFound("Test data filename not specified.")
-        path = tool.test_data_path(filename)
-        if path:
+        if path := tool.test_data_path(filename):
             if os.path.isfile(path):
                 trans.response.headers["Content-Disposition"] = f'attachment; filename="{filename}"'
                 return open(path, mode="rb")
             elif os.path.isdir(path):
                 # Set upstream_mod_zip to false, otherwise tool data must be among allowed internal routes
                 archive = ZipstreamWrapper(
                     upstream_mod_zip=False,
@@ -459,17 +457,16 @@
             return x.to_dict()
 
         tool = self.service._get_tool(trans, id, user=trans.user)
         if hasattr(tool, "lineage"):
             lineage_dict = tool.lineage.to_dict()
         else:
             lineage_dict = None
-        tool_shed_dependencies = tool.installed_tool_dependencies
         tool_shed_dependencies_dict: Optional[list] = None
-        if tool_shed_dependencies:
+        if tool_shed_dependencies := tool.installed_tool_dependencies:
             tool_shed_dependencies_dict = list(map(to_dict, tool_shed_dependencies))
         return {
             "tool_id": tool.id,
             "tool_version": tool.version,
             "dependency_shell_commands": tool.build_dependency_shell_commands(),
             "lineage": lineage_dict,
             "requirements": list(map(to_dict, tool.requirements)),
@@ -512,16 +509,15 @@
                 {
                     "id": input_id,
                     "src": input_src,
                 }
             ],
             "batch": input_src == "hdca",
         }
-        history_id = payload.get("history_id")
-        if history_id:
+        if history_id := payload.get("history_id"):
             decoded_id = self.decode_id(history_id)
             target_history = self.history_manager.get_owned(decoded_id, trans.user, current_history=trans.history)
         else:
             if input_src == "hdca":
                 target_history = self.hdca_manager.get_dataset_collection_instance(
                     trans, instance_type="history", id=input_id
                 ).history
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/toolshed.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/toolshed.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/tours.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/tours.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API Controller providing Galaxy Tours
 """
+
 import logging
 
 from galaxy.tours import (
     TourDetails,
     TourList,
     ToursRegistry,
 )
@@ -19,20 +20,20 @@
 router = Router(tags=["tours"])
 
 
 @router.cbv
 class FastAPITours:
     registry: ToursRegistry = depends(ToursRegistry)  # type: ignore[type-abstract]  # https://github.com/python/mypy/issues/4717
 
-    @router.get("/api/tours")
+    @router.get("/api/tours", public=True)
     def index(self) -> TourList:
         """Return list of available tours."""
         return self.registry.get_tours()
 
-    @router.get("/api/tours/{tour_id}")
+    @router.get("/api/tours/{tour_id}", public=True)
     def show(self, tour_id: str) -> TourDetails:
         """Return a tour definition."""
         return self.registry.tour_contents(tour_id)
 
     @router.post("/api/tours/{tour_id}", require_admin=True)
     def update_tour(self, tour_id: str) -> TourDetails:
         """Return a tour definition."""
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/trs_consumer.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Proxy requests to GA4GH TRS servers (e.g. Dockstore).
 
 Information on TRS can be found at https://github.com/ga4gh/tool-registry-service-schemas.
 """
+
 from galaxy.web import expose_api
 from galaxy.workflow.trs_proxy import TrsProxy
 from . import (
     BaseGalaxyAPIController,
     depends,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/trs_search.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/trs_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Proxy requests to GA4GH TRS servers (e.g. Dockstore).
 
 Information on TRS can be found at https://github.com/ga4gh/tool-registry-service-schemas.
 """
+
 import logging
 
 from galaxy.web import expose_api
 from galaxy.workflow.trs_proxy import (
     parse_search_kwds,
     TrsProxy,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/uploads.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/uploads.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 API operations for uploaded files in storage.
 """
+
 import logging
 
-from galaxy.web.framework.decorators import expose_api_raw_anonymous
+from galaxy.web.framework.decorators import expose_api_anonymous
 from . import BaseGalaxyAPIController
 
 log = logging.getLogger(__name__)
 
 
 class UploadsAPIController(BaseGalaxyAPIController):
     READ_CHUNK_SIZE = 2**16
 
-    @expose_api_raw_anonymous
+    @expose_api_anonymous
     def hooks(self, trans, **kwds):
         """
         Exposed as POST /api/upload/hooks and /api/upload/resumable_upload
         """
         # Internal endpoint, only purpose is to authenticate user, but may grow additional functionality in the future
         return None
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/users.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API operations on User objects.
 """
+
 import copy
 import json
 import logging
 import re
 from typing import (
     Any,
     Dict,
@@ -17,15 +18,14 @@
     Body,
     Path,
     Query,
     Response,
     status,
 )
 from markupsafe import escape
-from pydantic import Required
 
 from galaxy import (
     exceptions,
     util,
 )
 from galaxy.exceptions import ObjectInvalid
 from galaxy.managers import users
@@ -38,15 +38,14 @@
     HistoryDatasetAssociation,
     Role,
     UserAddress,
     UserQuotaUsage,
 )
 from galaxy.model.base import transaction
 from galaxy.schema import APIKeyModel
-from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.schema import (
     AnonUserModel,
     AsyncTaskResultSummary,
     CreatedUserModel,
     CustomBuildCreationPayload,
     CustomBuildsCollection,
     DeletedCustomBuild,
@@ -82,48 +81,47 @@
 )
 from galaxy.webapps.galaxy.api import (
     BaseGalaxyAPIController,
     depends,
     DependsOnTrans,
     Router,
 )
+from galaxy.webapps.galaxy.api.common import UserIdPathParam
 from galaxy.webapps.galaxy.services.users import UsersService
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["users"])
 
-ThemePathParam: str = Path(default=Required, title="Theme", description="The theme of the GUI")
+ThemePathParam: str = Path(default=..., title="Theme", description="The theme of the GUI")
 UserDeletedQueryParam: bool = Query(default=None, title="Deleted user", description="Indicates if the user is deleted")
 UsersDeletedQueryParam: bool = Query(
     default=False, title="Deleted users", description="Indicates if the collection will be about deleted users"
 )
 FilterEmailQueryParam: str = Query(default=None, title="Email filter", description="An email address to filter on")
 FilterNameQueryParam: str = Query(default=None, title="Name filter", description="An username address to filter on")
 FilterAnyQueryParam: str = Query(default=None, title="Any filter", description="Filter on username OR email")
-UserIdPathParamQueryParam: DecodedDatabaseIdField = Path(..., title="User ID", description="The ID of the user to get.")
-APIKeyPathParamQueryParam: str = Path(..., title="API Key", description="The API key of the user.")
 FlexibleUserIdPathParam: FlexibleUserIdType = Path(
     ..., title="User ID", description="The ID of the user to get or 'current'."
 )
 QuotaSourceLabelPathParam: str = Path(
     ...,
     title="Quota Source Label",
     description="The label corresponding to the quota source to fetch usage information about.",
 )
 ObjectTypePathParam: FavoriteObjectType = Path(
-    default=Required, title="Object type", description="The object type the user wants to favorite"
+    default=..., title="Object type", description="The object type the user wants to favorite"
 )
 ObjectIDPathParam: str = Path(
-    default=Required,
+    default=...,
     title="Object ID",
     description="The ID of an object the user wants to remove from favorites",
 )
 CustomBuildKeyPathParam: str = Path(
-    default=Required,
+    default=...,
     title="Custom build key",
     description="The key of the custom build to be deleted.",
 )
 
 RecalculateDiskUsageSummary = "Triggers a recalculation of the current user disk usage."
 RecalculateDiskUsageResponseDescriptions = {
     200: {
@@ -132,23 +130,23 @@
     },
     204: {
         "description": "The background task was submitted but there is no status tracking ID available.",
     },
 }
 
 UserDeletionBody = Body(default=None, title="Purge user", description="Purge the user.")
-UserUpdateBody = Body(default=Required, title="Update user", description="The user values to update.")
+UserUpdateBody = Body(default=..., title="Update user", description="The user values to update.")
 FavoriteObjectBody = Body(
-    default=Required, title="Set favorite", description="The id of an object the user wants to favorite."
+    default=..., title="Set favorite", description="The id of an object the user wants to favorite."
 )
 
 CustomBuildCreationBody = Body(
-    default=Required, title="Add custom build", description="The values to add a new custom build."
+    default=..., title="Add custom build", description="The values to add a new custom build."
 )
-UserCreationBody = Body(default=Required, title="Create User", description="The values to add create a user.")
+UserCreationBody = Body(default=..., title="Create User", description="The values to add create a user.")
 AnyUserModel = Union[DetailedUserModel, AnonUserModel]
 
 
 @router.cbv
 class FastAPIUsers:
     service: UsersService = depends(UsersService)
     user_serializer: users.UserSerializer = depends(users.UserSerializer)
@@ -168,15 +166,33 @@
         self,
         trans: ProvidesUserContext = DependsOnTrans,
     ):
         """This route will be removed in a future version.
 
         Please use `/api/users/current/recalculate_disk_usage` instead.
         """
-        result = self.service.recalculate_disk_usage(trans)
+        user_id = getattr(trans.user, "id", None)
+        if not user_id:
+            raise exceptions.AuthenticationRequired("Only registered users can recalculate disk usage.")
+        else:
+            result = self.service.recalculate_disk_usage(trans, user_id)
+            return Response(status_code=status.HTTP_204_NO_CONTENT) if result is None else result
+
+    @router.put(
+        "/api/users/{user_id}/recalculate_disk_usage",
+        summary=RecalculateDiskUsageSummary,
+        responses=RecalculateDiskUsageResponseDescriptions,
+        require_admin=True,
+    )
+    def recalculate_disk_usage_by_user_id(
+        self,
+        user_id: UserIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ):
+        result = self.service.recalculate_disk_usage(trans, user_id)
         return Response(status_code=status.HTTP_204_NO_CONTENT) if result is None else result
 
     @router.get(
         "/api/users/deleted",
         name="get_deleted_users",
         description="Return a collection of deleted users. Only admins can see deleted users.",
     )
@@ -193,40 +209,42 @@
         "/api/users/deleted/{user_id}/undelete",
         name="undelete_user",
         summary="Restore a deleted user. Only admins can restore users.",
         require_admin=True,
     )
     def undelete(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ) -> DetailedUserModel:
         user = self.service.get_user(trans=trans, user_id=user_id)
         self.service.user_manager.undelete(user)
         return self.service.user_to_detailed_model(user)
 
     @router.get(
         "/api/users/deleted/{user_id}",
         name="get_deleted_user",
         summary="Return information about a deleted user. Only admins can see deleted users.",
     )
     def show_deleted(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ) -> AnyUserModel:
         return self.service.show_user(trans=trans, user_id=user_id, deleted=True)
 
     @router.get(
         "/api/users/{user_id}/api_key",
         name="get_or_create_api_key",
         summary="Return the user's API key",
     )
     def get_or_create_api_key(
-        self, trans: ProvidesUserContext = DependsOnTrans, user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam
+        self,
+        user_id: UserIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
     ) -> str:
         return self.service.get_or_create_api_key(trans, user_id)
 
     @router.get(
         "/api/users/{user_id}/api_key/detailed",
         name="get_api_key_detailed",
         summary="Return the user's API key with extra information.",
@@ -237,51 +255,54 @@
             },
             204: {
                 "description": "The user doesn't have an API key.",
             },
         },
     )
     def get_api_key(
-        self, trans: ProvidesUserContext = DependsOnTrans, user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam
+        self,
+        user_id: UserIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
     ):
         api_key = self.service.get_api_key(trans, user_id)
         return api_key if api_key else Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.post("/api/users/{user_id}/api_key", name="create_api_key", summary="Create a new API key for the user")
     def create_api_key(
-        self, trans: ProvidesUserContext = DependsOnTrans, user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam
+        self,
+        user_id: UserIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
     ) -> str:
         return self.service.create_api_key(trans, user_id).key
 
     @router.delete(
         "/api/users/{user_id}/api_key",
         name="delete_api_key",
         summary="Delete the current API key of the user",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def delete_api_key(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ):
         self.service.delete_api_key(trans, user_id)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.get(
         "/api/users/{user_id}/usage",
         name="get_user_usage",
         summary="Return the user's quota usage summary broken down by quota source",
     )
     def usage(
         self,
         trans: ProvidesUserContext = DependsOnTrans,
         user_id: FlexibleUserIdType = FlexibleUserIdPathParam,
     ) -> List[UserQuotaUsage]:
-        user = self.service.get_user_full(trans, user_id, False)
-        if user:
+        if user := self.service.get_user_full(trans, user_id, False):
             rval = self.user_serializer.serialize_disk_usage(user)
             return rval
         else:
             return []
 
     @router.get(
         "/api/users/{user_id}/usage/{label}",
@@ -290,33 +311,32 @@
     )
     def usage_for(
         self,
         trans: ProvidesUserContext = DependsOnTrans,
         user_id: FlexibleUserIdType = FlexibleUserIdPathParam,
         label: str = QuotaSourceLabelPathParam,
     ) -> Optional[UserQuotaUsage]:
-        user = self.service.get_user_full(trans, user_id, False)
         effective_label: Optional[str] = label
         if label == "__null__":
             effective_label = None
-        if user:
+        if user := self.service.get_user_full(trans, user_id, False):
             rval = self.user_serializer.serialize_disk_usage_for(user, effective_label)
             return rval
         else:
             return None
 
     @router.get(
         "/api/users/{user_id}/beacon",
         name="get_beacon_settings",
         summary="Return information about beacon share settings",
     )
     def get_beacon(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ) -> UserBeaconSetting:
         """
         **Warning**: This endpoint is experimental and might change or disappear in future versions.
         """
         user = self.service.get_user(trans, user_id)
 
         enabled = user.preferences["beacon_enabled"] if "beacon_enabled" in user.preferences else False
@@ -326,38 +346,38 @@
     @router.post(
         "/api/users/{user_id}/beacon",
         name="set_beacon_settings",
         summary="Change beacon setting",
     )
     def set_beacon(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         payload: UserBeaconSetting = Body(...),
     ) -> UserBeaconSetting:
         """
         **Warning**: This endpoint is experimental and might change or disappear in future versions.
         """
         user = self.service.get_user(trans, user_id)
 
         user.preferences["beacon_enabled"] = payload.enabled
         with transaction(trans.sa_session):
             trans.sa_session.commit()
 
         return payload
 
     @router.delete(
-        "/api/users/{user_id}/favorites/{object_type}/{object_id}",
+        "/api/users/{user_id}/favorites/{object_type}/{object_id:path}",
         name="remove_favorite",
         summary="Remove the object from user's favorites",
     )
     def remove_favorite(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         object_type: FavoriteObjectType = ObjectTypePathParam,
         object_id: str = ObjectIDPathParam,
     ) -> FavoriteObjectsSummary:
         user = self.service.get_user(trans, user_id)
         favorites = json.loads(user.preferences["favorites"]) if "favorites" in user.preferences else {}
         if object_type.value == "tools":
             if "tools" in favorites:
@@ -375,16 +395,16 @@
     @router.put(
         "/api/users/{user_id}/favorites/{object_type}",
         name="set_favorite",
         summary="Add the object to user's favorites",
     )
     def set_favorite(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         object_type: FavoriteObjectType = ObjectTypePathParam,
         payload: FavoriteObject = FavoriteObjectBody,
     ) -> FavoriteObjectsSummary:
         user = self.service.get_user(trans, user_id)
         favorites = json.loads(user.preferences["favorites"]) if "favorites" in user.preferences else {}
         if object_type.value == "tools":
             tool_id = payload.object_id
@@ -408,16 +428,16 @@
     @router.put(
         "/api/users/{user_id}/theme/{theme}",
         name="set_theme",
         summary="Set the user's theme choice",
     )
     def set_theme(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         theme: str = ThemePathParam,
     ) -> str:
         user = self.service.get_user(trans, user_id)
         user.preferences["theme"] = theme
         with transaction(trans.sa_session):
             trans.sa_session.commit()
         return theme
@@ -425,17 +445,17 @@
     @router.put(
         "/api/users/{user_id}/custom_builds/{key}",
         name="add_custom_builds",
         summary="Add new custom build.",
     )
     def add_custom_builds(
         self,
+        user_id: UserIdPathParam,
         key: str = CustomBuildKeyPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         payload: CustomBuildCreationPayload = CustomBuildCreationBody,
     ) -> Any:
         user = self.service.get_user(trans, user_id)
         dbkeys = json.loads(user.preferences["dbkeys"]) if "dbkeys" in user.preferences else {}
         name = payload.name
         len_type = payload.len_type
         len_value = payload.len_value
@@ -509,16 +529,16 @@
             return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.get(
         "/api/users/{user_id}/custom_builds", name="get_custom_builds", summary=" Returns collection of custom builds."
     )
     def get_custom_builds(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesHistoryContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ) -> CustomBuildsCollection:
         user = self.service.get_user(trans, user_id)
         dbkeys = json.loads(user.preferences["dbkeys"]) if "dbkeys" in user.preferences else {}
         valid_dbkeys = {}
         update = False
         for key, dbkey in dbkeys.items():
             if "count" not in dbkey and "linecount" in dbkey:
@@ -536,24 +556,24 @@
                 valid_dbkeys[key] = dbkey
         if update:
             user.preferences["dbkeys"] = json.dumps(valid_dbkeys)
         dbkey_collection = []
         for key, attributes in valid_dbkeys.items():
             attributes["id"] = key
             dbkey_collection.append(attributes)
-        return CustomBuildsCollection.construct(__root__=dbkey_collection)
+        return CustomBuildsCollection.model_construct(root=dbkey_collection)
 
     @router.delete(
         "/api/users/{user_id}/custom_builds/{key}", name="delete_custom_build", summary="Delete a custom build"
     )
     def delete_custom_builds(
         self,
+        user_id: UserIdPathParam,
         key: str = CustomBuildKeyPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
     ) -> DeletedCustomBuild:
         user = self.service.get_user(trans, user_id)
         dbkeys = json.loads(user.preferences["dbkeys"]) if "dbkeys" in user.preferences else {}
         if key and key in dbkeys:
             del dbkeys[key]
             user.preferences["dbkeys"] = json.dumps(dbkeys)
             with transaction(trans.sa_session):
@@ -594,15 +614,15 @@
             ).rstrip()
             if message:
                 raise exceptions.RequestParameterInvalidException(message)
             else:
                 user = self.service.user_manager.create(email=email, username=username, password=password)
         else:
             raise exceptions.NotImplemented()
-        item = user.to_dict(view="element", value_mapper={"id": trans.security.encode_id, "total_disk_usage": float})
+        item = user.to_dict(view="element", value_mapper={"total_disk_usage": float})
         return item
 
     @router.get(
         "/api/users",
         name="get_users",
         description="Return a collection of users. Filters will only work if enabled in config or user is admin.",
         response_model_exclude_unset=True,
@@ -650,16 +670,16 @@
     @router.delete(
         "/api/users/{user_id}",
         name="delete_user",
         summary="Delete a user. Only admins can delete others or purge users.",
     )
     def delete(
         self,
+        user_id: UserIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        user_id: DecodedDatabaseIdField = UserIdPathParamQueryParam,
         payload: Optional[UserDeletionPayload] = UserDeletionBody,
     ) -> DetailedUserModel:
         user_to_update = self.service.user_manager.by_id(user_id)
         if payload:
             purge = payload.purge
         else:
             purge = False
@@ -672,14 +692,31 @@
         else:
             if trans.user == user_to_update:
                 self.service.user_manager.delete(user_to_update)
             else:
                 raise exceptions.InsufficientPermissionsException("You may only delete your own account.")
         return self.service.user_to_detailed_model(user_to_update)
 
+    @router.post(
+        "/api/users/{user_id}/send_activation_email",
+        name="send_activation_email",
+        summary="Sends activation email to user.",
+        require_admin=True,
+    )
+    def send_activation_email(
+        self,
+        user_id: UserIdPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ):
+        user = trans.sa_session.query(trans.model.User).get(user_id)
+        if not user:
+            raise exceptions.ObjectNotFound("User not found for given id.")
+        if not self.service.user_manager.send_activation_email(trans, user.email, user.username):
+            raise exceptions.MessageException("Unable to send activation email.")
+
 
 class UserAPIController(BaseGalaxyAPIController, UsesTagsMixin, BaseUIController, UsesFormDefinitionsMixin):
     service: UsersService = depends(UsersService)
     user_manager: users.UserManager = depends(users.UserManager)
 
     def _get_user_full(self, trans, user_id, **kwd):
         """Return referenced user or None if anonymous user is referenced."""
@@ -903,16 +940,15 @@
             username = payload.get("username")
             message = validate_publicname(trans, username, user)
             if message:
                 raise exceptions.RequestParameterInvalidException(message)
             if user.username != username:
                 user.username = username
         # Update user custom form
-        user_info_form_id = payload.get("info|form_id")
-        if user_info_form_id:
+        if user_info_form_id := payload.get("info|form_id"):
             prefix = "info|"
             user_info_form = trans.sa_session.get(FormDefinition, trans.security.decode_id(user_info_form_id))
             user_info_values = {}
             for item in payload:
                 if item.startswith(prefix):
                     user_info_values[item[len(prefix) :]] = payload[item]
             form_values = trans.model.FormValues(user_info_form, user_info_values)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/visualizations.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/visualizations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Visualizations resource control over the API.
 
 NOTE!: this is a work in progress and functionality and data structures
 may change often.
 """
+
 import json
 import logging
 from typing import Optional
 
 from fastapi import (
     Body,
     Path,
     Query,
     Response,
     status,
 )
+from typing_extensions import Annotated
 
 from galaxy import (
     exceptions,
     util,
     web,
 )
 from galaxy.managers.context import ProvidesUserContext
@@ -100,17 +102,18 @@
 
 SortDescQueryParam: bool = Query(
     default=True,
     title="Sort Descending",
     description="Sort in descending order?",
 )
 
-VisualizationIdPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Visualization ID", description="The encoded database identifier of the Visualization."
-)
+VisualizationIdPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Visualization ID", description="The encoded database identifier of the Visualization."),
+]
 
 
 @router.cbv
 class FastAPIVisualizations:
     service: VisualizationsService = depends(VisualizationsService)
 
     @router.get(
@@ -128,15 +131,15 @@
         show_own: bool = ShowOwnQueryParam,
         show_published: bool = ShowPublishedQueryParam,
         show_shared: bool = ShowSharedQueryParam,
         sort_by: VisualizationSortByEnum = SortByQueryParam,
         sort_desc: bool = SortDescQueryParam,
         search: Optional[str] = SearchQueryParam,
     ) -> VisualizationSummaryList:
-        payload = VisualizationIndexQueryPayload.construct(
+        payload = VisualizationIndexQueryPayload.model_construct(
             deleted=deleted,
             user_id=user_id,
             show_published=show_published,
             show_own=show_own,
             show_shared=show_shared,
             sort_by=sort_by,
             sort_desc=sort_desc,
@@ -150,90 +153,90 @@
 
     @router.get(
         "/api/visualizations/{id}/sharing",
         summary="Get the current sharing status of the given Visualization.",
     )
     def sharing(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
     ) -> SharingStatus:
         """Return the sharing status of the item."""
         return self.service.shareable_service.sharing(trans, id)
 
     @router.put(
         "/api/visualizations/{id}/enable_link_access",
         summary="Makes this item accessible by a URL link.",
     )
     def enable_link_access(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
     ) -> SharingStatus:
         """Makes this item accessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.enable_link_access(trans, id)
 
     @router.put(
         "/api/visualizations/{id}/disable_link_access",
         summary="Makes this item inaccessible by a URL link.",
     )
     def disable_link_access(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
     ) -> SharingStatus:
         """Makes this item inaccessible by a URL link and return the current sharing status."""
         return self.service.shareable_service.disable_link_access(trans, id)
 
     @router.put(
         "/api/visualizations/{id}/publish",
         summary="Makes this item public and accessible by a URL link.",
     )
     def publish(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
     ) -> SharingStatus:
         """Makes this item publicly available by a URL link and return the current sharing status."""
         return self.service.shareable_service.publish(trans, id)
 
     @router.put(
         "/api/visualizations/{id}/unpublish",
         summary="Removes this item from the published list.",
     )
     def unpublish(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
     ) -> SharingStatus:
         """Removes this item from the published list and return the current sharing status."""
         return self.service.shareable_service.unpublish(trans, id)
 
     @router.put(
         "/api/visualizations/{id}/share_with_users",
         summary="Share this item with specific users.",
     )
     def share_with_users(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
         payload: ShareWithPayload = Body(...),
     ) -> ShareWithStatus:
         """Shares this item with specific users and return the current sharing status."""
         return self.service.shareable_service.share_with_users(trans, id, payload)
 
     @router.put(
         "/api/visualizations/{id}/slug",
         summary="Set a new slug for this shared item.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def set_slug(
         self,
+        id: VisualizationIdPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = VisualizationIdPathParam,
         payload: SetSlugPayload = Body(...),
     ):
         """Sets a new slug to access this item by URL. The new slug must be unique."""
         self.service.shareable_service.set_slug(trans, id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
 
@@ -359,15 +362,15 @@
         #   - protection against malicious data content
         # all other conversions and processing (such as permissions, etc.) should happen down the line
 
         # keys listed here don't error when attempting to set, but fail silently
         #   this allows PUT'ing an entire model back to the server without attribute errors on uneditable attrs
         valid_but_uneditable_keys = (
             "id",
-            "model_class"
+            "model_class",
             # TODO: fill out when we create to_dict, get_dict, whatevs
         )
         # TODO: importable
         ValidationError = exceptions.RequestParameterInvalidException
 
         validated_payload = {}
         for key, val in payload.items():
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/webhooks.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 API Controller providing Galaxy Webhooks
 """
+
 import importlib.util
 import logging
 from typing import Any
 
 from galaxy.web import expose_api_anonymous_and_sessionless
 from galaxy.webapps.base.webapp import GalaxyWebTransaction
 from . import BaseGalaxyAPIController
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/api/workflows.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/api/workflows.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,75 +7,94 @@
 import os
 from io import BytesIO
 from typing import (
     Any,
     Dict,
     List,
     Optional,
+    Union,
 )
 
 from fastapi import (
     Body,
     Path,
     Query,
     Response,
     status,
 )
 from gxformat2._yaml import ordered_dump
 from markupsafe import escape
-from pydantic import Extra
+from pydantic import (
+    UUID1,
+    UUID4,
+)
 from starlette.responses import StreamingResponse
+from typing_extensions import Annotated
 
 from galaxy import (
     exceptions,
     model,
     util,
 )
 from galaxy.files.uris import (
     stream_url_to_str,
     validate_uri_access,
 )
-from galaxy.managers.context import ProvidesUserContext
-from galaxy.managers.jobs import (
-    fetch_job_states,
-    invocation_job_source_iter,
+from galaxy.managers.context import (
+    ProvidesHistoryContext,
+    ProvidesUserContext,
 )
 from galaxy.managers.workflows import (
     MissingToolsException,
     RefactorRequest,
+    RefactorResponse,
     WorkflowCreateOptions,
     WorkflowUpdateOptions,
 )
 from galaxy.model.base import transaction
 from galaxy.model.item_attrs import UsesAnnotations
 from galaxy.model.store import BcoExportOptions
 from galaxy.schema.fields import DecodedDatabaseIdField
-from galaxy.schema.invocation import InvocationMessageResponseModel
+from galaxy.schema.invocation import (
+    CreateInvocationFromStore,
+    CreateInvocationsFromStorePayload,
+    InvocationJobsResponse,
+    InvocationReport,
+    InvocationSerializationParams,
+    InvocationStep,
+    InvocationStepJobsResponseCollectionJobsModel,
+    InvocationStepJobsResponseJobModel,
+    InvocationStepJobsResponseStepModel,
+    InvocationUpdatePayload,
+    WorkflowInvocationResponse,
+)
 from galaxy.schema.schema import (
     AsyncFile,
     AsyncTaskResultSummary,
+    InvocationSortByEnum,
+    InvocationsStateCounts,
     SetSlugPayload,
     ShareWithPayload,
     ShareWithStatus,
     SharingStatus,
-    StoreContentSource,
     WorkflowSortByEnum,
 )
+from galaxy.schema.workflows import (
+    InvokeWorkflowPayload,
+    StoredWorkflowDetailed,
+)
 from galaxy.structured_app import StructuredApp
 from galaxy.tool_shed.galaxy_install.install_manager import InstallRepositoryManager
 from galaxy.tools import recommendations
 from galaxy.tools.parameters import populate_state
-from galaxy.tools.parameters.basic import workflow_building_modes
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
 from galaxy.util.sanitize_html import sanitize_html
 from galaxy.version import VERSION
 from galaxy.web import (
     expose_api,
-    expose_api_anonymous,
-    expose_api_anonymous_and_sessionless,
-    expose_api_raw,
     expose_api_raw_anonymous_and_sessionless,
     format_return_as_json,
 )
 from galaxy.webapps.base.controller import (
     SharableMixin,
     url_for,
     UsesStoredWorkflowMixin,
@@ -85,56 +104,46 @@
     BaseGalaxyAPIController,
     depends,
     DependsOnTrans,
     IndexQueryTag,
     Router,
     search_query_param,
 )
+from galaxy.webapps.galaxy.api.common import SerializationViewQueryParam
 from galaxy.webapps.galaxy.services.base import (
     ConsumesModelStores,
     ServesExportStores,
 )
 from galaxy.webapps.galaxy.services.invocations import (
     InvocationIndexPayload,
-    InvocationSerializationParams,
     InvocationsService,
     PrepareStoreDownloadPayload,
     WriteInvocationStoreToPayload,
 )
 from galaxy.webapps.galaxy.services.workflows import (
     WorkflowIndexPayload,
     WorkflowsService,
 )
 from galaxy.workflow.extract import extract_workflow
 from galaxy.workflow.modules import module_factory
-from galaxy.workflow.run import queue_invoke
-from galaxy.workflow.run_request import build_workflow_run_configs
 
 log = logging.getLogger(__name__)
 
 router = Router(tags=["workflows"])
 
 
-class CreateInvocationFromStore(StoreContentSource):
-    history_id: Optional[str]
-
-    class Config:
-        extra = Extra.allow
-
-
 class WorkflowsAPIController(
     BaseGalaxyAPIController,
     UsesStoredWorkflowMixin,
     UsesAnnotations,
     SharableMixin,
     ServesExportStores,
     ConsumesModelStores,
 ):
     service: WorkflowsService = depends(WorkflowsService)
-    invocations_service: InvocationsService = depends(InvocationsService)
 
     def __init__(self, app: StructuredApp):
         super().__init__(app)
         self.history_manager = app.history_manager
         self.workflow_manager = app.workflow_manager
         self.workflow_contents_manager = app.workflow_contents_manager
         self.tool_recommendations = recommendations.ToolRecommendations()
@@ -175,46 +184,14 @@
             user.stored_workflow_menu_entries.append(m)
         with transaction(session):
             session.commit()
         message = "Menu updated."
         trans.set_message(message)
         return {"message": message, "status": "done"}
 
-    @expose_api_anonymous_and_sessionless
-    def show(self, trans: GalaxyWebTransaction, id, **kwd):
-        """
-        GET /api/workflows/{encoded_workflow_id}
-
-        :param  instance:                 true if fetch by Workflow ID instead of StoredWorkflow id, false
-                                          by default.
-        :type   instance:                 boolean
-
-        Displays information needed to run a workflow.
-        """
-        stored_workflow = self.__get_stored_workflow(trans, id, **kwd)
-        if stored_workflow.importable is False and stored_workflow.user != trans.user and not trans.user_is_admin:
-            wf_count = 0 if not trans.user else trans.user.count_stored_workflow_user_assocs(stored_workflow)
-            if wf_count == 0:
-                message = "Workflow is neither importable, nor owned by or shared with current user"
-                raise exceptions.ItemAccessibilityException(message)
-        if kwd.get("legacy", False):
-            style = "legacy"
-        else:
-            style = "instance"
-        version = kwd.get("version")
-        if version is None and util.string_as_bool(kwd.get("instance", "false")):
-            # A Workflow instance may not be the latest workflow version attached to StoredWorkflow.
-            # This figures out the correct version so that we return the correct Workflow and version.
-            workflow_id = self.decode_id(id)
-            for i, workflow in enumerate(reversed(stored_workflow.workflows)):
-                if workflow.id == workflow_id:
-                    version = i
-                    break
-        return self.workflow_contents_manager.workflow_to_dict(trans, stored_workflow, style=style, version=version)
-
     @expose_api
     def create(self, trans: GalaxyWebTransaction, payload=None, **kwd):
         """
         POST /api/workflows
 
         Create workflows in various ways.
 
@@ -368,33 +345,32 @@
         :type   instance:                 boolean
         """
         stored_workflow = self.__get_stored_accessible_workflow(trans, workflow_id, **kwd)
 
         style = kwd.get("style", "export")
         download_format = kwd.get("format")
         version = kwd.get("version")
-        history_id = kwd.get("history_id")
         history = None
-        if history_id:
+        if history_id := kwd.get("history_id"):
             history = self.history_manager.get_accessible(
                 self.decode_id(history_id), trans.user, current_history=trans.history
             )
         ret_dict = self.workflow_contents_manager.workflow_to_dict(
             trans, stored_workflow, style=style, version=version, history=history
         )
         if download_format == "json-download":
             sname = stored_workflow.name
             sname = "".join(c in util.FILENAME_VALID_CHARS and c or "_" for c in sname)[0:150]
             if ret_dict.get("format-version", None) == "0.1":
                 extension = "ga"
             else:
                 extension = "gxwf.json"
-            trans.response.headers[
-                "Content-Disposition"
-            ] = f'attachment; filename="Galaxy-Workflow-{sname}.{extension}"'
+            trans.response.headers["Content-Disposition"] = (
+                f'attachment; filename="Galaxy-Workflow-{sname}.{extension}"'
+            )
             trans.response.set_content_type("application/galaxy-archive")
 
         if style == "format2" and download_format != "json-download":
             return ordered_dump(ret_dict)
         else:
             return format_return_as_json(ret_dict, pretty=True)
 
@@ -548,34 +524,14 @@
 
         else:
             message = "Updating workflow requires dictionary containing 'workflow' attribute with new JSON description."
             raise exceptions.RequestParameterInvalidException(message)
         return self.workflow_contents_manager.workflow_to_dict(trans, stored_workflow, style="instance")
 
     @expose_api
-    def refactor(self, trans, id, payload, **kwds):
-        """
-        * PUT /api/workflows/{id}/refactor
-            updates the workflow stored with ``id``
-
-        :type   id:      str
-        :param  id:      the encoded id of the workflow to update
-        :param  instance:                 true if fetch by Workflow ID instead of StoredWorkflow id, false
-                                          by default.
-        :type   instance:                 boolean
-        :type   payload: dict
-        :param  payload: a dictionary containing list of actions to apply.
-        :rtype:     dict
-        :returns:   serialized version of the workflow
-        """
-        stored_workflow = self.__get_stored_workflow(trans, id, **kwds)
-        refactor_request = RefactorRequest(**payload)
-        return self.workflow_contents_manager.refactor(trans, stored_workflow, refactor_request)
-
-    @expose_api
     def build_module(self, trans: GalaxyWebTransaction, payload=None):
         """
         POST /api/workflows/build_module
         Builds module models for the workflow editor.
         """
         # payload is tool state
         if payload is None:
@@ -599,20 +555,17 @@
             step_dict["tool_version"] = module.get_version()
         return step_dict
 
     @expose_api
     def get_tool_predictions(self, trans: ProvidesUserContext, payload, **kwd):
         """
         POST /api/workflows/get_tool_predictions
-
         Fetch predicted tools for a workflow
-
         :type   payload: dict
         :param  payload:
-
             a dictionary containing two parameters
             'tool_sequence' - comma separated sequence of tool ids
             'remote_model_url' - (optional) path to the deep learning model
         """
         remote_model_url = payload.get("remote_model_url", trans.app.config.tool_recommendation_model_path)
         tool_sequence = payload.get("tool_sequence", "")
         if "tool_sequence" not in payload or remote_model_url is None:
@@ -713,333 +666,14 @@
             raise exceptions.ItemDeletionException("You can't import this workflow because it has been deleted.")
         imported_workflow = self._import_shared_workflow(trans, stored_workflow)
         item = imported_workflow.to_dict(value_mapper={"id": trans.security.encode_id})
         encoded_id = trans.security.encode_id(imported_workflow.id)
         item["url"] = url_for("workflow", id=encoded_id)
         return item
 
-    @expose_api
-    def invoke(self, trans: GalaxyWebTransaction, workflow_id, payload, **kwd):
-        """
-        POST /api/workflows/{encoded_workflow_id}/invocations
-
-        Schedule the workflow specified by `workflow_id` to run.
-
-        .. note:: This method takes the same arguments as
-            :func:`galaxy.webapps.galaxy.api.workflows.WorkflowsAPIController.create` above.
-
-        :raises: exceptions.MessageException, exceptions.RequestParameterInvalidException
-        """
-        # Get workflow + accessibility check.
-        stored_workflow = self.__get_stored_accessible_workflow(trans, workflow_id, instance=kwd.get("instance", False))
-        workflow = stored_workflow.latest_workflow
-        run_configs = build_workflow_run_configs(trans, workflow, payload)
-        is_batch = payload.get("batch")
-        if not is_batch and len(run_configs) != 1:
-            raise exceptions.RequestParameterInvalidException("Must specify 'batch' to use batch parameters.")
-
-        require_exact_tool_versions = util.string_as_bool(payload.get("require_exact_tool_versions", "true"))
-        tools = self.workflow_contents_manager.get_all_tools(workflow)
-        missing_tools = [
-            tool
-            for tool in tools
-            if not self.app.toolbox.has_tool(
-                tool["tool_id"], tool_version=tool["tool_version"], exact=require_exact_tool_versions
-            )
-        ]
-        if missing_tools:
-            missing_tools_message = "Workflow was not invoked; the following required tools are not installed: "
-            if require_exact_tool_versions:
-                missing_tools_message += ", ".join(
-                    [f"{tool['tool_id']} (version {tool['tool_version']})" for tool in missing_tools]
-                )
-            else:
-                missing_tools_message += ", ".join([tool["tool_id"] for tool in missing_tools])
-            raise exceptions.MessageException(missing_tools_message)
-
-        invocations = []
-        for run_config in run_configs:
-            workflow_scheduler_id = payload.get("scheduler", None)
-            # TODO: workflow scheduler hints
-            work_request_params = dict(scheduler=workflow_scheduler_id)
-            workflow_invocation = queue_invoke(
-                trans=trans,
-                workflow=workflow,
-                workflow_run_config=run_config,
-                request_params=work_request_params,
-                flush=False,
-            )
-            invocations.append(workflow_invocation)
-
-        with transaction(trans.sa_session):
-            trans.sa_session.commit()
-        encoded_invocations = []
-        for invocation in invocations:
-            as_dict = workflow_invocation.to_dict()
-            as_dict = self.encode_all_ids(trans, as_dict, recursive=True)
-            as_dict["messages"] = [
-                InvocationMessageResponseModel.parse_obj(message).__root__.dict() for message in invocation.messages
-            ]
-            encoded_invocations.append(as_dict)
-
-        if is_batch:
-            return encoded_invocations
-        else:
-            return encoded_invocations[0]
-
-    @expose_api
-    def index_invocations(self, trans: GalaxyWebTransaction, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations
-        GET /api/invocations
-
-        Get the list of a user's workflow invocations. If workflow_id is supplied
-        (either via URL or query parameter) it should be an encoded StoredWorkflow id
-        and returned invocations will be restricted to that workflow. history_id (an encoded
-        History id) can be used to further restrict the query. If neither a workflow_id or
-        history_id is supplied, all the current user's workflow invocations will be indexed
-        (as determined by the invocation being executed on one of the user's histories).
-
-        :param  workflow_id:      an encoded stored workflow id to restrict query to
-        :type   workflow_id:      str
-
-        :param  instance:         true if fetch by Workflow ID instead of StoredWorkflow id, false
-                                  by default.
-        :type   instance:         boolean
-
-        :param  history_id:       an encoded history id to restrict query to
-        :type   history_id:       str
-
-        :param  job_id:           an encoded job id to restrict query to
-        :type   job_id:           str
-
-        :param  user_id:          an encoded user id to restrict query to, must be own id if not admin user
-        :type   user_id:          str
-
-        :param  view:             level of detail to return per invocation 'element' or 'collection'.
-        :type   view:             str
-
-        :param  step_details:     If 'view' is 'element', also include details on individual steps.
-        :type   step_details:     bool
-
-        :raises: exceptions.MessageException, exceptions.ObjectNotFound
-        """
-        invocation_payload = InvocationIndexPayload(**kwd)
-        serialization_params = InvocationSerializationParams(**kwd)
-        invocations, total_matches = self.invocations_service.index(trans, invocation_payload, serialization_params)
-        trans.response.headers["total_matches"] = total_matches
-        return invocations
-
-    @expose_api_anonymous
-    def create_invocations_from_store(self, trans, payload, **kwd):
-        """
-        POST /api/invocations/from_store
-
-        Create invocation(s) from a supplied model store.
-
-        Input can be an archive describing a Galaxy model store containing an
-        workflow invocation - for instance one created with with write_store
-        or prepare_store_download endpoint.
-        """
-        create_payload = CreateInvocationFromStore(**payload)
-        serialization_params = InvocationSerializationParams(**payload)
-        # refactor into a service...
-        return self._create_from_store(trans, create_payload, serialization_params)
-
-    def _create_from_store(
-        self, trans, payload: CreateInvocationFromStore, serialization_params: InvocationSerializationParams
-    ):
-        history = self.history_manager.get_owned(
-            self.decode_id(payload.history_id), trans.user, current_history=trans.history
-        )
-        object_tracker = self.create_objects_from_store(
-            trans,
-            payload,
-            history=history,
-        )
-        return self.invocations_service.serialize_workflow_invocations(
-            object_tracker.invocations_by_key.values(), serialization_params
-        )
-
-    @expose_api
-    def show_invocation(self, trans: GalaxyWebTransaction, invocation_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}
-        GET /api/invocations/{invocation_id}
-
-        Get detailed description of workflow invocation
-
-        :param  invocation_id:      the invocation id (required)
-        :type   invocation_id:      str
-
-        :param  step_details:       fetch details about individual invocation steps
-                                    and populate a steps attribute in the resulting
-                                    dictionary. Defaults to false.
-        :type   step_details:       bool
-
-        :param  legacy_job_state:   If step_details is true, and this is set to true
-                                    populate the invocation step state with the job state
-                                    instead of the invocation step state. This will also
-                                    produce one step per job in mapping jobs to mimic the
-                                    older behavior with respect to collections. Partially
-                                    scheduled steps may provide incomplete information
-                                    and the listed steps outputs are the mapped over
-                                    step outputs but the individual job outputs
-                                    when this is set - at least for now.
-        :type   legacy_job_state:   bool
-
-        :raises: exceptions.MessageException, exceptions.ObjectNotFound
-        """
-        decoded_workflow_invocation_id = self.decode_id(invocation_id)
-        workflow_invocation = self.workflow_manager.get_invocation(trans, decoded_workflow_invocation_id, eager=True)
-        if not workflow_invocation:
-            raise exceptions.ObjectNotFound()
-
-        return self.__encode_invocation(workflow_invocation, **kwd)
-
-    @expose_api
-    def cancel_invocation(self, trans: ProvidesUserContext, invocation_id, **kwd):
-        """
-        DELETE /api/workflows/{workflow_id}/invocations/{invocation_id}
-        DELETE /api/invocations/{invocation_id}
-        Cancel the specified workflow invocation.
-
-        :param  invocation_id:      the usage id (required)
-        :type   invocation_id:      str
-
-        :raises: exceptions.MessageException, exceptions.ObjectNotFound
-        """
-        decoded_workflow_invocation_id = self.decode_id(invocation_id)
-        workflow_invocation = self.workflow_manager.request_invocation_cancellation(
-            trans, decoded_workflow_invocation_id
-        )
-        return self.__encode_invocation(workflow_invocation, **kwd)
-
-    @expose_api
-    def show_invocation_report(self, trans: GalaxyWebTransaction, invocation_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}/report
-        GET /api/invocations/{invocation_id}/report
-
-        Get JSON summarizing invocation for reporting.
-        """
-        kwd["format"] = "json"
-        return self.workflow_manager.get_invocation_report(trans, invocation_id, **kwd)
-
-    @expose_api_raw
-    def show_invocation_report_pdf(self, trans: GalaxyWebTransaction, invocation_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}/report.pdf
-        GET /api/invocations/{invocation_id}/report.pdf
-
-        Get JSON summarizing invocation for reporting.
-        """
-        kwd["format"] = "pdf"
-        trans.response.set_content_type("application/pdf")
-        return self.workflow_manager.get_invocation_report(trans, invocation_id, **kwd)
-
-    @expose_api
-    def invocation_step(self, trans, invocation_id, step_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}/steps/{step_id}
-        GET /api/invocations/{invocation_id}/steps/{step_id}
-
-        :param  invocation_id:      the invocation id (required)
-        :type   invocation_id:      str
-
-        :param  step_id:      encoded id of the WorkflowInvocationStep (required)
-        :type   step_id:      str
-
-        :param  payload:       payload containing update action information
-                               for running workflow.
-
-        :raises: exceptions.MessageException, exceptions.ObjectNotFound
-        """
-        decoded_invocation_step_id = self.decode_id(step_id)
-        invocation_step = self.workflow_manager.get_invocation_step(trans, decoded_invocation_step_id)
-        return self.__encode_invocation_step(trans, invocation_step)
-
-    @expose_api_anonymous_and_sessionless
-    def invocation_step_jobs_summary(self, trans: GalaxyWebTransaction, invocation_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}/step_jobs_summary
-        GET /api/invocations/{invocation_id}/step_jobs_summary
-
-        return job state summary info aggregated across per step of the workflow invocation
-
-        Warning: We allow anyone to fetch job state information about any object they
-        can guess an encoded ID for - it isn't considered protected data. This keeps
-        polling IDs as part of state calculation for large histories and collections as
-        efficient as possible.
-
-        :param  invocation_id:    the invocation id (required)
-        :type   invocation_id:    str
-
-        :rtype:     dict[]
-        :returns:   an array of job summary object dictionaries for each step
-        """
-        decoded_invocation_id = self.decode_id(invocation_id)
-        ids = []
-        types = []
-        for job_source_type, job_source_id, _ in invocation_job_source_iter(trans.sa_session, decoded_invocation_id):
-            ids.append(job_source_id)
-            types.append(job_source_type)
-        return [self.encode_all_ids(trans, s) for s in fetch_job_states(trans.sa_session, ids, types)]
-
-    @expose_api_anonymous_and_sessionless
-    def invocation_jobs_summary(self, trans: GalaxyWebTransaction, invocation_id, **kwd):
-        """
-        GET /api/workflows/{workflow_id}/invocations/{invocation_id}/jobs_summary
-        GET /api/invocations/{invocation_id}/jobs_summary
-
-        return job state summary info aggregated across all current jobs of workflow invocation
-
-        Warning: We allow anyone to fetch job state information about any object they
-        can guess an encoded ID for - it isn't considered protected data. This keeps
-        polling IDs as part of state calculation for large histories and collections as
-        efficient as possible.
-
-        :param  invocation_id:    the invocation id (required)
-        :type   invocation_id:    str
-
-        :rtype:     dict
-        :returns:   a job summary object merged for all steps in workflow invocation
-        """
-        ids = [self.decode_id(invocation_id)]
-        types = ["WorkflowInvocation"]
-        return [self.encode_all_ids(trans, s) for s in fetch_job_states(trans.sa_session, ids, types)][0]
-
-    @expose_api
-    def update_invocation_step(self, trans: GalaxyWebTransaction, invocation_id, step_id, payload, **kwd):
-        """
-        PUT /api/workflows/{workflow_id}/invocations/{invocation_id}/steps/{step_id}
-        PUT /api/invocations/{invocation_id}/steps/{step_id}
-
-        Update state of running workflow step invocation - still very nebulous
-        but this would be for stuff like confirming paused steps can proceed
-        etc....
-
-        :param  invocation_id:      the usage id (required)
-        :type   invocation_id:      str
-
-        :param  step_id:      encoded id of the WorkflowInvocationStep (required)
-        :type   step_id:      str
-
-        :raises: exceptions.MessageException, exceptions.ObjectNotFound
-        """
-        decoded_invocation_step_id = self.decode_id(step_id)
-        action = payload.get("action", None)
-
-        invocation_step = self.workflow_manager.update_invocation_step(
-            trans,
-            decoded_invocation_step_id,
-            action=action,
-        )
-        return self.__encode_invocation_step(trans, invocation_step)
-
     def _workflow_from_dict(self, trans, data, workflow_create_options, source=None):
         """Creates a workflow from a dict.
 
         Created workflow is stored in the database and returned.
         """
         publish = workflow_create_options.publish
         importable = workflow_create_options.is_importable
@@ -1097,37 +731,58 @@
             item = tools[k]
             tool_shed_url = f"https://{item['tool_shed']}/"
             name = item["name"]
             owner = item["owner"]
             changeset_revision = item["changeset_revision"]
             irm.install(tool_shed_url, name, owner, changeset_revision, install_options)
 
-    def __encode_invocation_step(self, trans: ProvidesUserContext, invocation_step):
-        return self.encode_all_ids(trans, invocation_step.to_dict("element"), True)
-
     def __get_stored_accessible_workflow(self, trans, workflow_id, **kwd):
         instance = util.string_as_bool(kwd.get("instance", "false"))
         return self.workflow_manager.get_stored_accessible_workflow(trans, workflow_id, by_stored_id=not instance)
 
     def __get_stored_workflow(self, trans, workflow_id, **kwd):
         instance = util.string_as_bool(kwd.get("instance", "false"))
         return self.workflow_manager.get_stored_workflow(trans, workflow_id, by_stored_id=not instance)
 
-    def __encode_invocation(self, invocation, **kwd):
-        params = InvocationSerializationParams(**kwd)
-        return self.invocations_service.serialize_workflow_invocation(invocation, params)
 
+StoredWorkflowIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Stored Workflow ID", description="The encoded database identifier of the Stored Workflow."),
+]
 
-StoredWorkflowIDPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Stored Workflow ID", description="The encoded database identifier of the Stored Workflow."
-)
+InvocationIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(..., title="Invocation ID", description="The encoded database identifier of the Invocation."),
+]
 
-InvocationIDPathParam: DecodedDatabaseIdField = Path(
-    ..., title="Invocation ID", description="The encoded database identifier of the Invocation."
-)
+WorkflowInvocationStepIDPathParam = Annotated[
+    DecodedDatabaseIdField,
+    Path(
+        ...,
+        title="WorkflowInvocationStep ID",
+        description="The encoded database identifier of the WorkflowInvocationStep.",
+    ),
+]
+
+InvocationsInstanceQueryParam = Annotated[
+    Optional[bool],
+    Query(
+        title="Instance",
+        description="Is provided workflow id for Workflow instead of StoredWorkflow?",
+    ),
+]
+
+MultiTypeWorkflowIDPathParam = Annotated[
+    Union[UUID4, UUID1, DecodedDatabaseIdField],
+    Path(
+        ...,
+        title="Workflow ID",
+        description="The database identifier - UUID or encoded - of the Workflow.",
+    ),
+]
 
 DeletedQueryParam: bool = Query(
     default=False, title="Display deleted", description="Whether to restrict result to deleted workflows."
 )
 
 HiddenQueryParam: bool = Query(
     default=False, title="Display hidden", description="Whether to restrict result to hidden workflows."
@@ -1160,17 +815,36 @@
 LimitQueryParam: Optional[int] = Query(default=None, title="Limit number of queries.")
 
 OffsetQueryParam: Optional[int] = Query(
     default=0,
     title="Number of workflows to skip in sorted query (to enable pagination).",
 )
 
-InstanceQueryParam: Optional[bool] = Query(
-    default=False, title="True when fetching by Workflow ID, False when fetching by StoredWorkflow ID."
-)
+InstanceQueryParam = Annotated[
+    Optional[bool],
+    Query(
+        title="True when fetching by Workflow ID, False when fetching by StoredWorkflow ID.",
+    ),
+]
+
+LegacyQueryParam = Annotated[
+    Optional[bool],
+    Query(
+        title="Legacy",
+        description="Use the legacy workflow format.",
+    ),
+]
+
+VersionQueryParam = Annotated[
+    Optional[int],
+    Query(
+        title="Version",
+        description="The version of the workflow to fetch.",
+    ),
+]
 
 query_tags = [
     IndexQueryTag("name", "The stored workflow's name.", "n"),
     IndexQueryTag(
         "tag",
         "The workflow's tag, if the tag contains a colon an approach will be made to match the key and value of the tag separately.",
         "t",
@@ -1194,14 +868,32 @@
 
 SkipStepCountsQueryParam: bool = Query(
     default=False,
     title="Skip step counts.",
     description="Set this to true to skip joining workflow step counts and optimize the resulting index query. Response objects will not contain step counts.",
 )
 
+InvokeWorkflowBody = Annotated[
+    InvokeWorkflowPayload,
+    Body(
+        default=...,
+        title="Invoke workflow",
+        description="The values to invoke a workflow.",
+    ),
+]
+
+RefactorWorkflowBody = Annotated[
+    RefactorRequest,
+    Body(
+        default=...,
+        title="Refactor workflow",
+        description="The values to refactor a workflow.",
+    ),
+]
+
 
 @router.cbv
 class FastAPIWorkflows:
     service: WorkflowsService = depends(WorkflowsService)
 
     @router.get(
         "/api/workflows",
@@ -1221,15 +913,15 @@
         sort_desc: Optional[bool] = SortDescQueryParam,
         limit: Optional[int] = LimitQueryParam,
         offset: Optional[int] = OffsetQueryParam,
         search: Optional[str] = SearchQueryParam,
         skip_step_counts: bool = SkipStepCountsQueryParam,
     ) -> List[Dict[str, Any]]:
         """Lists stored workflows viewable by the user."""
-        payload = WorkflowIndexPayload.construct(
+        payload = WorkflowIndexPayload.model_construct(
             show_published=show_published,
             show_hidden=show_hidden,
             show_deleted=show_deleted,
             show_shared=show_shared,
             missing_tools=missing_tools,
             sort_by=sort_by,
             sort_desc=sort_desc,
@@ -1239,136 +931,182 @@
             skip_step_counts=skip_step_counts,
         )
         workflows, total_matches = self.service.index(trans, payload, include_total_count=True)
         response.headers["total_matches"] = str(total_matches)
         return workflows
 
     @router.get(
-        "/api/workflows/{id}/sharing",
+        "/api/workflows/{workflow_id}/sharing",
         summary="Get the current sharing status of the given item.",
     )
     def sharing(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ) -> SharingStatus:
         """Return the sharing status of the item."""
-        return self.service.shareable_service.sharing(trans, id)
+        return self.service.shareable_service.sharing(trans, workflow_id)
 
     @router.put(
-        "/api/workflows/{id}/enable_link_access",
+        "/api/workflows/{workflow_id}/enable_link_access",
         summary="Makes this item accessible by a URL link.",
     )
     def enable_link_access(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ) -> SharingStatus:
         """Makes this item accessible by a URL link and return the current sharing status."""
-        return self.service.shareable_service.enable_link_access(trans, id)
+        return self.service.shareable_service.enable_link_access(trans, workflow_id)
 
     @router.put(
-        "/api/workflows/{id}/disable_link_access",
+        "/api/workflows/{workflow_id}/disable_link_access",
         summary="Makes this item inaccessible by a URL link.",
     )
     def disable_link_access(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ) -> SharingStatus:
         """Makes this item inaccessible by a URL link and return the current sharing status."""
-        return self.service.shareable_service.disable_link_access(trans, id)
+        return self.service.shareable_service.disable_link_access(trans, workflow_id)
+
+    @router.put(
+        "/api/workflows/{workflow_id}/refactor",
+        summary="Updates the workflow stored with the given ID.",
+    )
+    def refactor(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        payload: RefactorWorkflowBody,
+        instance: InstanceQueryParam = False,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> RefactorResponse:
+        return self.service.refactor(trans, workflow_id, payload, instance or False)
 
     @router.put(
-        "/api/workflows/{id}/publish",
+        "/api/workflows/{workflow_id}/publish",
         summary="Makes this item public and accessible by a URL link.",
     )
     def publish(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ) -> SharingStatus:
         """Makes this item publicly available by a URL link and return the current sharing status."""
-        return self.service.shareable_service.publish(trans, id)
+        return self.service.shareable_service.publish(trans, workflow_id)
 
     @router.put(
-        "/api/workflows/{id}/unpublish",
+        "/api/workflows/{workflow_id}/unpublish",
         summary="Removes this item from the published list.",
     )
     def unpublish(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ) -> SharingStatus:
         """Removes this item from the published list and return the current sharing status."""
-        return self.service.shareable_service.unpublish(trans, id)
+        return self.service.shareable_service.unpublish(trans, workflow_id)
 
     @router.put(
-        "/api/workflows/{id}/share_with_users",
+        "/api/workflows/{workflow_id}/share_with_users",
         summary="Share this item with specific users.",
     )
     def share_with_users(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
         payload: ShareWithPayload = Body(...),
     ) -> ShareWithStatus:
         """Shares this item with specific users and return the current sharing status."""
-        return self.service.shareable_service.share_with_users(trans, id, payload)
+        return self.service.shareable_service.share_with_users(trans, workflow_id, payload)
 
     @router.put(
-        "/api/workflows/{id}/slug",
+        "/api/workflows/{workflow_id}/slug",
         summary="Set a new slug for this shared item.",
         status_code=status.HTTP_204_NO_CONTENT,
     )
     def set_slug(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
         payload: SetSlugPayload = Body(...),
     ):
         """Sets a new slug to access this item by URL. The new slug must be unique."""
-        self.service.shareable_service.set_slug(trans, id, payload)
+        self.service.shareable_service.set_slug(trans, workflow_id, payload)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.delete(
         "/api/workflows/{workflow_id}",
         summary="Add the deleted flag to a workflow.",
     )
     def delete_workflow(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        workflow_id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ):
         self.service.delete(trans, workflow_id)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
     @router.post(
         "/api/workflows/{workflow_id}/undelete",
         summary="Remove the deleted flag from a workflow.",
     )
     def undelete_workflow(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        workflow_id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
     ):
         self.service.undelete(trans, workflow_id)
         return Response(status_code=status.HTTP_204_NO_CONTENT)
 
+    @router.post(
+        "/api/workflows/{workflow_id}/invocations",
+        name="Invoke workflow",
+        summary="Schedule the workflow specified by `workflow_id` to run.",
+    )
+    @router.post(
+        "/api/workflows/{workflow_id}/usage",
+        name="Invoke workflow",
+        summary="Schedule the workflow specified by `workflow_id` to run.",
+        deprecated=True,
+    )
+    def invoke(
+        self,
+        payload: InvokeWorkflowBody,
+        workflow_id: MultiTypeWorkflowIDPathParam,
+        trans: ProvidesHistoryContext = DependsOnTrans,
+    ) -> Union[WorkflowInvocationResponse, List[WorkflowInvocationResponse]]:
+        return self.service.invoke_workflow(trans, workflow_id, payload)
+
     @router.get(
         "/api/workflows/{workflow_id}/versions",
         summary="List all versions of a workflow.",
     )
     def show_versions(
         self,
+        workflow_id: StoredWorkflowIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        workflow_id: DecodedDatabaseIdField = StoredWorkflowIDPathParam,
-        instance: Optional[bool] = InstanceQueryParam,
+        instance: InstanceQueryParam = False,
     ):
-        return self.service.get_versions(trans, workflow_id, instance)
+        return self.service.get_versions(trans, workflow_id, instance or False)
+
+    @router.get(
+        "/api/workflows/{workflow_id}/counts",
+        summary="Get state counts for accessible workflow.",
+        name="invocation_state_counts",
+        operation_id="workflows__invocation_counts",
+    )
+    def invocation_counts(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        instance: InvocationsInstanceQueryParam = False,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationsStateCounts:
+        return self.service.invocation_counts(trans, workflow_id, instance or False)
 
     @router.get(
         "/api/workflows/menu",
         summary="Get workflows present in the tools panel.",
     )
     def get_workflow_menu(
         self,
@@ -1387,62 +1125,605 @@
             missing_tools=missing_tools,
         )
         return self.service.get_workflow_menu(
             trans,
             payload=payload,
         )
 
+    @router.get(
+        "/api/workflows/{workflow_id}",
+        summary="Displays information needed to run a workflow.",
+        name="show_workflow",
+    )
+    def show_workflow(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        instance: InstanceQueryParam = False,
+        legacy: LegacyQueryParam = False,
+        version: VersionQueryParam = None,
+        trans: ProvidesHistoryContext = DependsOnTrans,
+    ) -> StoredWorkflowDetailed:
+        return self.service.show_workflow(trans, workflow_id, instance, legacy, version)
+
+
+StepDetailQueryParam = Annotated[
+    bool,
+    Query(
+        title="Include step details",
+        description=(
+            "Include details for individual invocation steps and populate a steps attribute in the resulting dictionary."
+        ),
+    ),
+]
+LegacyJobStateQueryParam = Annotated[
+    bool,
+    Query(
+        title="Replace with job state",
+        description=(
+            """Populate the invocation step state with the job state instead of the invocation step state.
+        This will also produce one step per job in mapping jobs to mimic the older behavior with respect to collections.
+        Partially scheduled steps may provide incomplete information and the listed steps outputs
+        are not the mapped over step outputs but the individual job outputs."""
+        ),
+    ),
+]
+
+WorkflowIdQueryParam = Annotated[
+    Optional[DecodedDatabaseIdField],
+    Query(
+        title="Workflow ID",
+        description="Return only invocations for this Workflow ID",
+    ),
+]
+
+HistoryIdQueryParam = Annotated[
+    Optional[DecodedDatabaseIdField],
+    Query(
+        title="History ID",
+        description="Return only invocations for this History ID",
+    ),
+]
+
+JobIdQueryParam = Annotated[
+    Optional[DecodedDatabaseIdField],
+    Query(
+        title="Job ID",
+        description="Return only invocations for this Job ID",
+    ),
+]
+
+UserIdQueryParam = Annotated[
+    Optional[DecodedDatabaseIdField],
+    Query(
+        title="User ID",
+        description="Return invocations for this User ID.",
+    ),
+]
+
+InvocationsSortByQueryParam = Annotated[
+    Optional[InvocationSortByEnum],
+    Query(
+        title="Sort By",
+        description="Sort Workflow Invocations by this attribute",
+    ),
+]
+
+InvocationsSortDescQueryParam = Annotated[
+    bool,
+    Query(
+        title="Sort Descending",
+        description="Sort in descending order?",
+    ),
+]
+
+InvocationsIncludeTerminalQueryParam = Annotated[
+    Optional[bool],
+    Query(
+        title="Include Terminal",
+        description="Set to false to only include terminal Invocations.",
+    ),
+]
+
+InvocationsLimitQueryParam = Annotated[
+    Optional[int],
+    Query(
+        title="Limit",
+        description="Limit the number of invocations to return.",
+    ),
+]
+
+InvocationsOffsetQueryParam = Annotated[
+    Optional[int],
+    Query(
+        title="Offset",
+        description="Number of invocations to skip.",
+    ),
+]
+
+
+CreateInvocationsFromStoreBody = Annotated[
+    CreateInvocationsFromStorePayload,
+    Body(
+        default=...,
+        title="Create invocations from store",
+        description="The values and serialization parameters for creating invocations from a supplied model store.",
+    ),
+]
+
 
 @router.cbv
 class FastAPIInvocations:
     invocations_service: InvocationsService = depends(InvocationsService)
 
     @router.post(
+        "/api/invocations/from_store",
+        name="create_invocations_from_store",
+        description="Create invocation(s) from a supplied model store.",
+    )
+    def create_invocations_from_store(
+        self,
+        payload: CreateInvocationsFromStoreBody,
+        trans: ProvidesHistoryContext = DependsOnTrans,
+    ) -> List[WorkflowInvocationResponse]:
+        """
+        Input can be an archive describing a Galaxy model store containing an
+        workflow invocation - for instance one created with with write_store
+        or prepare_store_download endpoint.
+        """
+        create_payload = CreateInvocationFromStore(**payload.model_dump())
+        serialization_params = InvocationSerializationParams(**payload.model_dump())
+        return self.invocations_service.create_from_store(trans, create_payload, serialization_params)
+
+    @router.get(
+        "/api/invocations",
+        summary="Get the list of a user's workflow invocations.",
+        name="index_invocations",
+    )
+    def index_invocations(
+        self,
+        response: Response,
+        workflow_id: WorkflowIdQueryParam = None,
+        history_id: HistoryIdQueryParam = None,
+        job_id: JobIdQueryParam = None,
+        user_id: UserIdQueryParam = None,
+        sort_by: InvocationsSortByQueryParam = None,
+        sort_desc: InvocationsSortDescQueryParam = False,
+        include_terminal: InvocationsIncludeTerminalQueryParam = True,
+        limit: InvocationsLimitQueryParam = None,
+        offset: InvocationsOffsetQueryParam = None,
+        instance: InvocationsInstanceQueryParam = False,
+        view: SerializationViewQueryParam = None,
+        step_details: StepDetailQueryParam = False,
+        include_nested_invocations: bool = True,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> List[WorkflowInvocationResponse]:
+        if not trans.user:
+            # Anon users don't have accessible invocations (currently, though published invocations should be a thing)
+            response.headers["total_matches"] = "0"
+            return []
+        invocation_payload = InvocationIndexPayload(
+            workflow_id=workflow_id,
+            history_id=history_id,
+            job_id=job_id,
+            user_id=user_id,
+            sort_by=sort_by,
+            sort_desc=sort_desc,
+            include_terminal=include_terminal,
+            limit=limit,
+            offset=offset,
+            instance=instance,
+            include_nested_invocations=include_nested_invocations,
+        )
+        serialization_params = InvocationSerializationParams(
+            view=view,
+            step_details=step_details,
+        )
+        invocations, total_matches = self.invocations_service.index(trans, invocation_payload, serialization_params)
+        response.headers["total_matches"] = str(total_matches)
+        return invocations
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations",
+        summary="Get the list of a user's workflow invocations.",
+        name="index_invocations",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage",
+        summary="Get the list of a user's workflow invocations.",
+        name="index_invocations",
+        deprecated=True,
+    )
+    def index_workflow_invocations(
+        self,
+        response: Response,
+        workflow_id: StoredWorkflowIDPathParam,
+        history_id: HistoryIdQueryParam = None,
+        job_id: JobIdQueryParam = None,
+        user_id: UserIdQueryParam = None,
+        sort_by: InvocationsSortByQueryParam = None,
+        sort_desc: InvocationsSortDescQueryParam = False,
+        include_terminal: InvocationsIncludeTerminalQueryParam = True,
+        limit: InvocationsLimitQueryParam = None,
+        offset: InvocationsOffsetQueryParam = None,
+        instance: InvocationsInstanceQueryParam = False,
+        view: SerializationViewQueryParam = None,
+        step_details: StepDetailQueryParam = False,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> List[WorkflowInvocationResponse]:
+        invocations = self.index_invocations(
+            response=response,
+            workflow_id=workflow_id,
+            history_id=history_id,
+            job_id=job_id,
+            user_id=user_id,
+            sort_by=sort_by,
+            sort_desc=sort_desc,
+            include_terminal=include_terminal,
+            limit=limit,
+            offset=offset,
+            instance=instance,
+            view=view,
+            step_details=step_details,
+            trans=trans,
+        )
+        return invocations
+
+    @router.post(
         "/api/invocations/{invocation_id}/prepare_store_download",
         summary="Prepare a workflow invocation export-style download.",
     )
     def prepare_store_download(
         self,
+        invocation_id: InvocationIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        invocation_id: DecodedDatabaseIdField = InvocationIDPathParam,
         payload: PrepareStoreDownloadPayload = Body(...),
     ) -> AsyncFile:
         return self.invocations_service.prepare_store_download(
             trans,
             invocation_id,
             payload,
         )
 
     @router.post(
         "/api/invocations/{invocation_id}/write_store",
         summary="Prepare a workflow invocation export-style download and write to supplied URI.",
     )
     def write_store(
         self,
+        invocation_id: InvocationIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        invocation_id: DecodedDatabaseIdField = InvocationIDPathParam,
         payload: WriteInvocationStoreToPayload = Body(...),
     ) -> AsyncTaskResultSummary:
         rval = self.invocations_service.write_store(
             trans,
             invocation_id,
             payload,
         )
         return rval
 
+    @router.get("/api/invocations/{invocation_id}", summary="Get detailed description of a workflow invocation.")
+    def show_invocation(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        step_details: StepDetailQueryParam = False,
+        legacy_job_state: LegacyJobStateQueryParam = False,
+    ) -> WorkflowInvocationResponse:
+        serialization_params = InvocationSerializationParams(
+            step_details=step_details, legacy_job_state=legacy_job_state
+        )
+        return self.invocations_service.show(trans, invocation_id, serialization_params, eager=True)
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}",
+        summary="Get detailed description of a workflow invocation.",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}",
+        summary="Get detailed description of a workflow invocation.",
+        deprecated=True,
+    )
+    def show_workflow_invocation(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        step_details: StepDetailQueryParam = False,
+        legacy_job_state: LegacyJobStateQueryParam = False,
+    ) -> WorkflowInvocationResponse:
+        """An alias for `GET /api/invocations/{invocation_id}`. `workflow_id` is ignored."""
+        return self.show_invocation(
+            trans=trans, invocation_id=invocation_id, step_details=step_details, legacy_job_state=legacy_job_state
+        )
+
+    @router.delete("/api/invocations/{invocation_id}", summary="Cancel the specified workflow invocation.")
+    def cancel_invocation(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        step_details: StepDetailQueryParam = False,
+        legacy_job_state: LegacyJobStateQueryParam = False,
+    ) -> WorkflowInvocationResponse:
+        serialization_params = InvocationSerializationParams(
+            step_details=step_details, legacy_job_state=legacy_job_state
+        )
+        return self.invocations_service.cancel(trans, invocation_id, serialization_params)
+
+    @router.delete(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}", summary="Cancel the specified workflow invocation."
+    )
+    @router.delete(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}",
+        summary="Cancel the specified workflow invocation.",
+        deprecated=True,
+    )
+    def cancel_workflow_invocation(
+        self,
+        invocation_id: InvocationIDPathParam,
+        workflow_id: StoredWorkflowIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        step_details: StepDetailQueryParam = False,
+        legacy_job_state: LegacyJobStateQueryParam = False,
+    ) -> WorkflowInvocationResponse:
+        """An alias for `DELETE /api/invocations/{invocation_id}`. `workflow_id` is ignored."""
+
+        return self.cancel_invocation(
+            trans=trans, invocation_id=invocation_id, step_details=step_details, legacy_job_state=legacy_job_state
+        )
+
+    @router.get(
+        "/api/invocations/{invocation_id}/report",
+        summary="Get JSON summarizing invocation for reporting.",
+    )
+    def show_invocation_report(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationReport:
+        return self.invocations_service.show_invocation_report(trans, invocation_id)
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/report",
+        summary="Get JSON summarizing invocation for reporting.",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/report",
+        summary="Get JSON summarizing invocation for reporting.",
+        deprecated=True,
+    )
+    def show_workflow_invocation_report(
+        self,
+        invocation_id: InvocationIDPathParam,
+        workflow_id: StoredWorkflowIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationReport:
+        """An alias for `GET /api/invocations/{invocation_id}/report`. `workflow_id` is ignored."""
+        return self.show_invocation_report(trans=trans, invocation_id=invocation_id)
+
+    @router.get(
+        "/api/invocations/{invocation_id}/report.pdf",
+        summary="Get PDF summarizing invocation for reporting.",
+        response_class=StreamingResponse,
+    )
+    def show_invocation_report_pdf(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ):
+        wfi_report = self.invocations_service.show_invocation_report(trans, invocation_id, format="pdf")
+        return StreamingResponse(
+            content=BytesIO(wfi_report),
+            media_type="application/pdf",
+            headers={
+                "Content-Disposition": f'attachment; filename="report_galaxy_invocation_{trans.security.encode_id(invocation_id)}.pdf"',
+                "Access-Control-Expose-Headers": "Content-Disposition",
+            },
+        )
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/report.pdf",
+        summary="Get PDF summarizing invocation for reporting.",
+        response_class=StreamingResponse,
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/report.pdf",
+        summary="Get PDF summarizing invocation for reporting.",
+        response_class=StreamingResponse,
+        deprecated=True,
+    )
+    def show_workflow_invocation_report_pdf(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ):
+        """An alias for `GET /api/invocations/{invocation_id}/report.pdf`. `workflow_id` is ignored."""
+        return self.show_invocation_report_pdf(trans=trans, invocation_id=invocation_id)
+
+    @router.get(
+        "/api/invocations/steps/{step_id}",
+        summary="Show details of workflow invocation step.",
+    )
+    def step(
+        self,
+        step_id: WorkflowInvocationStepIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationStep:
+        return self.invocations_service.show_invocation_step(trans, step_id)
+
+    @router.get(
+        "/api/invocations/{invocation_id}/steps/{step_id}",
+        summary="Show details of workflow invocation step.",
+    )
+    def invocation_step(
+        self,
+        invocation_id: InvocationIDPathParam,
+        step_id: WorkflowInvocationStepIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationStep:
+        """An alias for `GET /api/invocations/steps/{step_id}`. `invocation_id` is ignored."""
+        return self.step(trans=trans, step_id=step_id)
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/steps/{step_id}",
+        summary="Show details of workflow invocation step.",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/steps/{step_id}",
+        summary="Show details of workflow invocation step.",
+        deprecated=True,
+    )
+    def workflow_invocation_step(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        step_id: WorkflowInvocationStepIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationStep:
+        """An alias for `GET /api/invocations/{invocation_id}/steps/{step_id}`. `workflow_id` and `invocation_id` are ignored."""
+        return self.invocation_step(trans=trans, invocation_id=invocation_id, step_id=step_id)
+
+    @router.put(
+        "/api/invocations/{invocation_id}/steps/{step_id}",
+        summary="Update state of running workflow step invocation - still very nebulous but this would be for stuff like confirming paused steps can proceed etc.",
+    )
+    def update_invocation_step(
+        self,
+        invocation_id: InvocationIDPathParam,
+        step_id: WorkflowInvocationStepIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        payload: InvocationUpdatePayload = Body(...),
+    ) -> InvocationStep:
+        return self.invocations_service.update_invocation_step(trans=trans, step_id=step_id, action=payload.action)
+
+    @router.put(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/steps/{step_id}",
+        summary="Update state of running workflow step invocation.",
+    )
+    @router.put(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/steps/{step_id}",
+        summary="Update state of running workflow step invocation.",
+        deprecated=True,
+    )
+    def update_workflow_invocation_step(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        step_id: WorkflowInvocationStepIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+        payload: InvocationUpdatePayload = Body(...),
+    ) -> InvocationStep:
+        """An alias for `PUT /api/invocations/{invocation_id}/steps/{step_id}`. `workflow_id` is ignored."""
+        return self.update_invocation_step(trans=trans, invocation_id=invocation_id, step_id=step_id, payload=payload)
+
+    @router.get(
+        "/api/invocations/{invocation_id}/step_jobs_summary",
+        summary="Get job state summary info aggregated per step of the workflow invocation.",
+    )
+    def invocation_step_jobs_summary(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> List[
+        Union[
+            InvocationStepJobsResponseStepModel,
+            InvocationStepJobsResponseJobModel,
+            InvocationStepJobsResponseCollectionJobsModel,
+        ]
+    ]:
+        """
+        Warning: We allow anyone to fetch job state information about any object they
+        can guess an encoded ID for - it isn't considered protected data. This keeps
+        polling IDs as part of state calculation for large histories and collections as
+        efficient as possible.
+        """
+        step_jobs_summary = self.invocations_service.show_invocation_step_jobs_summary(trans, invocation_id)
+        return [
+            (
+                InvocationStepJobsResponseStepModel(**summary)
+                if summary["model"] == "WorkflowInvocationStep"
+                else (
+                    InvocationStepJobsResponseJobModel(**summary)
+                    if summary["model"] == "Job"
+                    else InvocationStepJobsResponseCollectionJobsModel(**summary)
+                )
+            )
+            for summary in step_jobs_summary
+        ]
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/step_jobs_summary",
+        summary="Get job state summary info aggregated per step of the workflow invocation.",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/step_jobs_summary",
+        summary="Get job state summary info aggregated per step of the workflow invocation.",
+        deprecated=True,
+    )
+    def workflow_invocation_step_jobs_summary(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> List[
+        Union[
+            InvocationStepJobsResponseStepModel,
+            InvocationStepJobsResponseJobModel,
+            InvocationStepJobsResponseCollectionJobsModel,
+        ]
+    ]:
+        """An alias for `GET /api/invocations/{invocation_id}/step_jobs_summary`. `workflow_id` is ignored."""
+        return self.invocation_step_jobs_summary(trans=trans, invocation_id=invocation_id)
+
+    @router.get(
+        "/api/invocations/{invocation_id}/jobs_summary",
+        summary="Get job state summary info aggregated across all current jobs of the workflow invocation.",
+    )
+    def invocation_jobs_summary(
+        self,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationJobsResponse:
+        """
+        Warning: We allow anyone to fetch job state information about any object they
+        can guess an encoded ID for - it isn't considered protected data. This keeps
+        polling IDs as part of state calculation for large histories and collections as
+        efficient as possible.
+        """
+        jobs_summary = self.invocations_service.show_invocation_jobs_summary(trans, invocation_id)
+        return InvocationJobsResponse(**jobs_summary)
+
+    @router.get(
+        "/api/workflows/{workflow_id}/invocations/{invocation_id}/jobs_summary",
+        summary="Get job state summary info aggregated across all current jobs of the workflow invocation.",
+    )
+    @router.get(
+        "/api/workflows/{workflow_id}/usage/{invocation_id}/jobs_summary",
+        summary="Get job state summary info aggregated across all current jobs of the workflow invocation.",
+        deprecated=True,
+    )
+    def workflow_invocation_jobs_summary(
+        self,
+        workflow_id: StoredWorkflowIDPathParam,
+        invocation_id: InvocationIDPathParam,
+        trans: ProvidesUserContext = DependsOnTrans,
+    ) -> InvocationJobsResponse:
+        """An alias for `GET /api/invocations/{invocation_id}/jobs_summary`. `workflow_id` is ignored."""
+        return self.invocation_jobs_summary(trans=trans, invocation_id=invocation_id)
+
     # TODO: remove this endpoint after 23.1 release
     @router.get(
         "/api/invocations/{invocation_id}/biocompute",
         summary="Return a BioCompute Object for the workflow invocation.",
         deprecated=True,
     )
     def export_invocation_bco(
         self,
+        invocation_id: InvocationIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        invocation_id: DecodedDatabaseIdField = InvocationIDPathParam,
         merge_history_metadata: Optional[bool] = Query(default=False),
     ):
         """
         The BioCompute Object endpoints are in beta - important details such
         as how inputs and outputs are represented, how the workflow is encoded,
         and how author and version information is encoded, and how URLs are
         generated will very likely change in important ways over time.
@@ -1467,16 +1748,16 @@
         "/api/invocations/{invocation_id}/biocompute/download",
         summary="Return a BioCompute Object for the workflow invocation as a file for download.",
         response_class=StreamingResponse,
         deprecated=True,
     )
     def download_invocation_bco(
         self,
+        invocation_id: InvocationIDPathParam,
         trans: ProvidesUserContext = DependsOnTrans,
-        invocation_id: DecodedDatabaseIdField = InvocationIDPathParam,
         merge_history_metadata: Optional[bool] = Query(default=False),
     ):
         """
         The BioCompute Object endpoints are in beta - important details such
         as how inputs and outputs are represented, how the workflow is encoded,
         and how author and version information is encoded, and how URLs are
         generated will very likely change in important ways over time.
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/buildapp.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/buildapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides factory methods to assemble the Galaxy web application
 """
+
 import atexit
 import logging
 import sys
 import threading
 import traceback
 from urllib.parse import urljoin
 
@@ -258,22 +259,24 @@
     webapp.add_client_route("/datasets/{dataset_id}/preview")
     webapp.add_client_route("/datasets/{dataset_id}/show_params")
     webapp.add_client_route("/collection/{collection_id}/edit")
     webapp.add_client_route("/jobs/submission/success")
     webapp.add_client_route("/jobs/{job_id}/view")
     webapp.add_client_route("/workflows/list")
     webapp.add_client_route("/workflows/list_published")
+    webapp.add_client_route("/workflows/list_shared_with_me")
     webapp.add_client_route("/workflows/edit")
     webapp.add_client_route("/workflows/export")
     webapp.add_client_route("/workflows/create")
     webapp.add_client_route("/workflows/run")
     webapp.add_client_route("/workflows/import")
     webapp.add_client_route("/workflows/trs_import")
     webapp.add_client_route("/workflows/trs_search")
     webapp.add_client_route("/workflows/invocations")
+    webapp.add_client_route("/workflows/invocations/{invocation_id}")
     webapp.add_client_route("/workflows/sharing")
     webapp.add_client_route("/workflows/{stored_workflow_id}/invocations")
     webapp.add_client_route("/workflows/invocations/report")
     # webapp.add_client_route('/workflows/invocations/view_bco')
     webapp.add_client_route("/custom_builds")
     webapp.add_client_route("/interactivetool_entry_points/list")
     webapp.add_client_route("/libraries{path:.*?}")
@@ -323,14 +326,29 @@
         "/api/upload/resumable_upload/{session_id}",
         controller="uploads",
         action="hooks",
         conditions=dict(method=["PATCH"]),
     )
     webapp.mapper.connect("/api/upload/resumable_upload", controller="uploads", action="hooks")
     webapp.mapper.connect("/api/upload/hooks", controller="uploads", action="hooks", conditions=dict(method=["POST"]))
+
+    webapp.mapper.connect(
+        "/api/job_files/resumable_upload/{session_id}",
+        controller="job_files",
+        action="tus_patch",
+        conditions=dict(method=["PATCH"]),
+    )
+    # user facing upload has this endpoint enabled but the middleware completely masks it and the controller
+    # is not used. Probably it isn't needed there but I am keeping the doc here until we remove both
+    # routes.
+    # webapp.mapper.connect("/api/job_files/resumable_upload", controller="job_files", action="tus_post")
+    webapp.mapper.connect(
+        "/api/job_files/tus_hooks", controller="job_files", action="tus_hooks", conditions=dict(method=["POST"])
+    )
+
     webapp.mapper.resource(
         "revision",
         "revisions",
         path_prefix="/api/pages/{page_id}",
         controller="page_revisions",
         parent_resources=dict(member_name="page", collection_name="pages"),
     )
@@ -572,17 +590,14 @@
 
     webapp.mapper.resource("visualization", "visualizations", path_prefix="/api")
     webapp.mapper.resource("plugins", "plugins", path_prefix="/api")
     webapp.mapper.connect("/api/workflows/build_module", action="build_module", controller="workflows")
     webapp.mapper.connect(
         "/api/workflows/menu", action="set_workflow_menu", controller="workflows", conditions=dict(method=["PUT"])
     )
-    webapp.mapper.connect(
-        "/api/workflows/{id}/refactor", action="refactor", controller="workflows", conditions=dict(method=["PUT"])
-    )
     webapp.mapper.resource("workflow", "workflows", path_prefix="/api")
 
     # ---- visualizations registry ---- generic template renderer
     # @deprecated: this route should be considered deprecated
     webapp.add_route(
         "/visualization/show/{visualization_name}", controller="visualization", action="render", visualization_name=None
     )
@@ -668,92 +683,26 @@
     # webapp.mapper.connect(
     #     "trs_consume_import_tool_version",
     #     "/api/trs_consume/{trs_server}/tools/{tool_id}/versions/{version_id}/import",
     #     controller="trs_consumer",
     #     action="import_tool_version",
     #     conditions=dict(method=["POST"]),
     # )
-
     webapp.mapper.connect(
-        "list_invocations",
-        "/api/invocations",
+        "/api/workflows/{encoded_workflow_id}",
         controller="workflows",
-        action="index_invocations",
-        conditions=dict(method=["GET"]),
+        action="update",
+        conditions=dict(method=["PUT"]),
     )
-
     webapp.mapper.connect(
-        "create_invovactions_from_store",
-        "/api/invocations/from_store",
+        "/api/workflows",
         controller="workflows",
-        action="create_invocations_from_store",
+        action="create",
         conditions=dict(method=["POST"]),
     )
-
-    # API refers to usages and invocations - these mean the same thing but the
-    # usage routes should be considered deprecated.
-    invoke_names = {
-        "invocations": "",
-        "usage": "_deprecated",
-    }
-    for noun, suffix in invoke_names.items():
-        name = f"{noun}{suffix}"
-        webapp.mapper.connect(
-            f"list_workflow_{name}",
-            "/api/workflows/{workflow_id}/%s" % noun,
-            controller="workflows",
-            action="index_invocations",
-            conditions=dict(method=["GET"]),
-        )
-        webapp.mapper.connect(
-            f"workflow_{name}",
-            "/api/workflows/{workflow_id}/%s" % noun,
-            controller="workflows",
-            action="invoke",
-            conditions=dict(method=["POST"]),
-        )
-
-    def connect_invocation_endpoint(endpoint_name, endpoint_suffix, action, conditions=None):
-        # /api/invocations/<invocation_id>
-        # /api/workflows/<workflow_id>/invocations/<invocation_id>
-        # /api/workflows/<workflow_id>/usage/<invocation_id> (deprecated)
-        conditions = conditions or dict(method=["GET"])
-        webapp.mapper.connect(
-            f"workflow_invocation_{endpoint_name}",
-            f"/api/workflows/{{workflow_id}}/invocations/{{invocation_id}}{endpoint_suffix}",
-            controller="workflows",
-            action=action,
-            conditions=conditions,
-        )
-        webapp.mapper.connect(
-            f"workflow_usage_{endpoint_name}",
-            f"/api/workflows/{{workflow_id}}/usage/{{invocation_id}}{endpoint_suffix}",
-            controller="workflows",
-            action=action,
-            conditions=conditions,
-        )
-        webapp.mapper.connect(
-            f"invocation_{endpoint_name}",
-            f"/api/invocations/{{invocation_id}}{endpoint_suffix}",
-            controller="workflows",
-            action=action,
-            conditions=conditions,
-        )
-
-    connect_invocation_endpoint("show", "", action="show_invocation")
-    connect_invocation_endpoint("show_report", "/report", action="show_invocation_report")
-    connect_invocation_endpoint("show_report_pdf", "/report.pdf", action="show_invocation_report_pdf")
-    connect_invocation_endpoint("jobs_summary", "/jobs_summary", action="invocation_jobs_summary")
-    connect_invocation_endpoint("step_jobs_summary", "/step_jobs_summary", action="invocation_step_jobs_summary")
-    connect_invocation_endpoint("cancel", "", action="cancel_invocation", conditions=dict(method=["DELETE"]))
-    connect_invocation_endpoint("show_step", "/steps/{step_id}", action="invocation_step")
-    connect_invocation_endpoint(
-        "update_step", "/steps/{step_id}", action="update_invocation_step", conditions=dict(method=["PUT"])
-    )
-
     # ================================
     # ===== USERS API =====
     # ================================
 
     webapp.mapper.connect(
         "get_information",
         "/api/users/{id}/information/inputs",
@@ -1080,16 +1029,15 @@
     conf = global_conf.copy()
     conf.update(local_conf)
     # First put into place httpexceptions, which must be most closely
     # wrapped around the application (it can interact poorly with
     # other middleware):
     app = wrap_if_allowed(app, stack, httpexceptions.make_middleware, name="paste.httpexceptions", args=(conf,))
     # Statsd request timing and profiling
-    statsd_host = conf.get("statsd_host", None)
-    if statsd_host:
+    if statsd_host := conf.get("statsd_host", None):
         from galaxy.web.framework.middleware.statsd import StatsdMiddleware
 
         app = wrap_if_allowed(
             app,
             stack,
             StatsdMiddleware,
             args=(
@@ -1138,14 +1086,27 @@
         TusMiddleware,
         kwargs={
             "upload_path": urljoin(f"{application_stack.config.galaxy_url_prefix}/", "api/upload/resumable_upload"),
             "tmp_dir": application_stack.config.tus_upload_store or application_stack.config.new_file_path,
             "max_size": application_stack.config.maximum_upload_file_size,
         },
     )
+    # TUS upload middleware for job files....
+    app = wrap_if_allowed(
+        app,
+        stack,
+        TusMiddleware,
+        kwargs={
+            "upload_path": urljoin(f"{application_stack.config.galaxy_url_prefix}/", "api/job_files/resumable_upload"),
+            "tmp_dir": application_stack.config.tus_upload_store_job_files
+            or application_stack.config.tus_upload_store
+            or application_stack.config.new_file_path,
+            "max_size": application_stack.config.maximum_upload_file_size,
+        },
+    )
     # X-Forwarded-Host handling
     app = wrap_if_allowed(app, stack, XForwardedHostMiddleware)
     # Request ID middleware
     app = wrap_if_allowed(app, stack, RequestIDMiddleware)
     if asbool(conf.get("enable_per_request_sql_debugging", False)):
         from galaxy.web.framework.middleware.sqldebug import SQLDebugMiddleware
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/admin.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,67 @@
 import logging
 from typing import Set
 
 from sqlalchemy import (
     false,
     func,
+    true,
 )
 from typing_extensions import TypedDict
 
 from galaxy import (
     model,
     util,
     web,
 )
-from galaxy.exceptions import (
-    ActionInputError,
-    MessageException,
-)
+from galaxy.exceptions import ActionInputError
 from galaxy.managers.quotas import QuotaManager
-from galaxy.model import tool_shed_install as install_model
 from galaxy.model.base import transaction
+from galaxy.model.index_filter_util import (
+    raw_text_column_filter,
+    text_column_filter,
+)
 from galaxy.security.validate_user_input import validate_password
 from galaxy.structured_app import StructuredApp
-from galaxy.util import (
-    nice_size,
-    pretty_print_time_interval,
-    sanitize_text,
+from galaxy.util.search import (
+    FilteredTerm,
+    parse_filters_structured,
+    RawTextTerm,
 )
 from galaxy.web import url_for
 from galaxy.web.framework.helpers import (
     grids,
     time_ago,
 )
 from galaxy.webapps.base import controller
-from tool_shed.util.web_util import escape
 
 log = logging.getLogger(__name__)
 
 
-class UserListGrid(grids.Grid):
-    class EmailColumn(grids.TextColumn):
-        def get_value(self, trans, grid, user):
-            return escape(user.email)
-
-    class UserNameColumn(grids.TextColumn):
-        def get_value(self, trans, grid, user):
-            if user.username:
-                return escape(user.username)
-            return "not set"
-
+class UserListGrid(grids.GridData):
     class StatusColumn(grids.GridColumn):
         def get_value(self, trans, grid, user):
             if user.purged:
-                return "purged"
+                return "Purged"
             elif user.deleted:
-                return "deleted"
-            return ""
+                return "Deleted"
+            return "Available"
 
     class GroupsColumn(grids.GridColumn):
         def get_value(self, trans, grid, user):
             if user.groups:
                 return len(user.groups)
             return 0
 
     class RolesColumn(grids.GridColumn):
         def get_value(self, trans, grid, user):
             if user.roles:
                 return len(user.roles)
             return 0
 
-    class ExternalColumn(grids.GridColumn):
-        def get_value(self, trans, grid, user):
-            if user.external:
-                return "yes"
-            return "no"
-
     class LastLoginColumn(grids.GridColumn):
         def get_value(self, trans, grid, user):
             if user.galaxy_sessions:
                 return self.format(user.current_galaxy_session.update_time)
             return "never"
 
         def sort(self, trans, query, ascending, column_name=None):
@@ -93,25 +77,14 @@
 
             if not ascending:
                 query = query.order_by((last_login_subquery.c.last_login).desc().nullslast())
             else:
                 query = query.order_by((last_login_subquery.c.last_login).asc().nullsfirst())
             return query
 
-    class TimeCreatedColumn(grids.GridColumn):
-        def get_value(self, trans, grid, user):
-            return user.create_time.strftime("%x")
-
-    class ActivatedColumn(grids.GridColumn):
-        def get_value(self, trans, grid, user):
-            if user.active:
-                return "Y"
-            else:
-                return "N"
-
     class DiskUsageColumn(grids.GridColumn):
         def get_value(self, trans, grid, user):
             return user.get_disk_usage(nice_size=True)
 
         def sort(self, trans, query, ascending, column_name=None):
             if column_name is None:
                 column_name = self.key
@@ -126,105 +99,70 @@
 
     # Grid definition
     title = "Users"
     title_id = "users-grid"
     model_class = model.User
     default_sort_key = "email"
     columns = [
-        EmailColumn(
-            "Email",
-            key="email",
-            link=(lambda item: dict(controller="user", action="information", id=item.id, webapp="galaxy")),
-            attach_popup=True,
-            filterable="advanced",
-            target="top",
-        ),
-        UserNameColumn("User Name", key="username", attach_popup=False, filterable="advanced"),
-        LastLoginColumn("Last Login", format=time_ago, key="last_login", sortable=True),
-        DiskUsageColumn("Disk Usage", key="disk_usage", attach_popup=False),
-        StatusColumn("Status", attach_popup=False, key="deleted"),
-        TimeCreatedColumn("Created", attach_popup=False, key="create_time"),
-        ActivatedColumn("Activated", attach_popup=False, key="active"),
-        GroupsColumn("Groups", attach_popup=False),
-        RolesColumn("Roles", attach_popup=False),
-        ExternalColumn("External", attach_popup=False, key="external"),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.PurgedColumn("Purged", key="purged", visible=False, filterable="advanced"),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-    global_actions = [grids.GridAction("Create new user", url_args=dict(action="users/create"))]
-    operations = [
-        grids.GridOperation(
-            "Manage Information",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(controller="user", action="information", webapp="galaxy"),
-        ),
-        grids.GridOperation(
-            "Manage Roles and Groups",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/manage_roles_and_groups_for_user"),
-        ),
-        grids.GridOperation(
-            "Reset Password",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=True,
-            url_args=dict(action="form/reset_user_password"),
-            target="top",
-        ),
-        grids.GridOperation("Recalculate Disk Usage", condition=(lambda item: not item.deleted), allow_multiple=False),
-        grids.GridOperation("Generate New API Key", allow_multiple=False, async_compatible=True),
-    ]
-
-    standard_filters = [
-        grids.GridColumnFilter("Active", args=dict(deleted=False)),
-        grids.GridColumnFilter("Deleted", args=dict(deleted=True, purged=False)),
-        grids.GridColumnFilter("Purged", args=dict(purged=True)),
-        grids.GridColumnFilter("All", args=dict(deleted="All")),
+        grids.GridColumn("Email", key="email"),
+        grids.GridColumn("User Name", key="username"),
+        LastLoginColumn("Last Login", key="last_login", format=time_ago),
+        DiskUsageColumn("Disk Usage", key="disk_usage"),
+        StatusColumn("Status", key="status"),
+        grids.GridColumn("Created", key="create_time"),
+        grids.GridColumn("Activated", key="active", escape=False),
+        GroupsColumn("Groups", key="groups"),
+        RolesColumn("Roles", key="roles"),
+        grids.GridColumn("External", key="external", escape=False),
+        grids.GridColumn("Deleted", key="deleted", escape=False),
+        grids.GridColumn("Purged", key="purged", escape=False),
     ]
-    num_rows_per_page = 50
-    use_paging = True
-    default_filter = dict(purged="False")
-    use_default_filter = True
-
-    def get_current_item(self, trans, **kwargs):
-        return trans.user
-
-
-class RoleListGrid(grids.Grid):
-    class NameColumn(grids.TextColumn):
-        def get_value(self, trans, grid, role):
-            return escape(role.name)
 
-    class DescriptionColumn(grids.TextColumn):
-        def get_value(self, trans, grid, role):
-            if role.description:
-                return escape(role.description)
-            return ""
-
-    class TypeColumn(grids.TextColumn):
-        def get_value(self, trans, grid, role):
-            return role.type
+    def apply_query_filter(self, query, **kwargs):
+        INDEX_SEARCH_FILTERS = {
+            "email": "email",
+            "username": "username",
+            "is": "is",
+        }
+        deleted = False
+        purged = False
+        search_query = kwargs.get("search")
+        if search_query:
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "email":
+                        query = query.filter(text_column_filter(self.model_class.email, term))
+                    elif key == "username":
+                        query = query.filter(text_column_filter(self.model_class.username, term))
+                    elif key == "is":
+                        if q == "deleted":
+                            deleted = True
+                        elif q == "purged":
+                            purged = True
+                elif isinstance(term, RawTextTerm):
+                    query = query.filter(
+                        raw_text_column_filter(
+                            [
+                                self.model_class.email,
+                                self.model_class.username,
+                            ],
+                            term,
+                        )
+                    )
+        if purged:
+            query = query.filter(self.model_class.purged == true())
+        else:
+            query = query.filter(self.model_class.deleted == (true() if deleted else false()))
+        return query
 
-    class StatusColumn(grids.GridColumn):
-        def get_value(self, trans, grid, role):
-            if role.deleted:
-                return "deleted"
-            return ""
 
+class RoleListGrid(grids.GridData):
     class GroupsColumn(grids.GridColumn):
         def get_value(self, trans, grid, role):
             if role.groups:
                 return len(role.groups)
             return 0
 
     class UsersColumn(grids.GridColumn):
@@ -235,84 +173,61 @@
 
     # Grid definition
     title = "Roles"
     title_id = "roles-grid"
     model_class = model.Role
     default_sort_key = "name"
     columns = [
-        NameColumn(
-            "Name",
-            key="name",
-            link=(lambda item: dict(action="form/manage_users_and_groups_for_role", id=item.id, webapp="galaxy")),
-            model_class=model.Role,
-            attach_popup=True,
-            filterable="advanced",
-            target="top",
-        ),
-        DescriptionColumn(
-            "Description", key="description", model_class=model.Role, attach_popup=False, filterable="advanced"
-        ),
-        TypeColumn("Type", key="type", model_class=model.Role, attach_popup=False, filterable="advanced"),
-        GroupsColumn("Groups", attach_popup=False),
-        UsersColumn("Users", attach_popup=False),
-        StatusColumn("Status", attach_popup=False),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
+        grids.GridColumn("Name", key="name"),
+        grids.GridColumn("Description", key="description"),
+        grids.GridColumn("Type", key="type"),
+        GroupsColumn("Groups", key="groups"),
+        UsersColumn("Users", key="users"),
+        grids.GridColumn("Deleted", key="deleted", escape=False),
+        grids.GridColumn("Purged", key="purged", escape=False),
         grids.GridColumn("Last Updated", key="update_time"),
     ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-    global_actions = [grids.GridAction("Add new role", url_args=dict(action="form/create_role"))]
-    operations = [
-        grids.GridOperation(
-            "Edit Name/Description",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/rename_role"),
-        ),
-        grids.GridOperation(
-            "Edit Permissions",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/manage_users_and_groups_for_role", webapp="galaxy"),
-        ),
-        grids.GridOperation("Delete", condition=(lambda item: not item.deleted), allow_multiple=True),
-        grids.GridOperation("Undelete", condition=(lambda item: item.deleted), allow_multiple=True),
-        grids.GridOperation("Purge", condition=(lambda item: item.deleted), allow_multiple=True),
-    ]
-    standard_filters = [
-        grids.GridColumnFilter("Active", args=dict(deleted=False)),
-        grids.GridColumnFilter("Deleted", args=dict(deleted=True)),
-        grids.GridColumnFilter("All", args=dict(deleted="All")),
-    ]
-    num_rows_per_page = 50
-    use_paging = True
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter(model.Role.type != model.Role.types.PRIVATE)
-
 
-class GroupListGrid(grids.Grid):
-    class NameColumn(grids.TextColumn):
-        def get_value(self, trans, grid, group):
-            return escape(group.name)
+    def apply_query_filter(self, query, **kwargs):
+        INDEX_SEARCH_FILTERS = {
+            "description": "description",
+            "name": "name",
+            "is": "is",
+        }
+        deleted = False
+        query = query.filter(self.model_class.type != self.model_class.types.PRIVATE)
+        search_query = kwargs.get("search")
+        if search_query:
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "name":
+                        query = query.filter(text_column_filter(self.model_class.name, term))
+                    if key == "description":
+                        query = query.filter(text_column_filter(self.model_class.description, term))
+                    elif key == "is":
+                        if q == "deleted":
+                            deleted = True
+                elif isinstance(term, RawTextTerm):
+                    query = query.filter(
+                        raw_text_column_filter(
+                            [
+                                self.model_class.description,
+                                self.model_class.name,
+                            ],
+                            term,
+                        )
+                    )
+        query = query.filter(self.model_class.deleted == (true() if deleted else false()))
+        return query
 
-    class StatusColumn(grids.GridColumn):
-        def get_value(self, trans, grid, group):
-            if group.deleted:
-                return "deleted"
-            return ""
 
+class GroupListGrid(grids.GridData):
     class RolesColumn(grids.GridColumn):
         def get_value(self, trans, grid, group):
             if group.roles:
                 return len(group.roles)
             return 0
 
     class UsersColumn(grids.GridColumn):
@@ -323,234 +238,124 @@
 
     # Grid definition
     title = "Groups"
     title_id = "groups-grid"
     model_class = model.Group
     default_sort_key = "name"
     columns = [
-        NameColumn(
-            "Name",
-            key="name",
-            link=(lambda item: dict(action="form/manage_users_and_roles_for_group", id=item.id, webapp="galaxy")),
-            model_class=model.Group,
-            attach_popup=True,
-            filterable="advanced",
-        ),
-        UsersColumn("Users", attach_popup=False),
-        RolesColumn("Roles", attach_popup=False),
-        StatusColumn("Status", attach_popup=False),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.GridColumn("Last Updated", key="update_time", format=pretty_print_time_interval),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search", cols_to_filter=[columns[0]], key="free-text-search", visible=False, filterable="standard"
-        )
-    )
-    global_actions = [grids.GridAction("Add new group", url_args=dict(action="form/create_group"))]
-    operations = [
-        grids.GridOperation(
-            "Edit Name",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/rename_group"),
-        ),
-        grids.GridOperation(
-            "Edit Permissions",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/manage_users_and_roles_for_group", webapp="galaxy"),
-        ),
-        grids.GridOperation("Delete", condition=(lambda item: not item.deleted), allow_multiple=True),
-        grids.GridOperation("Undelete", condition=(lambda item: item.deleted), allow_multiple=True),
-        grids.GridOperation("Purge", condition=(lambda item: item.deleted), allow_multiple=True),
-    ]
-    standard_filters = [
-        grids.GridColumnFilter("Active", args=dict(deleted=False)),
-        grids.GridColumnFilter("Deleted", args=dict(deleted=True)),
-        grids.GridColumnFilter("All", args=dict(deleted="All")),
+        grids.GridColumn("Name", key="name"),
+        UsersColumn("Users", key="users"),
+        RolesColumn("Roles", key="roles"),
+        grids.GridColumn("Deleted", key="deleted", escape=False),
+        grids.GridColumn("Last Updated", key="update_time"),
     ]
-    num_rows_per_page = 50
-    use_paging = True
-
 
-class QuotaListGrid(grids.Grid):
-    class NameColumn(grids.TextColumn):
-        def get_value(self, trans, grid, quota):
-            return escape(quota.name)
+    def apply_query_filter(self, query, **kwargs):
+        INDEX_SEARCH_FILTERS = {
+            "name": "name",
+            "is": "is",
+        }
+        deleted = False
+        search_query = kwargs.get("search")
+        if search_query:
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "name":
+                        query = query.filter(text_column_filter(self.model_class.name, term))
+                    elif key == "is":
+                        if q == "deleted":
+                            deleted = True
+                elif isinstance(term, RawTextTerm):
+                    query = query.filter(
+                        raw_text_column_filter(
+                            [
+                                self.model_class.name,
+                            ],
+                            term,
+                        )
+                    )
+        query = query.filter(self.model_class.deleted == (true() if deleted else false()))
+        return query
 
-    class DescriptionColumn(grids.TextColumn):
-        def get_value(self, trans, grid, quota):
-            if quota.description:
-                return escape(quota.description)
-            return ""
 
-    class AmountColumn(grids.TextColumn):
+class QuotaListGrid(grids.GridData):
+    class AmountColumn(grids.GridColumn):
         def get_value(self, trans, grid, quota):
             return quota.operation + quota.display_amount
 
-    class StatusColumn(grids.GridColumn):
+    class DefaultTypeColumn(grids.GridColumn):
         def get_value(self, trans, grid, quota):
-            if quota.deleted:
-                return "deleted"
-            elif quota.default:
-                return f"<strong>default for {quota.default[0].type} users</strong>"
-            return ""
+            if quota.default:
+                return quota.default[0].type
+            return None
 
     class UsersColumn(grids.GridColumn):
         def get_value(self, trans, grid, quota):
             if quota.users:
                 return len(quota.users)
             return 0
 
     class GroupsColumn(grids.GridColumn):
         def get_value(self, trans, grid, quota):
             if quota.groups:
                 return len(quota.groups)
             return 0
 
-    class QuotaSourceLabelColumn(grids.TextColumn):
-        def get_value(self, trans, grid, quota):
-            raw_label = quota.quota_source_label
-            if raw_label is None:
-                rval = "<i>unlabelled object stores</i>"
-            else:
-                rval = raw_label
-            return rval
-
     # Grid definition
     title = "Quotas"
     model_class = model.Quota
     default_sort_key = "name"
     columns = [
-        NameColumn(
-            "Name",
-            key="name",
-            link=(lambda item: dict(action="form/edit_quota", id=item.id)),
-            model_class=model.Quota,
-            attach_popup=True,
-            filterable="advanced",
-        ),
-        DescriptionColumn(
-            "Description", key="description", model_class=model.Quota, attach_popup=False, filterable="advanced"
-        ),
-        AmountColumn("Amount", key="amount", model_class=model.Quota, attach_popup=False),
-        UsersColumn("Users", attach_popup=False),
-        GroupsColumn("Groups", attach_popup=False),
-        QuotaSourceLabelColumn("Source Label", key="quota_source_label", visible=False, filterable="advanced"),
-        StatusColumn("Status", attach_popup=False),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-    global_actions = [grids.GridAction("Add new quota", dict(action="form/create_quota"))]
-    operations = [
-        grids.GridOperation(
-            "Rename",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/rename_quota"),
-        ),
-        grids.GridOperation(
-            "Change amount",
-            condition=(lambda item: not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/edit_quota"),
-        ),
-        grids.GridOperation(
-            "Manage users and groups",
-            condition=(lambda item: not item.default and not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/manage_users_and_groups_for_quota"),
-        ),
-        grids.GridOperation(
-            "Set as different type of default",
-            condition=(lambda item: item.default),
-            allow_multiple=False,
-            url_args=dict(action="form/set_quota_default"),
-        ),
-        grids.GridOperation(
-            "Set as default",
-            condition=(lambda item: not item.default and not item.deleted),
-            allow_multiple=False,
-            url_args=dict(action="form/set_quota_default"),
-        ),
-        grids.GridOperation(
-            "Unset as default", condition=(lambda item: item.default and not item.deleted), allow_multiple=False
-        ),
-        grids.GridOperation(
-            "Delete", condition=(lambda item: not item.deleted and not item.default), allow_multiple=True
-        ),
-        grids.GridOperation("Undelete", condition=(lambda item: item.deleted), allow_multiple=True),
-        grids.GridOperation("Purge", condition=(lambda item: item.deleted), allow_multiple=True),
-    ]
-    standard_filters = [
-        grids.GridColumnFilter("Active", args=dict(deleted=False)),
-        grids.GridColumnFilter("Deleted", args=dict(deleted=True)),
-        grids.GridColumnFilter("Purged", args=dict(purged=True)),
-        grids.GridColumnFilter("All", args=dict(deleted="All")),
-    ]
-    num_rows_per_page = 50
-    use_paging = True
-
-
-class ToolVersionListGrid(grids.Grid):
-    class ToolIdColumn(grids.TextColumn):
-        def get_value(self, trans, grid, tool_version):
-            toolbox = trans.app.toolbox
-            if toolbox.has_tool(tool_version.tool_id, exact=True):
-                link = url_for(controller="tool_runner", tool_id=tool_version.tool_id)
-                link_str = f'<a target="_blank" href="{link}">'
-                return f'<div class="count-box state-color-ok">{link_str}{tool_version.tool_id}</a></div>'
-            return tool_version.tool_id
-
-    class ToolVersionsColumn(grids.TextColumn):
-        def get_value(self, trans, grid, tool_version):
-            tool_ids_str = ""
-            toolbox = trans.app.toolbox
-            tool = toolbox._tools_by_id.get(tool_version.tool_id)
-            if tool:
-                for tool_id in tool.lineage.tool_ids:
-                    if toolbox.has_tool(tool_id, exact=True):
-                        link = url_for(controller="tool_runner", tool_id=tool_id)
-                        link_str = f'<a target="_blank" href="{link}">'
-                        tool_ids_str += f'<div class="count-box state-color-ok">{link_str}{tool_id}</a></div><br/>'
-                    else:
-                        tool_ids_str += f"{tool_version.tool_id}<br/>"
-            else:
-                tool_ids_str += f"{tool_version.tool_id}<br/>"
-            return tool_ids_str
-
-    # Grid definition
-    title = "Tool versions"
-    model_class = install_model.ToolVersion
-    default_sort_key = "tool_id"
-    columns = [
-        ToolIdColumn("Tool id", key="tool_id", attach_popup=False),
-        ToolVersionsColumn("Version lineage by tool id (parent/child ordered)"),
+        grids.GridColumn("Name", key="name"),
+        grids.GridColumn("Description", key="description"),
+        AmountColumn("Amount", key="amount", model_class=model.Quota),
+        UsersColumn("Users", key="users"),
+        GroupsColumn("Groups", key="groups"),
+        grids.GridColumn("Source", key="quota_source_label", escape=False),
+        DefaultTypeColumn("Type", key="default_type"),
+        grids.GridColumn("Deleted", key="deleted", escape=False),
+        grids.GridColumn("Updated", key="update_time"),
     ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search tool id", cols_to_filter=[columns[0]], key="free-text-search", visible=False, filterable="standard"
-        )
-    )
-    num_rows_per_page = 50
-    use_paging = True
 
-    def build_initial_query(self, trans, **kwd):
-        return trans.install_model.context.query(self.model_class)
+    def apply_query_filter(self, query, **kwargs):
+        INDEX_SEARCH_FILTERS = {
+            "name": "name",
+            "description": "description",
+            "is": "is",
+        }
+        deleted = False
+        search_query = kwargs.get("search")
+        if search_query:
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "name":
+                        query = query.filter(text_column_filter(self.model_class.name, term))
+                    if key == "description":
+                        query = query.filter(text_column_filter(self.model_class.description, term))
+                    elif key == "is":
+                        if q == "deleted":
+                            deleted = True
+                elif isinstance(term, RawTextTerm):
+                    query = query.filter(
+                        raw_text_column_filter(
+                            [
+                                self.model_class.name,
+                                self.model_class.description,
+                            ],
+                            term,
+                        )
+                    )
+        query = query.filter(self.model_class.deleted == (true() if deleted else false()))
+        return query
 
 
 # TODO: Convert admin UI to use the API and drop this.
 class DatatypesEntryT(TypedDict):
     status: str
     keys: list
     data: list
@@ -558,36 +363,14 @@
 
 
 class AdminGalaxy(controller.JSAppLauncher):
     user_list_grid = UserListGrid()
     role_list_grid = RoleListGrid()
     group_list_grid = GroupListGrid()
     quota_list_grid = QuotaListGrid()
-    tool_version_list_grid = ToolVersionListGrid()
-    delete_operation = grids.GridOperation(
-        "Delete", condition=(lambda item: not item.deleted and not item.purged), allow_multiple=True
-    )
-    undelete_operation = grids.GridOperation(
-        "Undelete", condition=(lambda item: item.deleted and not item.purged), allow_multiple=True
-    )
-    purge_operation = grids.GridOperation(
-        "Purge", condition=(lambda item: item.deleted and not item.purged), allow_multiple=True
-    )
-    impersonate_operation = grids.GridOperation(
-        "Impersonate",
-        url_args=dict(controller="admin", action="impersonate"),
-        condition=(lambda item: not item.deleted and not item.purged),
-        allow_multiple=False,
-    )
-    activate_operation = grids.GridOperation(
-        "Activate User", condition=(lambda item: not item.active), allow_multiple=False
-    )
-    resend_activation_email = grids.GridOperation(
-        "Resend Activation Email", condition=(lambda item: not item.active), allow_multiple=False
-    )
 
     def __init__(self, app: StructuredApp):
         super().__init__(app)
         self.quota_manager: QuotaManager = QuotaManager(app)
 
     @web.expose
     @web.json
@@ -626,88 +409,19 @@
             keys |= set(attrib.keys())
         return {"keys": list(keys), "data": datatypes, "message": message, "status": status}
 
     @web.expose
     @web.json
     @web.require_admin
     def users_list(self, trans, **kwd):
-        message = kwd.get("message", "")
-        status = kwd.get("status", "")
-        if "operation" in kwd:
-            id = kwd.get("id")
-            if not id:
-                message, status = (f"Invalid user id ({str(id)}) received.", "error")
-            ids = util.listify(id)
-            operation = kwd["operation"].lower()
-            if operation == "delete":
-                message, status = self._delete_user(trans, ids)
-            elif operation == "undelete":
-                message, status = self._undelete_user(trans, ids)
-            elif operation == "purge":
-                message, status = self._purge_user(trans, ids)
-            elif operation == "recalculate disk usage":
-                message, status = self._recalculate_user(trans, id)
-            elif operation == "generate new api key":
-                message, status = self._new_user_apikey(trans, id)
-            elif operation == "activate user":
-                message, status = self._activate_user(trans, id)
-            elif operation == "resend activation email":
-                message, status = self._resend_activation_email(trans, id)
-        if message and status:
-            kwd["message"] = util.sanitize_text(message)
-            kwd["status"] = status
-        if trans.app.config.allow_user_deletion:
-            if self.delete_operation not in self.user_list_grid.operations:
-                self.user_list_grid.operations.append(self.delete_operation)
-            if self.undelete_operation not in self.user_list_grid.operations:
-                self.user_list_grid.operations.append(self.undelete_operation)
-            if self.purge_operation not in self.user_list_grid.operations:
-                self.user_list_grid.operations.append(self.purge_operation)
-        if trans.app.config.allow_user_impersonation:
-            if self.impersonate_operation not in self.user_list_grid.operations:
-                self.user_list_grid.operations.append(self.impersonate_operation)
-        if trans.app.config.user_activation_on:
-            if self.activate_operation not in self.user_list_grid.operations:
-                self.user_list_grid.operations.append(self.activate_operation)
-                self.user_list_grid.operations.append(self.resend_activation_email)
         return self.user_list_grid(trans, **kwd)
 
     @web.legacy_expose_api
     @web.require_admin
     def quotas_list(self, trans, payload=None, **kwargs):
-        message = kwargs.get("message", "")
-        status = kwargs.get("status", "")
-        if "operation" in kwargs:
-            id = kwargs.get("id")
-            if not id:
-                return self.message_exception(trans, f"Invalid quota id ({str(id)}) received.")
-            quotas = []
-            for quota_id in util.listify(id):
-                try:
-                    quotas.append(get_quota(trans, quota_id))
-                except MessageException as e:
-                    return self.message_exception(trans, util.unicodify(e))
-            operation = kwargs.pop("operation").lower()
-            try:
-                if operation == "delete":
-                    message = self.quota_manager.delete_quota(quotas)
-                elif operation == "undelete":
-                    message = self.quota_manager.undelete_quota(quotas)
-                elif operation == "purge":
-                    message = self.quota_manager.purge_quota(quotas)
-                elif operation == "unset as default":
-                    message = self.quota_manager.unset_quota_default(quotas[0])
-            except ActionInputError as e:
-                message, status = (e.err_msg, "error")
-        if message:
-            kwargs["message"] = util.sanitize_text(message)
-            kwargs["status"] = status or "done"
-        labels = trans.app.object_store.get_quota_source_map().get_quota_source_labels()
-        if labels:
-            self.quota_list_grid.columns[5].visible = True
         return self.quota_list_grid(trans, **kwargs)
 
     @web.legacy_expose_api
     @web.require_admin
     def create_quota(self, trans, payload=None, **kwd):
         if trans.request.method == "GET":
             all_users = []
@@ -779,15 +493,15 @@
     def rename_quota(self, trans, payload=None, **kwd):
         id = kwd.get("id")
         if not id:
             return self.message_exception(trans, "No quota id received for renaming.")
         quota = get_quota(trans, id)
         if trans.request.method == "GET":
             return {
-                "title": "Change quota name and description for '%s'" % util.sanitize_text(quota.name),
+                "title": f"Change quota name and description for '{quota.name}'",
                 "inputs": [
                     {"name": "name", "label": "Name", "value": quota.name},
                     {"name": "description", "label": "Description", "value": quota.description},
                 ],
             }
         else:
             try:
@@ -848,15 +562,15 @@
     def edit_quota(self, trans, payload=None, **kwd):
         id = kwd.get("id")
         if not id:
             return self.message_exception(trans, "No quota id received for renaming.")
         quota = get_quota(trans, id)
         if trans.request.method == "GET":
             return {
-                "title": "Edit quota size for '%s'" % util.sanitize_text(quota.name),
+                "title": f"Edit quota size for '{quota.name}'",
                 "inputs": [
                     {
                         "name": "amount",
                         "label": "Amount",
                         "value": quota.display_amount,
                         "help": 'Examples: "10000MB", "99 gb", "0.2T", "unlimited"',
                     },
@@ -883,15 +597,15 @@
         quota = get_quota(trans, id)
         if trans.request.method == "GET":
             default_value = quota.default[0].type if quota.default else "no"
             default_options = [("No", "no")]
             for typ in trans.app.model.DefaultQuotaAssociation.types.__members__.values():
                 default_options.append((f"Yes, {typ}", typ))
             return {
-                "title": "Set quota default for '%s'" % util.sanitize_text(quota.name),
+                "title": f"Set quota default for '{quota.name}'",
                 "inputs": [
                     {
                         "name": "default",
                         "label": "Is this quota a default for a class of users (if yes, what type)?",
                         "options": default_options,
                         "value": default_value,
                         "help": "Warning: Any users or groups associated with this quota will be disassociated.",
@@ -906,16 +620,15 @@
 
     @web.expose
     @web.require_admin
     def impersonate(self, trans, **kwd):
         if not trans.app.config.allow_user_impersonation:
             return trans.show_error_message("User impersonation is not enabled in this instance of Galaxy.")
         user = None
-        user_id = kwd.get("id", None)
-        if user_id is not None:
+        if (user_id := kwd.get("id", None)) is not None:
             try:
                 user = trans.sa_session.query(trans.app.model.User).get(trans.security.decode_id(user_id))
                 if user:
                     trans.handle_user_logout()
                     trans.handle_user_login(user)
                     return trans.show_message(
                         f"You are now logged in as {user.email}, <a target=\"_top\" href=\"{url_for(controller='root')}\">return to the home page</a>",
@@ -923,40 +636,18 @@
                     )
             except Exception:
                 log.exception("Error fetching user for impersonation")
         return trans.response.send_redirect(
             web.url_for(controller="admin", action="users", message="Invalid user selected", status="error")
         )
 
-    @web.legacy_expose_api
-    @web.require_admin
-    def tool_versions_list(self, trans, **kwd):
-        return self.tool_version_list_grid(trans, **kwd)
-
     @web.expose
     @web.json
     @web.require_admin
     def roles_list(self, trans, **kwargs):
-        message = kwargs.get("message")
-        status = kwargs.get("status")
-        if "operation" in kwargs:
-            id = kwargs.get("id", None)
-            if not id:
-                message, status = (f"Invalid role id ({str(id)}) received.", "error")
-            ids = util.listify(id)
-            operation = kwargs["operation"].lower().replace("+", " ")
-            if operation == "delete":
-                message, status = self._delete_role(trans, ids)
-            elif operation == "undelete":
-                message, status = self._undelete_role(trans, ids)
-            elif operation == "purge":
-                message, status = self._purge_role(trans, ids)
-        if message and status:
-            kwargs["message"] = util.sanitize_text(message)
-            kwargs["status"] = status
         return self.role_list_grid(trans, **kwargs)
 
     @web.legacy_expose_api
     @web.require_admin
     def create_role(self, trans, payload=None, **kwd):
         if trans.request.method == "GET":
             all_users = []
@@ -1050,15 +741,15 @@
     def rename_role(self, trans, payload=None, **kwd):
         id = kwd.get("id")
         if not id:
             return self.message_exception(trans, "No role id received for renaming.")
         role = get_role(trans, id)
         if trans.request.method == "GET":
             return {
-                "title": "Change role name and description for '%s'" % util.sanitize_text(role.name),
+                "title": f"Change role name and description for '{role.name}'",
                 "inputs": [
                     {"name": "name", "label": "Name", "value": role.name},
                     {"name": "description", "label": "Description", "value": role.description},
                 ],
             }
         else:
             old_name = role.name
@@ -1146,109 +837,29 @@
                         trans.sa_session.commit()
             trans.app.security_agent.set_entity_role_associations(roles=[role], users=in_users, groups=in_groups)
             trans.sa_session.refresh(role)
             return {
                 "message": f"Role '{role.name}' has been updated with {len(in_users)} associated users and {len(in_groups)} associated groups."
             }
 
-    def _delete_role(self, trans, ids):
-        message = "Deleted %d roles: " % len(ids)
-        for role_id in ids:
-            role = get_role(trans, role_id)
-            role.deleted = True
-            trans.sa_session.add(role)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            message += f" {role.name} "
-        return (message, "done")
-
-    def _undelete_role(self, trans, ids):
-        count = 0
-        undeleted_roles = ""
-        for role_id in ids:
-            role = get_role(trans, role_id)
-            if not role.deleted:
-                return (f"Role '{role.name}' has not been deleted, so it cannot be undeleted.", "error")
-            role.deleted = False
-            trans.sa_session.add(role)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            count += 1
-            undeleted_roles += f" {role.name}"
-        return ("Undeleted %d roles: %s" % (count, undeleted_roles), "done")
-
-    def _purge_role(self, trans, ids):
-        # This method should only be called for a Role that has previously been deleted.
-        # Purging a deleted Role deletes all of the following from the database:
-        # - UserRoleAssociations where role_id == Role.id
-        # - DefaultUserPermissions where role_id == Role.id
-        # - DefaultHistoryPermissions where role_id == Role.id
-        # - GroupRoleAssociations where role_id == Role.id
-        # - DatasetPermissionss where role_id == Role.id
-        message = "Purged %d roles: " % len(ids)
-        for role_id in ids:
-            role = get_role(trans, role_id)
-            if not role.deleted:
-                return (f"Role '{role.name}' has not been deleted, so it cannot be purged.", "error")
-            # Delete UserRoleAssociations
-            for ura in role.users:
-                user = trans.sa_session.query(trans.app.model.User).get(ura.user_id)
-                # Delete DefaultUserPermissions for associated users
-                for dup in user.default_permissions:
-                    if role == dup.role:
-                        trans.sa_session.delete(dup)
-                # Delete DefaultHistoryPermissions for associated users
-                for history in user.histories:
-                    for dhp in history.default_permissions:
-                        if role == dhp.role:
-                            trans.sa_session.delete(dhp)
-                trans.sa_session.delete(ura)
-            # Delete GroupRoleAssociations
-            for gra in role.groups:
-                trans.sa_session.delete(gra)
-            # Delete DatasetPermissionss
-            for dp in role.dataset_actions:
-                trans.sa_session.delete(dp)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            message += f" {role.name} "
-        return (message, "done")
-
     @web.legacy_expose_api
     @web.require_admin
     def groups_list(self, trans, **kwargs):
-        message = kwargs.get("message")
-        status = kwargs.get("status")
-        if "operation" in kwargs:
-            id = kwargs.get("id")
-            if not id:
-                return self.message_exception(trans, f"Invalid group id ({str(id)}) received.")
-            ids = util.listify(id)
-            operation = kwargs["operation"].lower().replace("+", " ")
-            if operation == "delete":
-                message, status = self._delete_group(trans, ids)
-            elif operation == "undelete":
-                message, status = self._undelete_group(trans, ids)
-            elif operation == "purge":
-                message, status = self._purge_group(trans, ids)
-        if message and status:
-            kwargs["message"] = util.sanitize_text(message)
-            kwargs["status"] = status
         return self.group_list_grid(trans, **kwargs)
 
     @web.legacy_expose_api
     @web.require_admin
     def rename_group(self, trans, payload=None, **kwd):
         id = kwd.get("id")
         if not id:
             return self.message_exception(trans, "No group id received for renaming.")
         group = get_group(trans, id)
         if trans.request.method == "GET":
             return {
-                "title": "Change group name for '%s'" % util.sanitize_text(group.name),
+                "title": f"Change group name for '{group.name}'",
                 "inputs": [{"name": "name", "label": "Name", "value": group.name}],
             }
         else:
             old_name = group.name
             new_name = util.restore_text(payload.get("name"))
             if not new_name:
                 return self.message_exception(trans, "Enter a valid group name.")
@@ -1411,57 +1022,14 @@
                 )
                 if auto_create_checked:
                     message += (
                         "One of the roles associated with this group is the newly created role with the same name."
                     )
                 return {"message": message}
 
-    def _delete_group(self, trans, ids):
-        message = "Deleted %d groups: " % len(ids)
-        for group_id in ids:
-            group = get_group(trans, group_id)
-            group.deleted = True
-            trans.sa_session.add(group)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            message += f" {group.name} "
-        return (message, "done")
-
-    def _undelete_group(self, trans, ids):
-        count = 0
-        undeleted_groups = ""
-        for group_id in ids:
-            group = get_group(trans, group_id)
-            if not group.deleted:
-                return (f"Group '{group.name}' has not been deleted, so it cannot be undeleted.", "error")
-            group.deleted = False
-            trans.sa_session.add(group)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            count += 1
-            undeleted_groups += f" {group.name}"
-        return ("Undeleted %d groups: %s" % (count, undeleted_groups), "done")
-
-    def _purge_group(self, trans, ids):
-        message = "Purged %d groups: " % len(ids)
-        for group_id in ids:
-            group = get_group(trans, group_id)
-            if not group.deleted:
-                return (f"Group '{group.name}' has not been deleted, so it cannot be purged.", "error")
-            # Delete UserGroupAssociations
-            for uga in group.users:
-                trans.sa_session.delete(uga)
-            # Delete GroupRoleAssociations
-            for gra in group.roles:
-                trans.sa_session.delete(gra)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-            message += f" {group.name} "
-        return (message, "done")
-
     @web.expose
     @web.require_admin
     def create_new_user(self, trans, **kwd):
         return trans.response.send_redirect(web.url_for(controller="user", action="create", cntrller="admin"))
 
     @web.legacy_expose_api
     @web.require_admin
@@ -1488,97 +1056,14 @@
                     trans.sa_session.add(user)
                     with transaction(trans.sa_session):
                         trans.sa_session.commit()
                 return {"message": "Passwords reset for %d user(s)." % len(users)}
         else:
             return self.message_exception(trans, "Please specify user ids.")
 
-    def _delete_user(self, trans, ids):
-        message = "Deleted %d users: " % len(ids)
-        for user_id in ids:
-            user = get_user(trans, user_id)
-            # Actually do the delete
-            self.user_manager.delete(user)
-            # Accumulate messages for the return message
-            message += f" {user.email} "
-        return (message, "done")
-
-    def _undelete_user(self, trans, ids):
-        count = 0
-        undeleted_users = ""
-        for user_id in ids:
-            user = get_user(trans, user_id)
-            # Actually do the undelete
-            self.user_manager.undelete(user)
-            # Count and accumulate messages to return to the admin panel
-            count += 1
-            undeleted_users += f" {user.email}"
-        message = "Undeleted %d users: %s" % (count, undeleted_users)
-        return (message, "done")
-
-    def _purge_user(self, trans, ids):
-        # This method should only be called for a User that has previously been deleted.
-        # We keep the User in the database ( marked as purged ), and stuff associated
-        # with the user's private role in case we want the ability to unpurge the user
-        # some time in the future.
-        # Purging a deleted User deletes all of the following:
-        # - History where user_id = User.id
-        #    - HistoryDatasetAssociation where history_id = History.id
-        # - UserGroupAssociation where user_id == User.id
-        # - UserRoleAssociation where user_id == User.id EXCEPT FOR THE PRIVATE ROLE
-        # - UserAddress where user_id == User.id
-        # Purging Histories and Datasets must be handled via the cleanup_datasets.py script
-        message = "Purged %d users: " % len(ids)
-        for user_id in ids:
-            user = get_user(trans, user_id)
-            self.user_manager.purge(user)
-            message += f"\t{user.email}\n "
-        return (message, "done")
-
-    def _recalculate_user(self, trans, user_id):
-        user = trans.sa_session.query(trans.model.User).get(trans.security.decode_id(user_id))
-        if not user:
-            return (f"User not found for id ({sanitize_text(str(user_id))})", "error")
-        current = user.get_disk_usage()
-        user.calculate_and_set_disk_usage()
-        new = user.get_disk_usage()
-        if new in (current, None):
-            message = f"Usage is unchanged at {nice_size(current)}."
-        else:
-            message = f"Usage has changed by {nice_size(new - current)} to {nice_size(new)}."
-        return (message, "done")
-
-    def _new_user_apikey(self, trans, user_id):
-        user = trans.sa_session.query(trans.model.User).get(trans.security.decode_id(user_id))
-        if not user:
-            return (f"User not found for id ({sanitize_text(str(user_id))})", "error")
-        new_key = trans.app.model.APIKeys(
-            user_id=trans.security.decode_id(user_id), key=trans.app.security.get_new_guid()
-        )
-        trans.sa_session.add(new_key)
-        with transaction(trans.sa_session):
-            trans.sa_session.commit()
-        return (f"New key '{new_key.key}' generated for requested user '{user.email}'.", "done")
-
-    def _activate_user(self, trans, user_id):
-        user = trans.sa_session.query(trans.model.User).get(trans.security.decode_id(user_id))
-        if not user:
-            return (f"User not found for id ({sanitize_text(str(user_id))})", "error")
-        self.user_manager.activate(user)
-        return (f"Activated user: {user.email}.", "done")
-
-    def _resend_activation_email(self, trans, user_id):
-        user = trans.sa_session.query(trans.model.User).get(trans.security.decode_id(user_id))
-        if not user:
-            return (f"User not found for id ({sanitize_text(str(user_id))})", "error")
-        if self.user_manager.send_activation_email(trans, user.email, user.username):
-            return (f"Activation email has been sent to user: {user.email}.", "done")
-        else:
-            return (f"Unable to send activation email to user: {user.email}.", "error")
-
     @web.legacy_expose_api
     @web.require_admin
     def manage_roles_and_groups_for_user(self, trans, payload=None, **kwd):
         user_id = kwd.get("id")
         if not user_id:
             return self.message_exception(trans, f"Invalid user id ({str(user_id)}) received")
         user = get_user(trans, user_id)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/admin_toolshed.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/admin_toolshed.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/async.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/async.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Upload class
+Controller to handle communication of tools of type data_source_async
 """
 
 import logging
 from urllib.parse import urlencode
 
 import requests
 
@@ -35,51 +35,81 @@
         tool_id = str(tool_id)
 
         # redirect to main when getting no parameters
         if not kwd:
             return trans.response.send_redirect("/index")
 
         params = Params(kwd, sanitize=False)
-        STATUS = params.STATUS
-        URL = params.URL
         data_id = params.data_id
 
         log.debug(f"async dataid -> {data_id}")
         trans.log_event(f"Async dataid -> {str(data_id)}")
 
         # initialize the tool
         toolbox = self.get_toolbox()
         tool = toolbox.get_tool(tool_id)
         if not tool:
             return f"Tool with id {tool_id} not found"
 
-        #
-        # we have an incoming data_id
-        #
         if data_id:
-            if not URL:
-                return f"No URL parameter was submitted for data {data_id}"
+            #
+            # we have an incoming data_id
+            #
             data = trans.sa_session.query(trans.model.HistoryDatasetAssociation).get(data_id)
 
             if not data:
                 return f"Data {data_id} does not exist or has already been deleted"
+            if data.state in data.dataset.terminal_states:
+                log.debug(f"Tool {tool.id}: execution stopped as data {data_id} has entered terminal state prematurely")
+                trans.log_event(
+                    f"Tool {tool.id}: execution stopped as data {data_id} has entered terminal state prematurely"
+                )
+                return f"Data {data_id} has finished processing before job could be completed"
+
+            # map params from the tool's <request_param_translation> section;
+            # ignore any other params that may have been passed by the remote
+            # server with the exception of STATUS and URL;
+            # if name, info, dbkey and data_type are not handled via incoming params,
+            # use the metadata from the already existing dataset;
+            # preserve original params under nested dict
+            params_dict = dict(
+                STATUS=params.STATUS,
+                URL=params.URL,
+                name=data.name,
+                info=data.info,
+                dbkey=data.dbkey,
+                data_type=data.ext,
+                incoming_request_params=params.__dict__.copy(),
+            )
+            if tool.input_translator:
+                tool.input_translator.translate(params)
+                tool_declared_params = {
+                    translator.galaxy_name for translator in tool.input_translator.param_trans_dict.values()
+                }
+                for param in params:
+                    if param in tool_declared_params or not tool.wants_params_cleaned:
+                        params_dict[param] = params.get(param, None)
+            params = params_dict
+
+            if not params.get("URL"):
+                return f"No URL parameter was submitted for data {data_id}"
+
+            STATUS = params.get("STATUS")
 
             if STATUS == "OK":
                 key = hmac_new(trans.app.config.tool_secret, "%d:%d" % (data.id, data.history_id))
                 if key != data_secret:
                     return f"You do not have permission to alter data {data_id}."
+                if not params.get("GALAXY_URL"):
+                    # provide a fallback for GALAXY_URL
+                    params["GALAXY_URL"] = f"{trans.request.url_path}/async/{tool_id}/{data.id}/{key}"
                 # push the job into the queue
                 data.state = data.blurb = data.states.RUNNING
                 log.debug(f"executing tool {tool.id}")
                 trans.log_event(f"Async executing tool {tool.id}", tool_id=tool.id)
-                galaxy_url = f"{trans.request.url_path}/async/{tool_id}/{data.id}/{key}"
-                galaxy_url = params.get("GALAXY_URL", galaxy_url)
-                params = dict(
-                    URL=URL, GALAXY_URL=galaxy_url, name=data.name, info=data.info, dbkey=data.dbkey, data_type=data.ext
-                )
 
                 # Assume there is exactly one output file possible
                 TOOL_OUTPUT_TYPE = None
                 for key, obj in tool.outputs.items():
                     try:
                         TOOL_OUTPUT_TYPE = obj.format
                         params[key] = data.id
@@ -100,17 +130,29 @@
                 data.info = f"Error -> {STATUS}"
 
             with transaction(trans.sa_session):
                 trans.sa_session.commit()
 
             return f"Data {data_id} with status {STATUS} received. OK"
         else:
-            #
             # no data_id must be parameter submission
             #
+            # create new dataset, put it into running state,
+            # send request for data to remote server and see if the response
+            # ends in ok;
+            # the request that's getting sent goes to the URL found in
+            # params.URL or, in its absence, to the one found as the value of
+            # the "action" attribute of the data source tool's "inputs" tag.
+            # Included in the request are the parameters:
+            # - data_id, which indicates to the remote server that Galaxy is
+            #   ready to accept data
+            # - GALAXY_URL, which takes the form:
+            #   {base_url}/async/{tool_id}/{data_id}/{data_secret}, and which
+            #   when used by the remote server to send a data download link,
+            #   will trigger the if branch above.
             GALAXY_TYPE = None
             if params.data_type:
                 GALAXY_TYPE = params.data_type
             elif params.galaxyFileFormat == "wig":  # this is an undocumented legacy special case
                 GALAXY_TYPE = "wig"
             elif params.GALAXY_TYPE:
                 GALAXY_TYPE = params.GALAXY_TYPE
@@ -167,15 +209,15 @@
             try:
                 key = hmac_new(trans.app.config.tool_secret, "%d:%d" % (data.id, data.history_id))
                 galaxy_url = f"{trans.request.url_path}/async/{tool_id}/{data.id}/{key}"
                 params.update({"GALAXY_URL": galaxy_url})
                 params.update({"data_id": data.id})
 
                 # Use provided URL or fallback to tool action
-                url = URL or tool.action
+                url = params.URL or tool.action
                 # Does url already have query params?
                 if "?" in url:
                     url_join_char = "&"
                 else:
                     url_join_char = "?"
                 url = f"{url}{url_join_char}{urlencode(params.flatten())}"
                 log.debug(f"connecting to -> {url}")
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/authnz.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/authnz.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 OAuth 2.0 and OpenID Connect Authentication and Authorization Controller.
 """
 
-
 import datetime
 import json
 import logging
 
 import jwt
 
 from galaxy import (
@@ -199,21 +198,20 @@
         idp_provider = provider if provider else trans.get_cookie(name=PROVIDER_COOKIE_NAME)
         if idp_provider:
             return trans.response.send_redirect(url_for(controller="authnz", action="logout", provider=idp_provider))
 
     @web.expose
     @web.json
     def get_cilogon_idps(self, trans, **kwargs):
-        allowed_idps = trans.app.authnz_manager.get_allowed_idps()
         try:
             cilogon_idps = json.loads(url_get("https://cilogon.org/idplist/", params=dict(kwargs)))
         except Exception as e:
             raise Exception(f"Invalid server response. {str(e)}.")
 
-        if allowed_idps:
+        if allowed_idps := trans.app.authnz_manager.get_allowed_idps():
             validated_idps = list(filter(lambda idp: idp["EntityID"] in allowed_idps, cilogon_idps))
 
             if not (len(validated_idps) == len(allowed_idps)):
                 validated_entity_ids = [entity["EntityID"] for entity in validated_idps]
 
                 for idp in allowed_idps:
                     if idp not in validated_entity_ids:
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/data_manager.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/data_manager.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/dataset.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,16 +133,15 @@
         self, trans, dataset_id=None, preview=False, filename=None, to_ext=None, offset=None, ck_size=None, **kwd
     ):
         data = self._check_dataset(trans, dataset_id)
         if not isinstance(data, trans.app.model.DatasetInstance):
             return data
         if "hdca" in kwd:
             raise RequestParameterInvalidException("Invalid request parameter 'hdca' encountered.")
-        hdca_id = kwd.get("hdca_id", None)
-        if hdca_id:
+        if hdca_id := kwd.get("hdca_id", None):
             hdca = self.app.dataset_collection_manager.get_dataset_collection_instance(trans, "history", hdca_id)
             del kwd["hdca_id"]
             kwd["hdca"] = hdca
         # Ensure offset is an integer before passing through to datatypes.
         if offset:
             offset = int(offset)
         # Ensure ck_size is an integer before passing through to datatypes.
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/forms.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/forms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,118 +1,112 @@
 import copy
 import csv
 import logging
 import re
 
-from markupsafe import escape
-
-from galaxy import (
-    model,
-    util,
+from sqlalchemy import (
+    false,
+    true,
 )
+
+from galaxy import model
+from galaxy.managers.forms import get_form
 from galaxy.model.base import transaction
-from galaxy.web.framework.helpers import (
-    grids,
-    iff,
-    time_ago,
+from galaxy.model.index_filter_util import (
+    raw_text_column_filter,
+    text_column_filter,
+)
+from galaxy.util.search import (
+    FilteredTerm,
+    parse_filters_structured,
+    RawTextTerm,
 )
+from galaxy.web.framework.helpers import grids
 from galaxy.webapps.base.controller import (
     BaseUIController,
     web,
 )
 
 log = logging.getLogger(__name__)
 
 VALID_FIELDNAME_RE = re.compile(r"^[a-zA-Z0-9\_]+$")
 
 
-class FormsGrid(grids.Grid):
+class FormsGrid(grids.GridData):
     # Custom column types
-    class NameColumn(grids.TextColumn):
+    class NameColumn(grids.GridColumn):
         def get_value(self, trans, grid, form):
-            return escape(form.latest_form.name)
+            return form.latest_form.name
 
-    class DescriptionColumn(grids.TextColumn):
+    class DescriptionColumn(grids.GridColumn):
         def get_value(self, trans, grid, form):
-            return escape(form.latest_form.desc)
+            return form.latest_form.desc
 
-    class TypeColumn(grids.TextColumn):
+    class TypeColumn(grids.GridColumn):
         def get_value(self, trans, grid, form):
             return form.latest_form.type
 
-    class StatusColumn(grids.GridColumn):
-        def get_value(self, trans, grid, user):
-            if user.deleted:
-                return "deleted"
-            return "active"
-
     # Grid definition
     title = "Forms"
     model_class = model.FormDefinitionCurrent
-    default_sort_key = "-update_time"
-    num_rows_per_page = 50
-    use_paging = True
-    default_filter = dict(deleted="False")
+    default_sort_key = "update_time"
     columns = [
         NameColumn(
             "Name",
             key="name",
             model_class=model.FormDefinition,
-            link=(lambda item: iff(item.deleted, None, dict(controller="admin", action="form/edit_form", id=item.id))),
-            attach_popup=True,
-            filterable="advanced",
         ),
-        DescriptionColumn("Description", key="desc", model_class=model.FormDefinition, filterable="advanced"),
-        TypeColumn("Type"),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        StatusColumn("Status"),
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-    operations = [
-        grids.GridOperation("Delete", allow_multiple=True, condition=(lambda item: not item.deleted)),
-        grids.GridOperation("Undelete", condition=(lambda item: item.deleted)),
+        DescriptionColumn("Description", key="desc", model_class=model.FormDefinition),
+        TypeColumn("Type", key="type", model_class=model.FormDefinition),
+        grids.GridColumn("Last Updated", key="update_time"),
+        grids.GridColumn("Deleted", key="deleted", escape=False),
     ]
-    global_actions = [grids.GridAction("Create new form", dict(controller="admin", action="form/create_form"))]
 
-    def build_initial_query(self, trans, **kwargs):
-        return trans.sa_session.query(self.model_class).join(
-            model.FormDefinition, self.model_class.latest_form_id == model.FormDefinition.id
-        )
+    def apply_query_filter(self, query, **kwargs):
+        INDEX_SEARCH_FILTERS = {
+            "name": "name",
+            "description": "description",
+            "is": "is",
+        }
+        deleted = False
+        query = query.join(model.FormDefinition, self.model_class.latest_form_id == model.FormDefinition.id)
+        search_query = kwargs.get("search")
+        if search_query:
+            parsed_search = parse_filters_structured(search_query, INDEX_SEARCH_FILTERS)
+            for term in parsed_search.terms:
+                if isinstance(term, FilteredTerm):
+                    key = term.filter
+                    q = term.text
+                    if key == "name":
+                        query = query.filter(text_column_filter(model.FormDefinition.name, term))
+                    elif key == "description":
+                        query = query.filter(text_column_filter(model.FormDefinition.desc, term))
+                    elif key == "is":
+                        if q == "deleted":
+                            deleted = True
+                elif isinstance(term, RawTextTerm):
+                    query = query.filter(
+                        raw_text_column_filter(
+                            [
+                                model.FormDefinition.name,
+                                model.FormDefinition.desc,
+                            ],
+                            term,
+                        )
+                    )
+        query = query.filter(self.model_class.deleted == (true() if deleted else false()))
+        return query
 
 
 class Forms(BaseUIController):
     forms_grid = FormsGrid()
 
     @web.legacy_expose_api
     @web.require_admin
     def forms_list(self, trans, payload=None, **kwd):
-        message = kwd.get("message", "")
-        status = kwd.get("status", "")
-        if "operation" in kwd:
-            id = kwd.get("id")
-            if not id:
-                return self.message_exception(trans, f"Invalid form id ({str(id)}) received.")
-            ids = util.listify(id)
-            operation = kwd["operation"].lower()
-            if operation == "delete":
-                message, status = self._delete_form(trans, ids)
-            elif operation == "undelete":
-                message, status = self._undelete_form(trans, ids)
-        if message and status:
-            kwd["message"] = util.sanitize_text(message)
-            kwd["status"] = status
         return self.forms_grid(trans, **kwd)
 
     @web.legacy_expose_api
     @web.require_admin
     def create_form(self, trans, payload=None, **kwd):
         if trans.request.method == "GET":
             fd_types = sorted(trans.app.model.FormDefinition.types.__members__.items())
@@ -157,15 +151,15 @@
                         payload[f"{prefix}required"] = row[5].lower() == "true"
                     index = index + 1
             new_form, message = self.save_form_definition(trans, None, payload)
             if new_form is None:
                 return self.message_exception(trans, message)
             imported = (" with %i imported fields" % index) if index > 0 else ""
             message = f"The form '{payload.get('name')}' has been created{imported}."
-            return {"message": util.sanitize_text(message)}
+            return {"message": message}
 
     @web.legacy_expose_api
     @web.require_admin
     def edit_form(self, trans, payload=None, **kwd):
         id = kwd.get("id")
         if not id:
             return self.message_exception(trans, "No form id received for editing.")
@@ -190,15 +184,15 @@
                     "name": "selectlist",
                     "label": "Options",
                     "help": "*Only for fields which allow multiple selections, provide comma-separated values.",
                 },
                 {"name": "required", "label": "Required", "type": "boolean", "value": False},
             ]
             form_dict = {
-                "title": "Edit form for '%s'" % (util.sanitize_text(latest_form.name)),
+                "title": f"Edit form for '{latest_form.name}'",
                 "inputs": [
                     {"name": "name", "label": "Name", "value": latest_form.name},
                     {"name": "desc", "label": "Description", "value": latest_form.desc},
                     {
                         "name": "type",
                         "type": "select",
                         "options": [(ft[1], ft[1]) for ft in fd_types],
@@ -225,15 +219,15 @@
                 field_cache.append(new_field)
             return form_dict
         else:
             new_form, message = self.save_form_definition(trans, id, payload)
             if new_form is None:
                 return self.message_exception(trans, message)
             message = f"The form '{payload.get('name')}' has been updated."
-            return {"message": util.sanitize_text(message)}
+            return {"message": message}
 
     def get_current_form(self, trans, payload=None, **kwd):
         """
         This method gets all the unsaved user-entered form details and returns a
         dictionary containing the name, desc, type, layout & fields of the form
         """
         name = payload.get("name")
@@ -298,40 +292,7 @@
         # create corresponding row in the form_definition_current table
         form_definition.form_definition_current = form_definition_current
         form_definition_current.latest_form = form_definition
         trans.sa_session.add(form_definition_current)
         with transaction(trans.sa_session):
             trans.sa_session.commit()
         return form_definition, None
-
-    @web.expose
-    @web.require_admin
-    def _delete_form(self, trans, ids):
-        for form_id in ids:
-            form = get_form(trans, form_id)
-            form.deleted = True
-            trans.sa_session.add(form)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-        return ("Deleted %i form(s)." % len(ids), "done")
-
-    @web.expose
-    @web.require_admin
-    def _undelete_form(self, trans, ids):
-        for form_id in ids:
-            form = get_form(trans, form_id)
-            form.deleted = False
-            trans.sa_session.add(form)
-            with transaction(trans.sa_session):
-                trans.sa_session.commit()
-        return ("Undeleted %i form(s)." % len(ids), "done")
-
-
-# ---- Utility methods -------------------------------------------------------
-
-
-def get_form(trans, form_id):
-    """Get a FormDefinition from the database by id."""
-    form = trans.sa_session.query(trans.app.model.FormDefinitionCurrent).get(trans.security.decode_id(form_id))
-    if not form:
-        return trans.show_error_message(f"Form not found for id ({str(form_id)})")
-    return form
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/history.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/histories.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,785 +1,829 @@
+import glob
 import logging
+import os
+import shutil
+from pathlib import Path
+from tempfile import (
+    NamedTemporaryFile,
+    SpooledTemporaryFile,
+)
+from typing import (
+    cast,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
-from dateutil.parser import isoparse
-from markupsafe import escape
 from sqlalchemy import (
     false,
     select,
     true,
 )
-from sqlalchemy.orm import undefer
+from sqlalchemy.orm import Session
 
 from galaxy import (
-    exceptions,
+    exceptions as glx_exceptions,
     model,
-    web,
 )
-from galaxy.managers import histories
-from galaxy.managers.sharable import SlugBuilder
-from galaxy.model import Role
-from galaxy.model.base import transaction
-from galaxy.model.item_attrs import (
-    UsesAnnotations,
-    UsesItemRatings,
+from galaxy.celery.tasks import (
+    import_model_store,
+    prepare_history_download,
+    write_history_to,
+)
+from galaxy.files.uris import validate_uri_access
+from galaxy.managers.citations import CitationsManager
+from galaxy.managers.context import ProvidesHistoryContext
+from galaxy.managers.histories import (
+    HistoryDeserializer,
+    HistoryExportManager,
+    HistoryFilters,
+    HistoryManager,
+    HistorySerializer,
 )
-from galaxy.structured_app import StructuredApp
-from galaxy.util import (
-    listify,
-    sanitize_text,
-    string_as_bool,
-    unicodify,
+from galaxy.managers.notification import NotificationManager
+from galaxy.managers.users import UserManager
+from galaxy.model import HistoryDatasetAssociation
+from galaxy.model.base import transaction
+from galaxy.model.store import payload_to_source_uri
+from galaxy.schema import (
+    FilterQueryParams,
+    SerializationParams,
 )
-from galaxy.web import (
-    expose_api_anonymous,
-    url_for,
+from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.history import HistoryIndexQueryPayload
+from galaxy.schema.schema import (
+    AnyArchivedHistoryView,
+    AnyHistoryView,
+    ArchiveHistoryRequestPayload,
+    AsyncFile,
+    AsyncTaskResultSummary,
+    CreateHistoryFromStore,
+    CreateHistoryPayload,
+    CustomBuildsMetadataResponse,
+    ExportHistoryArchivePayload,
+    HistoryArchiveExportResult,
+    HistoryImportArchiveSourceType,
+    JobExportHistoryArchiveModel,
+    JobIdResponse,
+    JobImportHistoryResponse,
+    LabelValuePair,
+    ShareHistoryWithStatus,
+    ShareWithPayload,
+    StoreExportPayload,
+    WriteStoreToPayload,
 )
-from galaxy.web.framework.helpers import (
-    grids,
-    iff,
-    time_ago,
+from galaxy.schema.tasks import (
+    GenerateHistoryDownload,
+    ImportModelStoreTaskRequest,
+    WriteHistoryTo,
 )
-from galaxy.webapps.base.controller import (
-    BaseUIController,
-    ERROR,
-    INFO,
-    SharableMixin,
-    SUCCESS,
-    WARNING,
+from galaxy.schema.types import LatestLiteral
+from galaxy.security.idencoding import IdEncodingHelper
+from galaxy.short_term_storage import ShortTermStorageAllocator
+from galaxy.util import restore_text
+from galaxy.webapps.galaxy.services.base import (
+    async_task_summary,
+    ConsumesModelStores,
+    model_store_storage_target,
+    ServesExportStores,
+    ServiceBase,
 )
-from ..api import depends
+from galaxy.webapps.galaxy.services.sharable import ShareableService
 
 log = logging.getLogger(__name__)
 
+DEFAULT_ORDER_BY = "create_time-dsc"
 
-class NameColumn(grids.TextColumn):
-    def get_value(self, trans, grid, history):
-        return escape(history.get_display_name())
-
-
-class HistoryListGrid(grids.Grid):
-    # Custom column types
-    class ItemCountColumn(grids.GridColumn):
-        def get_value(self, trans, grid, history):
-            return str(history.hid_counter - 1)
-
-    class HistoryListNameColumn(NameColumn):
-        def get_link(self, trans, grid, history):
-            link = None
-            if not history.deleted:
-                link = dict(operation="Switch", id=history.id, use_panels=grid.use_panels, async_compatible=True)
-            return link
-
-    class StatusColumn(grids.GridColumn):
-        def get_accepted_filters(self):
-            """Returns a list of accepted filters for this column."""
-            accepted_filter_labels_and_vals = {
-                "active": "active",
-                "deleted": "deleted",
-                "archived": "archived",
-                "all": "all",
-            }
-            accepted_filters = []
-            for label, val in accepted_filter_labels_and_vals.items():
-                args = {self.key: val}
-                accepted_filters.append(grids.GridColumnFilter(label, args))
-            return accepted_filters
-
-        def filter(self, trans, user, query, column_filter):
-            """Modify query to filter self.model_class by state."""
-            if column_filter == "all":
-                return query
-            elif column_filter == "active":
-                return query.filter(self.model_class.deleted == false(), self.model_class.archived == false())
-            elif column_filter == "deleted":
-                return query.filter(self.model_class.deleted == true())
-            elif column_filter == "archived":
-                return query.filter(self.model_class.archived == true())
-
-        def get_value(self, trans, grid, history):
-            if history == trans.history:
-                return "<strong>current history</strong>"
-            if history.purged:
-                return "deleted permanently"
-            elif history.deleted:
-                return "deleted"
-            elif history.archived:
-                return "archived"
-            return ""
-
-        def sort(self, trans, query, ascending, column_name=None):
-            if ascending:
-                query = query.order_by(self.model_class.table.c.purged.asc(), self.model_class.update_time.desc())
-            else:
-                query = query.order_by(self.model_class.table.c.purged.desc(), self.model_class.update_time.desc())
-            return query
 
-    def build_initial_query(self, trans, **kwargs):
-        # Override to preload sharing information used when fetching data for grid.
-        query = super().build_initial_query(trans, **kwargs)
-        query = query.options(undefer("users_shared_with_count"))
-        return query
-
-    # Grid definition
-    title = "Saved Histories"
-    model_class = model.History
-    default_sort_key = "-update_time"
-    columns = [
-        HistoryListNameColumn("Name", key="name", attach_popup=True, filterable="advanced"),
-        ItemCountColumn("Items", key="item_count", sortable=False),
-        grids.GridColumn("Datasets", key="datasets_by_state", sortable=False, nowrap=True, delayed=True),
-        grids.IndividualTagsColumn(
-            "Tags",
-            key="tags",
-            model_tag_association_class=model.HistoryTagAssociation,
-            filterable="advanced",
-            grid_name="HistoryListGrid",
-        ),
-        grids.SharingStatusColumn(
-            "Sharing", key="sharing", filterable="advanced", sortable=False, use_shared_with_count=True
-        ),
-        grids.GridColumn("Size on Disk", key="disk_size", sortable=False, delayed=True),
-        grids.GridColumn("Created", key="create_time", format=time_ago),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        StatusColumn("Status", key="status", filterable="advanced"),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "search history names and tags",
-            cols_to_filter=[columns[0], columns[3]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
+class ShareableHistoryService(ShareableService):
+    share_with_status_cls = ShareHistoryWithStatus
+
+    def share_with_users(self, trans, id: DecodedDatabaseIdField, payload: ShareWithPayload) -> ShareHistoryWithStatus:
+        return cast(ShareHistoryWithStatus, super().share_with_users(trans, id, payload))
+
+
+class HistoriesService(ServiceBase, ConsumesModelStores, ServesExportStores):
+    """Common interface/service logic for interactions with histories in the context of the API.
+
+    Provides the logic of the actions invoked by API controllers and uses type definitions
+    and pydantic models to declare its parameters and return types.
+    """
+
+    def __init__(
+        self,
+        security: IdEncodingHelper,
+        manager: HistoryManager,
+        user_manager: UserManager,
+        serializer: HistorySerializer,
+        deserializer: HistoryDeserializer,
+        citations_manager: CitationsManager,
+        history_export_manager: HistoryExportManager,
+        filters: HistoryFilters,
+        short_term_storage_allocator: ShortTermStorageAllocator,
+        notification_manager: NotificationManager,
+    ):
+        super().__init__(security)
+        self.manager = manager
+        self.user_manager = user_manager
+        self.serializer = serializer
+        self.deserializer = deserializer
+        self.citations_manager = citations_manager
+        self.history_export_manager = history_export_manager
+        self.filters = filters
+        self.shareable_service = ShareableHistoryService(self.manager, self.serializer, notification_manager)
+        self.short_term_storage_allocator = short_term_storage_allocator
+
+    def index(
+        self,
+        trans: ProvidesHistoryContext,
+        serialization_params: SerializationParams,
+        filter_query_params: FilterQueryParams,
+        deleted_only: Optional[bool] = False,
+        all_histories: Optional[bool] = False,
+    ):
+        """
+        Return a collection of histories for the current user. Additional filters can be applied.
+
+        :type   deleted_only: optional boolean
+        :param  deleted_only: if True, show only deleted histories, if False, non-deleted
+
+        .. note:: Anonymous users are allowed to get their current history
+        """
+        # bail early with current history if user is anonymous
+        current_user = self.user_manager.current_user(trans)
+        if self.user_manager.is_anonymous(current_user):
+            current_history = self.manager.get_current(trans)
+            if not current_history:
+                return []
+            # note: ignores filters, limit, offset
+            return [self._serialize_history(trans, current_history, serialization_params)]
+
+        filter_params = self.filters.build_filter_params(filter_query_params)
+        filters = []
+        # support the old default of not-returning/filtering-out deleted_only histories
+        filters += self._get_deleted_filter(deleted_only, filter_params)
+
+        # if parameter 'all_histories' is true, throw exception if not admin
+        # else add current user filter to query (default behaviour)
+        if all_histories:
+            if not trans.user_is_admin:
+                message = "Only admins can query all histories"
+                raise glx_exceptions.AdminRequiredException(message)
+        else:
+            filters += [model.History.user == current_user]
+        # exclude archived histories
+        filters += [model.History.archived == false()]
+        # and apply any other filters
+        filters += self.filters.parse_filters(filter_params)
+        order_by = self._build_order_by(filter_query_params.order)
+
+        histories = self.manager.list(
+            filters=filters, order_by=order_by, limit=filter_query_params.limit, offset=filter_query_params.offset
         )
-    )
-    global_actions = [grids.GridAction("Import history", dict(controller="", action="histories/import"))]
-    operations = [
-        grids.GridOperation(
-            "Switch", allow_multiple=False, condition=(lambda item: not item.deleted), async_compatible=True
-        ),
-        grids.GridOperation("View", allow_multiple=False, url_args=dict(controller="", action="histories/view")),
-        grids.GridOperation(
-            "Share or Publish",
-            allow_multiple=False,
-            condition=(lambda item: not item.deleted),
-            url_args=dict(controller="", action="histories/sharing"),
-        ),
-        grids.GridOperation(
-            "Change Permissions",
-            allow_multiple=False,
-            condition=(lambda item: not item.deleted),
-            url_args=dict(controller="", action="histories/permissions"),
-        ),
-        grids.GridOperation(
-            "Copy", allow_multiple=False, condition=(lambda item: not item.deleted), async_compatible=False
-        ),
-        grids.GridOperation(
-            "Rename",
-            condition=(lambda item: not item.deleted),
-            url_args=dict(controller="", action="histories/rename"),
-            target="top",
-        ),
-        grids.GridOperation("Delete", condition=(lambda item: not item.deleted), async_compatible=True),
-        grids.GridOperation(
-            "Delete Permanently",
-            condition=(lambda item: not item.purged),
-            confirm="History contents will be removed from disk, this cannot be undone.  Continue?",
-            async_compatible=True,
-        ),
-        grids.GridOperation(
-            "Undelete", condition=(lambda item: item.deleted and not item.purged), async_compatible=True
-        ),
-    ]
-    standard_filters = [
-        grids.GridColumnFilter("Active", args=dict(deleted=False)),
-        grids.GridColumnFilter("Deleted", args=dict(deleted=True)),
-        grids.GridColumnFilter("All", args=dict(deleted="All")),
-    ]
-    default_filter = dict(name="All", status="active", tags="All", sharing="All")
-    num_rows_per_page = 15
-    use_paging = True
-    info_text = "Histories that have been deleted for more than a time period specified by the Galaxy administrator(s) may be permanently deleted."
-
-    def get_current_item(self, trans, **kwargs):
-        return trans.get_history()
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter_by(user=trans.user, importing=False)
-
-
-class SharedHistoryListGrid(grids.Grid):
-    # Custom column types
-    class DatasetsByStateColumn(grids.GridColumn):
-        def get_value(self, trans, grid, history):
-            rval = ""
-            for state in ("ok", "running", "queued", "error"):
-                total = sum(1 for d in history.active_datasets if d.state == state)
-                if total:
-                    rval += f'<div class="count-box state-color-{state}">{total}</div>'
-            return rval
-
-    class SharedByColumn(grids.GridColumn):
-        def get_value(self, trans, grid, history):
-            return escape(history.user.email)
-
-    # Grid definition
-    title = "Histories shared with you by others"
-    model_class = model.History
-    default_sort_key = "-update_time"
-    columns = [
-        grids.GridColumn("Name", key="name", attach_popup=True),
-        DatasetsByStateColumn("Datasets", sortable=False),
-        grids.GridColumn("Created", key="create_time", format=time_ago),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        SharedByColumn("Shared by", key="user_id"),
-    ]
-    operations = [
-        grids.GridOperation("View", allow_multiple=False, url_args=dict(controller="", action="histories/view")),
-        grids.GridOperation("Copy", allow_multiple=False),
-        grids.GridOperation("Unshare", allow_multiple=False),
-    ]
-
-    def build_initial_query(self, trans, **kwargs):
-        return trans.sa_session.query(self.model_class).join(self.model_class.users_shared_with)
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter(model.HistoryUserShareAssociation.user == trans.user)
-
-
-class HistoryController(BaseUIController, SharableMixin, UsesAnnotations, UsesItemRatings):
-    history_manager: histories.HistoryManager = depends(histories.HistoryManager)
-    history_serializer: histories.HistorySerializer = depends(histories.HistorySerializer)
-    slug_builder: SlugBuilder = depends(SlugBuilder)
-
-    def __init__(self, app: StructuredApp):
-        super().__init__(app)
-
-    @web.expose
-    def index(self, trans):
-        return ""
-
-    @web.expose
-    def list_as_xml(self, trans):
-        """XML history list for functional tests"""
-        trans.response.set_content_type("text/xml")
-        return trans.fill_template("/history/list_as_xml.mako")
-
-    # ......................................................................... lists
-    stored_list_grid = HistoryListGrid()
-    shared_list_grid = SharedHistoryListGrid()
-
-    @web.legacy_expose_api
-    @web.require_login("work with multiple histories")
-    def list(self, trans, **kwargs):
-        """List all available histories"""
-        current_history = trans.get_history()
-        message = kwargs.get("message")
-        status = kwargs.get("status")
-        if "operation" in kwargs:
-            operation = kwargs["operation"].lower()
-            history_ids = listify(kwargs.get("id", []))
-            # Display no message by default
-            status, message = None, None
-            # Load the histories and ensure they all belong to the current user
-            histories = []
-            for history_id in history_ids:
-                history = self.history_manager.get_owned(
-                    self.decode_id(history_id), trans.user, current_history=trans.history
-                )
-                if history:
-                    # Ensure history is owned by current user
-                    if history.user_id is not None and trans.user:
-                        assert trans.user.id == history.user_id, "History does not belong to current user"
-                    histories.append(history)
-                else:
-                    log.warning("Invalid history id '%r' passed to list", history_id)
-            if histories:
-                if operation == "switch":
-                    status, message = self._list_switch(trans, histories)
-                    # Take action to update UI to reflect history switch. If
-                    # grid is using panels, it is standalone and hence a redirect
-                    # to root is needed; if grid is not using panels, it is nested
-                    # in the main Galaxy UI and refreshing the history frame
-                    # is sufficient.
-                    use_panels = kwargs.get("use_panels", False) == "True"
-                    if use_panels:
-                        return trans.response.send_redirect(url_for("/"))
-                    else:
-                        kwargs["refresh_frames"] = ["history"]
-                elif operation in ("delete", "delete permanently"):
-                    status, message = self._list_delete(trans, histories, purge=(operation == "delete permanently"))
-                    if current_history in histories:
-                        # Deleted the current history, so a new, empty history was
-                        # created automatically, and we need to refresh the history frame
-                        kwargs["refresh_frames"] = ["history"]
-                elif operation == "undelete":
-                    status, message = self._list_undelete(trans, histories)
-
-                with transaction(trans.sa_session):
-                    trans.sa_session.commit()
-        # Render the list view
-        if message and status:
-            kwargs["message"] = sanitize_text(message)
-            kwargs["status"] = status
-        return self.stored_list_grid(trans, **kwargs)
-
-    def _list_delete(self, trans, histories, purge=False):
-        """Delete histories"""
-        n_deleted = 0
-        deleted_current = False
-        message_parts = []
-        status = SUCCESS
-        current_history = trans.get_history()
-        for history in histories:
-            try:
-                if history.users_shared_with:
-                    raise exceptions.ObjectAttributeInvalidException(
-                        f"History ({history.name}) has been shared with others, unshare it before deleting it."
-                    )
-                if purge:
-                    self.history_manager.purge(history, user=trans.user)
-                else:
-                    self.history_manager.delete(history)
-                if history == current_history:
-                    deleted_current = True
-            except Exception as e:
-                message_parts.append(unicodify(e))
-                status = ERROR
-            else:
-                trans.log_event(f"History ({history.name}) marked as deleted")
-                n_deleted += 1
 
-        if n_deleted:
-            part = "Deleted %d %s" % (n_deleted, iff(n_deleted != 1, "histories", "history"))
-            if purge and trans.app.config.allow_user_dataset_purge:
-                part += f" and removed {iff(n_deleted != 1, 'their', 'its')} dataset{iff(n_deleted != 1, 's', '')} from disk"
-            elif purge:
-                part += " but the datasets were not removed from disk because that feature is not enabled in this Galaxy instance"
-            message_parts.append(f"{part}.  ")
-        if deleted_current:
-            # if this history is the current history for this session,
-            # - attempt to find the most recently used, undeleted history and switch to it.
-            # - If no suitable recent history is found, create a new one and switch
-            # note: this needs to come after commits above or will use an empty history that was deleted above
-            not_deleted_or_purged = [model.History.deleted == false(), model.History.purged == false()]
-            most_recent_history = self.history_manager.most_recent(user=trans.user, filters=not_deleted_or_purged)
-            if most_recent_history:
-                self.history_manager.set_current(trans, most_recent_history)
-            else:
-                trans.get_or_create_default_history()
-            message_parts.append("Your active history was deleted, a new empty history is now active.  ")
-            status = INFO
-        return (status, " ".join(message_parts))
-
-    def _list_undelete(self, trans, histories):
-        """Undelete histories"""
-        n_undeleted = 0
-        n_already_purged = 0
-        for history in histories:
-            if history.purged:
-                n_already_purged += 1
-            if history.deleted:
-                history.deleted = False
-                if not history.default_permissions:
-                    # For backward compatibility - for a while we were deleting all DefaultHistoryPermissions on
-                    # the history when we deleted the history.  We are no longer doing this.
-                    # Need to add default DefaultHistoryPermissions in case they were deleted when the history was deleted
-                    default_action = trans.app.security_agent.permitted_actions.DATASET_MANAGE_PERMISSIONS
-                    private_user_role = trans.app.security_agent.get_private_user_role(history.user)
-                    default_permissions = {}
-                    default_permissions[default_action] = [private_user_role]
-                    trans.app.security_agent.history_set_default_permissions(history, default_permissions)
-                n_undeleted += 1
-                trans.log_event("History (%s) %d marked as undeleted" % (history.name, history.id))
-        status = SUCCESS
-        message_parts = []
-        if n_undeleted:
-            message_parts.append("Undeleted %d %s.  " % (n_undeleted, iff(n_undeleted != 1, "histories", "history")))
-        if n_already_purged:
-            message_parts.append("%d histories have already been purged and cannot be undeleted." % n_already_purged)
-            status = WARNING
-        return status, "".join(message_parts)
-
-    def _list_switch(self, trans, histories):
-        """Switch to a new different history"""
-        new_history = histories[0]
-        galaxy_session = trans.get_galaxy_session()
+        rval = [
+            self._serialize_history(trans, history, serialization_params, default_view="summary")
+            for history in histories
+        ]
+        return rval
+
+    def _get_deleted_filter(self, deleted: Optional[bool], filter_params: List[Tuple[str, str, str]]):
+        # TODO: this should all be removed (along with the default) in v2
+        # support the old default of not-returning/filtering-out deleted histories
         try:
-            stmt = (
-                select(trans.app.model.GalaxySessionToHistoryAssociation)
-                .filter_by(session_id=galaxy_session.id, history_id=new_history.id)
-                .limit(1)
+            # the consumer must explicitly ask for both deleted and non-deleted
+            #   but pull it from the parsed params (as the filter system will error on None)
+            deleted_filter_index = filter_params.index(("deleted", "eq", "None"))
+            filter_params.pop(deleted_filter_index)
+            return []
+        except ValueError:
+            pass
+
+        # the deleted string bool was also used as an 'include deleted' flag
+        if deleted is True:
+            return [model.History.deleted == true()]
+
+        # the third option not handled here is 'return only deleted'
+        #   if this is passed in (in the form below), simply return and let the filter system handle it
+        if ("deleted", "eq", "True") in filter_params:
+            return []
+
+        # otherwise, do the default filter of removing the deleted histories
+        return [model.History.deleted == false()]
+
+    def index_query(
+        self,
+        trans,
+        payload: HistoryIndexQueryPayload,
+        serialization_params: SerializationParams,
+        include_total_count: bool = False,
+    ) -> Tuple[List[AnyHistoryView], int]:
+        """Return a list of History accessible by the user
+
+        :rtype:     list
+        :returns:   dictionaries containing History details
+        """
+        entries, total_matches = self.manager.index_query(trans, payload, include_total_count)
+        return (
+            [self._serialize_history(trans, entry, serialization_params, default_view="summary") for entry in entries],
+            total_matches,
+        )
+
+    def create(
+        self,
+        trans: ProvidesHistoryContext,
+        payload: CreateHistoryPayload,
+        serialization_params: SerializationParams,
+    ):
+        """Create a new history from scratch, by copying an existing one or by importing
+        from URL or File depending on the provided parameters in the payload.
+        """
+        copy_this_history_id = payload.history_id
+        if trans.anonymous and not copy_this_history_id:  # Copying/Importing histories is allowed for anonymous users
+            raise glx_exceptions.AuthenticationRequired("You need to be logged in to create histories.")
+        if trans.user and trans.user.bootstrap_admin_user:
+            raise glx_exceptions.RealUserRequiredException("Only real users can create histories.")
+        hist_name = None
+        if payload.name is not None:
+            hist_name = restore_text(payload.name)
+
+        if payload.archive_source is not None or hasattr(payload.archive_file, "file"):
+            archive_source = payload.archive_source
+            archive_file = payload.archive_file
+            if archive_source:
+                archive_type = payload.archive_type
+            elif archive_file is not None and hasattr(archive_file, "file"):
+                archive_source = archive_file.file.name
+                archive_type = HistoryImportArchiveSourceType.file
+                if isinstance(archive_file.file, SpooledTemporaryFile):
+                    archive_source = self._save_upload_file_tmp(archive_file)
+            else:
+                raise glx_exceptions.MessageException("Please provide a url or file.")
+            if archive_type == HistoryImportArchiveSourceType.url:
+                assert archive_source
+                validate_uri_access(archive_source, trans.user_is_admin, trans.app.config.fetch_url_allowlist_ips)
+            job = self.manager.queue_history_import(trans, archive_type=archive_type, archive_source=archive_source)
+            job_dict = job.to_dict()
+            job_dict["message"] = (
+                f"Importing history from source '{archive_source}'. This history will be visible when the import is complete."
+            )
+            return JobImportHistoryResponse(**job_dict)
+
+        new_history = None
+        # if a history id was passed, copy that history
+        if copy_this_history_id:
+            original_history = self.manager.get_accessible(
+                copy_this_history_id, trans.user, current_history=trans.history
             )
-            association = trans.sa_session.scalars(stmt).first()
-        except Exception:
-            association = None
-        new_history.add_galaxy_session(galaxy_session, association=association)
+            hist_name = hist_name or (f"Copy of '{original_history.name}'")
+            new_history = original_history.copy(
+                name=hist_name, target_user=trans.user, all_datasets=payload.all_datasets
+            )
+
+        # otherwise, create a new empty history
+        else:
+            new_history = self.manager.create(user=trans.user, name=hist_name)
+
+        trans.app.security_agent.history_set_default_permissions(new_history)
         trans.sa_session.add(new_history)
         with transaction(trans.sa_session):
             trans.sa_session.commit()
-        trans.set_history(new_history)
-        # No message
-        return None, None
-
-    @web.expose
-    @web.json
-    @web.require_login("work with shared histories")
-    def list_shared(self, trans, **kwargs):
-        """List histories shared with current user by others"""
-        status = message = None
-        if "operation" in kwargs:
-            ids = listify(kwargs.get("id", []))
-            operation = kwargs["operation"].lower()
-            if operation == "unshare":
-                if not ids:
-                    message = "Select a history to unshare"
-                    status = "error"
-                for id in ids:
-                    # No need to check security, association below won't yield a
-                    # hit if this user isn't having the history shared with her.
-                    history = self.history_manager.by_id(self.decode_id(id))
-                    # Current user is the user with which the histories were shared
-                    stmt = select(trans.app.model.HistoryUserShareAssociation).filter_by(
-                        user=trans.user, history=history
-                    )
-                    association = trans.sa_session.execute(select(stmt)).scalar_one()
-                    trans.sa_session.delete(association)
-                    with transaction(trans.sa_session):
-                        trans.sa_session.commit()
-                message = "Unshared %d shared histories" % len(ids)
-                status = "done"
-        # Render the list view
-        return self.shared_list_grid(trans, status=status, message=message, **kwargs)
-
-    @web.expose
-    def as_xml(self, trans, id=None, show_deleted=None, show_hidden=None):
-        """
-        Return a history in xml format.
+
+        # an anonymous user can only have one history
+        if self.user_manager.is_anonymous(trans.user):
+            self.manager.set_current(trans, new_history)
+
+        return self._serialize_history(trans, new_history, serialization_params)
+
+    def create_from_store(
+        self,
+        trans,
+        payload: CreateHistoryFromStore,
+        serialization_params: SerializationParams,
+    ) -> AnyHistoryView:
+        self._ensure_can_create_history(trans)
+        object_tracker = self.create_objects_from_store(
+            trans,
+            payload,
+        )
+        return self._serialize_history(trans, object_tracker.new_history, serialization_params)
+
+    def create_from_store_async(
+        self,
+        trans,
+        payload: CreateHistoryFromStore,
+    ) -> AsyncTaskResultSummary:
+        self._ensure_can_create_history(trans)
+        source_uri = payload_to_source_uri(payload)
+        request = ImportModelStoreTaskRequest(
+            user=trans.async_request_user,
+            source_uri=source_uri,
+            for_library=False,
+            model_store_format=payload.model_store_format,
+        )
+        result = import_model_store.delay(request=request, task_user_id=getattr(trans.user, "id", None))
+        return async_task_summary(result)
+
+    def _ensure_can_create_history(self, trans):
+        if trans.anonymous:
+            raise glx_exceptions.AuthenticationRequired("You need to be logged in to create histories.")
+        if trans.user and trans.user.bootstrap_admin_user:
+            raise glx_exceptions.RealUserRequiredException("Only real users can create histories.")
+
+    def _save_upload_file_tmp(self, upload_file) -> str:
+        try:
+            suffix = Path(upload_file.filename).suffix
+            with NamedTemporaryFile(delete=False, suffix=suffix) as tmp:
+                shutil.copyfileobj(upload_file.file, tmp)
+                tmp_path = Path(tmp.name)
+        finally:
+            upload_file.file.close()
+        return str(tmp_path)
+
+    def show(
+        self,
+        trans: ProvidesHistoryContext,
+        serialization_params: SerializationParams,
+        history_id: Optional[DecodedDatabaseIdField] = None,
+    ):
         """
-        if trans.app.config.require_login and not trans.user:
-            return trans.fill_template("/no_access.mako", message="Please log in to access Galaxy histories.")
+        Returns detailed information about the history with the given encoded `id`. If no `id` is
+        provided, then the most recently used history will be returned.
 
-        if id:
-            history = self.history_manager.get_accessible(self.decode_id(id), trans.user, current_history=trans.history)
-        else:
-            history = trans.get_history(most_recent=True, create=True)
+        :param  history_id:      the encoded id of the history to query or None to use the most recently used
+
+        :param  serialization_params:   contains the optional `view`, `keys` and `default_view` for serialization
 
-        trans.response.set_content_type("text/xml")
-        return trans.fill_template_mako(
-            "history/as_xml.mako",
-            history=history,
-            show_deleted=string_as_bool(show_deleted),
-            show_hidden=string_as_bool(show_hidden),
-        )
-
-    @expose_api_anonymous
-    def view(self, trans, id=None, show_deleted=False, show_hidden=False, use_panels=True):
-        """
-        View a history. If a history is importable, then it is viewable by any user.
-        """
-        show_deleted = string_as_bool(show_deleted)
-        show_hidden = string_as_bool(show_hidden)
-        use_panels = string_as_bool(use_panels)
-
-        history_dictionary = {}
-        user_is_owner = False
-        if id:
-            history_to_view = self.history_manager.get_accessible(
-                self.decode_id(id), trans.user, current_history=trans.history
+        :returns:   detailed history information
+        """
+        if history_id is None:  # By default display the most recent history
+            history = self.manager.most_recent(
+                trans.user, filters=(model.History.deleted == false()), current_history=trans.history
             )
-            user_is_owner = history_to_view.user == trans.user
-            history_is_current = history_to_view == trans.history
         else:
-            history_to_view = trans.history
-            if not history_to_view:
-                raise exceptions.RequestParameterMissingException(
-                    "No 'id' parameter provided for history, and user does not have a current history."
-                )
-            user_is_owner = True
-            history_is_current = True
+            history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        return self._serialize_history(trans, history, serialization_params)
 
-        # include all datasets: hidden, deleted, and purged
-        history_dictionary = self.history_serializer.serialize_to_view(
-            history_to_view, view="dev-detailed", user=trans.user, trans=trans
-        )
-
-        return {
-            "history": history_dictionary,
-            "user_is_owner": user_is_owner,
-            "history_is_current": history_is_current,
-            "show_deleted": show_deleted,
-            "show_hidden": show_hidden,
-            "use_panels": use_panels,
-            "allow_user_dataset_purge": trans.app.config.allow_user_dataset_purge,
-        }
-
-    @web.expose
-    def display_by_username_and_slug(self, trans, username, slug, **kwargs):
-        """
-        Display history based on a username and slug.
-        """
-        # Get history.
-        session = trans.sa_session
-
-        user = session.scalars(select(model.User).filter_by(username=username).limit(1)).first()
-        history = session.scalars(select(model.History).filter_by(user=user, slug=slug, deleted=False).limit(1)).first()
-
-        if history is None:
-            raise web.httpexceptions.HTTPNotFound()
-
-        # Security check raises error if user cannot access history.
-        self.history_manager.error_unless_accessible(history, trans.user, current_history=trans.history)
-
-        # Encode history id.
-        history_id = trans.security.encode_id(history.id)
-
-        # Redirect to client.
-        return trans.response.send_redirect(
-            web.url_for(
-                controller="published",
-                action="history",
-                id=history_id,
-            )
+    def prepare_download(
+        self, trans: ProvidesHistoryContext, history_id: DecodedDatabaseIdField, payload: StoreExportPayload
+    ) -> AsyncFile:
+        history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        short_term_storage_target = model_store_storage_target(
+            self.short_term_storage_allocator,
+            history.name,
+            payload.model_store_format,
         )
+        export_association = self.history_export_manager.create_export_association(history.id)
+        request = GenerateHistoryDownload(
+            history_id=history.id,
+            short_term_storage_request_id=short_term_storage_target.request_id,
+            duration=short_term_storage_target.duration,
+            user=trans.async_request_user,
+            export_association_id=export_association.id,
+            **payload.dict(),
+        )
+        result = prepare_history_download.delay(request=request, task_user_id=getattr(trans.user, "id", None))
+        task_summary = async_task_summary(result)
+        export_association.task_uuid = task_summary.id
+        with transaction(trans.sa_session):
+            trans.sa_session.commit()
+        return AsyncFile(storage_request_id=short_term_storage_target.request_id, task=task_summary)
 
-    @web.legacy_expose_api
-    @web.require_login("changing default permissions")
-    def permissions(self, trans, payload=None, **kwd):
-        """
-        Sets the permissions on a history.
-        """
-        history_id = kwd.get("id")
-        if not history_id:
-            return self.message_exception(trans, f"Invalid history id ({str(history_id)}) received")
-        history = self.history_manager.get_owned(self.decode_id(history_id), trans.user, current_history=trans.history)
-        if trans.request.method == "GET":
-            inputs = []
-            all_roles = trans.user.all_roles()
-            current_actions = history.default_permissions
-            for action_key, action in trans.app.model.Dataset.permitted_actions.items():
-                in_roles = set()
-                for a in current_actions:
-                    if a.action == action.action:
-                        in_roles.add(a.role)
-                inputs.append(
-                    {
-                        "type": "select",
-                        "multiple": True,
-                        "optional": True,
-                        "individual": True,
-                        "name": action_key,
-                        "label": action.action,
-                        "help": action.description,
-                        "options": [(role.name, trans.security.encode_id(role.id)) for role in set(all_roles)],
-                        "value": [trans.security.encode_id(role.id) for role in in_roles],
-                    }
-                )
-            return {"title": "Change default dataset permissions for history '%s'" % history.name, "inputs": inputs}
+    def write_store(
+        self, trans: ProvidesHistoryContext, history_id: DecodedDatabaseIdField, payload: WriteStoreToPayload
+    ) -> AsyncTaskResultSummary:
+        history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        export_association = self.history_export_manager.create_export_association(history.id)
+        request = WriteHistoryTo(
+            user=trans.async_request_user,
+            history_id=history.id,
+            export_association_id=export_association.id,
+            **payload.dict(),
+        )
+        result = write_history_to.delay(request=request, task_user_id=getattr(trans.user, "id", None))
+        task_summary = async_task_summary(result)
+        export_association.task_uuid = task_summary.id
+        with transaction(trans.sa_session):
+            trans.sa_session.commit()
+        return task_summary
+
+    def update(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        payload,
+        serialization_params: SerializationParams,
+    ):
+        """Updates the values for the history with the given ``id``
+
+        :param  history_id:      the encoded id of the history to update
+        :param  payload: a dictionary containing any or all the
+            fields in :func:`galaxy.model.History.to_dict` and/or the following:
+
+            * annotation: an annotation for the history
+
+        :param  serialization_params:   contains the optional `view`, `keys` and `default_view` for serialization
+
+        :returns:   an error object if an error occurred or a dictionary containing
+            any values that were different from the original and, therefore, updated
+        """
+        # TODO: PUT /api/histories/{encoded_history_id} payload = { rating: rating } (w/ no security checks)
+        history = self.manager.get_mutable(history_id, trans.user, current_history=trans.history)
+        self.deserializer.deserialize(history, payload, user=trans.user, trans=trans)
+        return self._serialize_history(trans, history, serialization_params)
+
+    def delete(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        serialization_params: SerializationParams,
+        purge: bool = False,
+    ):
+        """Delete the history with the given ``id``
+
+        .. note:: Stops all active jobs in the history if purge is set.
+
+        You can purge a history, removing all it's datasets from disk (if unshared),
+        by passing in ``purge=True`` in the url.
+        """
+        history = self.manager.get_mutable(history_id, trans.user, current_history=trans.history)
+        if purge:
+            self.manager.purge(history)
         else:
-            self.history_manager.error_unless_mutable(history)
-            permissions = {}
-            for action_key, action in trans.app.model.Dataset.permitted_actions.items():
-                in_roles = payload.get(action_key) or []
-                in_roles = [trans.sa_session.get(Role, trans.security.decode_id(x)) for x in in_roles]
-                permissions[trans.app.security_agent.get_action(action.action)] = in_roles
-            trans.app.security_agent.history_set_default_permissions(history, permissions)
-            return {"message": "Default history '%s' dataset permissions have been changed." % history.name}
-
-    @web.legacy_expose_api
-    @web.require_login("make datasets private")
-    def make_private(self, trans, history_id=None, all_histories=False, **kwd):
+            self.manager.delete(history)
+        return self._serialize_history(trans, history, serialization_params)
+
+    def undelete(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        serialization_params: SerializationParams,
+    ):
+        """Undelete history (that hasn't been purged) with the given ``id``
+
+        :param  history_id:     the encoded id of the history to undelete
+
+        :param  serialization_params:   contains the optional `view`, `keys` and `default_view` for serialization
+
+        :returns:   the undeleted history
         """
-        Sets the datasets within a history to private.  Also sets the default
-        permissions for the history to private, for future datasets.
+        history = self.manager.get_mutable(history_id, trans.user, current_history=trans.history)
+        self.manager.undelete(history)
+        return self._serialize_history(trans, history, serialization_params)
+
+    def shared_with_me(
+        self,
+        trans: ProvidesHistoryContext,
+        serialization_params: SerializationParams,
+        filter_query_params: FilterQueryParams,
+    ):
         """
-        histories = []
-        all_histories = string_as_bool(all_histories)
-        if all_histories:
-            histories = trans.user.histories
-        elif history_id:
-            history = self.history_manager.get_owned(
-                self.decode_id(history_id), trans.user, current_history=trans.history
-            )
-            if history:
-                histories.append(history)
-        if not histories:
-            return self.message_exception(trans, "Invalid history or histories specified.")
-        private_role = trans.app.security_agent.get_private_user_role(trans.user)
-        user_roles = trans.user.all_roles()
-        private_permissions = {
-            trans.app.security_agent.permitted_actions.DATASET_MANAGE_PERMISSIONS: [private_role],
-            trans.app.security_agent.permitted_actions.DATASET_ACCESS: [private_role],
-        }
-        for history in histories:
-            self.history_manager.error_unless_mutable(history)
-            # Set default role for history to private
-            trans.app.security_agent.history_set_default_permissions(history, private_permissions)
-            # Set private role for all datasets
-            for hda in history.datasets:
-                if (
-                    not hda.dataset.library_associations
-                    and not trans.app.security_agent.dataset_is_private_to_user(trans, hda.dataset)
-                    and trans.app.security_agent.can_manage_dataset(user_roles, hda.dataset)
-                ):
-                    # If it's not private to me, and I can manage it, set fixed private permissions.
-                    trans.app.security_agent.set_all_dataset_permissions(hda.dataset, private_permissions)
-                    if not trans.app.security_agent.dataset_is_private_to_user(trans, hda.dataset):
-                        raise exceptions.InternalServerError("An error occurred and the dataset is NOT private.")
-        return {
-            "message": f"Success, requested permissions have been changed in {'all histories' if all_histories else history.name}."
-        }
-
-    @web.expose
-    def adjust_hidden(self, trans, id=None, **kwd):
-        """THIS METHOD IS A TEMPORARY ADDITION. It'll allow us to fix the
-        regression in history-wide actions, and will be removed in the first
-        release after 17.01"""
-        action = kwd.get("user_action", None)
-        if action == "delete":
-            for hda in trans.history.datasets:
-                if not hda.visible:
-                    hda.mark_deleted()
-        elif action == "unhide":
-            trans.history.unhide_datasets()
-        with transaction(trans.sa_session):
-            trans.sa_session.commit()
+        Return all histories that are shared with the current user. The results can be filtered.
+        """
+        current_user = trans.user
+        filters = self.filters.parse_query_filters(filter_query_params)
+        order_by = self._build_order_by(filter_query_params.order)
+        histories = self.manager.list_shared_with(
+            current_user,
+            filters=filters,
+            order_by=order_by,
+            limit=filter_query_params.limit,
+            offset=filter_query_params.offset,
+        )
+        rval = [
+            self._serialize_history(trans, history, serialization_params, default_view="summary")
+            for history in histories
+        ]
+        return rval
+
+    def count(
+        self,
+        trans: ProvidesHistoryContext,
+    ):
+        """
+        Returns number of histories for the current user.
+        """
+        current_user = self.user_manager.current_user(trans)
+        if self.user_manager.is_anonymous(current_user):
+            current_history = self.manager.get_current(trans)
+            return 1 if current_history else 0
+        return self.manager.get_active_count(current_user)
+
+    def published(
+        self,
+        trans: ProvidesHistoryContext,
+        serialization_params: SerializationParams,
+        filter_query_params: FilterQueryParams,
+    ):
+        """
+        Return all histories that are published. The results can be filtered.
+        """
+        filters = self.filters.parse_query_filters(filter_query_params)
+        order_by = self._build_order_by(filter_query_params.order)
+        histories = self.manager.list_published(
+            filters=filters,
+            order_by=order_by,
+            limit=filter_query_params.limit,
+            offset=filter_query_params.offset,
+        )
+        rval = [
+            self._serialize_history(trans, history, serialization_params, default_view="summary")
+            for history in histories
+        ]
+        return rval
+
+    def citations(self, trans: ProvidesHistoryContext, history_id: DecodedDatabaseIdField):
+        """
+        Return all the citations for the tools used to produce the datasets in
+        the history.
+        """
+        history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        tool_ids = set()
+        for dataset in history.datasets:
+            job = dataset.creating_job
+            if not job:
+                continue
+            tool_id = job.tool_id
+            if not tool_id:
+                continue
+            tool_ids.add(tool_id)
+        return [citation.to_dict("bibtex") for citation in self.citations_manager.citations_for_tool_ids(tool_ids)]
+
+    def index_exports(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        use_tasks: bool = False,
+        limit: Optional[int] = None,
+        offset: Optional[int] = None,
+    ):
+        if use_tasks:
+            return self.history_export_manager.get_task_exports(trans, history_id, limit, offset)
+        return self.history_export_manager.get_exports(trans, history_id)
+
+    def archive_export(
+        self,
+        trans,
+        history_id: DecodedDatabaseIdField,
+        payload: Optional[ExportHistoryArchivePayload] = None,
+    ) -> Tuple[HistoryArchiveExportResult, bool]:
+        """
+        start job (if needed) to create history export for corresponding
+        history.
 
-    # ......................................................................... actions/orig. async
+        :param  history_id:     the encoded id of the history to export
 
-    @web.expose
-    def purge_deleted_datasets(self, trans):
-        count = 0
-        if trans.app.config.allow_user_dataset_purge and trans.history:
-            for hda in trans.history.datasets:
-                if not hda.deleted or hda.purged:
-                    continue
-                hda.purge_usage_from_quota(trans.user, hda.dataset.quota_source_info)
-                hda.purged = True
-                trans.sa_session.add(hda)
-                trans.log_event(f"HDA id {hda.id} has been purged")
-                with transaction(trans.sa_session):
-                    trans.sa_session.commit()
-                if hda.dataset.user_can_purge:
-                    try:
-                        hda.dataset.full_delete()
-                        trans.log_event(
-                            f"Dataset id {hda.dataset.id} has been purged upon the purge of HDA id {hda.id}"
-                        )
-                        trans.sa_session.add(hda.dataset)
-                    except Exception:
-                        log.exception(f"Unable to purge dataset ({hda.dataset.id}) on purge of hda ({hda.id}):")
-                count += 1
-            return trans.show_ok_message(
-                "%d datasets have been deleted permanently" % count, refresh_frames=["history"]
+        :returns:   object containing url to fetch export from.
+        """
+        if payload is None:
+            payload = ExportHistoryArchivePayload()
+        history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        jeha = history.latest_export
+        exporting_to_uri = payload.directory_uri
+        # always just issue a new export when exporting to a URI.
+        up_to_date = not payload.force and not exporting_to_uri and (jeha and jeha.up_to_date)
+        job = None
+        if not up_to_date:
+            # Need to create new JEHA + job.
+            job = self.manager.queue_history_export(
+                trans,
+                history,
+                gzip=payload.gzip,
+                include_hidden=payload.include_hidden,
+                include_deleted=payload.include_deleted,
+                directory_uri=payload.directory_uri,
+                file_name=payload.file_name,
             )
-        return trans.show_error_message("Cannot purge deleted datasets from this session.")
+        else:
+            job = jeha.job
 
-    @web.expose
-    def resume_paused_jobs(self, trans, current=False, ids=None, **kwargs):
-        """Resume paused jobs the active history -- this does not require a logged in user."""
-        if not ids and string_as_bool(current):
-            histories = [trans.get_history()]
-            refresh_frames = ["history"]
+        ready = bool((up_to_date and jeha.ready) or exporting_to_uri)
+
+        if exporting_to_uri:
+            # we don't have a jeha, there will never be a download_url. Just let
+            # the client poll on the created job_id to determine when the file has been
+            # written.
+            return (JobIdResponse(job_id=job.id), ready)
+
+        if up_to_date and jeha.ready:
+            serialized_jeha = self.history_export_manager.serialize(trans, history_id, jeha)
+            return (JobExportHistoryArchiveModel(**serialized_jeha), ready)
         else:
-            raise NotImplementedError("You can currently only resume all the datasets of the current history.")
-        for history in histories:
-            history.resume_paused_jobs()
-            trans.sa_session.add(history)
-        with transaction(trans.sa_session):
-            trans.sa_session.commit()
-        return trans.show_ok_message("Your jobs have been resumed.", refresh_frames=refresh_frames)
-        # TODO: used in index.mako
+            # Valid request, just resource is not ready yet.
+            if jeha:
+                serialized_jeha = self.history_export_manager.serialize(trans, history_id, jeha)
+                return (JobExportHistoryArchiveModel(**serialized_jeha), ready)
+            else:
+                assert job is not None, "logic error, don't have a jeha or a job"
+                return (JobIdResponse(job_id=job.id), ready)
+
+    def get_ready_history_export(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        jeha_id: Union[DecodedDatabaseIdField, LatestLiteral],
+    ) -> model.JobExportHistoryArchive:
+        """Returns the exported history archive information if it's ready
+        or raises an exception if not."""
+        return self.history_export_manager.get_ready_jeha(trans, history_id, jeha_id)
+
+    def get_archive_download_path(
+        self,
+        trans: ProvidesHistoryContext,
+        jeha: model.JobExportHistoryArchive,
+    ) -> str:
+        """
+        If ready and available, return raw contents of exported history
+        using a generator function.
+        """
+        return self.manager.get_ready_history_export_file_path(trans, jeha)
+
+    def get_archive_media_type(self, jeha: model.JobExportHistoryArchive):
+        media_type = "application/x-tar"
+        if jeha.compressed:
+            media_type = "application/x-gzip"
+        return media_type
+
+    # TODO: remove this function and HistoryManager.legacy_serve_ready_history_export when
+    # removing the legacy HistoriesController
+    def legacy_archive_download(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        jeha_id: DecodedDatabaseIdField,
+    ):
+        """
+        If ready and available, return raw contents of exported history.
+        """
+        jeha = self.history_export_manager.get_ready_jeha(trans, history_id, jeha_id)
+        return self.manager.legacy_serve_ready_history_export(trans, jeha)
+
+    def get_custom_builds_metadata(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+    ) -> CustomBuildsMetadataResponse:
+        """
+        Returns metadata for custom builds.
+        """
+        history = self.manager.get_accessible(history_id, trans.user, current_history=trans.history)
+        installed_builds = []
+        for build in glob.glob(os.path.join(trans.app.config.len_file_path, "*.len")):
+            installed_builds.append(os.path.basename(build).split(".len")[0])
+        fasta_hdas = get_fasta_hdas_by_history(trans.sa_session, history.id)
+        return CustomBuildsMetadataResponse(
+            installed_builds=[LabelValuePair(label=ins, value=ins) for ins in installed_builds],
+            fasta_hdas=[
+                LabelValuePair(label=f"{hda.hid}: {hda.name}", value=trans.security.encode_id(hda.id))
+                for hda in fasta_hdas
+            ],
+        )
+
+    def _serialize_history(
+        self,
+        trans: ProvidesHistoryContext,
+        history: model.History,
+        serialization_params: SerializationParams,
+        default_view: str = "detailed",
+    ) -> AnyHistoryView:
+        """
+        Returns a dictionary with the corresponding values depending on the
+        serialization parameters provided.
+        """
+        serialization_params.default_view = default_view
+        serialized_history = self.serializer.serialize_to_view(
+            history, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
+        )
+        return serialized_history
+
+    def _build_order_by(self, order: Optional[str]):
+        return self.build_order_by(self.manager, order or DEFAULT_ORDER_BY)
+
+    def archive_history(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        payload: Optional[ArchiveHistoryRequestPayload] = None,
+    ) -> AnyArchivedHistoryView:
+        """Marks the history with the given id as archived and optionally associates it with the given archive export record in the payload.
 
-    @web.legacy_expose_api
-    @web.require_login("rename histories")
-    def rename(self, trans, payload=None, **kwd):
-        id = kwd.get("id")
-        if not id:
-            return self.message_exception(trans, "No history id received for renaming.")
-        user = trans.get_user()
-        id = listify(id)
-        histories = []
-        for history_id in id:
-            history = self.history_manager.get_mutable(
-                self.decode_id(history_id), trans.user, current_history=trans.history
+        Archived histories are not part of the active histories of the user, so they won't be shown to the user by default.
+        """
+        if trans.anonymous:
+            raise glx_exceptions.AuthenticationRequired("Only registered users can archive histories.")
+
+        history = self.manager.get_owned(history_id, trans.user)
+        if history.archived:
+            raise glx_exceptions.Conflict("History is already archived.")
+
+        archive_export_id = payload.archive_export_id if payload else None
+        if archive_export_id:
+            export_record = self.history_export_manager.get_task_export_by_id(archive_export_id)
+            self._ensure_export_record_can_be_associated_with_history_archival(history_id, export_record)
+            # After this point, the export record is valid and can be associated with the history archival
+        purge_history = payload.purge_history if payload else False
+        if purge_history:
+            if archive_export_id is None:
+                raise glx_exceptions.RequestParameterMissingException(
+                    "Cannot purge history without an export record. A valid archive_export_id is required."
+                )
+            self.manager.purge(history)
+        history = self.manager.archive_history(history, archive_export_id=archive_export_id)
+        return self._serialize_archived_history(trans, history)
+
+    def _ensure_export_record_can_be_associated_with_history_archival(
+        self, history_id: int, export_record: model.StoreExportAssociation
+    ):
+        if export_record.object_id != history_id or export_record.object_type != "history":
+            raise glx_exceptions.RequestParameterInvalidException(
+                "The given archive export record does not belong to this history."
             )
-            if history and history.user_id == user.id:
-                histories.append(history)
-        if trans.request.method == "GET":
-            return {
-                "title": "Change history name(s)",
-                "inputs": [
-                    {"name": "name_%i" % i, "label": f"Current: {h.name}", "value": h.name}
-                    for i, h in enumerate(histories)
-                ],
-            }
-        else:
-            messages = []
-            for i, h in enumerate(histories):
-                cur_name = h.get_display_name()
-                new_name = payload.get("name_%i" % i)
-                # validate name is empty
-                if not isinstance(new_name, str) or not new_name.strip():
-                    messages.append("You must specify a valid name for History '%s'." % cur_name)
-                # skip if not the owner
-                elif h.user_id != user.id:
-                    messages.append("History '%s' does not appear to belong to you." % cur_name)
-                # skip if it wouldn't be a change
-                elif new_name != cur_name:
-                    h.name = new_name
-                    trans.sa_session.add(h)
-                    with transaction(trans.sa_session):
-                        trans.sa_session.commit()
-                    trans.log_event(f"History renamed: id: {str(h.id)}, renamed to: {new_name}")
-                    messages.append(f"History '{cur_name}' renamed to '{new_name}'.")
-            message = sanitize_text(" ".join(messages)) if messages else "History names remain unchanged."
-            return {"message": message, "status": "success"}
-
-    # ------------------------------------------------------------------------- current history
-    @web.expose
-    @web.require_login("switch to a history")
-    def switch_to_history(self, trans, hist_id=None, **kwargs):
-        """Change the current user's current history to one with `hist_id`."""
-        # remains for backwards compat
-        self.set_as_current(trans, id=hist_id)
-        return trans.response.send_redirect(url_for("/"))
-
-    def get_item(self, trans, id):
-        return self.history_manager.get_owned(self.decode_id(id), trans.user, current_history=trans.history)
-        # TODO: override of base ui controller?
-
-    def history_data(self, trans, history):
-        """Return the given history in a serialized, dictionary form."""
-        return self.history_serializer.serialize_to_view(history, view="dev-detailed", user=trans.user, trans=trans)
-
-    # TODO: combine these next two - poss. with a redirect flag
-    # @web.require_login( "switch to a history" )
-    @web.json
-    @web.do_not_cache
-    def set_as_current(self, trans, id, **kwargs):
-        """Change the current user's current history to one with `id`."""
-        try:
-            history = self.history_manager.get_mutable(self.decode_id(id), trans.user, current_history=trans.history)
-            trans.set_history(history)
-            return self.history_data(trans, history)
-        except exceptions.MessageException as msg_exc:
-            trans.response.status = msg_exc.status_code
-            return {"err_msg": msg_exc.err_msg, "err_code": msg_exc.err_code.code}
-
-    @web.json
-    @web.do_not_cache
-    def current_history_json(self, trans, since=None, **kwargs):
-        """Return the current user's current history in a serialized, dictionary form."""
-        history = trans.get_history(most_recent=True, create=True)
-        if since and history.update_time <= isoparse(since):
-            # Should ideally be a 204 response, but would require changing web.json
-            # This endpoint should either give way to a proper API or a SSE loop
-            return
-        return self.history_data(trans, history)
-
-    @web.json
-    def create_new_current(self, trans, name=None, **kwargs):
-        """Create a new, current history for the current user"""
-        new_history = trans.new_history(name)
-        return self.history_data(trans, new_history)
+        export_metadata = self.history_export_manager.get_record_metadata(export_record)
+        if export_metadata is None:
+            log.error(
+                f"Trying to archive history [{history_id}] with an export record. "
+                f"But the given archive export record [{export_record.id}] does not have the required metadata."
+            )
+            raise glx_exceptions.RequestParameterInvalidException(
+                "The given archive export record does not have the required metadata."
+            )
+        if not export_metadata.is_ready():
+            raise glx_exceptions.RequestParameterInvalidException(
+                "The given archive export record must be ready before it can be used to archive a history. "
+                "Please wait for the export to finish and try again."
+            )
+        if export_metadata.is_short_term():
+            raise glx_exceptions.RequestParameterInvalidException(
+                "The given archive export record is temporal, only persistent sources can be used to archive a history."
+            )
+        # TODO: should we also ensure the export was requested to include files with `include_files`, `include_hidden`, etc.?
+
+    def restore_archived_history(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: DecodedDatabaseIdField,
+        force: Optional[bool] = False,
+    ) -> AnyHistoryView:
+        if trans.anonymous:
+            raise glx_exceptions.AuthenticationRequired("Only registered users can access archived histories.")
+
+        history = self.manager.get_owned(history_id, trans.user)
+        history = self.manager.restore_archived_history(history, force=force or False)
+        return self._serialize_archived_history(trans, history)
+
+    def get_archived_histories(
+        self,
+        trans: ProvidesHistoryContext,
+        serialization_params: SerializationParams,
+        filter_query_params: FilterQueryParams,
+        include_total_matches: bool = False,
+    ) -> Tuple[List[AnyArchivedHistoryView], Optional[int]]:
+        if trans.anonymous:
+            raise glx_exceptions.AuthenticationRequired("Only registered users can have or access archived histories.")
+
+        filters = self.filters.parse_query_filters(filter_query_params)
+        filters += [
+            model.History.user == trans.user,
+            model.History.archived == true(),
+        ]
+        total_matches = self.manager.count(filters=filters) if include_total_matches else None
+        order_by = self._build_order_by(filter_query_params.order)
+        histories = self.manager.list(
+            filters=filters, order_by=order_by, limit=filter_query_params.limit, offset=filter_query_params.offset
+        )
 
-    # TODO: /history/current to do all of the above: if ajax, return json; if post, read id and set to current
+        histories = [self._serialize_archived_history(trans, history, serialization_params) for history in histories]
+        return histories, total_matches
+
+    def _serialize_archived_history(
+        self,
+        trans: ProvidesHistoryContext,
+        history: model.History,
+        serialization_params: Optional[SerializationParams] = None,
+    ):
+        if serialization_params is None:
+            serialization_params = SerializationParams(default_view="summary")
+        archived_history = self.serializer.serialize_to_view(
+            history, user=trans.user, trans=trans, **serialization_params.dict()
+        )
+        export_record_data = self._get_export_record_data(history)
+        archived_history["export_record_data"] = export_record_data.dict() if export_record_data else None
+        return archived_history
+
+    def _get_export_record_data(self, history: model.History) -> Optional[WriteStoreToPayload]:
+        if history.archive_export_id:
+            export_record = self.history_export_manager.get_task_export_by_id(history.archive_export_id)
+            export_metadata = self.history_export_manager.get_record_metadata(export_record)
+            if export_metadata and isinstance(export_metadata.request_data.payload, WriteStoreToPayload):
+                return export_metadata.request_data.payload
+        return None
+
+
+def get_fasta_hdas_by_history(session: Session, history_id: int):
+    stmt = (
+        select(HistoryDatasetAssociation)
+        .filter_by(history_id=history_id, extension="fasta", deleted=False)
+        .order_by(HistoryDatasetAssociation.hid.desc())
+    )
+    return session.scalars(stmt).all()
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/page.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/workflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,609 +1,494 @@
+import logging
+from html.parser import HTMLParser
+
 from markupsafe import escape
-from sqlalchemy import (
-    false,
-    true,
-)
-from sqlalchemy.orm import (
-    joinedload,
-    undefer,
-)
+from sqlalchemy import desc
+from sqlalchemy.orm import joinedload
 
 from galaxy import (
     model,
     util,
     web,
 )
-from galaxy.managers.hdas import HDAManager
-from galaxy.managers.histories import (
-    HistoryManager,
-    HistorySerializer,
-)
-from galaxy.managers.pages import (
-    get_page as get_page_,
-    get_shared_pages,
-    page_exists,
-    PageManager,
-)
 from galaxy.managers.sharable import SlugBuilder
-from galaxy.managers.users import get_user_by_username
-from galaxy.managers.workflows import WorkflowsManager
+from galaxy.managers.workflows import (
+    MissingToolsException,
+    WorkflowUpdateOptions,
+)
 from galaxy.model.base import transaction
 from galaxy.model.item_attrs import UsesItemRatings
-from galaxy.schema.schema import CreatePagePayload
-from galaxy.structured_app import StructuredApp
+from galaxy.tools.parameters.workflow_building_modes import workflow_building_modes
+from galaxy.util import FILENAME_VALID_CHARS
 from galaxy.util.sanitize_html import sanitize_html
-from galaxy.web import (
-    error,
-    url_for,
-)
-from galaxy.web.framework.helpers import (
-    grids,
-    time_ago,
-)
+from galaxy.web import url_for
 from galaxy.webapps.base.controller import (
     BaseUIController,
     SharableMixin,
     UsesStoredWorkflowMixin,
-    UsesVisualizationMixin,
 )
-from galaxy.webapps.galaxy.api import depends
-
-
-def format_bool(b):
-    if b:
-        return "yes"
-    else:
-        return ""
-
-
-class PageListGrid(grids.Grid):
-    # Custom column.
-    class URLColumn(grids.PublicURLColumn):
-        def get_value(self, trans, grid, item):
-            return url_for(
-                controller="page", action="display_by_username_and_slug", username=item.user.username, slug=item.slug
-            )
-
-    # Grid definition
-    use_panels = True
-    title = "Pages"
-    model_class = model.Page
-    default_filter = {"published": "All", "tags": "All", "title": "All", "sharing": "All"}
-    default_sort_key = "-update_time"
-    columns = [
-        grids.TextColumn(
-            "Title",
-            key="title",
-            attach_popup=True,
-            filterable="advanced",
-            link=(
-                lambda item: dict(action="display_by_username_and_slug", username=item.user.username, slug=item.slug)
-            ),
-        ),
-        URLColumn("Permalink"),
-        grids.OwnerAnnotationColumn(
-            "Annotation",
-            key="annotation",
-            model_annotation_association_class=model.PageAnnotationAssociation,
-            filterable="advanced",
-        ),
-        grids.IndividualTagsColumn(
-            "Tags",
-            key="tags",
-            model_tag_association_class=model.PageTagAssociation,
-            filterable="advanced",
-            grid_name="PageListGrid",
-        ),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False),
-        grids.GridColumn("Created", key="create_time", format=time_ago),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-    global_actions = [grids.GridAction("Add new page", dict(controller="", action="pages/create"))]
-    operations = [
-        grids.DisplayByUsernameAndSlugGridOperation("View", allow_multiple=False),
-        grids.GridOperation("Edit content", allow_multiple=False, url_args=dict(controller="", action="pages/editor")),
-        grids.GridOperation("Edit attributes", allow_multiple=False, url_args=dict(controller="", action="pages/edit")),
-        grids.GridOperation(
-            "Share or Publish",
-            allow_multiple=False,
-            condition=(lambda item: not item.deleted),
-            url_args=dict(controller="", action="pages/sharing"),
-        ),
-        grids.GridOperation("Delete", confirm="Are you sure you want to delete this page?"),
-    ]
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter_by(user=trans.user, deleted=False)
-
-
-class PageAllPublishedGrid(grids.Grid):
-    # Grid definition
-    use_panels = True
-    title = "Published Pages"
-    model_class = model.Page
-    default_sort_key = "update_time"
-    default_filter = dict(title="All", username="All")
-    columns = [
-        grids.PublicURLColumn("Title", key="title", filterable="advanced"),
-        grids.OwnerAnnotationColumn(
-            "Annotation",
-            key="annotation",
-            model_annotation_association_class=model.PageAnnotationAssociation,
-            filterable="advanced",
-        ),
-        grids.OwnerColumn("Owner", key="username", model_class=model.User, filterable="advanced"),
-        grids.CommunityRatingColumn("Community Rating", key="rating"),
-        grids.CommunityTagsColumn(
-            "Community Tags",
-            key="tags",
-            model_tag_association_class=model.PageTagAssociation,
-            filterable="advanced",
-            grid_name="PageAllPublishedGrid",
-        ),
-        grids.ReverseSortColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search title, annotation, owner, and tags",
-            cols_to_filter=[columns[0], columns[1], columns[2], columns[4]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
-
-    def build_initial_query(self, trans, **kwargs):
-        # See optimization description comments and TODO for tags in matching public histories query.
-        return (
-            trans.sa_session.query(self.model_class)
-            .join("user")
-            .filter(model.User.deleted == false())
-            .options(
-                joinedload(self.model_class.user).load_only("username"),
-                joinedload(self.model_class.annotations),
-                undefer("average_rating"),
-            )
-        )
+from galaxy.workflow.extract import (
+    extract_workflow,
+    summarize,
+)
+from galaxy.workflow.modules import load_module_sections
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter(self.model_class.deleted == false()).filter(self.model_class.published == true())
+log = logging.getLogger(__name__)
 
 
-class ItemSelectionGrid(grids.Grid):
-    """Base class for pages' item selection grids."""
+# Simple HTML parser to get all content in a single tag.
+class SingleTagContentsParser(HTMLParser):
+    def __init__(self, target_tag):
+        # Cannot use super() because HTMLParser is an old-style class in Python2
+        HTMLParser.__init__(self)
+        self.target_tag = target_tag
+        self.cur_tag = None
+        self.tag_content = ""
 
-    # Custom columns.
-    class NameColumn(grids.TextColumn):
-        def get_value(self, trans, grid, item):
-            if hasattr(item, "get_display_name"):
-                return escape(item.get_display_name())
-            else:
-                return escape(item.name)
+    def handle_starttag(self, tag, attrs):
+        """Called for each start tag."""
+        self.cur_tag = tag
 
-    # Grid definition.
-    show_item_checkboxes = True
-    default_filter = {"deleted": "False", "sharing": "All"}
-    default_sort_key = "-update_time"
-    use_paging = True
-    num_rows_per_page = 10
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter_by(user=trans.user)
-
-
-class HistorySelectionGrid(ItemSelectionGrid):
-    """Grid for selecting histories."""
-
-    # Grid definition.
-    title = "Saved Histories"
-    model_class = model.History
-    columns = [
-        ItemSelectionGrid.NameColumn("Name", key="name", filterable="advanced"),
-        grids.IndividualTagsColumn(
-            "Tags", key="tags", model_tag_association_class=model.HistoryTagAssociation, filterable="advanced"
-        ),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False, visible=False),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
-    )
+    def handle_data(self, text):
+        """Called for each block of plain text."""
+        if self.cur_tag == self.target_tag:
+            self.tag_content += text
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter_by(user=trans.user, purged=False)
 
+class WorkflowController(BaseUIController, SharableMixin, UsesStoredWorkflowMixin, UsesItemRatings):
+    slug_builder = SlugBuilder()
 
-class HistoryDatasetAssociationSelectionGrid(ItemSelectionGrid):
-    """Grid for selecting HDAs."""
+    @web.expose
+    def display_by_username_and_slug(self, trans, username, slug, format="html", **kwargs):
+        """
+        Display workflow based on a username and slug. Format can be html, json, or json-download.
+        """
 
-    # Grid definition.
-    title = "Saved Datasets"
-    model_class = model.HistoryDatasetAssociation
-    columns = [
-        ItemSelectionGrid.NameColumn("Name", key="name", filterable="advanced"),
-        grids.IndividualTagsColumn(
-            "Tags",
-            key="tags",
-            model_tag_association_class=model.HistoryDatasetAssociationTagAssociation,
-            filterable="advanced",
-        ),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False, visible=False),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
+        # Get workflow by username and slug. Security is handled by the display methods below.
+        session = trans.sa_session
+        user = session.query(model.User).filter_by(username=username).first()
+        if not user:
+            raise web.httpexceptions.HTTPNotFound()
+        stored_workflow = (
+            trans.sa_session.query(model.StoredWorkflow).filter_by(user=user, slug=slug, deleted=False).first()
         )
-    )
+        if not stored_workflow:
+            raise web.httpexceptions.HTTPNotFound()
+        encoded_id = trans.security.encode_id(stored_workflow.id)
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        # To filter HDAs by user, need to join HDA and History table and then filter histories by user. This is necessary because HDAs do not have
-        # a user relation.
-        return query.select_from(model.HistoryDatasetAssociation.table.join(model.History.table)).filter(
-            model.History.user == trans.user
-        )
+        # Display workflow in requested format.
+        if format == "html":
+            return self._display(trans, stored_workflow)
+        elif format == "json":
+            return self.for_direct_import(trans, encoded_id)
+        elif format == "json-download":
+            return self.export_to_file(trans, encoded_id)
+
+    def _display(self, trans, stored_workflow):
+        """Diplay workflow in client."""
+        if stored_workflow is None:
+            raise web.httpexceptions.HTTPNotFound()
 
+        # Security check raises error if user cannot access workflow.
+        self.security_check(trans, stored_workflow, False, True)
 
-class WorkflowSelectionGrid(ItemSelectionGrid):
-    """Grid for selecting workflows."""
+        # Get data for workflow's steps.
+        self.get_stored_workflow_steps(trans, stored_workflow)
 
-    # Grid definition.
-    title = "Saved Workflows"
-    model_class = model.StoredWorkflow
-    columns = [
-        ItemSelectionGrid.NameColumn("Name", key="name", filterable="advanced"),
-        grids.IndividualTagsColumn(
-            "Tags", key="tags", model_tag_association_class=model.StoredWorkflowTagAssociation, filterable="advanced"
-        ),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False, visible=False),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
+        # Get annotations.
+        stored_workflow.annotation = self.get_item_annotation_str(
+            trans.sa_session, stored_workflow.user, stored_workflow
         )
-    )
-
+        for step in stored_workflow.latest_workflow.steps:
+            step.annotation = self.get_item_annotation_str(trans.sa_session, stored_workflow.user, step)
 
-class PageSelectionGrid(ItemSelectionGrid):
-    """Grid for selecting pages."""
+        # Encode page identifier.
+        workflow_id = trans.security.encode_id(stored_workflow.id)
 
-    # Grid definition.
-    title = "Saved Pages"
-    model_class = model.Page
-    columns = [
-        grids.TextColumn("Title", key="title", filterable="advanced"),
-        grids.IndividualTagsColumn(
-            "Tags", key="tags", model_tag_association_class=model.PageTagAssociation, filterable="advanced"
-        ),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-        # Columns that are valid for filtering but are not visible.
-        grids.DeletedColumn("Deleted", key="deleted", visible=False, filterable="advanced"),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False, visible=False),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[1]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
+        # Redirect to client.
+        return trans.response.send_redirect(
+            web.url_for(
+                controller="published",
+                action="workflow",
+                id=workflow_id,
+            )
         )
-    )
 
+    @web.expose
+    @web.require_login("to import a workflow", use_panels=True)
+    def imp(self, trans, id, **kwargs):
+        """Imports a workflow shared by other users."""
+        # Set referer message.
+        referer = trans.request.referer
+        if referer and not referer.startswith(f"{trans.request.application_url}{url_for('/login')}"):
+            referer_message = f"<a href='{escape(referer)}'>return to the previous page</a>"
+        else:
+            referer_message = f"<a href='{url_for('/')}'>go to Galaxy's start page</a>"
 
-class VisualizationSelectionGrid(ItemSelectionGrid):
-    """Grid for selecting visualizations."""
+        # Do import.
+        stored = self.get_stored_workflow(trans, id, check_ownership=False)
+        if stored.importable is False:
+            return trans.show_error_message(
+                f"The owner of this workflow has disabled imports via this link.<br>You can {referer_message}",
+                use_panels=True,
+            )
+        elif stored.deleted:
+            return trans.show_error_message(
+                f"You can't import this workflow because it has been deleted.<br>You can {referer_message}",
+                use_panels=True,
+            )
+        self._import_shared_workflow(trans, stored)
 
-    # Grid definition.
-    title = "Saved Visualizations"
-    model_class = model.Visualization
-    columns = [
-        grids.TextColumn("Title", key="title", filterable="advanced"),
-        grids.TextColumn("Type", key="type"),
-        grids.IndividualTagsColumn(
-            "Tags",
-            key="tags",
-            model_tag_association_class=model.VisualizationTagAssociation,
-            filterable="advanced",
-            grid_name="VisualizationListGrid",
-        ),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
+        # Redirect to load galaxy frames.
+        return trans.show_ok_message(
+            message="""Workflow "{}" has been imported. <br>You can <a href="{}">start using this workflow</a> or {}.""".format(
+                stored.name, web.url_for("/workflows/list"), referer_message
+            )
         )
-    )
-
-
-# Adapted from the _BaseHTMLProcessor class of https://github.com/kurtmckee/feedparser
-class PageController(BaseUIController, SharableMixin, UsesStoredWorkflowMixin, UsesVisualizationMixin, UsesItemRatings):
-    _page_list = PageListGrid()
-    _all_published_list = PageAllPublishedGrid()
-    _history_selection_grid = HistorySelectionGrid()
-    _workflow_selection_grid = WorkflowSelectionGrid()
-    _datasets_selection_grid = HistoryDatasetAssociationSelectionGrid()
-    _page_selection_grid = PageSelectionGrid()
-    _visualization_selection_grid = VisualizationSelectionGrid()
-    page_manager: PageManager = depends(PageManager)
-    history_manager: HistoryManager = depends(HistoryManager)
-    history_serializer: HistorySerializer = depends(HistorySerializer)
-    hda_manager: HDAManager = depends(HDAManager)
-    workflow_manager: WorkflowsManager = depends(WorkflowsManager)
-    slug_builder: SlugBuilder = depends(SlugBuilder)
-
-    def __init__(self, app: StructuredApp):
-        super().__init__(app)
 
     @web.expose
-    @web.json
-    @web.require_login()
-    def list(self, trans, *args, **kwargs):
-        """List user's pages."""
-        # Handle operation
-        if "operation" in kwargs and "id" in kwargs:
-            session = trans.sa_session
-            operation = kwargs["operation"].lower()
-            ids = util.listify(kwargs["id"])
-            for id in ids:
-                if operation == "delete":
-                    item = session.get(model.Page, self.decode_id(id))
-                    self.security_check(trans, item, check_ownership=True)
-                    item.deleted = True
-            with transaction(session):
-                session.commit()
+    @web.require_login("use Galaxy workflows")
+    def rename_async(self, trans, id, new_name=None, **kwargs):
+        stored = self.get_stored_workflow(trans, id)
+        if new_name:
+            san_new_name = sanitize_html(new_name)
+            stored.name = san_new_name
+            stored.latest_workflow.name = san_new_name
+            with transaction(trans.sa_session):
+                trans.sa_session.commit()
+            return stored.name
 
-        # Build grid dictionary.
-        grid = self._page_list(trans, *args, **kwargs)
-        grid["shared_by_others"] = self._get_shared(trans)
-        return grid
+    @web.expose
+    @web.require_login("use Galaxy workflows")
+    def annotate_async(self, trans, id, new_annotation=None, **kwargs):
+        stored = self.get_stored_workflow(trans, id)
+        if new_annotation:
+            # Sanitize annotation before adding it.
+            new_annotation = sanitize_html(new_annotation)
+            self.add_item_annotation(trans.sa_session, trans.get_user(), stored, new_annotation)
+            with transaction(trans.sa_session):
+                trans.sa_session.commit()
+            return new_annotation
 
     @web.expose
-    @web.json
-    def list_published(self, trans, *args, **kwargs):
-        grid = self._all_published_list(trans, *args, **kwargs)
-        grid["shared_by_others"] = self._get_shared(trans)
-        return grid
-
-    def _get_shared(self, trans):
-        """Identify shared pages"""
-        shared_by_others = get_shared_pages(trans.sa_session, trans.get_user())
-        return [
-            {"username": p.page.user.username, "slug": p.page.slug, "title": p.page.title} for p in shared_by_others
-        ]
+    @web.require_login("use Galaxy workflows")
+    def gen_image(self, trans, id, embed="false", version="", **kwargs):
+        embed = util.asbool(embed)
+        if version:
+            version_int_or_none = int(version)
+        else:
+            version_int_or_none = None
+        try:
+            s = trans.app.workflow_manager.get_workflow_svg_from_id(
+                trans, id, version=version_int_or_none, for_embed=embed
+            )
+            trans.response.set_content_type("image/svg+xml")
+            return s
+        except Exception as e:
+            log.exception("Failed to generate SVG image")
+            error_message = str(e)
+            return trans.show_error_message(error_message)
 
-    @web.expose_api
-    @web.require_login("create pages")
+    @web.legacy_expose_api
     def create(self, trans, payload=None, **kwd):
-        """
-        Create a new page.
-        """
         if trans.request.method == "GET":
-            form_title = "Create new Page"
-            title = ""
-            slug = ""
-            content = ""
-            content_hide = True
-            if "invocation_id" in kwd:
-                invocation_id = kwd.get("invocation_id")
-                form_title = f"{form_title} from Invocation Report"
-                slug = f"invocation-report-{invocation_id}"
-                invocation_report = self.workflow_manager.get_invocation_report(
-                    trans, trans.security.decode_id(invocation_id)
-                )
-                title = invocation_report.get("title")
-                content = invocation_report.get("markdown")
-                content_hide = False
             return {
-                "title": form_title,
+                "title": "Create Workflow",
                 "inputs": [
+                    {"name": "workflow_name", "label": "Name", "value": "Unnamed workflow"},
                     {
-                        "name": "title",
-                        "label": "Name",
-                        "value": title,
-                    },
-                    {
-                        "name": "slug",
-                        "label": "Identifier",
-                        "help": "A unique identifier that will be used for public links to this page. This field can only contain lowercase letters, numbers, and dashes (-).",
-                        "value": slug,
-                    },
-                    {
-                        "name": "annotation",
+                        "name": "workflow_annotation",
                         "label": "Annotation",
-                        "help": "A description of the page. The annotation is shown alongside published pages.",
-                    },
-                    {
-                        "name": "content_format",
-                        "label": "Content Format",
-                        "value": "markdown",
-                        "hidden": True,
-                    },
-                    {
-                        "name": "content",
-                        "label": "Content",
-                        "area": True,
-                        "value": content,
-                        "hidden": content_hide,
+                        "help": "A description of the workflow; annotation is shown alongside shared or published workflows.",
                     },
                 ],
             }
         else:
-            page = self.page_manager.create_page(trans, CreatePagePayload(**payload))
-            return {"message": "Page '%s' successfully created." % page.title, "status": "success"}
+            user = trans.get_user()
+            workflow_name = payload.get("workflow_name")
+            workflow_annotation = payload.get("workflow_annotation")
+            workflow_tags = payload.get("workflow_tags", [])
+            if not workflow_name:
+                return self.message_exception(trans, "Please provide a workflow name.")
+            # Create the new stored workflow
+            stored_workflow = model.StoredWorkflow()
+            stored_workflow.name = workflow_name
+            stored_workflow.user = user
+            self.slug_builder.create_item_slug(trans.sa_session, stored_workflow)
+            # And the first (empty) workflow revision
+            workflow = model.Workflow()
+            workflow.name = workflow_name
+            workflow.stored_workflow = stored_workflow
+            stored_workflow.latest_workflow = workflow
+            # Add annotation.
+            workflow_annotation = sanitize_html(workflow_annotation)
+            self.add_item_annotation(trans.sa_session, trans.get_user(), stored_workflow, workflow_annotation)
+            # Add tags
+            trans.tag_handler.set_tags_from_list(
+                trans.user,
+                stored_workflow,
+                workflow_tags,
+            )
+            # Persist
+            session = trans.sa_session
+            session.add(stored_workflow)
+            with transaction(session):
+                session.commit()
+            return {
+                "id": trans.security.encode_id(stored_workflow.id),
+                "message": f"Workflow {workflow_name} has been created.",
+            }
 
-    @web.legacy_expose_api
-    @web.require_login("edit pages")
-    def edit(self, trans, payload=None, **kwd):
+    @web.json
+    def save_workflow_as(
+        self, trans, workflow_name, workflow_data, workflow_annotation="", from_tool_form=False, **kwargs
+    ):
         """
-        Edit a page's attributes.
+        Creates a new workflow based on Save As command. It is a new workflow, but
+        is created with workflow_data already present.
         """
-        id = kwd.get("id")
-        if not id:
-            return self.message_exception(trans, "No page id received for editing.")
-        decoded_id = self.decode_id(id)
         user = trans.get_user()
-        p = trans.sa_session.get(model.Page, decoded_id)
-        p = self.security_check(trans, p, check_ownership=True)
-        if trans.request.method == "GET":
-            if p.slug is None:
-                self.slug_builder.create_item_slug(trans.sa_session, p)
-            return {
-                "title": "Edit page attributes",
-                "inputs": [
-                    {"name": "title", "label": "Name", "value": p.title},
-                    {
-                        "name": "slug",
-                        "label": "Identifier",
-                        "value": p.slug,
-                        "help": "A unique identifier that will be used for public links to this page. This field can only contain lowercase letters, numbers, and dashes (-).",
-                    },
-                    {
-                        "name": "annotation",
-                        "label": "Annotation",
-                        "value": self.get_item_annotation_str(trans.sa_session, user, p),
-                        "help": "A description of the page. The annotation is shown alongside published pages.",
-                    },
-                ],
-            }
-        else:
-            p_title = payload.get("title")
-            p_slug = payload.get("slug")
-            p_annotation = payload.get("annotation")
-            if not p_title:
-                return self.message_exception(trans, "Please provide a page name is required.")
-            elif not p_slug:
-                return self.message_exception(trans, "Please provide a unique identifier.")
-            elif not self._is_valid_slug(p_slug):
-                return self.message_exception(
-                    trans, "Page identifier can only contain lowercase letters, numbers, and dashes (-)."
+        if workflow_name is not None:
+            workflow_contents_manager = self.app.workflow_contents_manager
+            stored_workflow = model.StoredWorkflow()
+            stored_workflow.name = workflow_name
+            stored_workflow.user = user
+            self.slug_builder.create_item_slug(trans.sa_session, stored_workflow)
+            workflow = model.Workflow()
+            workflow.name = workflow_name
+            workflow.stored_workflow = stored_workflow
+            stored_workflow.latest_workflow = workflow
+            # Add annotation.
+            workflow_annotation = sanitize_html(workflow_annotation)
+            self.add_item_annotation(trans.sa_session, trans.get_user(), stored_workflow, workflow_annotation)
+
+            # Persist
+            session = trans.sa_session
+            session.add(stored_workflow)
+            with transaction(session):
+                session.commit()
+            workflow_update_options = WorkflowUpdateOptions(
+                update_stored_workflow_attributes=False,  # taken care of above
+                from_tool_form=from_tool_form,
+            )
+            try:
+                workflow, errors = workflow_contents_manager.update_workflow_from_raw_description(
+                    trans,
+                    stored_workflow,
+                    workflow_data,
+                    workflow_update_options,
                 )
-            elif p_slug != p.slug and page_exists(trans.sa_session, p.user, p_slug):
-                return self.message_exception(trans, "Page id must be unique.")
-            else:
-                p.title = p_title
-                p.slug = p_slug
-                if p_annotation:
-                    p_annotation = sanitize_html(p_annotation)
-                    self.add_item_annotation(trans.sa_session, user, p, p_annotation)
-                trans.sa_session.add(p)
-                with transaction(trans.sa_session):
-                    trans.sa_session.commit()
-            return {"message": "Attributes of '%s' successfully saved." % p.title, "status": "success"}
+            except MissingToolsException as e:
+                return dict(
+                    name=e.workflow.name,
+                    message=(
+                        "This workflow includes missing or invalid tools. "
+                        "It cannot be saved until the following steps are removed or the missing tools are enabled."
+                    ),
+                    errors=e.errors,
+                )
+            return trans.security.encode_id(stored_workflow.id)
+        else:
+            # This is an error state, 'save as' must have a workflow_name
+            log.exception("Error in Save As workflow: no name.")
 
     @web.expose
-    @web.require_login()
-    def display(self, trans, id, **kwargs):
-        id = self.decode_id(id)
-        page = trans.sa_session.get(model.Page, id)
-        if not page:
-            raise web.httpexceptions.HTTPNotFound()
-        return self.display_by_username_and_slug(trans, page.user.username, page.slug)
+    @web.json
+    @web.require_login("edit workflows")
+    def editor(self, trans, id=None, workflow_id=None, version=None, **kwargs):
+        """
+        Render the main workflow editor interface. The canvas is embedded as
+        an iframe (necessary for scrolling to work properly), which is
+        rendered by `editor_canvas`.
+        """
 
-    @web.expose
-    def display_by_username_and_slug(self, trans, username, slug, **kwargs):
-        """Display page based on a username and slug."""
+        new_workflow = False
+        if not id:
+            if workflow_id:
+                stored_workflow = self.app.workflow_manager.get_stored_workflow(trans, workflow_id, by_stored_id=False)
+                self.security_check(trans, stored_workflow, True, False)
+                id = trans.security.encode_id(stored_workflow.id)
+            else:
+                new_workflow = True
 
-        # Get page.
-        user = get_user_by_username(trans.sa_session, username)
-        page = get_page_(trans.sa_session, user, slug)
-        if page is None:
-            raise web.httpexceptions.HTTPNotFound()
+        # The following query loads all user-owned workflows,
+        # So that they can be copied or inserted in the workflow editor.
+        workflows = (
+            trans.sa_session.query(model.StoredWorkflow)
+            .filter_by(user=trans.user, deleted=False, hidden=False)
+            .order_by(desc(model.StoredWorkflow.table.c.update_time))
+            .options(joinedload(model.StoredWorkflow.latest_workflow).joinedload(model.Workflow.steps))
+            .all()
+        )
 
-        # Security check raises error if user cannot access page.
-        self.security_check(trans, page, False, True)
+        # create workflow module models
+        module_sections = []
+        for module_section in load_module_sections(trans).values():
+            module_sections.append(
+                {
+                    "title": module_section.get("title"),
+                    "name": module_section.get("name"),
+                    "elems": [
+                        {"name": elem.get("name"), "title": elem.get("title"), "description": elem.get("description")}
+                        for elem in module_section.get("modules")
+                    ],
+                }
+            )
 
-        # Encode page identifier.
-        page_id = trans.security.encode_id(page.id)
+        # create data manager tool models
+        data_managers = []
+        if trans.user_is_admin and trans.app.data_managers.data_managers:
+            for data_manager_val in trans.app.data_managers.data_managers.values():
+                tool = data_manager_val.tool
+                if not tool.hidden:
+                    data_managers.append(
+                        {
+                            "id": tool.id,
+                            "name": tool.name,
+                            "hidden": tool.hidden,
+                            "description": tool.description,
+                            "is_workflow_compatible": tool.is_workflow_compatible,
+                        }
+                    )
+
+        stored = None
+        if new_workflow is False:
+            stored = self.get_stored_workflow(trans, id)
 
-        # Redirect to client.
-        return trans.response.send_redirect(
-            web.url_for(
-                controller="published",
-                action="page",
-                id=page_id,
+            if version is None:
+                version = len(stored.workflows) - 1
+            else:
+                version = int(version)
+
+            # identify item tags
+            item_tags = stored.make_tag_string_list()
+
+        # create workflow models
+        workflows = [
+            {
+                "id": trans.security.encode_id(workflow.id),
+                "latest_id": trans.security.encode_id(workflow.latest_workflow.id),
+                "step_count": len(workflow.latest_workflow.steps),
+                "name": workflow.name,
+            }
+            for workflow in workflows
+            if new_workflow or workflow.id != stored.id
+        ]
+
+        # build workflow editor model
+        editor_config = {
+            "moduleSections": module_sections,
+            "dataManagers": data_managers,
+            "workflows": workflows,
+        }
+
+        # for existing workflow add its data to the model
+        if new_workflow is False:
+            editor_config.update(
+                {
+                    "id": trans.security.encode_id(stored.id),
+                    "name": stored.name,
+                    "tags": item_tags,
+                    "initialVersion": version,
+                    "annotation": self.get_item_annotation_str(trans.sa_session, trans.user, stored),
+                }
             )
-        )
 
-    @web.expose
-    @web.json
-    @web.require_login("select a history from saved histories")
-    def list_histories_for_selection(self, trans, **kwargs):
-        """Returns HTML that enables a user to select one or more histories."""
-        return self._history_selection_grid(trans, **kwargs)
+        # parse to mako
+        return editor_config
 
-    @web.expose
     @web.json
-    @web.require_login("select a workflow from saved workflows")
-    def list_workflows_for_selection(self, trans, **kwargs):
-        """Returns HTML that enables a user to select one or more workflows."""
-        return self._workflow_selection_grid(trans, **kwargs)
+    def load_workflow(self, trans, id, version=None, **kwargs):
+        """
+        Get the latest Workflow for the StoredWorkflow identified by `id` and
+        encode it as a json string that can be read by the workflow editor
+        web interface.
+        """
+        trans.workflow_building_mode = workflow_building_modes.ENABLED
+        stored = self.get_stored_workflow(trans, id, check_ownership=False, check_accessible=True)
+        workflow_contents_manager = self.app.workflow_contents_manager
+        return workflow_contents_manager.workflow_to_dict(trans, stored, style="editor", version=version)
 
-    @web.expose
-    @web.json
-    @web.require_login("select a visualization from saved visualizations")
-    def list_visualizations_for_selection(self, trans, **kwargs):
-        """Returns HTML that enables a user to select one or more visualizations."""
-        return self._visualization_selection_grid(trans, **kwargs)
+    @web.json_pretty
+    def for_direct_import(self, trans, id, **kwargs):
+        """
+        Get the latest Workflow for the StoredWorkflow identified by `id` and
+        encode it as a json string that can be imported back into Galaxy
 
-    @web.expose
-    @web.json
-    @web.require_login("select a page from saved pages")
-    def list_pages_for_selection(self, trans, **kwargs):
-        """Returns HTML that enables a user to select one or more pages."""
-        return self._page_selection_grid(trans, **kwargs)
+        This has slightly different information than the above. In particular,
+        it does not attempt to decode forms and build UIs, it just stores
+        the raw state.
+        """
+        stored = self.get_stored_workflow(trans, id, check_ownership=False, check_accessible=True)
+        return self._workflow_to_dict(trans, stored)
+
+    @web.json_pretty
+    def export_to_file(self, trans, id):
+        """
+        Get the latest Workflow for the StoredWorkflow identified by `id` and
+        export it to a JSON file that can be imported back into Galaxy.
+
+        This has slightly different information than the above. In particular,
+        it does not attempt to decode forms and build UIs, it just stores
+        the raw state.
+        """
+
+        # Get workflow.
+        stored = self.get_stored_workflow(trans, id, check_ownership=False, check_accessible=True)
+
+        # Stream workflow to file.
+        stored_dict = self._workflow_to_dict(trans, stored)
+        if not stored_dict:
+            # This workflow has a tool that's missing from the distribution
+            trans.response.status = 400
+            return "Workflow cannot be exported due to missing tools."
+        sname = stored.name
+        sname = "".join(c in FILENAME_VALID_CHARS and c or "_" for c in sname)[0:150]
+        trans.response.headers["Content-Disposition"] = f'attachment; filename="Galaxy-Workflow-{sname}.ga"'
+        trans.response.set_content_type("application/galaxy-archive")
+        return stored_dict
 
     @web.expose
-    @web.json
-    @web.require_login("select a dataset from saved datasets")
-    def list_datasets_for_selection(self, trans, **kwargs):
-        """Returns HTML that enables a user to select one or more datasets."""
-        return self._datasets_selection_grid(trans, **kwargs)
-
-    def get_page(self, trans, id, check_ownership=True, check_accessible=False):
-        """Get a page from the database by id."""
-        # Load history from database
-        id = self.decode_id(id)
-        page = trans.sa_session.get(model.Page, id)
-        if not page:
-            error("Page not found")
+    def build_from_current_history(
+        self,
+        trans,
+        job_ids=None,
+        dataset_ids=None,
+        dataset_collection_ids=None,
+        workflow_name=None,
+        dataset_names=None,
+        dataset_collection_names=None,
+        **kwargs,
+    ):
+        user = trans.get_user()
+        history = trans.get_history()
+        if not user:
+            return trans.show_error_message("Must be logged in to create workflows")
+        if (job_ids is None and dataset_ids is None) or workflow_name is None:
+            jobs, warnings = summarize(trans)
+            # Render
+            return trans.fill_template(
+                "workflow/build_from_current_history.mako", jobs=jobs, warnings=warnings, history=history
+            )
         else:
-            return self.security_check(trans, page, check_ownership, check_accessible)
-
-    def get_item(self, trans, id):
-        return self.get_page(trans, id)
+            # If there is just one dataset name selected or one dataset collection, these
+            # come through as string types instead of lists. xref #3247.
+            dataset_names = util.listify(dataset_names)
+            dataset_collection_names = util.listify(dataset_collection_names)
+            stored_workflow = extract_workflow(
+                trans,
+                user=user,
+                job_ids=job_ids,
+                dataset_ids=dataset_ids,
+                dataset_collection_ids=dataset_collection_ids,
+                workflow_name=workflow_name,
+                dataset_names=dataset_names,
+                dataset_collection_names=dataset_collection_names,
+            )
+            # Index page with message
+            workflow_id = trans.security.encode_id(stored_workflow.id)
+            edit_url = url_for(f"/workflows/edit?id={workflow_id}")
+            run_url = url_for(f"/workflows/run?id={workflow_id}")
+            return trans.show_message(
+                f'Workflow "{escape(workflow_name)}" created from current history. '
+                f'You can <a href="{edit_url}" target="_parent">edit</a> or <a href="{run_url}" target="_parent">run</a> the workflow.'
+            )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/root.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/root.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/shed_tool_static.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/shed_tool_static.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/tag.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tags Controller: handles tagging/untagging of entities
 and provides autocomplete support.
 """
+
 import logging
 
 from sqlalchemy.sql import select
 from sqlalchemy.sql.expression import (
     and_,
     func,
 )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/tool_runner.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/tool_runner.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Controller handles external tool related requests
 """
+
 import logging
 
 from markupsafe import escape
 
 import galaxy.util
 from galaxy import web
 from galaxy.tools import DataSourceTool
@@ -70,26 +71,47 @@
             )
         if not tool.allow_user_access(trans.user):
             return __tool_404__()
         # FIXME: Tool class should define behavior
         if tool.tool_type in ["default", "interactivetool"]:
             return trans.response.send_redirect(url_for(controller="root", tool_id=tool_id))
 
-        # execute tool without displaying form (used for datasource tools)
-        params = galaxy.util.Params(kwd, sanitize=False)
-        # do param translation here, used by datasource tools
+        # execute tool without displaying form
+        # (used for datasource tools, but note that data_source_async tools
+        # are handled separately by the async controller)
+        params = galaxy.util.Params(kwd, sanitize=False).__dict__
         if tool.input_translator:
-            tool.input_translator.translate(params)
-        if "runtool_btn" not in params.__dict__ and "URL" not in params.__dict__:
-            error("Tool execution through the `tool_runner` requires a `runtool_btn` flag or `URL` parameter.")
+            # perform test translation of the incoming params without affecting originals
+            # the actual translation will happen later
+            # this is only for checking if we end up with required parameters
+            test_params = params.copy()
+            tool.input_translator.translate(test_params)
+        else:
+            test_params = params
+        if tool.tool_type == "data_source":
+            if "URL" not in test_params:
+                error("Execution of `data_source` tools requires a `URL` parameter")
+            # preserve original params sent by the remote server as extra dict
+            # before in-place translation happens, then clean the incoming params
+            params.update({"incoming_request_params": params.copy()})
+            if tool.input_translator and tool.wants_params_cleaned:
+                for k in list(params.keys()):
+                    if k not in tool.input_translator.vocabulary and k not in ("URL", "incoming_request_params"):
+                        # the remote server has sent a param
+                        # that the tool is not expecting -> drop it
+                        del params[k]
+        else:
+            if "runtool_btn" not in test_params:
+                error("Tool execution through the `tool_runner` requires a `runtool_btn` flag")
+
         # We may be visiting Galaxy for the first time ( e.g., sending data from UCSC ),
         # so make sure to create a new history if we've never had one before.
         history = tool.get_default_history_by_trans(trans, create=True)
         try:
-            vars = tool.handle_input(trans, params.__dict__, history=history)
+            vars = tool.handle_input(trans, params, history=history)
         except Exception as e:
             error(galaxy.util.unicodify(e))
         if len(params) > 0:
             trans.log_event(f"Tool params: {str(params)}", tool_id=tool_id)
         return trans.fill_template("root/tool_runner.mako", **vars)
 
     @web.expose
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/user.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/controllers/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -244,16 +244,15 @@
         delta = timedelta(hours=int(activation_grace_period))
         time_difference = datetime.utcnow() - create_time
         return time_difference > delta or activation_grace_period == 0
 
     @web.expose
     @web.json
     def logout(self, trans, logout_all=False, **kwd):
-        message = trans.check_csrf_token(kwd)
-        if message:
+        if message := trans.check_csrf_token(kwd):
             return self.message_exception(trans, message)
         # Since logging an event requires a session, we'll log prior to ending the session
         trans.log_event("User logged out")
         trans.handle_user_logout(logout_all=logout_all)
         success_response = {"message": "Success."}  # This is a little weird as a response.
         if trans.app.config.use_remote_user and trans.app.config.remote_user_logout_href:
             success_response["redirect_uri"] = trans.app.config.remote_user_logout_href
@@ -337,16 +336,15 @@
         trans.handle_user_login(user)
         return {"message": "Password has been changed."}
 
     @expose_api_anonymous_and_sessionless
     def reset_password(self, trans, payload=None, **kwd):
         """Reset the user's password. Send an email with token that allows a password change."""
         payload = payload or {}
-        message = self.user_manager.send_reset_email(trans, payload)
-        if message:
+        if message := self.user_manager.send_reset_email(trans, payload):
             return self.message_exception(trans, message)
         return {"message": "Reset link has been sent to your email."}
 
     def __get_redirect_url(self, redirect):
         if not redirect or redirect == "None":
             return None
         root_url = url_for("/", qualified=True)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/controllers/visualization.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/datasets.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,861 +1,1016 @@
+"""
+API operations on the contents of a history dataset.
+"""
+
 import logging
-from json import loads
+import os
+from enum import Enum
+from typing import (
+    Any,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+)
 
-from markupsafe import escape
-from paste.httpexceptions import (
-    HTTPBadRequest,
-    HTTPNotFound,
-)
-from sqlalchemy import (
-    desc,
-    false,
-    or_,
-    text,
-    true,
-)
-from sqlalchemy.orm import (
-    joinedload,
-    undefer,
+from pydantic import (
+    ConfigDict,
+    Field,
+    RootModel,
 )
+from starlette.datastructures import URL
 
 from galaxy import (
+    exceptions as galaxy_exceptions,
     model,
     util,
     web,
 )
-from galaxy.managers.hdas import HDAManager
-from galaxy.managers.sharable import SlugBuilder
+from galaxy.celery.tasks import compute_dataset_hash
+from galaxy.datatypes.binary import Binary
+from galaxy.datatypes.dataproviders.exceptions import NoProviderAvailable
+from galaxy.managers.base import ModelSerializer
+from galaxy.managers.context import ProvidesHistoryContext
+from galaxy.managers.datasets import (
+    DatasetAssociationManager,
+    DatasetManager,
+)
+from galaxy.managers.hdas import (
+    HDAManager,
+    HDASerializer,
+)
+from galaxy.managers.hdcas import HDCASerializer
+from galaxy.managers.histories import HistoryManager
+from galaxy.managers.history_contents import (
+    HistoryContentsFilters,
+    HistoryContentsManager,
+)
+from galaxy.managers.lddas import LDDAManager
 from galaxy.model.base import transaction
-from galaxy.model.item_attrs import (
-    UsesAnnotations,
-    UsesItemRatings,
-)
-from galaxy.structured_app import StructuredApp
-from galaxy.util import (
-    sanitize_text,
-    unicodify,
-)
-from galaxy.util.sanitize_html import sanitize_html
-from galaxy.visualization.data_providers.phyloviz import PhylovizDataProvider
-from galaxy.visualization.genomes import (
-    decode_dbkey,
-    GenomeRegion,
-)
-from galaxy.visualization.plugins import registry
-from galaxy.web.framework.helpers import (
-    grids,
-    time_ago,
-)
-from galaxy.webapps.base.controller import (
-    BaseUIController,
-    SharableMixin,
-    UsesVisualizationMixin,
+from galaxy.objectstore.badges import BadgeDict
+from galaxy.schema import (
+    FilterQueryParams,
+    SerializationParams,
+)
+from galaxy.schema.drs import (
+    AccessMethod,
+    AccessMethodType,
+    AccessURL,
+    Checksum,
+    DrsObject,
+)
+from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.schema import (
+    AnyHDA,
+    AnyHistoryContentItem,
+    AsyncTaskResultSummary,
+    DatasetAssociationRoles,
+    DatasetSourceId,
+    DatasetSourceType,
+    EncodedDatasetSourceId,
+    Model,
+    UpdateDatasetPermissionsPayload,
+)
+from galaxy.schema.tasks import ComputeDatasetHashTaskRequest
+from galaxy.schema.types import RelativeUrl
+from galaxy.security.idencoding import IdEncodingHelper
+from galaxy.util.hash_util import HashFunctionNameEnum
+from galaxy.util.path import safe_walk
+from galaxy.visualization.data_providers.genome import (
+    BamDataProvider,
+    FeatureLocationIndexDataProvider,
+    SamDataProvider,
+)
+from galaxy.visualization.data_providers.registry import DataProviderRegistry
+from galaxy.webapps.base.controller import UsesVisualizationMixin
+from galaxy.webapps.galaxy.services.base import (
+    async_task_summary,
+    ServiceBase,
 )
-from ..api import depends
 
 log = logging.getLogger(__name__)
 
+DEFAULT_LIMIT = 500
 
-#
-# -- Grids --
-#
-class HistoryDatasetsSelectionGrid(grids.Grid):
-    class DbKeyColumn(grids.GridColumn):
-        def filter(self, trans, user, query, dbkey):
-            """Filter by dbkey through a raw SQL b/c metadata is a BLOB."""
-            dbkey_user, dbkey = decode_dbkey(dbkey)
-            dbkey = dbkey.replace("'", "\\'")
-            return query.filter(
-                or_(text(f'metadata like \'%"dbkey": ["{dbkey}"]%\'', f'metadata like \'%"dbkey": "{dbkey}"%\''))
-            )
 
-    class HistoryColumn(grids.GridColumn):
-        def get_value(self, trans, grid, hda):
-            return escape(hda.history.name)
-
-        def sort(self, trans, query, ascending, column_name=None):
-            """Sort query using this column."""
-            return grids.GridColumn.sort(self, trans, query, ascending, column_name="history_id")
-
-    available_tracks = None
-    title = "Add Datasets"
-    model_class = model.HistoryDatasetAssociation
-    default_filter = {"deleted": "False", "shared": "All"}
-    default_sort_key = "-hid"
-    columns = [
-        grids.GridColumn("Id", key="hid"),
-        grids.TextColumn("Name", key="name", model_class=model.HistoryDatasetAssociation),
-        grids.TextColumn("Type", key="extension", model_class=model.HistoryDatasetAssociation),
-        grids.TextColumn("history_id", key="history_id", model_class=model.HistoryDatasetAssociation, visible=False),
-        HistoryColumn("History", key="history", visible=True),
-        DbKeyColumn("Build", key="dbkey", model_class=model.HistoryDatasetAssociation, visible=True, sortable=False),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search name and filetype",
-            cols_to_filter=[columns[1], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
+class RequestDataType(str, Enum):
+    """Particular pieces of information that can be requested for a dataset."""
+
+    state = "state"
+    converted_datasets_state = "converted_datasets_state"
+    data = "data"
+    features = "features"
+    raw_data = "raw_data"
+    track_config = "track_config"
+    genome_data = "genome_data"
+    in_use_state = "in_use_state"
+
+
+class DatasetContentType(str, Enum):
+    """For retrieving content from a structured dataset (e.g. HDF5)"""
+
+    meta = "meta"
+    attr = "attr"
+    stats = "stats"
+    data = "data"
+
+
+class ConcreteObjectStoreQuotaSourceDetails(Model):
+    source: Optional[str] = Field(
+        description="The quota source label corresponding to the object store the dataset is stored in (or would be stored in)"
+    )
+    enabled: bool = Field(
+        description="Whether the object store tracks quota on the data (independent of Galaxy's configuration)"
     )
 
-    def build_initial_query(self, trans, **kwargs):
-        return trans.sa_session.query(self.model_class).join(model.History.table).join(model.Dataset.table)
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        if self.available_tracks is None:
-            self.available_tracks = trans.app.datatypes_registry.get_available_tracks()
-        return (
-            query.filter(model.History.user == trans.user)
-            .filter(model.HistoryDatasetAssociation.extension.in_(self.available_tracks))
-            .filter(model.Dataset.state == model.Dataset.states.OK)
-            .filter(model.HistoryDatasetAssociation.deleted == false())
-            .filter(model.HistoryDatasetAssociation.visible == true())
-        )
+class DatasetStorageDetails(Model):
+    object_store_id: Optional[str] = Field(
+        description="The identifier of the destination ObjectStore for this dataset.",
+    )
+    name: Optional[str] = Field(
+        description="The display name of the destination ObjectStore for this dataset.",
+    )
+    description: Optional[str] = Field(
+        description="A description of how this dataset is stored.",
+    )
+    percent_used: Optional[float] = Field(
+        description="The percentage indicating how full the store is.",
+    )
+    dataset_state: str = Field(
+        description="The model state of the supplied dataset instance.",
+    )
+    hashes: List[dict] = Field(description="The file contents hashes associated with the supplied dataset instance.")
+    sources: List[dict] = Field(description="The file sources associated with the supplied dataset instance.")
+    shareable: bool = Field(
+        description="Is this dataset shareable.",
+    )
+    quota: ConcreteObjectStoreQuotaSourceDetails = Field(
+        description="Information about quota sources around dataset storage."
+    )
+    badges: List[BadgeDict] = Field(
+        description="A list of badges describing object store properties for concrete object store dataset is stored in."
+    )
+    relocatable: bool = Field(
+        description="Indicator of whether the objectstore for this dataset can be switched by this user."
+    )
 
 
-class LibraryDatasetsSelectionGrid(grids.Grid):
-    available_tracks = None
-    title = "Add Datasets"
-    model_class = model.LibraryDatasetDatasetAssociation
-    default_filter = {"deleted": "False"}
-    default_sort_key = "-id"
-    columns = [
-        grids.GridColumn("Id", key="id"),
-        grids.TextColumn("Name", key="name", model_class=model.LibraryDatasetDatasetAssociation),
-        grids.TextColumn("Type", key="extension", model_class=model.LibraryDatasetDatasetAssociation),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search name and filetype",
-            cols_to_filter=[columns[1], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
+class DatasetInheritanceChainEntry(Model):
+    name: str = Field(
+        description="Name of the referenced dataset",
+    )
+    dep: str = Field(
+        description="Name of the source of the referenced dataset at this point of the inheritance chain.",
     )
 
-    def build_initial_query(self, trans, **kwargs):
-        return trans.sa_session.query(self.model_class).join(model.Dataset.table)
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        if self.available_tracks is None:
-            self.available_tracks = trans.app.datatypes_registry.get_available_tracks()
-        return (
-            query.filter(model.LibraryDatasetDatasetAssociation.user == trans.user)
-            .filter(model.LibraryDatasetDatasetAssociation.extension.in_(self.available_tracks))
-            .filter(model.Dataset.state == model.Dataset.states.OK)
-            .filter(model.LibraryDatasetDatasetAssociation.deleted == false())
-            .filter(model.LibraryDatasetDatasetAssociation.visible == true())
-        )
+class DatasetInheritanceChain(RootModel):
+    root: List[DatasetInheritanceChainEntry] = Field(
+        default=[],
+        title="Dataset inheritance chain",
+    )
 
 
-class TracksterSelectionGrid(grids.Grid):
-    title = "Insert into visualization"
-    model_class = model.Visualization
-    default_sort_key = "-update_time"
-    use_paging = False
-    show_item_checkboxes = True
-    columns = [
-        grids.TextColumn("Title", key="title", model_class=model.Visualization, filterable="standard"),
-        grids.TextColumn("Build", key="dbkey", model_class=model.Visualization),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-
-    def build_initial_query(self, trans, **kwargs):
-        return trans.sa_session.query(self.model_class)
-
-    def apply_query_filter(self, trans, query, **kwargs):
-        return (
-            query.filter(self.model_class.user_id == trans.user.id)
-            .filter(self.model_class.deleted == false())
-            .filter(self.model_class.type == "trackster")
-        )
+class ExtraFilesEntryClass(str, Enum):
+    Directory = "Directory"
+    File = "File"
 
 
-class VisualizationListGrid(grids.Grid):
-    def get_url_args(item):
-        """
-        Returns dictionary used to create item link.
-        """
-        url_kwargs = dict(controller="visualization", id=item.id)
-        # TODO: hack to build link to saved visualization - need trans in this function instead in order to do
-        # link_data = trans.app.visualizations_registry.get_visualizations( trans, item )
-        if item.type in registry.VisualizationsRegistry.BUILT_IN_VISUALIZATIONS:
-            url_kwargs["action"] = item.type
-        else:
-            url_kwargs["__route_name__"] = "saved_visualization"
-            url_kwargs["visualization_name"] = item.type
-            url_kwargs["action"] = "saved"
-        return url_kwargs
-
-    def get_display_name(self, trans, item):
-        if trans.app.visualizations_registry and item.type in trans.app.visualizations_registry.plugins:
-            plugin = trans.app.visualizations_registry.plugins[item.type]
-            return plugin.config.get("name", item.type)
-        return item.type
-
-    # Grid definition
-    title = "Saved Visualizations"
-    model_class = model.Visualization
-    default_sort_key = "-update_time"
-    default_filter = dict(title="All", deleted="False", tags="All", sharing="All")
-    columns = [
-        grids.TextColumn("Title", key="title", attach_popup=True, link=get_url_args),
-        grids.TextColumn("Type", method="get_display_name"),
-        grids.TextColumn("Build", key="dbkey"),
-        grids.IndividualTagsColumn(
-            "Tags",
-            key="tags",
-            model_tag_association_class=model.VisualizationTagAssociation,
-            filterable="advanced",
-            grid_name="VisualizationListGrid",
-        ),
-        grids.SharingStatusColumn("Sharing", key="sharing", filterable="advanced", sortable=False),
-        grids.GridColumn("Created", key="create_time", format=time_ago),
-        grids.GridColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search",
-            cols_to_filter=[columns[0], columns[2]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
+class ExtraFileEntry(Model):
+    class_: ExtraFilesEntryClass = Field(
+        alias="class",  # Is a reserved word so cannot be directly used as field
+        description="The class of this entry, either File or Directory.",
+    )
+    path: str = Field(
+        description="Relative path to the file or directory.",
     )
-    operations = [
-        grids.GridOperation("Open", allow_multiple=False, url_args=get_url_args),
-        grids.GridOperation(
-            "Edit Attributes", allow_multiple=False, url_args=dict(controller="", action="visualizations/edit")
-        ),
-        grids.GridOperation("Copy", allow_multiple=False, condition=(lambda item: not item.deleted)),
-        grids.GridOperation(
-            "Share or Publish",
-            allow_multiple=False,
-            condition=(lambda item: not item.deleted),
-            url_args=dict(controller="", action="visualizations/sharing"),
-        ),
-        grids.GridOperation(
-            "Delete",
-            condition=(lambda item: not item.deleted),
-            confirm="Are you sure you want to delete this visualization?",
-        ),
-    ]
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter_by(user=trans.user, deleted=False)
 
+class DatasetExtraFiles(RootModel):
+    """A list of extra files associated with a dataset."""
 
-class VisualizationAllPublishedGrid(grids.Grid):
-    # Grid definition
-    use_panels = True
-    title = "Published Visualizations"
-    model_class = model.Visualization
-    default_sort_key = "update_time"
-    default_filter = dict(title="All", username="All")
-    columns = [
-        grids.PublicURLColumn("Title", key="title", filterable="advanced"),
-        grids.OwnerAnnotationColumn(
-            "Annotation",
-            key="annotation",
-            model_annotation_association_class=model.VisualizationAnnotationAssociation,
-            filterable="advanced",
-        ),
-        grids.OwnerColumn("Owner", key="username", model_class=model.User, filterable="advanced"),
-        grids.CommunityRatingColumn("Community Rating", key="rating"),
-        grids.CommunityTagsColumn(
-            "Community Tags",
-            key="tags",
-            model_tag_association_class=model.VisualizationTagAssociation,
-            filterable="advanced",
-            grid_name="VisualizationAllPublishedGrid",
+    root: List[ExtraFileEntry]
+
+
+class DatasetTextContentDetails(Model):
+    item_data: Optional[str] = Field(
+        description="First chunk of text content (maximum 1MB) of the dataset.",
+    )
+    truncated: bool = Field(
+        description="Whether the text in `item_data` has been truncated or contains the whole contents.",
+    )
+    item_url: RelativeUrl = Field(
+        description="URL to access this dataset.",
+    )
+
+
+class ConvertedDatasetsMap(RootModel):
+    """Map of `file extension` -> `converted dataset encoded id`"""
+
+    root: Dict[str, DecodedDatabaseIdField]  # extension -> dataset ID
+    model_config = ConfigDict(
+        json_schema_extra={
+            "example": {
+                "csv": "dataset_id",
+            }
+        }
+    )
+
+
+class DataMode(str, Enum):
+    Coverage = "Coverage"
+    Auto = "Auto"
+
+
+class DataResult(Model):
+    data: List[Any]
+    dataset_type: Optional[str] = None
+    message: Optional[str] = None
+    extra_info: Optional[Any] = None  # Seems to be always None, deprecate?
+
+
+class BamDataResult(DataResult):
+    max_low: int
+    max_high: int
+
+
+class DeleteDatasetBatchPayload(Model):
+    datasets: List[DatasetSourceId] = Field(
+        description="The list of datasets IDs with their sources to be deleted/purged.",
+    )
+    purge: Optional[bool] = Field(
+        default=False,
+        description=(
+            "Whether to permanently delete from disk the specified datasets. "
+            "*Warning*: this is a destructive operation."
         ),
-        grids.ReverseSortColumn("Last Updated", key="update_time", format=time_ago),
-    ]
-    columns.append(
-        grids.MulticolFilterColumn(
-            "Search title, annotation, owner, and tags",
-            cols_to_filter=[columns[0], columns[1], columns[2], columns[4]],
-            key="free-text-search",
-            visible=False,
-            filterable="standard",
-        )
     )
 
-    def build_initial_query(self, trans, **kwargs):
-        # See optimization description comments and TODO for tags in matching public histories query.
-        return (
-            trans.sa_session.query(self.model_class)
-            .join(self.model_class.user)
-            .options(
-                joinedload(self.model_class.user).load_only("username"),
-                joinedload(self.model_class.annotations),
-                undefer("average_rating"),
-            )
-        )
 
-    def apply_query_filter(self, trans, query, **kwargs):
-        return query.filter(self.model_class.deleted == false()).filter(self.model_class.published == true())
+class ComputeDatasetHashPayload(Model):
+    hash_function: Optional[HashFunctionNameEnum] = Field(
+        default=HashFunctionNameEnum.md5, description="Hash function name to use to compute dataset hashes."
+    )
+    extra_files_path: Optional[str] = Field(default=None, description="If set, extra files path to compute a hash for.")
+    model_config = ConfigDict(use_enum_values=True)
+
+
+class UpdateObjectStoreIdPayload(Model):
+    object_store_id: str = Field(
+        ...,
+        description="Object store ID to update to, it must be an object store with the same device ID as the target dataset currently.",
+    )
+
+
+class DatasetErrorMessage(Model):
+    dataset: EncodedDatasetSourceId = Field(
+        description="The encoded ID of the dataset and its source.",
+    )
+    error_message: str = Field(
+        description="The error message returned while processing this dataset.",
+    )
+
+
+class DeleteDatasetBatchResult(Model):
+    success_count: int = Field(
+        description="The number of datasets successfully processed.",
+    )
+    errors: Optional[List[DatasetErrorMessage]] = Field(
+        default=None,
+        description=(
+            "A list of dataset IDs and the corresponding error message if something "
+            "went wrong while processing the dataset."
+        ),
+    )
 
 
-class VisualizationController(
-    BaseUIController, SharableMixin, UsesVisualizationMixin, UsesAnnotations, UsesItemRatings
-):
-    _visualization_list_grid = VisualizationListGrid()
-    _published_list_grid = VisualizationAllPublishedGrid()
-    _history_datasets_grid = HistoryDatasetsSelectionGrid()
-    _library_datasets_grid = LibraryDatasetsSelectionGrid()
-    _tracks_grid = TracksterSelectionGrid()
-    hda_manager: HDAManager = depends(HDAManager)
-    slug_builder: SlugBuilder = depends(SlugBuilder)
-
-    def __init__(self, app: StructuredApp):
-        super().__init__(app)
-
-    #
-    # -- Functions for listing visualizations. --
-    #
-
-    @web.expose
-    @web.json
-    @web.require_login("see all available libraries")
-    def list_libraries(self, trans, **kwargs):
-        """List all libraries that can be used for selecting datasets."""
-        return self._libraries_grid(trans, **kwargs)
-
-    @web.expose
-    @web.json
-    @web.require_login("see a history's datasets that can added to this visualization")
-    def list_history_datasets(self, trans, **kwargs):
-        """List a history's datasets that can be added to a visualization."""
-        kwargs["show_item_checkboxes"] = "True"
-        return self._history_datasets_grid(trans, **kwargs)
-
-    @web.expose
-    @web.json
-    @web.require_login("see a history's datasets that can added to this visualization")
-    def list_library_datasets(self, trans, **kwargs):
-        """List a library's datasets that can be added to a visualization."""
-        kwargs["show_item_checkboxes"] = "True"
-        return self._library_datasets_grid(trans, **kwargs)
-
-    @web.expose
-    @web.json
-    def list_tracks(self, trans, **kwargs):
-        return self._tracks_grid(trans, **kwargs)
-
-    @web.expose
-    @web.json
-    def list_published(self, trans, *args, **kwargs):
-        grid = self._published_list_grid(trans, **kwargs)
-        grid["shared_by_others"] = self._get_shared(trans)
-        return grid
-
-    @web.legacy_expose_api
-    @web.require_login("use Galaxy visualizations", use_panels=True)
-    def list(self, trans, **kwargs):
-        message = kwargs.get("message")
-        status = kwargs.get("status")
-        if "operation" in kwargs and "id" in kwargs:
-            session = trans.sa_session
-            operation = kwargs["operation"].lower()
-            ids = util.listify(kwargs["id"])
-            for id in ids:
-                if operation == "delete":
-                    item = self.get_visualization(trans, id)
-                    item.deleted = True
-                if operation == "copy":
-                    self.copy(trans, **kwargs)
-            with transaction(session):
-                session.commit()
-        kwargs["embedded"] = True
-        if message and status:
-            kwargs["message"] = sanitize_text(message)
-            kwargs["status"] = status
-        grid = self._visualization_list_grid(trans, **kwargs)
-        grid["shared_by_others"] = self._get_shared(trans)
-        return grid
-
-    def _get_shared(self, trans):
-        """Identify shared visualizations"""
-        shared_by_others = (
-            trans.sa_session.query(model.VisualizationUserShareAssociation)
-            .filter_by(user=trans.get_user())
-            .join(model.Visualization.table)
-            .filter(model.Visualization.deleted == false())
-            .order_by(desc(model.Visualization.update_time))
-            .all()
+class DatasetsService(ServiceBase, UsesVisualizationMixin):
+    def __init__(
+        self,
+        security: IdEncodingHelper,
+        history_manager: HistoryManager,
+        hda_manager: HDAManager,
+        hda_serializer: HDASerializer,
+        hdca_serializer: HDCASerializer,
+        ldda_manager: LDDAManager,
+        history_contents_manager: HistoryContentsManager,
+        history_contents_filters: HistoryContentsFilters,
+        data_provider_registry: DataProviderRegistry,
+        dataset_manager: DatasetManager,
+    ):
+        super().__init__(security)
+        self.history_manager = history_manager
+        self.hda_manager = hda_manager
+        self.hda_serializer = hda_serializer
+        self.hdca_serializer = hdca_serializer
+        self.ldda_manager = ldda_manager
+        self.history_contents_manager = history_contents_manager
+        self.history_contents_filters = history_contents_filters
+        self.data_provider_registry = data_provider_registry
+        self.dataset_manager = dataset_manager
+
+    @property
+    def serializer_by_type(self) -> Dict[str, ModelSerializer]:
+        return {"dataset": self.hda_serializer, "dataset_collection": self.hdca_serializer}
+
+    @property
+    def dataset_manager_by_type(self) -> Dict[str, DatasetAssociationManager]:
+        return {"hda": self.hda_manager, "ldda": self.ldda_manager}
+
+    def index(
+        self,
+        trans: ProvidesHistoryContext,
+        history_id: Optional[DecodedDatabaseIdField],
+        serialization_params: SerializationParams,
+        filter_query_params: FilterQueryParams,
+    ) -> List[AnyHistoryContentItem]:
+        """
+        Search datasets or collections using a query system and returns a list
+        containing summary of dataset or dataset_collection information.
+        """
+        user = self.get_authenticated_user(trans)
+        filters = self.history_contents_filters.parse_query_filters(filter_query_params)
+        serialization_params.default_view = "summary"
+        order_by = self.build_order_by(self.history_contents_manager, filter_query_params.order or "create_time-dsc")
+        container = None
+        if history_id:
+            container = self.history_manager.get_accessible(history_id, user)
+        contents = self.history_contents_manager.contents(
+            container=container,
+            filters=filters,
+            limit=filter_query_params.limit or DEFAULT_LIMIT,
+            offset=filter_query_params.offset,
+            order_by=order_by,
+            user_id=user.id,
         )
         return [
-            {"username": v.visualization.user.username, "slug": v.visualization.slug, "title": v.visualization.title}
-            for v in shared_by_others
+            self.serializer_by_type[content.history_content_type].serialize_to_view(
+                content, user=user, trans=trans, encode_id=False, **serialization_params.model_dump()
+            )
+            for content in contents
         ]
 
-    #
-    # -- Functions for operating on visualizations. --
-    #
-
-    @web.expose
-    @web.require_login("use Galaxy visualizations", use_panels=True)
-    def index(self, trans, *args, **kwargs):
-        """Lists user's saved visualizations."""
-        return self.list(trans, *args, **kwargs)
-
-    @web.expose
-    @web.require_login()
-    def copy(self, trans, id, **kwargs):
-        visualization = self.get_visualization(trans, id, check_ownership=False, check_accessible=True)
-        user = trans.get_user()
-        owner = visualization.user == user
-        new_title = f"Copy of '{visualization.title}'"
-        if not owner:
-            new_title += f" shared by {visualization.user.email}"
-
-        copied_viz = visualization.copy(user=trans.user, title=new_title)
-
-        # Persist
-        session = trans.sa_session
-        session.add(copied_viz)
-        with transaction(session):
-            session.commit()
-
-        # Display the management page
-        trans.set_message(f'Created new visualization with name "{copied_viz.title}"')
-        return
-
-    @web.expose
-    @web.require_login("share Galaxy visualizations")
-    def imp(self, trans, id, **kwargs):
-        """Import a visualization into user's workspace."""
-        # Set referer message.
-        referer = trans.request.referer
-        if referer and not referer.startswith(f"{trans.request.application_url}{web.url_for('/login')}"):
-            referer_message = f"<a href='{escape(referer)}'>return to the previous page</a>"
+    def show(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        hda_ldda: DatasetSourceType,
+        serialization_params: SerializationParams,
+        data_type: Optional[RequestDataType] = None,
+        **extra_params,
+    ):
+        """
+        Displays information about and/or content of a dataset.
+        """
+        dataset = self.dataset_manager_by_type[hda_ldda].get_accessible(dataset_id, trans.user)
+
+        # Use data type to return particular type of data.
+        rval: Any
+        if data_type == RequestDataType.state:
+            rval = self._dataset_state(dataset)
+        elif data_type == RequestDataType.converted_datasets_state:
+            rval = self._converted_datasets_state(
+                trans,
+                dataset,
+                chrom=extra_params.get("chrom", None),
+                retry=extra_params.get("retry", False),
+            )
+        elif data_type == RequestDataType.data:
+            rval = self._data(trans, dataset, **extra_params)
+        elif data_type == RequestDataType.features:
+            rval = self._search_features(trans, dataset, query=extra_params.get("query", None))
+        elif data_type == RequestDataType.raw_data:
+            rval = self._raw_data(trans, dataset, **extra_params)
+        elif data_type == RequestDataType.track_config:
+            rval = self.get_new_track_config(trans, dataset)
+        elif data_type == RequestDataType.genome_data:
+            rval = self._get_genome_data(trans, dataset, dbkey=extra_params.get("dbkey", None))
+        elif data_type == RequestDataType.in_use_state:
+            rval = self._dataset_in_use_state(dataset)
+        else:
+            # Default: return dataset as dict.
+            if hda_ldda == DatasetSourceType.hda:
+                return self.hda_serializer.serialize_to_view(
+                    dataset, view=serialization_params.view or "detailed", user=trans.user, trans=trans
+                )
+            else:
+                dataset_dict = dataset.to_dict()
+                rval = self.encode_all_ids(dataset_dict)
+        return rval
+
+    def show_storage(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        hda_ldda: DatasetSourceType = DatasetSourceType.hda,
+    ) -> DatasetStorageDetails:
+        """
+        Display user-facing storage details related to the objectstore a
+        dataset resides in.
+        """
+        dataset_instance = self.dataset_manager_by_type[hda_ldda].get_accessible(dataset_id, trans.user)
+        dataset = dataset_instance.dataset
+        object_store = trans.app.object_store
+        object_store_id = dataset.object_store_id
+        name = object_store.get_concrete_store_name(dataset)
+        description = object_store.get_concrete_store_description_markdown(dataset)
+        badges = object_store.get_concrete_store_badges(dataset)
+        # not really working (existing problem)
+        try:
+            percent_used = object_store.get_store_usage_percent()
+        except AttributeError:
+            # not implemented on nestedobjectstores yet.
+            percent_used = None
+        except FileNotFoundError:
+            # uninitialized directory (empty) disk object store can cause this...
+            percent_used = None
+
+        quota_source = dataset.quota_source_info
+        quota = ConcreteObjectStoreQuotaSourceDetails(
+            source=quota_source.label,
+            enabled=quota_source.use,
+        )
+        relocatable = trans.app.security_agent.can_change_object_store_id(trans.user, dataset)
+        dataset_state = dataset.state
+        hashes = [h.to_dict() for h in dataset.hashes]
+        sources = [s.to_dict() for s in dataset.sources]
+        return DatasetStorageDetails(
+            object_store_id=object_store_id,
+            shareable=dataset.shareable,
+            name=name,
+            description=description,
+            percent_used=percent_used,
+            dataset_state=dataset_state,
+            hashes=hashes,
+            sources=sources,
+            quota=quota,
+            badges=badges,
+            relocatable=relocatable,
+        )
+
+    def show_inheritance_chain(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        hda_ldda: DatasetSourceType = DatasetSourceType.hda,
+    ) -> DatasetInheritanceChain:
+        """
+        Display inheritance chain for the given dataset.
+        """
+        dataset_instance = self.dataset_manager_by_type[hda_ldda].get_accessible(dataset_id, trans.user)
+        inherit_chain = dataset_instance.source_dataset_chain
+        result = []
+        for dep in inherit_chain:
+            result.append(DatasetInheritanceChainEntry(name=f"{dep[0].name}", dep=dep[1]))
+
+        return DatasetInheritanceChain(root=result)
+
+    def compute_hash(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        payload: ComputeDatasetHashPayload,
+        hda_ldda: DatasetSourceType = DatasetSourceType.hda,
+    ) -> AsyncTaskResultSummary:
+        dataset_instance = self.dataset_manager_by_type[hda_ldda].get_accessible(dataset_id, trans.user)
+        request = ComputeDatasetHashTaskRequest(
+            dataset_id=dataset_instance.dataset.id,
+            extra_files_path=payload.extra_files_path,
+            hash_function=payload.hash_function,
+            user=trans.async_request_user,
+        )
+        result = compute_dataset_hash.delay(request=request, task_user_id=getattr(trans.user, "id", None))
+        return async_task_summary(result)
+
+    def drs_dataset_instance(self, object_id: str) -> Tuple[int, DatasetSourceType]:
+        if object_id.startswith("hda-"):
+            decoded_object_id = self.decode_id(object_id[len("hda-") :], kind="drs")
+            hda_ldda = DatasetSourceType.hda
+        elif object_id.startswith("ldda-"):
+            decoded_object_id = self.decode_id(object_id[len("ldda-") :], kind="drs")
+            hda_ldda = DatasetSourceType.ldda
         else:
-            referer_message = f"<a href='{web.url_for('/')}'>go to Galaxy's start page</a>"
+            raise galaxy_exceptions.RequestParameterInvalidException(
+                "Invalid object_id format specified for this Galaxy server"
+            )
+        return decoded_object_id, hda_ldda
 
-        # Do import.
-        session = trans.sa_session
-        visualization = self.get_visualization(trans, id, check_ownership=False, check_accessible=True)
-        if visualization.importable is False:
-            return trans.show_error_message(
-                f"The owner of this visualization has disabled imports via this link.<br>You can {referer_message}",
-                use_panels=True,
+    def get_drs_object(self, trans: ProvidesHistoryContext, object_id: str, request_url: URL) -> DrsObject:
+        decoded_object_id, hda_ldda = self.drs_dataset_instance(object_id)
+        dataset_instance = self.dataset_manager_by_type[hda_ldda].get_accessible(decoded_object_id, trans.user)
+        if not trans.app.security_agent.dataset_is_public(dataset_instance.dataset):
+            # Only public datasets may be access as DRS datasets currently
+            raise galaxy_exceptions.ObjectNotFound("Cannot find a public dataset with specified object ID.")
+
+        # TODO: issue warning if not being served on HTTPS @ 443 - required by the spec.
+        self_uri = f"drs://drs.{request_url.components.netloc}/{object_id}"
+        checksums: List[Checksum] = []
+        for dataset_hash in dataset_instance.dataset.hashes:
+            if dataset_hash.extra_files_path:
+                continue
+            type = dataset_hash.hash_function
+            checksum = dataset_hash.hash_value
+            checksums.append(Checksum(type=type, checksum=checksum))
+
+        if len(checksums) == 0:
+            hash_funciton = HashFunctionNameEnum.md5
+            request = ComputeDatasetHashTaskRequest(
+                dataset_id=dataset_instance.dataset.id,
+                extra_files_path=None,
+                hash_function=hash_funciton,
+                user=None,
             )
-        elif visualization.deleted:
-            return trans.show_error_message(
-                f"You can't import this visualization because it has been deleted.<br>You can {referer_message}",
-                use_panels=True,
+            compute_dataset_hash.delay(request=request, task_user_id=getattr(trans.user, "id", None))
+            raise galaxy_exceptions.AcceptedRetryLater(
+                "required checksum task for DRS object response launched.", retry_after=60
             )
-        else:
-            # Create imported visualization via copy.
-            #   TODO: need to handle custom db keys.
 
-            imported_visualization = visualization.copy(user=trans.user, title=f"imported: {visualization.title}")
+        base = str(request_url).split("/ga4gh", 1)[0]
+        access_url = base + f"/api/drs_download/{object_id}"
 
-            # Persist
-            session = trans.sa_session
-            session.add(imported_visualization)
-            with transaction(session):
-                session.commit()
-
-            # Redirect to load galaxy frames.
-            return trans.show_ok_message(
-                message="""Visualization "{}" has been imported. <br>You can <a href="{}">start using this visualization</a> or {}.""".format(
-                    visualization.title, web.url_for("/visualizations/list"), referer_message
-                ),
-                use_panels=True,
-            )
+        access_method = AccessMethod(
+            type=AccessMethodType.https,
+            access_url=AccessURL(url=access_url),
+        )
+
+        return DrsObject(
+            id=object_id,
+            self_uri=self_uri,
+            size=dataset_instance.dataset.file_size,
+            created_time=dataset_instance.create_time,
+            checksums=checksums,
+            access_methods=[access_method],
+        )
+
+    def update_permissions(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        payload: UpdateDatasetPermissionsPayload,
+        hda_ldda: DatasetSourceType = DatasetSourceType.hda,
+    ) -> DatasetAssociationRoles:
+        """
+        Updates permissions of a dataset.
+        """
+        self.check_user_is_authenticated(trans)
+        payload_dict = payload.model_dump(by_alias=True)
+        dataset_manager = self.dataset_manager_by_type[hda_ldda]
+        dataset = dataset_manager.get_accessible(dataset_id, trans.user)
+        dataset_manager.update_permissions(trans, dataset, **payload_dict)
+        return dataset_manager.serialize_dataset_association_roles(trans, dataset)
+
+    def extra_files(
+        self,
+        trans: ProvidesHistoryContext,
+        history_content_id: DecodedDatabaseIdField,
+    ):
+        """
+        Generate list of extra files.
+        """
+        hda = self.hda_manager.get_accessible(history_content_id, trans.user)
+        rval = []
+        if not hda.is_pending and hda.extra_files_path_exists():
+            extra_files_path = hda.extra_files_path
+            for root, directories, files in safe_walk(extra_files_path):
+                for directory in directories:
+                    rval.append(
+                        {"class": "Directory", "path": os.path.relpath(os.path.join(root, directory), extra_files_path)}
+                    )
+                for file in files:
+                    rval.append({"class": "File", "path": os.path.relpath(os.path.join(root, file), extra_files_path)})
 
-    @web.expose
-    def display_by_username_and_slug(self, trans, username, slug, **kwargs):
-        """Display visualization based on a username and slug."""
-
-        # Get visualization.
-        session = trans.sa_session
-        user = session.query(model.User).filter_by(username=username).first()
-        visualization = (
-            trans.sa_session.query(model.Visualization).filter_by(user=user, slug=slug, deleted=False).first()
-        )
-        if visualization is None:
-            raise web.httpexceptions.HTTPNotFound()
+        return rval
 
-        # Security check raises error if user cannot access visualization.
-        self.security_check(trans, visualization, check_ownership=False, check_accessible=True)
+    def display(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        hda_ldda: DatasetSourceType = DatasetSourceType.hda,
+        preview: bool = False,
+        filename: Optional[str] = None,
+        to_ext: Optional[str] = None,
+        raw: bool = False,
+        offset: Optional[int] = None,
+        ck_size: Optional[int] = None,
+        **kwd,
+    ):
+        """
+        Displays history content (dataset).
+
+        The query parameter 'raw' should be considered experimental and may be dropped at
+        some point in the future without warning. Generally, data should be processed by its
+        datatype prior to display (the default if raw is unspecified or explicitly false.
+        """
+        headers = {}
+        rval: Any = ""
+        try:
+            dataset_instance = self.dataset_manager_by_type[hda_ldda].get_accessible(dataset_id, trans.user)
+            if raw:
+                if filename and filename != "index":
+                    object_store = trans.app.object_store
+                    dir_name = dataset_instance.dataset.extra_files_path_name
+                    file_path = object_store.get_filename(
+                        dataset_instance.dataset, extra_dir=dir_name, alt_name=filename
+                    )
+                else:
+                    file_path = dataset_instance.get_file_name()
+                rval = open(file_path, "rb")
+            else:
+                if offset is not None:
+                    kwd["offset"] = offset
+                if ck_size is not None:
+                    kwd["ck_size"] = ck_size
+                rval, headers = dataset_instance.datatype.display_data(
+                    trans, dataset_instance, preview, filename, to_ext, **kwd
+                )
+        except galaxy_exceptions.MessageException:
+            raise
+        except Exception as e:
+            raise galaxy_exceptions.InternalServerError(f"Could not get display data for dataset: {util.unicodify(e)}")
+        return rval, headers
+
+    def get_content_as_text(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+    ) -> DatasetTextContentDetails:
+        """Returns dataset content as Text."""
+        user = trans.user
+        hda = self.hda_manager.get_accessible(dataset_id, user)
+        hda = self.hda_manager.error_if_uploading(hda)
+        truncated, dataset_data = self.hda_manager.text_data(hda, preview=True)
+        item_url = web.url_for(
+            controller="dataset",
+            action="display_by_username_and_slug",
+            username=hda.user and hda.user.username,
+            slug=self.encode_id(hda.id),
+            preview=False,
+        )
+        return DatasetTextContentDetails(
+            item_data=dataset_data,
+            truncated=truncated,
+            item_url=item_url,
+        )
+
+    def get_metadata_file(
+        self,
+        trans: ProvidesHistoryContext,
+        history_content_id: DecodedDatabaseIdField,
+        metadata_file: str,
+        open_file: bool = False,
+    ):
+        """
+        Gets the associated metadata file.
+
+        The `open_file` parameter determines if we return the path of the file or the opened file handle.
+        TODO: Remove the `open_file` parameter when removing the associated legacy endpoint.
+        """
+        hda = self.hda_manager.get_accessible(history_content_id, trans.user)
+        file_ext = hda.metadata.spec.get(metadata_file).get("file_ext", metadata_file)
+        fname = "".join(c in util.FILENAME_VALID_CHARS and c or "_" for c in hda.name)[0:150]
+        headers = {}
+        headers["Content-Type"] = "application/octet-stream"
+        headers["Content-Disposition"] = f'attachment; filename="Galaxy{hda.hid}-[{fname}].{file_ext}"'
+        file_path = hda.metadata.get(metadata_file).get_file_name()
+        if open_file:
+            return open(file_path, "rb"), headers
+        return file_path, headers
+
+    def converted_ext(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        ext: str,
+        serialization_params: SerializationParams,
+    ) -> AnyHDA:
+        """
+        Return information about datasets made by converting this dataset to a new format
+        """
+        hda = self.hda_manager.get_accessible(dataset_id, trans.user)
+        serialization_params.default_view = "detailed"
+        converted = self._get_or_create_converted(trans, hda, ext)
+        return self.hda_serializer.serialize_to_view(
+            converted, user=trans.user, trans=trans, **serialization_params.model_dump()
+        )
+
+    def converted(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+    ) -> ConvertedDatasetsMap:
+        """
+        Return a `file extension` -> `converted dataset encoded id` map
+        with all the existing converted datasets associated with this instance.
+        """
+        hda = self.hda_manager.get_accessible(dataset_id, trans.user)
+        return self.hda_serializer.serialize_converted_datasets(hda, "converted")
+
+    def delete_batch(
+        self,
+        trans: ProvidesHistoryContext,
+        payload: DeleteDatasetBatchPayload,
+    ) -> DeleteDatasetBatchResult:
+        """
+        Deletes or purges a batch of datasets.
+        Warning: only the ownership of the dataset and upload state for HDAs is checked, no other checks or restrictions are made.
+        """
+        success_count = 0
+        errors: List[DatasetErrorMessage] = []
+        for dataset in payload.datasets:
+            try:
+                manager = self.dataset_manager_by_type[dataset.src]
+                dataset_instance = manager.get_owned(dataset.id, trans.user)
+                manager.error_unless_mutable(dataset_instance.history)
+                if dataset.src == DatasetSourceType.hda:
+                    self.hda_manager.error_if_uploading(dataset_instance)
+                if payload.purge:
+                    manager.purge(dataset_instance, flush=True)
+                else:
+                    manager.delete(dataset_instance, flush=False)
+                success_count += 1
+            except galaxy_exceptions.MessageException as e:
+                errors.append(
+                    DatasetErrorMessage(
+                        dataset=EncodedDatasetSourceId(id=dataset.id, src=dataset.src),
+                        error_message=str(e),
+                    )
+                )
 
-        # Encode page identifier.
-        visualization_id = trans.security.encode_id(visualization.id)
+        if success_count:
+            with transaction(trans.sa_session):
+                trans.sa_session.commit()
+        return DeleteDatasetBatchResult.model_construct(success_count=success_count, errors=errors)
+
+    def get_structured_content(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset_id: DecodedDatabaseIdField,
+        content_type: DatasetContentType,
+        **params,
+    ):
+        """
+        Retrieves contents of a dataset. It is left to the datatype to decide how
+        to interpret the content types.
+        """
+        headers = {}
+        content: Any = ""
+        dataset = self.hda_manager.get_accessible(dataset_id, trans.user)
+        if not isinstance(dataset.datatype, Binary):
+            raise galaxy_exceptions.InvalidFileFormatError("Only available for structured datatypes")
+        try:
+            content, headers = dataset.datatype.get_structured_content(dataset, content_type, **params)
+        except galaxy_exceptions.MessageException:
+            raise
+        except Exception as e:
+            raise galaxy_exceptions.InternalServerError(f"Could not get content for dataset: {util.unicodify(e)}")
+        return content, headers
+
+    def update_object_store_id(self, trans, dataset_id: DecodedDatabaseIdField, payload: UpdateObjectStoreIdPayload):
+        hda = self.hda_manager.get_accessible(dataset_id, trans.user)
+        dataset = hda.dataset
+        self.dataset_manager.update_object_store_id(trans, dataset, payload.object_store_id)
 
-        # Redirect to client.
-        return trans.response.send_redirect(
-            web.url_for(
-                controller="published",
-                action="visualization",
-                id=visualization_id,
+    def _get_or_create_converted(self, trans, original: model.DatasetInstance, target_ext: str):
+        try:
+            original.get_converted_dataset(trans, target_ext)
+            converted = original.get_converted_files_by_type(target_ext)
+            return converted
+
+        except model.NoConverterException:
+            exc_data = dict(
+                source=original.ext, target=target_ext, available=list(original.get_converter_types().keys())
             )
-        )
+            raise galaxy_exceptions.RequestParameterInvalidException("Conversion not possible", **exc_data)
 
-    @web.json
-    def save(self, trans, vis_json=None, type=None, id=None, title=None, dbkey=None, annotation=None, **kwargs):
+    def _dataset_in_use_state(self, dataset: model.DatasetInstance) -> bool:
         """
-        Save a visualization; if visualization does not have an ID, a new
-        visualization is created. Returns JSON of visualization.
+        Return True if dataset is currently used as an input or output. False otherwise.
         """
-        # Get visualization attributes from kwargs or from config.
-        vis_config = loads(vis_json)
-        vis_type = type or vis_config["type"]
-        vis_id = id or vis_config.get("id", None)
-        vis_title = title or vis_config.get("title", None)
-        vis_dbkey = dbkey or vis_config.get("dbkey", None)
-        vis_annotation = annotation or vis_config.get("annotation", None)
-        return self.save_visualization(trans, vis_config, vis_type, vis_id, vis_title, vis_dbkey, vis_annotation)
-
-    @web.legacy_expose_api
-    @web.require_login("edit visualizations")
-    def edit(self, trans, payload=None, **kwd):
-        """
-        Edit a visualization's attributes.
-        """
-        id = kwd.get("id")
-        if not id:
-            return self.message_exception(trans, "No visualization id received for editing.")
-        trans_user = trans.get_user()
-        v = self.get_visualization(trans, id, check_ownership=True)
-        if trans.request.method == "GET":
-            if v.slug is None:
-                self.slug_builder.create_item_slug(trans.sa_session, v)
-            return {
-                "title": "Edit visualization attributes",
-                "inputs": [
-                    {"name": "title", "label": "Name", "value": v.title},
-                    {
-                        "name": "slug",
-                        "label": "Identifier",
-                        "value": v.slug,
-                        "help": "A unique identifier that will be used for public links to this visualization. This field can only contain lowercase letters, numbers, and dashes (-).",
-                    },
-                    {
-                        "name": "dbkey",
-                        "label": "Build",
-                        "type": "select",
-                        "optional": True,
-                        "value": v.dbkey,
-                        "options": trans.app.genomes.get_dbkeys(trans_user, chrom_info=True),
-                        "help": "Parameter to associate your visualization with a database key.",
-                    },
-                    {
-                        "name": "annotation",
-                        "label": "Annotation",
-                        "value": self.get_item_annotation_str(trans.sa_session, trans.user, v),
-                        "help": "A description of the visualization. The annotation is shown alongside published visualizations.",
-                    },
-                ],
-            }
-        else:
-            v_title = payload.get("title")
-            v_slug = payload.get("slug")
-            v_dbkey = payload.get("dbkey")
-            v_annotation = payload.get("annotation")
-            if not v_title:
-                return self.message_exception(trans, "Please provide a visualization name is required.")
-            elif not v_slug:
-                return self.message_exception(trans, "Please provide a unique identifier.")
-            elif not self._is_valid_slug(v_slug):
-                return self.message_exception(
-                    trans, "Visualization identifier can only contain lowercase letters, numbers, and dashes (-)."
-                )
-            elif (
-                v_slug != v.slug
-                and trans.sa_session.query(model.Visualization)
-                .filter_by(user=v.user, slug=v_slug, deleted=False)
-                .first()
-            ):
-                return self.message_exception(trans, "Visualization id must be unique.")
-            else:
-                v.title = v_title
-                v.slug = v_slug
-                v.dbkey = v_dbkey
-                if v_annotation:
-                    v_annotation = sanitize_html(v_annotation)
-                    self.add_item_annotation(trans.sa_session, trans_user, v, v_annotation)
-                trans.sa_session.add(v)
-                with transaction(trans.sa_session):
-                    trans.sa_session.commit()
-            return {"message": "Attributes of '%s' successfully saved." % v.title, "status": "success"}
-
-    # ------------------------- registry.
-    @web.expose
-    @web.require_login("use Galaxy visualizations", use_panels=True)
-    def render(self, trans, visualization_name, embedded=None, **kwargs):
-        """
-        Render the appropriate visualization template, parsing the `kwargs`
-        into appropriate variables and resources (such as ORM models)
-        based on this visualizations `param` data in visualizations_conf.xml.
+        return not dataset.ok_to_edit_metadata()
 
-        URL: /visualization/show/{visualization_name}
+    def _dataset_state(self, dataset: model.DatasetInstance) -> model.Dataset.conversion_messages:
         """
-        plugin = self._get_plugin_from_registry(trans, visualization_name)
-        try:
-            return plugin.render(trans=trans, embedded=embedded, **kwargs)
-        except Exception as exception:
-            self._handle_plugin_error(trans, visualization_name, exception)
-
-    def _get_plugin_from_registry(self, trans, visualization_name):
-        """
-        Get the named plugin from the registry.
-        :raises HTTPNotFound: if registry has been turned off in config.
-        :raises HTTPNotFound: if visualization_name isn't a registered plugin.
-        """
-        if not trans.app.visualizations_registry:
-            raise HTTPNotFound("No visualization registry (possibly disabled in galaxy.ini)")
-        return trans.app.visualizations_registry.get_plugin(visualization_name)
-
-    def _handle_plugin_error(self, trans, visualization_name, exception):
-        """
-        Log, raise if debugging; log and show html message if not.
-        """
-        log.exception("error rendering visualization (%s)", visualization_name)
-        if trans.debug:
-            raise exception
-        return trans.show_error_message(
-            "There was an error rendering the visualization. "
-            + "Contact your Galaxy administrator if the problem persists."
-            + "<br/>Details: "
-            + unicodify(exception),
-            use_panels=False,
-        )
-
-    @web.expose
-    @web.require_login("use Galaxy visualizations", use_panels=True)
-    def saved(self, trans, id=None, revision=None, type=None, config=None, title=None, **kwargs):
-        """
-        Save (on POST) or load (on GET) a visualization then render.
-        """
-        # TODO: consider merging saved and render at this point (could break saved URLs, tho)
-        if trans.request.method == "POST":
-            self._POST_to_saved(trans, id=id, revision=revision, type=type, config=config, title=title, **kwargs)
-
-        # check the id and load the saved visualization
-        if id is None:
-            return HTTPBadRequest("A valid visualization id is required to load a visualization")
-        visualization = self.get_visualization(trans, id, check_ownership=False, check_accessible=True)
-
-        # re-add title to kwargs for passing to render
-        if title:
-            kwargs["title"] = title
-        plugin = self._get_plugin_from_registry(trans, visualization.type)
-        try:
-            return plugin.render_saved(visualization, trans=trans, **kwargs)
-        except Exception as exception:
-            self._handle_plugin_error(trans, visualization.type, exception)
-
-    def _POST_to_saved(self, trans, id=None, revision=None, type=None, config=None, title=None, **kwargs):
-        """
-        Save the visualiztion info (revision, type, config, title, etc.) to
-        the Visualization at `id` or to a new Visualization if `id` is None.
-
-        Uses POST/redirect/GET after a successful save, redirecting to GET.
-        """
-        DEFAULT_VISUALIZATION_NAME = "Unnamed Visualization"
-
-        # post to saved in order to save a visualization
-        if type is None or config is None:
-            return HTTPBadRequest("A visualization type and config are required to save a visualization")
-        if isinstance(config, str):
-            config = loads(config)
-        title = title or DEFAULT_VISUALIZATION_NAME
-
-        # TODO: allow saving to (updating) a specific revision - should be part of UsesVisualization
-        # TODO: would be easier if this returned the visualization directly
-        # check security if posting to existing visualization
-        if id is not None:
-            self.get_visualization(trans, id, check_ownership=True, check_accessible=False)
-            # ??: on not owner: error raised, but not returned (status = 200)
-        # TODO: there's no security check in save visualization (if passed an id)
-        returned = self.save_visualization(trans, config, type, id, title)
-
-        # redirect to GET to prevent annoying 'Do you want to post again?' dialog on page reload
-        render_url = web.url_for(controller="visualization", action="saved", id=returned.get("vis_id"))
-        return trans.response.send_redirect(render_url)
-
-    #
-    # Visualizations.
-    #
-    @web.expose
-    @web.require_login()
-    def trackster(self, trans, **kwargs):
-        """
-        Display browser for the visualization denoted by id and add the datasets listed in `dataset_ids`.
-        """
-
-        # define app configuration
-        app = {"jscript": "trackster"}
-
-        # get dataset to add
-        id = kwargs.get("id", None)
-
-        # get dataset to add
-        new_dataset_id = kwargs.get("dataset_id", None)
-
-        # set up new browser if no id provided
-        if not id:
-            # use dbkey from dataset to be added or from incoming parameter
-            dbkey = None
-            if new_dataset_id:
-                decoded_id = self.decode_id(new_dataset_id)
-                hda = self.hda_manager.get_owned(decoded_id, trans.user, current_history=trans.user)
-                dbkey = hda.dbkey
-                if dbkey == "?":
-                    dbkey = kwargs.get("dbkey", None)
+        Returns state of dataset.
+        """
+        msg = self.hda_manager.data_conversion_status(dataset)
+        if not msg:
+            msg = dataset.conversion_messages.DATA
 
-            # save database key
-            app["default_dbkey"] = dbkey
-        else:
-            # load saved visualization
-            vis = self.get_visualization(trans, id, check_ownership=False, check_accessible=True)
-            app["viz_config"] = self.get_visualization_config(trans, vis)
+        return msg
 
-        # backup id
-        app["id"] = id
+    def _converted_datasets_state(
+        self,
+        trans,
+        dataset: model.DatasetInstance,
+        chrom: Optional[str] = None,
+        retry: bool = False,
+    ) -> Union[model.Dataset.conversion_messages, dict]:
+        """
+        Init-like method that returns state of dataset's converted datasets.
+        Returns valid chroms for that dataset as well.
+        """
+        msg = self.hda_manager.data_conversion_status(dataset)
+        if msg:
+            return msg
 
-        # add dataset id
-        app["add_dataset"] = new_dataset_id
+        # Get datasources and check for messages (which indicate errors). Retry if flag is set.
+        data_sources = dataset.get_datasources(trans)
+        messages_list = [data_source_dict["message"] for data_source_dict in data_sources.values()]
+        msg = self._get_highest_priority_msg(messages_list)
+        if msg:
+            if retry:
+                # Clear datasources and then try again.
+                dataset.clear_associated_files()
+                return self._converted_datasets_state(trans, dataset, chrom)
+            else:
+                return msg
 
-        # check for gene region
-        gene_region = GenomeRegion.from_str(kwargs.get("gene_region", ""))
+        # If there is a chrom, check for data on the chrom.
+        if chrom:
+            data_provider = self.data_provider_registry.get_data_provider(
+                trans, original_dataset=dataset, source="index"
+            )
+            if not data_provider.has_data(chrom):
+                return dataset.conversion_messages.NO_DATA
 
-        # update gene region of saved visualization if user parses a new gene region in the url
-        if gene_region.chrom is not None:
-            app["gene_region"] = {"chrom": gene_region.chrom, "start": gene_region.start, "end": gene_region.end}
+        # Have data if we get here
+        return {"status": dataset.conversion_messages.DATA, "valid_chroms": None}
 
-        # fill template
-        return trans.fill_template("visualization/trackster.mako", config={"app": app, "bundle": "extended"})
+    def _search_features(
+        self,
+        trans,
+        dataset: model.DatasetInstance,
+        query: Optional[str],
+    ) -> List[List[str]]:
+        """
+        Returns features, locations in dataset that match query. Format is a
+        list of features; each feature is a list itself: [name, location]
+        """
+        if query is None:
+            raise galaxy_exceptions.RequestParameterMissingException(
+                "Parameter `query` is required when searching features."
+            )
+        if dataset.can_convert_to("fli"):
+            converted_dataset = dataset.get_converted_dataset(trans, "fli")
+            if converted_dataset:
+                data_provider = FeatureLocationIndexDataProvider(converted_dataset=converted_dataset)
+                if data_provider:
+                    return data_provider.get_data(query)
+
+        return []
+
+    def _data(
+        self,
+        trans: ProvidesHistoryContext,
+        dataset: model.DatasetInstance,
+        chrom: str,
+        low: int,
+        high: int,
+        start_val: int = 0,
+        max_vals: Optional[int] = None,
+        **kwargs,
+    ) -> Union[model.Dataset.conversion_messages, BamDataResult, DataResult]:
+        """
+        Provides a block of data from a dataset.
+        """
+        # Parameter check.
+        if not chrom:
+            return dataset.conversion_messages.NO_DATA
+
+        # Dataset check.
+        if msg := self.hda_manager.data_conversion_status(dataset):
+            return msg
+
+        # Get datasources and check for messages.
+        data_sources = dataset.get_datasources(trans)
+        messages_list = [data_source_dict["message"] for data_source_dict in data_sources.values()]
+        if return_message := self._get_highest_priority_msg(messages_list):
+            return return_message
+
+        extra_info = None
+        mode = kwargs.get("mode", "Auto")
+
+        # Coverage mode uses index data.
+        if mode == "Coverage":
+            # Get summary using minimal cutoffs.
+            indexer = self._get_indexer(trans, dataset)
+            return indexer.get_data(chrom, low, high, **kwargs)
+
+        # TODO:
+        # (1) add logic back in for no_detail
+        # (2) handle scenario where mode is Squish/Pack but data requested is large, so reduced data needed to be returned.
+
+        # If mode is Auto, need to determine what type of data to return.
+        if mode == "Auto":
+            # Get stats from indexer.
+            indexer = self._get_indexer(trans, dataset)
+            stats = indexer.get_data(chrom, low, high, stats=True)
+
+            # If stats were requested, return them.
+            if "stats" in kwargs:
+                if stats["data"]["max"] == 0:
+                    return DataResult(dataset_type=indexer.dataset_type, data=[])
+                else:
+                    return stats
+
+            # Stats provides features/base and resolution is bases/pixel, so
+            # multiplying them yields features/pixel.
+            features_per_pixel = stats["data"]["max"] * float(kwargs["resolution"])
+
+            # Use heuristic based on features/pixel and region size to determine whether to
+            # return coverage data. When zoomed out and region is large, features/pixel
+            # is determining factor. However, when sufficiently zoomed in and region is
+            # small, coverage data is no longer provided.
+            if int(high) - int(low) > 50000 and features_per_pixel > 1000:
+                return indexer.get_data(chrom, low, high)
+
+        #
+        # Provide individual data points.
+        #
+
+        # Get data provider.
+        data_provider = self.data_provider_registry.get_data_provider(trans, original_dataset=dataset, source="data")
+
+        # Allow max_vals top be data provider set if not passed
+        if max_vals is None:
+            max_vals = data_provider.get_default_max_vals()
+
+        # Get reference sequence and mean depth for region; these is used by providers for aligned reads.
+        region = None
+        mean_depth = None
+        if isinstance(data_provider, (SamDataProvider, BamDataProvider)):
+            # Get reference sequence.
+            if dataset.dbkey:
+                # FIXME: increase region 1M each way to provide sequence for
+                # spliced/gapped reads. Probably should provide refseq object
+                # directly to data provider.
+                region = trans.app.genomes.reference(
+                    trans,
+                    dbkey=dataset.dbkey,
+                    chrom=chrom,
+                    low=(max(0, int(low) - 1000000)),
+                    high=(int(high) + 1000000),
+                )
 
-    @web.expose
-    def circster(self, trans, id=None, hda_ldda=None, dataset_id=None, dbkey=None, **kwargs):
-        """
-        Display a circster visualization.
-        """
+            # Get mean depth.
+            indexer = self._get_indexer(trans, dataset)
+            stats = indexer.get_data(chrom, low, high, stats=True)
+            mean_depth = stats["data"]["mean"]
+
+        # Get and return data from data_provider.
+        result = data_provider.get_data(
+            chrom, int(low), int(high), int(start_val), int(max_vals), ref_seq=region, mean_depth=mean_depth, **kwargs
+        )
+        result.update({"dataset_type": data_provider.dataset_type, "extra_info": extra_info})
+        return result
+
+    def _raw_data(
+        self,
+        trans,
+        dataset,
+        provider=None,
+        **kwargs,
+    ) -> Union[model.Dataset.conversion_messages, BamDataResult, DataResult]:
+        """
+        Uses original (raw) dataset to return data. This method is useful
+        when the dataset is not yet indexed and hence using data would
+        be slow because indexes need to be created.
+        """
+        # Dataset check.
+        if msg := self.hda_manager.data_conversion_status(dataset):
+            return msg
+
+        registry = self.data_provider_registry
+
+        # allow the caller to specify which provider is used
+        #   pulling from the original providers if possible, then the new providers
+        if provider:
+            if provider in registry.dataset_type_name_to_data_provider:
+                data_provider = registry.get_data_provider(trans, name=provider, original_dataset=dataset)
+
+            elif dataset.datatype.has_dataprovider(provider):
+                kwargs = dataset.datatype.dataproviders[provider].parse_query_string_settings(kwargs)
+                # use dictionary to allow more than the data itself to be returned (data totals, other meta, etc.)
+                return DataResult(data=list(dataset.datatype.dataprovider(dataset, provider, **kwargs)))
 
-        # Get dataset to add.
-        dataset = None
-        if dataset_id:
-            dataset = self.get_hda_or_ldda(trans, hda_ldda, dataset_id)
+            else:
+                raise NoProviderAvailable(dataset.datatype, provider)
 
-        # Get/create vis.
-        if id:
-            # Display existing viz.
-            vis = self.get_visualization(trans, id, check_ownership=False, check_accessible=True)
-            dbkey = vis.dbkey
+        # no provider name: look up by datatype
         else:
-            # Create new viz.
-            if not dbkey:
-                # If dbkey not specified, use dataset's dbkey.
-                dbkey = dataset.dbkey
-                if not dbkey or dbkey == "?":
-                    # Circster requires a valid dbkey.
-                    return trans.show_error_message(
-                        "You must set the dataset's dbkey to view it. You can set "
-                        "a dataset's dbkey by clicking on the pencil icon and editing "
-                        "its attributes.",
-                        use_panels=True,
-                    )
+            data_provider = registry.get_data_provider(trans, raw=True, original_dataset=dataset)
 
-            vis = self.create_visualization(trans, type="genome", dbkey=dbkey, save=False)
+        # Return data.
+        data = data_provider.get_data(**kwargs)
 
-        # Get the vis config and work with it from here on out. Working with the
-        # config is only possible because the config structure of trackster/genome
-        # visualizations is well known.
-        viz_config = self.get_visualization_config(trans, vis)
-
-        # Add dataset if specified.
-        if dataset:
-            viz_config["tracks"].append(self.get_new_track_config(trans, dataset))
-
-        # Get genome info.
-        chroms_info = self.app.genomes.chroms(trans, dbkey=dbkey)
-        genome = {"dbkey": dbkey, "chroms_info": chroms_info}
-
-        # Add genome-wide data to each track in viz.
-        tracks = viz_config.get("tracks", [])
-        for track in tracks:
-            dataset_dict = track["dataset"]
-            dataset = self.get_hda_or_ldda(trans, dataset_dict["hda_ldda"], dataset_dict["id"])
-
-            genome_data = self._get_genome_data(trans, dataset, dbkey)
-            if not isinstance(genome_data, str):
-                track["preloaded_data"] = genome_data
-
-        # define app configuration for generic mako template
-        app = {"jscript": "circster", "viz_config": viz_config, "genome": genome}
-
-        # fill template
-        return trans.fill_template("visualization/trackster.mako", config={"app": app, "bundle": "extended"})
-
-    @web.expose
-    def sweepster(self, trans, id=None, hda_ldda=None, dataset_id=None, regions=None, **kwargs):
-        """
-        Displays a sweepster visualization using the incoming parameters. If id is available,
-        get the visualization with the given id; otherwise, create a new visualization using
-        a given dataset and regions.
-        """
-        regions = regions or "{}"
-        # Need to create history if necessary in order to create tool form.
-        trans.get_history(most_recent=True, create=True)
-
-        if id:
-            # Loading a shared visualization.
-            viz = self.get_visualization(trans, id)
-            viz_config = self.get_visualization_config(trans, viz)
-            decoded_id = self.decode_id(viz_config["dataset_id"])
-            dataset = self.hda_manager.get_owned(decoded_id, trans.user, current_history=trans.history)
-        else:
-            # Loading new visualization.
-            dataset = self.get_hda_or_ldda(trans, hda_ldda, dataset_id)
-            job = self.hda_manager.creating_job(dataset)
-            viz_config = {"dataset_id": dataset_id, "tool_id": job.tool_id, "regions": loads(regions)}
-
-        # Add tool, dataset attributes to config based on id.
-        tool = trans.app.toolbox.get_tool(viz_config["tool_id"])
-        viz_config["tool"] = tool.to_dict(trans, io_details=True)
-        viz_config["dataset"] = trans.security.encode_dict_ids(dataset.to_dict())
-
-        return trans.fill_template_mako("visualization/sweepster.mako", config=viz_config)
-
-    def get_item(self, trans, id):
-        return self.get_visualization(trans, id)
-
-    @web.expose
-    def phyloviz(self, trans, id=None, dataset_id=None, tree_index=0, **kwargs):
-        config = None
-        data = None
-
-        # if id, then this is a saved visualization; get its config and the dataset_id from there
-        if id:
-            visualization = self.get_visualization(trans, id)
-            config = self.get_visualization_config(trans, visualization)
-            dataset_id = config.get("dataset_id", None)
-
-        # get the hda if we can, then its data using the phyloviz parsers
-        if dataset_id:
-            decoded_id = self.decode_id(dataset_id)
-            hda = self.hda_manager.get_accessible(decoded_id, trans.user)
-            hda = self.hda_manager.error_if_uploading(hda)
-        else:
-            return trans.show_message("Phyloviz couldn't find a dataset_id")
-
-        pd = PhylovizDataProvider(original_dataset=hda)
-        data = pd.get_data(tree_index=tree_index)
+        return data
 
-        # ensure at least a default configuration (gen. an new/unsaved visualization)
-        if not config:
-            config = {
-                "dataset_id": dataset_id,
-                "title": hda.display_name(),
-                "ext": hda.datatype.file_ext,
-                "treeIndex": tree_index,
-                "saved_visualization": False,
-            }
-        return trans.fill_template_mako("visualization/phyloviz.mako", data=data, config=config)
+    def _get_indexer(self, trans, dataset):
+        indexer = self.data_provider_registry.get_data_provider(trans, original_dataset=dataset, source="index")
+        if indexer is None:
+            msg = f"No indexer available for dataset {self.encode_id(dataset.id)}"
+            log.exception(msg)
+            raise galaxy_exceptions.ObjectNotFound(msg)
+        return indexer
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/fast_app.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 )
 
 from a2wsgi import WSGIMiddleware
 from fastapi import (
     FastAPI,
     Request,
 )
+from fastapi.openapi.constants import REF_TEMPLATE
 from starlette.middleware.cors import CORSMiddleware
 from starlette.responses import Response
 
+from galaxy.schema.invocation import CustomJsonSchema
 from galaxy.version import VERSION
 from galaxy.webapps.base.api import (
     add_exception_handler,
     add_request_id_middleware,
     GalaxyFileResponse,
     include_all_package_routers,
 )
@@ -95,16 +97,15 @@
         super().__init__(*args, **kwds)
 
     def is_allowed_origin(self, origin: str) -> bool:
         return config_allows_origin(origin, self.config)
 
 
 def add_galaxy_middleware(app: FastAPI, gx_app):
-    x_frame_options = gx_app.config.x_frame_options
-    if x_frame_options:
+    if x_frame_options := gx_app.config.x_frame_options:
 
         @app.middleware("http")
         async def add_x_frame_options(request: Request, call_next):
             response = await call_next(request)
             response.headers["X-Frame-Options"] = x_frame_options
             return response
 
@@ -165,28 +166,29 @@
     return get_openapi(
         title=app.title,
         version=app.version,
         openapi_version="3.1.0",
         description=app.description,
         routes=app.routes,
         license_info=app.license_info,
+        schema_generator=CustomJsonSchema(ref_template=REF_TEMPLATE),
     )
 
 
 def initialize_fast_app(gx_wsgi_webapp, gx_app):
     root_path = "" if gx_app.config.galaxy_url_prefix == "/" else gx_app.config.galaxy_url_prefix
     app = get_fastapi_instance(root_path=root_path)
     add_exception_handler(app)
     add_galaxy_middleware(app, gx_app)
     add_request_id_middleware(app)
     include_all_package_routers(app, "galaxy.webapps.galaxy.api")
     include_legacy_openapi(app, gx_app)
     wsgi_handler = WSGIMiddleware(gx_wsgi_webapp)
     gx_app.haltables.append(("WSGI Middleware threadpool", wsgi_handler.executor.shutdown))
-    app.mount("/", wsgi_handler)
+    app.mount("/", wsgi_handler)  # type: ignore[arg-type]
     if gx_app.config.galaxy_url_prefix != "/":
         parent_app = FastAPI()
         parent_app.mount(gx_app.config.galaxy_url_prefix, app=app)
         return parent_app
     return app
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/fast_factory.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/fast_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/_fetch_util.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/_fetch_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from galaxy.exceptions import RequestParameterInvalidException
 from galaxy.files.uris import validate_non_local
 from galaxy.model.store.discover import (
     get_required_item,
     replace_request_syntax_sugar,
 )
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.tools.actions.upload_common import validate_datatype_extension
 from galaxy.util import relpath
 
 log = logging.getLogger(__name__)
 
 VALID_DESTINATION_TYPES = ["library", "library_folder", "hdca", "hdas"]
 # These elements_from cannot be sym linked to because they only exist during upload.
@@ -44,15 +44,15 @@
             description = destination.get("description", "")
             synopsis = destination.get("synopsis", "")
             library = trans.app.library_manager.create(trans, library_name, description=description, synopsis=synopsis)
             destination["type"] = "library_folder"
             for key in ["name", "description", "synopsis"]:
                 if key in destination:
                     del destination[key]
-            destination["library_folder_id"] = DecodedDatabaseIdField.encode(library.root_folder.id)
+            destination["library_folder_id"] = Security.security.encode_id(library.root_folder.id)
 
     # Unlike upload.py we don't transmit or use run_as_real_user in the job - we just make sure
     # in_place and purge_source are set on the individual upload fetch sources as needed based
     # on this.
     run_as_real_user = trans.app.config.external_chown_script is not None  # See comment in upload.py
     purge_ftp_source = getattr(trans.app.config, "ftp_upload_purge", True) and not run_as_real_user
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/authenticate.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/base.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 from galaxy.model.store import (
     get_export_store_factory,
     ModelExportStore,
 )
 from galaxy.schema.fields import EncodedDatabaseIdField
 from galaxy.schema.schema import AsyncTaskResultSummary
 from galaxy.security.idencoding import IdEncodingHelper
-from galaxy.util import ready_name_for_url
-from galaxy.web.short_term_storage import (
+from galaxy.short_term_storage import (
     ShortTermStorageAllocator,
     ShortTermStorageTarget,
 )
+from galaxy.util import ready_name_for_url
 
 
 def ensure_celery_tasks_enabled(config):
     if not config.enable_celery_tasks:
         raise ConfigDoesNotAllowException(
             "This operation requires asynchronous tasks to be enabled on the Galaxy server and they are not, please contact the server admin."
         )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/dataset_collections.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/dataset_collections.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
     Optional,
     Set,
     TYPE_CHECKING,
     Union,
 )
 
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
+    RootModel,
     ValidationError,
 )
 from typing_extensions import Literal
 
 from galaxy import exceptions
 from galaxy.datatypes.registry import Registry
 from galaxy.managers.collections import DatasetCollectionManager
@@ -52,46 +53,44 @@
 log = getLogger(__name__)
 
 
 class UpdateCollectionAttributePayload(Model):
     """Contains attributes that can be updated for all elements in a dataset collection."""
 
     dbkey: str = Field(..., description="TODO")
-
-    class Config:
-        extra = Extra.forbid  # will cause validation to fail if extra attributes are included,
+    model_config = ConfigDict(extra="forbid")
 
 
 class DatasetCollectionAttributesResult(Model):
     dbkey: str = Field(..., description="TODO")
     # Are the following fields really used/needed?
-    extension: str = Field(..., description="The dataset file extension.", example="txt")
+    extension: str = Field(..., description="The dataset file extension.", examples=["txt"])
     model_class: Literal["HistoryDatasetCollectionAssociation"] = ModelClassField("HistoryDatasetCollectionAssociation")
     dbkeys: Optional[Set[str]]
     extensions: Optional[Set[str]]
     tags: TagCollection
 
 
 class SuitableConverter(Model):
     tool_id: str = Field(..., description="The ID of the tool that can perform the type conversion.")
     name: str = Field(..., description="The name of the converter.")
     target_type: str = Field(..., description="The type to convert to.")
     original_type: str = Field(..., description="The type to convert from.")
 
 
-class SuitableConverters(Model):
+class SuitableConverters(RootModel):
     """Collection of converters that can be used on a particular dataset collection."""
 
-    __root__: List[SuitableConverter]
+    root: List[SuitableConverter]
 
 
-class DatasetCollectionContentElements(Model):
+class DatasetCollectionContentElements(RootModel):
     """Represents a collection of elements contained in the dataset collection."""
 
-    __root__: List[DCESummary]
+    root: List[DCESummary]
 
 
 class DatasetCollectionsService(ServiceBase, UsesLibraryMixinItems):
     def __init__(
         self,
         security: IdEncodingHelper,
         history_manager: HistoryManager,
@@ -213,15 +212,15 @@
         if not dce:
             raise exceptions.ObjectNotFound("No DatasetCollectionElement found")
         if not trans.user_is_admin:
             collection = dce.child_collection or dce.collection
             if not trans.app.security_agent.can_access_collection(trans.get_current_user_roles(), collection):
                 raise exceptions.ItemAccessibilityException("Collection not accessible by user.")
         serialized_dce = dictify_element_reference(dce, recursive=False, security=trans.security)
-        return trans.security.encode_all_ids(serialized_dce, recursive=True)
+        return serialized_dce
 
     def contents(
         self,
         trans: ProvidesHistoryContext,
         hdca_id: DecodedDatabaseIdField,
         parent_id: DecodedDatabaseIdField,
         instance_type: DatasetCollectionInstanceType = "history",
@@ -267,18 +266,17 @@
             if result["element_type"] == DCEType.dataset_collection:
                 assert trans.url_builder
                 result["object"]["contents_url"] = trans.url_builder(
                     "contents_dataset_collection",
                     hdca_id=self.encode_id(hdca.id),
                     parent_id=self.encode_id(result["object"]["id"]),
                 )
-            trans.security.encode_all_ids(result, recursive=True)
             return result
 
         rval = [serialize_element(el) for el in contents]
         try:
-            return DatasetCollectionContentElements.construct(__root__=rval)
+            return DatasetCollectionContentElements(root=rval)
         except ValidationError:
             log.exception(
                 f"Serializing DatasetCollectionContentsElements failed. Collection is populated: {hdca.collection.populated}"
             )
             raise
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/help.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/history_contents.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/history_contents.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Optional,
     Set,
     Union,
 )
 
 from celery import chain
 from pydantic import (
-    Extra,
+    ConfigDict,
     Field,
 )
 from typing_extensions import (
     Literal,
     Protocol,
 )
 
@@ -93,15 +93,14 @@
     HistoryContentBulkOperationPayload,
     HistoryContentBulkOperationResult,
     HistoryContentItem,
     HistoryContentItemOperation,
     HistoryContentsArchiveDryRunResult,
     HistoryContentSource,
     HistoryContentsResult,
-    HistoryContentStats,
     HistoryContentsWithStatsResult,
     HistoryContentType,
     JobSourceType,
     MaterializeDatasetInstanceRequest,
     Model,
     StoreContentSource,
     StoreExportPayload,
@@ -113,16 +112,16 @@
 from galaxy.schema.tasks import (
     GenerateHistoryContentDownload,
     MaterializeDatasetInstanceTaskRequest,
     PrepareDatasetCollectionDownload,
     WriteHistoryContentTo,
 )
 from galaxy.security.idencoding import IdEncodingHelper
+from galaxy.short_term_storage import ShortTermStorageAllocator
 from galaxy.util.zipstream import ZipstreamWrapper
-from galaxy.web.short_term_storage import ShortTermStorageAllocator
 from galaxy.webapps.galaxy.services.base import (
     async_task_summary,
     ConsumesModelStores,
     ensure_celery_tasks_enabled,
     model_store_storage_target,
     ServesExportStores,
     ServiceBase,
@@ -221,15 +220,15 @@
         title="Collection Type",
         description="The type of the nested collection. For example, `list`, `paired`, `list:paired`.",
     )
 
 
 # Required for self-referencing models
 # See https://pydantic-docs.helpmanual.io/usage/postponed_annotations/#self-referencing-models
-CollectionElementIdentifier.update_forward_refs()
+CollectionElementIdentifier.model_rebuild()
 
 
 class CreateHistoryContentFromStore(StoreContentSource):
     pass
 
 
 class CreateHistoryContentPayloadFromCollection(CreateHistoryContentPayloadFromCopy):
@@ -245,16 +244,15 @@
             "If the source is a collection, whether to copy child HDAs into the target "
             "history as well. Prior to the galaxy release 23.1 this defaulted to false."
         ),
     )
 
 
 class CreateHistoryContentPayload(CreateHistoryContentPayloadFromCollection, CreateNewCollectionPayload):
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
 
 class HistoriesContentsService(ServiceBase, ServesExportStores, ConsumesModelStores):
     """Common interface/service logic for interactions with histories contents in the context of the API.
 
     Provides the logic of the actions invoked by API controllers and uses type definitions
     and pydantic models to declare its parameters and return types.
@@ -382,15 +380,15 @@
             model_store_format,
         )
         request = GenerateHistoryContentDownload(
             short_term_storage_request_id=short_term_storage_target.request_id,
             user=trans.async_request_user,
             content_type=contents_type,
             content_id=content_id,
-            **payload.dict(),
+            **payload.model_dump(),
         )
         result = prepare_history_content_download.delay(request=request, task_user_id=getattr(trans.user, "id", None))
         return AsyncFile(storage_request_id=short_term_storage_target.request_id, task=async_task_summary(result))
 
     def write_store(
         self,
         trans: ProvidesHistoryContext,
@@ -404,15 +402,15 @@
             content_id = hda.id
         elif contents_type == HistoryContentType.dataset_collection:
             dataset_collection_instance = self.__get_accessible_collection(trans, id)
             content_id = dataset_collection_instance.id
         else:
             raise exceptions.UnknownContentsType(f"Unknown contents type: {contents_type}")
         request = WriteHistoryContentTo(
-            user=trans.async_request_user, content_id=content_id, contents_type=contents_type, **payload.dict()
+            user=trans.async_request_user, content_id=content_id, contents_type=contents_type, **payload.model_dump()
         )
         result = write_history_content_to.delay(request=request, task_user_id=getattr(trans.user, "id", None))
         return async_task_summary(result)
 
     def index_jobs_summary(
         self,
         trans,
@@ -428,15 +426,15 @@
         """
         ids = params.ids
         types = params.types
         if len(ids) != len(types):
             raise exceptions.RequestParameterInvalidException(
                 f"The number of ids ({len(ids)}) and types ({len(types)}) must match."
             )
-        return [self.encode_all_ids(job_state) for job_state in fetch_job_states(trans.sa_session, ids, types)]
+        return fetch_job_states(trans.sa_session, ids, types)
 
     def show_jobs_summary(
         self,
         trans,
         id: DecodedDatabaseIdField,
         contents_type: HistoryContentType,
     ) -> AnyJobStateSummary:
@@ -545,33 +543,34 @@
             history=history,
         )
         rval: List[AnyHistoryContentItem] = []
         serialization_params.default_view = "detailed"
         for hda in object_tracker.hdas_by_key.values():
             if hda.visible:
                 hda_dict = self.hda_serializer.serialize_to_view(
-                    hda, user=trans.user, trans=trans, **serialization_params.dict()
+                    hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
                 )
                 rval.append(hda_dict)
         for hdca in object_tracker.hdcas_by_key.values():
             hdca_dict = self.hdca_serializer.serialize_to_view(
-                hdca, user=trans.user, trans=trans, **serialization_params.dict()
+                hdca, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
             )
             rval.append(hdca_dict)
         return rval
 
     def materialize(
         self,
         trans,
         request: MaterializeDatasetInstanceRequest,
     ) -> AsyncTaskResultSummary:
         # DO THIS JUST TO MAKE SURE IT IS OWNED...
         self.history_manager.get_mutable(request.history_id, trans.user, current_history=trans.history)
         assert trans.app.config.enable_celery_tasks
-        task_request = MaterializeDatasetInstanceTaskRequest(
+        # values already validated and coerced, use model_construct
+        task_request = MaterializeDatasetInstanceTaskRequest.model_construct(
             history_id=request.history_id,
             source=request.source,
             content=request.content,
             user=trans.async_request_user,
         )
         results = materialize_task.delay(request=task_request)
         return async_task_summary(results)
@@ -593,21 +592,21 @@
             - access_ids[]: list of Role.id defining roles that should have access permission on the dataset
             - manage_ids[]: list of Role.id defining roles that should have manage permission on the dataset
             - modify_ids[]: list of Role.id defining roles that should have modify permission on the library dataset item
 
         :raises: RequestParameterInvalidException, ObjectNotFound, InsufficientPermissionsException, InternalServerError
                     RequestParameterMissingException
         """
-        payload_dict = payload.dict(by_alias=True)
+        payload_dict = payload.model_dump(by_alias=True)
         hda = self.hda_manager.get_owned(history_content_id, trans.user, current_history=trans.history, trans=trans)
         assert hda is not None
         self.history_manager.error_unless_mutable(hda.history)
         self.hda_manager.update_permissions(trans, hda, **payload_dict)
         roles = self.hda_manager.serialize_dataset_association_roles(trans, hda)
-        return DatasetAssociationRoles.construct(**roles)
+        return DatasetAssociationRoles(**roles)
 
     def update(
         self,
         trans,
         history_id: DecodedDatabaseIdField,
         id: DecodedDatabaseIdField,
         payload: Dict[str, Any],
@@ -660,25 +659,27 @@
         hdca_ids: List[DecodedDatabaseIdField] = []
         for item in items:
             contents_type = item.history_content_type
             if contents_type == HistoryContentType.dataset:
                 hda_ids.append(item.id)
             else:
                 hdca_ids.append(item.id)
-        payload_dict = payload.dict(exclude_unset=True)
+        payload_dict = payload.model_dump(exclude_unset=True)
         hdas = self.__datasets_for_update(trans, history, hda_ids, payload_dict)
         rval = []
         for hda in hdas:
             self.__deserialize_dataset(trans, hda, payload_dict)
             serialization_params.default_view = "summary"
             rval.append(
-                self.hda_serializer.serialize_to_view(hda, user=trans.user, trans=trans, **serialization_params.dict())
+                self.hda_serializer.serialize_to_view(
+                    hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
+                )
             )
         for hdca_id in hdca_ids:
-            self.__update_dataset_collection(trans, hdca_id, payload.dict(exclude_defaults=True))
+            self.__update_dataset_collection(trans, hdca_id, payload.model_dump(exclude_defaults=True))
             dataset_collection_instance = self.__get_accessible_collection(trans, hdca_id)
             rval.append(self.__collection_dict(trans, dataset_collection_instance, view="summary"))
         return rval
 
     def bulk_operation(
         self,
         trans: ProvidesHistoryContext,
@@ -701,15 +702,15 @@
                 history,
                 filters,
             )
         errors = self._apply_bulk_operation(contents, payload.operation, payload.params, trans)
         with transaction(trans.sa_session):
             trans.sa_session.commit()
         success_count = len(contents) - len(errors)
-        return HistoryContentBulkOperationResult.construct(success_count=success_count, errors=errors)
+        return HistoryContentBulkOperationResult(success_count=success_count, errors=errors)
 
     def validate(self, trans, history_id: DecodedDatabaseIdField, history_content_id: DecodedDatabaseIdField):
         """
         Validates the metadata associated with a dataset within a History.
 
         :type   history_id: str
         :param  history_id: encoded id string of the items's History
@@ -841,15 +842,15 @@
 
         # filter the contents that contain datasets using any filters possible from index above and map the datasets
         filters = self.history_contents_filters.parse_query_filters(filter_query_params)
         self.history_contents_manager.map_datasets(history, build_archive_files_and_paths, filters=filters)
 
         # if dry_run, return the structure as json for debugging
         if dry_run:
-            return HistoryContentsArchiveDryRunResult.construct(__root__=paths_and_files)
+            return HistoryContentsArchiveDryRunResult(root=paths_and_files)
 
         # create the archive, add the dataset files, then stream the archive as a download
         archive = ZipstreamWrapper(
             archive_name=archive_base_name,
             upstream_mod_zip=trans.app.config.upstream_mod_zip,
             upstream_gzip=trans.app.config.upstream_gzip,
         )
@@ -866,15 +867,17 @@
 
         async_result = None
         if purge:
             async_result = self.hda_manager.purge(hda, user=trans.user)
         else:
             self.hda_manager.delete(hda, stop_job=stop_job)
         serialization_params.default_view = "detailed"
-        rval = self.hda_serializer.serialize_to_view(hda, user=trans.user, trans=trans, **serialization_params.dict())
+        rval = self.hda_serializer.serialize_to_view(
+            hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
+        )
         rval["async_result"] = async_result is not None
         return rval
 
     def __update_dataset_collection(self, trans, id: DecodedDatabaseIdField, payload: Dict[str, Any]):
         return self.dataset_collection_manager.update(trans, "history", id, payload)
 
     def __update_dataset(
@@ -883,20 +886,19 @@
         history: History,
         id: DecodedDatabaseIdField,
         payload: Dict[str, Any],
         serialization_params: SerializationParams,
     ):
         # anon user: ensure that history ids match up and the history is the current,
         #   check for uploading, and use only the subset of attribute keys manipulatable by anon users
-        hda = self.__datasets_for_update(trans, history, [id], payload)[0]
-        if hda:
+        if hda := self.__datasets_for_update(trans, history, [id], payload)[0]:
             self.__deserialize_dataset(trans, hda, payload)
             serialization_params.default_view = "detailed"
             return self.hda_serializer.serialize_to_view(
-                hda, user=trans.user, trans=trans, **serialization_params.dict()
+                hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
             )
         return {}
 
     def __datasets_for_update(
         self, trans, history: History, hda_ids: List[DecodedDatabaseIdField], payload: Dict[str, Any]
     ):
         anonymous_user = not trans.user_is_admin and trans.user is None
@@ -930,31 +932,31 @@
         self,
         trans,
         history_id: DecodedDatabaseIdField,
         legacy_params: LegacyHistoryContentsIndexParams,
     ) -> HistoryContentsResult:
         """Legacy implementation of the `index` action."""
         history = self._get_history(trans, history_id)
-        legacy_params_dict = legacy_params.dict(exclude_defaults=True)
-        ids = legacy_params_dict.get("ids")
-        if ids:
+        legacy_params_dict = legacy_params.model_dump(exclude_defaults=True)
+        if ids := legacy_params_dict.get("ids"):
             legacy_params_dict["ids"] = self.decode_ids(ids)
+        else:
+            legacy_params_dict.pop("ids", None)
 
         object_store_ids = None
-        shareable = legacy_params.shareable
-        if shareable is not None:
+        if (shareable := legacy_params.shareable) is not None:
             object_store_ids = self.object_store.object_store_ids(private=not shareable)
             if object_store_ids:
                 legacy_params_dict["object_store_ids"] = object_store_ids
         contents = history.contents_iter(**legacy_params_dict)
         items = [
             self._serialize_legacy_content_item(trans, content, legacy_params_dict.get("dataset_details"))
             for content in contents
         ]
-        return HistoryContentsResult.construct(__root__=items)
+        return HistoryContentsResult(root=items)
 
     def __index_v2(
         self,
         trans,
         history_id: DecodedDatabaseIdField,
         params: HistoryContentsIndexParams,
         serialization_params: SerializationParams,
@@ -997,17 +999,16 @@
             for content in contents
         ]
         if stats_requested:
             total_matches = self.history_contents_manager.contents_count(
                 history,
                 filters=filters,
             )
-            stats = HistoryContentStats.construct(total_matches=total_matches)
-            return HistoryContentsWithStatsResult.construct(contents=items, stats=stats)
-        return HistoryContentsResult.construct(__root__=items)
+            return HistoryContentsWithStatsResult(contents=items, stats={"total_matches": total_matches})
+        return HistoryContentsResult(root=items)
 
     def _handle_extra_serialization_for_media_type(
         self,
         serialization_params: SerializationParams,
         request_media_type: str,
     ) -> SerializationParams:
         """According to the requested media type the response may include extra information."""
@@ -1023,15 +1024,17 @@
         content,
         dataset_details: Optional[DatasetDetailsType] = None,
     ):
         encoded_content_id = content.id
         detailed = dataset_details and (dataset_details == "all" or (encoded_content_id in dataset_details))
         if isinstance(content, HistoryDatasetAssociation):
             view = "detailed" if detailed else "summary"
-            return self.hda_serializer.serialize_to_view(content, view=view, user=trans.user, trans=trans)
+            return self.hda_serializer.serialize_to_view(
+                content, view=view, user=trans.user, trans=trans, encode_id=False
+            )
         elif isinstance(content, HistoryDatasetCollectionAssociation):
             view = "element" if detailed else "collection"
             return self.__collection_dict(trans, content, view=view)
 
     def _serialize_content_item(
         self,
         trans,
@@ -1040,43 +1043,45 @@
         serialization_params: SerializationParams,
         default_view: str = "summary",
     ):
         """
         Returns a dictionary with the appropriate values depending on the
         serialization parameters provided.
         """
-        serialization_params_dict = serialization_params.dict()
+        serialization_params_dict = serialization_params.model_dump()
         view = serialization_params_dict.pop("view", default_view) or default_view
 
         serializer: Optional[ModelSerializer] = None
         if isinstance(content, HistoryDatasetAssociation):
             serializer = self.hda_serializer
             if dataset_details and (dataset_details == "all" or content.id in dataset_details):
                 view = "detailed"
         elif isinstance(content, HistoryDatasetCollectionAssociation):
             serializer = self.hdca_serializer
 
         if serializer is None:
             raise exceptions.UnknownContentsType(f"Unknown contents type: {content.content_type}")
 
         rval = serializer.serialize_to_view(
-            content, user=trans.user, trans=trans, view=view, **serialization_params_dict
+            content, user=trans.user, trans=trans, view=view, encode_id=False, **serialization_params_dict
         )
         # Override URL generation to use UrlBuilder
         if trans.url_builder:
             if rval.get("url"):
                 rval["url"] = trans.url_builder(
                     "history_content_typed",
-                    history_id=rval["history_id"],
-                    id=rval["id"],
+                    history_id=self.encode_id(rval["history_id"]),
+                    id=self.encode_id(rval["id"]),
                     type=rval["history_content_type"],
                 )
             if rval.get("contents_url"):
                 rval["contents_url"] = trans.url_builder(
-                    "contents_dataset_collection", hdca_id=rval["id"], parent_id=self.encode_id(content.collection_id)
+                    "contents_dataset_collection",
+                    hdca_id=self.encode_id(rval["id"]),
+                    parent_id=self.encode_id(content.collection_id),
                 )
         return rval
 
     def __collection_dict(self, trans, dataset_collection_instance, **kwds):
         return dictify_dataset_collection_instance(
             dataset_collection_instance,
             security=trans.security,
@@ -1094,15 +1099,17 @@
         self,
         trans,
         id: DecodedDatabaseIdField,
         serialization_params: SerializationParams,
     ):
         serialization_params.default_view = "detailed"
         hda = self.hda_manager.get_accessible(id, trans.user)
-        return self.hda_serializer.serialize_to_view(hda, user=trans.user, trans=trans, **serialization_params.dict())
+        return self.hda_serializer.serialize_to_view(
+            hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
+        )
 
     def __show_dataset_collection(
         self,
         trans,
         id: DecodedDatabaseIdField,
         serialization_params: SerializationParams,
         fuzzy_count: Optional[int] = None,
@@ -1158,15 +1165,15 @@
                 return rval
 
             for ld in traverse(folder):
                 hda = ld.library_dataset_dataset_association.to_history_dataset_association(
                     history, add_to_history=True
                 )
                 hda_dict = self.hda_serializer.serialize_to_view(
-                    hda, user=trans.user, trans=trans, **serialization_params.dict()
+                    hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
                 )
                 rval.append(hda_dict)
         else:
             message = f"Invalid 'source' parameter in request: {source}"
             raise exceptions.RequestParameterInvalidException(message)
 
         with transaction(trans.sa_session):
@@ -1194,15 +1201,17 @@
             hda = self.__create_hda_from_copy(trans, history, content)
 
         if hda is None:
             return None
 
         with transaction(trans.sa_session):
             trans.sa_session.commit()
-        return self.hda_serializer.serialize_to_view(hda, user=trans.user, trans=trans, **serialization_params.dict())
+        return self.hda_serializer.serialize_to_view(
+            hda, user=trans.user, trans=trans, encode_id=False, **serialization_params.model_dump()
+        )
 
     def __create_hda_from_ldda(self, trans, history: History, ldda_id: int):
         decoded_ldda_id = ldda_id
         ld = self.ldda_manager.get(trans, decoded_ldda_id)
         if type(ld) is not LibraryDataset:
             raise exceptions.RequestParameterInvalidException("Library content id is not a dataset")
         hda = ld.library_dataset_dataset_association.to_history_dataset_association(history, add_to_history=True)
@@ -1257,15 +1266,15 @@
 
          :raises: RequestParameterInvalidException, RequestParameterMissingException
         """
         source = payload.source or HistoryContentSource.new_collection
 
         dataset_collection_manager = self.dataset_collection_manager
         if source == HistoryContentSource.new_collection:
-            create_params = api_payload_to_create_params(payload.dict())
+            create_params = api_payload_to_create_params(payload.model_dump())
             dataset_collection_instance = dataset_collection_manager.create(
                 trans, parent=history, history=history, **create_params
             )
         elif source == HistoryContentSource.hdca:
             content = payload.content
             if content is None:
                 raise exceptions.RequestParameterMissingException("'content' id of target to copy is missing")
@@ -1290,15 +1299,19 @@
         else:
             message = f"Invalid 'source' parameter in request: {source}"
             raise exceptions.RequestParameterInvalidException(message)
 
         # if the consumer specified keys or view, use the secondary serializer
         if serialization_params.view or serialization_params.keys:
             return self.hdca_serializer.serialize_to_view(
-                dataset_collection_instance, user=trans.user, trans=trans, **serialization_params.dict()
+                dataset_collection_instance,
+                user=trans.user,
+                trans=trans,
+                encode_id=False,
+                **serialization_params.model_dump(),
             )
 
         return self.__collection_dict(trans, dataset_collection_instance, view="element")
 
     def _validate_bulk_operation_params(
         self, payload: HistoryContentBulkOperationPayload, user: User, trans: ProvidesHistoryContext
     ):
@@ -1333,15 +1346,15 @@
         item: HistoryItemModel,
         params: Optional[AnyBulkOperationParams],
         trans: ProvidesHistoryContext,
     ) -> Optional[BulkOperationItemError]:
         try:
             self.item_operator.apply(operation, item, params, trans)
             return None
-        except BaseException as exc:
+        except Exception as exc:
             return BulkOperationItemError(
                 item=EncodedHistoryContentItem(id=item.id, history_content_type=item.history_content_type),
                 error=str(exc),
             )
 
     def _get_contents_by_item_list(
         self, trans, history: History, items: List[HistoryContentItem]
@@ -1364,16 +1377,15 @@
         contents.extend(collections)
         return contents
 
 
 class ItemOperation(Protocol):
     def __call__(
         self, item: HistoryItemModel, params: Optional[AnyBulkOperationParams], trans: ProvidesHistoryContext
-    ) -> None:
-        ...
+    ) -> None: ...
 
 
 class HistoryItemOperator:
     """Defines operations on history items."""
 
     def __init__(
         self,
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/jobs.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/jobs.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,26 +7,25 @@
 )
 
 from galaxy import (
     exceptions,
     model,
 )
 from galaxy.managers import hdas
+from galaxy.managers.base import security_check
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.managers.jobs import (
     JobManager,
     JobSearch,
     view_show_job,
 )
+from galaxy.model import Job
 from galaxy.schema.fields import DecodedDatabaseIdField
 from galaxy.schema.jobs import JobAssociation
-from galaxy.schema.schema import (
-    EncodedDatasetSourceId,
-    JobIndexQueryPayload,
-)
+from galaxy.schema.schema import JobIndexQueryPayload
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.webapps.galaxy.services.base import ServiceBase
 
 
 class JobIndexViewEnum(str, Enum):
     collection = "collection"
     admin_job_list = "admin_job_list"
@@ -63,40 +62,49 @@
         return view_show_job(trans, job, bool(full))
 
     def index(
         self,
         trans: ProvidesUserContext,
         payload: JobIndexPayload,
     ):
-        security = trans.security
         is_admin = trans.user_is_admin
         view = payload.view
         if view == JobIndexViewEnum.admin_job_list:
             payload.user_details = True
         user_details = payload.user_details
         decoded_user_id = payload.user_id
-
         if not is_admin:
-            self._check_nonadmin_access(view, user_details, decoded_user_id, trans.user.id)
+            self._check_nonadmin_access(view, user_details, decoded_user_id, trans.user and trans.user.id)
 
+        check_security_of_jobs = (
+            payload.invocation_id is not None
+            or payload.implicit_collection_jobs_id is not None
+            or payload.history_id is not None
+        )
         jobs = self.job_manager.index_query(trans, payload)
         out = []
         for job in jobs.yield_per(model.YIELD_PER_ROWS):
+            # TODO: optimize if this crucial
+            if check_security_of_jobs and not security_check(trans, job.history, check_accessible=True):
+                raise exceptions.ItemAccessibilityException("Cannot access the request job objects.")
             job_dict = job.to_dict(view, system_details=is_admin)
-            j = security.encode_all_ids(job_dict, True)
             if view == JobIndexViewEnum.admin_job_list:
-                j["decoded_job_id"] = job.id
+                job_dict["decoded_job_id"] = job.id
             if user_details:
-                j["user_email"] = job.get_user_email()
-            out.append(j)
+                job_dict["user_email"] = job.get_user_email()
+            out.append(job_dict)
 
         return out
 
     def _check_nonadmin_access(
-        self, view: str, user_details: bool, decoded_user_id: Optional[DecodedDatabaseIdField], trans_user_id: int
+        self,
+        view: str,
+        user_details: bool,
+        decoded_user_id: Optional[DecodedDatabaseIdField],
+        trans_user_id: Optional[int],
     ):
         """Verify admin-only resources are not being accessed."""
         if view == JobIndexViewEnum.admin_job_list:
             raise exceptions.AdminRequiredException("Only admins can use the admin_job_list view")
         if user_details:
             raise exceptions.AdminRequiredException("Only admins can index the jobs with user details enabled")
         if decoded_user_id is not None and decoded_user_id != trans_user_id:
@@ -104,36 +112,37 @@
 
     def get_job(
         self,
         trans: ProvidesUserContext,
         job_id: Optional[int] = None,
         dataset_id: Optional[int] = None,
         hda_ldda: str = "hda",
-    ):
+    ) -> Job:
         if job_id is not None:
             return self.job_manager.get_accessible_job(trans, decoded_job_id=job_id)
         elif dataset_id is not None:
             # Following checks dataset accessible
             if hda_ldda == "hda":
                 dataset_instance = self.hda_manager.get_accessible(id=dataset_id, user=trans.user)
             else:
                 dataset_instance = self.hda_manager.ldda_manager.get(trans, id=dataset_id)
+            if not dataset_instance.creating_job:
+                raise ValueError("No job found for dataset id")
             return dataset_instance.creating_job
         else:
             # Raise an exception if neither job_id nor dataset_id is provided
             raise ValueError("Either job_id or dataset_id must be provided.")
 
     def dictify_associations(self, trans, *association_lists) -> List[JobAssociation]:
         rval: List[JobAssociation] = []
         for association_list in association_lists:
             rval.extend(self.__dictify_association(trans, a) for a in association_list)
         return rval
 
     def __dictify_association(self, trans, job_dataset_association) -> JobAssociation:
         dataset_dict = None
-        dataset = job_dataset_association.dataset
-        if dataset:
+        if dataset := job_dataset_association.dataset:
             if isinstance(dataset, model.HistoryDatasetAssociation):
-                dataset_dict = EncodedDatasetSourceId(src="hda", id=dataset.id)
+                dataset_dict = {"src": "hda", "id": dataset.id}
             else:
-                dataset_dict = EncodedDatasetSourceId(src="ldda", id=dataset.id)
+                dataset_dict = {"src": "ldda", "id": dataset.id}
         return JobAssociation(name=job_dataset_association.name, dataset=dataset_dict)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/libraries.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/libraries.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
         """
         query, prefetched_ids = self.library_manager.list(trans, deleted)
         libraries = []
         for library in query:
             library_dict = self.library_manager.get_library_dict(trans, library, prefetched_ids)
             libraries.append(LibrarySummary(**library_dict))
-        return LibrarySummaryList(__root__=libraries)
+        return LibrarySummaryList(root=libraries)
 
     def show(self, trans, id: DecodedDatabaseIdField) -> LibrarySummary:
         """Returns detailed information about a library."""
         library = self.library_manager.get(trans, id)
         return self._to_summary(trans, library)
 
     def create(self, trans, payload: CreateLibraryPayload) -> LibrarySummary:
@@ -158,32 +158,31 @@
         if not (is_admin or trans.app.security_agent.can_manage_library_item(current_user_roles, library)):
             raise exceptions.InsufficientPermissionsException(
                 "You do not have proper permission to access permissions of this library."
             )
 
         if scope == LibraryPermissionScope.current or scope is None:
             roles = self.library_manager.get_current_roles(trans, library)
-            return LibraryCurrentPermissions.construct(**roles)
+            return LibraryCurrentPermissions.model_construct(**roles)
 
         #  Return roles that are available to select.
         elif scope == LibraryPermissionScope.available:
             roles, total_roles = trans.app.security_agent.get_valid_roles(
                 trans, library, query, page, page_limit, is_library_access
             )
 
             return_roles = []
             for role in roles:
-                role_id = DecodedDatabaseIdField.encode(role.id)
-                return_roles.append(BasicRoleModel(id=role_id, name=role.name, type=role.type))
-            return LibraryAvailablePermissions.construct(
+                return_roles.append(BasicRoleModel(id=role.id, name=role.name, type=role.type))
+            return LibraryAvailablePermissions.model_construct(
                 roles=return_roles, page=page, page_limit=page_limit, total=total_roles
             )
         else:
             raise exceptions.RequestParameterInvalidException(
-                "The value of 'scope' parameter is invalid. Alllowed values: current, available"
+                "The value of 'scope' parameter is invalid. Allowed values: current, available"
             )
 
     def set_permissions(
         self, trans, id: DecodedDatabaseIdField, payload: Dict[str, Any]
     ) -> Union[LibraryLegacySummary, LibraryCurrentPermissions]:  # Old legacy response
         """Set permissions of the given library to the given role ids.
 
@@ -307,15 +306,15 @@
             trans.app.security_agent.copy_library_permissions(trans, library, library.root_folder)
         else:
             raise exceptions.RequestParameterInvalidException(
                 'The mandatory parameter "action" has an invalid value.'
                 'Allowed values are: "remove_restrictions", set_permissions"'
             )
         roles = self.library_manager.get_current_roles(trans, library)
-        return LibraryCurrentPermissions.construct(**roles)
+        return LibraryCurrentPermissions.model_construct(**roles)
 
     def set_permissions_old(self, trans, library, payload: Dict[str, Any]) -> LibraryLegacySummary:
         """
         *** old implementation for backward compatibility ***
 
         Updates the library permissions.
         """
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/library_folder_contents.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folder_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/library_folders.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/library_folders.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,15 @@
 from galaxy.exceptions import (
     InsufficientPermissionsException,
     RequestParameterInvalidException,
     RequestParameterMissingException,
 )
 from galaxy.managers.folders import FolderManager
 from galaxy.managers.roles import RoleManager
-from galaxy.schema.fields import (
-    DecodedDatabaseIdField,
-    LibraryFolderDatabaseIdField,
-)
+from galaxy.schema.fields import LibraryFolderDatabaseIdField
 from galaxy.schema.schema import (
     BasicRoleModel,
     CreateLibraryFolderPayload,
     LibraryAvailablePermissions,
     LibraryFolderCurrentPermissions,
     LibraryFolderDetails,
     LibraryPermissionScope,
@@ -50,15 +47,15 @@
         :type   id:      an encoded id string (has to be prefixed by 'F')
 
         :returns:   dictionary including details of the folder
         :rtype:     dict
         """
         folder = self.folder_manager.get(trans, folder_id, check_manageable=False, check_accessible=True)
         return_dict = self.folder_manager.get_folder_dict(trans, folder)
-        return LibraryFolderDetails.construct(**return_dict)
+        return LibraryFolderDetails(**return_dict)
 
     def create(
         self, trans, parent_folder_id: LibraryFolderDatabaseIdField, payload: CreateLibraryFolderPayload
     ) -> LibraryFolderDetails:
         """
         Create a new folder object underneath the one specified in the parameters.
 
@@ -74,15 +71,15 @@
         :returns:   information about newly created folder, notably including ID
         :rtype:     dictionary
         :raises: RequestParameterMissingException
         """
         parent_folder = self.folder_manager.get(trans, parent_folder_id)
         new_folder = self.folder_manager.create(trans, parent_folder.id, payload.name, payload.description)
         return_dict = self.folder_manager.get_folder_dict(trans, new_folder)
-        return LibraryFolderDetails.construct(**return_dict)
+        return LibraryFolderDetails(**return_dict)
 
     def get_permissions(
         self,
         trans,
         folder_id: LibraryFolderDatabaseIdField,
         scope: Optional[LibraryPermissionScope] = LibraryPermissionScope.current,
         page: int = 1,
@@ -109,25 +106,22 @@
         if not (is_admin or trans.app.security_agent.can_manage_library_item(current_user_roles, folder)):
             raise InsufficientPermissionsException(
                 "You do not have proper permission to access permissions of this folder."
             )
 
         if scope is None or scope == LibraryPermissionScope.current:
             current_permissions = self.folder_manager.get_current_roles(trans, folder)
-            return LibraryFolderCurrentPermissions.construct(**current_permissions)
+            return LibraryFolderCurrentPermissions.model_construct(**current_permissions)
         #  Return roles that are available to select.
         elif scope == LibraryPermissionScope.available:
             roles, total_roles = trans.app.security_agent.get_valid_roles(trans, folder, query, page, page_limit)
             return_roles = []
             for role in roles:
-                role_id = DecodedDatabaseIdField.encode(role.id)
-                return_roles.append(BasicRoleModel(id=role_id, name=role.name, type=role.type))
-            return LibraryAvailablePermissions.construct(
-                roles=return_roles, page=page, page_limit=page_limit, total=total_roles
-            )
+                return_roles.append(BasicRoleModel(id=role.id, name=role.name, type=role.type))
+            return LibraryAvailablePermissions(roles=return_roles, page=page, page_limit=page_limit, total=total_roles)
         else:
             raise RequestParameterInvalidException(
                 "The value of 'scope' parameter is invalid. Allowed values: current, available"
             )
 
     def set_permissions(
         self, trans, folder_id: LibraryFolderDatabaseIdField, payload: dict
@@ -223,15 +217,15 @@
 
             trans.app.security_agent.set_all_library_permissions(trans, folder, permissions)
         else:
             raise RequestParameterInvalidException(
                 'The mandatory parameter "action" has an invalid value.' 'Allowed values are: "set_permissions"'
             )
         current_permissions = self.folder_manager.get_current_roles(trans, folder)
-        return LibraryFolderCurrentPermissions.construct(**current_permissions)
+        return LibraryFolderCurrentPermissions(**current_permissions)
 
     def delete(
         self, trans, folder_id: LibraryFolderDatabaseIdField, undelete: Optional[bool] = False
     ) -> LibraryFolderDetails:
         """
         Mark the folder with the given ``encoded_folder_id`` as `deleted`
         (or remove the `deleted` mark if the `undelete` param is true).
@@ -246,15 +240,15 @@
         :returns:   detailed folder information
         :rtype:     dictionary
 
         """
         folder = self.folder_manager.get(trans, folder_id, True)
         folder = self.folder_manager.delete(trans, folder, undelete)
         folder_dict = self.folder_manager.get_folder_dict(trans, folder)
-        return LibraryFolderDetails.construct(**folder_dict)
+        return LibraryFolderDetails(**folder_dict)
 
     def update(
         self, trans, folder_id: LibraryFolderDatabaseIdField, payload: UpdateLibraryFolderPayload
     ) -> LibraryFolderDetails:
         """
          Update the folder with id ``folder_id`` with the data in the payload.
 
@@ -271,8 +265,8 @@
          :rtype:     dict
 
          :raises: RequestParameterMissingException
         """
         folder = self.folder_manager.get(trans, folder_id)
         updated_folder = self.folder_manager.update(trans, folder, payload.name, payload.description)
         folder_dict = self.folder_manager.get_folder_dict(trans, updated_folder)
-        return LibraryFolderDetails.construct(**folder_dict)
+        return LibraryFolderDetails(**folder_dict)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/notifications.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AuthenticationRequired,
     ObjectNotFound,
     RequestParameterInvalidException,
 )
 from galaxy.managers.context import ProvidesUserContext
 from galaxy.managers.notification import NotificationManager
 from galaxy.model import User
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import Security
 from galaxy.schema.notifications import (
     BroadcastNotificationCreateRequest,
     BroadcastNotificationListResponse,
     BroadcastNotificationResponse,
     NotificationBroadcastUpdateRequest,
     NotificationCreatedResponse,
     NotificationCreateRequest,
@@ -44,29 +44,30 @@
         self, sender_context: ProvidesUserContext, payload: NotificationCreateRequest
     ) -> NotificationCreatedResponse:
         """Sends a notification to a list of recipients (users, groups or roles)."""
         self.notification_manager.ensure_notifications_enabled()
         self._ensure_user_can_send_notifications(sender_context)
         notification, recipient_user_count = self.notification_manager.send_notification_to_recipients(payload)
         return NotificationCreatedResponse(
-            total_notifications_sent=recipient_user_count, notification=NotificationResponse.from_orm(notification)
+            total_notifications_sent=recipient_user_count,
+            notification=NotificationResponse.model_validate(notification),
         )
 
     def broadcast(
         self, sender_context: ProvidesUserContext, payload: BroadcastNotificationCreateRequest
     ) -> NotificationCreatedResponse:
         """Creates a notification broadcast.
 
         Broadcasted notifications are a special type of notification are accessible by every user.
         """
         self.notification_manager.ensure_notifications_enabled()
         self._ensure_user_can_broadcast_notifications(sender_context)
         notification = self.notification_manager.create_broadcast_notification(payload)
         return NotificationCreatedResponse(
-            total_notifications_sent=1, notification=NotificationResponse.from_orm(notification)
+            total_notifications_sent=1, notification=NotificationResponse.model_validate(notification)
         )
 
     def get_notifications_status(self, user_context: ProvidesUserContext, since: datetime) -> NotificationStatusSummary:
         """Returns the status of (unread or updated) notifications received by the user **since** a particular date and time.
 
         If the user is **anonymous**, only the `broadcasted notifications` will be returned.
         """
@@ -88,57 +89,57 @@
     ) -> UserNotificationListResponse:
         """Returns all the notifications received by the user that haven't expired yet..
 
         **Anonymous** users cannot receive personal notifications.
         """
         self.notification_manager.ensure_notifications_enabled()
         if user_context.anonymous:
-            return UserNotificationListResponse(__root__=[])
+            return UserNotificationListResponse(root=[])
         user_notifications = self._get_user_notifications(user_context, limit, offset)
-        return UserNotificationListResponse(__root__=user_notifications)
+        return UserNotificationListResponse(root=user_notifications)
 
     def get_broadcasted_notification(
         self, user_context: ProvidesUserContext, notification_id: int
     ) -> BroadcastNotificationResponse:
         """Gets a single `broadcasted` notification by ID.
         Admin users can access inactive notifications (scheduled or recently expired).
         """
         self.notification_manager.ensure_notifications_enabled()
         active_only = not user_context.user_is_admin
         try:
             broadcasted_notification = self.notification_manager.get_broadcasted_notification(
                 notification_id, active_only
             )
-            return BroadcastNotificationResponse.from_orm(broadcasted_notification)
+            return BroadcastNotificationResponse.model_validate(broadcasted_notification)
         except ObjectNotFound:
             self._raise_notification_not_found(notification_id)
 
     def get_all_broadcasted_notifications(self, user_context: ProvidesUserContext) -> BroadcastNotificationListResponse:
         """Gets all the `broadcasted` notifications currently published.
         Admin users will also get inactive notifications (scheduled or recently expired)."""
         self.notification_manager.ensure_notifications_enabled()
         active_only = not user_context.user_is_admin
         broadcasted_notifications = self._get_all_broadcasted(active_only=active_only)
-        return BroadcastNotificationListResponse(__root__=broadcasted_notifications)
+        return BroadcastNotificationListResponse(root=broadcasted_notifications)
 
     def get_user_notification(self, user: User, notification_id: int) -> UserNotificationResponse:
         """Gets the information of the notification received by the user with the given ID."""
         self.notification_manager.ensure_notifications_enabled()
         try:
             notification = self.notification_manager.get_user_notification(user, notification_id)
-            return UserNotificationResponse.from_orm(notification)
+            return UserNotificationResponse.model_validate(notification)
         except ObjectNotFound:
             self._raise_notification_not_found(notification_id)
 
     def update_user_notification(
         self, user_context: ProvidesUserContext, notification_id: int, request: UserNotificationUpdateRequest
     ):
         """Updates a single notification received by the user with the requested values."""
         self.notification_manager.ensure_notifications_enabled()
-        updated_response = self.update_user_notifications(user_context, set([notification_id]), request)
+        updated_response = self.update_user_notifications(user_context, {notification_id}, request)
         if not updated_response.updated_count:
             self._raise_notification_not_found(notification_id)
 
     def update_broadcasted_notification(
         self, user_context: ProvidesUserContext, notification_id: int, request: NotificationBroadcastUpdateRequest
     ):
         """Updates a single notification received by the user with the requested values."""
@@ -205,26 +206,26 @@
             raise RequestParameterInvalidException("Please specify at least one value to update for notifications.")
 
     def _get_all_broadcasted(
         self, since: Optional[datetime] = None, active_only: Optional[bool] = True
     ) -> List[BroadcastNotificationResponse]:
         notifications = self.notification_manager.get_all_broadcasted_notifications(since, active_only)
         broadcasted_notifications = [
-            BroadcastNotificationResponse.from_orm(notification) for notification in notifications
+            BroadcastNotificationResponse.model_validate(notification) for notification in notifications
         ]
         return broadcasted_notifications
 
     def _get_user_notifications(
         self,
         user_context: ProvidesUserContext,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         since: Optional[datetime] = None,
     ) -> List[UserNotificationResponse]:
         notifications = self.notification_manager.get_user_notifications(user_context.user, limit, offset, since)
-        user_notifications = [UserNotificationResponse.from_orm(notification) for notification in notifications]
+        user_notifications = [UserNotificationResponse.model_validate(notification) for notification in notifications]
         return user_notifications
 
     def _raise_notification_not_found(self, notification_id: int) -> NoReturn:
         raise ObjectNotFound(
-            f"The requested notification with id '{DecodedDatabaseIdField.encode(notification_id)}' was not found."
+            f"The requested notification with id '{Security.security.encode_id(notification_id)}' was not found."
         )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/pages.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/pages.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     PageDetails,
     PageIndexQueryPayload,
     PageSummary,
     PageSummaryList,
 )
 from galaxy.schema.tasks import GeneratePdfDownload
 from galaxy.security.idencoding import IdEncodingHelper
-from galaxy.web.short_term_storage import ShortTermStorageAllocator
+from galaxy.short_term_storage import ShortTermStorageAllocator
 from galaxy.webapps.galaxy.services.base import (
     async_task_summary,
     ensure_celery_tasks_enabled,
     ServiceBase,
 )
 from galaxy.webapps.galaxy.services.sharable import ShareableService
 
@@ -70,56 +70,66 @@
         if not trans.user_is_admin:
             user_id = trans.user and trans.user.id
             if payload.user_id and payload.user_id != user_id:
                 raise exceptions.AdminRequiredException("Only admins can index the pages of others")
 
         pages, total_matches = self.manager.index_query(trans, payload, include_total_count)
         return (
-            PageSummaryList.construct(
-                __root__=[trans.security.encode_all_ids(p.to_dict(), recursive=True) for p in pages]
-            ),
+            PageSummaryList(root=[p.to_dict() for p in pages]),
             total_matches,
         )
 
     def create(self, trans, payload: CreatePagePayload) -> PageSummary:
         """
         Create a page and return Page summary
         """
         page = self.manager.create_page(trans, payload)
-        rval = trans.security.encode_all_ids(page.to_dict(), recursive=True)
+        rval = page.to_dict()
         rval["content"] = page.latest_revision.content
         self.manager.rewrite_content_for_export(trans, rval)
-        return PageSummary.construct(**rval)
+        return PageSummary(**rval)
 
     def delete(self, trans, id: DecodedDatabaseIdField):
         """
         Mark page as deleted
 
         :param  id:    ID of the page to be deleted
         """
         page = base.get_object(trans, id, "Page", check_ownership=True)
 
         page.deleted = True
         with transaction(trans.sa_session):
             trans.sa_session.commit()
 
+    def undelete(self, trans, id: DecodedDatabaseIdField):
+        """
+        Undelete page
+
+        :param  id:    ID of the page to be undeleted
+        """
+        page = base.get_object(trans, id, "Page", check_ownership=True)
+
+        page.deleted = False
+        with transaction(trans.sa_session):
+            trans.sa_session.commit()
+
     def show(self, trans, id: DecodedDatabaseIdField) -> PageDetails:
         """View a page summary and the content of the latest revision
 
         :param  id:    ID of page to be displayed
 
         :rtype:     dict
         :returns:   Dictionary return of the Page.to_dict call with the 'content' field populated by the most recent revision
         """
         page = base.get_object(trans, id, "Page", check_ownership=False, check_accessible=True)
-        rval = trans.security.encode_all_ids(page.to_dict(), recursive=True)
+        rval = page.to_dict()
         rval["content"] = page.latest_revision.content
         rval["content_format"] = page.latest_revision.content_format
         self.manager.rewrite_content_for_export(trans, rval)
-        return PageDetails.construct(**rval)
+        return PageDetails(**rval)
 
     def show_pdf(self, trans, id: DecodedDatabaseIdField):
         """
         View a page summary and the content of the latest revision as PDF.
 
         :param  id: ID of page to be displayed
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/quotas.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/quotas.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     CreateQuotaResult,
     DefaultQuotaValues,
     DeleteQuotaPayload,
     QuotaDetails,
     QuotaSummaryList,
     UpdateQuotaParams,
 )
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import (
+    DecodedDatabaseIdField,
+    Security,
+)
 from galaxy.security.idencoding import IdEncodingHelper
 from galaxy.web import url_for
 from galaxy.webapps.galaxy.services.base import ServiceBase
 
 log = logging.getLogger(__name__)
 
 
@@ -44,41 +47,39 @@
         if deleted:
             route = "deleted_quota"
             quotas = get_quotas(trans.sa_session, deleted=True)
         else:
             route = "quota"
             quotas = get_quotas(trans.sa_session, deleted=False)
         for quota in quotas:
-            item = quota.to_dict(value_mapper={"id": DecodedDatabaseIdField.encode})
-            encoded_id = DecodedDatabaseIdField.encode(quota.id)
+            item = quota.to_dict()
+            encoded_id = Security.security.encode_id(quota.id)
             item["url"] = url_for(route, id=encoded_id)
             rval.append(item)
-        return QuotaSummaryList.construct(__root__=rval)
+        return QuotaSummaryList(root=rval)
 
     def show(self, trans: ProvidesUserContext, id: DecodedDatabaseIdField, deleted: bool = False) -> QuotaDetails:
         """Displays information about a quota."""
         quota = self.quota_manager.get_quota(trans, id, deleted=deleted)
-        rval = quota.to_dict(
-            view="element", value_mapper={"id": DecodedDatabaseIdField.encode, "total_disk_usage": float}
-        )
-        return QuotaDetails.construct(**rval)
+        rval = quota.to_dict(view="element", value_mapper={"total_disk_usage": float})
+        return QuotaDetails(**rval)
 
     def create(self, trans: ProvidesUserContext, params: CreateQuotaParams) -> CreateQuotaResult:
         """Creates a new quota."""
-        payload = params.dict()
+        payload = params.model_dump()
         self.validate_in_users_and_groups(trans, payload)
         quota, message = self.quota_manager.create_quota(payload)
-        item = quota.to_dict(value_mapper={"id": DecodedDatabaseIdField.encode})
-        item["url"] = url_for("quota", id=DecodedDatabaseIdField.encode(quota.id))
+        item = quota.to_dict()
+        item["url"] = url_for("quota", id=Security.security.encode_id(quota.id))
         item["message"] = message
-        return CreateQuotaResult.construct(**item)
+        return CreateQuotaResult(**item)
 
     def update(self, trans: ProvidesUserContext, id: DecodedDatabaseIdField, params: UpdateQuotaParams) -> str:
         """Modifies a quota."""
-        payload = params.dict()
+        payload = params.model_dump()
         self.validate_in_users_and_groups(trans, payload)
         quota = self.quota_manager.get_quota(trans, id, deleted=False)
 
         params = UpdateQuotaParams(**payload)
         # FIXME: Doing it this way makes the update non-atomic if a method fails after an earlier one has succeeded.
         methods = []
         if params.name or params.description:
@@ -106,14 +107,19 @@
             trans, id, deleted=False
         )  # deleted quotas are not technically members of this collection
         message = self.quota_manager.delete_quota(quota)
         if payload and payload.purge:
             message += self.quota_manager.purge_quota(quota)
         return message
 
+    def purge(self, trans: ProvidesUserContext, id: DecodedDatabaseIdField) -> str:
+        """Purges a previously deleted quota."""
+        quota = self.quota_manager.get_quota(trans, id, deleted=True)
+        return self.quota_manager.purge_quota(quota)
+
     def undelete(self, trans: ProvidesUserContext, id: DecodedDatabaseIdField) -> str:
         """Restores a previously deleted quota."""
         quota = self.quota_manager.get_quota(trans, id, deleted=True)
         return self.quota_manager.undelete_quota(quota)
 
     def validate_in_users_and_groups(self, trans, payload):
         """
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/sharable.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/sharable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import (
     Dict,
     List,
     Optional,
     Set,
     Tuple,
+    Type,
     Union,
 )
 
 from sqlalchemy import false
 
 from galaxy.managers import base
 from galaxy.managers.notification import NotificationManager
@@ -56,14 +57,16 @@
     Provides the common logic used by the API to share *any* kind of
     resource with other users.
 
     The Manager class of the particular resource must implement the SharableModelManager
     and have a compatible SharableModelSerializer implementation.
     """
 
+    share_with_status_cls: Type[ShareWithStatus] = ShareWithStatus
+
     def __init__(
         self,
         manager: SharableModelManager,
         serializer: SharableModelSerializer,
         notification_manager: NotificationManager,
     ) -> None:
         self.manager = manager
@@ -108,16 +111,15 @@
         return self._get_sharing_status(trans, item)
 
     def share_with_users(self, trans, id: DecodedDatabaseIdField, payload: ShareWithPayload) -> ShareWithStatus:
         item = self._get_item_by_id(trans, id)
         users, errors = self._get_users(trans, payload.user_ids)
         extra, users_to_notify = self._share_with_options(trans, item, users, errors, payload.share_option)
         base_status = self._get_sharing_status(trans, item)
-        status = ShareWithStatus.construct(**base_status.dict())
-        status.extra = extra
+        status = self.share_with_status_cls.model_construct(**base_status.model_dump(), extra=extra)
         status.errors.extend(errors)
         self._send_notification_to_users(users_to_notify, item, status)
         return status
 
     def _share_with_options(
         self,
         trans,
@@ -135,20 +137,19 @@
 
     def _get_item_by_id(self, trans, id: DecodedDatabaseIdField):
         class_name = self.manager.model_class.__name__
         item = base.get_object(trans, id, class_name, check_ownership=True, check_accessible=True, deleted=False)
         return item
 
     def _get_sharing_status(self, trans, item):
-        status = self.serializer.serialize_to_view(item, user=trans.user, trans=trans, default_view="sharing")
-        status["users_shared_with"] = [
-            {"id": self.manager.app.security.encode_id(a.user.id), "email": a.user.email}
-            for a in item.users_shared_with
-        ]
-        return SharingStatus.construct(**status)
+        status = self.serializer.serialize_to_view(
+            item, user=trans.user, trans=trans, default_view="sharing", encode_id=False
+        )
+        status["users_shared_with"] = [{"id": a.user.id, "email": a.user.email} for a in item.users_shared_with]
+        return SharingStatus(**status)
 
     def _get_users(self, trans, emails_or_ids: List[UserIdentifier]) -> Tuple[Set[User], Set[str]]:
         send_to_users: Set[User] = set()
         send_to_err: Set[str] = set()
         for email_or_id in set(emails_or_ids):
             send_to_user = None
             if isinstance(email_or_id, int):
@@ -190,15 +191,15 @@
 
     @staticmethod
     def build_notification_request(
         item: SharableItem, users_to_notify: Set[User], status: ShareWithStatus
     ) -> NotificationCreateRequest:
         user_ids = [user.id for user in users_to_notify]
         request = NotificationCreateRequest(
-            recipients=NotificationRecipients.construct(user_ids=user_ids),
+            recipients=NotificationRecipients.model_construct(user_ids=user_ids),
             notification=NotificationCreateData(
                 source=SharedItemNotificationFactory.source,
                 variant="info",
                 category=PersonalNotificationCategory.new_shared_item,
                 content=NewSharedItemNotificationContent(
                     item_type=SharedItemNotificationFactory.type_map[type(item)],
                     item_name=status.title,
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/storage_cleaner.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/storage_cleaner.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/tool_shed_repositories.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tool_shed_repositories.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,18 @@
     cast,
     Integer,
     select,
 )
 
 from galaxy.model.scoped_session import install_model_scoped_session
 from galaxy.model.tool_shed_install import ToolShedRepository
-from galaxy.schema.fields import DecodedDatabaseIdField
+from galaxy.schema.fields import (
+    DecodedDatabaseIdField,
+    Security,
+)
 from galaxy.schema.schema import (
     CheckForUpdatesResponse,
     InstalledToolShedRepository,
 )
 from galaxy.tool_shed.util.repository_util import check_for_updates
 from galaxy.util.tool_shed.tool_shed_registry import Registry
 from galaxy.web import url_for
@@ -58,16 +61,15 @@
 
     def check_for_updates(self, repository_id: Optional[int]) -> CheckForUpdatesResponse:
         message, status = check_for_updates(self._tool_shed_registry, self._install_model_context, repository_id)
         return CheckForUpdatesResponse(message=message, status=status)
 
     def _show(self, tool_shed_repository: ToolShedRepository) -> InstalledToolShedRepository:
         tool_shed_repository_dict = tool_shed_repository.as_dict()
-        encoded_id = DecodedDatabaseIdField.encode(tool_shed_repository.id)
-        tool_shed_repository_dict["id"] = encoded_id
+        encoded_id = Security.security.encode_id(tool_shed_repository.id)
         tool_shed_repository_dict["error_message"] = tool_shed_repository.error_message or ""
         tool_shed_repository_dict["url"] = url_for("tool_shed_repositories", id=encoded_id)
         return InstalledToolShedRepository(**tool_shed_repository_dict)
 
     def _get_tool_shed_repositories(self, **kwd):
         stmt = select(ToolShedRepository)
         for key, value in kwd.items():
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/tools.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def create_fetch(
         self,
         trans: ProvidesHistoryContext,
         fetch_payload: Union[FetchDataFormPayload, FetchDataPayload],
         files: Optional[List[UploadFile]] = None,
     ):
-        payload = fetch_payload.dict(exclude_unset=True)
+        payload = fetch_payload.model_dump(exclude_unset=True)
         request_version = "1"
         history_id = payload.pop("history_id")
         clean_payload = {}
         files_payload = {}
         if files:
             for i, upload_file in enumerate(files):
                 with tempfile.NamedTemporaryFile(
@@ -130,16 +130,15 @@
                 log.warning(
                     f'User "{trans.user.email}" attempts to execute tool, but account activation is turned on and user account is not active.'
                 )
 
         # Set running history from payload parameters.
         # History not set correctly as part of this API call for
         # dataset upload.
-        history_id = payload.get("history_id")
-        if history_id:
+        if history_id := payload.get("history_id"):
             history_id = trans.security.decode_id(history_id) if isinstance(history_id, str) else history_id
             target_history = self.history_manager.get_mutable(history_id, trans.user, current_history=trans.history)
         else:
             target_history = None
 
         # Set up inputs.
         inputs = payload.get("inputs", {})
@@ -197,31 +196,30 @@
         return self._handle_inputs_output_to_api_response(trans, tool, target_history, vars)
 
     def _handle_inputs_output_to_api_response(self, trans, tool, target_history, vars):
         # TODO: check for errors and ensure that output dataset(s) are available.
         output_datasets = vars.get("out_data", [])
         rval: Dict[str, Any] = {"outputs": [], "output_collections": [], "jobs": [], "implicit_collections": []}
         rval["produces_entry_points"] = tool.produces_entry_points
-        job_errors = vars.get("job_errors", [])
-        if job_errors:
+        if job_errors := vars.get("job_errors", []):
             # If we are here - some jobs were successfully executed but some failed.
             rval["errors"] = job_errors
 
         outputs = rval["outputs"]
         # TODO:?? poss. only return ids?
         for output_name, output in output_datasets:
             output_dict = output.to_dict()
             # add the output name back into the output data structure
             # so it's possible to figure out which newly created elements
             # correspond with which tool file outputs
             output_dict["output_name"] = output_name
-            outputs.append(trans.security.encode_dict_ids(output_dict, skip_startswith="metadata_"))
+            outputs.append(output_dict)
 
         for job in vars.get("jobs", []):
-            rval["jobs"].append(self.encode_all_ids(job.to_dict(view="collection"), recursive=True))
+            rval["jobs"].append(job.to_dict(view="collection"))
 
         for output_name, collection_instance in vars.get("output_collections", []):
             history = target_history or trans.history
             output_dict = dictify_dataset_collection_instance(
                 collection_instance,
                 security=trans.security,
                 url_builder=trans.url_builder,
@@ -237,14 +235,15 @@
                 security=trans.security,
                 url_builder=trans.url_builder,
                 parent=history,
             )
             output_dict["output_name"] = output_name
             rval["implicit_collections"].append(output_dict)
 
+        trans.security.encode_all_ids(rval, recursive=True)
         return rval
 
     def _search(self, q, view):
         """
         Perform the search on the given query.
         Boosts and numer of results are configurable in galaxy.ini file.
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/users.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/users.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,48 +66,49 @@
         self.user_serializer = user_serializer
         self.user_deserializer = user_deserializer
         self.quota_agent = quota_agent
 
     def recalculate_disk_usage(
         self,
         trans: ProvidesUserContext,
+        user_id: int,
     ):
         if trans.anonymous:
             raise glx_exceptions.AuthenticationRequired("Only registered users can recalculate disk usage.")
         if trans.app.config.enable_celery_tasks:
             from galaxy.celery.tasks import recalculate_user_disk_usage
 
-            result = recalculate_user_disk_usage.delay(task_user_id=getattr(trans.user, "id", None))
+            result = recalculate_user_disk_usage.delay(task_user_id=user_id)
             return async_task_summary(result)
         else:
             send_local_control_task(
                 trans.app,
                 "recalculate_user_disk_usage",
                 kwargs={
-                    "user_id": trans.user.id,
+                    "user_id": user_id,
                 },
             )
             return None
 
     def get_api_key(self, trans: ProvidesUserContext, user_id: int) -> Optional[APIKeyModel]:
         """Returns the current API key or None if the user doesn't have any valid API key."""
         user = self.get_user(trans, user_id)
         api_key = self.api_key_manager.get_api_key(user)
-        return APIKeyModel.construct(key=api_key.key, create_time=api_key.create_time) if api_key else None
+        return APIKeyModel.model_construct(key=api_key.key, create_time=api_key.create_time) if api_key else None
 
     def get_or_create_api_key(self, trans: ProvidesUserContext, user_id: int) -> str:
         """Returns the current API key (as plain string) or creates a new one."""
         user = self.get_user(trans, user_id)
         return self.api_key_manager.get_or_create_api_key(user)
 
     def create_api_key(self, trans: ProvidesUserContext, user_id: int) -> APIKeyModel:
         """Creates a new API key for the given user"""
         user = self.get_user(trans, user_id)
         api_key = self.api_key_manager.create_api_key(user)
-        result = APIKeyModel.construct(key=api_key.key, create_time=api_key.create_time)
+        result = APIKeyModel.model_construct(key=api_key.key, create_time=api_key.create_time)
         return result
 
     def delete_api_key(self, trans: ProvidesUserContext, user_id: int) -> None:
         """Deletes a particular API key"""
         user = self.get_user(trans, user_id)
         self.api_key_manager.delete_api_key(user)
 
@@ -117,19 +118,19 @@
             raise glx_exceptions.InsufficientPermissionsException("Access denied.")
         user = self.user_manager.by_id(user_id)
         return user
 
     def _anon_user_api_value(self, trans: ProvidesHistoryContext):
         """Return data for an anonymous user, truncated to only usage and quota_percent"""
         if not trans.user and not trans.history:
-            # Can't return info about this user, may not have a history yet.
-            # return {}
-            raise glx_exceptions.MessageException(err_msg="The user has no history, which should always be the case.")
-        usage = self.quota_agent.get_usage(trans, history=trans.history)
-        percent = self.quota_agent.get_percent(trans=trans, usage=usage)
+            usage: Optional[float] = 0.0
+            percent: Optional[int] = 0
+        else:
+            usage = self.quota_agent.get_usage(trans, history=trans.history)
+            percent = self.quota_agent.get_percent(trans=trans, usage=usage)
         usage = usage or 0
         return {
             "total_disk_usage": int(usage),
             "nice_total_disk_usage": util.nice_size(usage),
             "quota_percent": percent,
         }
 
@@ -189,15 +190,15 @@
         anon_response = self._anon_user_api_value(trans)
         return AnonUserModel(**anon_response)
 
     def user_to_detailed_model(
         self,
         user: User,
     ) -> DetailedUserModel:
-        user_response = self.user_serializer.serialize_to_view(user, view="detailed")
+        user_response = self.user_serializer.serialize_to_view(user, view="detailed", encode_id=False)
         return DetailedUserModel(**user_response)
 
     def get_index(
         self,
         trans: ProvidesUserContext,
         deleted: bool,
         f_email: Optional[str],
@@ -234,19 +235,22 @@
             # special case2: if the galaxy admin has specified that other user email/names are
             #   exposed, we don't want special case #1
             if (
                 not trans.user_is_admin
                 and not trans.app.config.expose_user_name
                 and not trans.app.config.expose_user_email
             ):
-                item = trans.user.to_dict(value_mapper={"id": trans.security.encode_id})
-                return [item]
+                if trans.user:
+                    item = trans.user.to_dict()
+                    return [item]
+                else:
+                    return []
             stmt = stmt.filter(User.deleted == false())
         for user in trans.sa_session.scalars(stmt).all():
-            item = user.to_dict(value_mapper={"id": trans.security.encode_id})
+            item = user.to_dict()
             # If NOT configured to expose_email, do not expose email UNLESS the user is self, or
             # the user is an admin
             if user is not trans.user and not trans.user_is_admin:
                 expose_keys = ["id"]
                 if trans.app.config.expose_user_name:
                     expose_keys.append("username")
                 if trans.app.config.expose_user_email:
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/galaxy/services/visualizations.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/galaxy/services/visualizations.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,10 +53,10 @@
         if not trans.user_is_admin:
             user_id = trans.user and trans.user.id
             if payload.user_id and payload.user_id != user_id:
                 raise exceptions.AdminRequiredException("Only admins can index the visualizations of others")
 
         entries, total_matches = self.manager.index_query(trans, payload, include_total_count)
         return (
-            VisualizationSummaryList(__root__=[entry.to_dict() for entry in entries]),
+            VisualizationSummaryList(root=[entry.to_dict() for entry in entries]),
             total_matches,
         )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/app.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/app.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/buildapp.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/buildapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Provides factory methods to assemble the Galaxy web application
 """
+
 import atexit
 import logging
 import os
 from inspect import isclass
 
 from paste import httpexceptions
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/config.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Universe configuration builder."""
+
 import logging
 import os
 import re
 
 from galaxy.util import string_as_bool
 
 log = logging.getLogger(__name__)
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/history.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/history.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,25 +155,24 @@
             - the name of history
             - the number of dataset foreach type
         """
         message = escape(util.restore_text(kwd.get("message", "")))
         user_cutoff = int(kwd.get("user_cutoff", 60))
         descending = 1 if kwd.get("descending", "desc") == "desc" else -1
         reverse = descending == 1
-        user_selection = kwd.get("user_selection", None)
 
         # select d.state, h.name
         # from dataset d, history h , history_dataset_association hda
         # where hda.history_id=h.id and hda.dataset_id=d.id order by h.state;
         from_obj = [
             galaxy.model.Dataset.table,
             galaxy.model.History.table,
             galaxy.model.HistoryDatasetAssociation.table,
         ]
-        if user_selection is not None:
+        if (user_selection := kwd.get("user_selection", None)) is not None:
             from_obj.append(galaxy.model.User.table)
             whereclause = and_(
                 galaxy.model.Dataset.table.c.id == galaxy.model.HistoryDatasetAssociation.table.c.dataset_id,
                 galaxy.model.History.table.c.id == galaxy.model.HistoryDatasetAssociation.table.c.history_id,
                 galaxy.model.User.table.c.id == galaxy.model.History.table.c.user_id,
                 galaxy.model.User.table.c.email == user_selection,
             )
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/home.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/home.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/jobs.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,14 @@
             .join(model.User)
             .filter(model.Job.table.c.user_id != monitor_user_id)
             .enable_eagerloads(False)
         )
 
 
 class Jobs(BaseUIController, ReportQueryBuilder):
-
     """
     Class contains functions for querying data requested by user via the webapp. It exposes the functions and
     responds to requests with the filled .mako templates.
     """
 
     specified_date_list_grid = SpecifiedDateListGrid()
 
@@ -1302,11 +1301,10 @@
 
 
 def get_monitor_id(trans, monitor_email):
     """
     A convenience method to obtain the monitor job id.
     """
     monitor_user_id = None
-    monitor_row = get_user_by_email(trans.sa_session, monitor_email)
-    if monitor_row is not None:
+    if (monitor_row := get_user_by_email(trans.sa_session, monitor_email)) is not None:
         monitor_user_id = monitor_row[0]
     return monitor_user_id
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/query.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Mixin to help build advanced queries for reports interface.
 """
+
 import sqlalchemy as sa
 
 
 class ReportQueryBuilder:
     def group_by_month(self, column):
         if self.app.targets_mysql:
             return [sa.func.year(column), sa.func.month(sa.func.date(column))]
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/system.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/system.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/tools.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/tools.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/users.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/users.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/controllers/workflows.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/controllers/workflows.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/fast_app.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_app.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,9 +18,10 @@
         docs_url="/api/docs",
         redoc_url="/api/redoc",
     )
     add_exception_handler(app)
     add_request_id_middleware(app)
     include_all_package_routers(app, "galaxy.webapps.reports.api")
     wsgi_handler = WSGIMiddleware(gx_webapp)
-    app.mount("/", wsgi_handler)
+    # https://github.com/abersheeran/a2wsgi/issues/44
+    app.mount("/", wsgi_handler)  # type: ignore[arg-type]
     return app
```

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/reports/fast_factory.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/reports/fast_factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy/webapps/util.py` & `galaxy-web-apps-24.0.0/galaxy/webapps/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/PKG-INFO` & `galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,70 @@
 Metadata-Version: 2.1
 Name: galaxy-web-apps
-Version: 23.2.1
+Version: 24.0.0
 Summary: Galaxy web apps
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: galaxy-app
+Requires-Dist: galaxy-data
+Requires-Dist: galaxy-job-execution
+Requires-Dist: galaxy-tool-util
+Requires-Dist: galaxy-util[jstree,template]
+Requires-Dist: galaxy-web-framework
+Requires-Dist: galaxy-web-stack
+Requires-Dist: a2wsgi
+Requires-Dist: apispec
+Requires-Dist: Babel
+Requires-Dist: Cheetah3
+Requires-Dist: fastapi>=0.101.0
+Requires-Dist: gunicorn
+Requires-Dist: gxformat2
+Requires-Dist: importlib-resources; python_version < "3.9"
+Requires-Dist: Mako
+Requires-Dist: MarkupSafe
+Requires-Dist: mercurial
+Requires-Dist: Paste
+Requires-Dist: pydantic!=2.6.0,!=2.6.1,>=2
+Requires-Dist: PyJWT
+Requires-Dist: python-dateutil
+Requires-Dist: python-multipart
+Requires-Dist: PyYAML
+Requires-Dist: requests
+Requires-Dist: Routes
+Requires-Dist: SQLAlchemy<2,>=1.4.25
+Requires-Dist: sqlalchemy-migrate
+Requires-Dist: starlette
+Requires-Dist: starlette-context
+Requires-Dist: tuswsgi
+Requires-Dist: typing-extensions
+Requires-Dist: uvicorn
+Requires-Dist: uvloop
+Requires-Dist: WebOb
+Requires-Dist: Whoosh
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-apps.svg
    :target: https://pypi.python.org/pypi/galaxy-web-apps/
 
 
 Overview
@@ -42,14 +78,93 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.0 (2024-04-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* tus wants a json response from v2.0.0 by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17246 <https://github.com/galaxyproject/galaxy/pull/17246>`_
+* Fix quotas ID encoding by `@davelopez <https://github.com/davelopez>`_ in `#17335 <https://github.com/galaxyproject/galaxy/pull/17335>`_
+* Fixes for flake8-bugbear 24.1.17 by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17340 <https://github.com/galaxyproject/galaxy/pull/17340>`_
+* Fix data_source and data_source_async bugs by `@wm75 <https://github.com/wm75>`_ in `#17422 <https://github.com/galaxyproject/galaxy/pull/17422>`_
+* Only check access permissions in ``/api/{history_dataset_collection_id}/contents/{dataset_collection_id}`` by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17444 <https://github.com/galaxyproject/galaxy/pull/17444>`_
+* Associate default history with session when creating a new session by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17557 <https://github.com/galaxyproject/galaxy/pull/17557>`_
+* Fix tool shed webapp by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17597 <https://github.com/galaxyproject/galaxy/pull/17597>`_
+* Don't call ``get_or_create_default_history()`` twice for invalidated sessions by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17613 <https://github.com/galaxyproject/galaxy/pull/17613>`_
+* Fix tool panel workflow and favorites button bugs by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17634 <https://github.com/galaxyproject/galaxy/pull/17634>`_
+* Fix DataResult type by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17639 <https://github.com/galaxyproject/galaxy/pull/17639>`_
+* Prevent 500 for anon /api/invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17640 <https://github.com/galaxyproject/galaxy/pull/17640>`_
+* Don't fail for anon /api/users request by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17645 <https://github.com/galaxyproject/galaxy/pull/17645>`_
+* Limit new anon histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17657 <https://github.com/galaxyproject/galaxy/pull/17657>`_
+* Fix histories API index_query serialization by `@davelopez <https://github.com/davelopez>`_ in `#17726 <https://github.com/galaxyproject/galaxy/pull/17726>`_
+* Handle missing indexer for a dataset by `@ahmedhamidawan <https://github.com/ahmedhamidawan>`_ in `#17736 <https://github.com/galaxyproject/galaxy/pull/17736>`_
+* Don't require history to calculate anon disk usage by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17765 <https://github.com/galaxyproject/galaxy/pull/17765>`_
+* Fix anon user values again by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17772 <https://github.com/galaxyproject/galaxy/pull/17772>`_
+* Fix new default history creation when in remote or single user mode by `@dannon <https://github.com/dannon>`_ in `#17796 <https://github.com/galaxyproject/galaxy/pull/17796>`_
+* Return published histories first in display_by_username_and_slug by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17808 <https://github.com/galaxyproject/galaxy/pull/17808>`_
+* Fix archived histories mixing with active in histories list by `@davelopez <https://github.com/davelopez>`_ in `#17856 <https://github.com/galaxyproject/galaxy/pull/17856>`_
+
+============
+Enhancements
+============
+
+* New Workflow List and Card View by `@itisAliRH <https://github.com/itisAliRH>`_ in `#16607 <https://github.com/galaxyproject/galaxy/pull/16607>`_
+* port invocation API to fastapi by `@martenson <https://github.com/martenson>`_ in `#16707 <https://github.com/galaxyproject/galaxy/pull/16707>`_
+* Python 3.8 as minimum by `@mr-c <https://github.com/mr-c>`_ in `#16954 <https://github.com/galaxyproject/galaxy/pull/16954>`_
+* Support for OIDC API Auth and OIDC integration tests by `@nuwang <https://github.com/nuwang>`_ in `#16977 <https://github.com/galaxyproject/galaxy/pull/16977>`_
+* Toward declarative help for Galaxy markdown directives. by `@jmchilton <https://github.com/jmchilton>`_ in `#16979 <https://github.com/galaxyproject/galaxy/pull/16979>`_
+* Vueify Admin User Grid by `@guerler <https://github.com/guerler>`_ in `#17030 <https://github.com/galaxyproject/galaxy/pull/17030>`_
+* Remove web framework dependency from tools by `@davelopez <https://github.com/davelopez>`_ in `#17058 <https://github.com/galaxyproject/galaxy/pull/17058>`_
+* Vueify Admin Roles Grid by `@guerler <https://github.com/guerler>`_ in `#17118 <https://github.com/galaxyproject/galaxy/pull/17118>`_
+* SA2.0 updates: handling "object is being merged into a Session along the backref cascade path" by `@jdavcs <https://github.com/jdavcs>`_ in `#17122 <https://github.com/galaxyproject/galaxy/pull/17122>`_
+* Vueify Admin Groups Grid by `@guerler <https://github.com/guerler>`_ in `#17126 <https://github.com/galaxyproject/galaxy/pull/17126>`_
+* Towards SQLAlchemy 2.0: fix last cases of RemovedIn20Warning by `@jdavcs <https://github.com/jdavcs>`_ in `#17132 <https://github.com/galaxyproject/galaxy/pull/17132>`_
+* Vueify Admin Forms and Quota grids by `@guerler <https://github.com/guerler>`_ in `#17141 <https://github.com/galaxyproject/galaxy/pull/17141>`_
+* Migrate dataset extra files store to Pinia by `@davelopez <https://github.com/davelopez>`_ in `#17145 <https://github.com/galaxyproject/galaxy/pull/17145>`_
+* Create pydantic model for the return of show operation -  get: `/api/jobs/{job_id}`  by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17153 <https://github.com/galaxyproject/galaxy/pull/17153>`_
+* Remove legacy tool versions list from admin panel by `@guerler <https://github.com/guerler>`_ in `#17155 <https://github.com/galaxyproject/galaxy/pull/17155>`_
+* Don't require admin user to list ``/api/tool_data`` by `@jozh2008 <https://github.com/jozh2008>`_ in `#17161 <https://github.com/galaxyproject/galaxy/pull/17161>`_
+* Drop fastapi-utils.InferringRouter in favor of fastapi.APIRouter  by `@jdavcs <https://github.com/jdavcs>`_ in `#17184 <https://github.com/galaxyproject/galaxy/pull/17184>`_
+* Vendorize fastapi-utls.cbv by `@jdavcs <https://github.com/jdavcs>`_ in `#17205 <https://github.com/galaxyproject/galaxy/pull/17205>`_
+* Vueifiy History Grids by `@guerler <https://github.com/guerler>`_ in `#17219 <https://github.com/galaxyproject/galaxy/pull/17219>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17235 <https://github.com/galaxyproject/galaxy/pull/17235>`_
+* Refactor two of the missing invocation routes to FastAPI by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17237 <https://github.com/galaxyproject/galaxy/pull/17237>`_
+* Allow job files to consume TUS uploads by `@jmchilton <https://github.com/jmchilton>`_ in `#17242 <https://github.com/galaxyproject/galaxy/pull/17242>`_
+* Migrate models to pydantic 2 by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17262 <https://github.com/galaxyproject/galaxy/pull/17262>`_
+* Adds delete, purge and undelete batch operations to History Grid by `@guerler <https://github.com/guerler>`_ in `#17282 <https://github.com/galaxyproject/galaxy/pull/17282>`_
+* Fix any type for tool_data_file_path by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17293 <https://github.com/galaxyproject/galaxy/pull/17293>`_
+* API endpoint that allows "changing" the objectstore for "safe" scenarios.  by `@jmchilton <https://github.com/jmchilton>`_ in `#17329 <https://github.com/galaxyproject/galaxy/pull/17329>`_
+* Update Python dependencies by `@galaxybot <https://github.com/galaxybot>`_ in `#17333 <https://github.com/galaxyproject/galaxy/pull/17333>`_
+* Combines legacy qv-pattern and advanced filter pattern in history index endpoint by `@guerler <https://github.com/guerler>`_ in `#17368 <https://github.com/galaxyproject/galaxy/pull/17368>`_
+* Update to black 2024 stable style by `@nsoranzo <https://github.com/nsoranzo>`_ in `#17391 <https://github.com/galaxyproject/galaxy/pull/17391>`_
+* Replaces Trackster Grids with Data Dialog, Removes Phyloviz, Circster and Sweepster by `@guerler <https://github.com/guerler>`_ in `#17415 <https://github.com/galaxyproject/galaxy/pull/17415>`_
+* Removes outdated Grid controller and backbone modules by `@guerler <https://github.com/guerler>`_ in `#17434 <https://github.com/galaxyproject/galaxy/pull/17434>`_
+* Allow using tool data bundles as inputs to reference data select parameters by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17435 <https://github.com/galaxyproject/galaxy/pull/17435>`_
+* Modernize bits and pieces of storage display by `@jmchilton <https://github.com/jmchilton>`_ in `#17436 <https://github.com/galaxyproject/galaxy/pull/17436>`_
+* UI for "relocating" a dataset to a new object store (when safe) by `@jmchilton <https://github.com/jmchilton>`_ in `#17437 <https://github.com/galaxyproject/galaxy/pull/17437>`_
+* Refactor Workflow API routes - Part 1 by `@heisner-tillman <https://github.com/heisner-tillman>`_ in `#17463 <https://github.com/galaxyproject/galaxy/pull/17463>`_
+* Consolidate resource grids into tab views by `@guerler <https://github.com/guerler>`_ in `#17487 <https://github.com/galaxyproject/galaxy/pull/17487>`_
+* Display workflow invocation counts. by `@jmchilton <https://github.com/jmchilton>`_ in `#17488 <https://github.com/galaxyproject/galaxy/pull/17488>`_
+* Removes legacy history xml makos by `@guerler <https://github.com/guerler>`_ in `#17505 <https://github.com/galaxyproject/galaxy/pull/17505>`_
+* add encode ID API endpoint by `@mira-miracoli <https://github.com/mira-miracoli>`_ in `#17510 <https://github.com/galaxyproject/galaxy/pull/17510>`_
+* Fixing data_source tools and incrementing tool profile by `@wm75 <https://github.com/wm75>`_ in `#17515 <https://github.com/galaxyproject/galaxy/pull/17515>`_
+* Filter out subworkflow invocations by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17558 <https://github.com/galaxyproject/galaxy/pull/17558>`_
+* Links to individual invocations. by `@jmchilton <https://github.com/jmchilton>`_ in `#17566 <https://github.com/galaxyproject/galaxy/pull/17566>`_
+* Restore histories API behavior for `keys` query parameter by `@davelopez <https://github.com/davelopez>`_ in `#17779 <https://github.com/galaxyproject/galaxy/pull/17779>`_
+* Fix datasets API custom keys encoding by `@davelopez <https://github.com/davelopez>`_ in `#17793 <https://github.com/galaxyproject/galaxy/pull/17793>`_
+
+-------------------
 23.2.1 (2024-02-21)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-web-apps-23.2.1/galaxy_web_apps.egg-info/SOURCES.txt` & `galaxy-web-apps-24.0.0/galaxy_web_apps.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -266,19 +266,15 @@
 galaxy/webapps/base/templates/legacy/grid_base_async.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/binary_file.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/copy_view.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/display.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/large_file.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/tabular_chunked.mako
 galaxy/webapps/base/templates/webapps/galaxy/dataset/display_application/display.mako
-galaxy/webapps/base/templates/webapps/galaxy/history/as_xml.mako
-galaxy/webapps/base/templates/webapps/galaxy/history/list_as_xml.mako
 galaxy/webapps/base/templates/webapps/galaxy/root/tool_runner.mako
-galaxy/webapps/base/templates/webapps/galaxy/visualization/phyloviz.mako
-galaxy/webapps/base/templates/webapps/galaxy/visualization/sweepster.mako
 galaxy/webapps/base/templates/webapps/galaxy/visualization/trackster.mako
 galaxy/webapps/base/templates/webapps/galaxy/workflow/build_from_current_history.mako
 galaxy/webapps/base/templates/webapps/reports/base_panels.mako
 galaxy/webapps/base/templates/webapps/reports/dataset_info.mako
 galaxy/webapps/base/templates/webapps/reports/history_and_dataset_per_user.mako
 galaxy/webapps/base/templates/webapps/reports/history_and_dataset_type.mako
 galaxy/webapps/base/templates/webapps/reports/history_per_user.mako
@@ -319,14 +315,15 @@
 galaxy/webapps/galaxy/buildapp.py
 galaxy/webapps/galaxy/fast_app.py
 galaxy/webapps/galaxy/fast_factory.py
 galaxy/webapps/galaxy/workers.py
 galaxy/webapps/galaxy/api/__init__.py
 galaxy/webapps/galaxy/api/annotations.py
 galaxy/webapps/galaxy/api/authenticate.py
+galaxy/webapps/galaxy/api/cbv.py
 galaxy/webapps/galaxy/api/cloud.py
 galaxy/webapps/galaxy/api/cloudauthz.py
 galaxy/webapps/galaxy/api/common.py
 galaxy/webapps/galaxy/api/configuration.py
 galaxy/webapps/galaxy/api/container_resolution.py
 galaxy/webapps/galaxy/api/dataset_collections.py
 galaxy/webapps/galaxy/api/datasets.py
```

### Comparing `galaxy-web-apps-23.2.1/setup.cfg` & `galaxy-web-apps-24.0.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 	Development Status :: 5 - Production/Stable
 	Environment :: Console
 	Intended Audience :: Developers
 	License :: OSI Approved :: Academic Free License (AFL)
 	Natural Language :: English
 	Operating System :: POSIX
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Software Development
 	Topic :: Software Development :: Code Generators
 	Topic :: Software Development :: Testing
 description = Galaxy web apps
 keywords = 
 	Galaxy
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-web-apps
 url = https://github.com/galaxyproject/galaxy
-version = 23.2.1
+version = 24.0.0
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-app
 	galaxy-data
 	galaxy-job-execution
@@ -39,24 +39,23 @@
 	galaxy-util[jstree,template]
 	galaxy-web-framework
 	galaxy-web-stack
 	a2wsgi
 	apispec
 	Babel
 	Cheetah3
-	fastapi>=0.68.2,!=0.69.0,!=0.70.0,!=0.70.1,<0.99
-	fastapi-utils
+	fastapi>=0.101.0
 	gunicorn
 	gxformat2
-	importlib_resources
+	importlib-resources;python_version<'3.9'
 	Mako
 	MarkupSafe
 	mercurial
 	Paste
-	pydantic<2
+	pydantic>=2,!=2.6.0,!=2.6.1
 	PyJWT
 	python-dateutil
 	python-multipart  # required to support form parsing in FastAPI/Starlette
 	PyYAML
 	requests
 	Routes
 	SQLAlchemy>=1.4.25,<2
@@ -66,15 +65,15 @@
 	tuswsgi
 	typing-extensions
 	uvicorn
 	uvloop
 	WebOb
 	Whoosh
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.8
 
 [options.packages.find]
 exclude = 
 	tests*
 	tool_shed.test*
 
 [egg_info]
```

