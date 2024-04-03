# Comparing `tmp/bycon-1.6.3.tar.gz` & `tmp/bycon-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bycon-1.6.3.tar", last modified: Fri Mar  8 14:53:07 2024, max compression
+gzip compressed data, was "bycon-1.6.5.tar", last modified: Wed Apr  3 06:56:10 2024, max compression
```

## Comparing `bycon-1.6.3.tar` & `bycon-1.6.5.tar`

### file list

```diff
@@ -1,573 +1,574 @@
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.320298 bycon-1.6.3/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.188870 bycon-1.6.3/.github/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.247882 bycon-1.6.3/.github/workflows/
--rw-r--r--   0 mbaudis    (501) staff       (20)      486 2023-05-12 18:37:11.000000 bycon-1.6.3/.github/workflows/mk-bycon-docs.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      232 2023-08-22 12:24:33.000000 bycon-1.6.3/.gitignore
--rw-r--r--   0 mbaudis    (501) staff       (20)     7048 2023-05-12 18:37:11.000000 bycon-1.6.3/LICENSE
--rw-r--r--   0 mbaudis    (501) staff       (20)      124 2023-05-12 18:26:34.000000 bycon-1.6.3/MANIFEST.in
--rw-r--r--   0 mbaudis    (501) staff       (20)     2844 2024-03-08 14:53:07.320227 bycon-1.6.3/PKG-INFO
--rw-r--r--   0 mbaudis    (501) staff       (20)     1306 2023-07-24 09:02:43.000000 bycon-1.6.3/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.248203 bycon-1.6.3/bycon/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1362 2024-03-08 13:05:42.000000 bycon-1.6.3/bycon/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.250488 bycon-1.6.3/bycon/beaconServer/
--rw-r--r--   0 mbaudis    (501) staff       (20)      118 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/beaconServer/README.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:26:34.000000 bycon-1.6.3/bycon/beaconServer/__init__.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2783 2024-03-08 13:27:13.000000 bycon-1.6.3/bycon/beaconServer/beacon.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1054 2024-03-06 09:18:52.000000 bycon-1.6.3/bycon/beaconServer/cohorts.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1036 2024-02-29 12:53:03.000000 bycon-1.6.3/bycon/beaconServer/configuration.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1032 2024-03-06 10:42:26.000000 bycon-1.6.3/bycon/beaconServer/datasets.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1091 2024-02-29 12:52:31.000000 bycon-1.6.3/bycon/beaconServer/entry_types.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1098 2024-03-06 10:42:04.000000 bycon-1.6.3/bycon/beaconServer/filtering_terms.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1659 2024-03-08 13:09:44.000000 bycon-1.6.3/bycon/beaconServer/info.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1030 2024-02-29 12:53:38.000000 bycon-1.6.3/bycon/beaconServer/map.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     1147 2024-03-08 13:09:59.000000 bycon-1.6.3/bycon/beaconServer/service_info.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.252239 bycon-1.6.3/bycon/beaconServer/tests/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1215 2024-02-21 11:11:55.000000 bycon-1.6.3/bycon/beaconServer/tests/GET-examples.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      772 2024-02-07 09:34:45.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      958 2024-02-07 09:44:28.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      564 2024-02-07 09:34:45.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      450 2024-02-09 08:13:23.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      591 2024-02-07 09:43:52.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      850 2024-02-07 09:42:58.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      634 2024-02-07 09:43:23.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      897 2024-02-07 09:58:17.000000 bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      126 2024-02-07 09:50:47.000000 bycon-1.6.3/bycon/beaconServer/tests/terminal-examples.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     2572 2024-03-08 14:22:15.000000 bycon-1.6.3/bycon/config.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.253232 bycon-1.6.3/bycon/definitions/
--rw-r--r--   0 mbaudis    (501) staff       (20)    12346 2024-03-07 15:10:41.000000 bycon-1.6.3/bycon/definitions/argument_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-08-22 12:13:19.000000 bycon-1.6.3/bycon/definitions/dataset_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    15338 2024-03-06 08:49:04.000000 bycon-1.6.3/bycon/definitions/datatable_mappings.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4401 2024-03-08 14:02:13.000000 bycon-1.6.3/bycon/definitions/entity_defaults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    11612 2024-03-07 13:33:08.000000 bycon-1.6.3/bycon/definitions/filter_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2202 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/definitions/geoloc_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6329 2024-02-28 09:44:52.000000 bycon-1.6.3/bycon/definitions/handover_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2213 2024-02-14 14:30:00.000000 bycon-1.6.3/bycon/definitions/interval_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3705 2024-02-23 08:26:00.000000 bycon-1.6.3/bycon/definitions/variant_request_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5237 2024-03-01 16:09:30.000000 bycon-1.6.3/bycon/definitions/variant_type_definitions.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.256096 bycon-1.6.3/bycon/lib/
--rw-r--r--   0 mbaudis    (501) staff       (20)        0 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/lib/__init__.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1664 2024-02-29 12:32:23.000000 bycon-1.6.3/bycon/lib/args_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     2428 2024-03-06 08:59:44.000000 bycon-1.6.3/bycon/lib/beacon_auth.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    32825 2024-03-08 14:24:25.000000 bycon-1.6.3/bycon/lib/beacon_response_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    10377 2024-03-07 14:51:28.000000 bycon-1.6.3/bycon/lib/bycon_helpers.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     6664 2024-03-08 13:27:49.000000 bycon-1.6.3/bycon/lib/cgi_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     2362 2024-02-23 13:27:02.000000 bycon-1.6.3/bycon/lib/dataset_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     6584 2024-02-21 13:00:12.000000 bycon-1.6.3/bycon/lib/genome_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3587 2024-02-29 17:28:42.000000 bycon-1.6.3/bycon/lib/handover_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     1230 2024-02-21 13:34:58.000000 bycon-1.6.3/bycon/lib/parse_filters_request.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     5630 2024-02-28 08:14:57.000000 bycon-1.6.3/bycon/lib/parse_variant_request.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    11205 2024-03-06 09:36:00.000000 bycon-1.6.3/bycon/lib/query_execution.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    26694 2024-03-08 13:28:02.000000 bycon-1.6.3/bycon/lib/query_generation.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     5700 2024-03-08 14:46:16.000000 bycon-1.6.3/bycon/lib/read_specs.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    11940 2024-03-08 12:51:08.000000 bycon-1.6.3/bycon/lib/response_remapping.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     3350 2024-03-08 13:30:26.000000 bycon-1.6.3/bycon/lib/schema_parsing.py
--rw-r--r--   0 mbaudis    (501) staff       (20)     4344 2024-03-08 13:31:28.000000 bycon-1.6.3/bycon/lib/service_utils.py
--rw-r--r--   0 mbaudis    (501) staff       (20)    12264 2024-03-07 08:10:00.000000 bycon-1.6.3/bycon/lib/variant_mapping.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.256509 bycon-1.6.3/bycon/rsrc/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:53.000000 bycon-1.6.3/bycon/rsrc/.DS_Store
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.256631 bycon-1.6.3/bycon/rsrc/genomes/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2024-02-09 08:01:48.000000 bycon-1.6.3/bycon/rsrc/genomes/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.256796 bycon-1.6.3/bycon/rsrc/genomes/grch38/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30914 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)     2007 2023-06-29 20:11:54.000000 bycon-1.6.3/bycon/rsrc/genomes/grch38/refseq_chromosomes.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.256986 bycon-1.6.3/bycon/rsrc/genomes/hg16/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30743 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.257156 bycon-1.6.3/bycon/rsrc/genomes/hg17/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.257315 bycon-1.6.3/bycon/rsrc/genomes/hg18/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.257485 bycon-1.6.3/bycon/rsrc/genomes/hg19/
--rw-r--r--   0 mbaudis    (501) staff       (20)    30754 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.257657 bycon-1.6.3/bycon/rsrc/genomes/mSarHar1.11/
--rw-r--r--   0 mbaudis    (501) staff       (20)      543 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.257826 bycon-1.6.3/bycon/rsrc/genomes/mm8/
--rw-r--r--   0 mbaudis    (501) staff       (20)    13771 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.258003 bycon-1.6.3/bycon/rsrc/genomes/mm9/
--rw-r--r--   0 mbaudis    (501) staff       (20)    13786 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.258163 bycon-1.6.3/bycon/rsrc/genomes/zf7/
--rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.258595 bycon-1.6.3/bycon/schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2024-02-09 08:01:53.000000 bycon-1.6.3/bycon/schemas/.DS_Store
--rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:26:34.000000 bycon-1.6.3/bycon/schemas/README.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/__init__.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.258857 bycon-1.6.3/bycon/schemas/bin/
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     7331 2024-02-06 13:56:06.000000 bycon-1.6.3/bycon/schemas/bin/beaconYamler.py
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.199256 bycon-1.6.3/bycon/schemas/bin/config/
--rw-r--r--   0 mbaudis    (501) staff       (20)      602 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/bin/config/beaconYamler.yaml
--rwxr-xr-x   0 mbaudis    (501) staff       (20)      889 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/bin/yamlerRunner.sh
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.259035 bycon-1.6.3/bycon/schemas/framework/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.3/bycon/schemas/framework/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.259761 bycon-1.6.3/bycon/schemas/framework/json/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.260757 bycon-1.6.3/bycon/schemas/framework/json/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      572 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/basicElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    11798 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/beaconCommonComponents.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      566 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/elementWithDescription.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.261792 bycon-1.6.3/bycon/schemas/framework/json/common/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      125 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/basicElement-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1936 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      197 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/elementWithDescription-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      346 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/ontologizedElement-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      127 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/ontologyTerm-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      336 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      239 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      697 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/ontologizedElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      933 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/ontologyTerm.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1017 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/referenceToAnSchema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.261937 bycon-1.6.3/bycon/schemas/framework/json/common/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2011 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.262683 bycon-1.6.3/bycon/schemas/framework/json/configuration/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3213 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4791 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/beaconMapSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3992 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/entryTypeDefinition.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      764 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/entryTypesSchema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.263800 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2281 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      540 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      223 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconMap-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      588 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1318 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      561 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3152 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/configuration/filteringTermsSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.264392 bycon-1.6.3/bycon/schemas/framework/json/requests/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2238 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/beaconRequestBody.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      874 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/beaconRequestMeta.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.264733 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      830 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      114 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MIN-example.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.265246 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      231 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-sections/beaconRequestMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      495 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-sections/filteringTerms-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      386 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/examples-sections/requestParameters-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5169 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      452 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/requestParameters.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.265423 bycon-1.6.3/bycon/schemas/framework/json/requests/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4243 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/requests/validation/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.267756 bycon-1.6.3/bycon/schemas/framework/json/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1231 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconBooleanResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1290 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      727 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1277 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconCountResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      681 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      645 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconErrorResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      664 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      716 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconInfoResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      707 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconMapResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1454 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.269658 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      745 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2451 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      782 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2832 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1533 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2452 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1164 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1183 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1279 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      538 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1522 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      767 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.271834 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)       85 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconBooleanResponseSection-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      115 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconCountResponseSection-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      166 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconInformationalResponseMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      656 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      180 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      214 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsetEmpty-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1070 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      526 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       87 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5381 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.273673 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      522 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      730 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3545 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4676 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      896 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2688 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1801 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2444 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconResultsets.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      702 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.273966 bycon-1.6.3/bycon/schemas/framework/src/
--rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.275107 bycon-1.6.3/bycon/schemas/framework/src/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)      393 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/basicElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9289 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/framework/src/common/beaconCommonComponents.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      356 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/elementWithDescription.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.276887 bycon-1.6.3/bycon/schemas/framework/src/common/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)       96 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/basicElement-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1305 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      159 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/elementWithDescription-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      272 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/ontologizedElement-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       98 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/ontologyTerm-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      201 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      462 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/ontologizedElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/ontologyTerm.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      717 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/referenceToAnSchema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.277088 bycon-1.6.3/bycon/schemas/framework/src/common/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1459 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.278086 bycon-1.6.3/bycon/schemas/framework/src/configuration/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2395 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3917 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3395 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.279226 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1545 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      312 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconConfigurationFilteringTerms-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      152 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconMap-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      810 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      396 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_MIN_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1014 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      440 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/entryTypeDefinition-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2412 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.279840 bycon-1.6.3/bycon/schemas/framework/src/requests/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1678 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/beaconRequestBody.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      693 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.280166 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      449 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       80 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MIN-example.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.280658 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      153 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-sections/beaconRequestMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      284 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-sections/filteringTerms-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/examples-sections/requestParameters-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3535 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      340 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/requestParameters.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.280822 bycon-1.6.3/bycon/schemas/framework/src/requests/validation/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2786 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.282389 bycon-1.6.3/bycon/schemas/framework/src/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)      996 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1342 2024-02-06 13:37:14.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      565 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1042 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconCountResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      517 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      481 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconErrorResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconFilteringTermsResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      554 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      545 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconMapResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1157 2023-05-24 09:00:05.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.284290 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/
--rw-r--r--   0 mbaudis    (501) staff       (20)      418 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconBooleanResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1323 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      432 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1834 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      954 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1579 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      586 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      675 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1035 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      433 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.285865 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)       67 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconBooleanResponseSection-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       90 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconCountResponseSection-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      130 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconInformationalResponseMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      380 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      137 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResponseMeta-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResultsetEmpty-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      582 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       69 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4108 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.287638 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/
--rw-r--r--   0 mbaudis    (501) staff       (20)      424 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconBooleanResponseSection.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      579 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2403 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3084 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      679 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2269 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1472 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1589 2023-05-24 11:46:35.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      558 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.259189 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.183561 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.259554 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1369 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResponse.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      837 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResults.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.183715 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/src/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.199727 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/src/responses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1102 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResponse.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      497 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResults.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.287807 bycon-1.6.3/bycon/schemas/models/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.3/bycon/schemas/models/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.287991 bycon-1.6.3/bycon/schemas/models/json/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2023-07-29 14:31:39.000000 bycon-1.6.3/bycon/schemas/models/json/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.289220 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     7277 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxAnalysis.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7943 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6146 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2544 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2541 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.289796 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.290449 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2525 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.290805 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      399 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      180 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7268 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     7602 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/beaconMap.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.291257 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8054 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.291563 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      498 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      305 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.292057 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)    12858 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    13483 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.292512 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      161 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      288 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.297412 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4718 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5549 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/VRSallele.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     4919 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/VRScopyNumberChange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      408 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/age.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      515 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ageRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      939 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ancestry.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1122 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/celllineInfo.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5647 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1632 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/complexValue.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2465 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3142 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/disease.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/doseInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      984 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/evidence.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1642 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/exposure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1034 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/externalReference.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1269 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/file.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2039 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/measurement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      925 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/metaData.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      933 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5291 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/pedigree.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3428 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1824 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/procedure.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      923 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/provenance.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      721 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/quantity.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      961 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/referenceRange.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1150 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/resource.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      857 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/timeElement.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      835 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/timeInterval.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1745 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/treatment.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      511 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/update.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      345 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/value.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1525 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.297919 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    19091 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.298241 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      132 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      825 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.299457 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)    25440 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.299979 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3473 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      707 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      647 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      275 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/filteringTerms.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     6629 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2718 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.300458 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4870 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.301087 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      160 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.301390 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/phenopackets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    15893 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.301854 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3807 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json
--rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/endpoints.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.302157 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      532 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      178 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MIN-example.json
--rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/filteringTerms.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.303964 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3342 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Collation.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      782 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/CytobandMapping.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1779 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2422 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1999 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json
--rw-r--r--   0 mbaudis    (501) staff       (20)      370 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/OntologyClassGroup.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1314 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     3224 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     5034 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Publication.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2382 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json
--rw-r--r--   0 mbaudis    (501) staff       (20)     2936 2024-03-06 12:40:56.000000 bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.304197 bycon-1.6.3/bycon/schemas/models/src/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-29 14:30:02.000000 bycon-1.6.3/bycon/schemas/models/src/.DS_Store
--rw-r--r--   0 mbaudis    (501) staff       (20)      294 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/README.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.304664 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     4489 2024-02-24 10:53:00.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxAnalysis.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4973 2023-06-30 11:06:24.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     4181 2024-01-18 17:19:59.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1692 2023-06-23 14:30:27.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1574 2023-05-31 15:03:17.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.305088 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-08-14 11:09:55.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/.DS_Store
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.305392 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1517 2023-06-23 14:32:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.305702 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5073 2023-07-24 15:07:04.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5216 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/beaconMap.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.306009 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     7846 2023-06-22 20:21:56.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.306316 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.306766 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8616 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     7822 2024-03-06 12:40:43.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.307241 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.312746 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3565 2023-08-15 08:02:14.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3771 2023-08-11 10:39:01.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/VRSallele.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3458 2023-08-11 10:39:01.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/VRScopyNumberChange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/age.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/ageRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      585 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      747 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3893 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1015 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1160 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/disease.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1177 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/evidence.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1094 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/exposure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      765 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      884 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/file.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1281 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/measurement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      553 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/metaData.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3116 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1175 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/procedure.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1018 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/provenance.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/quantity.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      701 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/resource.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      601 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/treatment.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      362 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/update.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      229 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/value.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1200 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.313136 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)    11022 2024-03-06 11:52:16.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.313516 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       72 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.314170 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-26 11:46:15.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/.DS_Store
--rw-r--r--   0 mbaudis    (501) staff       (20)    16186 2023-08-11 10:39:01.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.314707 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/filteringTerms.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5747 2023-10-24 11:35:29.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2486 2023-11-19 15:02:46.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.315036 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/
--rw-r--r--   0 mbaudis    (501) staff       (20)     3015 2023-06-23 14:31:14.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.315691 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.316007 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/phenopackets/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1301 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     9236 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.316491 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2476 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.316789 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/examples/
--rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MAX-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MIN-example.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/filteringTerms.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.317499 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/
--rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-26 11:44:44.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/.DS_Store
--rw-r--r--   0 mbaudis    (501) staff       (20)     1859 2023-10-20 16:01:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Collation.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      664 2023-08-26 14:05:41.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/CytobandMapping.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1207 2024-01-18 17:19:59.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1590 2023-06-29 20:11:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1394 2023-06-29 20:11:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      257 2023-05-12 18:37:11.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/OntologyClassGroup.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      872 2023-06-29 20:11:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1713 2023-06-29 20:11:54.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1148 2023-08-15 07:53:42.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     3292 2023-06-09 05:05:31.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1855 2023-06-09 05:05:31.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     2131 2024-01-18 17:19:59.000000 bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.319841 bycon-1.6.3/bycon.egg-info/
--rw-r--r--   0 mbaudis    (501) staff       (20)     2844 2024-03-08 14:53:07.000000 bycon-1.6.3/bycon.egg-info/PKG-INFO
--rw-r--r--   0 mbaudis    (501) staff       (20)    60911 2024-03-08 14:53:07.000000 bycon-1.6.3/bycon.egg-info/SOURCES.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)        1 2024-03-08 14:53:07.000000 bycon-1.6.3/bycon.egg-info/dependency_links.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)       83 2024-03-08 14:53:07.000000 bycon-1.6.3/bycon.egg-info/requires.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)        6 2024-03-08 14:53:07.000000 bycon-1.6.3/bycon.egg-info/top_level.txt
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.318480 bycon-1.6.3/docs/
--rw-r--r--   0 mbaudis    (501) staff       (20)       20 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/CNAME
--rw-r--r--   0 mbaudis    (501) staff       (20)    36980 2024-03-08 14:53:00.000000 bycon-1.6.3/docs/changes.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      176 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/code-notes.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.318594 bycon-1.6.3/docs/css/
--rw-r--r--   0 mbaudis    (501) staff       (20)     1076 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/css/extra.css
--rw-r--r--   0 mbaudis    (501) staff       (20)     3220 2023-08-11 10:39:01.000000 bycon-1.6.3/docs/future.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.318849 bycon-1.6.3/docs/generated/
--rw-r--r--   0 mbaudis    (501) staff       (20)    11819 2024-03-07 18:11:52.000000 bycon-1.6.3/docs/generated/argument_definitions.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     8395 2024-03-07 18:11:52.000000 bycon-1.6.3/docs/generated/plot_defaults.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      862 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/handovers.md
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.319084 bycon-1.6.3/docs/img/
--rw-r--r--   0 mbaudis    (501) staff       (20)     8070 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/img/site-logo-main.png
--rw-r--r--   0 mbaudis    (501) staff       (20)     6264 2023-05-12 18:37:11.000000 bycon-1.6.3/docs/img/site-logo-topright.png
--rw-r--r--   0 mbaudis    (501) staff       (20)     2885 2023-11-19 15:02:46.000000 bycon-1.6.3/docs/index.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     7610 2023-11-19 15:02:46.000000 bycon-1.6.3/docs/installation.md
--rw-r--r--   0 mbaudis    (501) staff       (20)     5250 2024-01-18 17:19:59.000000 bycon-1.6.3/docs/tests.md
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     3337 2024-02-24 13:23:02.000000 bycon-1.6.3/install.py
--rw-r--r--   0 mbaudis    (501) staff       (20)      194 2023-06-29 20:11:54.000000 bycon-1.6.3/install.yaml
-drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-03-08 14:53:07.319667 bycon-1.6.3/local/
--rw-r--r--   0 mbaudis    (501) staff       (20)      950 2023-08-22 12:13:26.000000 bycon-1.6.3/local/README.md
--rw-r--r--   0 mbaudis    (501) staff       (20)      205 2023-12-20 15:51:43.000000 bycon-1.6.3/local/authorizations.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      805 2023-08-22 12:13:19.000000 bycon-1.6.3/local/dataset_definitions.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     5104 2024-03-08 14:48:24.000000 bycon-1.6.3/local/instance_overrides.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      277 2024-02-24 14:18:41.000000 bycon-1.6.3/local/local_paths.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)     1874 2024-02-22 13:41:39.000000 bycon-1.6.3/mkdocs.yaml
--rw-r--r--   0 mbaudis    (501) staff       (20)      161 2024-02-15 15:43:16.000000 bycon-1.6.3/requirements.txt
--rw-r--r--   0 mbaudis    (501) staff       (20)       74 2024-03-08 14:53:07.320554 bycon-1.6.3/setup.cfg
--rwxr-xr-x   0 mbaudis    (501) staff       (20)     2100 2024-03-08 14:48:59.000000 bycon-1.6.3/setup.py
--rwxr-xr-x   0 mbaudis    (501) staff       (20)      395 2024-03-07 09:44:11.000000 bycon-1.6.3/updev.sh
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.654362 bycon-1.6.5/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.514169 bycon-1.6.5/.github/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.575144 bycon-1.6.5/.github/workflows/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      486 2023-05-12 18:37:11.000000 bycon-1.6.5/.github/workflows/mk-bycon-docs.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      232 2023-08-22 12:24:33.000000 bycon-1.6.5/.gitignore
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7048 2023-05-12 18:37:11.000000 bycon-1.6.5/LICENSE
+-rw-r--r--   0 mbaudis    (501) staff       (20)      124 2023-05-12 18:26:34.000000 bycon-1.6.5/MANIFEST.in
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2844 2024-04-03 06:56:10.654224 bycon-1.6.5/PKG-INFO
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1306 2023-07-24 09:02:43.000000 bycon-1.6.5/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.575555 bycon-1.6.5/bycon/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1397 2024-03-27 14:09:45.000000 bycon-1.6.5/bycon/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.578006 bycon-1.6.5/bycon/beaconServer/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      118 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/beaconServer/README.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:26:34.000000 bycon-1.6.5/bycon/beaconServer/__init__.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2783 2024-03-08 13:27:13.000000 bycon-1.6.5/bycon/beaconServer/beacon.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1054 2024-03-06 09:18:52.000000 bycon-1.6.5/bycon/beaconServer/cohorts.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1036 2024-02-29 12:53:03.000000 bycon-1.6.5/bycon/beaconServer/configuration.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1032 2024-03-06 10:42:26.000000 bycon-1.6.5/bycon/beaconServer/datasets.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1091 2024-02-29 12:52:31.000000 bycon-1.6.5/bycon/beaconServer/entry_types.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1098 2024-03-06 10:42:04.000000 bycon-1.6.5/bycon/beaconServer/filtering_terms.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1659 2024-03-08 13:09:44.000000 bycon-1.6.5/bycon/beaconServer/info.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1030 2024-02-29 12:53:38.000000 bycon-1.6.5/bycon/beaconServer/map.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     1147 2024-03-08 13:09:59.000000 bycon-1.6.5/bycon/beaconServer/service_info.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.579676 bycon-1.6.5/bycon/beaconServer/tests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1215 2024-02-21 11:11:55.000000 bycon-1.6.5/bycon/beaconServer/tests/GET-examples.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      772 2024-02-07 09:34:45.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      958 2024-02-07 09:44:28.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      564 2024-02-07 09:34:45.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      450 2024-02-09 08:13:23.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-individuals-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      591 2024-02-07 09:43:52.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      850 2024-02-07 09:42:58.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      634 2024-02-07 09:43:23.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      897 2024-02-07 09:58:17.000000 bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      126 2024-02-07 09:50:47.000000 bycon-1.6.5/bycon/beaconServer/tests/terminal-examples.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2572 2024-03-08 14:22:15.000000 bycon-1.6.5/bycon/config.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.580497 bycon-1.6.5/bycon/definitions/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13007 2024-04-02 22:15:12.000000 bycon-1.6.5/bycon/definitions/argument_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-08-22 12:13:19.000000 bycon-1.6.5/bycon/definitions/dataset_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15632 2024-03-09 09:31:36.000000 bycon-1.6.5/bycon/definitions/datatable_mappings.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4401 2024-03-08 14:02:13.000000 bycon-1.6.5/bycon/definitions/entity_defaults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11612 2024-03-07 13:33:08.000000 bycon-1.6.5/bycon/definitions/filter_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2202 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/definitions/geoloc_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6329 2024-02-28 09:44:52.000000 bycon-1.6.5/bycon/definitions/handover_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2213 2024-02-14 14:30:00.000000 bycon-1.6.5/bycon/definitions/interval_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3975 2024-04-02 13:20:42.000000 bycon-1.6.5/bycon/definitions/variant_request_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6650 2024-04-02 14:32:02.000000 bycon-1.6.5/bycon/definitions/variant_type_definitions.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.583254 bycon-1.6.5/bycon/lib/
+-rw-r--r--   0 mbaudis    (501) staff       (20)        0 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/lib/__init__.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1664 2024-02-29 12:32:23.000000 bycon-1.6.5/bycon/lib/args_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2428 2024-03-06 08:59:44.000000 bycon-1.6.5/bycon/lib/beacon_auth.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    33080 2024-03-27 15:00:07.000000 bycon-1.6.5/bycon/lib/beacon_response_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    10401 2024-03-25 12:34:48.000000 bycon-1.6.5/bycon/lib/bycon_helpers.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6664 2024-03-08 13:27:49.000000 bycon-1.6.5/bycon/lib/cgi_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8714 2024-03-27 14:36:59.000000 bycon-1.6.5/bycon/lib/cytoband_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2362 2024-02-23 13:27:02.000000 bycon-1.6.5/bycon/lib/dataset_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8683 2024-04-02 14:45:38.000000 bycon-1.6.5/bycon/lib/genome_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3695 2024-03-26 09:16:36.000000 bycon-1.6.5/bycon/lib/handover_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1230 2024-02-21 13:34:58.000000 bycon-1.6.5/bycon/lib/parse_filters_request.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5773 2024-04-02 14:27:59.000000 bycon-1.6.5/bycon/lib/parse_variant_request.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13182 2024-04-02 15:10:42.000000 bycon-1.6.5/bycon/lib/query_execution.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    31519 2024-04-02 22:20:15.000000 bycon-1.6.5/bycon/lib/query_generation.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5779 2024-03-27 14:33:47.000000 bycon-1.6.5/bycon/lib/read_specs.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11940 2024-03-08 12:51:08.000000 bycon-1.6.5/bycon/lib/response_remapping.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3350 2024-03-08 13:30:26.000000 bycon-1.6.5/bycon/lib/schema_parsing.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4344 2024-03-08 13:31:28.000000 bycon-1.6.5/bycon/lib/service_utils.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)    12264 2024-03-07 08:10:00.000000 bycon-1.6.5/bycon/lib/variant_mapping.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.583614 bycon-1.6.5/bycon/rsrc/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:53.000000 bycon-1.6.5/bycon/rsrc/.DS_Store
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.583790 bycon-1.6.5/bycon/rsrc/genomes/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2024-02-09 08:01:48.000000 bycon-1.6.5/bycon/rsrc/genomes/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.583979 bycon-1.6.5/bycon/rsrc/genomes/grch38/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30914 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2007 2023-06-29 20:11:54.000000 bycon-1.6.5/bycon/rsrc/genomes/grch38/refseq_chromosomes.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.584251 bycon-1.6.5/bycon/rsrc/genomes/hg16/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30743 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.584485 bycon-1.6.5/bycon/rsrc/genomes/hg17/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.584674 bycon-1.6.5/bycon/rsrc/genomes/hg18/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30748 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.584848 bycon-1.6.5/bycon/rsrc/genomes/hg19/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    30754 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.585063 bycon-1.6.5/bycon/rsrc/genomes/mSarHar1.11/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      543 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.585279 bycon-1.6.5/bycon/rsrc/genomes/mm8/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13771 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.585443 bycon-1.6.5/bycon/rsrc/genomes/mm9/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13786 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.585607 bycon-1.6.5/bycon/rsrc/genomes/zf7/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      716 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.586124 bycon-1.6.5/bycon/schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2024-02-09 08:01:53.000000 bycon-1.6.5/bycon/schemas/.DS_Store
+-rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:26:34.000000 bycon-1.6.5/bycon/schemas/README.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)       14 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/__init__.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.586406 bycon-1.6.5/bycon/schemas/bin/
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     7331 2024-02-06 13:56:06.000000 bycon-1.6.5/bycon/schemas/bin/beaconYamler.py
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.524730 bycon-1.6.5/bycon/schemas/bin/config/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      602 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/bin/config/beaconYamler.yaml
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)      889 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/bin/yamlerRunner.sh
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.586574 bycon-1.6.5/bycon/schemas/framework/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.5/bycon/schemas/framework/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.587340 bycon-1.6.5/bycon/schemas/framework/json/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.588587 bycon-1.6.5/bycon/schemas/framework/json/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      572 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/basicElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11798 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/beaconCommonComponents.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      566 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/elementWithDescription.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.590066 bycon-1.6.5/bycon/schemas/framework/json/common/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      125 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/basicElement-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1936 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      197 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/elementWithDescription-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      346 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/ontologizedElement-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      127 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/ontologyTerm-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      336 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      239 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/examples/referenceToAnSchema-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      697 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/ontologizedElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      933 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/ontologyTerm.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1017 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/referenceToAnSchema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.590253 bycon-1.6.5/bycon/schemas/framework/json/common/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2011 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.591123 bycon-1.6.5/bycon/schemas/framework/json/configuration/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3213 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4791 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/beaconMapSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3992 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/entryTypeDefinition.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      764 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/entryTypesSchema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.592301 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2281 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      540 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      223 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconMap-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      588 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1318 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      561 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3152 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/configuration/filteringTermsSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8386 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.592944 bycon-1.6.5/bycon/schemas/framework/json/requests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2238 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/beaconRequestBody.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      874 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/beaconRequestMeta.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.593393 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      830 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      114 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MIN-example.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.594023 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      231 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-sections/beaconRequestMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      495 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-sections/filteringTerms-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      386 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/examples-sections/requestParameters-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5169 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      452 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/requestParameters.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.594260 bycon-1.6.5/bycon/schemas/framework/json/requests/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4243 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/requests/validation/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.596246 bycon-1.6.5/bycon/schemas/framework/json/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1231 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconBooleanResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1290 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      727 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1277 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconCountResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      681 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      645 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconErrorResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      664 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      716 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconInfoResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      707 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconMapResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1454 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.598852 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      745 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2451 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      782 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2832 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1533 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2452 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1164 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1183 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1279 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      538 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1522 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      767 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.602453 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       85 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconBooleanResponseSection-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      115 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconCountResponseSection-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      166 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconInformationalResponseMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      656 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      180 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      214 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsetEmpty-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1070 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      526 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       87 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5381 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.604870 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      522 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      730 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3545 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4676 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      896 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2688 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1801 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2444 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconResultsets.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      702 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.605239 bycon-1.6.5/bycon/schemas/framework/src/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.606107 bycon-1.6.5/bycon/schemas/framework/src/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      393 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/basicElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9289 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/framework/src/common/beaconCommonComponents.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      356 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/elementWithDescription.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.607301 bycon-1.6.5/bycon/schemas/framework/src/common/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       96 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/basicElement-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1305 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      159 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/elementWithDescription-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      272 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/ontologizedElement-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       98 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/ontologyTerm-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      201 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/examples/referenceToAnSchema-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      462 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/ontologizedElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/ontologyTerm.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      717 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/referenceToAnSchema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.607452 bycon-1.6.5/bycon/schemas/framework/src/common/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1459 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.608196 bycon-1.6.5/bycon/schemas/framework/src/configuration/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2395 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3917 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3395 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      532 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.609265 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1545 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      312 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconConfigurationFilteringTerms-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      152 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconMap-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      810 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      396 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_MIN_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1014 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      440 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/entryTypeDefinition-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2412 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4640 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.610276 bycon-1.6.5/bycon/schemas/framework/src/requests/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1678 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/beaconRequestBody.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      693 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.610655 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      449 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       80 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-fullDocuments/beaconRequestBody-MIN-example.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.611173 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      153 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-sections/beaconRequestMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      284 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-sections/filteringTerms-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      271 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/examples-sections/requestParameters-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3535 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      340 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/requestParameters.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.611343 bycon-1.6.5/bycon/schemas/framework/src/requests/validation/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2786 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.612994 bycon-1.6.5/bycon/schemas/framework/src/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      996 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1342 2024-02-06 13:37:14.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      565 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1042 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconCountResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      517 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      481 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconErrorResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconFilteringTermsResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      554 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      545 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconMapResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1157 2023-05-24 09:00:05.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.614900 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      418 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconBooleanResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1323 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      432 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1834 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      954 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1579 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      586 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      675 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1035 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      433 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.616485 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       67 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconBooleanResponseSection-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       90 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconCountResponseSection-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      130 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconInformationalResponseMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      380 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      137 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconReceivedRequestSummary-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      428 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResponseMeta-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      132 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResultsetEmpty-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      582 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      280 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       69 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4108 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.618192 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      424 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconBooleanResponseSection.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      579 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2403 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3084 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      679 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2269 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1472 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1589 2023-05-24 11:46:35.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      558 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.586719 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.508792 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.587118 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1369 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResponse.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      837 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResults.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.508924 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/src/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.525344 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/src/responses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1102 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResponse.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      497 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResults.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.618351 bycon-1.6.5/bycon/schemas/models/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-02-09 08:01:48.000000 bycon-1.6.5/bycon/schemas/models/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.618514 bycon-1.6.5/bycon/schemas/models/json/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8196 2023-07-29 14:31:39.000000 bycon-1.6.5/bycon/schemas/models/json/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.619349 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7277 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxAnalysis.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7943 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6146 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2544 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2541 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.619893 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.620475 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2525 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    10867 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.620801 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      399 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      180 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/examples/analyses-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7268 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7602 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/beaconMap.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.621358 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8054 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16217 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.622227 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      498 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      305 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/examples/biosample-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.623090 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    12858 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13483 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.623785 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2335 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1216 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      161 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      288 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.629541 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4718 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5549 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/VRSallele.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4919 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/VRScopyNumberChange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      408 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/age.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      515 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ageRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      939 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ancestry.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1122 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/celllineInfo.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5647 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1632 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/complexValue.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2465 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3142 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/disease.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/doseInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      984 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/evidence.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1642 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/exposure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1034 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/externalReference.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1269 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/file.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1343 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2039 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/measurement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      925 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/metaData.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      933 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5291 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/pedigree.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3428 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1824 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/procedure.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      923 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/provenance.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      721 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/quantity.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      961 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/referenceRange.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1150 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/resource.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      857 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/timeElement.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      835 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/timeInterval.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1745 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/treatment.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      511 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/update.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      345 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/value.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1525 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.630045 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2312 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    19091 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.630365 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      132 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      825 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9407 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.631219 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    25440 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    17332 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.631939 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3473 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      707 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      647 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      275 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/filteringTerms.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6629 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2718 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.632464 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4870 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15884 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.633234 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1534 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      160 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2224 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1101 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.633541 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/phenopackets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    15893 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.634029 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3807 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)    13255 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/endpoints.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.634492 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      532 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      178 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MIN-example.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)       91 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/filteringTerms.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.636413 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3342 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Collation.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      782 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/CytobandMapping.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1779 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2422 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1999 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)      370 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/OntologyClassGroup.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1314 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3224 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1822 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5034 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Publication.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2382 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2936 2024-03-06 12:40:56.000000 bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.636661 bycon-1.6.5/bycon/schemas/models/src/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-29 14:30:02.000000 bycon-1.6.5/bycon/schemas/models/src/.DS_Store
+-rw-r--r--   0 mbaudis    (501) staff       (20)      294 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/README.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.637171 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4489 2024-02-24 10:53:00.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxAnalysis.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4973 2023-06-30 11:06:24.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     4181 2024-01-18 17:19:59.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1692 2023-06-23 14:30:27.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1574 2023-05-31 15:03:17.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.637621 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2024-03-13 18:07:48.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/.DS_Store
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.637950 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1517 2023-06-23 14:32:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6325 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.638251 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      309 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      144 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/examples/analyses-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5073 2023-07-24 15:07:04.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5216 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/beaconMap.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.638636 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7846 2023-06-22 20:21:56.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9356 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.639011 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      330 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      213 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/examples/biosample-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.639567 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8616 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7822 2024-03-06 12:40:43.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.640057 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1233 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      653 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      123 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      193 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.646219 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3565 2023-08-15 08:02:14.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3771 2023-08-11 10:39:01.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/VRSallele.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3458 2023-08-11 10:39:01.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/VRScopyNumberChange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      299 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/age.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      373 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/ageRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      585 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      747 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3893 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1015 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1160 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1891 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/disease.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1177 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      702 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/evidence.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1094 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/exposure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      765 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      884 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/file.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1097 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1281 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/measurement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      553 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/metaData.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      689 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3116 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2460 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1175 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/procedure.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1018 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/provenance.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      500 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/quantity.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      563 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      701 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/resource.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      601 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      594 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1108 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/treatment.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      362 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/update.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      229 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/value.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1200 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.646606 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1577 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11022 2024-03-06 11:52:16.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.647014 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      103 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      534 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       72 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5661 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.647709 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-26 11:46:15.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/.DS_Store
+-rw-r--r--   0 mbaudis    (501) staff       (20)    16186 2023-08-11 10:39:01.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9682 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.648258 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1937 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      401 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      376 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      158 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/filteringTerms.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5747 2023-10-24 11:35:29.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2486 2023-11-19 15:02:46.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.648620 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3015 2023-06-23 14:31:14.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9227 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.649255 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      820 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      104 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1095 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      600 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.649564 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/phenopackets/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1301 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     9236 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.650119 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2476 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7624 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.650448 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/examples/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      379 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MAX-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      142 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/examples/runs-MIN-example.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)       73 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/filteringTerms.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.651176 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6148 2023-07-26 11:44:44.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/.DS_Store
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1859 2023-10-20 16:01:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Collation.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      664 2023-08-26 14:05:41.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/CytobandMapping.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1207 2024-01-18 17:19:59.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1590 2023-06-29 20:11:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1394 2023-06-29 20:11:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      257 2023-05-12 18:37:11.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/OntologyClassGroup.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      872 2023-06-29 20:11:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1713 2023-06-29 20:11:54.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1148 2023-08-15 07:53:42.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3292 2023-06-09 05:05:31.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1855 2023-06-09 05:05:31.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2131 2024-01-18 17:19:59.000000 bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.653768 bycon-1.6.5/bycon.egg-info/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2844 2024-04-03 06:56:10.000000 bycon-1.6.5/bycon.egg-info/PKG-INFO
+-rw-r--r--   0 mbaudis    (501) staff       (20)    60982 2024-04-03 06:56:10.000000 bycon-1.6.5/bycon.egg-info/SOURCES.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)        1 2024-04-03 06:56:10.000000 bycon-1.6.5/bycon.egg-info/dependency_links.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)       83 2024-04-03 06:56:10.000000 bycon-1.6.5/bycon.egg-info/requires.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)        6 2024-04-03 06:56:10.000000 bycon-1.6.5/bycon.egg-info/top_level.txt
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.652249 bycon-1.6.5/docs/
+-rw-r--r--   0 mbaudis    (501) staff       (20)       20 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/CNAME
+-rw-r--r--   0 mbaudis    (501) staff       (20)    38945 2024-04-03 06:53:53.000000 bycon-1.6.5/docs/changes.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      176 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/code-notes.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.652385 bycon-1.6.5/docs/css/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1076 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/css/extra.css
+-rw-r--r--   0 mbaudis    (501) staff       (20)     3220 2023-08-11 10:39:01.000000 bycon-1.6.5/docs/future.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.652662 bycon-1.6.5/docs/generated/
+-rw-r--r--   0 mbaudis    (501) staff       (20)    11819 2024-03-07 18:11:52.000000 bycon-1.6.5/docs/generated/argument_definitions.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8395 2024-03-07 18:11:52.000000 bycon-1.6.5/docs/generated/plot_defaults.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      862 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/handovers.md
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.652941 bycon-1.6.5/docs/img/
+-rw-r--r--   0 mbaudis    (501) staff       (20)     8070 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/img/site-logo-main.png
+-rw-r--r--   0 mbaudis    (501) staff       (20)     6264 2023-05-12 18:37:11.000000 bycon-1.6.5/docs/img/site-logo-topright.png
+-rw-r--r--   0 mbaudis    (501) staff       (20)     2885 2023-11-19 15:02:46.000000 bycon-1.6.5/docs/index.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     7610 2023-11-19 15:02:46.000000 bycon-1.6.5/docs/installation.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5250 2024-01-18 17:19:59.000000 bycon-1.6.5/docs/tests.md
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     3337 2024-02-24 13:23:02.000000 bycon-1.6.5/install.py
+-rw-r--r--   0 mbaudis    (501) staff       (20)      194 2023-06-29 20:11:54.000000 bycon-1.6.5/install.yaml
+drwxr-xr-x   0 mbaudis    (501) staff       (20)        0 2024-04-03 06:56:10.653595 bycon-1.6.5/local/
+-rw-r--r--   0 mbaudis    (501) staff       (20)      950 2023-08-22 12:13:26.000000 bycon-1.6.5/local/README.md
+-rw-r--r--   0 mbaudis    (501) staff       (20)      205 2023-12-20 15:51:43.000000 bycon-1.6.5/local/authorizations.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      805 2023-08-22 12:13:19.000000 bycon-1.6.5/local/dataset_definitions.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     5058 2024-03-09 07:26:38.000000 bycon-1.6.5/local/instance_overrides.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      277 2024-02-24 14:18:41.000000 bycon-1.6.5/local/local_paths.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)     1874 2024-02-22 13:41:39.000000 bycon-1.6.5/mkdocs.yaml
+-rw-r--r--   0 mbaudis    (501) staff       (20)      161 2024-02-15 15:43:16.000000 bycon-1.6.5/requirements.txt
+-rw-r--r--   0 mbaudis    (501) staff       (20)       74 2024-04-03 06:56:10.654713 bycon-1.6.5/setup.cfg
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)     2100 2024-04-03 06:52:51.000000 bycon-1.6.5/setup.py
+-rwxr-xr-x   0 mbaudis    (501) staff       (20)      441 2024-03-13 18:02:21.000000 bycon-1.6.5/updev.sh
```

### Comparing `bycon-1.6.3/LICENSE` & `bycon-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/PKG-INFO` & `bycon-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bycon
-Version: 1.6.3
+Version: 1.6.5
 Summary: A Python-based environment for the Beacon v2 genomics API
 Home-page: https://github.com/progenetix/bycon
 Author: Michael Baudis
 Author-email: contact@progenetix.org
 Project-URL: Bug Reports, https://github.com/progenetix/bycon/issues
 Project-URL: Source, https://github.com/progenetix/bycon/
 Project-URL: Helpers, https://github.com/progenetix/byconaut/
