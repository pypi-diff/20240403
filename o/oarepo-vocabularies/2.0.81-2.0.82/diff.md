# Comparing `tmp/oarepo-vocabularies-2.0.81.tar.gz` & `tmp/oarepo-vocabularies-2.0.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-vocabularies-2.0.81.tar", last modified: Wed Mar 27 13:56:07 2024, max compression
+gzip compressed data, was "oarepo-vocabularies-2.0.82.tar", last modified: Wed Apr  3 07:31:59 2024, max compression
```

## Comparing `oarepo-vocabularies-2.0.81.tar` & `oarepo-vocabularies-2.0.82.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.729881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.729881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/ext_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.729881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/resources/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/hacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/models/ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/systemfields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/records/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/records/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.733881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/components/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/components/scanning_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/custom_fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/custom_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/custom_fields/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/type_ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/ui_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.717881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.717881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.717881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.717881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.717881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.737881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.741881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.741881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.741881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/deposit.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.741881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.741881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.745881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.745881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.721881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.745881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.745881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.749881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.753881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.725881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/webpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-27 13:56:07.000000 oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-03-27 13:56:07.757881 oarepo-vocabularies-2.0.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 13:52:01.000000 oarepo-vocabularies-2.0.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.206923 oarepo-vocabularies-2.0.82/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 07:31:59.206923 oarepo-vocabularies-2.0.82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.174923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/ext_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/resources/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/hacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/models/ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.178923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/vocabularies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/systemfields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/records/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/components/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/components/scanning_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/custom_fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/custom_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/custom_fields/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/type_ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/ui_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.182923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.186923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/deposit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.190923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.190923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/TaxonomyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/VocabularyArray.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/VocabularyItem.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.166923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.190923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/SidebarLink.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesForm.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSearch.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/descendants.html
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/search.html
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/translations.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.190923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.194923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.198923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/VocabularyButtonSidebar.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyButtonSidebar/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/translationKeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.170923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/breadcrumb.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/collections/grid.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/themes/default/modules/vocabulary_cf.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.174923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.174923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.174923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/webpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:31:59.202923 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-03 07:31:58.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-03 07:31:59.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:31:58.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-03 07:31:58.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-03 07:31:58.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 07:31:58.000000 oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-04-03 07:31:59.206923 oarepo-vocabularies-2.0.82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:27:17.000000 oarepo-vocabularies-2.0.82/setup.py
```

### Comparing `oarepo-vocabularies-2.0.81/LICENSE` & `oarepo-vocabularies-2.0.82/LICENSE`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/MANIFEST.in` & `oarepo-vocabularies-2.0.82/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/PKG-INFO` & `oarepo-vocabularies-2.0.82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.81
+Version: 2.0.82
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo-vocabularies-2.0.81/README.md` & `oarepo-vocabularies-2.0.82/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/components.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/components.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/ext.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/resources/resource.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/resources/resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             id=resource_requestctx.view_args["type"]
         ).one()
         if not authority_service:
             return "No authority getter.", 404
 
         # Get hits from authority.
         params = resource_requestctx.args
-        q, page, size = params["q"], params["page"], params["size"]
+        q, page, size = params.get("suggest"), params.get("page", 1), params.get("size", 20)
         results = authority_service.search(query=q, page=page, size=size)
 
         # Mark external, resolve uuid.
         ids = [item["id"] for item in results["hits"]["hits"]]
 
         internal_query = db.session.query(PersistentIdentifier.pid_value).filter(
             db.and_(
```

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/authorities/service.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/authorities/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ext.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/fixtures.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/fixtures.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/hacks.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/hacks.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/models/ui.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/models/ui.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/api.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/jsonschemas/vocabularies/vocabulary-ext-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/records/systemfields.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/records/systemfields.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/records/ui.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/ui.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/resources/vocabulary_type/resource.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/components/hierarchy.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/components/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/custom_fields/hierarchy.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/custom_fields/hierarchy.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/facets.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/permissions.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/schema.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/search.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/service.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/services/ui_schema.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/services/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/theme/assets/semantic-ui/translations/oarepo_vocabularies/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/translations/messages.pot` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/ext.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/deposit.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/deposit.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/components/vocabulary_ui_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/resource.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/config.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/resources/vocabulary_type/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/TaxonomyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/VocabularyItem.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/VocabularyItem.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesDetail.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesList.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesMain.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/VocabulariesSidebar.jinja`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/templates/semantic-ui/oarepo_vocabularies_ui/test_header_template.html`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/custom-components.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/DetailSearchApp.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/Results.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/detail/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/FormAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/VocabularyFormSchema.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/CurrentLocationInformation.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumb.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/CurrentLocationInformation/VocabularyBreadcrumbMessage.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/FeaturedButton/FeaturedButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/LocalVocabularySelectField/LocalVocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PropFieldsComponent/PropFieldsComponent.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/PublishButton/PublishButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/ResetButton/ResetButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormControlPanel/VocabularyFormControlPanel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyFormFields/VocabularyFormFields.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularyMultilingualInputField/VocabularyMultilingualInputField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/components/VocabularySelectField/VocabularySelectField.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/form/hooks.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/app.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/NewItemButton/NewItemButton.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/search/components/VocabularyResultsListItem/VocabularyResultsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/js/oarepo_vocabularies_ui/utils.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/dl_table.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/sample.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/less/oarepo_vocabularies_ui/definitions/vocabulary_cf.less`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/assets/semantic-ui/translations/oarepo_vocabularies_ui/messages/en/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/theme/webpack.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/utils.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/ui/views.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/ui/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/api.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies/views/app.py` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies/views/app.py`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/PKG-INFO` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-vocabularies
-Version: 2.0.81
+Version: 2.0.82
 Summary: Support for custom fields and hierarchy on Invenio vocabularies
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: invenio-vocabularies
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
```

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/SOURCES.txt` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/oarepo_vocabularies.egg-info/entry_points.txt` & `oarepo-vocabularies-2.0.82/oarepo_vocabularies.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-vocabularies-2.0.81/setup.cfg` & `oarepo-vocabularies-2.0.82/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-vocabularies
-version = 2.0.81
+version = 2.0.82
 description = Support for custom fields and hierarchy on Invenio vocabularies
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

