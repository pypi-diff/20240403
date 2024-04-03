# Comparing `tmp/osm-fieldwork-0.6.1.tar.gz` & `tmp/osm-fieldwork-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm-fieldwork-0.6.1.tar", last modified: Mon Mar 25 05:51:42 2024, max compression
+gzip compressed data, was "osm-fieldwork-0.7.0.tar", last modified: Wed Apr  3 14:05:45 2024, max compression
```

## Comparing `osm-fieldwork-0.6.1.tar` & `osm-fieldwork-0.7.0.tar`

### file list

```diff
@@ -1,88 +1,89 @@
--rw-r--r--   0        0        0    34102 2024-03-25 05:51:33.967916 osm-fieldwork-0.6.1/LICENSE.md
--rw-r--r--   0        0        0    14494 2024-03-25 05:51:33.967916 osm-fieldwork-0.6.1/README.md
--rwxr-xr-x   0        0        0    13091 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/CSVDump.py
--rwxr-xr-x   0        0        0     5037 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/ODKDump.py
--rwxr-xr-x   0        0        0     5072 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/ODKForm.py
--rwxr-xr-x   0        0        0     4919 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/ODKInstance.py
--rwxr-xr-x   0        0        0    60820 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/OdkCentral.py
--rw-r--r--   0        0        0       99 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/__init__.py
--rw-r--r--   0        0        0       22 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/__version__.py
--rwxr-xr-x   0        0        0    20165 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/basemapper.py
--rwxr-xr-x   0        0        0    11364 2024-03-25 05:51:33.975916 osm-fieldwork-0.6.1/osm_fieldwork/convert.py
--rw-r--r--   0        0        0   683456 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
--rw-r--r--   0        0        0      883 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/__init__.py
--rw-r--r--   0        0        0      387 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/amenities.yaml
--rw-r--r--   0        0        0      348 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/buildings.yaml
--rw-r--r--   0        0        0      247 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/camping.yaml
--rw-r--r--   0        0        0      777 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/category.yaml
--rw-r--r--   0        0        0      126 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/cemeteries.yaml
--rw-r--r--   0        0        0      437 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/education.yaml
--rw-r--r--   0        0        0      126 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/emergency.yaml
--rw-r--r--   0        0        0      490 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/health.yaml
--rw-r--r--   0        0        0      193 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/highways.yaml
--rw-r--r--   0        0        0       80 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/landusage.yaml
--rw-r--r--   0        0        0    14028 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/models.yaml
--rw-r--r--   0        0        0       90 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/nature.yaml
--rw-r--r--   0        0        0       88 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/places.yaml
--rw-r--r--   0        0        0       91 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/religious.yaml
--rw-r--r--   0        0        0        0 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/taginfo-db.db
--rw-r--r--   0        0        0      253 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/toilets.yaml
--rwxr-xr-x   0        0        0     4643 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/validate.py
--rw-r--r--   0        0        0      415 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/wastedisposal.yaml
--rw-r--r--   0        0        0      185 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/waterpoints.yaml
--rw-r--r--   0        0        0      128 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/data_models/waterways.yaml
--rw-r--r--   0        0        0     1609 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/filter.yaml
--rwxr-xr-x   0        0        0     8929 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/filter_data.py
--rw-r--r--   0        0        0      798 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/imagery.yaml
--rwxr-xr-x   0        0        0    15977 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/json2osm.py
--rwxr-xr-x   0        0        0     7371 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/make_data_extract.py
--rw-r--r--   0        0        0     3405 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/models.yaml
--rwxr-xr-x   0        0        0     5416 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/odk2csv.py
--rwxr-xr-x   0        0        0     4298 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/odk2geojson.py
--rwxr-xr-x   0        0        0     5348 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/odk2osm.py
--rwxr-xr-x   0        0        0    17845 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/odk_client.py
--rwxr-xr-x   0        0        0    23342 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/odk_merge.py
--rwxr-xr-x   0        0        0     5302 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/osm2favorities.py
--rwxr-xr-x   0        0        0    15231 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/osmfile.py
--rwxr-xr-x   0        0        0     9381 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/sqlite.py
--rw-r--r--   0        0        0     3717 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/xforms.yaml
--rw-r--r--   0        0        0     3795 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/Makefile
--rw-r--r--   0        0        0     1151 2024-03-25 05:51:33.979916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/__init__.py
--rw-r--r--   0        0        0  1469440 2024-03-25 05:51:33.983916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/amenities.xls
--rw-r--r--   0        0        0   240128 2024-03-25 05:51:33.983916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/buildings.xls
--rw-r--r--   0        0        0  3986944 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/camping.xls
--rw-r--r--   0        0        0    98816 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/cemeteries.xls
--rw-r--r--   0        0        0   111104 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/education.xls
--rw-r--r--   0        0        0      220 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/entities/__init__.py
--rw-r--r--   0        0        0   108032 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/entities/registration_form.xls
--rw-r--r--   0        0        0    69120 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/health.xls
--rw-r--r--   0        0        0    40448 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/highways.xls
--rw-r--r--   0        0        0    22528 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/historical.xls
--rw-r--r--   0        0        0    15872 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/hotspring.xls
--rw-r--r--   0        0        0    59904 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/landusage.xls
--rw-r--r--   0        0        0   129536 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/landuse.xls
--rw-r--r--   0        0        0     1629 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/amenities.csv
--rw-r--r--   0        0        0      466 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/buildings.csv
--rw-r--r--   0        0        0       40 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/municipality.csv
--rw-r--r--   0        0        0      353 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/opening_hours.csv
--rw-r--r--   0        0        0      160 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/operational_status.csv
--rw-r--r--   0        0        0      171 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/provider.csv
--rw-r--r--   0        0        0     1737 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/towns.csv
--rw-r--r--   0        0        0       76 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/waste.csv
--rw-r--r--   0        0        0       41 2024-03-25 05:51:33.995916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/municipality.csv
--rw-r--r--   0        0        0    59392 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/nature.xls
--rw-r--r--   0        0        0   126976 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/places.xls
--rw-r--r--   0        0        0   103424 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/religious.xls
--rw-r--r--   0        0        0   115963 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/solidwaste.xlsx
--rw-r--r--   0        0        0   265216 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/test.xls
--rw-r--r--   0        0        0   353280 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/thamel.xls
--rw-r--r--   0        0        0   118272 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/toilets.xls
--rw-r--r--   0        0        0      112 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/towns.csv
--rw-r--r--   0        0        0    40448 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/transportation.xls
--rw-r--r--   0        0        0    15186 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waste_collection.xlsx
--rw-r--r--   0        0        0   101888 2024-03-25 05:51:33.999916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/wastedisposal.xls
--rw-r--r--   0        0        0   211456 2024-03-25 05:51:34.003916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waterpoints.xls
--rw-r--r--   0        0        0   269312 2024-03-25 05:51:34.003916 osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waterways.xls
--rwxr-xr-x   0        0        0     5443 2024-03-25 05:51:34.003916 osm-fieldwork-0.6.1/osm_fieldwork/yamlfile.py
--rw-r--r--   0        0        0     3525 2024-03-25 05:51:34.003916 osm-fieldwork-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34102 2024-04-03 14:05:37.625084 osm-fieldwork-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    14494 2024-04-03 14:05:37.625084 osm-fieldwork-0.7.0/README.md
+-rwxr-xr-x   0        0        0    13091 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/CSVDump.py
+-rwxr-xr-x   0        0        0     5037 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/ODKDump.py
+-rwxr-xr-x   0        0        0     5072 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/ODKForm.py
+-rwxr-xr-x   0        0        0     4919 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/ODKInstance.py
+-rwxr-xr-x   0        0        0    60821 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/OdkCentral.py
+-rwxr-xr-x   0        0        0    17469 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/OdkCentralAsync.py
+-rw-r--r--   0        0        0       99 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/__version__.py
+-rwxr-xr-x   0        0        0    20165 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/basemapper.py
+-rwxr-xr-x   0        0        0    11364 2024-04-03 14:05:37.629084 osm-fieldwork-0.7.0/osm_fieldwork/convert.py
+-rw-r--r--   0        0        0   683456 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx
+-rw-r--r--   0        0        0      883 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/__init__.py
+-rw-r--r--   0        0        0      387 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/amenities.yaml
+-rw-r--r--   0        0        0      348 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/buildings.yaml
+-rw-r--r--   0        0        0      247 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/camping.yaml
+-rw-r--r--   0        0        0      777 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/category.yaml
+-rw-r--r--   0        0        0      126 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/cemeteries.yaml
+-rw-r--r--   0        0        0      437 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/education.yaml
+-rw-r--r--   0        0        0      126 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/emergency.yaml
+-rw-r--r--   0        0        0      490 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/health.yaml
+-rw-r--r--   0        0        0      193 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/highways.yaml
+-rw-r--r--   0        0        0       80 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/landusage.yaml
+-rw-r--r--   0        0        0    14028 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/models.yaml
+-rw-r--r--   0        0        0       90 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/nature.yaml
+-rw-r--r--   0        0        0       88 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/places.yaml
+-rw-r--r--   0        0        0       91 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/religious.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/taginfo-db.db
+-rw-r--r--   0        0        0      253 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/toilets.yaml
+-rwxr-xr-x   0        0        0     4643 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/validate.py
+-rw-r--r--   0        0        0      415 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/wastedisposal.yaml
+-rw-r--r--   0        0        0      185 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/waterpoints.yaml
+-rw-r--r--   0        0        0      128 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/data_models/waterways.yaml
+-rw-r--r--   0        0        0     1609 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/filter.yaml
+-rwxr-xr-x   0        0        0     8929 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/filter_data.py
+-rw-r--r--   0        0        0      798 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/imagery.yaml
+-rwxr-xr-x   0        0        0    15977 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/json2osm.py
+-rwxr-xr-x   0        0        0     7371 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/make_data_extract.py
+-rw-r--r--   0        0        0     3405 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/models.yaml
+-rwxr-xr-x   0        0        0     5416 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/odk2csv.py
+-rwxr-xr-x   0        0        0     4298 2024-04-03 14:05:37.633084 osm-fieldwork-0.7.0/osm_fieldwork/odk2geojson.py
+-rwxr-xr-x   0        0        0     5348 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/odk2osm.py
+-rwxr-xr-x   0        0        0    17845 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/odk_client.py
+-rwxr-xr-x   0        0        0    23342 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/odk_merge.py
+-rwxr-xr-x   0        0        0     5302 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/osm2favorities.py
+-rwxr-xr-x   0        0        0    15231 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/osmfile.py
+-rwxr-xr-x   0        0        0     9381 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/sqlite.py
+-rw-r--r--   0        0        0     3717 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/xforms.yaml
+-rw-r--r--   0        0        0     3795 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/Makefile
+-rw-r--r--   0        0        0     1151 2024-04-03 14:05:37.637084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/__init__.py
+-rw-r--r--   0        0        0  1469440 2024-04-03 14:05:37.641084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/amenities.xls
+-rw-r--r--   0        0        0   240128 2024-04-03 14:05:37.641084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/buildings.xls
+-rw-r--r--   0        0        0  3986944 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/camping.xls
+-rw-r--r--   0        0        0    98816 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/cemeteries.xls
+-rw-r--r--   0        0        0   111104 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/education.xls
+-rw-r--r--   0        0        0      220 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/entities/__init__.py
+-rw-r--r--   0        0        0   108032 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/entities/registration_form.xls
+-rw-r--r--   0        0        0    69120 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/health.xls
+-rw-r--r--   0        0        0    40448 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/highways.xls
+-rw-r--r--   0        0        0    22528 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/historical.xls
+-rw-r--r--   0        0        0    15872 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/hotspring.xls
+-rw-r--r--   0        0        0    59904 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/landusage.xls
+-rw-r--r--   0        0        0   129536 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/landuse.xls
+-rw-r--r--   0        0        0     1629 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/amenities.csv
+-rw-r--r--   0        0        0      466 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/buildings.csv
+-rw-r--r--   0        0        0       40 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/municipality.csv
+-rw-r--r--   0        0        0      353 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/opening_hours.csv
+-rw-r--r--   0        0        0      160 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/operational_status.csv
+-rw-r--r--   0        0        0      171 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/provider.csv
+-rw-r--r--   0        0        0     1737 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/towns.csv
+-rw-r--r--   0        0        0       76 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/waste.csv
+-rw-r--r--   0        0        0       41 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/municipality.csv
+-rw-r--r--   0        0        0    59392 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/nature.xls
+-rw-r--r--   0        0        0   126976 2024-04-03 14:05:37.653084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/places.xls
+-rw-r--r--   0        0        0   103424 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/religious.xls
+-rw-r--r--   0        0        0   115963 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/solidwaste.xlsx
+-rw-r--r--   0        0        0   265216 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/test.xls
+-rw-r--r--   0        0        0   353280 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/thamel.xls
+-rw-r--r--   0        0        0   118272 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/toilets.xls
+-rw-r--r--   0        0        0      112 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/towns.csv
+-rw-r--r--   0        0        0    40448 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/transportation.xls
+-rw-r--r--   0        0        0    15186 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waste_collection.xlsx
+-rw-r--r--   0        0        0   101888 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/wastedisposal.xls
+-rw-r--r--   0        0        0   211456 2024-04-03 14:05:37.657084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waterpoints.xls
+-rw-r--r--   0        0        0   269312 2024-04-03 14:05:37.661084 osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waterways.xls
+-rwxr-xr-x   0        0        0     5443 2024-04-03 14:05:37.661084 osm-fieldwork-0.7.0/osm_fieldwork/yamlfile.py
+-rw-r--r--   0        0        0     3547 2024-04-03 14:05:37.661084 osm-fieldwork-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    15261 1970-01-01 00:00:00.000000 osm-fieldwork-0.7.0/PKG-INFO
```

### Comparing `osm-fieldwork-0.6.1/LICENSE.md` & `osm-fieldwork-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/README.md` & `osm-fieldwork-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/CSVDump.py` & `osm-fieldwork-0.7.0/osm_fieldwork/CSVDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/ODKDump.py` & `osm-fieldwork-0.7.0/osm_fieldwork/ODKDump.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/ODKForm.py` & `osm-fieldwork-0.7.0/osm_fieldwork/ODKForm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/ODKInstance.py` & `osm-fieldwork-0.7.0/osm_fieldwork/ODKInstance.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/OdkCentral.py` & `osm-fieldwork-0.7.0/osm_fieldwork/OdkCentral.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,17 +154,14 @@
 
         # Authentication with session token
         self.authenticate()
 
         # These are just cached data from the queries
         self.projects = dict()
         self.users = list()