```

### Comparing `bycon-1.6.3/README.md` & `bycon-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/__init__.py` & `bycon-1.6.5/bycon/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from config import *
 
     from args_parsing import *
     from beacon_auth import *
     from beacon_response_generation import *
     from bycon_helpers import *
     from cgi_parsing import *
+    from cytoband_parsing import *
     from dataset_parsing import *
     from genome_utils import *
     from handover_generation import *
     from parse_filters_request import *
     from query_execution import *
     from query_generation import *
     from read_specs import *
```

### Comparing `bycon-1.6.3/bycon/beaconServer/beacon.py` & `bycon-1.6.5/bycon/beaconServer/beacon.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/cohorts.py` & `bycon-1.6.5/bycon/beaconServer/cohorts.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/configuration.py` & `bycon-1.6.5/bycon/beaconServer/configuration.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/datasets.py` & `bycon-1.6.5/bycon/beaconServer/datasets.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/entry_types.py` & `bycon-1.6.5/bycon/beaconServer/entry_types.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/filtering_terms.py` & `bycon-1.6.5/bycon/beaconServer/filtering_terms.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/info.py` & `bycon-1.6.5/bycon/beaconServer/info.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/map.py` & `bycon-1.6.5/bycon/beaconServer/map.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/service_info.py` & `bycon-1.6.5/bycon/beaconServer/service_info.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/GET-examples.md` & `bycon-1.6.5/bycon/beaconServer/tests/GET-examples.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters-no-descendants.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-biosamples-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-core-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-phenopackets-from-NCIT-filters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json` & `bycon-1.6.5/bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/config.py` & `bycon-1.6.5/bycon/config.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/argument_definitions.yaml` & `bycon-1.6.5/bycon/definitions/argument_definitions.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -74,23 +74,25 @@
     * include resultset responses, e.g. HIT, MISS
     * kind of a holdover from Beacon pre-v1
 
 # query / data selection
 
 dataset_ids:
   type: array
-  items: string
+  items:
+    type: string
   cmdFlags:
     - -d
     - --datasetIds
   description: dataset ids
 
 filters:
   type: array
-  items: string
+  items:
+    type: string
   cmdFlags:
     - --filters
   description: prefixed filter values, comma concatenated
 
 filter_precision:
   type: string
   cmdFlags:
@@ -198,17 +200,19 @@
   db_key: info.var_length
   pattern: '^\d+?$'
   cmdFlags:
     - --variantMaxLength
   description: 'variantMaxLength: The maximum variant length in bases for e.g. CNV queries.'
 
 gene_id:
-  type: string
+  type: array
+  items:
+    type: string
+    pattern: '^\w+?(\w+?(\-\w+?)?)?$'
   db_key: Null
-  pattern: '^\w+?(\w+?(\-\w+?)?)?$'
   cmdFlags:
     - --geneId
   description: gene id
 
 aminoacid_change:
   type: string
   db_key: molecular_attributes.aminoacid_changes 
@@ -231,14 +235,26 @@
     - --genomicAlleleShortForm
   description: 'Genomic HGVSId descriptor'
 
 # ------------------------------------------------------------------------------
 # variant parameters - non-standard
 # ------------------------------------------------------------------------------
 
+variant_query_digests:
+  type: array
+  db_key: Null
+  items:
+    type: string
+    pattern: '^(?:chro?)?([12]?[\dXY]):(\d+?(?:-\d+?)?)(?:--(\d+?(?:-\d+?)?))?(?::([\w\:\>]+?))?$'
+  cmdFlags:
+    - --variantQueryDigests
+  examples:
+    - "9:9000001-21975098--21967753-24000000:DEL"
+  description: 'Variant query digest-style short form'
+
 variant_internal_id:
   type: string
   db_key: variant_internal_id 
   pattern: '^\w[\w\:\-\,]+?\w$'
   examples:
     - '11:52900000-134452384:EFO_0030067'
   cmdFlags:
@@ -277,46 +293,56 @@
     - 'pgxind-kftx25eh'
   cmdFlags:
     - --id
   description: An id; this parameter only makes sense for specific REST entry types
 
 ids:
   type: array
-  items: string
+  items:
+    type: string
+    pattern: '^\w[\w:-]+\w$'
   cmdFlags:
     - --ids
   description: 'One or more ids; this parameter only makes sense for specific REST entry types'
 
 biosample_ids:
   type: array
-  items: string
+  items:
+    type: string
+    pattern: '^\w[\w:-]+\w$'
   byc_entity: biosample
   cmdFlags:
     - --biosampleIds
   description: biosample ids
 
 analysis_ids:
   type: array
-  items: string
+  items:
+    type: string
+    pattern: '^\w[\w:-]+\w$'
   byc_entity: analysis
   cmdFlags:
     - --analysisIds
   description: callset / analysis ids
 
 individual_ids:
   type: array
-  items: string
+  items:
+    type: string
+    pattern: '^\w[\w:-]+\w$'
   byc_entity: individual
   cmdFlags:
     - --individualIds
   description: subject ids
 
 variant_ids:
   type: array
-  items: string
+  items:
+    type: string
+    pattern: '^\w[\w:-]+\w$'
   byc_entity: genomicVariant
   cmdFlags:
     - --variantIds
   description: variant ids
 
 # ------------------------------------------------------------------------------
 # technical / procedural - non-standard
@@ -461,59 +487,66 @@
 #   cmdFlags:
 #     - -q
 #     - --query
 #   description: complete query string, e.g. `{"biosamples":{"external_references.id":"geo:GSE7428"}}`
 
 delivery_keys:
   type: array
-  items: string
+  items:
+    type: string
   cmdFlags:
     - --deliveryKeys
   description: delivery keys
 
 collation_types:
   type: array