-        # The number of threads is based on the CPU cores
-        info = get_cpu_info()
-        self.cores = info["count"]
 
     def authenticate(
         self,
         url: str = None,
         user: str = None,
         passwd: str = None,
     ):
@@ -426,14 +423,18 @@
         Args:
             project_id (int): The ID of the project on ODK Central
             xforms (list): The list of XForms to get the submissions of
 
         Returns:
             (json): All of the submissions for all of the XForm in a project
         """
+        # The number of threads is based on the CPU cores
+        info = get_cpu_info()
+        self.cores = info["count"]
+
         timer = Timer(text="getAllSubmissions() took {seconds:.0f}s")
         timer.start()
         if not xforms:
             xforms_data = self.listForms(project_id)
             xforms = [d["xmlFormId"] for d in xforms_data]
 
         chunk = round(len(xforms) / self.cores) if round(len(xforms) / self.cores) > 0 else 1
```

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/basemapper.py` & `osm-fieldwork-0.7.0/osm_fieldwork/basemapper.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/convert.py` & `osm-fieldwork-0.7.0/osm_fieldwork/convert.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx` & `osm-fieldwork-0.7.0/osm_fieldwork/data_models/Impact Areas - Data Models V1.1.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/data_models/__init__.py` & `osm-fieldwork-0.7.0/osm_fieldwork/data_models/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/data_models/category.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/data_models/category.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/data_models/models.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/data_models/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/data_models/validate.py` & `osm-fieldwork-0.7.0/osm_fieldwork/data_models/validate.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/filter.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/filter.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/filter_data.py` & `osm-fieldwork-0.7.0/osm_fieldwork/filter_data.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/imagery.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/imagery.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/json2osm.py` & `osm-fieldwork-0.7.0/osm_fieldwork/json2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/make_data_extract.py` & `osm-fieldwork-0.7.0/osm_fieldwork/make_data_extract.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/models.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/models.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/odk2csv.py` & `osm-fieldwork-0.7.0/osm_fieldwork/odk2csv.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/odk2geojson.py` & `osm-fieldwork-0.7.0/osm_fieldwork/odk2geojson.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/odk2osm.py` & `osm-fieldwork-0.7.0/osm_fieldwork/odk2osm.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/odk_client.py` & `osm-fieldwork-0.7.0/osm_fieldwork/odk_client.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/odk_merge.py` & `osm-fieldwork-0.7.0/osm_fieldwork/odk_merge.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/osm2favorities.py` & `osm-fieldwork-0.7.0/osm_fieldwork/osm2favorities.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/osmfile.py` & `osm-fieldwork-0.7.0/osm_fieldwork/osmfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/sqlite.py` & `osm-fieldwork-0.7.0/osm_fieldwork/sqlite.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xforms.yaml` & `osm-fieldwork-0.7.0/osm_fieldwork/xforms.yaml`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/Makefile` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/Makefile`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/__init__.py` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/__init__.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/amenities.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/amenities.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/buildings.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/buildings.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/camping.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/camping.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/cemeteries.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/cemeteries.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/education.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/education.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/entities/registration_form.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/entities/registration_form.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/health.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/health.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/highways.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/highways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/historical.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/historical.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/hotspring.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/hotspring.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/landusage.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/landusage.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/landuse.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/landuse.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/amenities.csv` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/amenities.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/lib/towns.csv` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/lib/towns.csv`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/nature.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/nature.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/places.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/places.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/religious.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/religious.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/solidwaste.xlsx` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/solidwaste.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/test.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/test.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/thamel.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/thamel.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/toilets.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/toilets.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/transportation.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/transportation.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waste_collection.xlsx` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waste_collection.xlsx`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/wastedisposal.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/wastedisposal.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waterpoints.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waterpoints.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/xlsforms/waterways.xls` & `osm-fieldwork-0.7.0/osm_fieldwork/xlsforms/waterways.xls`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/osm_fieldwork/yamlfile.py` & `osm-fieldwork-0.7.0/osm_fieldwork/yamlfile.py`

 * *Files identical despite different names*

### Comparing `osm-fieldwork-0.6.1/pyproject.toml` & `osm-fieldwork-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "mercantile>=1.2.1",
     "pySmartDL>=1.3.4",
     "pandas>=1.5.0",
     "py-cpuinfo>=9.0.0",
     "requests>=2.26.0",
     "pmtiles>=3.2.0",
     "osm-rawdata>=0.1.7",
+    "aiohttp>=3.9.3",
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 license = "GPL-3.0-only"
 keywords = [
     "hot",
     "odk",
@@ -38,15 +39,15 @@
 classifiers = [
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering :: GIS",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "0.6.1"
+version = "0.7.0"
 
 [project.urls]
 homepage = "https://github.com/hotosm/osm-fieldwork/wiki"
 documentation = "https://hotosm.github.io/osm-fieldwork"
 repository = "https://github.com/hotosm/osm-fieldwork"
 
 [project.scripts]
@@ -72,15 +73,15 @@
 testpaths = [
     "tests",
 ]
 pythonpath = "osm_fieldwork"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.1"
+version = "0.7.0"
 version_files = [
     "pyproject.toml:version",
     "osm_fieldwork/__version__.py",
     "Makefile:VERSION",
 ]
 update_changelog_on_bump = true
```

### Comparing `osm-fieldwork-0.6.1/PKG-INFO` & `osm-fieldwork-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm-fieldwork
-Version: 0.6.1
+Version: 0.7.0
 Summary: Processing field data from ODK to OpenStreetMap format.
 License: GPL-3.0-only
 Keywords: hot,odk,openstreetmap,fmtm
 Author-email: Rob Savoye <rob.savoye@hotosm.org>,Sam Woodcock <sam.woodcock@hotosm.org>
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.6.1 Summary: Processing
+Metadata-Version: 2.1 Name: osm-fieldwork Version: 0.7.0 Summary: Processing
 field data from ODK to OpenStreetMap format. License: GPL-3.0-only Keywords:
 hot,odk,openstreetmap,fmtm Author-email: Rob Savoye
 hotosm.org>,Sam Woodcock
 hotosm.org> Requires-Python: >=3.10 Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Utilities Project-URL: documentation, https://
```