-  items: string
+  items:
+    type: string
   cmdFlags:
     - --collationTypes
   description: selected collation types, e.g. "EFO"
 
 with_samples:
   type: integer
   cmdFlags:
     - --withSamples
   description: only for the collations; number of code_matches...
 
 selected_beacons:
   type: array
-  items: string
+  items:
+    type: string
 
 # ------------------------------------------------------------------------------
 # genomic parameters
 # ------------------------------------------------------------------------------
 
 genome_binning:
   type: string
   default: "1Mb"
   cmdFlags:
     - --genomeBinning
   description: "one of the predefined genome binning keys - default 1Mb"
 
 cyto_bands:
-  type: string
+  type: array
   db_key: Null
-  pattern: ^(?:chro?)?([12]?[\dXY])([pq](?:(?:ter)|(?:cen)|(?:[1-4](?:\d(?:\.\d\d*?)?)?)?))?\-?([pq](?:(?:cen)|(?:ter)|(?:[1-4](?:\d(?:\.\d\d*?)?)?)?))?$
+  items:
+    type: string
+    pattern: ^(?:chro?)?([12]?[\dXY])([pq](?:(?:ter)|(?:cen)|(?:[1-4](?:\d(?:\.\d\d*?)?)?)?))?\-?([pq](?:(?:cen)|(?:ter)|(?:[1-4](?:\d(?:\.\d\d*?)?)?)?))?$
   cmdFlags:
     - --cytoBands
   description: cytobands, e.g. 8q21q24.1
 
 chro_bases:
-  type: string
+  type: array
+  items:
+    type: string
+    pattern: ^(chro?)?([12]?[\dXY])\:(\d+?)(\-(\d+?))?$
   db_key: Null
-  pattern: ^(chro?)?([12]?[\dXY])\:(\d+?)(\-(\d+?))?$
   cmdFlags:
     - --chroBases
   description: only for the cytoband converter ... e.g. 8:0-120000000
 
 ################################################################################
 # geographic ...
 ################################################################################
```

### Comparing `bycon-1.6.3/bycon/definitions/datatable_mappings.yaml` & `bycon-1.6.5/bycon/definitions/datatable_mappings.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,25 @@
         beacon_key: False
         compact: True
       cbioportal_label:
         type: string
         db_key: references.cbioportal.label
         beacon_key: False
         compact: True
+      tcgaproject_id:
+        type: string
+        db_key: references.tcgaproject.id
+        indexed: True
+        beacon_key: False
+        compact: True
+      tcgaproject_label:
+        type: string
+        db_key: references.tcgaproject.label
+        beacon_key: False
+        compact: True
       external_references:
         type: array
         beacon_key: biosamples.externalReferences
         db_key: external_references
         indexed: True
         compact: True
         examples:
```

### Comparing `bycon-1.6.3/bycon/definitions/entity_defaults.yaml` & `bycon-1.6.5/bycon/definitions/entity_defaults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/filter_definitions.yaml` & `bycon-1.6.5/bycon/definitions/filter_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/geoloc_definitions.yaml` & `bycon-1.6.5/bycon/definitions/geoloc_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/handover_definitions.yaml` & `bycon-1.6.5/bycon/definitions/handover_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/interval_definitions.yaml` & `bycon-1.6.5/bycon/definitions/interval_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/definitions/variant_request_definitions.yaml` & `bycon-1.6.5/bycon/definitions/variant_request_definitions.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -14,38 +14,52 @@
   - start
   - end
   - variant_min_length
   - variant_max_length
   - gene_id
   - aminoacid_change
   - genomic_allele_short_form
+  - cyto_bands
+  - variant_query_digests
 
 # As long as there are no variant query schemas to define valid Beacon
 # variant parameter combinations the `request_types` here provide sets
 # of combinations valid at least for `bycon` Progenetix etc. data.
 request_types:
 
+  variantQueryDigestsRequest:
+    all_of:
+      - variant_query_digests
+
+  cytoBandRequest:
+    all_of:
+      - cyto_bands
+    optional:
+      - variant_type
+      - variant_min_length
+      - variant_max_length
+
   aminoacidChangeRequest:
     all_of:
       - aminoacid_change
     optional:
       - gene_id
 
   genomicAlleleShortFormRequest:
     all_of:
       - genomic_allele_short_form
 
-  variantTypeRequest:
-    description: >-
-      This dangerous query only uses a variant type, e.g. to limit an "all variants"
-      retrieval to SNVs or CNVs.
-      TODO: Add some private parameter to make this work on ly for special
-      circumstances... May be used w/ a combination of filter length >0 check.
-    all_of:
-      - variant_type
+  # variantTypeRequest:
+  #   description: >-
+  #     This dangerous query only uses a variant type, e.g. to limit an "all variants"
+  #     retrieval to SNVs or CNVs.
+  #     TODO: Add some private parameter to make this work only for special
+  #     circumstances... May be used w/ a combination of filter length > 0 check.
+  #   all_of:
+  #     - variant_type
 
   variantBracketRequest:
     description: >-
       This specific request allows for the bracketed search of genomic variants
       with start and end coordinates and a variant type. in contrast to a
       beaconRangeRequest, the start and end positions of the matched variants
       have to fall into the (1 base or longer) intervals for start and end,
@@ -56,16 +70,16 @@
       fuzzy matching of CNVs and similar variants of imprecise length and
       position.
     all_of:
       - assembly_id
       - start
       - end
       - reference_name
-      - variant_type
     optional:
+      - variant_type
       - variant_min_length
       - variant_max_length
 
   variantRangeRequest:
     description: >-
       The beaconRangeRequest queries variants falling between start and end.
       `start` and `end` parameters should be single values.
```

### Comparing `bycon-1.6.3/bycon/definitions/variant_type_definitions.yaml` & `bycon-1.6.5/bycon/definitions/variant_type_definitions.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -61,26 +61,48 @@
     - EFO:0020073
     - EFO:0030069
     - EFO:0030070
     - EFO:0030071
     - EFO:0030072
     - EFO:0030073      
 
+SO:0001743:
+  description: >-
+    This is an alternative to `EFO:0030067`. The SO definitions for CNVs are
+    slightly misleading (type of `sequence_length_alteration`) and do not
+    include the more specific child terms from EFO or VRS. 
+  variant_state:
+    id: SO:0001743
+    label: copy_number_loss
+  DUPDEL: DEL
+  variant_type_id: SO:0001743
+  variant_type: DEL
+  VRS_type: CopyNumberChange
+  VCF_symbolic_allele: <DEL>
+  cnv_dummy_value: -1
+  child_terms:
+    - EFO:0030067
+    - SO:0001743
+    - EFO:0030068
+    - EFO:0020073
+    - EFO:0030069
+
 EFO:0030067:
   variant_state:
     id: EFO:0030067
     label: copy number loss
   DUPDEL: DEL
   variant_type_id: EFO:0030067
   variant_type: DEL
   VRS_type: CopyNumberChange
   VCF_symbolic_allele: <DEL>
   cnv_dummy_value: -1
   child_terms:
     - EFO:0030067
+    - SO:0001743
     - EFO:0030068
     - EFO:0020073
     - EFO:0030069
 
 EFO:0030068:
   variant_state:
     id: EFO:0030068
@@ -129,14 +151,36 @@
   variant_type_id: EFO:0030070
   variant_type: DUP
   VRS_type: CopyNumberChange
   VCF_symbolic_allele: <DUP>
   cnv_dummy_value: 0.58
   child_terms:
     - EFO:0030070
+    - SO:0001742
+    - EFO:0030071
+    - EFO:0030072
+    - EFO:0030073
+
+SO:0001742:
+  description: >-
+    This is an alternative to `EFO:0030070`. The SO definitions for CNVs are
+    slightly misleading (type of `sequence_length_alteration`) and do not
+    include the more specific child terms from EFO or VRS. 
+  variant_state:
+    id: SO:0001742
+    label: copy_number_gain
+  DUPDEL: DUP
+  variant_type_id: SO:0001742
+  variant_type: DUP
+  VRS_type: CopyNumberChange
+  VCF_symbolic_allele: <DUP>
+  cnv_dummy_value: 0.58
+  child_terms:
+    - EFO:0030070
+    - SO:0001742
     - EFO:0030071
     - EFO:0030072
     - EFO:0030073
 
 EFO:0030071:
   variant_state:
     id: EFO:0030071
@@ -188,14 +232,15 @@
   VCF_symbolic_allele: Null
   cnv_dummy_value: Null
   child_terms:
     - SO:0001059
     - SO:0001483
     - SO:0002007
     - SO:0000667
+    - SO:0001743
 
 SO:0001483:
   variant_state:
     id: SO:0001483
     label: SNP
   DUPDEL: Null
   variant_type_id: SO:0001059
@@ -227,7 +272,20 @@
   variant_type_id: SO:0000667
   variant_type: INS
   VRS_type: Allele
   VCF_symbolic_allele: Null
   cnv_dummy_value: Null
   child_terms:
     - SO:0000667
+
+SO:0001413:
+  variant_state:
+    id: SO:0001413
+    label: translocation breakpoint
+  DUPDEL: Null
+  variant_type_id: SO:0001413
+  variant_type: BND
+  VRS_type: Null
+  VCF_symbolic_allele: <BND>
+  cnv_dummy_value: Null
+  child_terms:
+    - SO:0001413
```

### Comparing `bycon-1.6.3/bycon/lib/args_parsing.py` & `bycon-1.6.5/bycon/lib/args_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/beacon_auth.py` & `bycon-1.6.5/bycon/lib/beacon_auth.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/beacon_response_generation.py` & `bycon-1.6.5/bycon/lib/beacon_response_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,17 @@
             f_s = '|'.join(ft_fs)
             f_re = re.compile(r'^' + '|'.join(ft_fs))
         else:
             f_re = None
 
         # TODO: This should be derived from some entity definitions
         # TODO: whole query generation in separate function ...
-        scopes = ["biosamples", "individuals", "analyses", "genomicVariations"]
+        # now added globally to filters since Q aggregation and 
+        # https://github.com/ga4gh-beacon/beacon-v2/pull/118
+        scopes = BYC.get("data_pipeline_entities", [])
         query = {}
         q_list = []
 
         q_scope = BYC_PARS.get("scope", "___none___")
         if q_scope in scopes:
             q_list.append({"scope": q_scope})
 
@@ -466,14 +468,16 @@
                 if "ontologyTerm" in f_t["type"]:
                     f_t.update({"type": f.get("name", "ontologyTerm")})
                 ft_k = f.get("db_key")
                 ft_s = f.get("scope")
                 if ft_k and ft_s:
                     f_t.update({"target": f'{ft_s}.{ft_k}'})
 
+                f_t.update({"scopes": scopes})
+
                 lab = f_t.get("label")
                 if lab is None:
                     f_t.pop("label", None)
 
                 # TODO: this is not required & also not as defined (singular `scope`)
                 # f_t.update({"scopes": scopes})
                 t_f_t_s.append(f_t)
@@ -749,15 +753,17 @@
             mongo_client = MongoClient(host=DB_MONGOHOST)
             data_db = mongo_client[ ds_id ]
             v_coll = mongo_client[ ds_id ][ "variants" ]
 
             r_s_res = []
 
             if "variants._id" in ds_results:
-                for v_id in ds_results["variants._id"]["target_values"]:
+                q_v_s = ds_results["variants._id"]["target_values"]
+                q_v_s = return_paginated_list(q_v_s, self.skip, self.limit)
+                for v_id in q_v_s:
                     v = v_coll.find_one({"_id":v_id})
                     r_s_res.append(v)
                 self.datasets_data.update({ds_id: r_s_res})
 
         ds_v_duration = datetime.datetime.now() - ds_v_start
 
         dbm = f'... variants retrieval needed {ds_v_duration.total_seconds()} seconds'
```

### Comparing `bycon-1.6.3/bycon/lib/bycon_helpers.py` & `bycon-1.6.5/bycon/lib/bycon_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,16 @@
             return float(value)
         elif "bool" in p_d_t:
             return test_truthy(value)
         else:
             return str(value)
     else:
         BYC["WARNINGS"].append(f"!!! Multiple values for {parameter} in request")
-        return '::'.join(values)
+        # re-joining ...
+        return ','.join(values)
 
 
 ################################################################################
 
 def select_this_server(byc: dict) -> str:
     """
     Cloudflare based encryption may lead to "http" based server addresses in the
```

### Comparing `bycon-1.6.3/bycon/lib/cgi_parsing.py` & `bycon-1.6.5/bycon/lib/cgi_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/dataset_parsing.py` & `bycon-1.6.5/bycon/lib/dataset_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/genome_utils.py` & `bycon-1.6.5/bycon/lib/genome_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -131,14 +131,70 @@
                 refseq_stripped: c_d["chr"],
                 c_d["genbank_id"]: c_d["chr"]
             })
 
 
 ################################################################################
 
+class VariantTypes:
+    def __init__(self, variant_type_definitions):
+        self.vtds = variant_type_definitions
+        self.variant_state = None
+        self.child_terms = set()
+
+
+    # -------------------------------------------------------------------------#
+    # ----------------------------- public ------------------------------------#
+    # -------------------------------------------------------------------------#
+
+    def variantState(self, variant_type="___none___"):
+        self.__variant_state_from_variant_type(variant_type)
+        return self.variant_state
+
+
+    # -------------------------------------------------------------------------#
+
+    def variantStateId(self, variant_type="___none___"):
+        self.__variant_state_from_variant_type(variant_type)
+        return self.variant_state.get("id", "___none___")
+
+
+    # -------------------------------------------------------------------------#
+
+    def variantStateChildren(self, variant_type="___none___"):
+        self.child_terms = set()
+        self.__variant_state_from_variant_type(variant_type)
+        return list(self.child_terms)
+
+
+    # -------------------------------------------------------------------------#
+    # ----------------------------- private -----------------------------------#
+    # -------------------------------------------------------------------------#
+
+    def __variant_state_from_variant_type(self, variant_type):
+        v_t_defs = self.vtds
+        for k, d in v_t_defs.items():
+            for p, v in d.items():
+                if v is None:
+                    continue
+                if type(v) is list:
+                    continue
+                if "variant_state" in p:
+                    v = v.get("id", "___none___")
+                if type(v) is not str:
+                    continue
+                if variant_type.lower() == v.lower():
+                    self.variant_state = d.get("variant_state", "___none___")
+                    self.child_terms.update(d.get("child_terms", []))
+
+
+
+
+################################################################################
+
 class GeneInfo:
     def __init__(self):
         self.gene_data = []
 
 
     # -------------------------------------------------------------------------#
     # ----------------------------- public ------------------------------------#
```

### Comparing `bycon-1.6.3/bycon/lib/handover_generation.py` & `bycon-1.6.5/bycon/lib/handover_generation.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,19 @@
             p_t = p_f + limit
             p_s = 0
             while p_f < target_count + 1:
                 if target_count < p_t:
                     p_t = target_count
                 l = f"{p_f + 1}-{p_t}"
                 u = __handover_create_url(h_o_server, h_o_defs, ds_id, accessid, p_s, limit)
-                h_o_r["pages"].append( { "handover_type": {"id": h_o_defs["handoverType"][ "id" ], "label": l }, "url": u } )
+                h_o_r["pages"].append( {
+                    "handover_type": {"id": h_o_defs["handoverType"][ "id" ],"label": l }, 
+                    "info": { "content_id": h_o_t},
+                    "url": u
+                } )
                 p_s += 1
                 p_f += limit
                 p_t = p_f + limit
             h_o_r["url"] += f'&skip={skip}&limit={limit}'
         if "url" in h_o_r:
             b_h_o.append( h_o_r )
```

### Comparing `bycon-1.6.3/bycon/lib/parse_filters_request.py` & `bycon-1.6.5/bycon/lib/parse_filters_request.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/parse_variant_request.py` & `bycon-1.6.5/bycon/lib/parse_variant_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     for v_p, v_v in BYC_PARS.items():
         if v_p in v_p_s:
             variant_pars.update({ v_p: v_v })
 
     # value checks
     v_p_c = { }
     variant_pars = __translate_reference_name(variant_pars, byc)
-    prdbug(variant_pars)
 
     for p_k, v_p in variant_pars.items():
         v_p = variant_pars[ p_k ]
         if "variant_type" in p_k:
             v_s = __variant_state_from_variant_par(v_p, byc)
             if v_s is False:
                 v_p_c[ p_k ] = None
@@ -87,14 +86,18 @@
             brts_k = [ "variantBracketRequest" ]
     elif "aminoacid_change" in v_pars:
         brts_k = [ "aminoacidChangeRequest" ]
     elif "genomic_allele_short_form" in v_pars:
         brts_k = [ "genomicAlleleShortFormRequest" ]
     elif "gene_id" in v_pars:
         brts_k = [ "geneVariantRequest" ]
+    elif "cyto_bands" in  v_pars:
+        brts_k = [ "cytoBandRequest" ]
+    elif "variant_query_digests" in  v_pars:
+        brts_k = [ "variantQueryDigestsRequest" ]
         
     vrt_matches = [ ]
     for vrt in brts_k:
         matched_par_no = 0
         needed_par_no = 0
         if "one_of" in brts[vrt]:
             needed_par_no = 1
```

### Comparing `bycon-1.6.3/bycon/lib/query_execution.py` & `bycon-1.6.5/bycon/lib/query_execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 def execute_bycon_queries(ds_id, BQ, byc):
     """podmd
     
     Pre-configured queries are performed in an aggregation pipeline against
     the standard "Progenetix"-type MongoDB collections.
         
     podmd"""
+
+    # TODO: a new type, where we use query aggregation for multiple
+    # variants observed in the same biosample to get aggregated; _i.e._ 
+    # different from a AND query for variants which would require the variant
+    # to fulfill both conditions
+
     h_o_methods = byc["handover_definitions"]["h->o_methods"]
     r_e_id = str(byc.get("response_entity_id", "___none___"))
 
     exe_queries = {}
     if "dataset_results" not in byc.keys():
         byc.update({"dataset_results": {}})
 
@@ -48,16 +54,16 @@
         "pref_m": "",
         "h_o_def": {},
         "query": {}
     }
 
     ############################################################################
 
-    dbm = f'queries at execution: {exe_queries}'
-    prdbug(dbm)
+    prdbug(f'queries at execution:')
+    prdbug(exe_queries)
 
     if not exe_queries.keys():
         return prefetch
 
     ############################################################################
 
     """podmd
@@ -135,34 +141,70 @@
         of callset `id` values from the different queries are intersected. Otherwise, the analyses
         from the variants query are the final ones.
         3. Since so far not all matching variants have been retrieved (only the biosamples which
         contain them), they are now fetched using the original query or a combination of the
         original query and the matching biosamples from the intersect.
         podmd"""
 
+        if type(variants_query) is not list:
+            variants_query = [variants_query]
+
+        v_q_l = variants_query.copy()
+
         pref_k = "variants.biosample_id->biosamples.id"
         prevars.update({
             "pref_m": pref_k,
-            "query": variants_query,
+            "query": v_q_l.pop(0),
             "h_o_def": h_o_methods.get(pref_k)
         })
         prefetch.update({pref_k: _prefetch_data(prevars)})
 
         if "biosamples.id" in prefetch.keys():
             bsids = list(set(prefetch["biosamples.id"]["target_values"]) & set(
                 prefetch[pref_k]["target_values"]))
             prefetch["biosamples.id"].update({"target_values": bsids, "target_count": len(bsids)})
-            variants_query = {"$and": [variants_query, {"biosample_id": {"$in": bsids}}]}
+            # variants_query = [{"$and": [variants_query[0], {"biosample_id": {"$in": bsids}}]}]
         else:
             prefetch["biosamples.id"] = prefetch[pref_k]
 
+        # if there are more than 1 variant query, intersect the biosample_ids from
+        # the previous queries (_i.e._ all variants have to occurr in the same biosample)
+        if len(v_q_l) > 0:
+            for v_q in v_q_l:
+                v_bsids = prefetch["biosamples.id"]["target_values"]
+                prdbug(f'before {prefetch["biosamples.id"]["target_count"]}')
+                if (len(v_bsids) == 0):
+                    break
+                v_q = {"$and": [v_q, {"biosample_id": {"$in": v_bsids}}]}
+                prevars.update({
+                    "pref_m": pref_k,
+                    "query": v_q,
+                    "h_o_def": h_o_methods.get(pref_k)
+                })
+                prefetch.update({pref_k: _prefetch_data(prevars)})
+                prefetch["biosamples.id"] = prefetch[pref_k]
+                prdbug(f'after {prefetch["biosamples.id"]["target_count"]}')
+
+        # collect variants from the multi match
+        # here we can use the $or query since the requirement (all variant results
+        # have to intersect for the same biosamples) has been met
         pref_k = "variants._id"
+        if len(variants_query) > 1:
+            v_v_q = {"$or": variants_query}
+        else:
+            v_v_q = variants_query[0]
+        if len(prefetch["biosamples.id"]["target_values"]) > 0:
+            v_v_q = {"$and": [v_v_q, {"biosample_id": {"$in": prefetch["biosamples.id"]["target_values"]}}]}
+        else:
+            # fallback for 0 match results
+            v_v_q = {"$and": [v_v_q, {"biosample_id": {"$in": ["___undefined___"]}}]}
+
         prevars.update({
             "pref_m": pref_k,
-            "query": variants_query,
+            "query": v_v_q,
             "h_o_def": h_o_methods.get(pref_k)
         })
         prefetch.update({pref_k: _prefetch_data(prevars)})
 
         # prevars["pref_m"] = "variants.variant_internal_id"
         # prevars["query"] = {"_id": {"$in": prefetch["variants._id"]["target_values"]}}
         # prefetch.update({prevars["pref_m"]: _prefetch_data(prevars)})
@@ -284,14 +326,16 @@
     previous queries for procedural use or second-pass data retrieval.
 
     podmd"""
 
     pref_m = prevars["pref_m"]
     data_db = prevars["data_db"]
     h_o_def = prevars["h_o_def"]
+    # prdbug(pref_m)
+    # prdbug(prevars["query"])
     dist = data_db[h_o_def["source_collection"]].distinct(h_o_def["source_key"], prevars["query"])
     h_o = {**h_o_def}
     t_v_s = dist if dist else []
     h_o.update(
         {
             "id": str(uuid4()),
             "source_db": prevars["ds_id"],
```

### Comparing `bycon-1.6.3/bycon/lib/query_generation.py` & `bycon-1.6.5/bycon/lib/query_generation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import inspect, pymongo, re, sys
 from bson import SON
 from os import environ
 from pymongo import MongoClient
 
 from bycon_helpers import days_from_iso8601duration, prdbug, return_paginated_list
 from config import *
-from genome_utils import GeneInfo
+from cytoband_parsing import bands_from_cytobands
+from genome_utils import ChroNames, GeneInfo, VariantTypes
 
 ################################################################################
 
 class ByconQuery():
     """
     Bycon queries are collected as an object with per data collection query objects,
     ready to be run against the respective entity databases.
@@ -45,22 +46,25 @@
         f_t_d = self.response_types.get("filteringTerm", {})
         self.filtering_terms_coll = f_t_d.get("collection", "___none___")
         if dataset_id is False:
             self.ds_id = byc.get("dataset_ids", False)[0]
         else:
             self.ds_id = dataset_id
         self.argument_definitions = byc.get("argument_definitions", {})
+        self.cytoband_definitions = byc.get("cytobands", [])
+        self.ChroNames = ChroNames()
         self.filters = byc.get("filters", [])
 
         self.requested_entity = byc.get("request_entity_id", False)
         self.response_entity = byc.get("response_entity_id", "___none___")
         self.path_id_value = byc.get("request_entity_path_id_value", False)
 
         self.variant_request_type = byc.get("variant_request_type", "___none___")
         self.variant_request_definitions = byc.get("variant_request_definitions", {})
+        self.VariantTypes = VariantTypes(byc.get("variant_type_definitions", {}))
         self.varguments = byc.get("varguments", {})
 
         self.filter_definitions = byc.get("filter_definitions", {})
         self.geoloc_definitions = byc.get("geoloc_definitions", {})
 
         self.limit = BYC_PARS.get("limit")
         self.skip = BYC_PARS.get("skip")
@@ -202,61 +206,160 @@
         if self.variant_request_type not in self.variant_request_definitions.get("request_types", {}).keys():
             return
 
         r_e = "genomicVariant"
         r_t_s = self.response_types
         r_c = r_t_s[r_e].get("collection")
 
-        prdbug(f'... Gene Id: {self.varguments.get("gene_id")} => {self.variant_request_type}')
-
         q = False
 
-        # The `geneVariantRequest` will generate a `variantRangeRequest`
-        if "geneVariantRequest" in  self.variant_request_type:
-            self.__create_geneVariantRequest_query()
-
-        if "variantTypeRequest" in self.variant_request_type and len(self.filters) > 0:
-            q = self.__create_variantTypeRequest_query()
+        # if "variantTypeRequest" in self.variant_request_type and len(self.filters) > 0:
+        #     q = self.__create_variantTypeRequest_query()
 
-        if "aminoacidChangeRequest" in self.variant_request_type:
-           q = self.__create_aminoacidChangeRequest_query()
+        if "geneVariantRequest" in  self.variant_request_type:
+            q = self.__create_geneVariantRequest_query()
+        elif "cytoBandRequest" in  self.variant_request_type:
+            q = self.__create_cytoBandRequest_query()
+        elif "variantQueryDigestsRequest" in  self.variant_request_type:
+            q = self.__create_variantQueryDigestsRequest_query()
+        elif "aminoacidChangeRequest" in self.variant_request_type:
+            q = self.__create_aminoacidChangeRequest_query()
         elif "genomicAlleleShortFormRequest" in self.variant_request_type:
-           q = self.__create_genomicAlleleShortFormRequest_query()
+            q = self.__create_genomicAlleleShortFormRequest_query()
         elif "variantBracketRequest" in self.variant_request_type:
             q = self.__create_variantBracketRequest_query()
         elif "variantRangeRequest" in self.variant_request_type:
             q = self.__create_variantRangeRequest_query()
         elif "variantAlleleRequest" in self.variant_request_type:
             q = self.__create_variantAlleleRequest_query()
 
 
         if q is False:
             return
 
         self.queries["entities"].update({r_e: {"query": q, "collection": r_c}})
+        prdbug(self.queries)
 
 
     #--------------------------------------------------------------------------#
 
     def __create_geneVariantRequest_query(self):
         # query database for gene and use coordinates to create range query
         vp = self.varguments
-        gene_data = GeneInfo().returnGene(vp["gene_id"])
-        # TODO: error report/warning
-        if not gene_data:
-            return
-        gene = gene_data[0]
+        q = []
+        for g in vp["gene_id"]:
+            gene_data = GeneInfo().returnGene(g)
+            # TODO: error report/warning
+            if not gene_data:
+                continue
+            gene = gene_data[0]
+            # Since this is a pre-processor to the range request
+            self.varguments.update( {
+                "reference_name": f'refseq:{gene.get("accession_version", "___none___")}',
+                "start": [ gene.get("start", 0) ],
+                "end": [ gene.get("end", 1) ]
+            } )
+            self.variant_request_type = "variantRangeRequest"
+            q_t = self.__create_variantRangeRequest_query()
+            q.append(q_t)
+
+        return q
+
+    #--------------------------------------------------------------------------#
+
+    def __create_variantQueryDigestsRequest_query(self):
+        # query database for gene and use coordinates to create range query
+        # http://progenetix.test/beacon/biosamples/?datasetIds=progenetix&filters=NCIT:C3058&variantQueryDigests=9:21000001-21975098--21967753-24000000:DEL,8:120000000-125000000--121000000-126000000:DUP&debugMode=
+        # http://progenetix.test/services/sampleplots/?datasetIds=progenetix&filters=NCIT:C3058&variantQueryDigests=8:1-23000000--26000000-120000000:DUP,9:21000001-21975098--21967753-24000000:DEL&debugMode=
+        vp = self.varguments
+        a_d = self.argument_definitions
+        vqd_pat = re.compile(a_d["variant_query_digests"]["items"]["pattern"])
 
-        # Since this is a pre-processor to the range request
+        vd_s = vp.get("variant_query_digests", [])
+        q = []
+        for qd in vd_s:
+            if not vqd_pat.match(qd):
+                prdbug(f'!!! no match {qd}')
+                continue
+            chro, start, end, change = vqd_pat.match(qd).group(1, 2, 3, 4)
+            self.varguments.update( {
+                "reference_name": self.ChroNames.refseq(chro),
+                "start": list(map(int, re.split('-', start))),
+                "end": list(map(int, re.split('-', end)))
+            } )
+            # TODO: This overrides potentially a global variant_type; so right now
+            # one has to leave the type out and use a global (or none), or provide
+            # a type w/ each digest
+            if change:
+                self.varguments.update( {
+                    "variant_type": { "$in": self.VariantTypes.variantStateChildren(change) }
+                } )
+
+            if len(self.varguments.get("start", [])) == 2:
+                if len(self.varguments.get("end", [])) == 2:
+                    self.variant_request_type = "variantBracketRequest"
+                    q_t = self.__create_variantBracketRequest_query()
+                    q.append(q_t)
+            elif len(self.varguments.get("start", [])) == 1:
+                if len(self.varguments.get("end", [])) == 1:
+                    self.variant_request_type = "variantRangeRequest"
+                    q_t = self.__create_variantRangeRequest_query()
+                    q.append(q_t)
+
+        return q
+
+
+    #--------------------------------------------------------------------------#
+
+    def __create_cytoBandRequest_query(self):
+        # query database for cytoband(s) and use coordinates to create range query
+        vp = self.varguments
+        a_d = self.argument_definitions
+        c_b_d = self.cytoband_definitions
+
+        cb_s = vp.get("cyto_bands", [])
+        cbs1, chro1, start1, end1, error1 = bands_from_cytobands(cb_s[0], c_b_d, a_d)
+        s_id1 = self.ChroNames.refseq(chro1)
         self.varguments.update( {
-            "reference_name": f'refseq:{gene.get("accession_version", "___none___")}',
-            "start": [ gene.get("start", 0) ],
-            "end": [ gene.get("end", 1) ]
+            "reference_name": s_id1,
+            "start": [ start1 ],
+            "end": [ end1 ]
         } )
-        self.variant_request_type = "variantRangeRequest"
+        if len(cb_s) == 1:           
+            self.variant_request_type = "variantRangeRequest"
+            q = self.__create_variantRangeRequest_query()
+            return q
+
+        elif len(cb_s) > 1:
+            cbs2, chro2, start2, end2, error2 = bands_from_cytobands(cb_s[1], c_b_d, a_d)
+            s_id2 = self.ChroNames.refseq(chro2)
+
+            # TODO: here is a prototype for a variant query list, used for co-occurring
+            # variants in the same biosample
+            if s_id1 != s_id2:
+                v_q_l = []
+                q1 = self.__create_variantRangeRequest_query()
+                v_q_l.append(q1)
+                self.varguments.update( {
+                    "reference_name": s_id2,
+                    "start": [ start2 ],
+                    "end": [ end2 ]
+                } )
+                q2 = self.__create_variantRangeRequest_query()
+                v_q_l.append(q2)
+                self.variant_request_type = "variantsMultimatchRequest"
+                return v_q_l
+
+            self.varguments.update( {
+                "start": [ start1, start2 ],
+                "end": [ end1, end2 ]
+            } )
+            self.variant_request_type = "variantBracketRequest"
+            q = self.__create_variantBracketRequest_query()
+            return q
 
 
     #--------------------------------------------------------------------------#
 
     def __create_aminoacidChangeRequest_query(self):    
         vp = self.varguments
         if not "aminoacid_change" in vp:
@@ -328,18 +431,18 @@
 
     def __create_variantBracketRequest_query(self):
         vp = self.varguments
         v_p_defs = self.argument_definitions
 
         v_q = { "$and": [
             { v_p_defs["reference_name"]["db_key"]: vp["reference_name"] },
-            { v_p_defs["start"]["db_key"]: { "$lt": vp["start"][-1] } },
-            { v_p_defs["end"]["db_key"]: { "$gte": vp["end"][0] } },
-            { v_p_defs["start"]["db_key"]: { "$gte": vp["start"][0] } },
-            { v_p_defs["end"]["db_key"]: { "$lt": vp["end"][-1] } },
+            { v_p_defs["start"]["db_key"]: { "$lt": sorted(vp["start"])[-1] } },
+            { v_p_defs["end"]["db_key"]: { "$gte": sorted(vp["end"])[0] } },
+            { v_p_defs["start"]["db_key"]: { "$gte": sorted(vp["start"])[0] } },
+            { v_p_defs["end"]["db_key"]: { "$lt": sorted(vp["end"])[-1] } },
             self.__create_in_query_for_parameter("variant_type", v_p_defs["variant_type"]["db_key"], vp)
         ]}
 
         return v_q
 
 
     #--------------------------------------------------------------------------#
```

### Comparing `bycon-1.6.3/bycon/lib/read_specs.py` & `bycon-1.6.5/bycon/lib/read_specs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from deepmerge import always_merger
 from json_ref_dict import RefDict, materialize
 from os import path, pardir, scandir, environ
 from pathlib import Path
 from pymongo import MongoClient
 
 from cgi_parsing import prdbug
+from cytoband_parsing import parse_cytoband_file
 from config import *
 
 ################################################################################
 
 def read_service_definition_files(byc):
     """podmd
     Reading the config from the same wrapper dir:
@@ -31,14 +32,16 @@
         with open( ofp ) as od:
             o = yaml.load( od , Loader=yaml.FullLoader)
         if d in BYC.keys():
             BYC.update({d: o})
         else:
             byc.update({d: o})
 
+    parse_cytoband_file(byc)
+
 ################################################################################
 
 def set_entity_mappings():
     b_e_d = BYC.get("entity_defaults", {})
     p_e_m = BYC.get("path_entry_type_mappings", {})
     e_p_m = BYC.get("entry_type_path_mappings", {})
     d_p_e = BYC.get("data_pipeline_entities", [])
```

### Comparing `bycon-1.6.3/bycon/lib/response_remapping.py` & `bycon-1.6.5/bycon/lib/response_remapping.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/schema_parsing.py` & `bycon-1.6.5/bycon/lib/schema_parsing.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/service_utils.py` & `bycon-1.6.5/bycon/lib/service_utils.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/lib/variant_mapping.py` & `bycon-1.6.5/bycon/lib/variant_mapping.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/.DS_Store` & `bycon-1.6.5/bycon/rsrc/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/.DS_Store` & `bycon-1.6.5/bycon/rsrc/genomes/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/grch38/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/grch38/refseq_chromosomes.yaml` & `bycon-1.6.5/bycon/rsrc/genomes/grch38/refseq_chromosomes.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/hg16/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/hg17/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/hg18/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/hg19/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/mSarHar1.11/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/mm8/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/mm9/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt` & `bycon-1.6.5/bycon/rsrc/genomes/zf7/cytoBandIdeo.txt`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/.DS_Store` & `bycon-1.6.5/bycon/schemas/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/bin/beaconYamler.py` & `bycon-1.6.5/bycon/schemas/bin/beaconYamler.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/bin/config/beaconYamler.yaml` & `bycon-1.6.5/bycon/schemas/bin/config/beaconYamler.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/bin/yamlerRunner.sh` & `bycon-1.6.5/bycon/schemas/bin/yamlerRunner.sh`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/.DS_Store` & `bycon-1.6.5/bycon/schemas/framework/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/basicElement.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/basicElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/beaconCommonComponents.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/beaconCommonComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/elementWithDescription.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/elementWithDescription.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/examples/beaconCommonComponents-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/ontologizedElement.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/ontologizedElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/ontologyTerm.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/ontologyTerm.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/referenceToAnSchema.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/referenceToAnSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json` & `bycon-1.6.5/bycon/schemas/framework/json/common/validation/beaconCommonComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/beaconConfigurationSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/beaconMapSchema.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/beaconMapSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/entryTypeDefinition.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/entryTypeDefinition.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/entryTypesSchema.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/entryTypesSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconConfiguration-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconConfigurationFilteringTerms-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/beaconMap-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_MIN_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entriesCollectionDefinition_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/examples/entryTypeDefinition-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/configuration/filteringTermsSchema.json` & `bycon-1.6.5/bycon/schemas/framework/json/configuration/filteringTermsSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/endpoints.json` & `bycon-1.6.5/bycon/schemas/framework/json/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/requests/beaconRequestBody.json` & `bycon-1.6.5/bycon/schemas/framework/json/requests/beaconRequestBody.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/requests/beaconRequestMeta.json` & `bycon-1.6.5/bycon/schemas/framework/json/requests/beaconRequestMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/requests/examples-fullDocuments/beaconRequestBody-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/requests/filteringTerms.json` & `bycon-1.6.5/bycon/schemas/framework/json/requests/filteringTerms.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/requests/validation/filteringTerms.json` & `bycon-1.6.5/bycon/schemas/framework/json/requests/validation/filteringTerms.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconBooleanResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconBooleanResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconCollectionsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconConfigurationResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconCountResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconCountResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconEntryTypesResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconErrorResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconErrorResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconFilteringTermsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconInfoResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconInfoResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconMapResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconMapResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/beaconResultsetsResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconBooleanResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCollectionsResponse-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconConfigurationResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconCountResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconEntryTypesResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconErrorResponse_example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconInfo-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconMapResponse-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-fullDocuments/beaconResultsetResponse-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconReceivedRequestSummary-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResponseMeta-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/examples-sections/beaconResultsets-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/ga4gh-service-info-1-0-0-schema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconBooleanResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconCountResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconFilteringTermsResults.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconInfoResults.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconInformationalResponseMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconReceivedRequestSummary.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconResponseMeta.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconResultsets.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconResultsets.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json` & `bycon-1.6.5/bycon/schemas/framework/json/responses/sections/beaconSummaryResponseSection.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/common/beaconCommonComponents.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/common/beaconCommonComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/common/examples/beaconCommonComponents-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/common/ontologyTerm.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/common/ontologyTerm.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/common/referenceToAnSchema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/common/referenceToAnSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/common/validation/beaconCommonComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/beaconConfigurationSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/beaconMapSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/entryTypeDefinition.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/entryTypesSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconConfiguration-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/beaconMap-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/examples/entriesCollectionDefinition_example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/configuration/filteringTermsSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/requests/beaconRequestBody.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/requests/beaconRequestBody.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/requests/beaconRequestMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/requests/filteringTerms.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/requests/filteringTerms.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/requests/validation/filteringTerms.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconBooleanResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconCollectionsResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconConfigurationResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconCountResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconCountResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconEntryTypesResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconInfoResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconMapResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconMapResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/beaconResultsetsResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCollectionsResponse-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconConfigurationResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconCountResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconEntryTypesResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconErrorResponse_example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconFilteringTermsResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconInfo-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-fullDocuments/beaconMapResponse-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/examples-sections/beaconResultsets-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/ga4gh-service-info-1-0-0-schema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconCountResponseSection.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconFilteringTermsResults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconInfoResults.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconInformationalResponseMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconReceivedRequestSummary.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconResponseMeta.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconResultsets.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml` & `bycon-1.6.5/bycon/schemas/framework/src/responses/sections/beaconSummaryResponseSection.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/.DS_Store` & `bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResponse.json` & `bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResponse.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResults.json` & `bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/json/responses/byconautServiceResults.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResponse.yaml` & `bycon-1.6.5/bycon/schemas/framework-byconaut-service-additions/src/responses/byconautServiceResponse.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/json/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxAnalysis.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxAnalysis.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxBiosample.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxCollation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxIndividual.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-database-schemas/pgxVariant.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/analyses/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/beaconConfiguration.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/beaconMap.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/beaconMap.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/biosamples/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/cohorts/examples/cohorts-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/GeoLocation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/VRSallele.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/VRSallele.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/VRScopyNumberChange.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/VRScopyNumberChange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ageRange.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ageRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ancestry.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ancestry.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/celllineInfo.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/celllineInfo.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/commonDefinitions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/complexValue.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/complexValue.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/dataUseConditions.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/disease.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/disease.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/doseInterval.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/doseInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/evidence.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/evidence.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/exposure.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/exposure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/externalReference.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/externalReference.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/file.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/file.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/gestationalAge.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/measurement.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/measurement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/metaData.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/metaData.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/ontologyTerm.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/pedigree.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/pedigree.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/phenotypicFeature.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/procedure.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/procedure.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/provenance.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/provenance.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/quantity.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/quantity.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/referenceRange.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/referenceRange.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/resource.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/resource.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/timeElement.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/timeElement.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/timeInterval.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/timeInterval.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/treatment.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/treatment.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/common/vitalStatus.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/datasets/examples/dataset-Max-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-VRS-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/examples/genomicVariant-MIN-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParameters.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/genomicVariations/requestParametersComponents.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/individuals/examples/pedigree-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/phenopackets/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/phenopackets/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/defaultSchema.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/endpoints.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/endpoints.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-model/runs/examples/runs-MAX-example.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Collation.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Collation.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/CytobandMapping.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/CytobandMapping.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencies.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/IntervalFrequencyItem.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/OntologyClass.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Progenetix.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/ProgenetixGene.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Provenance.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/Publication.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/Publication.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/PublicationSampleCounts.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json` & `bycon-1.6.5/bycon/schemas/models/json/progenetix-service-schemas/QueryBufferItem.json`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxAnalysis.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxAnalysis.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxBiosample.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxCollation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxIndividual.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-database-schemas/pgxVariant.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/analyses/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/beaconConfiguration.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/beaconMap.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/beaconMap.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/biosamples/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MAX-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/cohorts/examples/cohorts-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/GeoLocation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/VRSallele.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/VRSallele.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/VRScopyNumberChange.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/VRScopyNumberChange.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/ancestry.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/celllineInfo.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/commonDefinitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/complexValue.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/dataUseConditions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/disease.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/disease.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/doseInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/evidence.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/evidence.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/exposure.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/exposure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/externalReference.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/file.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/file.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/gestationalAge.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/measurement.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/measurement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/metaData.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/metaData.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/ontologyTerm.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/pedigree.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/phenotypicFeature.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/procedure.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/procedure.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/provenance.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/provenance.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/referenceRange.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/resource.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/resource.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/timeElement.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/timeInterval.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/treatment.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/treatment.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/common/vitalStatus.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/datasets/examples/dataset-Max-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/examples/genomicVariant-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParameters.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/genomicVariations/requestParametersComponents.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/individual-with-pedigree-MID-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/individuals/examples/pedigree-example.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/phenopackets/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/phenopackets/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/defaultSchema.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-model/runs/endpoints.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/.DS_Store` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/.DS_Store`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Collation.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Collation.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/CytobandMapping.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/CytobandMapping.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencies.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/IntervalFrequencyItem.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/OntologyClass.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Progenetix.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/ProgenetixGene.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Provenance.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/Publication.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/PublicationSampleCounts.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml` & `bycon-1.6.5/bycon/schemas/models/src/progenetix-service-schemas/QueryBufferItem.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/bycon.egg-info/PKG-INFO` & `bycon-1.6.5/bycon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bycon
-Version: 1.6.3
+Version: 1.6.5
 Summary: A Python-based environment for the Beacon v2 genomics API
 Home-page: https://github.com/progenetix/bycon
 Author: Michael Baudis
 Author-email: contact@progenetix.org
 Project-URL: Bug Reports, https://github.com/progenetix/bycon/issues
 Project-URL: Source, https://github.com/progenetix/bycon/
 Project-URL: Helpers, https://github.com/progenetix/byconaut/
```

### Comparing `bycon-1.6.3/bycon.egg-info/SOURCES.txt` & `bycon-1.6.5/bycon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 ./bycon/definitions/variant_type_definitions.yaml
 ./bycon/lib/__init__.py
 ./bycon/lib/args_parsing.py
 ./bycon/lib/beacon_auth.py
 ./bycon/lib/beacon_response_generation.py
 ./bycon/lib/bycon_helpers.py
 ./bycon/lib/cgi_parsing.py
+./bycon/lib/cytoband_parsing.py
 ./bycon/lib/dataset_parsing.py
 ./bycon/lib/genome_utils.py
 ./bycon/lib/handover_generation.py
 ./bycon/lib/parse_filters_request.py
 ./bycon/lib/parse_variant_request.py
 ./bycon/lib/query_execution.py
 ./bycon/lib/query_generation.py
@@ -452,14 +453,15 @@
 bycon/beaconServer/tests/PUT-variants-for-CDKN2A-DEL-gliomas.json
 bycon/beaconServer/tests/PUT-variants-for-biosampleIds.json
 bycon/beaconServer/tests/PUT-variants-for-specific-alt-bases.json
 bycon/beaconServer/tests/terminal-examples.md
 bycon/definitions/argument_definitions.yaml
 bycon/definitions/dataset_definitions.yaml
 bycon/definitions/datatable_mappings.yaml
+bycon/definitions/entity_defaults.yaml
 bycon/definitions/filter_definitions.yaml
 bycon/definitions/geoloc_definitions.yaml
 bycon/definitions/handover_definitions.yaml
 bycon/definitions/interval_definitions.yaml
 bycon/definitions/variant_request_definitions.yaml
 bycon/definitions/variant_type_definitions.yaml
 bycon/lib/__init__.py
```

### Comparing `bycon-1.6.3/docs/changes.md` & `bycon-1.6.5/docs/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,54 @@
 the code base from this specific use case.
 
 An earlier version of the Progenetix && Beacon "BeaconPlus" stack had been provided
 through the Perl based [**PGX** project](http://github.com/progenetix/PGX/).
 
 ## Changes Tracker
 
+### 2023-04-03 (v1.6.5)
+
+#### Multi-variant matches first pass
+
+We now implement an experimental version of multi-variant matching, to retrieve
+samples which show co-occurrence of 2 or more variants. This so far is limited to
+a few parameters:
+
+* NEW: `variantQueryDigests` in the form of `9:9000001-21975098--21967753-24000000:DEL`
+    - several of those can be comma-concatenated
+    - probably not final name or format
+    - only bracket matches & ranges working (but will change ...)
+    - different variant types can be used
+* `geneId` has been morphed to a list parameter (though keeping the standard name)
+    - usual comma-concatenation etc.
+    - here only a global `variantType` can be provided
+* future versions to implement mixed matches etc. (e.g. sequence variant & CNV)
+
+#### Other ...
+
+* fixed paginated handovers missing the `info.content_id` parameter which is used
+  by the progenetix-web etc. front ends
+* changed the `cytoBands` argument to `type: array`, to allow definition of multiple
+  cytogenetic regions, e.g. to indicate fusions or bracket requests
+    - this might be a temporary solution for testing purposes and e.g. replaced
+      by a future parsing of simple statements like `t(8;14)(q24;q32)`
+* moved some cytoband functionality to the main `bycon` package, from `byconaut`,
+  to allow processing of cytoband requests in the main Beacon service
+* `byconaut` was restructured for exacutables, with `housekeepers` and `importers`
+  directories
+
+### 2024-03-25 (v1.6.4)
+
+* added `scopes` to `beacon/filtering_terms/`
+    - see <https://github.com/ga4gh-beacon/beacon-v2/pull/118>
+* fixed bug where the default splitting of input parameters by comma led to over-splitting
+  of the "embedded list" values in `plotPars` (e.g. using `plotPars=plotGeneSymbols=MYC,T,TP53`
+  would lead to `plotPars=plotGeneSymbols=MYC::T::TP53` ... and later errors)
+    - now "non-list" strings w/ internal `,` are just re-joined & a warning is created
+
 ### 2024-03-07 (v1.6.3)
 
 * configuration changes:
     - `beacon_defaults` file changed to `entity_defaults` since only entities
       defined in it
     - paths are now defined within the entity definitions, no separate aliases etc.
     - local overrides for the Beacon entity defaults now in `local/instance_overrides.yaml`
```

### Comparing `bycon-1.6.3/docs/css/extra.css` & `bycon-1.6.5/docs/css/extra.css`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/future.md` & `bycon-1.6.5/docs/future.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/generated/argument_definitions.md` & `bycon-1.6.5/docs/generated/argument_definitions.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/generated/plot_defaults.md` & `bycon-1.6.5/docs/generated/plot_defaults.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/handovers.md` & `bycon-1.6.5/docs/handovers.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/img/site-logo-main.png` & `bycon-1.6.5/docs/img/site-logo-main.png`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/img/site-logo-topright.png` & `bycon-1.6.5/docs/img/site-logo-topright.png`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/index.md` & `bycon-1.6.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/installation.md` & `bycon-1.6.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/docs/tests.md` & `bycon-1.6.5/docs/tests.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/install.py` & `bycon-1.6.5/install.py`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/local/README.md` & `bycon-1.6.5/local/README.md`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/local/dataset_definitions.yaml` & `bycon-1.6.5/local/dataset_definitions.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/local/instance_overrides.yaml` & `bycon-1.6.5/local/instance_overrides.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
   entity_defaults:
     info:
       collection: Null
       response_schema: beaconInfoResponse
       beacon_schema:
         entity_type: configuration
         schema: https://progenetix.org/services/schemas/beaconInfoResults/
-      # TODO: move `content` to `local` file.
       content:
         beacon_id: org.progenetix
         name: Progenetix Cancer Genomics Beacon+
         api_version: v2.1.0-beaconplus
         version: v2.1.0-beaconplus
         id: org.progenetix.beacon
         environment: prod
```

### Comparing `bycon-1.6.3/mkdocs.yaml` & `bycon-1.6.5/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `bycon-1.6.3/setup.py` & `bycon-1.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="bycon",
-    version="1.6.3",
+    version="1.6.5",
     description="A Python-based environment for the Beacon v2 genomics API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/progenetix/bycon",
     author="Michael Baudis",
     author_email="contact@progenetix.org",
     classifiers=[
```

