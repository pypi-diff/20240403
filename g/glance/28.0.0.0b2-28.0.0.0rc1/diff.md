# Comparing `tmp/glance-28.0.0.0b2.tar.gz` & `tmp/glance-28.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glance-28.0.0.0b2.tar", last modified: Fri Jan 12 15:30:32 2024, max compression
+gzip compressed data, was "glance-28.0.0.0rc1.tar", last modified: Thu Mar 14 19:58:42 2024, max compression
```

## Comparing `glance-28.0.0.0b2.tar` & `glance-28.0.0.0rc1.tar`

### file list

```diff
@@ -1,981 +1,999 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15610 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25787 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   228548 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.854989 glance-28.0.0.0b2/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.866990 glance-28.0.0.0b2/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6702 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/heading-level-guide.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.866990 glance-28.0.0.0b2/api-ref/source/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/cache-manage-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/cache-manage.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1712 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/discovery-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/discovery.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4662 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-data.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22513 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-images-v2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13388 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-import.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-parameters-descriptions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21246 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-schemas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-sharing-v2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/images-tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-objects.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6374 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-properties.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8772 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13711 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-resourcetypes.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/metadefs-schemas.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.878990 glance-28.0.0.0b2/api-ref/source/v2/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/cache-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-details-deactivate-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-import-c-i-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-import-g-d-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-import-gd-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-import-w-d-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-info-import-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-member-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-member-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-member-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-member-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-member-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-members-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-tasks-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/image-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/images-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request-simple.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response-simple.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespaces-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7469 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-objects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-properties-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-assoc-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-assoc-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-resource-type-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-resource-types-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tag-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tag-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tag-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tag-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tags-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tags-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-tags-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-member-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-members-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7811 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11491 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-images-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-object-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6101 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4593 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-property-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-task-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-tasks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/stores-list-detail-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/stores-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/task-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/task-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-failure-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-processing-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-success-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/tasks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/samples/usage-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/stores.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/tasks-parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/tasks-schemas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/v2/tasks.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.878990 glance-28.0.0.0b2/api-ref/source/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3669 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/versions/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.878990 glance-28.0.0.0b2/api-ref/source/versions/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4454 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/versions/samples/image-versions-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/api-ref/source/versions/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.878990 glance-28.0.0.0b2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.882990 glance-28.0.0.0b2/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.882990 glance-28.0.0.0b2/doc/source/_extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/_extra/.htaccess
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.882990 glance-28.0.0.0b2/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.882990 glance-28.0.0.0b2/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/apache-httpd.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/authentication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/cache.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8121 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/controllingservers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/db-sqlalchemy-migrate.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/db.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/flows.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31604 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/interoperable-image-import.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13329 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/manage-images.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7589 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/multistores.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/os_hash_algo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/policies.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3824 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/property-protections.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7550 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/requirements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/rollingupgrades.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/tasks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16419 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/troubleshooting.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26695 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/useful-image-properties.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/admin/zero-downtime-db-upgrade.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.886990 glance-28.0.0.0b2/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/footer.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/general_options.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glanceapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancecachecleaner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancecachemanage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancecacheprefetcher.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancecachepruner.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancecontrol.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancemanage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancereplicator.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5295 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancescrubber.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/glancestatus.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/header.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/cli/openstack_options.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.886990 glance-28.0.0.0b2/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61077 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/configuring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/glance_api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/glance_cache.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/glance_manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/glance_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/glance_scrubber.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/configuration/sample-configuration.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.890990 glance-28.0.0.0b2/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3839 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/blueprints.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8712 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5869 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/core_reviewer_guidelines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/database_architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13229 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/database_migrations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/documentation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/domain_implementation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10110 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/domain_model.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/gerrit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/glance-groups.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/minor-code-changes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/refreshing-configs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12244 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/release-cpl.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/release-notes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/contributor/releasecycle.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/deprecation-note.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   120177 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.890990 glance-28.0.0.0b2/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48303 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/architecture.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108006 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/glance_db.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32606 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/glance_layers.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   250651 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/image_status_transition.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28449 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/instance-life-1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39847 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/instance-life-2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30176 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images/instance-life-3.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.894990 glance-28.0.0.0b2/doc/source/images_src/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57938 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images_src/architecture.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12358 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images_src/glance_db.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21398 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images_src/glance_layers.graphml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/images_src/image_status_transition.dot
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.894990 glance-28.0.0.0b2/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/configure-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/edit-glance-api-conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/get-started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6686 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/install-debian.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/install-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6814 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6675 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/note_configuration_vary_by_distribution.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/register-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.894990 glance-28.0.0.0b2/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/common-image-properties.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6185 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/formats.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34733 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/glanceapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/glanceclient.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19470 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/glancemetadefcatalogapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/identifiers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8930 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/metadefs-concepts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4682 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/os_hash_algo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/signature.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/source/user/statuses.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.898990 glance-28.0.0.0b2/doc/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4624 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/doc/test/redirect-tests.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.898990 glance-28.0.0.0b2/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   204721 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-api.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82774 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-cache.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8409 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-image-import.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10401 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-manage.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85943 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-scrubber.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/glance-swift.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.902990 glance-28.0.0.0b2/etc/metadefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5190 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/cim-processor-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/cim-resource-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5168 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/cim-storage-allocation-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5239 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/cim-virtual-system-setting-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-aggr-disk-filter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-aggr-iops-filter.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-aggr-num-instances.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-cpu-mode.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-cpu-pinning.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-guest-memory-backing.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-guest-shutdown.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-host-capabilities.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-hypervisor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-instance-data.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7583 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-libvirt-image.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-libvirt.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-quota.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-randomgen.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vcputopology.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vmware-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vmware-quota-flavor.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vmware.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vtpm-hw.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-vtpm.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-watchdog.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/compute-xenapi.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/glance-common-image-props.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/image-signature-verification.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/operating-system.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18731 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/software-databases.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5252 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/software-runtimes.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5772 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/software-webservers.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/metadefs/storage-volume-type.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.906990 glance-28.0.0.0b2/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/oslo-config-generator/glance-api.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/oslo-config-generator/glance-cache.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/oslo-config-generator/glance-image-import.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/oslo-config-generator/glance-manage.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/oslo-config-generator/glance-scrubber.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/ovf-metadata.json.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/property-protections-policies.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/property-protections-roles.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/etc/schema-image.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.906990 glance-28.0.0.0b2/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.906990 glance-28.0.0.0b2/glance/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8321 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.910990 glance-28.0.0.0b2/glance/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5750 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/gzip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4515 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/middleware/version_negotiation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7339 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/property_protections.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.910990 glance-28.0.0.0b2/glance/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v1/router.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.910990 glance-28.0.0.0b2/glance/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10253 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/cached_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6785 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/image_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26019 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/image_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19505 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/image_members.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/image_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84197 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38032 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/metadef_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/metadef_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/metadef_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14015 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/metadef_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/metadef_tags.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.914990 glance-28.0.0.0b2/glance/api/v2/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_property_item_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2354 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_property_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/model/metadef_tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17869 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29774 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16565 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/v2/tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/api/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.914990 glance-28.0.0.0b2/glance/async_/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.914990 glance-28.0.0.0b2/glance/async_/flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.914990 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5431 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/base_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/copy_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/glance_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/web_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41972 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/api_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20847 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/base_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/convert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11075 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/ovf_process.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.918990 glance-28.0.0.0b2/glance/async_/flows/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/image_conversion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5747 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/image_decompression.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/inject_image_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/no_op.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/flows/plugins/plugin_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7319 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/taskflow_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/async_/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.918990 glance-28.0.0.0b2/glance/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/cache_cleaner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17537 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/cache_prefetcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/cache_pruner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13626 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23152 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27453 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/replicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12068 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22672 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28492 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/crypt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14512 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/exception.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    25753 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/format_inspector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/common/location_strategy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4768 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/location_strategy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/location_strategy/location_order.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4352 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/location_strategy/store_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9594 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/property_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/removed_config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/common/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/common/scripts/api_image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/api_image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/api_image_import/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/common/scripts/image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6684 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/image_import/main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/scripts/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9190 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/trust_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26263 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47441 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/wsgi_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/common/wsme_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35374 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.922990 glance-28.0.0.0b2/glance/db/simple/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/simple/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69950 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/simple/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.926990 glance-28.0.0.0b2/glance/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.926990 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10416 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9108 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7878 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/alembic.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.930990 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3949 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/migrate.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1283 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2217 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5857 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    84402 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19654 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadata.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10830 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/property.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8271 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7716 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/tag.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7137 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/models_metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/sqlalchemy/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/db/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/domain/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23897 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/domain/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20262 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/domain/proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8814 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/gateway.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4119 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/housekeeping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/image_cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16440 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/cleaner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4433 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/image_cache/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6566 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17261 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/drivers/sqlite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16698 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/drivers/xattr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/prefetcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/image_cache/pruner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.934990 glance-28.0.0.0b2/glance/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59075 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/de/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   168210 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53588 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/es/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    54628 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/fr/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53703 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/it/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    66528 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/ja/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57013 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53118 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65007 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/ru/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44846 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49820 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/glance.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.858990 glance-28.0.0.0b2/glance/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48320 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/glance.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25816 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32705 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5231 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11416 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4471 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/policies/tasks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.938990 glance-28.0.0.0b2/glance/quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14945 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/quota/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/quota/keystone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8048 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15248 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/scrubber.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.942990 glance-28.0.0.0b2/glance/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.942990 glance-28.0.0.0b2/glance/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/etc/glance-swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/etc/policy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/etc/property-protections-policies.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/etc/property-protections.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/etc/schema-image.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.942990 glance-28.0.0.0b2/glance/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71295 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.946990 glance-28.0.0.0b2/glance/tests/functional/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   117013 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35782 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/base_metadef.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.946990 glance-28.0.0.0b2/glance/tests/functional/db/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka02.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_contract01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7851 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7706 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_contract01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1749 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand02.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_train_migrate01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_wallaby_expand01.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11436 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17728 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/db/test_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/ft_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.946990 glance-28.0.0.0b2/glance/tests/functional/serial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/serial/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16797 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/serial/test_scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6839 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16376 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_cache_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_client_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_client_redirects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3750 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_cors_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_glance_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_gzip_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_healthcheck_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2790 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5833 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_reload.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_sqlite.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7126 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/test_wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.950991 glance-28.0.0.0b2/glance/tests/functional/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/metadef_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14754 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_cache_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8759 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_cache_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6274 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   322003 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40391 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_images_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9095 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_images_import_locking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12996 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_legacy_update_cinder_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9384 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_member_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31238 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_namespace_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18312 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_namespaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12372 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_object_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18926 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16330 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_properties.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12598 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_property_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11533 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetypes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14844 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_tag_api_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16401 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_schemas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_tasks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/functional/v2/test_tasks_api_policy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.950991 glance-28.0.0.0b2/glance/tests/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/integration/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.950991 glance-28.0.0.0b2/glance/tests/integration/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/integration/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6182 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/integration/v2/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/integration/v2/test_property_quota_violations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20800 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/integration/v2/test_tasks_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/stubs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/test_hacking.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6390 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/middleware/test_cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9192 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/test_cmd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6792 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14130 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/api/test_property_protections.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/async_/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/async_/flows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15047 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_image_conversion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4986 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59084 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_api_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_base_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8260 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_convert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9323 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_copy_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7858 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_glance_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18116 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_introspect.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7116 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_ovf_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_web_download.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/test_async.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6448 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/test_taskflow_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/async_/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6263 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.958990 glance-28.0.0.0b2/glance/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/common/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/scripts/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/common/scripts/image_import/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/scripts/image_import/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6491 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/scripts/image_import/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/scripts/test_scripts_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2840 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15011 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_format_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8449 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_location_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24239 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_property_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_scripts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8765 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37906 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33403 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/common/test_wsgi_app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/fake_rados.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/image_cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/image_cache/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/image_cache/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/image_cache/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/image_cache/drivers/test_sqlite.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.962991 glance-28.0.0.0b2/glance/tests/unit/keymgr/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/keymgr/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/keymgr/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20879 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4007 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_cache_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18172 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_cache_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17069 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_cached_images.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8667 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_context_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_data_migration_framework.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41436 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24028 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_db_metadef.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24646 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11419 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_domain_proxy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_gateway.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4556 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_glance_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23570 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_glance_replicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10568 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_housekeeping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23350 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_image_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33977 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34473 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18800 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37417 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_scrubber.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48017 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_store_image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3218 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_store_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12410 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.966991 glance-28.0.0.0b2/glance/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_cache_management_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_discovery_image_import.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5599 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_discovery_stores.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_image_actions_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48624 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_image_data_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24562 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_image_members_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_image_tags_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   286556 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_images_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   100689 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_metadef_resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_schemas_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38857 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_tasks_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38246 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/unit/v2/test_v2_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25420 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.966991 glance-28.0.0.0b2/glance/tests/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/ca.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/ca.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/testserver-bad-ovf.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/testserver-no-disk.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/testserver-no-ovf.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   164385 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/testserver-not-tar.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/tests/var/testserver.ova
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/glance/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.906990 glance-28.0.0.0b2/glance.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3272 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    39567 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2024-01-12 15:30:31.000000 glance-28.0.0.0b2/glance.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.966991 glance-28.0.0.0b2/httpd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/httpd/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/httpd/glance-api-uwsgi.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/httpd/uwsgi-glance-api.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.966991 glance-28.0.0.0b2/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/playbooks/enable-fips.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/playbooks/post-check-metadata-injection.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.970991 glance-28.0.0.0b2/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/rally-jobs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.970991 glance-28.0.0.0b2/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/rally-jobs/extra/fake.img
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/rally-jobs/glance.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.970991 glance-28.0.0.0b2/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/rally-jobs/plugins/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.990991 glance-28.0.0.0b2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/Prevent-removing-last-image-location-d5ee3e00efe14f34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-all-visibility-image-filter-ea2f3948ff778fe3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-cli-and-cache-opts-902f28d65c8fb827.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-cpu-thread-pinning-metadata-09b1866b875c4647.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-description-common-image-property-95ab1139d41579d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-glance-download-method-be6d9e927b8b0a43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-ploop-format-fdd583849504ab15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-processlimits-to-qemu-img-c215f5d90f741d8a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add-vhdx-format-2be99354ad320cca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add_capability_to_purge_all_deleted_rows-7b3b9b767669b1a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/added-quota-usage-api-f1914054132f2021.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/added-store-detail-api-215810aa85dfbb99.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bobcat-milestone-1-releasenotes-2d109105530877d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bobcat-milestone-2-releasenotes-085084b03f66d671.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bp-mitigate-ossn-0075-c0e74e60d86d8ea2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bp-upgrade-checks-b3272c3ddb4e8cf7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bp-virtio-packed-ring-configuration-support-0cd0333c1c52c02b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1593177-8ef35458d29ec93c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1861334-ebc2026b85675d47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1881958-d0e16538f3c0ffaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1979699-70182ec2aead0383.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/bump-api-2-4-efa266aef0928e04.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/cache-api-b806ccfb8c5d9bb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/clean-up-acceptable-values-store_type_preference-39081e4045894731.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/cleanout_registry_data-api-9d91368aed83497e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/cleanup-enable_v2_api-9b9b467f4ae8c3b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/delete_from_store-a1d9b9bd5cf27546.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-glance-api-opts-23bdbd1ad7625999.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-owner_is_tenant-ec8ea36a3f7e9268.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/deprecate-windows-support-557481e4d45912ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/drop-py-2-7-863871c7bc047146.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/drop-python-3-6-and-3-7-c6f051d5b2b40329.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/drop-sheepdog-b55aae84807d31d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/drop-support-for-sqlalchemy-migrate-4bcbe7b200697586.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/enable-enforce-scope-and-new-defaults-ef543183e6c2eabb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/exp-emc-mig-fix-a7e28d547ac38f9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/expanding-stores-details-d3aa8ebb76ad68d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/fix-md-tag-create-multiple-c04756cf5155983d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/fix_1889640-95d543629d7dadce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/fix_1889676-f8d302fd240c8a57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/fix_httpd_docs-3efff0395f96a94d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/glance-unified-quotas-fba62fabb00379af.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/image-conversion-plugin-5aee45e1a1a5bb2b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/image-not-found-policy-override-removed-52616c483a270bcf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8505 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/image_decompression_plugin-5f085666aae01f29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/immediate-caching-image-e38055575c361d32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/lock_path_config_option-2771feaa649e4563.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/metadef-api-admin-operations-b9a2d863913b0cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2867 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/multihash-081466a98601da20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/no_plugins_for_copy-image-26c0e384a368bf6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/os-glance-injection-disallowed-5dad244dfb071938.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/os-glance-namespace-reserved-1fcb8a5fddca4e0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/pending-delete-rollback-444ff94c0056bbdb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-admin_role-f508754e98331fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-db-downgrade-0d1cc45b97605775.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-owner_is_tenant-b30150def293effc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove-s3-driver-639c60b71761eb6f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove_enable_image_import_option-ec4a859ac9a7ea7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/remove_secure_proxy_ssl_header-2a95ad48ffa471ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/replicator-token-cleanup-4a573c86f1acccc0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/rocky-metadefs-changes-cb00c006ff51b541.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/scrubber-exit-e5d77f6f1a38ffb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/scrubber-refactor-73ddbd61ebbf1e86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/soft_delete-tasks-43ea983695faa565.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/store-weight-3ed3ee612579bc25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/support-cinder-multiple-stores-eb4e6d912d549ee9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/trust-support-registry-cfd17a6a9ab21d70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/update-show_multiple_locations-helptext-7fa692642b6b6d52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/use-cursive-c6b15d94845232da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/ussuri-final-b377a21508ada060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/virtuozzo-hypervisor-fada477b64ae829d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/wallaby-m3-releasenotes-bdc9fe6938aba8cc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/windows-support-f4aae61681dba569.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/xena-m2-releasenotes-e68fd81ece1d514a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.990991 glance-28.0.0.0b2/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.990991 glance-28.0.0.0b2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.990991 glance-28.0.0.0b2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8927 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.990991 glance-28.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   249018 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   123718 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.862990 glance-28.0.0.0b2/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12811 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3094 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-01-12 15:30:31.994991 glance-28.0.0.0b2/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3184 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/tools/test-setup.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4037 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/tools/test_format_inspector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-01-12 15:29:47.000000 glance-28.0.0.0b2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17319 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25864 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   229881 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.922335 glance-28.0.0.0rc1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.934336 glance-28.0.0.0rc1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6702 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/heading-level-guide.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.938336 glance-28.0.0.0rc1/api-ref/source/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/cache-manage-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/cache-manage.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1712 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/discovery-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/discovery.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4662 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-data.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22513 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-images-v2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13388 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-import.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-parameters-descriptions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21246 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2688 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-schemas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9338 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-sharing-v2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/images-tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2776 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-objects.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6374 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-properties.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5884 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8772 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13711 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3729 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-resourcetypes.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/metadefs-schemas.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/api-ref/source/v2/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/cache-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      726 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      893 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-details-deactivate-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-import-c-i-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-import-g-d-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-import-gd-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-import-w-d-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-info-import-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-member-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-member-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-member-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-member-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-member-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-members-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-tasks-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      910 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/image-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2246 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/images-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-request-simple.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1102 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      470 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-response-simple.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1213 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3629 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespaces-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      635 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7469 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-objects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4387 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-properties-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-resource-type-assoc-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-resource-type-assoc-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-resource-type-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-resource-types-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tag-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tag-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tag-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tag-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tags-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tags-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-tags-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-member-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-members-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7811 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11491 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-images-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9122 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-object-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6101 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4593 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2861 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-property-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1458 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2072 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-task-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2455 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-tasks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/stores-list-detail-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/stores-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/task-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/task-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-failure-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-processing-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      714 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-success-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/tasks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/samples/usage-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/stores.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5095 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/tasks-parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/tasks-schemas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/v2/tasks.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/api-ref/source/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3669 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/versions/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/api-ref/source/versions/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4454 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/versions/samples/image-versions-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/api-ref/source/versions/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1292 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/doc/source/_extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3326 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/_extra/.htaccess
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.950336 glance-28.0.0.0rc1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.954336 glance-28.0.0.0rc1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/apache-httpd.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3779 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/authentication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9196 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/cache.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8121 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/controllingservers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/db-sqlalchemy-migrate.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9263 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/db.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/flows.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31580 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/interoperable-image-import.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13329 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/manage-images.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7589 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/multistores.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5366 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/os_hash_algo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/policies.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3824 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/property-protections.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7550 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3479 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/requirements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/rollingupgrades.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7053 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/tasks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16419 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/troubleshooting.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26695 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/useful-image-properties.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/admin/zero-downtime-db-upgrade.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.958336 glance-28.0.0.0rc1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/footer.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/general_options.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glanceapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancecachecleaner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancecachemanage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancecacheprefetcher.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancecachepruner.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancecontrol.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3961 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancemanage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2017 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancereplicator.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5295 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancescrubber.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/glancestatus.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/header.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      734 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/cli/openstack_options.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.958336 glance-28.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62996 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/configuring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/glance_api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/glance_cache.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/glance_manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/glance_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/glance_scrubber.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/configuration/sample-configuration.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.958336 glance-28.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3839 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3275 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/blueprints.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8712 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5869 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/core_reviewer_guidelines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/database_architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13229 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/database_migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/documentation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4965 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/domain_implementation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10110 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/domain_model.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/gerrit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4297 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/glance-groups.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4650 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/minor-code-changes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/refreshing-configs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12244 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/release-cpl.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2487 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/release-notes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5452 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/contributor/releasecycle.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/deprecation-note.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   120177 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.962336 glance-28.0.0.0rc1/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48303 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/architecture.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108006 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/glance_db.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32606 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/glance_layers.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   250651 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/image_status_transition.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28449 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/instance-life-1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    39847 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/instance-life-2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30176 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images/instance-life-3.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.962336 glance-28.0.0.0rc1/doc/source/images_src/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57938 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images_src/architecture.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12358 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images_src/glance_db.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21398 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images_src/glance_layers.graphml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/images_src/image_status_transition.dot
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.966336 glance-28.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/configure-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1491 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/edit-glance-api-conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3378 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/get-started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6686 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/install-debian.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6814 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6675 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/note_configuration_vary_by_distribution.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/register-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4183 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.966336 glance-28.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3511 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/common-image-properties.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6185 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/formats.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34733 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/glanceapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/glanceclient.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19470 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/glancemetadefcatalogapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/identifiers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8930 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/metadefs-concepts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4682 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/os_hash_algo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6281 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/signature.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6027 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/source/user/statuses.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.966336 glance-28.0.0.0rc1/doc/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4624 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/doc/test/redirect-tests.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.970336 glance-28.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   206768 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-api.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    83359 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-cache.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8409 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-image-import.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10197 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-manage.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    87017 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-scrubber.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/glance-swift.conf.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.974336 glance-28.0.0.0rc1/etc/metadefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5190 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/cim-processor-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/cim-resource-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5168 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/cim-storage-allocation-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5239 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/cim-virtual-system-setting-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-aggr-disk-filter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1043 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-aggr-iops-filter.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-aggr-num-instances.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-cpu-mode.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-cpu-pinning.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1145 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-guest-memory-backing.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-guest-shutdown.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9206 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-host-capabilities.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-hypervisor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-instance-data.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7583 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-libvirt-image.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-libvirt.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-quota.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-randomgen.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2004 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vcputopology.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1773 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vmware-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1644 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vmware-quota-flavor.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8441 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vmware.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vtpm-hw.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1071 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-vtpm.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1430 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-watchdog.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/compute-xenapi.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/glance-common-image-props.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1687 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/image-signature-verification.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1314 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/operating-system.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18731 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/software-databases.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5252 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/software-runtimes.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5772 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/software-webservers.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/metadefs/storage-volume-type.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.974336 glance-28.0.0.0rc1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/oslo-config-generator/glance-api.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/oslo-config-generator/glance-cache.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/oslo-config-generator/glance-image-import.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/oslo-config-generator/glance-manage.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/oslo-config-generator/glance-scrubber.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/ovf-metadata.json.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1402 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/property-protections-policies.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/property-protections-roles.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/etc/schema-image.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.978336 glance-28.0.0.0rc1/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.978336 glance-28.0.0.0rc1/glance/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8321 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.978336 glance-28.0.0.0rc1/glance/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5750 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2279 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/gzip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4515 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/middleware/version_negotiation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7339 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5096 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/property_protections.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.978336 glance-28.0.0.0rc1/glance/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v1/router.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.982336 glance-28.0.0.0rc1/glance/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10253 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/cached_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6785 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4763 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/image_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26019 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/image_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19505 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/image_members.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4696 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/image_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    84197 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38032 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/metadef_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18163 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/metadef_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/metadef_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14015 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/metadef_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/metadef_tags.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.982336 glance-28.0.0.0rc1/glance/api/v2/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3021 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1768 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_property_item_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2354 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_property_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1139 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/model/metadef_tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17869 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29774 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3947 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16565 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/v2/tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/api/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.982336 glance-28.0.0.0rc1/glance/async_/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7077 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.986336 glance-28.0.0.0rc1/glance/async_/flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.986336 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7580 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5431 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/base_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5889 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/copy_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4711 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/glance_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3600 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/web_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41972 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/api_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20847 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/base_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5962 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/convert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11075 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/ovf_process.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.986336 glance-28.0.0.0rc1/glance/async_/flows/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1202 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/image_conversion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5747 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/image_decompression.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2975 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/inject_image_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/no_op.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/flows/plugins/plugin_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7319 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/taskflow_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4214 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/async_/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4199 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/cache_cleaner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17776 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2134 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/cache_prefetcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/cache_pruner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13626 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23152 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27596 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/replicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6100 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2924 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12068 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22672 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28834 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3208 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/crypt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14512 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/exception.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    25800 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/format_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/common/location_strategy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5081 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/location_strategy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/location_strategy/location_order.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4668 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/location_strategy/store_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9594 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/property_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/removed_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/common/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/common/scripts/api_image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/api_image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/api_image_import/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.990336 glance-28.0.0.0rc1/glance/common/scripts/image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6684 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/image_import/main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/scripts/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9190 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4854 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2890 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/trust_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26263 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47650 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5736 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/wsgi_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/common/wsme_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.994336 glance-28.0.0.0rc1/glance/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35374 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.994336 glance-28.0.0.0rc1/glance/db/simple/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/simple/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75209 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/simple/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.994336 glance-28.0.0.0rc1/glance/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.994336 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3287 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10416 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9108 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7878 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1557 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/alembic.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.998336 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/2024_1_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2331 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3949 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      993 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/migrate.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.002336 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2024_1_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3306 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2024_1_expand01_add_cache_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1289 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1283 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2217 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5857 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1135 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1222 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      816 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      819 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      920 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      919 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    91819 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19654 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadata.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.002336 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10830 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/property.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3635 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/resource_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8271 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/resource_type_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7716 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/tag.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12016 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7137 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/models_metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/sqlalchemy/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2522 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.002336 glance-28.0.0.0rc1/glance/domain/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23897 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/domain/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20262 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/domain/proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8814 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/gateway.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.002336 glance-28.0.0.0rc1/glance/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4121 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4519 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/housekeeping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/image_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16841 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      733 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/cleaner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4433 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/image_cache/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6566 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13107 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/centralized_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15838 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/sqlite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16698 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/drivers/xattr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3455 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/prefetcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/image_cache/pruner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59075 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/de/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   168210 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/en_GB/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53588 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/es/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    54628 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/fr/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53703 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/it/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.926335 glance-28.0.0.0rc1/glance/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    66528 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/ja/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57013 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/ko_KR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53118 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/pt_BR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65007 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/ru/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44846 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/tr_TR/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49820 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/zh_CN/LC_MESSAGES/glance.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/glance/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.006336 glance-28.0.0.0rc1/glance/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48320 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/locale/zh_TW/LC_MESSAGES/glance.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25816 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32705 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4822 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.010336 glance-28.0.0.0rc1/glance/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5230 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11416 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12900 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4471 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/policies/tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.010336 glance-28.0.0.0rc1/glance/quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14945 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/quota/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6472 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/quota/keystone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8048 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16721 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6310 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/sqlite_migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.010336 glance-28.0.0.0rc1/glance/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.010336 glance-28.0.0.0rc1/glance/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/etc/glance-swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/etc/policy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/etc/property-protections-policies.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1467 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/etc/property-protections.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        3 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/etc/schema-image.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.014336 glance-28.0.0.0rc1/glance/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71085 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.014336 glance-28.0.0.0rc1/glance/tests/functional/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116945 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35782 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/base_metadef.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.014336 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2958 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_2024_1_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1862 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_mitaka01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2752 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_mitaka02.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_contract01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7851 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7706 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_contract01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1799 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_rocky_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1749 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_rocky_expand02.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_train_migrate01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2346 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_wallaby_expand01.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11436 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22429 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/db/test_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/ft_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.014336 glance-28.0.0.0rc1/glance/tests/functional/image_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/image_cache/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.018336 glance-28.0.0.0rc1/glance/tests/functional/image_cache/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/image_cache/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21963 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/image_cache/drivers/test_centralized_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.018336 glance-28.0.0.0rc1/glance/tests/functional/serial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/serial/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16780 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/serial/test_scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2859 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6839 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16319 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_cache_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4522 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_client_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5036 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_client_redirects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_cors_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7257 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_glance_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1689 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_gzip_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_healthcheck_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2790 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5833 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_reload.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_sqlite.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7066 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/test_wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.022336 glance-28.0.0.0rc1/glance/tests/functional/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2481 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/metadef_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14922 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_cache_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8759 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_cache_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6341 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   322076 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40391 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_images_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9095 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_images_import_locking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12996 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_legacy_update_cinder_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9384 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_member_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31238 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_namespace_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18312 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_namespaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12372 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_object_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18925 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16330 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_properties.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12598 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_property_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10282 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11532 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_resourcetypes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14844 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_tag_api_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16400 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2430 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_schemas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_tasks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3995 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/functional/v2/test_tasks_api_policy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.022336 glance-28.0.0.0rc1/glance/tests/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/integration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.022336 glance-28.0.0.0rc1/glance/tests/integration/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/integration/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6182 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/integration/v2/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/integration/v2/test_property_quota_violations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20800 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/integration/v2/test_tasks_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4104 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/stubs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/test_hacking.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.026336 glance-28.0.0.0rc1/glance/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.026336 glance-28.0.0.0rc1/glance/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.026336 glance-28.0.0.0rc1/glance/tests/unit/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6390 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/middleware/test_cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9192 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/test_cmd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6792 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14130 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/api/test_property_protections.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.030336 glance-28.0.0.0rc1/glance/tests/unit/async_/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.034336 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.034336 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15047 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/test_image_conversion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4986 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59084 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_api_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8957 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_base_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8260 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_convert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9323 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_copy_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7858 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_glance_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18116 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4801 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_introspect.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7116 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_ovf_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_web_download.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/test_async.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6456 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/test_taskflow_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2968 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/async_/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6263 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.034336 glance-28.0.0.0rc1/glance/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3054 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/image_import/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/image_import/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6491 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/image_import/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8539 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/scripts/test_scripts_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2840 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4581 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16282 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_format_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8449 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_location_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24239 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_property_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_scripts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8765 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37906 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33955 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10820 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/common/test_wsgi_app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3150 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/fake_rados.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7744 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/image_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/image_cache/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/image_cache/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/image_cache/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/image_cache/drivers/test_sqlite.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.038336 glance-28.0.0.0rc1/glance/tests/unit/keymgr/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/keymgr/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/keymgr/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20879 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4007 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_cache_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18172 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_cache_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17069 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_cached_images.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8667 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6238 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_context_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8656 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_data_migration_framework.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46728 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24028 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_db_metadef.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24646 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11419 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_domain_proxy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_gateway.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4556 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_glance_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23570 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_glance_replicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10568 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_housekeeping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28744 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_image_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33977 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34326 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18800 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38087 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5937 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_scrubber.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7751 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_sqlite_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48017 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_store_image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3218 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_store_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12410 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.042336 glance-28.0.0.0rc1/glance/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6387 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_cache_management_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_discovery_image_import.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5599 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_discovery_stores.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6487 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_actions_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48624 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_data_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24562 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_members_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_tags_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   286594 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_images_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   100689 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_metadef_resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_schemas_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38857 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_tasks_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38246 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/unit/v2/test_v2_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25607 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.042336 glance-28.0.0.0rc1/glance/tests/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/ca.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5518 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/privatekey.key
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/testserver-bad-ovf.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/testserver-no-disk.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10240 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/testserver-no-ovf.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   164385 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/testserver-not-tar.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20480 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/tests/var/testserver.ova
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      731 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/glance/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.978336 glance-28.0.0.0rc1/glance.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3375 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40540 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2147 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      790 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2024-03-14 19:58:41.000000 glance-28.0.0.0rc1/glance.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.042336 glance-28.0.0.0rc1/httpd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/httpd/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/httpd/glance-api-uwsgi.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/httpd/uwsgi-glance-api.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.042336 glance-28.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/playbooks/enable-fips.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/playbooks/post-check-metadata-injection.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.042336 glance-28.0.0.0rc1/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.046336 glance-28.0.0.0rc1/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/rally-jobs/extra/fake.img
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/rally-jobs/glance.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.046336 glance-28.0.0.0rc1/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/rally-jobs/plugins/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.066336 glance-28.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/Prevent-removing-last-image-location-d5ee3e00efe14f34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3197 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      756 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-all-visibility-image-filter-ea2f3948ff778fe3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-cli-and-cache-opts-902f28d65c8fb827.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3422 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-cpu-thread-pinning-metadata-09b1866b875c4647.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-description-common-image-property-95ab1139d41579d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-glance-download-method-be6d9e927b8b0a43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-ploop-format-fdd583849504ab15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      511 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-processlimits-to-qemu-img-c215f5d90f741d8a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add-vhdx-format-2be99354ad320cca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add_capability_to_purge_all_deleted_rows-7b3b9b767669b1a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/added-quota-usage-api-f1914054132f2021.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/added-store-detail-api-215810aa85dfbb99.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1947 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      632 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2905 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bobcat-milestone-1-releasenotes-2d109105530877d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bobcat-milestone-2-releasenotes-085084b03f66d671.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1721 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bp-mitigate-ossn-0075-c0e74e60d86d8ea2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bp-upgrade-checks-b3272c3ddb4e8cf7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bp-virtio-packed-ring-configuration-support-0cd0333c1c52c02b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1593177-8ef35458d29ec93c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      400 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1861334-ebc2026b85675d47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1881958-d0e16538f3c0ffaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1979699-70182ec2aead0383.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      539 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/bump-api-2-4-efa266aef0928e04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/cache-api-b806ccfb8c5d9bb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/caracal-milestone-3-releasenotes-534b1daa3e1f254c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/clean-up-acceptable-values-store_type_preference-39081e4045894731.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/cleanout_registry_data-api-9d91368aed83497e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/cleanup-enable_v2_api-9b9b467f4ae8c3b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/delete_from_store-a1d9b9bd5cf27546.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2952 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      729 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-glance-api-opts-23bdbd1ad7625999.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-glance-cache-manage-c88f07d33fcc7ca5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-location_strategy-f658e69700204bbf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-owner_is_tenant-ec8ea36a3f7e9268.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-scrubber-862c38e0d65557f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1456 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-sqlite-cache-driver-1f5f67862f56e0ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/deprecate-windows-support-557481e4d45912ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/drop-py-2-7-863871c7bc047146.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-c6f051d5b2b40329.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/drop-sheepdog-b55aae84807d31d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/drop-support-for-sqlalchemy-migrate-4bcbe7b200697586.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/enable-enforce-scope-and-new-defaults-ef543183e6c2eabb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/exp-emc-mig-fix-a7e28d547ac38f9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/expanding-stores-details-d3aa8ebb76ad68d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/fix-md-tag-create-multiple-c04756cf5155983d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/fix_1889640-95d543629d7dadce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/fix_1889676-f8d302fd240c8a57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/fix_httpd_docs-3efff0395f96a94d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/glance-unified-quotas-fba62fabb00379af.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2209 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/image-conversion-plugin-5aee45e1a1a5bb2b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      469 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/image-not-found-policy-override-removed-52616c483a270bcf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8505 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/image_decompression_plugin-5f085666aae01f29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/immediate-caching-image-e38055575c361d32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/lock_path_config_option-2771feaa649e4563.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      730 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/metadef-api-admin-operations-b9a2d863913b0cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2867 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/multihash-081466a98601da20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      871 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/no_plugins_for_copy-image-26c0e384a368bf6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/os-glance-injection-disallowed-5dad244dfb071938.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/os-glance-namespace-reserved-1fcb8a5fddca4e0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/pending-delete-rollback-444ff94c0056bbdb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      586 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-admin_role-f508754e98331fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-db-downgrade-0d1cc45b97605775.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      711 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-owner_is_tenant-b30150def293effc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove-s3-driver-639c60b71761eb6f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove_enable_image_import_option-ec4a859ac9a7ea7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      796 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/remove_secure_proxy_ssl_header-2a95ad48ffa471ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/replicator-token-cleanup-4a573c86f1acccc0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      478 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/rocky-metadefs-changes-cb00c006ff51b541.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/scrubber-exit-e5d77f6f1a38ffb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/scrubber-refactor-73ddbd61ebbf1e86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/soft_delete-tasks-43ea983695faa565.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/store-weight-3ed3ee612579bc25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/support-cinder-multiple-stores-eb4e6d912d549ee9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/trust-support-registry-cfd17a6a9ab21d70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/update-show_multiple_locations-helptext-7fa692642b6b6d52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/use-cursive-c6b15d94845232da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1315 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/ussuri-final-b377a21508ada060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1657 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1033 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/virtuozzo-hypervisor-fada477b64ae829d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/wallaby-m3-releasenotes-bdc9fe6938aba8cc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/windows-support-f4aae61681dba569.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2369 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/xena-m2-releasenotes-e68fd81ece1d514a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      845 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      755 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8927 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.934336 glance-28.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   249018 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.930335 glance-28.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   123718 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:41.934336 glance-28.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12811 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1412 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3174 2024-03-14 19:58:42.074336 glance-28.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      839 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 19:58:42.070336 glance-28.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3184 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/tools/test-setup.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4037 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/tools/test_format_inspector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5663 2024-03-14 19:57:46.000000 glance-28.0.0.0rc1/tox.ini
```

### Comparing `glance-28.0.0.0b2/.mailmap` & `glance-28.0.0.0rc1/.mailmap`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/.zuul.yaml` & `glance-28.0.0.0rc1/.zuul.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -250,14 +250,55 @@
               output_format: raw
         test-config:
           "$TEMPEST_CONFIG":
             image:
               image_caching_enabled: True
 
 - job:
+    name: glance-centralized-cache
+    parent: tempest-integrated-storage-import
+    description: |
+      The regular job to test with glance centralized cache driver
+    vars:
+      devstack_local_conf:
+        post-config:
+          $GLANCE_API_CONF:
+            DEFAULT:
+              image_cache_driver: "centralized_db"
+
+- job:
+    name: glance-grenade-centralized-cache
+    parent: grenade-multinode
+    description: |
+      Glance grenade multinode job where old glance will use
+      sqlite as cache driver and new glance will use centralized_db
+      as cache driver.
+    required-projects:
+      - opendev.org/openstack/grenade
+      - opendev.org/openstack/glance
+    vars:
+      # NOTE(abhishekk): We always want base devstack to install from
+      # stable/2023.2 where 'sqlite' is default cache driver, so that
+      # on upgrade we can verify that cache data is transferred from
+      # sqlite to central database. We will remove this job in 'E'
+      # cycle when 'sqlite' cache driver is removed from the glance.
+      grenade_from_branch: stable/2023.2
+      grenade_devstack_localrc:
+        shared:
+          GLANCE_STANDALONE: False
+          GLANCE_USE_IMPORT_WORKFLOW: True
+      devstack_local_conf:
+        test-config:
+          "$TEMPEST_CONFIG":
+            image:
+              image_caching_enabled: True
+      tox_envlist: all
+      tempest_test_regex: tempest.api.image.v2.admin.test_image_caching
+
+- job:
     name: glance-multistore-cinder-import
     parent: tempest-integrated-storage-import
     description: |
       The regular import workflow job to test with multiple cinder stores
     timeout: 10800
     vars:
       devstack_localrc:
@@ -341,15 +382,16 @@
       - openstack-python3-jobs
       - openstack-python3-jobs-arm64
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
-        - openstack-tox-functional-py38-fips
+        - openstack-tox-functional-py38-fips:
+            voting: false
         - openstack-tox-functional-py39
         - openstack-tox-functional-py310
         - glance-tox-functional-py39-rbac-defaults
         - glance-tox-functional-py39-sqlalchemy-tips
         - glance-ceph-thin-provisioning:
             voting: false
             irrelevant-files: &tempest-irrelevant-files
@@ -375,14 +417,20 @@
             irrelevant-files: *tempest-irrelevant-files
         - grenade:
             irrelevant-files: *tempest-irrelevant-files
         - tempest-ipv6-only:
             irrelevant-files: *tempest-irrelevant-files
         - nova-ceph-multistore:
             irrelevant-files: *tempest-irrelevant-files
+        - glance-centralized-cache:
+            voting: false
+            irrelevant-files: *tempest-irrelevant-files
+        - glance-grenade-centralized-cache:
+            voting: false
+            irrelevant-files: *tempest-irrelevant-files
         - glance-secure-rbac-protection-functional
 
     gate:
       jobs:
         - openstack-tox-functional-py39
         - openstack-tox-functional-py310
         - tempest-integrated-storage:
```

### Comparing `glance-28.0.0.0b2/AUTHORS` & `glance-28.0.0.0rc1/AUTHORS`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
 Eric Windisch <eric@cloudscaling.com>
 Erik Olof Gunnar Andersson <eandersson@blizzard.com>
 Erno Kuvaja <jokke@hp.com>
 Erno Kuvaja <jokke@usr.fi>
 Ethan Myers <ethan@ethanmye.rs>
 Eugeniya Kudryashova <ekudryashova@mirantis.com>
 Ewan Mellor <ewan.mellor@citrix.com>
+Fabian Wiesel <fabian.wiesel@sap.com>
 Fabio M. Di Nitto <fdinitto@redhat.com>
 Fei Long Wang <flwang@catalyst.net.nz>
 Fei Long Wang <flwang@cn.ibm.com>
 Fengqian Gao <fengqian.gao@intel.com>
 Flaper Fesp <flaper87@gmail.com>
 Flavio Percoco <flaper87@gmail.com>
 Florent Flament <florent.flament-ext@cloudwatt.com>
@@ -335,14 +336,15 @@
 Maurice Leeflang <maurice@leeflang.net>
 Mauro S. M. Rodrigues <maurosr@linux.vnet.ibm.com>
 Maxim Nestratov <mnestratov@virtuozzo.com>
 Mehdi Abaakouk <sileht@redhat.com>
 Michael J Fork <mjfork@us.ibm.com>
 Michael Krotscheck <krotscheck@gmail.com>
 Michael Still <mikal@stillhq.com>
+Michal Arbet <michal.arbet@ultimum.io>
 Michal Dulko <michal.dulko@intel.com>
 Mike Abrams <mabrams@redhat.com>
 Mike Bayer <mike_mp@zzzcomputing.com>
 Mike Fedosin <mfedosin@mirantis.com>
 Mike Fedosin <mikhail.fedosin.ext@nokia.com>
 Mike Lundy <mike@pistoncloud.com>
 Mike Turvey <michael.w.turvey@intel.com>
```

### Comparing `glance-28.0.0.0b2/CONTRIBUTING.rst` & `glance-28.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/ChangeLog` & `glance-28.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,46 @@
 CHANGES
 =======
 
+28.0.0.0rc1
+-----------
+
+* Fix glance-api if cache is disabled
+* Refresh Glance example configs for caracal m3
+* Release notes for Caracal Milestone 3
+* New grenade job to upgrding cache driver
+* Require more specific exception
+* Make \`centralized\_db\` cache driver default
+* Use centralized\_db cache driver in tempest jobs
+* Set a lock\_path for tests
+* Fix flaky test related to cache migration
+* [docs] Configure centralized\_db cache driver
+* Prepare for castellan 4.4.0
+* Migrate from SQLite to Centralized db
+* [minor] Fix doc string for class
+* Deprecate glance scrubber
+* Make openstack-tox-functional-py38-fips job non-voting
+* Move sqlite code in common module
+* Read global config file for cache utilities
+* Introduce centralized database driver for image cache
+* Deprecate the "location\_strategy" option
+* Add required database API(s) for cache
+* inject\_image\_metadata plugin: Fix documentation
+* reno: Update master for yoga Unmaintained status
+* Add new tables for cache operations
+* Support Stream Optimized VMDKs
+* Drop ineffective options from config file
+* Replace CRLF by LF
+* Bump hacking
+* Replace usage of deprecated [DATABASE] sql\_connection
+* Deprecate the "glance-cache-manage" command
+* Deprecate sqlite cache driver
+* Fix test failures with oslo.limit 2.3.0
+* Update python classifier in setup.cfg
+
 28.0.0.0b2
 ----------
 
 * Add Packed Virtqueue extra spec and image properties
 * Increase timeout for glance cinder multistore job
 * Deprecate Windows OS support
 * Revert "Make glance-tox-functional-py39-sqlalchemy-tips job non-voting"
```

### Comparing `glance-28.0.0.0b2/HACKING.rst` & `glance-28.0.0.0rc1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/LICENSE` & `glance-28.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/PKG-INFO` & `glance-28.0.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: glance
-Version: 28.0.0.0b2
+Version: 28.0.0.0rc1
 Summary: OpenStack Image Service
 Home-page: https://docs.openstack.org/glance/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         OpenStack Glance
@@ -80,8 +80,10 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `glance-28.0.0.0b2/README.rst` & `glance-28.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/conf.py` & `glance-28.0.0.0rc1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/heading-level-guide.txt` & `glance-28.0.0.0rc1/api-ref/source/heading-level-guide.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/index.rst` & `glance-28.0.0.0rc1/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/cache-manage-parameters.yaml` & `glance-28.0.0.0rc1/api-ref/source/v2/cache-manage-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/cache-manage.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/cache-manage.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/discovery-parameters.yaml` & `glance-28.0.0.0rc1/api-ref/source/v2/discovery-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/discovery.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/discovery.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-data.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-data.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-images-v2.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-images-v2.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-import.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-import.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-parameters-descriptions.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-parameters-descriptions.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-parameters.yaml` & `glance-28.0.0.0rc1/api-ref/source/v2/images-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-schemas.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-sharing-v2.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-sharing-v2.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/images-tags.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/images-tags.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/index.rst` & `glance-28.0.0.0rc1/api-ref/source/v2/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-index.rst` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-objects.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-objects.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-properties.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-properties.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces-tags.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces-tags.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-namespaces.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-namespaces.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-parameters.yaml` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-resourcetypes.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-resourcetypes.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/metadefs-schemas.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/metadefs-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-create-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-details-deactivate-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-details-deactivate-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-members-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-members-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-tasks-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-tasks-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/image-update-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/image-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/images-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/images-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-request.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-create-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-details-with-rt-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespace-update-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespace-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-namespaces-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-namespaces-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-request.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-create-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-details-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-request.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-update-request.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-object-update-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-object-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-objects-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-objects-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-properties-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-properties-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-request.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-create-request.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-create-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-details-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-details-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-request.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-update-request.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-property-update-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-property-update-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/metadef-resource-types-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/metadef-resource-types-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-member-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-member-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-members-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-members-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-image-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-image-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-images-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-images-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-namespace-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-namespaces-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-object-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-object-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-objects-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-properties-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-property-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-property-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-resource-type-association-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-resource-type-associations-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-tag-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-metadef-tags-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-task-show-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-task-show-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/schemas-tasks-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/schemas-tasks-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/stores-list-detail-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/stores-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/stores-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/stores-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/task-create-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/task-create-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-failure-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-failure-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-processing-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-processing-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/task-show-success-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/task-show-success-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/samples/tasks-list-response.json` & `glance-28.0.0.0rc1/api-ref/source/v2/samples/tasks-list-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/stores.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/stores.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/tasks-parameters.yaml` & `glance-28.0.0.0rc1/api-ref/source/v2/tasks-parameters.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/tasks-schemas.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/tasks-schemas.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/v2/tasks.inc` & `glance-28.0.0.0rc1/api-ref/source/v2/tasks.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/versions/index.rst` & `glance-28.0.0.0rc1/api-ref/source/versions/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/versions/samples/image-versions-response.json` & `glance-28.0.0.0rc1/api-ref/source/versions/samples/image-versions-response.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/api-ref/source/versions/versions.inc` & `glance-28.0.0.0rc1/api-ref/source/versions/versions.inc`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/bindep.txt` & `glance-28.0.0.0rc1/bindep.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/_extra/.htaccess` & `glance-28.0.0.0rc1/doc/source/_extra/.htaccess`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/apache-httpd.rst` & `glance-28.0.0.0rc1/doc/source/admin/apache-httpd.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/authentication.rst` & `glance-28.0.0.0rc1/doc/source/admin/authentication.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/cache.rst` & `glance-28.0.0.0rc1/doc/source/admin/cache.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/controllingservers.rst` & `glance-28.0.0.0rc1/doc/source/admin/controllingservers.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/db-sqlalchemy-migrate.rst` & `glance-28.0.0.0rc1/doc/source/admin/db-sqlalchemy-migrate.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/db.rst` & `glance-28.0.0.0rc1/doc/source/admin/db.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/flows.rst` & `glance-28.0.0.0rc1/doc/source/admin/flows.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/interoperable-image-import.rst` & `glance-28.0.0.0rc1/doc/source/admin/interoperable-image-import.rst`

 * *Files 1% similar despite different names*

```diff
@@ -553,15 +553,15 @@
    .. code-block:: ini
 
        [image_import_opts]
        image_import_plugins = [inject_image_metadata]
 
        [inject_metadata_properties]
        ignore_user_roles = admin,...
-       inject = "property1":"value1","property2":"value2",...
+       inject = property1:value1,property2:value2,...
 
    The first section, ``image_import_opts``, is used to enable the plugin by
    specifying the plugin name as one of the elements of the list that is the
    value of the `image_import_plugins` parameter.  The plugin name is simply
    the module name under glance/async\_/flows/plugins/
 
    The second section, ``inject_metadata_properties``, is where you set the
@@ -572,16 +572,15 @@
    * ``ignore_user_roles`` is a comma-separated list of Keystone roles that the
      plugin will ignore.  In other words, if the user making the image import
      call has any of these roles, the plugin will not inject any properties
      into the image.
 
    * ``inject`` is a comma-separated list of properties and values that will be
      injected into the image record for the imported image.  Each property and
-     value should be quoted and separated by a colon (':') as shown in the
-     example above.
+     value should be separated by a colon (':') as shown in the example above.
 
 2. If your use case is such that you don't want to allow end-users to create,
    modify, or delete metadata properties that you are injecting during the
    interoperable image import process, you will need to protect these
    properties using the Glance property protection feature (available since
    the Havana release).
```

### Comparing `glance-28.0.0.0b2/doc/source/admin/manage-images.rst` & `glance-28.0.0.0rc1/doc/source/admin/manage-images.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/multistores.rst` & `glance-28.0.0.0rc1/doc/source/admin/multistores.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/notifications.rst` & `glance-28.0.0.0rc1/doc/source/admin/notifications.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/os_hash_algo.rst` & `glance-28.0.0.0rc1/doc/source/admin/os_hash_algo.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/policies.rst` & `glance-28.0.0.0rc1/doc/source/admin/policies.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/property-protections.rst` & `glance-28.0.0.0rc1/doc/source/admin/property-protections.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/quotas.rst` & `glance-28.0.0.0rc1/doc/source/admin/quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/requirements.rst` & `glance-28.0.0.0rc1/doc/source/admin/requirements.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/rollingupgrades.rst` & `glance-28.0.0.0rc1/doc/source/admin/rollingupgrades.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/tasks.rst` & `glance-28.0.0.0rc1/doc/source/admin/tasks.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/troubleshooting.rst` & `glance-28.0.0.0rc1/doc/source/admin/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/useful-image-properties.rst` & `glance-28.0.0.0rc1/doc/source/admin/useful-image-properties.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/admin/zero-downtime-db-upgrade.rst` & `glance-28.0.0.0rc1/doc/source/admin/zero-downtime-db-upgrade.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/general_options.txt` & `glance-28.0.0.0rc1/doc/source/cli/general_options.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancecachecleaner.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancecachecleaner.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancecachemanage.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancecachemanage.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancecacheprefetcher.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancecacheprefetcher.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancecachepruner.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancecachepruner.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancecontrol.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancecontrol.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancemanage.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancemanage.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancereplicator.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancereplicator.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancescrubber.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancescrubber.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/glancestatus.rst` & `glance-28.0.0.0rc1/doc/source/cli/glancestatus.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/cli/openstack_options.txt` & `glance-28.0.0.0rc1/doc/source/cli/openstack_options.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/conf.py` & `glance-28.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/configuration/configuring.rst` & `glance-28.0.0.0rc1/doc/source/configuration/configuring.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1485,23 +1485,37 @@
   Default: ``/var/lib/glance/image-cache``
 
   This is the base directory the image cache can write files to.
   Make sure the directory is writable by the user running the
   ``glance-api`` server
 
 ``image_cache_driver=DRIVER``
-  Optional. Choice of ``sqlite`` or ``xattr``
+  Optional. Choice of ``sqlite``, ``xattr`` or ``centralized_db``
 
-  Default: ``sqlite``
+  Default: ``centralized_db``
 
-  The default ``sqlite`` cache driver has no special dependencies, other
+  The default ``centralized_db`` cache driver has no special
+  dependencies, other than ``worker_self_reference_url`` which needs
+  to be configured to store the reference of node in the database.
+  Earlier cache database used to be independent for each glance api
+  service, now with ``centralized_db`` cache driver it stores
+  information about the cached files at one place which is in
+  a central database. Old records from SQLite database will
+  be :ref:`migrated <sqlite-to-centralized_db-migration>` to
+  central database on service restart during upgrade process.
+
+  The ``sqlite`` cache driver has no special dependencies, other
   than the ``python-sqlite3`` library, which is installed on virtually
   all operating systems with modern versions of Python. It stores
   information about the cached files in a SQLite database.
 
+  **NOTE**
+  In Caracal release ``sqlite`` cache driver has been deprecated and will
+  be removed in ``F`` development cycle.
+
   The ``xattr`` cache driver required the ``python-xattr>=0.6.0`` library
   and requires that the filesystem containing ``image_cache_dir`` have
   access times tracked for all files (in other words, the noatime option
   CANNOT be set for that filesystem). In addition, ``user_xattr`` must be
   set on the filesystem's description line in fstab. Because of these
   requirements, the ``xattr`` cache driver is not available on Windows.
 
@@ -1510,27 +1524,51 @@
 
   Default: ``cache.db``
 
   When using the ``sqlite`` cache driver, you can set the name of the database
   that will be used to store the cached images information. The database
   is always contained in the ``image_cache_dir``.
 
+  **NOTE**
+  In Caracal release ``image_cache_sqlite_db`` option has been deprecated
+  and will be removed in ``F`` development cycle.
+
 ``image_cache_max_size=SIZE``
   Optional.
 
   Default: ``10737418240`` (10 GB)
 
   Size, in bytes, that the image cache should be constrained to. Images files
   are cached automatically in the local image cache, even if the writing of
   that image file would put the total cache size over this size. The
   ``glance-cache-pruner`` executable is what prunes the image cache to be equal
   to or less than this value. The ``glance-cache-pruner`` executable is
   designed to be run via cron on a regular basis. See more about this
   executable in :ref:`Controlling the Growth of the Image Cache <image-cache>`
 
+
+.. _sqlite-to-centralized_db-migration:
+
+Migrating records from SQLite to Central database
+-------------------------------------------------
+
+In case of upgrades/updates we need to deal with migrating existing records
+from SQLite database to central database. This operation will be performed
+one time during service startup. If SQLite database file, configured using
+``image_cache_sqlite_db`` configuration option (default ``cache.db``) is
+present at service start and ``image_cache_driver`` is not set to
+``centralized_db`` then we will read records from SQLite database and
+insert those in newly created ``cached_images`` table in central database.
+Once all records are migrated we will clear the SQLite database table
+and keep the SQLite database file as it is (to be deleted by
+administrator/operator later if required). Important point here is once
+deployer chooses to use ``centralized_db`` and we migrate their records out
+of SQLite database to central database, then we will not migrate them back
+if deployer wants to revert back to ``sqlite`` driver.
+
 Configuring Notifications
 -------------------------
 
 Glance can optionally generate notifications to be logged or sent to a message
 queue. The configuration options are specified in the ``glance-api.conf``
 configuration file.
```

### Comparing `glance-28.0.0.0b2/doc/source/configuration/sample-configuration.rst` & `glance-28.0.0.0rc1/doc/source/configuration/sample-configuration.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/architecture.rst` & `glance-28.0.0.0rc1/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/blueprints.rst` & `glance-28.0.0.0rc1/doc/source/contributor/blueprints.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/contributing.rst` & `glance-28.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/core_reviewer_guidelines.rst` & `glance-28.0.0.0rc1/doc/source/contributor/core_reviewer_guidelines.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/database_architecture.rst` & `glance-28.0.0.0rc1/doc/source/contributor/database_architecture.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/database_migrations.rst` & `glance-28.0.0.0rc1/doc/source/contributor/database_migrations.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/documentation.rst` & `glance-28.0.0.0rc1/doc/source/contributor/documentation.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/domain_implementation.rst` & `glance-28.0.0.0rc1/doc/source/contributor/domain_implementation.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/domain_model.rst` & `glance-28.0.0.0rc1/doc/source/contributor/domain_model.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/gerrit.rst` & `glance-28.0.0.0rc1/doc/source/contributor/gerrit.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/glance-groups.rst` & `glance-28.0.0.0rc1/doc/source/contributor/glance-groups.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/index.rst` & `glance-28.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/minor-code-changes.rst` & `glance-28.0.0.0rc1/doc/source/contributor/minor-code-changes.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/refreshing-configs.rst` & `glance-28.0.0.0rc1/doc/source/contributor/refreshing-configs.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/release-cpl.rst` & `glance-28.0.0.0rc1/doc/source/contributor/release-cpl.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/release-notes.rst` & `glance-28.0.0.0rc1/doc/source/contributor/release-notes.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/contributor/releasecycle.rst` & `glance-28.0.0.0rc1/doc/source/contributor/releasecycle.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/glossary.rst` & `glance-28.0.0.0rc1/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/architecture.png` & `glance-28.0.0.0rc1/doc/source/images/architecture.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/glance_db.png` & `glance-28.0.0.0rc1/doc/source/images/glance_db.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/glance_layers.png` & `glance-28.0.0.0rc1/doc/source/images/glance_layers.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/image_status_transition.png` & `glance-28.0.0.0rc1/doc/source/images/image_status_transition.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/instance-life-1.png` & `glance-28.0.0.0rc1/doc/source/images/instance-life-1.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/instance-life-2.png` & `glance-28.0.0.0rc1/doc/source/images/instance-life-2.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images/instance-life-3.png` & `glance-28.0.0.0rc1/doc/source/images/instance-life-3.png`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images_src/architecture.graphml` & `glance-28.0.0.0rc1/doc/source/images_src/architecture.graphml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images_src/glance_db.graphml` & `glance-28.0.0.0rc1/doc/source/images_src/glance_db.graphml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images_src/glance_layers.graphml` & `glance-28.0.0.0rc1/doc/source/images_src/glance_layers.graphml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/images_src/image_status_transition.dot` & `glance-28.0.0.0rc1/doc/source/images_src/image_status_transition.dot`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/index.rst` & `glance-28.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/configure-quotas.rst` & `glance-28.0.0.0rc1/doc/source/install/configure-quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/edit-glance-api-conf.rst` & `glance-28.0.0.0rc1/doc/source/install/edit-glance-api-conf.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/get-started.rst` & `glance-28.0.0.0rc1/doc/source/install/get-started.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/index.rst` & `glance-28.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/install-debian.rst` & `glance-28.0.0.0rc1/doc/source/install/install-debian.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/install-obs.rst` & `glance-28.0.0.0rc1/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/install-rdo.rst` & `glance-28.0.0.0rc1/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/install-ubuntu.rst` & `glance-28.0.0.0rc1/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/register-quotas.rst` & `glance-28.0.0.0rc1/doc/source/install/register-quotas.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/install/verify.rst` & `glance-28.0.0.0rc1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/common-image-properties.rst` & `glance-28.0.0.0rc1/doc/source/user/common-image-properties.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/formats.rst` & `glance-28.0.0.0rc1/doc/source/user/formats.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/glanceapi.rst` & `glance-28.0.0.0rc1/doc/source/user/glanceapi.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/glanceclient.rst` & `glance-28.0.0.0rc1/doc/source/user/glanceclient.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/glancemetadefcatalogapi.rst` & `glance-28.0.0.0rc1/doc/source/user/glancemetadefcatalogapi.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/identifiers.rst` & `glance-28.0.0.0rc1/doc/source/user/identifiers.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/metadefs-concepts.rst` & `glance-28.0.0.0rc1/doc/source/user/metadefs-concepts.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/os_hash_algo.rst` & `glance-28.0.0.0rc1/doc/source/user/os_hash_algo.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/signature.rst` & `glance-28.0.0.0rc1/doc/source/user/signature.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/source/user/statuses.rst` & `glance-28.0.0.0rc1/doc/source/user/statuses.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/doc/test/redirect-tests.txt` & `glance-28.0.0.0rc1/doc/test/redirect-tests.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/glance-api-paste.ini` & `glance-28.0.0.0rc1/etc/glance-api-paste.ini`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/glance-api.conf` & `glance-28.0.0.0rc1/etc/glance-api.conf`

 * *Files 0% similar despite different names*

```diff
@@ -504,15 +504,15 @@
 #
 # Related options:
 #     * public_endpoint
 #
 #  (string value)
 #worker_self_reference_url = <None>
 
-#
+# DEPRECATED:
 # Strategy to determine the preference order of image locations.
 #
 # This configuration option indicates the strategy to determine
 # the order in which an image's locations must be accessed to
 # serve the image's data. Glance then retrieves the image data
 # from the first responsive active location it finds in this list.
 #
@@ -531,14 +531,20 @@
 # Related options:
 #     * store_type_preference
 #
 #  (string value)
 # Possible values:
 # location_order - <No description provided>
 # store_type - <No description provided>
+# This option is deprecated for removal since Caracal.
+# Its value may be silently ignored in the future.
+# Reason:
+# In Bobcat, a new weighing mechanism has been introduced, which makes the
+# location strategy obsolete.  This option is scheduled to be removed during the
+# Dalmatian development cycle.
 #location_strategy = location_order
 
 #
 # The location of the property protection file.
 #
 # Provide a valid path to the property protection file which contains
 # the rules for property protections and the roles/policies associated
@@ -774,15 +780,15 @@
 #enabled_backends = <None>
 
 # This argument is used internally on Windows. Glance passes a pipe handle to
 # child processes, which is then used for inter-process communication. (string
 # value)
 #pipe_handle = <None>
 
-#
+# DEPRECATED:
 # The relative path to sqlite file database that will be used for image cache
 # management.
 #
 # This is a relative path to the sqlite file database that tracks the age and
 # usage statistics of image cache. The path is relative to image cache base
 # directory, specified by the configuration option ``image_cache_dir``.
 #
@@ -791,14 +797,20 @@
 # Possible values:
 #     * A valid relative path to sqlite file database
 #
 # Related options:
 #     * ``image_cache_dir``
 #
 #  (string value)
+# This option is deprecated for removal since Caracal (2024.1).
+# Its value may be silently ignored in the future.
+# Reason:
+# As centralized database will now be used for image cache management, the use
+# of `sqlite` database and driver will be dropped from 'E' (2025.1)
+# development cycle.
 #image_cache_sqlite_db = cache.db
 
 #
 # The driver to use for image cache management.
 #
 # This configuration option provides the flexibility to choose between the
 # different image-cache drivers available. An image-cache driver is responsible
@@ -809,32 +821,41 @@
 #
 # The essential functions of a driver are defined in the base class
 # ``glance.image_cache.drivers.base.Driver``. All image-cache drivers (existing
 # and prospective) must implement this interface. Currently available drivers
 # are ``sqlite`` and ``xattr``. These drivers primarily differ in the way they
 # store the information about cached images:
 #
-# * The ``sqlite`` driver uses a sqlite database (which sits on every glance
-#   node locally) to track the usage of cached images.
+# * The ``centralized_db`` driver uses a central database (which will be common
+#   for all glance nodes) to track the usage of cached images.
+# * The ``sqlite`` (deprecated) driver uses a sqlite database (which sits on
+#   every glance node locally) to track the usage of cached images.
 # * The ``xattr`` driver uses the extended attributes of files to store this
 #   information. It also requires a filesystem that sets ``atime`` on the files
 #   when accessed.
 #
+# Deprecation warning:
+#     * As centralized database will now be used for image cache management, the
+#       use of `sqlite` database and driver will be dropped from 'E' (2025.1)
+#       development cycle.
+#
 # Possible values:
+#     * centralized_db
 #     * sqlite
 #     * xattr
 #
 # Related options:
 #     * None
 #
 #  (string value)
 # Possible values:
+# centralized_db - <No description provided>
 # sqlite - <No description provided>
 # xattr - <No description provided>
-#image_cache_driver = sqlite
+#image_cache_driver = centralized_db
 
 #
 # The upper limit on cache size, in bytes, after which the cache-pruner cleans
 # up the image cache.
 #
 # NOTE: This is just a threshold for cache-pruner to act upon. It is NOT a
 # hard limit beyond which the image cache would never grow. In fact, depending
@@ -963,15 +984,15 @@
 #
 # Related options:
 #     * None
 #
 #  (list value)
 #disabled_notifications =
 
-#
+# DEPRECATED:
 # The amount of time, in seconds, to delay image scrubbing.
 #
 # When delayed delete is turned on, an image is put into ``pending_delete``
 # state upon deletion until the scrubber deletes its image data. Typically, soon
 # after the image is put into ``pending_delete`` state, it is available for
 # scrubbing. However, scrubbing can be delayed until a later point using this
 # configuration option. This option denotes the time period an image spends in
@@ -985,17 +1006,21 @@
 #     * Any non-negative integer
 #
 # Related options:
 #     * ``delayed_delete``
 #
 #  (integer value)
 # Minimum value: 0
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #scrub_time = 0
 
-#
+# DEPRECATED:
 # The size of thread pool to be used for scrubbing images.
 #
 # When there are a large number of images to scrub, it is beneficial to scrub
 # images in parallel so that the scrub queue stays in control and the backend
 # storage is reclaimed in a timely fashion. This configuration option denotes
 # the maximum number of images to be scrubbed in parallel. The default value is
 # one, which signifies serial scrubbing. Any value above one indicates parallel
@@ -1005,17 +1030,21 @@
 #     * Any non-zero positive integer
 #
 # Related options:
 #     * ``delayed_delete``
 #
 #  (integer value)
 # Minimum value: 1
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #scrub_pool_size = 1
 
-#
+# DEPRECATED:
 # Turn on/off delayed delete.
 #
 # Typically when an image is deleted, the ``glance-api`` service puts the image
 # into ``deleted`` state and deletes its data at the same time. Delayed delete
 # is a feature in Glance that delays the actual deletion of image data until a
 # later point in time (as determined by the configuration option
 # ``scrub_time``).
@@ -1035,14 +1064,18 @@
 #
 # Related options:
 #     * ``scrub_time``
 #     * ``wakeup_time``
 #     * ``scrub_pool_size``
 #
 #  (boolean value)
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #delayed_delete = false
 
 #
 # From oslo.log
 #
 
 # If set to true, the logging level will be set to DEBUG instead of the default
@@ -1102,15 +1135,18 @@
 # is set. (boolean value)
 #use_json = false
 
 # Log output to standard error. This option is ignored if log_config_append is
 # set. (boolean value)
 #use_stderr = false
 
-# Log output to Windows Event Log. (boolean value)
+# DEPRECATED: Log output to Windows Event Log. (boolean value)
+# This option is deprecated for removal.
+# Its value may be silently ignored in the future.
+# Reason: Windows support is no longer maintained.
 #use_eventlog = false
 
 # The amount of time before the log files are rotated. This option is ignored
 # unless log_rotation_type is set to "interval". (integer value)
 #log_rotate_interval = 1
 
 # Rotation interval type. The time of the last file change (or the time when the
@@ -1759,22 +1795,14 @@
 #mysql_sql_mode = TRADITIONAL
 
 # For Galera only, configure wsrep_sync_wait causality checks on new
 # connections.  Default is None, meaning don't configure any setting. (integer
 # value)
 #mysql_wsrep_sync_wait = <None>
 
-# DEPRECATED: If True, transparently enables support for handling MySQL Cluster
-# (NDB). (boolean value)
-# This option is deprecated for removal since 12.1.0.
-# Its value may be silently ignored in the future.
-# Reason: Support for the MySQL NDB Cluster storage engine has been deprecated
-# and will be removed in a future release.
-#mysql_enable_ndb = false
-
 # Connections which have been present in the connection pool longer than this
 # number of seconds will be replaced with a new one the next time they are
 # checked out from the pool. (integer value)
 #connection_recycle_time = 3600
 
 # Maximum number of SQL connections to keep open in a pool. Setting a value of 0
 # indicates no limit. (integer value)
@@ -2147,39 +2175,32 @@
 #
 # Related options:
 #     * rbd_store_user
 #
 #  (string value)
 #rbd_store_ceph_conf =
 
-# DEPRECATED:
+#
 # Timeout value for connecting to Ceph cluster.
 #
 # This configuration option takes in the timeout value in seconds used
 # when connecting to the Ceph cluster i.e. it sets the time to wait for
 # glance-api before closing the connection. This prevents glance-api
 # hangups during the connection to RBD. If the value for this option
-# is set to less than or equal to 0, no timeout is set and the default
-# librados value is used.
+# is set to less than 0, no timeout is set and the default librados value
+# is used.
 #
 # Possible Values:
 #     * Any integer value
 #
 # Related options:
 #     * None
 #
 #  (integer value)
-# This option is deprecated for removal since Zed.
-# Its value may be silently ignored in the future.
-# Reason:
-# This option has not had any effect in years. Users willing to set a timeout
-# for
-# connecting to the Ceph cluster should use 'client_mount_timeout' in Ceph's
-# configuration file.
-#rados_connect_timeout = 0
+#rados_connect_timeout = -1
 
 #
 # Enable or not thin provisioning in this backend.
 #
 # This configuration option enable the feature of not really write null byte
 # sequences on the RBD backend, the holes who can appear will automatically
 # be interpreted by Ceph as null bytes, and do not really consume your storage.
@@ -3907,39 +3928,32 @@
 #
 # Related options:
 #     * rbd_store_user
 #
 #  (string value)
 #rbd_store_ceph_conf =
 
-# DEPRECATED:
+#
 # Timeout value for connecting to Ceph cluster.
 #
 # This configuration option takes in the timeout value in seconds used
 # when connecting to the Ceph cluster i.e. it sets the time to wait for
 # glance-api before closing the connection. This prevents glance-api
 # hangups during the connection to RBD. If the value for this option
-# is set to less than or equal to 0, no timeout is set and the default
-# librados value is used.
+# is set to less than 0, no timeout is set and the default librados value
+# is used.
 #
 # Possible Values:
 #     * Any integer value
 #
 # Related options:
 #     * None
 #
 #  (integer value)
-# This option is deprecated for removal since Zed.
-# Its value may be silently ignored in the future.
-# Reason:
-# This option has not had any effect in years. Users willing to set a timeout
-# for
-# connecting to the Ceph cluster should use 'client_mount_timeout' in Ceph's
-# configuration file.
-#rados_connect_timeout = 0
+#rados_connect_timeout = -1
 
 #
 # Enable or not thin provisioning in this backend.
 #
 # This configuration option enable the feature of not really write null byte
 # sequences on the RBD backend, the holes who can appear will automatically
 # be interpreted by Ceph as null bytes, and do not really consume your storage.
@@ -4895,14 +4909,22 @@
 # (boolean value)
 #detailed = false
 
 # Additional backends that can perform health checks and report that information
 # back as part of a request. (list value)
 #backends =
 
+# A list of network addresses to limit source ip allowed to access healthcheck
+# information. Any request from ip outside of these network addresses are
+# ignored. (list value)
+#allowed_source_ranges =
+
+# Ignore requests with proxy headers. (boolean value)
+#ignore_proxied_requests = false
+
 # Check the presence of a file to determine if an application is running on a
 # port. Used by DisableByFileHealthcheck plugin. (string value)
 #disable_by_file_path = <None>
 
 # Check the presence of a file based on a port to determine if an application is
 # running on a port. Expects a "port:path" list of strings. Used by
 # DisableByFilesPortsHealthcheck plugin. (list value)
@@ -5336,14 +5358,18 @@
 #status_code_retries = <None>
 
 # Delay (in seconds) between two retries for retriable status codes. If not set,
 # exponential retry starting with 0.5 seconds up to a maximum of 60 seconds is
 # used. (floating point value)
 #status_code_retry_delay = <None>
 
+# List of retriable HTTP status codes that should be retried. If not set default
+# to  [503] (list value)
+#retriable_status_codes = <None>
+
 
 [oslo_messaging_amqp]
 
 #
 # From oslo.messaging
 #
 
@@ -5765,29 +5791,32 @@
 # rabbit_quorum_queue is enabled, Default 0 which means dont set a limit.
 # (integer value)
 # Deprecated group/name - [oslo_messaging_rabbit]/rabbit_quroum_max_memory_bytes
 #rabbit_quorum_max_memory_bytes = 0
 
 # Positive integer representing duration in seconds for queue TTL (x-expires).
 # Queues which are unused for the duration of the TTL are automatically deleted.
-# The parameter affects only reply and fanout queues. (integer value)
-# Minimum value: 1
+# The parameter affects only reply and fanout queues. Setting 0 as value will
+# disable the x-expires. If doing so, make sure you have a rabbitmq policy to
+# delete the queues or you deployment will create an infinite number of queue
+# over time. (integer value)
+# Minimum value: 0
 #rabbit_transient_queues_ttl = 1800
 
 # Specifies the number of messages to prefetch. Setting to zero allows unlimited
 # messages. (integer value)
 #rabbit_qos_prefetch_count = 0
 
 # Number of seconds after which the Rabbit broker is considered down if
 # heartbeat's keep-alive fails (0 disables heartbeat). (integer value)
 #heartbeat_timeout_threshold = 60
 
 # How often times during the heartbeat_timeout_threshold we check the heartbeat.
 # (integer value)
-#heartbeat_rate = 2
+#heartbeat_rate = 3
 
 # DEPRECATED: (DEPRECATED) Enable/Disable the RabbitMQ mandatory flag for direct
 # send. The direct send is used as reply, so the MessageUndeliverable exception
 # is raised in case the client queue does not exist.MessageUndeliverable
 # exception will be used to loop for a timeout to lets a chance to sender to
 # recover.This flag is deprecated and it will not be possible to deactivate this
 # functionality anymore (boolean value)
@@ -6089,15 +6118,15 @@
 
 [store_type_location_strategy]
 
 #
 # From glance.api
 #
 
-#
+# DEPRECATED:
 # Preference order of storage backends.
 #
 # Provide a comma separated list of store names in the order in
 # which images should be retrieved from storage backends.
 # These store names must be registered with the ``stores``
 # configuration option.
 #
@@ -6117,14 +6146,20 @@
 #         * vmware
 #
 # Related options:
 #     * location_strategy
 #     * stores
 #
 #  (list value)
+# This option is deprecated for removal since Caracal.
+# Its value may be silently ignored in the future.
+# Reason:
+# In Bobcat, a new weighing mechanism has been introduced, which makes the
+# location strategy obsolete.  This option is scheduled to be removed during the
+# Dalmatian development cycle.
 #store_type_preference =
 
 
 [task]
 
 #
 # From glance.api
@@ -6296,14 +6331,17 @@
 
 # AppRole secret_id for authentication with vault (string value)
 #approle_secret_id = <None>
 
 # Mountpoint of KV store in Vault to use, for example: secret (string value)
 #kv_mountpoint = secret
 
+# Path relative to root of KV store in Vault to use. (string value)
+#kv_path = <None>
+
 # Version of KV store in Vault to use, for example: 2 (integer value)
 #kv_version = 2
 
 # Use this endpoint to connect to Vault, for example: "http://127.0.0.1:8200"
 # (string value)
 #vault_url = http://127.0.0.1:8200
```

### Comparing `glance-28.0.0.0b2/etc/glance-cache.conf` & `glance-28.0.0.0rc1/etc/glance-cache.conf`

 * *Files 1% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 #
 # Related options:
 #     * public_endpoint
 #
 #  (string value)
 #worker_self_reference_url = <None>
 
-#
+# DEPRECATED:
 # The relative path to sqlite file database that will be used for image cache
 # management.
 #
 # This is a relative path to the sqlite file database that tracks the age and
 # usage statistics of image cache. The path is relative to image cache base
 # directory, specified by the configuration option ``image_cache_dir``.
 #
@@ -463,14 +463,20 @@
 # Possible values:
 #     * A valid relative path to sqlite file database
 #
 # Related options:
 #     * ``image_cache_dir``
 #
 #  (string value)
+# This option is deprecated for removal since Caracal (2024.1).
+# Its value may be silently ignored in the future.
+# Reason:
+# As centralized database will now be used for image cache management, the use
+# of `sqlite` database and driver will be dropped from 'E' (2025.1)
+# development cycle.
 #image_cache_sqlite_db = cache.db
 
 #
 # The driver to use for image cache management.
 #
 # This configuration option provides the flexibility to choose between the
 # different image-cache drivers available. An image-cache driver is responsible
@@ -481,32 +487,41 @@
 #
 # The essential functions of a driver are defined in the base class
 # ``glance.image_cache.drivers.base.Driver``. All image-cache drivers (existing
 # and prospective) must implement this interface. Currently available drivers
 # are ``sqlite`` and ``xattr``. These drivers primarily differ in the way they
 # store the information about cached images:
 #
-# * The ``sqlite`` driver uses a sqlite database (which sits on every glance
-#   node locally) to track the usage of cached images.
+# * The ``centralized_db`` driver uses a central database (which will be common
+#   for all glance nodes) to track the usage of cached images.
+# * The ``sqlite`` (deprecated) driver uses a sqlite database (which sits on
+#   every glance node locally) to track the usage of cached images.
 # * The ``xattr`` driver uses the extended attributes of files to store this
 #   information. It also requires a filesystem that sets ``atime`` on the files
 #   when accessed.
 #
+# Deprecation warning:
+#     * As centralized database will now be used for image cache management, the
+#       use of `sqlite` database and driver will be dropped from 'E' (2025.1)
+#       development cycle.
+#
 # Possible values:
+#     * centralized_db
 #     * sqlite
 #     * xattr
 #
 # Related options:
 #     * None
 #
 #  (string value)
 # Possible values:
+# centralized_db - <No description provided>
 # sqlite - <No description provided>
 # xattr - <No description provided>
-#image_cache_driver = sqlite
+#image_cache_driver = centralized_db
 
 #
 # The upper limit on cache size, in bytes, after which the cache-pruner cleans
 # up the image cache.
 #
 # NOTE: This is just a threshold for cache-pruner to act upon. It is NOT a
 # hard limit beyond which the image cache would never grow. In fact, depending
@@ -651,15 +666,18 @@
 # is set. (boolean value)
 #use_json = false
 
 # Log output to standard error. This option is ignored if log_config_append is
 # set. (boolean value)
 #use_stderr = false
 
-# Log output to Windows Event Log. (boolean value)
+# DEPRECATED: Log output to Windows Event Log. (boolean value)
+# This option is deprecated for removal.
+# Its value may be silently ignored in the future.
+# Reason: Windows support is no longer maintained.
 #use_eventlog = false
 
 # The amount of time before the log files are rotated. This option is ignored
 # unless log_rotation_type is set to "interval". (integer value)
 #log_rotate_interval = 1
 
 # Rotation interval type. The time of the last file change (or the time when the
@@ -1482,39 +1500,32 @@
 #
 # Related options:
 #     * rbd_store_user
 #
 #  (string value)
 #rbd_store_ceph_conf =
 
-# DEPRECATED:
+#
 # Timeout value for connecting to Ceph cluster.
 #
 # This configuration option takes in the timeout value in seconds used
 # when connecting to the Ceph cluster i.e. it sets the time to wait for
 # glance-api before closing the connection. This prevents glance-api
 # hangups during the connection to RBD. If the value for this option
-# is set to less than or equal to 0, no timeout is set and the default
-# librados value is used.
+# is set to less than 0, no timeout is set and the default librados value
+# is used.
 #
 # Possible Values:
 #     * Any integer value
 #
 # Related options:
 #     * None
 #
 #  (integer value)
-# This option is deprecated for removal since Zed.
-# Its value may be silently ignored in the future.
-# Reason:
-# This option has not had any effect in years. Users willing to set a timeout
-# for
-# connecting to the Ceph cluster should use 'client_mount_timeout' in Ceph's
-# configuration file.
-#rados_connect_timeout = 0
+#rados_connect_timeout = -1
 
 #
 # Enable or not thin provisioning in this backend.
 #
 # This configuration option enable the feature of not really write null byte
 # sequences on the RBD backend, the holes who can appear will automatically
 # be interpreted by Ceph as null bytes, and do not really consume your storage.
```

### Comparing `glance-28.0.0.0b2/etc/glance-image-import.conf.sample` & `glance-28.0.0.0rc1/etc/glance-image-import.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/glance-manage.conf` & `glance-28.0.0.0rc1/etc/glance-manage.conf`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,18 @@
 # is set. (boolean value)
 #use_json = false
 
 # Log output to standard error. This option is ignored if log_config_append is
 # set. (boolean value)
 #use_stderr = false
 
-# Log output to Windows Event Log. (boolean value)
+# DEPRECATED: Log output to Windows Event Log. (boolean value)
+# This option is deprecated for removal.
+# Its value may be silently ignored in the future.
+# Reason: Windows support is no longer maintained.
 #use_eventlog = false
 
 # The amount of time before the log files are rotated. This option is ignored
 # unless log_rotation_type is set to "interval". (integer value)
 #log_rotate_interval = 1
 
 # Rotation interval type. The time of the last file change (or the time when the
@@ -179,22 +182,14 @@
 #mysql_sql_mode = TRADITIONAL
 
 # For Galera only, configure wsrep_sync_wait causality checks on new
 # connections.  Default is None, meaning don't configure any setting. (integer
 # value)
 #mysql_wsrep_sync_wait = <None>
 
-# DEPRECATED: If True, transparently enables support for handling MySQL Cluster
-# (NDB). (boolean value)
-# This option is deprecated for removal since 12.1.0.
-# Its value may be silently ignored in the future.
-# Reason: Support for the MySQL NDB Cluster storage engine has been deprecated
-# and will be removed in a future release.
-#mysql_enable_ndb = false
-
 # Connections which have been present in the connection pool longer than this
 # number of seconds will be replaced with a new one the next time they are
 # checked out from the pool. (integer value)
 #connection_recycle_time = 3600
 
 # Maximum number of SQL connections to keep open in a pool. Setting a value of 0
 # indicates no limit. (integer value)
```

### Comparing `glance-28.0.0.0b2/etc/glance-scrubber.conf` & `glance-28.0.0.0rc1/etc/glance-scrubber.conf`

 * *Files 2% similar despite different names*

```diff
@@ -446,15 +446,15 @@
 #
 # Related options:
 #     * public_endpoint
 #
 #  (string value)
 #worker_self_reference_url = <None>
 
-#
+# DEPRECATED:
 # The amount of time, in seconds, to delay image scrubbing.
 #
 # When delayed delete is turned on, an image is put into ``pending_delete``
 # state upon deletion until the scrubber deletes its image data. Typically, soon
 # after the image is put into ``pending_delete`` state, it is available for
 # scrubbing. However, scrubbing can be delayed until a later point using this
 # configuration option. This option denotes the time period an image spends in
@@ -468,17 +468,21 @@
 #     * Any non-negative integer
 #
 # Related options:
 #     * ``delayed_delete``
 #
 #  (integer value)
 # Minimum value: 0
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #scrub_time = 0
 
-#
+# DEPRECATED:
 # The size of thread pool to be used for scrubbing images.
 #
 # When there are a large number of images to scrub, it is beneficial to scrub
 # images in parallel so that the scrub queue stays in control and the backend
 # storage is reclaimed in a timely fashion. This configuration option denotes
 # the maximum number of images to be scrubbed in parallel. The default value is
 # one, which signifies serial scrubbing. Any value above one indicates parallel
@@ -488,17 +492,21 @@
 #     * Any non-zero positive integer
 #
 # Related options:
 #     * ``delayed_delete``
 #
 #  (integer value)
 # Minimum value: 1
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #scrub_pool_size = 1
 
-#
+# DEPRECATED:
 # Turn on/off delayed delete.
 #
 # Typically when an image is deleted, the ``glance-api`` service puts the image
 # into ``deleted`` state and deletes its data at the same time. Delayed delete
 # is a feature in Glance that delays the actual deletion of image data until a
 # later point in time (as determined by the configuration option
 # ``scrub_time``).
@@ -518,17 +526,21 @@
 #
 # Related options:
 #     * ``scrub_time``
 #     * ``wakeup_time``
 #     * ``scrub_pool_size``
 #
 #  (boolean value)
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #delayed_delete = false
 
-#
+# DEPRECATED:
 # Time interval, in seconds, between scrubber runs in daemon mode.
 #
 # Scrubber can be run either as a cron job or daemon. When run as a daemon, this
 # configuration time specifies the time period between two runs. When the
 # scrubber wakes up, it fetches and scrubs all ``pending_delete`` images that
 # are available for scrubbing after taking ``scrub_time`` into consideration.
 #
@@ -541,17 +553,21 @@
 #
 # Related options:
 #     * ``daemon``
 #     * ``delayed_delete``
 #
 #  (integer value)
 # Minimum value: 0
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #wakeup_time = 300
 
-#
+# DEPRECATED:
 # Run scrubber as a daemon.
 #
 # This boolean configuration option indicates whether scrubber should
 # run as a long-running process that wakes up at regular intervals to
 # scrub images. The wake up interval can be specified using the
 # configuration option ``wakeup_time``.
 #
@@ -564,29 +580,37 @@
 #     * True
 #     * False
 #
 # Related options:
 #     * ``wakeup_time``
 #
 #  (boolean value)
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #daemon = false
 
-#
+# DEPRECATED:
 # Restore the image status from 'pending_delete' to 'active'.
 #
 # This option is used by administrator to reset the image's status from
 # 'pending_delete' to 'active' when the image is deleted by mistake and
 # 'pending delete' feature is enabled in Glance. Please make sure the
 # glance-scrubber daemon is stopped before restoring the image to avoid image
 # data inconsistency.
 #
 # Possible values:
 #     * image's uuid
 #
 #  (string value)
+# This option is deprecated for removal since 2024.1 (Caracal).
+# Its value may be silently ignored in the future.
+# Reason: The entire glance scrubber, including this option, is scheduled to be
+# removed during the 2024.2 (Dalmatian) development cycle.
 #restore = <None>
 
 #
 # From oslo.log
 #
 
 # If set to true, the logging level will be set to DEBUG instead of the default
@@ -646,15 +670,18 @@
 # is set. (boolean value)
 #use_json = false
 
 # Log output to standard error. This option is ignored if log_config_append is
 # set. (boolean value)
 #use_stderr = false
 
-# Log output to Windows Event Log. (boolean value)
+# DEPRECATED: Log output to Windows Event Log. (boolean value)
+# This option is deprecated for removal.
+# Its value may be silently ignored in the future.
+# Reason: Windows support is no longer maintained.
 #use_eventlog = false
 
 # The amount of time before the log files are rotated. This option is ignored
 # unless log_rotation_type is set to "interval". (integer value)
 #log_rotate_interval = 1
 
 # Rotation interval type. The time of the last file change (or the time when the
@@ -764,22 +791,14 @@
 #mysql_sql_mode = TRADITIONAL
 
 # For Galera only, configure wsrep_sync_wait causality checks on new
 # connections.  Default is None, meaning don't configure any setting. (integer
 # value)
 #mysql_wsrep_sync_wait = <None>
 
-# DEPRECATED: If True, transparently enables support for handling MySQL Cluster
-# (NDB). (boolean value)
-# This option is deprecated for removal since 12.1.0.
-# Its value may be silently ignored in the future.
-# Reason: Support for the MySQL NDB Cluster storage engine has been deprecated
-# and will be removed in a future release.
-#mysql_enable_ndb = false
-
 # Connections which have been present in the connection pool longer than this
 # number of seconds will be replaced with a new one the next time they are
 # checked out from the pool. (integer value)
 #connection_recycle_time = 3600
 
 # Maximum number of SQL connections to keep open in a pool. Setting a value of 0
 # indicates no limit. (integer value)
@@ -1584,39 +1603,32 @@
 #
 # Related options:
 #     * rbd_store_user
 #
 #  (string value)
 #rbd_store_ceph_conf =
 
-# DEPRECATED:
+#
 # Timeout value for connecting to Ceph cluster.
 #
 # This configuration option takes in the timeout value in seconds used
 # when connecting to the Ceph cluster i.e. it sets the time to wait for
 # glance-api before closing the connection. This prevents glance-api
 # hangups during the connection to RBD. If the value for this option
-# is set to less than or equal to 0, no timeout is set and the default
-# librados value is used.
+# is set to less than 0, no timeout is set and the default librados value
+# is used.
 #
 # Possible Values:
 #     * Any integer value
 #
 # Related options:
 #     * None
 #
 #  (integer value)
-# This option is deprecated for removal since Zed.
-# Its value may be silently ignored in the future.
-# Reason:
-# This option has not had any effect in years. Users willing to set a timeout
-# for
-# connecting to the Ceph cluster should use 'client_mount_timeout' in Ceph's
-# configuration file.
-#rados_connect_timeout = 0
+#rados_connect_timeout = -1
 
 #
 # Enable or not thin provisioning in this backend.
 #
 # This configuration option enable the feature of not really write null byte
 # sequences on the RBD backend, the holes who can appear will automatically
 # be interpreted by Ceph as null bytes, and do not really consume your storage.
```

### Comparing `glance-28.0.0.0b2/etc/glance-swift.conf.sample` & `glance-28.0.0.0rc1/etc/glance-swift.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/cim-processor-allocation-setting-data.json` & `glance-28.0.0.0rc1/etc/metadefs/cim-processor-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/cim-resource-allocation-setting-data.json` & `glance-28.0.0.0rc1/etc/metadefs/cim-resource-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/cim-storage-allocation-setting-data.json` & `glance-28.0.0.0rc1/etc/metadefs/cim-storage-allocation-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/cim-virtual-system-setting-data.json` & `glance-28.0.0.0rc1/etc/metadefs/cim-virtual-system-setting-data.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-aggr-disk-filter.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-aggr-disk-filter.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-aggr-iops-filter.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-aggr-iops-filter.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-aggr-num-instances.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-aggr-num-instances.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-cpu-mode.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-cpu-mode.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-cpu-pinning.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-cpu-pinning.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-guest-memory-backing.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-guest-memory-backing.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-guest-shutdown.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-guest-shutdown.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-host-capabilities.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-host-capabilities.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-hypervisor.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-hypervisor.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-instance-data.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-instance-data.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-libvirt-image.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-libvirt-image.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-libvirt.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-libvirt.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-quota.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-quota.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-randomgen.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-randomgen.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vcputopology.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vcputopology.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vmware-flavor.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vmware-flavor.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vmware-quota-flavor.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vmware-quota-flavor.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vmware.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vmware.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vtpm-hw.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vtpm-hw.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-vtpm.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-vtpm.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-watchdog.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-watchdog.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/compute-xenapi.json` & `glance-28.0.0.0rc1/etc/metadefs/compute-xenapi.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/glance-common-image-props.json` & `glance-28.0.0.0rc1/etc/metadefs/glance-common-image-props.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/image-signature-verification.json` & `glance-28.0.0.0rc1/etc/metadefs/image-signature-verification.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/operating-system.json` & `glance-28.0.0.0rc1/etc/metadefs/operating-system.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/software-databases.json` & `glance-28.0.0.0rc1/etc/metadefs/software-databases.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/software-runtimes.json` & `glance-28.0.0.0rc1/etc/metadefs/software-runtimes.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/software-webservers.json` & `glance-28.0.0.0rc1/etc/metadefs/software-webservers.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/metadefs/storage-volume-type.json` & `glance-28.0.0.0rc1/etc/metadefs/storage-volume-type.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/oslo-config-generator/glance-api.conf` & `glance-28.0.0.0rc1/etc/oslo-config-generator/glance-api.conf`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/property-protections-policies.conf.sample` & `glance-28.0.0.0rc1/etc/property-protections-policies.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/property-protections-roles.conf.sample` & `glance-28.0.0.0rc1/etc/property-protections-roles.conf.sample`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/etc/schema-image.json` & `glance-28.0.0.0rc1/etc/schema-image.json`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/__init__.py` & `glance-28.0.0.0rc1/glance/api/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/common.py` & `glance-28.0.0.0rc1/glance/api/common.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/middleware/cache.py` & `glance-28.0.0.0rc1/glance/api/middleware/cache.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/middleware/cache_manage.py` & `glance-28.0.0.0rc1/glance/api/middleware/cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/middleware/context.py` & `glance-28.0.0.0rc1/glance/api/middleware/context.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/middleware/gzip.py` & `glance-28.0.0.0rc1/glance/api/middleware/gzip.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/middleware/version_negotiation.py` & `glance-28.0.0.0rc1/glance/api/middleware/version_negotiation.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/policy.py` & `glance-28.0.0.0rc1/glance/api/policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/property_protections.py` & `glance-28.0.0.0rc1/glance/api/property_protections.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v1/router.py` & `glance-28.0.0.0rc1/glance/api/v1/router.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/cached_images.py` & `glance-28.0.0.0rc1/glance/api/v2/cached_images.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/discovery.py` & `glance-28.0.0.0rc1/glance/api/v2/discovery.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/image_actions.py` & `glance-28.0.0.0rc1/glance/api/v2/image_actions.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/image_data.py` & `glance-28.0.0.0rc1/glance/api/v2/image_data.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/image_members.py` & `glance-28.0.0.0rc1/glance/api/v2/image_members.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/image_tags.py` & `glance-28.0.0.0rc1/glance/api/v2/image_tags.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/images.py` & `glance-28.0.0.0rc1/glance/api/v2/images.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/metadef_namespaces.py` & `glance-28.0.0.0rc1/glance/api/v2/metadef_namespaces.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/metadef_objects.py` & `glance-28.0.0.0rc1/glance/api/v2/metadef_objects.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/metadef_properties.py` & `glance-28.0.0.0rc1/glance/api/v2/metadef_properties.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/metadef_resource_types.py` & `glance-28.0.0.0rc1/glance/api/v2/metadef_resource_types.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/metadef_tags.py` & `glance-28.0.0.0rc1/glance/api/v2/metadef_tags.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_namespace.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_namespace.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_object.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_object.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_property_item_type.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_property_item_type.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_property_type.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_property_type.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_resource_type.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_resource_type.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/model/metadef_tag.py` & `glance-28.0.0.0rc1/glance/api/v2/model/metadef_tag.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/policy.py` & `glance-28.0.0.0rc1/glance/api/v2/policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/router.py` & `glance-28.0.0.0rc1/glance/api/v2/router.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/schemas.py` & `glance-28.0.0.0rc1/glance/api/v2/schemas.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/v2/tasks.py` & `glance-28.0.0.0rc1/glance/api/v2/tasks.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/api/versions.py` & `glance-28.0.0.0rc1/glance/api/versions.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/__init__.py` & `glance-28.0.0.0rc1/glance/async_/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/__init__.py` & `glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/base_download.py` & `glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/base_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/copy_image.py` & `glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/copy_image.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/glance_download.py` & `glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/glance_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/_internal_plugins/web_download.py` & `glance-28.0.0.0rc1/glance/async_/flows/_internal_plugins/web_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/api_image_import.py` & `glance-28.0.0.0rc1/glance/async_/flows/api_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/base_import.py` & `glance-28.0.0.0rc1/glance/async_/flows/base_import.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/convert.py` & `glance-28.0.0.0rc1/glance/async_/flows/convert.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/introspect.py` & `glance-28.0.0.0rc1/glance/async_/flows/introspect.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/ovf_process.py` & `glance-28.0.0.0rc1/glance/async_/flows/ovf_process.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/__init__.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/image_conversion.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/image_conversion.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/image_decompression.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/image_decompression.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/inject_image_metadata.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/inject_image_metadata.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/no_op.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/no_op.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/flows/plugins/plugin_opts.py` & `glance-28.0.0.0rc1/glance/async_/flows/plugins/plugin_opts.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/taskflow_executor.py` & `glance-28.0.0.0rc1/glance/async_/taskflow_executor.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/async_/utils.py` & `glance-28.0.0.0rc1/glance/async_/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/api.py` & `glance-28.0.0.0rc1/glance/cmd/api.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/cache_cleaner.py` & `glance-28.0.0.0rc1/glance/cmd/cache_cleaner.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/cache_manage.py` & `glance-28.0.0.0rc1/glance/cmd/cache_manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,14 +495,17 @@
     if answer == "":
         return default
     else:
         return answer.lower() in ("yes", "y")
 
 
 def main():
+    print('In the Caracal development cycle, the glance-cache-manage command '
+          'has been deprecated in favor of the new Cache API. It is scheduled '
+          'to be removed in the Dalmatian development cycle.', file=sys.stderr)
     parser = argparse.ArgumentParser(
         description=_format_command_help(),
         formatter_class=argparse.RawDescriptionHelpFormatter)
     args = parse_args(parser)
 
     if args.command[0] == 'help' and len(args.command) == 1:
         parser.print_help()
```

### Comparing `glance-28.0.0.0b2/glance/cmd/cache_prefetcher.py` & `glance-28.0.0.0rc1/glance/cmd/cache_prefetcher.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/cache_pruner.py` & `glance-28.0.0.0rc1/glance/cmd/cache_pruner.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/control.py` & `glance-28.0.0.0rc1/glance/cmd/control.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/manage.py` & `glance-28.0.0.0rc1/glance/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/replicator.py` & `glance-28.0.0.0rc1/glance/cmd/replicator.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,16 +504,18 @@
                 # Upload the image itself
                 with open(os.path.join(path, image_uuid + '.img')) as img_file:
                     try:
                         headers, body = client.add_image(meta, img_file)
                         _check_upload_response_headers(headers, body)
                         updated.append(meta['id'])
                     except exc.HTTPConflict:
-                        LOG.error(_LE(IMAGE_ALREADY_PRESENT_MESSAGE)
-                                  % image_uuid)  # noqa
+                        # NOTE(tkajinam): noqa does not work with multi-line,
+                        # so split this interpolation to a separate line
+                        msg = _LE(IMAGE_ALREADY_PRESENT_MESSAGE) % image_uuid
+                        LOG.error(msg)
 
     return updated
 
 
 def replication_livecopy(options, args):
     """%(prog)s livecopy <fromserver:port> <toserver:port>
```

### Comparing `glance-28.0.0.0b2/glance/cmd/scrubber.py` & `glance-28.0.0.0rc1/glance/cmd/scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/cmd/status.py` & `glance-28.0.0.0rc1/glance/cmd/status.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/auth.py` & `glance-28.0.0.0rc1/glance/common/auth.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/client.py` & `glance-28.0.0.0rc1/glance/common/client.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/config.py` & `glance-28.0.0.0rc1/glance/common/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,15 +653,20 @@
          project='glance',
          version=version.cached_version_string(),
          usage=usage,
          default_config_files=default_config_files)
 
 
 def parse_cache_args(args=None):
-    config_files = cfg.find_config_files(project='glance', prog='glance-cache')
+    config_files = cfg.find_config_files(project='glance', prog='glance-api')
+    # NOTE(abhishekk): Reading glance-api file first and glance-cache file
+    # later so that if glance-cache file has different values set for some
+    # cache related options then they should take precedence.
+    config_files.extend(cfg.find_config_files(project='glance',
+                                              prog='glance-cache'))
     parse_args(args=args, default_config_files=config_files)
 
 
 def _get_deployment_flavor(flavor=None):
     """
     Retrieve the paste_deploy.flavor config item, formatted appropriately
     for appending to the application name.
```

### Comparing `glance-28.0.0.0b2/glance/common/crypt.py` & `glance-28.0.0.0rc1/glance/common/crypt.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/exception.py` & `glance-28.0.0.0rc1/glance/common/exception.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/format_inspector.py` & `glance-28.0.0.0rc1/glance/common/format_inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -508,15 +508,15 @@
 # createType=XXX line that specifies the mechanism by which the data
 # extents are stored in this file. We only support the
 # "monolithicSparse" format, so we just need to confirm that this file
 # contains that specifier.
 #
 # https://www.vmware.com/app/vmdk/?src=vmdk
 class VMDKInspector(FileInspector):
-    """vmware VMDK format (monolithicSparse variant only)
+    """vmware VMDK format (monolithicSparse and streamOptimized variants only)
 
     This needs to store the 512 byte header and the descriptor region
     which should be just after that. The descriptor region is some
     variable number of 512 byte sectors, but is just text defining the
     layout of the disk.
     """
 
@@ -578,15 +578,15 @@
         type_end = descriptor.find(b'"', type_idx)
         # Make sure we don't grab and log a huge chunk of data in a
         # maliciously-formatted descriptor region
         if type_end - type_idx < 64:
             vmdktype = descriptor[type_idx:type_end]
         else:
             vmdktype = b'formatnotfound'
-        if vmdktype != b'monolithicSparse':
+        if vmdktype not in (b'monolithicSparse', b'streamOptimized'):
             LOG.warning('Unsupported VMDK format %s', vmdktype)
             return 0
 
         # If we have the descriptor, we definitely have the header
         _sig, _ver, _flags, sectors, _grain, _desc_sec, _desc_num = (
             struct.unpack('<IIIQQQQ', self.region('header').data[:44]))
```

### Comparing `glance-28.0.0.0b2/glance/common/location_strategy/__init__.py` & `glance-28.0.0.0rc1/glance/common/location_strategy/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,21 @@
 from oslo_log import log as logging
 import stevedore
 
 from glance.i18n import _, _LE
 
 location_strategy_opts = [
     cfg.StrOpt('location_strategy',
+               deprecated_for_removal=True,
+               deprecated_since="Caracal",
+               deprecated_reason=_("""
+In Bobcat, a new weighing mechanism has been introduced, which makes the
+location strategy obsolete.  This option is scheduled to be removed during the
+Dalmatian development cycle.
+"""),
                default='location_order',
                choices=('location_order', 'store_type'),
                help=_("""
 Strategy to determine the preference order of image locations.
 
 This configuration option indicates the strategy to determine
 the order in which an image's locations must be accessed to
```

### Comparing `glance-28.0.0.0b2/glance/common/location_strategy/location_order.py` & `glance-28.0.0.0rc1/glance/common/location_strategy/location_order.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/location_strategy/store_type.py` & `glance-28.0.0.0rc1/glance/common/location_strategy/store_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,21 @@
 from oslo_config import cfg
 
 from glance.i18n import _
 
 store_type_opts = [
     cfg.ListOpt('store_type_preference',
                 default=[],
+                deprecated_for_removal=True,
+                deprecated_since="Caracal",
+                deprecated_reason=_("""
+In Bobcat, a new weighing mechanism has been introduced, which makes the
+location strategy obsolete.  This option is scheduled to be removed during the
+Dalmatian development cycle.
+"""),
                 help=_("""
 Preference order of storage backends.
 
 Provide a comma separated list of store names in the order in
 which images should be retrieved from storage backends.
 These store names must be registered with the ``stores``
 configuration option.
```

### Comparing `glance-28.0.0.0b2/glance/common/property_utils.py` & `glance-28.0.0.0rc1/glance/common/property_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/removed_config.py` & `glance-28.0.0.0rc1/glance/common/removed_config.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/scripts/__init__.py` & `glance-28.0.0.0rc1/glance/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/scripts/api_image_import/main.py` & `glance-28.0.0.0rc1/glance/common/scripts/api_image_import/main.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/scripts/image_import/main.py` & `glance-28.0.0.0rc1/glance/common/scripts/image_import/main.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/scripts/utils.py` & `glance-28.0.0.0rc1/glance/common/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/store_utils.py` & `glance-28.0.0.0rc1/glance/common/store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/swift_store_utils.py` & `glance-28.0.0.0rc1/glance/common/swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/timeutils.py` & `glance-28.0.0.0rc1/glance/common/timeutils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/trust_auth.py` & `glance-28.0.0.0rc1/glance/common/trust_auth.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/utils.py` & `glance-28.0.0.0rc1/glance/common/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/common/wsgi.py` & `glance-28.0.0.0rc1/glance/common/wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 from glance.common import exception
 from glance.common import store_utils
 from glance.common import utils
 import glance.db
 from glance import housekeeping
 from glance import i18n
 from glance.i18n import _, _LE, _LI, _LW
+from glance import sqlite_migration
 
 
 bind_opts = [
     cfg.HostAddressOpt('bind_host',
                        default='0.0.0.0',
                        help=_("""
 IP address to bind the glance servers to.
@@ -450,14 +451,18 @@
 
         :param application: The application to be run in the WSGI server
         :param default_port: Port to bind to if none is specified in conf
         """
         self.application = application
         self.default_port = default_port
         self.configure()
+
+        # NOTE(abhishekk): This will raise RuntimeError if
+        # worker_self_reference_url is not set in glance-api.conf
+        sqlite_migration.migrate_if_required()
         self.start_wsgi()
 
         # NOTE(danms): This may raise GlanceException if the staging store is
         # not configured properly, which will be caught and printed by
         # cmd/api.py as an error message and abort startup.
         staging = housekeeping.staging_store_path()
         if not os.path.exists(staging) and CONF.enabled_import_methods:
```

### Comparing `glance-28.0.0.0b2/glance/common/wsgi_app.py` & `glance-28.0.0.0rc1/glance/common/wsgi_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from glance.api import common
 import glance.async_
 from glance.common import config
 from glance.common import store_utils
 from glance import housekeeping
 from glance.i18n import _, _LW
 from glance import notifier
+from glance import sqlite_migration
 
 CONF = cfg.CONF
 CONF.import_group("profiler", "glance.common.wsgi")
 CONF.import_opt("enabled_backends", "glance.common.wsgi")
 logging.register_options(CONF)
 LOG = logging.getLogger(__name__)
 
@@ -137,14 +138,18 @@
         glance_store.create_multi_stores(CONF, reserved_stores=RESERVED_STORES)
         glance_store.verify_store()
     else:
         glance_store.register_opts(CONF)
         glance_store.create_stores(CONF)
         glance_store.verify_default_store()
 
+    # NOTE(abhishekk): This will raise RuntimeError if
+    # worker_self_reference_url is not set in glance-api.conf
+    sqlite_migration.migrate_if_required()
+
     # NOTE(danms): This may raise GlanceException if the staging store is
     # not configured properly, which will bubble up to the WSGI server,
     # aborting application load as desired.
     staging = housekeeping.staging_store_path()
     if not os.path.exists(staging) and CONF.enabled_import_methods:
         LOG.warning(_LW('Import methods are enabled but staging directory '
                         '%(path)s does not exist; Imports will fail!'),
```

### Comparing `glance-28.0.0.0b2/glance/common/wsme_utils.py` & `glance-28.0.0.0rc1/glance/common/wsme_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         for attribute in model._wsme_attributes:
             names.append(attribute.name)
 
         values = {}
         for name in names:
             value = getattr(db_entity, name, None)
             if value is not None:
-                if type(value) == datetime:
+                if isinstance(value, datetime):
                     iso_datetime_value = timeutils.isotime(value)
                     values.update({name: iso_datetime_value})
                 else:
                     values.update({name: value})
 
         if schema:
             values['schema'] = schema
```

### Comparing `glance-28.0.0.0b2/glance/context.py` & `glance-28.0.0.0rc1/glance/context.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/__init__.py` & `glance-28.0.0.0rc1/glance/db/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/metadata.py` & `glance-28.0.0.0rc1/glance/db/metadata.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/migration.py` & `glance-28.0.0.0rc1/glance/db/migration.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 
 db_options.set_defaults(cfg.CONF)
 
 
 # Migration-related constants
 EXPAND_BRANCH = 'expand'
 CONTRACT_BRANCH = 'contract'
-CURRENT_RELEASE = '2023_2'
+CURRENT_RELEASE = '2024_1'
 ALEMBIC_INIT_VERSION = 'liberty'
```

### Comparing `glance-28.0.0.0b2/glance/db/simple/api.py` & `glance-28.0.0.0rc1/glance/db/simple/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,24 @@
 from glance.db import utils as db_utils
 from glance.i18n import _, _LI, _LW
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 DATA = {
+    'cached_images': {},
     'images': {},
     'members': [],
     'metadef_namespace_resource_types': [],
     'metadef_namespaces': [],
     'metadef_objects': [],
     'metadef_properties': [],
     'metadef_resource_types': [],
     'metadef_tags': [],
+    'node_reference': {},
     'tags': {},
     'locations': [],
     'tasks': {},
     'task_info': {},
 }
 
 INDEX = 0
@@ -72,22 +74,24 @@
         LOG.critical(msg)
         raise SystemExit(msg)
 
 
 def reset():
     global DATA
     DATA = {
+        'cached_images': {},
         'images': {},
         'members': [],
         'metadef_namespace_resource_types': [],
         'metadef_namespaces': [],
         'metadef_objects': [],
         'metadef_properties': [],
         'metadef_resource_types': [],
         'metadef_tags': [],
+        'node_reference': {},
         'tags': {},
         'locations': [],
         'tasks': {},
         'task_info': {},
     }
 
 
@@ -1024,16 +1028,16 @@
 def _task_soft_delete(context):
     """Scrub task entities which are expired """
     global DATA
     now = timeutils.utcnow()
     tasks = DATA['tasks'].values()
 
     for task in tasks:
-        if(task['owner'] == context.owner and task['deleted'] == False
-           and task['expires_at'] <= now):
+        if (task['owner'] == context.owner and task['deleted'] == False
+                and task['expires_at'] <= now):
 
             task['deleted'] = True
             task['deleted_at'] = timeutils.utcnow()
 
 
 @log_call
 def task_get_all(context, filters=None, marker=None, limit=None,
@@ -2132,7 +2136,166 @@
         raise exception.MetadefForbidden(emsg)
 
 
 def _get_metadef_id():
     global INDEX
     INDEX += 1
     return INDEX
+
+
+def _cached_image_format(cached_image):
+    """Format a cached image for consumption outside of this module"""
+    image_dict = {
+        'id': cached_image['id'],
+        'image_id': cached_image['image_id'],
+        'last_accessed': cached_image['last_accessed'].timestamp(),
+        'last_modified': cached_image['last_modified'].timestamp(),
+        'size': cached_image['size'],
+        'hits': cached_image['hits'],
+        'checksum': cached_image['checksum']
+    }
+
+    return image_dict
+
+
+@log_call
+def node_reference_get_by_url(context, node_reference_url):
+    global DATA
+    db_data = DATA['node_reference']
+    for node_reference in db_data:
+        if db_data[node_reference]['node_reference_url'] == node_reference_url:
+            return db_data[node_reference]
+    else:
+        raise exception.NotFound()
+
+
+@log_call
+def node_reference_create(context, node_reference_url, **values):
+    global DATA
+    node_reference_id = values.get('node_reference_id', 1)
+
+    if node_reference_id in DATA['node_reference']:
+        raise exception.Duplicate()
+
+    node_reference = {
+        'node_reference_id': node_reference_id,
+        'node_reference_url': node_reference_url
+    }
+
+    DATA['node_reference'][node_reference_id] = node_reference
+    return node_reference
+
+
+@log_call
+def get_hit_count(context, image_id, node_reference_url):
+    global DATA
+    if image_id not in DATA['cached_images']:
+        return 0
+
+    cached_image = _cached_image_format(DATA['cached_images'][image_id])
+    return cached_image['hits']
+
+
+@log_call
+def get_cached_images(context, node_reference_url):
+    global DATA
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    all_images = DATA['cached_images']
+    cached_images = []
+    for image_id in all_images:
+        if all_images[image_id]['node_reference_id'] == \
+                node_reference['node_reference_id']:
+            cached_images.append(_cached_image_format(all_images[image_id]))
+
+    return cached_images
+
+
+@log_call
+def delete_all_cached_images(context, node_reference_url):
+    global DATA
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    all_images = all_images = tuple(DATA['cached_images'].keys())
+    for image_id in all_images:
+        if DATA['cached_images'][image_id]['node_reference_id'] == \
+                node_reference['node_reference_id']:
+            del DATA['cached_images'][image_id]
+
+
+@log_call
+def delete_cached_image(context, image_id, node_reference_url):
+    global DATA
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    all_images = tuple(DATA['cached_images'].keys())
+    for image in all_images:
+        if DATA['cached_images'][image]['node_reference_id'] == \
+                node_reference['node_reference_id'] and image_id == \
+                DATA['cached_images'][image]['image_id']:
+            del DATA['cached_images'][image]
+            break
+
+
+@log_call
+def get_least_recently_accessed(context, node_reference_url):
+    global DATA
+    all_images = get_cached_images(context, node_reference_url)
+    if all_images:
+        return all_images[0]['image_id']
+    return None
+
+
+@log_call
+def is_image_cached_for_node(context, node_reference_url, image_id):
+    global DATA
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    all_images = DATA['cached_images']
+    for image_id in all_images:
+        if all_images[image_id]['node_reference_id'] == \
+                node_reference['node_reference_id'] and image_id == \
+                all_images[image_id]['image_id']:
+            return True
+    return False
+
+
+@log_call
+def insert_cache_details(context, node_reference_url, image_id,
+                         size, checksum=None, last_accessed=None,
+                         last_modified=None, hits=None):
+    global DATA
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    accessed = last_accessed or timeutils.utcnow()
+    modified = last_modified or timeutils.utcnow()
+
+    values = {
+        'last_accessed': accessed,
+        'last_modified': modified,
+        'node_reference_id': node_reference['node_reference_id'],
+        'checksum': checksum,
+        'image_id': image_id,
+        'size': size,
+        'hits': hits or 0,
+        'id': str(uuid.uuid4()),
+    }
+
+    if image_id in DATA['cached_images']:
+        raise exception.Duplicate()
+
+    DATA['cached_images'][image_id] = values
+
+
+@log_call
+def update_hit_count(context, image_id, node_reference_url):
+    global DATA
+    last_hit_count = get_hit_count(context, image_id, node_reference_url)
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    all_images = DATA['cached_images']
+    last_accessed = timeutils.utcnow()
+    values = {
+        'hits': last_hit_count + 1,
+        'last_accessed': last_accessed
+    }
+
+    for image_id in all_images:
+        if all_images[image_id]['node_reference_id'] == \
+                node_reference['node_reference_id'] and image_id == \
+                all_images[image_id]['image_id']:
+            all_images[image_id].update(values)
+            break
```

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/__init__.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_artifacts_tables.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_images_tables.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/alembic.ini` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/env.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/migrate.cfg` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/migrate.cfg`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/pike_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/queens_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/queens_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_contract02_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand01_add_os_hidden.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/rocky_expand02_add_os_hash_.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/train_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/train_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/ussuri_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/wallaby_expand01_add_user_imageid_requestid_to_tasks.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/xena_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/xena_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/yoga_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/zed_contract01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/alembic_migrations/versions/zed_expand01_empty.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/api.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -388,26 +388,26 @@
     """
 
     if 'id' not in sort_keys:
         # TODO(justinsb): If this ever gives a false-positive, check
         # the actual primary key, rather than assuming its id
         LOG.warning(_LW('Id not in sort_keys; is sort_keys unique?'))
 
-    assert(not (sort_dir and sort_dirs))  # nosec
+    assert (not (sort_dir and sort_dirs))  # nosec
     # nosec: This function runs safely if the assertion fails.
 
     # Default the sort direction to ascending
     if sort_dir is None:
         sort_dir = 'asc'
 
     # Ensure a per-column sort direction
     if sort_dirs is None:
         sort_dirs = [sort_dir] * len(sort_keys)
 
-    assert(len(sort_dirs) == len(sort_keys))  # nosec
+    assert (len(sort_dirs) == len(sort_keys))  # nosec
     # nosec: This function runs safely if the assertion fails.
     if len(sort_dirs) < len(sort_keys):
         sort_dirs += [sort_dir] * (len(sort_keys) - len(sort_dirs))
 
     # Add sorting
     for current_sort_key, current_sort_dir in zip(sort_keys, sort_dirs):
         sort_dir_func = {
@@ -2365,7 +2365,218 @@
 
 
 def metadef_tag_count(context, namespace_name):
     """Get count of tags for a namespace, raise if ns doesn't exist."""
     session = get_session()
     with session.begin():
         return metadef_tag_api.count(context, session, namespace_name)
+
+
+def _cached_image_format(cached_image):
+    """Format a cached image for consumption outside of this module"""
+    image_dict = {
+        'id': cached_image['id'],
+        'image_id': cached_image['image_id'],
+        'last_accessed': cached_image['last_accessed'].timestamp(),
+        'last_modified': cached_image['last_modified'].timestamp(),
+        'size': cached_image['size'],
+        'hits': cached_image['hits'],
+        'checksum': cached_image['checksum']
+    }
+
+    return image_dict
+
+
+def node_reference_get_by_url(context, node_reference_url):
+    """Get a node reference by node reference url"""
+    session = get_session()
+    with session.begin():
+        try:
+            query = session.query(models.NodeReference)
+            query = query.filter_by(node_reference_url=node_reference_url)
+            return query.one()
+        except sa_orm.exc.NoResultFound:
+            msg = _("The node reference %s"
+                    " was not found." % node_reference_url)
+            LOG.debug(msg)
+            raise exception.NotFound(msg)
+
+
+@utils.no_4byte_params
+def node_reference_create(context, node_reference_url):
+    """Create a node_reference  or raise if it already exists."""
+    session = get_session()
+    values = {'node_reference_url': node_reference_url}
+
+    with session.begin():
+        node_reference = models.NodeReference()
+        node_reference.update(values.copy())
+        try:
+            node_reference.save(session=session)
+        except db_exception.DBDuplicateEntry:
+            raise exception.Duplicate()
+
+    return node_reference
+
+
+def get_hit_count(context, image_id, node_reference_url):
+    session = get_session()
+    node_id = models.NodeReference.node_reference_id
+    filters = [
+        models.CachedImages.image_id == image_id,
+        models.NodeReference.node_reference_url == node_reference_url,
+    ]
+    with session.begin():
+        try:
+            query = session.query(
+                models.CachedImages.hits).join(
+                models.NodeReference,
+                node_id == models.CachedImages.node_reference_id,
+                isouter=True).filter(sa_sql.and_(*filters))
+            return query.one()[0]
+        except sa_orm.exc.NoResultFound:
+            msg = _("Referenced %s is not cached on"
+                    " %s." % (image_id, node_reference_url))
+            LOG.debug(msg)
+            # NOTE(abhishekk): Since image is not cached yet, assuming
+            # hit count as 0
+            return 0
+
+
+def get_cached_images(context, node_reference_url):
+    node_id = models.NodeReference.node_reference_id
+    session = get_session()
+    with session.begin():
+        query = session.query(
+            models.CachedImages).join(
+            models.NodeReference,
+            node_id == models.CachedImages.node_reference_id,
+            isouter=True).filter(
+            models.NodeReference.node_reference_url == node_reference_url)
+
+        cached_images = []
+        for image in query.all():
+            cached_images.append(_cached_image_format(image))
+        return cached_images
+
+
+@utils.no_4byte_params
+def delete_all_cached_images(context, node_reference_url):
+    session = get_session()
+    with session.begin():
+        node_id = session.query(models.NodeReference.node_reference_id).filter(
+            models.NodeReference.node_reference_url == node_reference_url
+        ).scalar_subquery()
+
+        query = session.query(models.CachedImages)
+        query = query.filter_by(node_reference_id=node_id)
+
+        query.delete(synchronize_session=False)
+
+
+def delete_cached_image(context, image_id, node_reference_url):
+    session = get_session()
+    with session.begin():
+        node_id = session.query(models.NodeReference.node_reference_id).filter(
+            models.NodeReference.node_reference_url == node_reference_url
+        ).scalar_subquery()
+
+        query = session.query(models.CachedImages)
+        query = query.filter(
+            models.CachedImages.image_id == image_id)
+        query = query.filter_by(node_reference_id=node_id)
+
+        query.delete(synchronize_session=False)
+
+
+def get_least_recently_accessed(context, node_reference_url):
+    node_id = models.NodeReference.node_reference_id
+    session = get_session()
+    with session.begin():
+        query = session.query(
+            models.CachedImages.image_id).join(
+            models.NodeReference,
+            node_id == models.CachedImages.node_reference_id,
+            isouter=True).filter(
+            models.NodeReference.node_reference_url == node_reference_url)
+        query = query.order_by(models.CachedImages.last_accessed)
+        try:
+            image_id = query.first()[0]
+        except TypeError:
+            # There are no more cached images
+            return None
+
+    return image_id
+
+
+def is_image_cached_for_node(context, node_reference_url, image_id):
+    node_id = models.NodeReference.node_reference_id
+    filters = [
+        models.CachedImages.image_id == image_id,
+        models.NodeReference.node_reference_url == node_reference_url,
+    ]
+    session = get_session()
+    with session.begin():
+        try:
+            query = session.query(
+                models.CachedImages.id).join(
+                models.NodeReference,
+                node_id == models.CachedImages.node_reference_id,
+                isouter=True).filter(sa_sql.and_(*filters))
+            if query.one()[0]:
+                return True
+        except sa_orm.exc.NoResultFound:
+            msg = _("Referenced %s is not cached on"
+                    " %s." % (image_id, node_reference_url))
+            LOG.debug(msg)
+            return False
+
+
+@utils.no_4byte_params
+def insert_cache_details(context, node_reference_url, image_id,
+                         filesize, checksum=None, last_accessed=None,
+                         last_modified=None, hits=None):
+    node_reference = node_reference_get_by_url(context, node_reference_url)
+    session = get_session()
+    accessed = last_accessed or timeutils.utcnow()
+    modified = last_modified or timeutils.utcnow()
+
+    values = {
+        'image_id': image_id,
+        'size': filesize,
+        'last_accessed': accessed,
+        'last_modified': modified,
+        'hits': hits or 0,
+        'checksum': checksum,
+        'node_reference_id': node_reference['node_reference_id']
+    }
+
+    with session.begin():
+        cached_image = models.CachedImages()
+        cached_image.update(values.copy())
+        try:
+            cached_image.save(session=session)
+        except db_exception.DBDuplicateEntry:
+            msg = _("Cache entry for %s for %s"
+                    " already exists." % (image_id, node_reference_url))
+            LOG.debug(msg)
+
+
+@utils.no_4byte_params
+def update_hit_count(context, image_id, node_reference_url):
+    session = get_session()
+    last_accessed = timeutils.utcnow()
+
+    with session.begin():
+        node_id = session.query(models.NodeReference.node_reference_id).filter(
+            models.NodeReference.node_reference_url == node_reference_url
+        ).scalar_subquery()
+
+        query = session.query(models.CachedImages)
+        query = query.filter(
+            models.CachedImages.image_id == image_id)
+        query = query.filter_by(node_reference_id=node_id)
+
+        query.update({
+            'hits': models.CachedImages.hits + 1,
+            'last_accessed': last_accessed
+        }, synchronize_session='fetch')
```

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadata.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadata.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/namespace.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/namespace.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/object.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/object.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/property.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/property.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/resource_type.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/resource_type_association.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/resource_type_association.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/tag.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/tag.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/metadef_api/utils.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/metadef_api/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/models.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -254,14 +254,51 @@
     # SQLAlchemy marshals the data to/from JSON using custom type
     # JSONEncodedDict. It uses simplejson underneath.
     input = Column(JSONEncodedDict())
     result = Column(JSONEncodedDict())
     message = Column(Text)
 
 
+class NodeReference(BASE, models.ModelBase):
+    """Represents node info in the datastore"""
+    __tablename__ = 'node_reference'
+    __table_args__ = (UniqueConstraint(
+        'node_reference_url',
+        name='uq_node_reference_node_reference_url'),)
+
+    node_reference_id = Column(BigInteger().with_variant(Integer, 'sqlite'),
+                               primary_key=True,
+                               nullable=False, autoincrement=True)
+    node_reference_url = Column(String(length=255),
+                                nullable=False)
+
+
+class CachedImages(BASE, models.ModelBase):
+    """Represents an image tag in the datastore."""
+    __tablename__ = 'cached_images'
+    __table_args__ = (UniqueConstraint(
+        'image_id',
+        'node_reference_id',
+        name='ix_cached_images_image_id_node_reference_id'),)
+
+    id = Column(BigInteger().with_variant(Integer, 'sqlite'),
+                primary_key=True, autoincrement=True,
+                nullable=False)
+    image_id = Column(String(36), nullable=False)
+    last_accessed = Column(DateTime, nullable=False)
+    last_modified = Column(DateTime, nullable=False)
+    size = Column(BigInteger(), nullable=False)
+    hits = Column(Integer, nullable=False)
+    checksum = Column(String(32), nullable=True)
+    node_reference_id = Column(
+        BigInteger().with_variant(Integer, 'sqlite'),
+        ForeignKey('node_reference.node_reference_id'),
+        nullable=False)
+
+
 def register_models(engine):
     """Create database tables for all models with the given engine."""
     models = (Image, ImageProperty, ImageMember)
     for model in models:
         model.metadata.create_all(engine)
```

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/models_metadef.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/models_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/sqlalchemy/schema.py` & `glance-28.0.0.0rc1/glance/db/sqlalchemy/schema.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/db/utils.py` & `glance-28.0.0.0rc1/glance/db/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/domain/__init__.py` & `glance-28.0.0.0rc1/glance/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/domain/proxy.py` & `glance-28.0.0.0rc1/glance/domain/proxy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/gateway.py` & `glance-28.0.0.0rc1/glance/gateway.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/hacking/checks.py` & `glance-28.0.0.0rc1/glance/hacking/checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,25 +91,25 @@
         "glance/quota",
         "glance/store",
         "glance/tests",
     ]
 
     if max([name in filename for name in dirs]):
         if logical_line.startswith("LOG.debug(_("):
-            yield(0, "G319: Don't translate debug level logs")
+            yield (0, "G319: Don't translate debug level logs")
 
 
 @core.flake8ext
 def check_no_contextlib_nested(logical_line):
     msg = ("G327: contextlib.nested is deprecated since Python 2.7. See "
            "https://docs.python.org/2/library/contextlib.html#contextlib."
            "nested for more information.")
     if ("with contextlib.nested(" in logical_line or
             "with nested(" in logical_line):
-        yield(0, msg)
+        yield (0, msg)
 
 
 @core.flake8ext
 def dict_constructor_with_list_copy(logical_line):
     msg = ("G328: Must use a dict comprehension instead of a dict constructor "
            "with a sequence of key-value pairs.")
     if dict_constructor_with_list_copy_re.match(logical_line):
```

### Comparing `glance-28.0.0.0b2/glance/housekeeping.py` & `glance-28.0.0.0rc1/glance/housekeeping.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/i18n.py` & `glance-28.0.0.0rc1/glance/i18n.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/__init__.py` & `glance-28.0.0.0rc1/glance/image_cache/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 from glance.common import exception
 from glance.common import utils
 from glance.i18n import _, _LE, _LI, _LW
 
 LOG = logging.getLogger(__name__)
 
 image_cache_opts = [
-    cfg.StrOpt('image_cache_driver', default='sqlite',
-               choices=('sqlite', 'xattr'), ignore_case=True,
+    cfg.StrOpt('image_cache_driver', default='centralized_db',
+               choices=('centralized_db', 'sqlite', 'xattr'), ignore_case=True,
                help=_("""
 The driver to use for image cache management.
 
 This configuration option provides the flexibility to choose between the
 different image-cache drivers available. An image-cache driver is responsible
 for providing the essential functions of image-cache like write images to/read
 images from cache, track age and usage of cached images, provide a list of
@@ -46,21 +46,29 @@
 
 The essential functions of a driver are defined in the base class
 ``glance.image_cache.drivers.base.Driver``. All image-cache drivers (existing
 and prospective) must implement this interface. Currently available drivers
 are ``sqlite`` and ``xattr``. These drivers primarily differ in the way they
 store the information about cached images:
 
-* The ``sqlite`` driver uses a sqlite database (which sits on every glance
-  node locally) to track the usage of cached images.
+* The ``centralized_db`` driver uses a central database (which will be common
+  for all glance nodes) to track the usage of cached images.
+* The ``sqlite`` (deprecated) driver uses a sqlite database (which sits on
+  every glance node locally) to track the usage of cached images.
 * The ``xattr`` driver uses the extended attributes of files to store this
   information. It also requires a filesystem that sets ``atime`` on the files
   when accessed.
 
+Deprecation warning:
+    * As centralized database will now be used for image cache management, the
+      use of `sqlite` database and driver will be dropped from 'E' (2025.1)
+      development cycle.
+
 Possible values:
+    * centralized_db
     * sqlite
     * xattr
 
 Related options:
     * None
 
 """)),
```

### Comparing `glance-28.0.0.0b2/glance/image_cache/base.py` & `glance-28.0.0.0rc1/glance/image_cache/base.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/cleaner.py` & `glance-28.0.0.0rc1/glance/image_cache/cleaner.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/client.py` & `glance-28.0.0.0rc1/glance/image_cache/client.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/drivers/base.py` & `glance-28.0.0.0rc1/glance/image_cache/drivers/base.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/drivers/sqlite.py` & `glance-28.0.0.0rc1/glance/image_cache/drivers/xattr.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,95 +10,70 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 """
-Cache driver that uses SQLite to store information about cached images
+Cache driver that uses xattr file tags and requires a filesystem
+that has atimes set.
+
+Assumptions
+===========
+
+1. Cache data directory exists on a filesystem that updates atime on
+   reads ('noatime' should NOT be set)
+
+2. Cache data directory exists on a filesystem that supports xattrs.
+   This is optional, but highly recommended since it allows us to
+   present ops with useful information pertaining to the cache, like
+   human readable filenames and statistics.
+
+3. `glance-prune` is scheduled to run as a periodic job via cron. This
+    is needed to run the LRU prune strategy to keep the cache size
+    within the limits set by the config file.
+
+
+Cache Directory Notes
+=====================
+
+The image cache data directory contains the main cache path, where the
+active cache entries and subdirectories for handling partial downloads
+and errored-out cache images.
+
+The layout looks like:
+
+$image_cache_dir/
+  entry1
+  entry2
+  ...
+  incomplete/
+  invalid/
+  queue/
 """
 from contextlib import contextmanager
+import errno
 import os
-import sqlite3
 import stat
 import time
 
-from eventlet import sleep
-from eventlet import timeout
-from oslo_concurrency import lockutils
 from oslo_config import cfg
 from oslo_log import log as logging
+from oslo_utils import encodeutils
 from oslo_utils import excutils
 from oslo_utils import fileutils
+import xattr
 
 from glance.common import exception
-from glance.i18n import _, _LE, _LI, _LW
+from glance.i18n import _, _LI
 from glance.image_cache.drivers import base
 
 LOG = logging.getLogger(__name__)
 
-sqlite_opts = [
-    cfg.StrOpt('image_cache_sqlite_db', default='cache.db',
-               help=_("""
-The relative path to sqlite file database that will be used for image cache
-management.
-
-This is a relative path to the sqlite file database that tracks the age and
-usage statistics of image cache. The path is relative to image cache base
-directory, specified by the configuration option ``image_cache_dir``.
-
-This is a lightweight database with just one table.
-
-Possible values:
-    * A valid relative path to sqlite file database
-
-Related options:
-    * ``image_cache_dir``
-
-""")),
-]
-
 CONF = cfg.CONF
-CONF.register_opts(sqlite_opts)
-
-DEFAULT_SQL_CALL_TIMEOUT = 2
-
-
-class SqliteConnection(sqlite3.Connection):
-
-    """
-    SQLite DB Connection handler that plays well with eventlet,
-    slightly modified from Swift's similar code.
-    """
-
-    def __init__(self, *args, **kwargs):
-        self.timeout_seconds = kwargs.get('timeout', DEFAULT_SQL_CALL_TIMEOUT)
-        kwargs['timeout'] = 0
-        sqlite3.Connection.__init__(self, *args, **kwargs)
-
-    def _timeout(self, call):
-        with timeout.Timeout(self.timeout_seconds):
-            while True:
-                try:
-                    return call()
-                except sqlite3.OperationalError as e:
-                    if 'locked' not in str(e):
-                        raise
-                sleep(0.05)
-
-    def execute(self, *args, **kwargs):
-        return self._timeout(lambda: sqlite3.Connection.execute(
-            self, *args, **kwargs))
-
-    def commit(self):
-        return self._timeout(lambda: sqlite3.Connection.commit(self))
-
-
-def dict_factory(cur, row):
-    return {col[0]: row[idx] for idx, col in enumerate(cur.description)}
 
 
 class Driver(base.Driver):
 
     """
     Cache driver that uses xattr file tags and requires a filesystem
     that has atimes set.
@@ -107,90 +82,83 @@
     def configure(self):
         """
         Configure the driver to use the stored configuration options
         Any store that needs special configuration should implement
         this method. If the store was not able to successfully configure
         itself, it should raise `exception.BadDriverConfiguration`
         """
-        super(Driver, self).configure()
-
-        # Create the SQLite database that will hold our cache attributes
-        self.initialize_db()
-
-    def initialize_db(self):
-        db = CONF.image_cache_sqlite_db
-        self.db_path = os.path.join(self.base_dir, db)
-        lockutils.set_defaults(self.base_dir)
-
-        @lockutils.synchronized('image_cache_db_init', external=True)
-        def create_db():
-            try:
-                conn = sqlite3.connect(self.db_path, check_same_thread=False,
-                                       factory=SqliteConnection)
-                conn.executescript("""
-                    CREATE TABLE IF NOT EXISTS cached_images (
-                        image_id TEXT PRIMARY KEY,
-                        last_accessed REAL DEFAULT 0.0,
-                        last_modified REAL DEFAULT 0.0,
-                        size INTEGER DEFAULT 0,
-                        hits INTEGER DEFAULT 0,
-                        checksum TEXT
-                    );
-                """)
-                conn.close()
-            except sqlite3.DatabaseError as e:
-                msg = _("Failed to initialize the image cache database. "
-                        "Got error: %s") % e
+        # Here we set up the various file-based image cache paths
+        # that we need in order to find the files in different states
+        # of cache management.
+        self.set_paths()
+
+        # We do a quick attempt to write a user xattr to a temporary file
+        # to check that the filesystem is even enabled to support xattrs
+        image_cache_dir = self.base_dir
+        fake_image_filepath = os.path.join(image_cache_dir, 'checkme')
+        with open(fake_image_filepath, 'wb') as fake_file:
+            fake_file.write(b"XXX")
+            fake_file.flush()
+        try:
+            set_xattr(fake_image_filepath, 'hits', '1')
+        except IOError as e:
+            if e.errno == errno.EOPNOTSUPP:
+                msg = (_("The device housing the image cache directory "
+                         "%(image_cache_dir)s does not support xattr. It is"
+                         " likely you need to edit your fstab and add the "
+                         "user_xattr option to the appropriate line for the"
+                         " device housing the cache directory.") %
+                       {'image_cache_dir': image_cache_dir})
                 LOG.error(msg)
-                raise exception.BadDriverConfiguration(driver_name='sqlite',
+                raise exception.BadDriverConfiguration(driver_name="xattr",
                                                        reason=msg)
-
-        create_db()
+        else:
+            # Cleanup after ourselves...
+            fileutils.delete_if_exists(fake_image_filepath)
 
     def get_cache_size(self):
         """
         Returns the total size in bytes of the image cache.
         """
         sizes = []
-        for path in self.get_cache_files(self.base_dir):
-            if path == self.db_path:
-                continue
+        for path in get_all_regular_files(self.base_dir):
             file_info = os.stat(path)
             sizes.append(file_info[stat.ST_SIZE])
         return sum(sizes)
 
     def get_hit_count(self, image_id):
         """
         Return the number of hits that an image has.
 
         :param image_id: Opaque image identifier
         """
         if not self.is_cached(image_id):
             return 0
 
-        hits = 0
-        with self.get_db() as db:
-            cur = db.execute("""SELECT hits FROM cached_images
-                             WHERE image_id = ?""",
-                             (image_id,))
-            hits = cur.fetchone()[0]
-        return hits
+        path = self.get_image_filepath(image_id)
+        return int(get_xattr(path, 'hits', default=0))
 
     def get_cached_images(self):
         """
         Returns a list of records about cached images.
         """
         LOG.debug("Gathering cached image entries.")
-        with self.get_db() as db:
-            cur = db.execute("""SELECT
-                             image_id, hits, last_accessed, last_modified, size
-                             FROM cached_images
-                             ORDER BY image_id""")
-            cur.row_factory = dict_factory
-            return [r for r in cur]
+        entries = []
+        for path in get_all_regular_files(self.base_dir):
+            image_id = os.path.basename(path)
+
+            entry = {'image_id': image_id}
+            file_info = os.stat(path)
+            entry['last_modified'] = file_info[stat.ST_MTIME]
+            entry['last_accessed'] = file_info[stat.ST_ATIME]
+            entry['size'] = file_info[stat.ST_SIZE]
+            entry['hits'] = self.get_hit_count(image_id)
+
+            entries.append(entry)
+        return entries
 
     def is_cached(self, image_id):
         """
         Returns True if the image with the supplied ID has its image
         file cached.
 
         :param image_id: Image ID
@@ -217,151 +185,114 @@
         """
         path = self.get_image_filepath(image_id, 'incomplete')
         return os.path.exists(path)
 
     def is_queued(self, image_id):
         """
         Returns True if the image identifier is in our cache queue.
-
-        :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id, 'queue')
         return os.path.exists(path)
 
     def delete_all_cached_images(self):
         """
         Removes all cached image files and any attributes about the images
         """
         deleted = 0
-        with self.get_db() as db:
-            for path in self.get_cache_files(self.base_dir):
-                delete_cached_file(path)
-                deleted += 1
-            db.execute("""DELETE FROM cached_images""")
-            db.commit()
+        for path in get_all_regular_files(self.base_dir):
+            delete_cached_file(path)
+            deleted += 1
         return deleted
 
     def delete_cached_image(self, image_id):
         """
         Removes a specific cached image file and any attributes about the image
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id)
-        with self.get_db() as db:
-            delete_cached_file(path)
-            db.execute("""DELETE FROM cached_images WHERE image_id = ?""",
-                       (image_id, ))
-            db.commit()
+        delete_cached_file(path)
 
     def delete_all_queued_images(self):
         """
         Removes all queued image files and any attributes about the images
         """
-        files = [f for f in self.get_cache_files(self.queue_dir)]
+        files = [f for f in get_all_regular_files(self.queue_dir)]
         for file in files:
             fileutils.delete_if_exists(file)
         return len(files)
 
     def delete_queued_image(self, image_id):
         """
         Removes a specific queued image file and any attributes about the image
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id, 'queue')
         fileutils.delete_if_exists(path)
 
-    def clean(self, stall_time=None):
-        """
-        Delete any image files in the invalid directory and any
-        files in the incomplete directory that are older than a
-        configurable amount of time.
-        """
-        self.delete_invalid_files()
-
-        if stall_time is None:
-            stall_time = CONF.image_cache_stall_time
-
-        now = time.time()
-        older_than = now - stall_time
-        self.delete_stalled_files(older_than)
-
     def get_least_recently_accessed(self):
         """
         Return a tuple containing the image_id and size of the least recently
         accessed cached file, or None if no cached files.
         """
-        with self.get_db() as db:
-            cur = db.execute("""SELECT image_id FROM cached_images
-                             ORDER BY last_accessed LIMIT 1""")
-            try:
-                image_id = cur.fetchone()[0]
-            except TypeError:
-                # There are no more cached images
-                return None
-
-        path = self.get_image_filepath(image_id)
-        try:
+        stats = []
+        for path in get_all_regular_files(self.base_dir):
             file_info = os.stat(path)
-            size = file_info[stat.ST_SIZE]
-        except OSError:
-            size = 0
-        return image_id, size
+            stats.append((file_info[stat.ST_ATIME],  # access time
+                          file_info[stat.ST_SIZE],   # size in bytes
+                          path))                     # absolute path
+
+        if not stats:
+            return None
+
+        stats.sort()
+        return os.path.basename(stats[0][2]), stats[0][1]
 
     @contextmanager
     def open_for_write(self, image_id):
         """
         Open a file for writing the image file for an image
         with supplied identifier.
 
         :param image_id: Image ID
         """
         incomplete_path = self.get_image_filepath(image_id, 'incomplete')
 
+        def set_attr(key, value):
+            set_xattr(incomplete_path, key, value)
+
         def commit():
-            with self.get_db() as db:
-                final_path = self.get_image_filepath(image_id)
-                LOG.debug("Fetch finished, moving "
-                          "'%(incomplete_path)s' to '%(final_path)s'",
-                          dict(incomplete_path=incomplete_path,
-                               final_path=final_path))
-                os.rename(incomplete_path, final_path)
-
-                # Make sure that we "pop" the image from the queue...
-                if self.is_queued(image_id):
-                    fileutils.delete_if_exists(
-                        self.get_image_filepath(image_id, 'queue'))
-
-                filesize = os.path.getsize(final_path)
-                now = time.time()
-
-                db.execute("""INSERT INTO cached_images
-                           (image_id, last_accessed, last_modified, hits, size)
-                           VALUES (?, ?, ?, 0, ?)""",
-                           (image_id, now, now, filesize))
-                db.commit()
+            set_attr('hits', 0)
+
+            final_path = self.get_image_filepath(image_id)
+            LOG.debug("Fetch finished, moving "
+                      "'%(incomplete_path)s' to '%(final_path)s'",
+                      dict(incomplete_path=incomplete_path,
+                           final_path=final_path))
+            os.rename(incomplete_path, final_path)
+
+            # Make sure that we "pop" the image from the queue...
+            if self.is_queued(image_id):
+                LOG.debug("Removing image '%s' from queue after "
+                          "caching it.", image_id)
+                fileutils.delete_if_exists(
+                    self.get_image_filepath(image_id, 'queue'))
 
         def rollback(e):
-            with self.get_db() as db:
-                if os.path.exists(incomplete_path):
-                    invalid_path = self.get_image_filepath(image_id, 'invalid')
-
-                    msg = (_LW("Fetch of cache file failed (%(e)s), rolling "
-                               "back by moving '%(incomplete_path)s' to "
-                               "'%(invalid_path)s'"),
-                           {'e': e,
-                            'incomplete_path': incomplete_path,
-                            'invalid_path': invalid_path})
-                    LOG.warning(msg)
-                    os.rename(incomplete_path, invalid_path)
-
-                db.execute("""DELETE FROM cached_images
-                           WHERE image_id = ?""", (image_id, ))
-                db.commit()
+            set_attr('error', encodeutils.exception_to_unicode(e))
+
+            invalid_path = self.get_image_filepath(image_id, 'invalid')
+            LOG.debug("Fetch of cache file failed (%(e)s), rolling back by "
+                      "moving '%(incomplete_path)s' to "
+                      "'%(invalid_path)s'",
+                      {'e': encodeutils.exception_to_unicode(e),
+                       'incomplete_path': incomplete_path,
+                       'invalid_path': invalid_path})
+            os.rename(incomplete_path, invalid_path)
 
         try:
             with open(incomplete_path, 'wb') as cache_file:
                 yield cache_file
         except Exception as e:
             with excutils.save_and_reraise_exception():
                 rollback(e)
@@ -383,44 +314,16 @@
         with supplied identifier.
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id)
         with open(path, 'rb') as cache_file:
             yield cache_file
-        now = time.time()
-        with self.get_db() as db:
-            db.execute("""UPDATE cached_images
-                       SET hits = hits + 1, last_accessed = ?
-                       WHERE image_id = ?""",
-                       (now, image_id))
-            db.commit()
-
-    @contextmanager
-    def get_db(self):
-        """
-        Returns a context manager that produces a database connection that
-        self-closes and calls rollback if an error occurs while using the
-        database connection
-        """
-        conn = sqlite3.connect(self.db_path, check_same_thread=False,
-                               factory=SqliteConnection)
-        conn.row_factory = sqlite3.Row
-        conn.text_factory = str
-        conn.execute('PRAGMA synchronous = NORMAL')
-        conn.execute('PRAGMA count_changes = OFF')
-        conn.execute('PRAGMA temp_store = MEMORY')
-        try:
-            yield conn
-        except sqlite3.DatabaseError as e:
-            msg = _LE("Error executing SQLite call. Got error: %s") % e
-            LOG.error(msg)
-            conn.rollback()
-        finally:
-            conn.close()
+        path = self.get_image_filepath(image_id)
+        inc_xattr(path, 'hits', 1)
 
     def queue_image(self, image_id):
         """
         This adds a image to be cache to the queue.
 
         If the image already exists in the queue or has already been
         cached, we return False, True otherwise
@@ -437,71 +340,157 @@
             return False
 
         if self.is_queued(image_id):
             LOG.info(_LI("Not queueing image '%s'. Already queued."), image_id)
             return False
 
         path = self.get_image_filepath(image_id, 'queue')
+        LOG.debug("Queueing image '%s'.", image_id)
 
         # Touch the file to add it to the queue
         with open(path, "w"):
             pass
 
         return True
 
-    def delete_invalid_files(self):
-        """
-        Removes any invalid cache entries
-        """
-        for path in self.get_cache_files(self.invalid_dir):
-            fileutils.delete_if_exists(path)
-            LOG.info(_LI("Removed invalid cache file %s"), path)
-
-    def delete_stalled_files(self, older_than):
-        """
-        Removes any incomplete cache entries older than a
-        supplied modified time.
-
-        :param older_than: Files written to on or before this timestamp
-                           will be deleted.
-        """
-        for path in self.get_cache_files(self.incomplete_dir):
-            if os.path.getmtime(path) < older_than:
-                try:
-                    fileutils.delete_if_exists(path)
-                    LOG.info(_LI("Removed stalled cache file %s"), path)
-                except Exception as e:
-                    msg = (_LW("Failed to delete file %(path)s. "
-                               "Got error: %(e)s"),
-                           dict(path=path, e=e))
-                    LOG.warning(msg)
-
     def get_queued_images(self):
         """
         Returns a list of image IDs that are in the queue. The
         list should be sorted by the time the image ID was inserted
         into the queue.
         """
-        files = [f for f in self.get_cache_files(self.queue_dir)]
+        files = [f for f in get_all_regular_files(self.queue_dir)]
         items = []
         for path in files:
             mtime = os.path.getmtime(path)
             items.append((mtime, os.path.basename(path)))
 
         items.sort()
         return [image_id for (modtime, image_id) in items]
 
-    def get_cache_files(self, basepath):
+    def _reap_old_files(self, dirpath, entry_type, grace=None):
+        now = time.time()
+        reaped = 0
+        for path in get_all_regular_files(dirpath):
+            mtime = os.path.getmtime(path)
+            age = now - mtime
+            if not grace:
+                LOG.debug("No grace period, reaping '%(path)s'"
+                          " immediately", {'path': path})
+                delete_cached_file(path)
+                reaped += 1
+            elif age > grace:
+                LOG.debug("Cache entry '%(path)s' exceeds grace period, "
+                          "(%(age)i s > %(grace)i s)",
+                          {'path': path, 'age': age, 'grace': grace})
+                delete_cached_file(path)
+                reaped += 1
+
+        LOG.info(_LI("Reaped %(reaped)s %(entry_type)s cache entries"),
+                 {'reaped': reaped, 'entry_type': entry_type})
+        return reaped
+
+    def reap_invalid(self, grace=None):
+        """Remove any invalid cache entries
+
+        :param grace: Number of seconds to keep an invalid entry around for
+                      debugging purposes. If None, then delete immediately.
+        """
+        return self._reap_old_files(self.invalid_dir, 'invalid', grace=grace)
+
+    def reap_stalled(self, grace=None):
+        """Remove any stalled cache entries
+
+        :param grace: Number of seconds to keep an invalid entry around for
+                      debugging purposes. If None, then delete immediately.
         """
-        Returns cache files in the supplied directory
+        return self._reap_old_files(self.incomplete_dir, 'stalled',
+                                    grace=grace)
 
-        :param basepath: Directory to look in for cache files
+    def clean(self, stall_time=None):
         """
-        for fname in os.listdir(basepath):
-            path = os.path.join(basepath, fname)
-            if path != self.db_path and os.path.isfile(path):
-                yield path
+        Delete any image files in the invalid directory and any
+        files in the incomplete directory that are older than a
+        configurable amount of time.
+        """
+        self.reap_invalid()
+
+        if stall_time is None:
+            stall_time = CONF.image_cache_stall_time
+
+        self.reap_stalled(stall_time)
+
+
+def get_all_regular_files(basepath):
+    for fname in os.listdir(basepath):
+        path = os.path.join(basepath, fname)
+        if os.path.isfile(path):
+            yield path
 
 
 def delete_cached_file(path):
     LOG.debug("Deleting image cache file '%s'", path)
     fileutils.delete_if_exists(path)
+
+
+def _make_namespaced_xattr_key(key, namespace='user'):
+    """
+    Create a fully-qualified xattr-key by including the intended namespace.
+
+    Namespacing differs among OSes[1]:
+
+        FreeBSD: user, system
+        Linux: user, system, trusted, security
+        MacOS X: not needed
+
+    Mac OS X won't break if we include a namespace qualifier, so, for
+    simplicity, we always include it.
+
+    --
+    [1] http://en.wikipedia.org/wiki/Extended_file_attributes
+    """
+    namespaced_key = ".".join([namespace, key])
+    return namespaced_key
+
+
+def get_xattr(path, key, **kwargs):
+    """Return the value for a particular xattr
+
+    If the key doesn't not exist, or xattrs aren't supported by the file
+    system then a KeyError will be raised, that is, unless you specify a
+    default using kwargs.
+    """
+    namespaced_key = _make_namespaced_xattr_key(key)
+    try:
+        return xattr.getxattr(path, namespaced_key)
+    except IOError:
+        if 'default' in kwargs:
+            return kwargs['default']
+        else:
+            raise
+
+
+def set_xattr(path, key, value):
+    """Set the value of a specified xattr.
+
+    If xattrs aren't supported by the file-system, we skip setting the value.
+    """
+    namespaced_key = _make_namespaced_xattr_key(key)
+    if not isinstance(value, bytes):
+        value = str(value).encode('utf-8')
+    xattr.setxattr(path, namespaced_key, value)
+
+
+def inc_xattr(path, key, n=1):
+    """
+    Increment the value of an xattr (assuming it is an integer).
+
+    BEWARE, this code *does* have a RACE CONDITION, since the
+    read/update/write sequence is not atomic.
+
+    Since the use-case for this function is collecting stats--not critical--
+    the benefits of simple, lock-free code out-weighs the possibility of an
+    occasional hit not being counted.
+    """
+    count = int(get_xattr(path, key))
+    count += n
+    set_xattr(path, key, str(count))
```

### Comparing `glance-28.0.0.0b2/glance/image_cache/drivers/xattr.py` & `glance-28.0.0.0rc1/glance/image_cache/drivers/sqlite.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,70 +10,68 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 """
-Cache driver that uses xattr file tags and requires a filesystem
-that has atimes set.
-
-Assumptions
-===========
-
-1. Cache data directory exists on a filesystem that updates atime on
-   reads ('noatime' should NOT be set)
-
-2. Cache data directory exists on a filesystem that supports xattrs.
-   This is optional, but highly recommended since it allows us to
-   present ops with useful information pertaining to the cache, like
-   human readable filenames and statistics.
-
-3. `glance-prune` is scheduled to run as a periodic job via cron. This
-    is needed to run the LRU prune strategy to keep the cache size
-    within the limits set by the config file.
-
-
-Cache Directory Notes
-=====================
-
-The image cache data directory contains the main cache path, where the
-active cache entries and subdirectories for handling partial downloads
-and errored-out cache images.
-
-The layout looks like:
-
-$image_cache_dir/
-  entry1
-  entry2
-  ...
-  incomplete/
-  invalid/
-  queue/
+Cache driver that uses SQLite to store information about cached images
 """
 from contextlib import contextmanager
-import errno
 import os
+import sqlite3
 import stat
 import time
 
+from oslo_concurrency import lockutils
 from oslo_config import cfg
 from oslo_log import log as logging
-from oslo_utils import encodeutils
 from oslo_utils import excutils
 from oslo_utils import fileutils
-import xattr
 
 from glance.common import exception
-from glance.i18n import _, _LI
+from glance.i18n import _, _LI, _LW
 from glance.image_cache.drivers import base
+from glance.image_cache.drivers import common
+
 
 LOG = logging.getLogger(__name__)
 
+DEPRECATION_REASON = """
+As centralized database will now be used for image cache management, the use
+of `sqlite` database and driver will be dropped from 'E' (2025.1)
+development cycle.
+"""
+
+sqlite_opts = [
+    cfg.StrOpt('image_cache_sqlite_db', default='cache.db',
+               deprecated_for_removal=True,
+               deprecated_reason=DEPRECATION_REASON,
+               deprecated_since='Caracal (2024.1)',
+               help=_("""
+The relative path to sqlite file database that will be used for image cache
+management.
+
+This is a relative path to the sqlite file database that tracks the age and
+usage statistics of image cache. The path is relative to image cache base
+directory, specified by the configuration option ``image_cache_dir``.
+
+This is a lightweight database with just one table.
+
+Possible values:
+    * A valid relative path to sqlite file database
+
+Related options:
+    * ``image_cache_dir``
+
+""")),
+]
+
 CONF = cfg.CONF
+CONF.register_opts(sqlite_opts)
 
 
 class Driver(base.Driver):
 
     """
     Cache driver that uses xattr file tags and requires a filesystem
     that has atimes set.
@@ -82,83 +80,91 @@
     def configure(self):
         """
         Configure the driver to use the stored configuration options
         Any store that needs special configuration should implement
         this method. If the store was not able to successfully configure
         itself, it should raise `exception.BadDriverConfiguration`
         """
-        # Here we set up the various file-based image cache paths
-        # that we need in order to find the files in different states
-        # of cache management.
-        self.set_paths()
-
-        # We do a quick attempt to write a user xattr to a temporary file
-        # to check that the filesystem is even enabled to support xattrs
-        image_cache_dir = self.base_dir
-        fake_image_filepath = os.path.join(image_cache_dir, 'checkme')
-        with open(fake_image_filepath, 'wb') as fake_file:
-            fake_file.write(b"XXX")
-            fake_file.flush()
-        try:
-            set_xattr(fake_image_filepath, 'hits', '1')
-        except IOError as e:
-            if e.errno == errno.EOPNOTSUPP:
-                msg = (_("The device housing the image cache directory "
-                         "%(image_cache_dir)s does not support xattr. It is"
-                         " likely you need to edit your fstab and add the "
-                         "user_xattr option to the appropriate line for the"
-                         " device housing the cache directory.") %
-                       {'image_cache_dir': image_cache_dir})
+        LOG.warning(_(DEPRECATION_REASON))
+        super(Driver, self).configure()
+
+        # Create the SQLite database that will hold our cache attributes
+        self.initialize_db()
+
+    def initialize_db(self):
+        db = CONF.image_cache_sqlite_db
+        self.db_path = os.path.join(self.base_dir, db)
+        lockutils.set_defaults(self.base_dir)
+
+        @lockutils.synchronized('image_cache_db_init', external=True)
+        def create_db():
+            try:
+                conn = sqlite3.connect(self.db_path, check_same_thread=False,
+                                       factory=common.SqliteConnection)
+                conn.executescript("""
+                    CREATE TABLE IF NOT EXISTS cached_images (
+                        image_id TEXT PRIMARY KEY,
+                        last_accessed REAL DEFAULT 0.0,
+                        last_modified REAL DEFAULT 0.0,
+                        size INTEGER DEFAULT 0,
+                        hits INTEGER DEFAULT 0,
+                        checksum TEXT
+                    );
+                """)
+                conn.close()
+            except sqlite3.DatabaseError as e:
+                msg = _("Failed to initialize the image cache database. "
+                        "Got error: %s") % e
                 LOG.error(msg)
-                raise exception.BadDriverConfiguration(driver_name="xattr",
+                raise exception.BadDriverConfiguration(driver_name='sqlite',
                                                        reason=msg)
-        else:
-            # Cleanup after ourselves...
-            fileutils.delete_if_exists(fake_image_filepath)
+
+        create_db()
 
     def get_cache_size(self):
         """
         Returns the total size in bytes of the image cache.
         """
         sizes = []
-        for path in get_all_regular_files(self.base_dir):
+        for path in self.get_cache_files(self.base_dir):
+            if path == self.db_path:
+                continue
             file_info = os.stat(path)
             sizes.append(file_info[stat.ST_SIZE])
         return sum(sizes)
 
     def get_hit_count(self, image_id):
         """
         Return the number of hits that an image has.
 
         :param image_id: Opaque image identifier
         """
         if not self.is_cached(image_id):
             return 0
 
-        path = self.get_image_filepath(image_id)
-        return int(get_xattr(path, 'hits', default=0))
+        hits = 0
+        with common.get_db(self.db_path) as db:
+            cur = db.execute("""SELECT hits FROM cached_images
+                             WHERE image_id = ?""",
+                             (image_id,))
+            hits = cur.fetchone()[0]
+        return hits
 
     def get_cached_images(self):
         """
         Returns a list of records about cached images.
         """
         LOG.debug("Gathering cached image entries.")
-        entries = []
-        for path in get_all_regular_files(self.base_dir):
-            image_id = os.path.basename(path)
-
-            entry = {'image_id': image_id}
-            file_info = os.stat(path)
-            entry['last_modified'] = file_info[stat.ST_MTIME]
-            entry['last_accessed'] = file_info[stat.ST_ATIME]
-            entry['size'] = file_info[stat.ST_SIZE]
-            entry['hits'] = self.get_hit_count(image_id)
-
-            entries.append(entry)
-        return entries
+        with common.get_db(self.db_path) as db:
+            cur = db.execute("""SELECT
+                             image_id, hits, last_accessed, last_modified, size
+                             FROM cached_images
+                             ORDER BY image_id""")
+            cur.row_factory = common.dict_factory
+            return [r for r in cur]
 
     def is_cached(self, image_id):
         """
         Returns True if the image with the supplied ID has its image
         file cached.
 
         :param image_id: Image ID
@@ -185,114 +191,151 @@
         """
         path = self.get_image_filepath(image_id, 'incomplete')
         return os.path.exists(path)
 
     def is_queued(self, image_id):
         """
         Returns True if the image identifier is in our cache queue.
+
+        :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id, 'queue')
         return os.path.exists(path)
 
     def delete_all_cached_images(self):
         """
         Removes all cached image files and any attributes about the images
         """
         deleted = 0
-        for path in get_all_regular_files(self.base_dir):
-            delete_cached_file(path)
-            deleted += 1
+        with common.get_db(self.db_path) as db:
+            for path in self.get_cache_files(self.base_dir):
+                delete_cached_file(path)
+                deleted += 1
+            db.execute("""DELETE FROM cached_images""")
+            db.commit()
         return deleted
 
     def delete_cached_image(self, image_id):
         """
         Removes a specific cached image file and any attributes about the image
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id)
-        delete_cached_file(path)
+        with common.get_db(self.db_path) as db:
+            delete_cached_file(path)
+            db.execute("""DELETE FROM cached_images WHERE image_id = ?""",
+                       (image_id, ))
+            db.commit()
 
     def delete_all_queued_images(self):
         """
         Removes all queued image files and any attributes about the images
         """
-        files = [f for f in get_all_regular_files(self.queue_dir)]
+        files = [f for f in self.get_cache_files(self.queue_dir)]
         for file in files:
             fileutils.delete_if_exists(file)
         return len(files)
 
     def delete_queued_image(self, image_id):
         """
         Removes a specific queued image file and any attributes about the image
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id, 'queue')
         fileutils.delete_if_exists(path)
 
+    def clean(self, stall_time=None):
+        """
+        Delete any image files in the invalid directory and any
+        files in the incomplete directory that are older than a
+        configurable amount of time.
+        """
+        self.delete_invalid_files()
+
+        if stall_time is None:
+            stall_time = CONF.image_cache_stall_time
+
+        now = time.time()
+        older_than = now - stall_time
+        self.delete_stalled_files(older_than)
+
     def get_least_recently_accessed(self):
         """
         Return a tuple containing the image_id and size of the least recently
         accessed cached file, or None if no cached files.
         """
-        stats = []
-        for path in get_all_regular_files(self.base_dir):
-            file_info = os.stat(path)
-            stats.append((file_info[stat.ST_ATIME],  # access time
-                          file_info[stat.ST_SIZE],   # size in bytes
-                          path))                     # absolute path
-
-        if not stats:
-            return None
+        with common.get_db(self.db_path) as db:
+            cur = db.execute("""SELECT image_id FROM cached_images
+                             ORDER BY last_accessed LIMIT 1""")
+            try:
+                image_id = cur.fetchone()[0]
+            except TypeError:
+                # There are no more cached images
+                return None
 
-        stats.sort()
-        return os.path.basename(stats[0][2]), stats[0][1]
+        path = self.get_image_filepath(image_id)
+        try:
+            file_info = os.stat(path)
+            size = file_info[stat.ST_SIZE]
+        except OSError:
+            size = 0
+        return image_id, size
 
     @contextmanager
     def open_for_write(self, image_id):
         """
         Open a file for writing the image file for an image
         with supplied identifier.
 
         :param image_id: Image ID
         """
         incomplete_path = self.get_image_filepath(image_id, 'incomplete')
 
-        def set_attr(key, value):
-            set_xattr(incomplete_path, key, value)
-
         def commit():
-            set_attr('hits', 0)
-
-            final_path = self.get_image_filepath(image_id)
-            LOG.debug("Fetch finished, moving "
-                      "'%(incomplete_path)s' to '%(final_path)s'",
-                      dict(incomplete_path=incomplete_path,
-                           final_path=final_path))
-            os.rename(incomplete_path, final_path)
-
-            # Make sure that we "pop" the image from the queue...
-            if self.is_queued(image_id):
-                LOG.debug("Removing image '%s' from queue after "
-                          "caching it.", image_id)
-                fileutils.delete_if_exists(
-                    self.get_image_filepath(image_id, 'queue'))
+            with common.get_db(self.db_path) as db:
+                final_path = self.get_image_filepath(image_id)
+                LOG.debug("Fetch finished, moving "
+                          "'%(incomplete_path)s' to '%(final_path)s'",
+                          dict(incomplete_path=incomplete_path,
+                               final_path=final_path))
+                os.rename(incomplete_path, final_path)
+
+                # Make sure that we "pop" the image from the queue...
+                if self.is_queued(image_id):
+                    fileutils.delete_if_exists(
+                        self.get_image_filepath(image_id, 'queue'))
+
+                filesize = os.path.getsize(final_path)
+                now = time.time()
+
+                db.execute("""INSERT INTO cached_images
+                           (image_id, last_accessed, last_modified, hits, size)
+                           VALUES (?, ?, ?, 0, ?)""",
+                           (image_id, now, now, filesize))
+                db.commit()
 
         def rollback(e):
-            set_attr('error', encodeutils.exception_to_unicode(e))
-
-            invalid_path = self.get_image_filepath(image_id, 'invalid')
-            LOG.debug("Fetch of cache file failed (%(e)s), rolling back by "
-                      "moving '%(incomplete_path)s' to "
-                      "'%(invalid_path)s'",
-                      {'e': encodeutils.exception_to_unicode(e),
-                       'incomplete_path': incomplete_path,
-                       'invalid_path': invalid_path})
-            os.rename(incomplete_path, invalid_path)
+            with common.get_db(self.db_path) as db:
+                if os.path.exists(incomplete_path):
+                    invalid_path = self.get_image_filepath(image_id, 'invalid')
+
+                    msg = (_LW("Fetch of cache file failed (%(e)s), rolling "
+                               "back by moving '%(incomplete_path)s' to "
+                               "'%(invalid_path)s'"),
+                           {'e': e,
+                            'incomplete_path': incomplete_path,
+                            'invalid_path': invalid_path})
+                    LOG.warning(msg)
+                    os.rename(incomplete_path, invalid_path)
+
+                db.execute("""DELETE FROM cached_images
+                           WHERE image_id = ?""", (image_id, ))
+                db.commit()
 
         try:
             with open(incomplete_path, 'wb') as cache_file:
                 yield cache_file
         except Exception as e:
             with excutils.save_and_reraise_exception():
                 rollback(e)
@@ -314,16 +357,21 @@
         with supplied identifier.
 
         :param image_id: Image ID
         """
         path = self.get_image_filepath(image_id)
         with open(path, 'rb') as cache_file:
             yield cache_file
-        path = self.get_image_filepath(image_id)
-        inc_xattr(path, 'hits', 1)
+        now = time.time()
+        with common.get_db(self.db_path) as db:
+            db.execute("""UPDATE cached_images
+                       SET hits = hits + 1, last_accessed = ?
+                       WHERE image_id = ?""",
+                       (now, image_id))
+            db.commit()
 
     def queue_image(self, image_id):
         """
         This adds a image to be cache to the queue.
 
         If the image already exists in the queue or has already been
         cached, we return False, True otherwise
@@ -340,157 +388,71 @@
             return False
 
         if self.is_queued(image_id):
             LOG.info(_LI("Not queueing image '%s'. Already queued."), image_id)
             return False
 
         path = self.get_image_filepath(image_id, 'queue')
-        LOG.debug("Queueing image '%s'.", image_id)
 
         # Touch the file to add it to the queue
         with open(path, "w"):
             pass
 
         return True
 
+    def delete_invalid_files(self):
+        """
+        Removes any invalid cache entries
+        """
+        for path in self.get_cache_files(self.invalid_dir):
+            fileutils.delete_if_exists(path)
+            LOG.info(_LI("Removed invalid cache file %s"), path)
+
+    def delete_stalled_files(self, older_than):
+        """
+        Removes any incomplete cache entries older than a
+        supplied modified time.
+
+        :param older_than: Files written to on or before this timestamp
+                           will be deleted.
+        """
+        for path in self.get_cache_files(self.incomplete_dir):
+            if os.path.getmtime(path) < older_than:
+                try:
+                    fileutils.delete_if_exists(path)
+                    LOG.info(_LI("Removed stalled cache file %s"), path)
+                except Exception as e:
+                    msg = (_LW("Failed to delete file %(path)s. "
+                               "Got error: %(e)s"),
+                           dict(path=path, e=e))
+                    LOG.warning(msg)
+
     def get_queued_images(self):
         """
         Returns a list of image IDs that are in the queue. The
         list should be sorted by the time the image ID was inserted
         into the queue.
         """
-        files = [f for f in get_all_regular_files(self.queue_dir)]
+        files = [f for f in self.get_cache_files(self.queue_dir)]
         items = []
         for path in files:
             mtime = os.path.getmtime(path)
             items.append((mtime, os.path.basename(path)))
 
         items.sort()
         return [image_id for (modtime, image_id) in items]
 
-    def _reap_old_files(self, dirpath, entry_type, grace=None):
-        now = time.time()
-        reaped = 0
-        for path in get_all_regular_files(dirpath):
-            mtime = os.path.getmtime(path)
-            age = now - mtime
-            if not grace:
-                LOG.debug("No grace period, reaping '%(path)s'"
-                          " immediately", {'path': path})
-                delete_cached_file(path)
-                reaped += 1
-            elif age > grace:
-                LOG.debug("Cache entry '%(path)s' exceeds grace period, "
-                          "(%(age)i s > %(grace)i s)",
-                          {'path': path, 'age': age, 'grace': grace})
-                delete_cached_file(path)
-                reaped += 1
-
-        LOG.info(_LI("Reaped %(reaped)s %(entry_type)s cache entries"),
-                 {'reaped': reaped, 'entry_type': entry_type})
-        return reaped
-
-    def reap_invalid(self, grace=None):
-        """Remove any invalid cache entries
-
-        :param grace: Number of seconds to keep an invalid entry around for
-                      debugging purposes. If None, then delete immediately.
+    def get_cache_files(self, basepath):
         """
-        return self._reap_old_files(self.invalid_dir, 'invalid', grace=grace)
-
-    def reap_stalled(self, grace=None):
-        """Remove any stalled cache entries
+        Returns cache files in the supplied directory
 
-        :param grace: Number of seconds to keep an invalid entry around for
-                      debugging purposes. If None, then delete immediately.
+        :param basepath: Directory to look in for cache files
         """
-        return self._reap_old_files(self.incomplete_dir, 'stalled',
-                                    grace=grace)
-
-    def clean(self, stall_time=None):
-        """
-        Delete any image files in the invalid directory and any
-        files in the incomplete directory that are older than a
-        configurable amount of time.
-        """
-        self.reap_invalid()
-
-        if stall_time is None:
-            stall_time = CONF.image_cache_stall_time
-
-        self.reap_stalled(stall_time)
-
-
-def get_all_regular_files(basepath):
-    for fname in os.listdir(basepath):
-        path = os.path.join(basepath, fname)
-        if os.path.isfile(path):
-            yield path
+        for fname in os.listdir(basepath):
+            path = os.path.join(basepath, fname)
+            if path != self.db_path and os.path.isfile(path):
+                yield path
 
 
 def delete_cached_file(path):
     LOG.debug("Deleting image cache file '%s'", path)
     fileutils.delete_if_exists(path)
-
-
-def _make_namespaced_xattr_key(key, namespace='user'):
-    """
-    Create a fully-qualified xattr-key by including the intended namespace.
-
-    Namespacing differs among OSes[1]:
-
-        FreeBSD: user, system
-        Linux: user, system, trusted, security
-        MacOS X: not needed
-
-    Mac OS X won't break if we include a namespace qualifier, so, for
-    simplicity, we always include it.
-
-    --
-    [1] http://en.wikipedia.org/wiki/Extended_file_attributes
-    """
-    namespaced_key = ".".join([namespace, key])
-    return namespaced_key
-
-
-def get_xattr(path, key, **kwargs):
-    """Return the value for a particular xattr
-
-    If the key doesn't not exist, or xattrs aren't supported by the file
-    system then a KeyError will be raised, that is, unless you specify a
-    default using kwargs.
-    """
-    namespaced_key = _make_namespaced_xattr_key(key)
-    try:
-        return xattr.getxattr(path, namespaced_key)
-    except IOError:
-        if 'default' in kwargs:
-            return kwargs['default']
-        else:
-            raise
-
-
-def set_xattr(path, key, value):
-    """Set the value of a specified xattr.
-
-    If xattrs aren't supported by the file-system, we skip setting the value.
-    """
-    namespaced_key = _make_namespaced_xattr_key(key)
-    if not isinstance(value, bytes):
-        value = str(value).encode('utf-8')
-    xattr.setxattr(path, namespaced_key, value)
-
-
-def inc_xattr(path, key, n=1):
-    """
-    Increment the value of an xattr (assuming it is an integer).
-
-    BEWARE, this code *does* have a RACE CONDITION, since the
-    read/update/write sequence is not atomic.
-
-    Since the use-case for this function is collecting stats--not critical--
-    the benefits of simple, lock-free code out-weighs the possibility of an
-    occasional hit not being counted.
-    """
-    count = int(get_xattr(path, key))
-    count += n
-    set_xattr(path, key, str(count))
```

### Comparing `glance-28.0.0.0b2/glance/image_cache/prefetcher.py` & `glance-28.0.0.0rc1/glance/image_cache/prefetcher.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/image_cache/pruner.py` & `glance-28.0.0.0rc1/glance/image_cache/pruner.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/de/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/de/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/en_GB/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/en_GB/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/es/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/es/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/fr/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/fr/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/it/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/it/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/ja/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/ja/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/ko_KR/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/ko_KR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/pt_BR/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/pt_BR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/ru/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/ru/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/tr_TR/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/tr_TR/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/zh_CN/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/zh_CN/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/locale/zh_TW/LC_MESSAGES/glance.po` & `glance-28.0.0.0rc1/glance/locale/zh_TW/LC_MESSAGES/glance.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/location.py` & `glance-28.0.0.0rc1/glance/location.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/notifier.py` & `glance-28.0.0.0rc1/glance/notifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         'tags': list(image.tags),
         'deleted': False,
         'deleted_at': None,
     }
 
 
 def format_image_member_notification(image_member):
-    """Given a glance.domain.ImageMember object, return a dictionary of relevant
-    notification information.
+    """Given a glance.domain.ImageMember object, return a dictionary of
+    relevant notification information.
     """
     return {
         'image_id': image_member.image_id,
         'member_id': image_member.member_id,
         'status': image_member.status,
         'created_at': timeutils.isotime(image_member.created_at),
         'updated_at': timeutils.isotime(image_member.updated_at),
```

### Comparing `glance-28.0.0.0b2/glance/opts.py` & `glance-28.0.0.0rc1/glance/opts.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/__init__.py` & `glance-28.0.0.0rc1/glance/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/base.py` & `glance-28.0.0.0rc1/glance/policies/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     f'rule:context_is_admin or (role:member and {IMAGE_MEMBER_CHECK})'
 )
 ADMIN_OR_PROJECT_READER_OR_SHARED_MEMBER = (
     f'rule:context_is_admin or '
     f'role:reader and (project_id:%(project_id)s or {IMAGE_MEMBER_CHECK})'
 )
 
-ADMIN = f'rule:context_is_admin'
+ADMIN = 'rule:context_is_admin'
 
 rules = [
     policy.RuleDefault(name='default', check_str='',
                        description='Defines the default rule used for '
                                    'policies that historically had an empty '
                                    'policy in the supplied policy.json file.',
                        deprecated_rule=policy.DeprecatedRule(
```

### Comparing `glance-28.0.0.0b2/glance/policies/cache.py` & `glance-28.0.0.0rc1/glance/policies/cache.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/discovery.py` & `glance-28.0.0.0rc1/glance/policies/discovery.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/image.py` & `glance-28.0.0.0rc1/glance/policies/image.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/metadef.py` & `glance-28.0.0.0rc1/glance/policies/metadef.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/policies/tasks.py` & `glance-28.0.0.0rc1/glance/policies/tasks.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/quota/__init__.py` & `glance-28.0.0.0rc1/glance/quota/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/quota/keystone.py` & `glance-28.0.0.0rc1/glance/quota/keystone.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/schema.py` & `glance-28.0.0.0rc1/glance/schema.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/scrubber.py` & `glance-28.0.0.0rc1/glance/scrubber.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,27 +16,37 @@
 import calendar
 import time
 
 import eventlet
 from glance_store import exceptions as store_exceptions
 from oslo_config import cfg
 from oslo_log import log as logging
+from oslo_log import versionutils
 from oslo_utils import encodeutils
 
 from glance.common import crypt
 from glance.common import exception
 from glance.common import timeutils
 from glance import context
 import glance.db as db_api
 from glance.i18n import _, _LC, _LE, _LI, _LW
 
 LOG = logging.getLogger(__name__)
+DEPRECATED_SUBSTRING = ('is scheduled to be removed during the 2024.2 '
+                        '(Dalmatian) development cycle.')
+DEPRECATED_SCRUBBER_MSG = ('The glance scrubber has been deprecated and '
+                           + DEPRECATED_SUBSTRING)
+DEPRECATED_OPTS_MSG = ('The entire glance scrubber, including this option, '
+                       + DEPRECATED_SUBSTRING)
 
 scrubber_opts = [
     cfg.IntOpt('scrub_time', default=0, min=0,
+               deprecated_for_removal=True,
+               deprecated_since='2024.1 (Caracal)',
+               deprecated_reason=DEPRECATED_OPTS_MSG,
                help=_("""
 The amount of time, in seconds, to delay image scrubbing.
 
 When delayed delete is turned on, an image is put into ``pending_delete``
 state upon deletion until the scrubber deletes its image data. Typically, soon
 after the image is put into ``pending_delete`` state, it is available for
 scrubbing. However, scrubbing can be delayed until a later point using this
@@ -51,14 +61,17 @@
     * Any non-negative integer
 
 Related options:
     * ``delayed_delete``
 
 """)),
     cfg.IntOpt('scrub_pool_size', default=1, min=1,
+               deprecated_for_removal=True,
+               deprecated_since='2024.1 (Caracal)',
+               deprecated_reason=DEPRECATED_OPTS_MSG,
                help=_("""
 The size of thread pool to be used for scrubbing images.
 
 When there are a large number of images to scrub, it is beneficial to scrub
 images in parallel so that the scrub queue stays in control and the backend
 storage is reclaimed in a timely fashion. This configuration option denotes
 the maximum number of images to be scrubbed in parallel. The default value is
@@ -69,14 +82,17 @@
     * Any non-zero positive integer
 
 Related options:
     * ``delayed_delete``
 
 """)),
     cfg.BoolOpt('delayed_delete', default=False,
+                deprecated_for_removal=True,
+                deprecated_since='2024.1 (Caracal)',
+                deprecated_reason=DEPRECATED_OPTS_MSG,
                 help=_("""
 Turn on/off delayed delete.
 
 Typically when an image is deleted, the ``glance-api`` service puts the image
 into ``deleted`` state and deletes its data at the same time. Delayed delete
 is a feature in Glance that delays the actual deletion of image data until a
 later point in time (as determined by the configuration option ``scrub_time``).
@@ -100,14 +116,17 @@
     * ``scrub_pool_size``
 
 """)),
 ]
 
 scrubber_cmd_opts = [
     cfg.IntOpt('wakeup_time', default=300, min=0,
+               deprecated_for_removal=True,
+               deprecated_since='2024.1 (Caracal)',
+               deprecated_reason=DEPRECATED_OPTS_MSG,
                help=_("""
 Time interval, in seconds, between scrubber runs in daemon mode.
 
 Scrubber can be run either as a cron job or daemon. When run as a daemon, this
 configuration time specifies the time period between two runs. When the
 scrubber wakes up, it fetches and scrubs all ``pending_delete`` images that
 are available for scrubbing after taking ``scrub_time`` into consideration.
@@ -126,14 +145,17 @@
 """))
 ]
 
 scrubber_cmd_cli_opts = [
     cfg.BoolOpt('daemon',
                 short='D',
                 default=False,
+                deprecated_for_removal=True,
+                deprecated_since='2024.1 (Caracal)',
+                deprecated_reason=DEPRECATED_OPTS_MSG,
                 help=_("""
 Run scrubber as a daemon.
 
 This boolean configuration option indicates whether scrubber should
 run as a long-running process that wakes up at regular intervals to
 scrub images. The wake up interval can be specified using the
 configuration option ``wakeup_time``.
@@ -149,14 +171,17 @@
 
 Related options:
     * ``wakeup_time``
 
 """)),
     cfg.StrOpt('restore',
                metavar='<IMAGE_ID>',
+               deprecated_for_removal=True,
+               deprecated_since='2024.1 (Caracal)',
+               deprecated_reason=DEPRECATED_OPTS_MSG,
                help=_("""
 Restore the image status from 'pending_delete' to 'active'.
 
 This option is used by administrator to reset the image's status from
 'pending_delete' to 'active' when the image is deleted by mistake and
 'pending delete' feature is enabled in Glance. Please make sure the
 glance-scrubber daemon is stopped before restoring the image to avoid image
@@ -284,14 +309,15 @@
     if not _db_queue:
         _db_queue = ScrubDBQueue()
     return _db_queue
 
 
 class Daemon(object):
     def __init__(self, wakeup_time=300, threads=100):
+        versionutils.report_deprecated_feature(LOG, DEPRECATED_SCRUBBER_MSG)
         LOG.info(_LI("Starting Daemon: wakeup_time=%(wakeup_time)s "
                      "threads=%(threads)s"),
                  {'wakeup_time': wakeup_time, 'threads': threads})
         self.wakeup_time = wakeup_time
         self.event = eventlet.event.Event()
         # This pool is used for periodic instantiation of scrubber
         self.daemon_pool = eventlet.greenpool.GreenPool(threads)
@@ -311,14 +337,15 @@
         self.daemon_pool.spawn_n(application.run, self.event)
         eventlet.spawn_after(self.wakeup_time, self._run, application)
         LOG.debug("Next run scheduled in %s seconds", self.wakeup_time)
 
 
 class Scrubber(object):
     def __init__(self, store_api):
+        versionutils.report_deprecated_feature(LOG, DEPRECATED_SCRUBBER_MSG)
         LOG.info(_LI("Initializing scrubber"))
         self.store_api = store_api
         self.admin_context = context.get_admin_context(show_deleted=True)
         self.db_queue = get_scrub_queue()
         self.pool = eventlet.greenpool.GreenPool(CONF.scrub_pool_size)
 
     def _get_delete_jobs(self):
```

### Comparing `glance-28.0.0.0b2/glance/tests/__init__.py` & `glance-28.0.0.0rc1/glance/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/etc/glance-swift.conf` & `glance-28.0.0.0rc1/glance/tests/etc/glance-swift.conf`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/etc/property-protections-policies.conf` & `glance-28.0.0.0rc1/glance/tests/etc/property-protections-policies.conf`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/etc/property-protections.conf` & `glance-28.0.0.0rc1/glance/tests/etc/property-protections.conf`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/__init__.py` & `glance-28.0.0.0rc1/glance/tests/functional/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
         self.needs_database = False
         self.log_file = None
         self.sock = sock
         self.fork_socket = True
         self.process_pid = None
         self.server_module = None
         self.stop_kill = False
-        self.send_identity_credentials = False
 
     def write_conf(self, **kwargs):
         """
         Writes the configuration file for the server to its intended
         destination.  Returns the name of the configuration file and
         the over-ridden config content (may be useful for populating
         error messages).
@@ -177,16 +176,16 @@
         """Create database if required for this server"""
         if self.needs_database:
             conf_dir = os.path.join(self.test_dir, 'etc')
             utils.safe_mkdirs(conf_dir)
             conf_filepath = os.path.join(conf_dir, 'glance-manage.conf')
 
             with open(conf_filepath, 'w') as conf_file:
-                conf_file.write('[DEFAULT]\n')
-                conf_file.write('sql_connection = %s' % self.sql_connection)
+                conf_file.write('[database]\n')
+                conf_file.write('connection = %s' % self.sql_connection)
                 conf_file.flush()
 
             glance_db_env = 'GLANCE_DB_TEST_SQLITE_FILE'
             if glance_db_env in os.environ:
                 # use the empty db created and cached as a tempfile
                 # instead of spending the time creating a new one
                 db_location = os.environ[glance_db_env]
@@ -416,48 +415,45 @@
                                              default_sql_connection)
         self.user_storage_quota = '0'
         self.lock_path = self.test_dir
 
         self.location_strategy = 'location_order'
         self.store_type_location_strategy_preference = ""
 
-        self.send_identity_headers = False
-
         self.node_staging_uri = 'file://%s' % os.path.join(
             self.test_dir, 'staging')
 
         self.conf_base = """[DEFAULT]
 debug = %(debug)s
 default_log_levels = eventlet.wsgi.server=DEBUG,stevedore.extension=INFO
 bind_host = %(bind_host)s
 bind_port = %(bind_port)s
 metadata_encryption_key = %(metadata_encryption_key)s
-send_identity_credentials = %(send_identity_credentials)s
 log_file = %(log_file)s
 image_size_cap = %(image_size_cap)d
 delayed_delete = %(delayed_delete)s
 workers = %(workers)s
 scrub_time = %(scrub_time)s
-send_identity_headers = %(send_identity_headers)s
 image_cache_dir = %(image_cache_dir)s
 image_cache_driver = %(image_cache_driver)s
-sql_connection = %(sql_connection)s
 show_image_direct_url = %(show_image_direct_url)s
 show_multiple_locations = %(show_multiple_locations)s
 user_storage_quota = %(user_storage_quota)s
 lock_path = %(lock_path)s
 property_protection_file = %(property_protection_file)s
 property_protection_rule_format = %(property_protection_rule_format)s
 image_member_quota=%(image_member_quota)s
 image_property_quota=%(image_property_quota)s
 image_tag_quota=%(image_tag_quota)s
 image_location_quota=%(image_location_quota)s
 location_strategy=%(location_strategy)s
 allow_additional_image_properties = True
 node_staging_uri=%(node_staging_uri)s
+[database]
+connection = %(sql_connection)s
 [oslo_policy]
 policy_file = %(policy_file)s
 policy_default_rule = %(policy_default_rule)s
 enforce_new_defaults=%(enforce_new_defaults)s
 [paste_deploy]
 flavor = %(deployment_flavor)s
 [store_type_location_strategy]
@@ -609,45 +605,42 @@
                                              default_sql_connection)
         self.user_storage_quota = '0'
         self.lock_path = self.test_dir
 
         self.location_strategy = 'location_order'
         self.store_type_location_strategy_preference = ""
 
-        self.send_identity_headers = False
-
         self.conf_base = """[DEFAULT]
 debug = %(debug)s
 default_log_levels = eventlet.wsgi.server=DEBUG,stevedore.extension=INFO
 bind_host = %(bind_host)s
 bind_port = %(bind_port)s
 metadata_encryption_key = %(metadata_encryption_key)s
-send_identity_credentials = %(send_identity_credentials)s
 log_file = %(log_file)s
 image_size_cap = %(image_size_cap)d
 delayed_delete = %(delayed_delete)s
 workers = %(workers)s
 scrub_time = %(scrub_time)s
-send_identity_headers = %(send_identity_headers)s
 image_cache_dir = %(image_cache_dir)s
 image_cache_driver = %(image_cache_driver)s
-sql_connection = %(sql_connection)s
 show_image_direct_url = %(show_image_direct_url)s
 show_multiple_locations = %(show_multiple_locations)s
 user_storage_quota = %(user_storage_quota)s
 lock_path = %(lock_path)s
 property_protection_file = %(property_protection_file)s
 property_protection_rule_format = %(property_protection_rule_format)s
 image_member_quota=%(image_member_quota)s
 image_property_quota=%(image_property_quota)s
 image_tag_quota=%(image_tag_quota)s
 image_location_quota=%(image_location_quota)s
 location_strategy=%(location_strategy)s
 allow_additional_image_properties = True
 enabled_backends=file1:file,file2:file,file3:file
+[database]
+connection = %(sql_connection)s
 [oslo_policy]
 policy_file = %(policy_file)s
 policy_default_rule = %(policy_default_rule)s
 enforce_new_defaults=%(enforce_new_defaults)s
 [paste_deploy]
 flavor = %(deployment_flavor)s
 [store_type_location_strategy]
@@ -781,26 +774,25 @@
 
         default_sql_connection = SQLITE_CONN_TEMPLATE % self.test_dir
         self.sql_connection = os.environ.get('GLANCE_TEST_SQL_CONNECTION',
                                              default_sql_connection)
         self.policy_file = policy_file
         self.policy_default_rule = 'default'
 
-        self.send_identity_headers = False
-
         self.conf_base = """[DEFAULT]
 debug = %(debug)s
 log_file = %(log_file)s
 daemon = %(daemon)s
 wakeup_time = 2
 scrub_time = %(scrub_time)s
 metadata_encryption_key = %(metadata_encryption_key)s
 lock_path = %(lock_path)s
-sql_connection = %(sql_connection)s
 sql_idle_timeout = 3600
+[database]
+connection = %(sql_connection)s
 [glance_store]
 filesystem_store_datadir=%(image_dir)s
 [oslo_policy]
 policy_file = %(policy_file)s
 policy_default_rule = %(policy_default_rule)s
 """
 
@@ -834,15 +826,15 @@
         # Please disable it by explicitly setting 'self.include_scrubber' to
         # False in the test SetUps that do not require Scrubber to run.
         self.include_scrubber = True
 
         # The clients will try to connect to this address. Let's make sure
         # we're not using the default '0.0.0.0'
         self.config(bind_host='127.0.0.1')
-
+        self.config(image_cache_dir=self.test_dir)
         self.tracecmd = tracecmd_osmap.get(platform.system())
 
         conf_dir = os.path.join(self.test_dir, 'etc')
         utils.safe_mkdirs(conf_dir)
         self.copy_data_file('schema-image.json', conf_dir)
         self.copy_data_file('property-protections.conf', conf_dir)
         self.copy_data_file('property-protections-policies.conf', conf_dir)
@@ -1634,27 +1626,30 @@
     def setUp(self):
         super(SynchronousAPIBase, self).setUp()
 
         self.setup_database()
         self.setup_simple_paste()
         self.setup_stores()
 
-    def start_server(self, enable_cache=True):
+    def start_server(self, enable_cache=True, set_worker_url=True):
         """Builds and "starts" the API server.
 
         Note that this doesn't actually "start" anything like
         FunctionalTest does above, but that terminology is used here
         to make it seem like the same sort of pattern.
         """
         config.set_config_defaults()
         root_app = 'glance-api'
         if enable_cache:
             root_app = 'glance-api-cachemanagement'
             self.config(image_cache_dir=self._store_dir('cache'))
 
+        if set_worker_url:
+            self.config(worker_self_reference_url='http://workerx')
+
         self.api = config.load_paste_app(root_app,
                                          conf_file=self.paste_config)
         self.config(enforce_new_defaults=True,
                     group='oslo_policy')
         self.config(enforce_scope=True,
                     group='oslo_policy')
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/__init__.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/__init__.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/base.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2252,15 +2252,15 @@
             self.assertEqual('public', i['visibility'])
 
     def test_unknown_admin_is_public_false(self):
         images = self.db_api.image_get_all(self.admin_none_context,
                                            is_public=False)
         self.assertEqual(8, len(images))
         for i in images:
-            self.assertTrue(i['visibility'] in ['shared', 'private'])
+            self.assertIn(i['visibility'], ['shared', 'private'])
 
     def test_unknown_admin_is_public_none(self):
         images = self.db_api.image_get_all(self.admin_none_context)
         self.assertEqual(12, len(images))
 
     def test_unknown_admin_visibility_public(self):
         images = self.db_api.image_get_all(self.admin_none_context,
@@ -2306,16 +2306,15 @@
             self.assertEqual('public', i['visibility'])
 
     def test_known_admin_is_public_false(self):
         images = self.db_api.image_get_all(self.admin_context,
                                            is_public=False)
         self.assertEqual(9, len(images))
         for i in images:
-            self.assertTrue(i['visibility']
-                            in ['shared', 'private', 'community'])
+            self.assertIn(i['visibility'], ['shared', 'private', 'community'])
 
     def test_known_admin_is_public_none(self):
         images = self.db_api.image_get_all(self.admin_context)
         self.assertEqual(13, len(images))
 
     def test_admin_as_user_true(self):
         images = self.db_api.image_get_all(self.admin_context,
@@ -2425,16 +2424,15 @@
 
     def test_tenant1_is_public_false(self):
         images = self.db_api.image_get_all(self.tenant1_context,
                                            is_public=False)
         self.assertEqual(3, len(images))
         for i in images:
             self.assertEqual(i['owner'], self.tenant1)
-            self.assertTrue(i['visibility']
-                            in ['private', 'shared', 'community'])
+            self.assertIn(i['visibility'], ['private', 'shared', 'community'])
 
     def test_tenant1_is_public_none(self):
         images = self.db_api.image_get_all(self.tenant1_context)
         self.assertEqual(7, len(images))
         for i in images:
             if not ('public' == i['visibility']):
                 self.assertEqual(self.tenant1, i['owner'])
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/base_metadef.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/base_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_mitaka01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_mitaka02.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_mitaka02.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_contract01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_contract01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_expand01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_ocata_migrate01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_ocata_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_contract01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_contract01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_expand01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_pike_migrate01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_pike_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_rocky_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_rocky_expand02.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_rocky_expand02.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_train_migrate01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_train_migrate01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/migrations/test_wallaby_expand01.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/migrations/test_wallaby_expand01.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/test_migrations.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/db/test_sqlalchemy.py` & `glance-28.0.0.0rc1/glance/tests/functional/db/test_sqlalchemy.py`

 * *Files 21% similar despite different names*

```diff
@@ -170,14 +170,136 @@
 
     def setUp(self):
         db_tests.load(get_db, reset_db_metadef)
         super(TestMetadefSqlAlchemyDriver, self).setUp()
         self.addCleanup(db_tests.reset)
 
 
+class TestImageCacheOperations(base.TestDriver,
+                               base.FunctionalInitWrapper):
+
+    def setUp(self):
+        db_tests.load(get_db, reset_db)
+        super(TestImageCacheOperations, self).setUp()
+
+        self.addCleanup(db_tests.reset)
+
+        # Create two images
+        self.images = []
+        for num in range(0, 2):
+            size = 100
+            image = self.db_api.image_create(
+                self.adm_context,
+                {'status': 'active',
+                 'owner': self.adm_context.owner,
+                 'size': size,
+                 'name': 'test-%s-%i' % ('active', num)})
+            self.images.append(image)
+
+        # Create two node_references
+        self.node_references = [
+            self.db_api.node_reference_create(
+                self.adm_context, 'node_url_1'),
+            self.db_api.node_reference_create(
+                self.adm_context, 'node_url_2'),
+        ]
+
+        # Cache two images on node_url_1
+        for node in self.node_references:
+            if node['node_reference_url'] == 'node_url_2':
+                continue
+
+            for image in self.images:
+                self.db_api.insert_cache_details(
+                    self.adm_context, 'node_url_1',
+                    image['id'], image['size'], hits=3)
+
+    def test_node_reference_get_by_url(self):
+        node_reference = self.db_api.node_reference_get_by_url(
+            self.adm_context, 'node_url_1')
+        self.assertEqual('node_url_1',
+                         node_reference['node_reference_url'])
+
+    def test_node_reference_get_by_url_not_found(self):
+        self.assertRaises(exception.NotFound,
+                          self.db_api.node_reference_get_by_url,
+                          self.adm_context,
+                          'garbage_url')
+
+    def test_get_cached_images(self):
+        # Two images are cached on node 'node_url_1'
+        cached_images = self.db_api.get_cached_images(
+            self.adm_context, 'node_url_1')
+        self.assertEqual(2, len(cached_images))
+
+        # Nothing is cached on node 'node_url_2'
+        cached_images = self.db_api.get_cached_images(
+            self.adm_context, 'node_url_2')
+        self.assertEqual(0, len(cached_images))
+
+    def test_get_hit_count(self):
+        # Hit count will be 3 for image on node_url_1
+        hit_count = self.db_api.get_hit_count(
+            self.adm_context, self.images[0]['id'], 'node_url_1')
+        self.assertEqual(3, hit_count)
+
+        # Hit count will be 0 for image on node_url_2
+        hit_count = self.db_api.get_hit_count(
+            self.adm_context, self.images[0]['id'], 'node_url_2')
+        self.assertEqual(0, hit_count)
+
+    def test_delete_all_cached_images(self):
+        # delete all images from node_url_1
+        self.db_api.delete_all_cached_images(
+            self.adm_context, 'node_url_1')
+        # Verify all images are deleted
+        cached_images = self.db_api.get_cached_images(
+            self.adm_context, 'node_url_1')
+        self.assertEqual(0, len(cached_images))
+
+    def test_delete_cached_image(self):
+        # Delete cached image from node_url_1
+        self.db_api.delete_cached_image(
+            self.adm_context, self.images[0]['id'], 'node_url_1')
+
+        # verify that image is deleted
+        self.assertFalse(self.db_api.is_image_cached_for_node(
+            self.adm_context, 'node_url_1', self.images[0]['id']))
+
+    def test_get_least_recently_accessed(self):
+        recently_accessed = self.db_api.get_least_recently_accessed(
+            self.adm_context, 'node_url_1')
+        # Verify we get last cached image in response
+        self.assertEqual(self.images[0]['id'], recently_accessed)
+
+    def test_is_image_cached_for_node(self):
+        # Verify image is cached for node_url_1
+        self.assertTrue(self.db_api.is_image_cached_for_node(
+            self.adm_context, 'node_url_1', self.images[0]['id']))
+
+        # Verify image is not cached for node_url_2
+        self.assertFalse(self.db_api.is_image_cached_for_node(
+            self.adm_context, 'node_url_2', self.images[0]['id']))
+
+    def test_update_hit_count(self):
+        # Verify image on node_url_1 has 3 as hit count
+        hit_count = self.db_api.get_hit_count(
+            self.adm_context, self.images[0]['id'], 'node_url_1')
+        self.assertEqual(3, hit_count)
+
+        # Update the hit count of UUID1
+        self.db_api.update_hit_count(
+            self.adm_context, self.images[0]['id'], 'node_url_1')
+
+        # Verify hit count is now 4
+        hit_count = self.db_api.get_hit_count(
+            self.adm_context, self.images[0]['id'], 'node_url_1')
+        self.assertEqual(4, hit_count)
+
+
 class TestImageAtomicOps(base.TestDriver,
                          base.FunctionalInitWrapper):
 
     def setUp(self):
         db_tests.load(get_db, reset_db)
         super(TestImageAtomicOps, self).setUp()
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/ft_utils.py` & `glance-28.0.0.0rc1/glance/tests/functional/ft_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/serial/test_scrubber.py` & `glance-28.0.0.0rc1/glance/tests/functional/serial/test_scrubber.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 class TestScrubber(functional.FunctionalTest):
 
     """Test that delayed_delete works and the scrubber deletes"""
 
     def setUp(self):
         super(TestScrubber, self).setUp()
         self.api_server.deployment_flavor = 'noauth'
-        self.api_server.send_identity_credentials = True
         self.admin_context = context.get_admin_context(show_deleted=True)
-        CONF.set_override('sql_connection', self.api_server.sql_connection)
+        CONF.set_override('connection', self.api_server.sql_connection,
+                          group='database')
 
     def _headers(self, custom_headers=None):
         base_headers = {
             'X-Identity-Status': 'Confirmed',
             'X-Auth-Token': '932c5c84-02ac-4fe5-a9ba-620af0e2bb96',
             'X-User-Id': 'f9a41d13-0c13-47e9-bee2-ce4e8bfe958e',
             'X-Tenant-Id': uuids.TENANT1,
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/store_utils.py` & `glance-28.0.0.0rc1/glance/tests/functional/store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_api.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_api.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_cache_middleware.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_cache_middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -394,13 +394,12 @@
 
         self.inited = True
         self.disabled = False
 
         super(TestImageCacheSqlite, self).setUp()
 
         self.api_server.deployment_flavor = "caching"
-        self.api_server.send_identity_credentials = True
 
     def tearDown(self):
         super(TestImageCacheSqlite, self).tearDown()
         if os.path.exists(self.api_server.image_cache_dir):
             shutil.rmtree(self.api_server.image_cache_dir)
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_client_exceptions.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_client_exceptions.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_client_redirects.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_client_redirects.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_cors_middleware.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_cors_middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     the test suite in oslo_middleware.
     '''
 
     def setUp(self):
         super(TestCORSMiddleware, self).setUp()
         # Cleanup is handled in teardown of the parent class.
         self.api_server.deployment_flavor = "caching"
-        self.api_server.send_identity_credentials = True
         self.start_servers(**self.__dict__.copy())
         self.http = httplib2.Http()
         self.api_path = "http://%s:%d/v2/images" % ("127.0.0.1", self.api_port)
 
     def _headers(self, extra=None):
         headers = {
             'X-Identity-Status': 'Confirmed',
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_glance_manage.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_glance_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_gzip_middleware.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_gzip_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_healthcheck_middleware.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_healthcheck_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_logging.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_reload.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_reload.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_sqlite.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/test_wsgi.py` & `glance-28.0.0.0rc1/glance/tests/functional/test_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         # Should fail - connection timed out so we get nothing from the server
         self.assertFalse(get_request(delay=1.1))
 
 
 class StagingCleanupBase:
     def _configure_api_server(self):
         self.my_api_server.deployment_flavor = 'noauth'
-        self.my_api_server.send_identity_credentials = True
 
     def _url(self, path):
         return 'http://127.0.0.1:%d%s' % (self.api_port, path)
 
     def _headers(self, custom_headers=None):
         base_headers = {
             'X-Identity-Status': 'Confirmed',
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/metadef_base.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/metadef_base.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_cache_api.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_cache_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,17 @@
 
     def set_policy_rules(self, rules):
         self.policy.set_rules(
             oslo_policy.policy.Rules.from_dict(rules),
             overwrite=True)
 
     def start_server(self, enable_cache=True):
+        # NOTE(abhishekk): Once sqlite driver is removed, fix these tests
+        # to work with centralized_db driver
+        self.config(image_cache_driver='sqlite')
         with mock.patch.object(policy, 'Enforcer') as mock_enf:
             mock_enf.return_value = self.policy
             super(TestImageCache, self).start_server(enable_cache=enable_cache)
 
     def load_data(self):
         output = {}
         # Create 1 queued image as well for testing
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_cache_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_cache_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_discovery.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from glance.tests.functional.v2.test_images import get_enforcer_class
 from glance.tests import utils as test_utils
 
 
 class TestDiscovery(functional.SynchronousAPIBase):
     def setUp(self):
         super(TestDiscovery, self).setUp()
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
 
         self.enforcer_mock = self.useFixture(
             fixtures.MockPatchObject(ks_quota, 'limit')).mock
 
     def set_limit(self, limits):
         self.enforcer_mock.Enforcer = get_enforcer_class(limits)
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_images.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_images.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,14 @@
         self.include_scrubber = False
         self.api_server.deployment_flavor = 'noauth'
         for i in range(3):
             ret = test_utils.start_http_server("foo_image_id%d" % i,
                                                "foo_image%d" % i)
             setattr(self, 'http_server%d' % i, ret[1])
             setattr(self, 'http_port%d' % i, ret[2])
-        self.api_server.send_identity_credentials = True
 
     def tearDown(self):
         for i in range(3):
             httpd = getattr(self, 'http_server%d' % i, None)
             if httpd:
                 httpd.shutdown()
                 httpd.server_close()
@@ -3736,15 +3735,14 @@
         base_headers.update(custom_headers or {})
         return base_headers
 
     def test_image_list_ipv6(self):
         # Image list should be empty
 
         self.api_server.deployment_flavor = "caching"
-        self.api_server.send_identity_credentials = True
         self.start_servers(**self.__dict__.copy())
 
         url = f'http://[::1]:{self.api_port}'
         path = '/'
         requests.get(url + path, headers=self._headers())
 
         path = '/v2/images'
@@ -6931,25 +6929,25 @@
         resp = requests.Response()
         resp.status_code = 202
         resp.headers['x-openstack-request-id'] = 'req-remote'
         self.ksa_client.return_value.post.return_value = resp
 
         # Stage it on worker1
         self.config(worker_self_reference_url='http://worker1')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         image_id = self._create_and_stage()
 
         # Make sure we can't see the stage host key
         image = self.api_get('/v2/images/%s' % image_id).json
         self.assertIn('container_format', image)
         self.assertNotIn('os_glance_stage_host', image)
 
         # Import call goes to worker2
         self.config(worker_self_reference_url='http://worker2')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         r = self._import_direct(image_id, ['store1'])
 
         # Assert that it was proxied back to worker1
         self.assertEqual(202, r.status_code)
         self.assertEqual('req-remote', r.headers['x-openstack-request-id'])
         self.ksa_client.return_value.post.assert_called_once_with(
             'http://worker1/v2/images/%s/import' % image_id,
@@ -6964,20 +6962,20 @@
         resp.status_code = 409
         resp.reason = 'Something Failed (tm)'
         self.ksa_client.return_value.post.return_value = resp
         self.ksa_client.return_value.delete.return_value = resp
 
         # Stage it on worker1
         self.config(worker_self_reference_url='http://worker1')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         image_id = self._create_and_stage()
 
         # Import call goes to worker2
         self.config(worker_self_reference_url='http://worker2')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         r = self._import_direct(image_id, ['store1'])
 
         # Make sure we see the relevant details from worker1
         self.assertEqual(409, r.status_code)
         self.assertEqual('409 Something Failed (tm)', r.status)
 
         # For a 40x, we should get the same on delete
@@ -6987,20 +6985,20 @@
 
     def _test_import_proxy_fail_requests(self, error, status):
         self.ksa_client.return_value.post.side_effect = error
         self.ksa_client.return_value.delete.side_effect = error
 
         # Stage it on worker1
         self.config(worker_self_reference_url='http://worker1')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         image_id = self._create_and_stage()
 
         # Import call goes to worker2
         self.config(worker_self_reference_url='http://worker2')
-        self.start_server()
+        self.start_server(set_worker_url=False)
         r = self._import_direct(image_id, ['store1'])
         self.assertEqual(status, r.status)
         self.assertIn(b'Stage host is unavailable', r.body)
 
         # Make sure we can still delete it
         r = self.api_delete('/v2/images/%s' % image_id)
         self.assertEqual(204, r.status_code)
@@ -7046,14 +7044,15 @@
 
     return FakeEnforcer
 
 
 class TestKeystoneQuotas(functional.SynchronousAPIBase):
     def setUp(self):
         super(TestKeystoneQuotas, self).setUp()
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         self.config(filesystem_store_datadir='/tmp/foo',
                     group='os_glance_tasks_store')
 
         self.enforcer_mock = self.useFixture(
             fixtures.MockPatchObject(ks_quota, 'limit')).mock
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_images_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_images_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_images_import_locking.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_images_import_locking.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_legacy_update_cinder_store.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_legacy_update_cinder_store.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_member_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_member_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_namespace_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_namespace_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_namespaces.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_namespaces.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_object_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_object_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_objects.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
         # Simple key values
         checked_values = set([
             'name',
             'description',
         ])
         for key, value in expected_metadata_object.items():
-            if(key in checked_values):
+            if key in checked_values:
                 self.assertEqual(metadata_object[key], value, key)
         # Complex key values - properties
         for key, value in (
                 expected_metadata_object["properties"]['property2'].items()):
             self.assertEqual(
                 metadata_object["properties"]["property2"][key],
                 value, key
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_properties.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_properties.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_property_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_property_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_resourcetype_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_resourcetypes.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_resourcetypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         # Simple key values
         checked_values = set([
             u'name',
             u'prefix',
             u'properties_target',
         ])
         for key, value in expected_metadef_resource_types.items():
-            if(key in checked_values):
+            if key in checked_values:
                 self.assertEqual(
                     resource_type['resource_type_associations'][0][key],
                     value, key)
 
         # Deassociate of metadef resource type resource_type1
         path = self._url('/v2/metadefs/namespaces/%s/resource_types/%s' %
                          (namespace_name, metadef_resource_type_name))
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_tag_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_tag_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_metadef_tags.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_metadef_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         }
 
         # Simple key values
         checked_values = set([
             'name'
         ])
         for key, value in expected_metadata_tag.items():
-            if(key in checked_values):
+            if key in checked_values:
                 self.assertEqual(metadata_tag[key], value, key)
 
         # Try to create a duplicate metadata tag
         headers = self._headers({'content-type': 'application/json'})
         response = requests.post(path, headers=headers)
         self.assertEqual(http.CONFLICT, response.status_code)
```

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_schemas.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_schemas.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_tasks.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_tasks.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/functional/v2/test_tasks_api_policy.py` & `glance-28.0.0.0rc1/glance/tests/functional/v2/test_tasks_api_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/integration/v2/base.py` & `glance-28.0.0.0rc1/glance/tests/integration/v2/base.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/integration/v2/test_property_quota_violations.py` & `glance-28.0.0.0rc1/glance/tests/integration/v2/test_property_quota_violations.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/integration/v2/test_tasks_api.py` & `glance-28.0.0.0rc1/glance/tests/integration/v2/test_tasks_api.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/stubs.py` & `glance-28.0.0.0rc1/glance/tests/stubs.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/test_hacking.py` & `glance-28.0.0.0rc1/glance/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/api/middleware/test_cache_manage.py` & `glance-28.0.0.0rc1/glance/tests/unit/api/middleware/test_cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/api/test_cmd.py` & `glance-28.0.0.0rc1/glance/tests/unit/api/test_cmd.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/api/test_common.py` & `glance-28.0.0.0rc1/glance/tests/unit/api/test_common.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/api/test_property_protections.py` & `glance-28.0.0.0rc1/glance/tests/unit/api/test_property_protections.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_image_conversion.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/test_image_conversion.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/plugins/test_inject_image_metadata.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_api_image_import.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_api_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_base_download.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_base_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_convert.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_convert.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_copy_image.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_copy_image.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_glance_download.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_glance_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_import.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_import.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_introspect.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_introspect.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_ovf_process.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_ovf_process.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/flows/test_web_download.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/flows/test_web_download.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/test_async.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/test_async.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/test_taskflow_executor.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/test_taskflow_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             self.assertRaises(RuntimeError, self.executor.begin_processing,
                               self.task.task_id)
         self.assertEqual('failure', self.task.status)
         self.task_repo.save.assert_called_with(self.task)
 
     def test_task_fail_upload(self):
         with mock.patch.object(image_import, 'set_image_data') as import_mock:
-            import_mock.side_effect = IOError
+            import_mock.side_effect = IOError  # noqa
 
             self.task_repo.get.return_value = self.task
             self.executor.begin_processing(self.task.task_id)
 
         self.assertEqual('failure', self.task.status)
         self.task_repo.save.assert_called_with(self.task)
         self.assertEqual(1, import_mock.call_count)
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/async_/test_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/async_/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/base.py` & `glance-28.0.0.0rc1/glance/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/cmd/test_status.py` & `glance-28.0.0.0rc1/glance/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/scripts/image_import/test_main.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/scripts/image_import/test_main.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/scripts/test_scripts_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/scripts/test_scripts_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_client.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_client.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_config.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_config.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_exception.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_exception.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_format_inspector.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_format_inspector.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,46 +47,59 @@
         super(TestFormatInspectors, self).tearDown()
         for fn in self._created_files:
             try:
                 os.remove(fn)
             except Exception:
                 pass
 
-    def _create_img(self, fmt, size):
+    def _create_img(self, fmt, size, subformat=None):
         if fmt == 'vhd':
             # QEMU calls the vhd format vpc
             fmt = 'vpc'
 
-        fn = tempfile.mktemp(prefix='glance-unittest-formatinspector-',
+        opt = ''
+        prefix = 'glance-unittest-formatinspector-'
+
+        if subformat:
+            opt = ' -o subformat=%s' % subformat
+            prefix += subformat + '-'
+
+        fn = tempfile.mktemp(prefix=prefix,
                              suffix='.%s' % fmt)
         self._created_files.append(fn)
         subprocess.check_output(
-            'qemu-img create -f %s %s %i' % (fmt, fn, size),
+            'qemu-img create -f %s %s %s %i' % (fmt, opt, fn, size),
             shell=True)
         return fn
 
-    def _create_allocated_vmdk(self, size_mb):
+    def _create_allocated_vmdk(self, size_mb, subformat=None):
         # We need a "big" VMDK file to exercise some parts of the code of the
         # format_inspector. A way to create one is to first create an empty
         # file, and then to convert it with the -S 0 option.
-        fn = tempfile.mktemp(prefix='glance-unittest-formatinspector-',
-                             suffix='.vmdk')
+
+        if subformat is None:
+            # Matches qemu-img default, see `qemu-img convert -O vmdk -o help`
+            subformat = 'monolithicSparse'
+
+        prefix = 'glance-unittest-formatinspector-%s-' % subformat
+        fn = tempfile.mktemp(prefix=prefix, suffix='.vmdk')
         self._created_files.append(fn)
-        zeroes = tempfile.mktemp(prefix='glance-unittest-formatinspector-',
-                                 suffix='.zero')
-        self._created_files.append(zeroes)
+        raw = tempfile.mktemp(prefix=prefix, suffix='.raw')
+        self._created_files.append(raw)
 
-        # Create an empty file
+        # Create a file with pseudo-random data, otherwise it will get
+        # compressed in the streamOptimized format
         subprocess.check_output(
-            'dd if=/dev/zero of=%s bs=1M count=%i' % (zeroes, size_mb),
+            'dd if=/dev/urandom of=%s bs=1M count=%i' % (raw, size_mb),
             shell=True)
 
         # Convert it to VMDK
         subprocess.check_output(
-            'qemu-img convert -f raw -O vmdk -S 0 %s %s' % (zeroes, fn),
+            'qemu-img convert -f raw -O vmdk -o subformat=%s -S 0 %s %s' % (
+                subformat, raw, fn),
             shell=True)
         return fn
 
     def _test_format_at_block_size(self, format_name, img, block_size):
         fmt = format_inspector.get_inspector(format_name)()
         self.assertIsNotNone(fmt,
                              'Did not get format inspector for %s' % (
@@ -97,16 +110,17 @@
             chunk = wrapper.read(block_size)
             if not chunk:
                 break
 
         wrapper.close()
         return fmt
 
-    def _test_format_at_image_size(self, format_name, image_size):
-        img = self._create_img(format_name, image_size)
+    def _test_format_at_image_size(self, format_name, image_size,
+                                   subformat=None):
+        img = self._create_img(format_name, image_size, subformat=subformat)
 
         # Some formats have internal alignment restrictions making this not
         # always exactly like image_size, so get the real value for comparison
         virtual_size = get_size_from_qemu_img(img)
 
         # Read the format in various sizes, some of which will read whole
         # sections in a single read, others will be completely unaligned, etc.
@@ -120,38 +134,42 @@
                               'block %i') % (format_name, image_size,
                                              block_size))
             memory = sum(fmt.context_info.values())
             self.assertLess(memory, 512 * units.Ki,
                             'Format used more than 512KiB of memory: %s' % (
                                 fmt.context_info))
 
-    def _test_format(self, format_name):
+    def _test_format(self, format_name, subformat=None):
         # Try a few different image sizes, including some odd and very small
         # sizes
         for image_size in (512, 513, 2057, 7):
-            self._test_format_at_image_size(format_name, image_size * units.Mi)
+            self._test_format_at_image_size(format_name, image_size * units.Mi,
+                                            subformat=subformat)
 
     def test_qcow2(self):
         self._test_format('qcow2')
 
     def test_vhd(self):
         self._test_format('vhd')
 
     def test_vhdx(self):
         self._test_format('vhdx')
 
     def test_vmdk(self):
         self._test_format('vmdk')
 
-    def test_vmdk_bad_descriptor_offset(self):
+    def test_vmdk_stream_optimized(self):
+        self._test_format('vmdk', 'streamOptimized')
+
+    def _test_vmdk_bad_descriptor_offset(self, subformat=None):
         format_name = 'vmdk'
         image_size = 10 * units.Mi
         descriptorOffsetAddr = 0x1c
         BAD_ADDRESS = 0x400
-        img = self._create_img(format_name, image_size)
+        img = self._create_img(format_name, image_size, subformat=subformat)
 
         # Corrupt the header
         fd = open(img, 'r+b')
         fd.seek(descriptorOffsetAddr)
         fd.write(struct.pack('<Q', BAD_ADDRESS // 512))
         fd.close()
 
@@ -163,24 +181,31 @@
                             'Failed to match %s at size %i block %i' % (
                                 format_name, image_size, block_size))
             self.assertEqual(0, fmt.virtual_size,
                              ('Calculated a virtual size for a corrupt %s at '
                               'size %i block %i') % (format_name, image_size,
                                                      block_size))
 
-    def test_vmdk_bad_descriptor_mem_limit(self):
+    def test_vmdk_bad_descriptor_offset(self):
+        self._test_vmdk_bad_descriptor_offset()
+
+    def test_vmdk_bad_descriptor_offset_stream_optimized(self):
+        self._test_vmdk_bad_descriptor_offset(subformat='streamOptimized')
+
+    def _test_vmdk_bad_descriptor_mem_limit(self, subformat=None):
         format_name = 'vmdk'
         image_size = 5 * units.Mi
         virtual_size = 5 * units.Mi
         descriptorOffsetAddr = 0x1c
         descriptorSizeAddr = descriptorOffsetAddr + 8
         twoMBInSectors = (2 << 20) // 512
         # We need a big VMDK because otherwise we will not have enough data to
         # fill-up the CaptureRegion.
-        img = self._create_allocated_vmdk(image_size // units.Mi)
+        img = self._create_allocated_vmdk(image_size // units.Mi,
+                                          subformat=subformat)
 
         # Corrupt the end of descriptor address so it "ends" at 2MB
         fd = open(img, 'r+b')
         fd.seek(descriptorSizeAddr)
         fd.write(struct.pack('<Q', twoMBInSectors))
         fd.close()
 
@@ -196,14 +221,20 @@
                               'block %i') % (format_name, image_size,
                                              block_size))
             memory = sum(fmt.context_info.values())
             self.assertLess(memory, 1.5 * units.Mi,
                             'Format used more than 1.5MiB of memory: %s' % (
                                 fmt.context_info))
 
+    def test_vmdk_bad_descriptor_mem_limit(self):
+        self._test_vmdk_bad_descriptor_mem_limit()
+
+    def test_vmdk_bad_descriptor_mem_limit_stream_optimized(self):
+        self._test_vmdk_bad_descriptor_mem_limit(subformat='streamOptimized')
+
     def test_vdi(self):
         self._test_format('vdi')
 
     def _test_format_with_invalid_data(self, format_name):
         fmt = format_inspector.get_inspector(format_name)()
         wrapper = format_inspector.InfoWrapper(open(__file__, 'rb'), fmt)
         while True:
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_location_strategy.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_location_strategy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_property_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_property_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_scripts.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_scripts.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_swift_store_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_timeutils.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/common/test_wsgi.py` & `glance-28.0.0.0rc1/glance/tests/unit/common/test_wsgi.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,15 +573,18 @@
         enabled_backends = {'os_glance_file_store': 'file'}
         self.config(enabled_backends=enabled_backends)
         server = wsgi.Server(threads=1, initialize_glance_store=True)
         self.assertRaises(RuntimeError, server.configure)
 
     @mock.patch.object(prefetcher, 'Prefetcher')
     @mock.patch.object(wsgi.Server, 'configure_socket')
-    def test_http_keepalive(self, mock_configure_socket, mock_prefetcher):
+    @mock.patch('glance.sqlite_migration.can_migrate_to_central_db')
+    def test_http_keepalive(self, mock_migrate_db, mock_configure_socket,
+                            mock_prefetcher):
+        mock_migrate_db.return_value = False
         self.config(http_keepalive=False)
         self.config(workers=0)
 
         server = wsgi.Server(threads=1)
         server.sock = 'fake_socket'
         # mocking eventlet.wsgi server method to check it is called with
         # configured 'http_keepalive' value.
@@ -595,16 +598,18 @@
                                                 log=server._logger,
                                                 debug=False,
                                                 custom_pool=server.pool,
                                                 keepalive=False,
                                                 socket_timeout=900)
 
     @mock.patch.object(prefetcher, 'Prefetcher')
-    def test_number_of_workers_posix(self, mock_prefetcher):
+    @mock.patch('glance.sqlite_migration.can_migrate_to_central_db')
+    def test_number_of_workers_posix(self, mock_migrate_db, mock_prefetcher):
         """Ensure the number of workers matches num cpus limited to 8."""
+        mock_migrate_db.return_value = False
         if os.name == 'nt':
             raise self.skipException("Unsupported platform.")
 
         def pid():
             i = 1
             while True:
                 i = i + 1
@@ -633,24 +638,28 @@
             fake_application = "fake-application"
             server.start(fake_application, None)
             cpus = processutils.get_worker_count()
             expected_workers = cpus if cpus < 8 else 8
             self.assertEqual(expected_workers,
                              len(server.children))
 
-    def test_invalid_staging_uri(self):
+    @mock.patch('glance.sqlite_migration.can_migrate_to_central_db')
+    def test_invalid_staging_uri(self, mock_migrate_db):
+        mock_migrate_db.return_value = False
         self.config(node_staging_uri='http://good.luck')
         server = wsgi.Server()
         with mock.patch.object(server, 'start_wsgi'):
             # Make sure a stating URI with an bad scheme will abort startup
             self.assertRaises(exception.GlanceException,
                               server.start, 'fake-application', 34567)
 
     @mock.patch('os.path.exists')
-    def test_missing_staging_dir(self, mock_exists):
+    @mock.patch('glance.sqlite_migration.can_migrate_to_central_db')
+    def test_missing_staging_dir(self, mock_migrate_db, mock_exists):
+        mock_migrate_db.return_value = False
         mock_exists.return_value = False
         server = wsgi.Server()
         with mock.patch.object(server, 'start_wsgi'):
             # Since we are mocking out start_wsgi, create a fake pool ourselves
             server.pool = mock.MagicMock()
             with mock.patch.object(wsgi, 'LOG') as mock_log:
                 server.start('fake-application', 34567)
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/fake_rados.py` & `glance-28.0.0.0rc1/glance/tests/unit/fake_rados.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/fixtures.py` & `glance-28.0.0.0rc1/glance/tests/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/image_cache/drivers/test_sqlite.py` & `glance-28.0.0.0rc1/glance/tests/unit/image_cache/drivers/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/keymgr/fake.py` & `glance-28.0.0.0rc1/glance/tests/unit/keymgr/fake.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_auth.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_cache_manage.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_cache_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_cache_middleware.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_cache_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_cached_images.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_cached_images.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_context.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_context_middleware.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_context_middleware.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_data_migration_framework.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_data_migration_framework.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_db.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,17 @@
 CHCKSUM1 = '43264c3edf4972c9f1cb309543d38a55'
 
 
 TASK_ID_1 = 'b3006bd0-461e-4228-88ea-431c14e918b4'
 TASK_ID_2 = '07b6b562-6770-4c8b-a649-37a515144ce9'
 TASK_ID_3 = '72d16bb6-4d70-48a5-83fe-14bb842dc737'
 
+NODE_REFERENCE_ID_1 = 1
+NODE_REFERENCE_ID_2 = 2
+
 
 def _db_fixture(id, **kwargs):
     obj = {
         'id': id,
         'name': None,
         'is_public': False,
         'properties': {},
@@ -115,25 +118,68 @@
         'deleted_at': None,
         'deleted': False
     }
     obj.update(kwargs)
     return obj
 
 
+def _db_node_reference_fixture(node_id, node_url, **kwargs):
+    obj = {
+        'node_reference_id': node_id,
+        'node_reference_url': node_url,
+    }
+    obj.update(kwargs)
+    return obj
+
+
+def _db_cached_images_fixture(id, **kwargs):
+    obj = {
+        'id': id,
+        'image_id': kwargs.get('image_id'),
+        'size': kwargs.get('size'),
+        'hits': kwargs.get('hits')
+    }
+    obj.update(kwargs)
+    return obj
+
+
 class TestImageRepo(test_utils.BaseTestCase):
 
     def setUp(self):
         super(TestImageRepo, self).setUp()
         self.db = unit_test_utils.FakeDB(initialize=False)
         self.context = glance.context.RequestContext(
             user=USER1, tenant=TENANT1)
         self.image_repo = glance.db.ImageRepo(self.context, self.db)
         self.image_factory = glance.domain.ImageFactory()
         self._create_images()
         self._create_image_members()
+        # Centralized cache
+        self._create_node_references()
+        self._create_cached_images()
+
+    def _create_node_references(self):
+        self.node_references = [
+            _db_node_reference_fixture(NODE_REFERENCE_ID_1, 'node_url_1'),
+            _db_node_reference_fixture(NODE_REFERENCE_ID_2, 'node_url_2'),
+        ]
+        [self.db.node_reference_create(
+            None, node_reference['node_reference_url'],
+            node_reference_id=node_reference['node_reference_id']
+        ) for node_reference in self.node_references]
+
+    def _create_cached_images(self):
+        self.cached_images = [
+            _db_cached_images_fixture(1, image_id=UUID1, size=256, hits=3),
+            _db_cached_images_fixture(1, image_id=UUID3, size=1024, hits=0)
+        ]
+        [self.db.insert_cache_details(
+            None, 'node_url_1', cached_image['image_id'],
+            cached_image['size'], hits=cached_image['hits']
+        ) for cached_image in self.cached_images]
 
     def _create_images(self):
         self.images = [
             _db_fixture(UUID1, owner=TENANT1, checksum=CHECKSUM,
                         name='1', size=256,
                         is_public=True, status='active',
                         locations=[{'url': UUID1_LOCATION,
@@ -203,14 +249,101 @@
         self.image_members = [
             _db_image_member_fixture(UUID2, TENANT2),
             _db_image_member_fixture(UUID2, TENANT3, status='accepted'),
         ]
         [self.db.image_member_create(None, image_member)
             for image_member in self.image_members]
 
+    def test_node_reference_get_by_url(self):
+        node_reference = self.db.node_reference_get_by_url(self.context,
+                                                           'node_url_1')
+        self.assertEqual(NODE_REFERENCE_ID_1,
+                         node_reference['node_reference_id'])
+
+    def test_node_reference_get_by_url_not_found(self):
+        self.assertRaises(exception.NotFound,
+                          self.db.node_reference_get_by_url,
+                          self.context,
+                          'garbage_url')
+
+    def test_get_cached_images(self):
+        # Two images are cached on node 'node_url_1'
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_1')
+        self.assertEqual(2, len(cached_images))
+
+        # Nothing is cached on node 'node_url_2'
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_2')
+        self.assertEqual(0, len(cached_images))
+
+    def test_get_hit_count(self):
+        # Hit count will be 3 for image UUID1
+        self.assertEqual(3, self.db.get_hit_count(self.context,
+                                                  UUID1, 'node_url_1'))
+
+        # Hit count will be 0 for uncached image
+        self.assertEqual(0, self.db.get_hit_count(self.context,
+                                                  UUID2, 'node_url_1'))
+
+    def test_delete_all_cached_images(self):
+        # Verify that we have image cached
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_1')
+        self.assertEqual(2, len(cached_images))
+
+        # Delete cached images from node_url_1
+        self.db.delete_all_cached_images(self.context, 'node_url_1')
+
+        # Verify that all cached images from node_url_1 are deleted
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_1')
+        self.assertEqual(0, len(cached_images))
+
+    def test_delete_cached_image(self):
+        # Verify that we have image cached
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_1')
+        self.assertEqual(2, len(cached_images))
+
+        # Delete cached image from node_url_1
+        self.db.delete_cached_image(self.context, UUID1, 'node_url_1')
+
+        # Verify that given image from node_url_1 is deleted
+        cached_images = self.db.get_cached_images(self.context,
+                                                  'node_url_1')
+        self.assertEqual(1, len(cached_images))
+
+    def test_get_least_recently_accessed(self):
+        recently_accessed = self.db.get_least_recently_accessed(
+            self.context, 'node_url_1')
+        # Verify we will only get one image in response
+        self.assertEqual(UUID1, recently_accessed)
+
+    def test_is_image_cached_for_node(self):
+        # Verify UUID1 is cached for node_url_1
+        self.assertTrue(self.db.is_image_cached_for_node(
+            self.context, 'node_url_1', UUID1))
+
+        # Verify UUID3 is not cached for node_url_2
+        self.assertFalse(self.db.is_image_cached_for_node(
+            self.context, 'node_url_2', UUID3))
+
+    def test_update_hit_count(self):
+        # Verify UUID1 on node_url_1 has 3 as hit count
+        self.assertEqual(3, self.db.get_hit_count(self.context,
+                                                  UUID1, 'node_url_1'))
+
+        # Update the hit count of UUID1
+        self.db.update_hit_count(self.context, UUID1, 'node_url_1')
+
+        # Verify hit count is now 4
+        self.assertEqual(4, self.db.get_hit_count(self.context,
+                                                  UUID1, 'node_url_1'))
+
     def test_get(self):
         image = self.image_repo.get(UUID1)
         self.assertEqual(UUID1, image.image_id)
         self.assertEqual('1', image.name)
         self.assertEqual(set(['ping', 'pong']), image.tags)
         self.assertEqual('public', image.visibility)
         self.assertEqual('active', image.status)
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_db_metadef.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_db_metadef.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_domain.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_domain.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_domain_proxy.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_domain_proxy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_gateway.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_gateway.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_glance_manage.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_glance_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_glance_replicator.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_glance_replicator.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_housekeeping.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_housekeeping.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_image_cache.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_image_cache.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from contextlib import contextmanager
 import datetime
+import errno
 import io
 import os
 import tempfile
 import time
 from unittest import mock
 
 import fixtures
 import glance_store as store
 from oslo_config import cfg
+from oslo_utils import fileutils
 from oslo_utils import secretutils
 from oslo_utils import units
 
 from glance import async_
 from glance.common import exception
 from glance import context
 from glance import gateway as glance_gateway
@@ -125,14 +127,40 @@
             self.assertTrue(self.cache.is_cached(image_id))
 
         self.cache.delete_all_cached_images()
 
         for image_id in (1, 2):
             self.assertFalse(self.cache.is_cached(image_id))
 
+    def _test_clean_invalid_path(self, failure=False):
+        invalid_file_path = os.path.join(self.cache_dir, 'invalid', '1')
+        invalid_file = open(invalid_file_path, 'wb')
+        invalid_file.write(FIXTURE_DATA)
+        invalid_file.close()
+
+        self.assertTrue(os.path.exists(invalid_file_path))
+
+        self.delay_inaccurate_clock()
+        if failure:
+            with mock.patch.object(
+                    fileutils, 'delete_if_exists') as mock_delete:
+                mock_delete.side_effect = OSError(errno.ENOENT, '')
+                try:
+                    self.cache.clean()
+                except OSError:
+                    self.assertTrue(os.path.exists(invalid_file_path))
+        else:
+            self.cache.clean()
+            self.assertFalse(os.path.exists(invalid_file_path))
+
+    @skip_if_disabled
+    def test_clean_invalid_path(self):
+        """Test the clean method removes expected image from invalid path."""
+        self._test_clean_invalid_path()
+
     @skip_if_disabled
     def test_clean_stalled(self):
         """Test the clean method removes expected images."""
         incomplete_file_path = os.path.join(self.cache_dir, 'incomplete', '1')
         incomplete_file = open(incomplete_file_path, 'wb')
         incomplete_file.write(FIXTURE_DATA)
         incomplete_file.close()
@@ -140,44 +168,62 @@
         self.assertTrue(os.path.exists(incomplete_file_path))
 
         self.delay_inaccurate_clock()
         self.cache.clean(stall_time=0)
 
         self.assertFalse(os.path.exists(incomplete_file_path))
 
-    @skip_if_disabled
-    def test_clean_stalled_nonzero_stall_time(self):
+    def _test_clean_stall_time(self, stall_time=None, days=2,
+                               stall_failed=False):
         """
         Test the clean method removes the stalled images as expected
         """
         incomplete_file_path_1 = os.path.join(self.cache_dir,
                                               'incomplete', '1')
         incomplete_file_path_2 = os.path.join(self.cache_dir,
                                               'incomplete', '2')
         for f in (incomplete_file_path_1, incomplete_file_path_2):
             incomplete_file = open(f, 'wb')
             incomplete_file.write(FIXTURE_DATA)
             incomplete_file.close()
 
         mtime = os.path.getmtime(incomplete_file_path_1)
         pastday = (datetime.datetime.fromtimestamp(mtime) -
-                   datetime.timedelta(days=1))
+                   datetime.timedelta(days=days))
         atime = int(time.mktime(pastday.timetuple()))
         mtime = atime
         os.utime(incomplete_file_path_1, (atime, mtime))
 
         self.assertTrue(os.path.exists(incomplete_file_path_1))
         self.assertTrue(os.path.exists(incomplete_file_path_2))
 
-        self.cache.clean(stall_time=3600)
+        # If stall_time is None then it will wait for default time
+        # of `image_cache_stall_time` which is 24 hours
+        if stall_failed:
+            with mock.patch.object(
+                    fileutils, 'delete_if_exists') as mock_delete:
+                mock_delete.side_effect = OSError(errno.ENOENT, '')
+                self.cache.clean(stall_time=stall_time)
+                self.assertTrue(os.path.exists(incomplete_file_path_1))
+        else:
+            self.cache.clean(stall_time=stall_time)
+            self.assertFalse(os.path.exists(incomplete_file_path_1))
 
-        self.assertFalse(os.path.exists(incomplete_file_path_1))
         self.assertTrue(os.path.exists(incomplete_file_path_2))
 
     @skip_if_disabled
+    def test_clean_stalled_none_stall_time(self):
+        self._test_clean_stall_time()
+
+    @skip_if_disabled
+    def test_clean_stalled_nonzero_stall_time(self):
+        """Test the clean method removes expected images."""
+        self._test_clean_stall_time(stall_time=3600, days=1)
+
+    @skip_if_disabled
     def test_prune(self):
         """
         Test that pruning the cache works as expected...
         """
         self.assertEqual(0, self.cache.get_cache_size())
 
         # Add a bunch of images to the cache. The max cache size for the cache
@@ -276,14 +322,27 @@
         self.assertFalse(self.cache.is_queued(1))
         self.assertTrue(self.cache.is_cached(1))
 
         self.assertFalse(self.cache.queue_image(1))
 
         self.cache.delete_cached_image(1)
 
+        # Test that we return false if image is being cached
+        incomplete_file_path = os.path.join(self.cache_dir, 'incomplete', '1')
+        incomplete_file = open(incomplete_file_path, 'wb')
+        incomplete_file.write(FIXTURE_DATA)
+        incomplete_file.close()
+
+        self.assertFalse(self.cache.is_queued(1))
+        self.assertFalse(self.cache.is_cached(1))
+        self.assertTrue(self.cache.driver.is_being_cached(1))
+
+        self.assertFalse(self.cache.queue_image(1))
+        self.cache.clean(stall_time=0)
+
         for x in range(3):
             self.assertTrue(self.cache.queue_image(x))
 
         self.assertEqual(['0', '1', '2'],
                          self.cache.get_queued_images())
 
     @skip_if_disabled
@@ -417,28 +476,36 @@
         image = b"12345678990abcdefghijklmnop"
         image_id = 123
 
         md5 = secretutils.md5(usedforsecurity=False)
         md5.update(image)
         checksum = md5.hexdigest()
 
-        cache = image_cache.ImageCache()
+        with mock.patch('glance.db.get_api') as mock_get_db:
+            db = unit_test_utils.FakeDB(initialize=False)
+            mock_get_db.return_value = db
+            cache = image_cache.ImageCache()
+
         img_iter = cache.get_caching_iter(image_id, checksum, [image])
         for chunk in img_iter:
             pass
         # checksum is valid, fake image should be cached:
         self.assertTrue(cache.is_cached(image_id))
 
     @skip_if_disabled
     def test_gate_caching_iter_bad_checksum(self):
         image = b"12345678990abcdefghijklmnop"
         image_id = 123
         checksum = "foobar"  # bad.
 
-        cache = image_cache.ImageCache()
+        with mock.patch('glance.db.get_api') as mock_get_db:
+            db = unit_test_utils.FakeDB(initialize=False)
+            mock_get_db.return_value = db
+            cache = image_cache.ImageCache()
+
         img_iter = cache.get_caching_iter(image_id, checksum, [image])
 
         def reader():
             for chunk in img_iter:
                 pass
         self.assertRaises(exception.GlanceException, reader)
         # checksum is invalid, caching will fail:
@@ -482,14 +549,76 @@
         if not xattr_writes_supported(self.cache_dir):
             self.inited = True
             self.disabled = True
             self.disabled_message = ("filesystem does not support xattr")
             return
 
 
+class TestImageCacheCentralizedDb(test_utils.BaseTestCase,
+                                  ImageCacheTestCase):
+
+    """Tests image caching when Centralized DB is used in cache"""
+
+    def setUp(self):
+        super(TestImageCacheCentralizedDb, self).setUp()
+
+        self.inited = True
+        self.disabled = False
+        self.cache_dir = self.useFixture(fixtures.TempDir()).path
+        self.config(image_cache_dir=self.cache_dir,
+                    image_cache_driver='centralized_db',
+                    image_cache_max_size=5 * units.Ki,
+                    worker_self_reference_url='http://workerx')
+
+        with mock.patch('glance.db.get_api') as mock_get_db:
+            self.db = unit_test_utils.FakeDB(initialize=False)
+            mock_get_db.return_value = self.db
+            self.cache = image_cache.ImageCache()
+
+    def test_node_reference_create_duplicate(self):
+        with mock.patch('glance.db.get_api') as mock_get_db:
+            self.db = unit_test_utils.FakeDB(initialize=False)
+            mock_get_db.return_value = self.db
+            with mock.patch.object(
+                    self.db, 'node_reference_create') as mock_node_create:
+                mock_node_create.side_effect = exception.Duplicate
+                with mock.patch.object(
+                        image_cache.drivers.centralized_db, 'LOG') as mock_log:
+                    image_cache.ImageCache()
+                    expected_calls = [
+                        mock.call('Node reference is already recorded, '
+                                  'ignoring it')
+                    ]
+                    mock_log.debug.assert_has_calls(expected_calls)
+
+    def test_get_least_recently_accessed_os_error(self):
+        self.assertEqual(0, self.cache.get_cache_size())
+        for x in range(10):
+            FIXTURE_FILE = io.BytesIO(FIXTURE_DATA)
+            self.assertTrue(self.cache.cache_image_file(x, FIXTURE_FILE))
+
+        self.assertEqual(10 * units.Ki, self.cache.get_cache_size())
+
+        with mock.patch.object(os, 'stat') as mock_stat:
+            mock_stat.side_effect = OSError
+            image_id, size = self.cache.driver.get_least_recently_accessed()
+            self.assertEqual(0, size)
+
+    @skip_if_disabled
+    def test_clean_stalled_fails(self):
+        """Test the clean method fails to delete file, ignores the failure"""
+        self._test_clean_stall_time(stall_time=3600, days=1,
+                                    stall_failed=True)
+
+    @skip_if_disabled
+    def test_clean_invalid_path_fails(self):
+        """Test the clean method fails to remove image from invalid path."""
+        self._test_clean_invalid_path(failure=True)
+
+
 class TestImageCacheSqlite(test_utils.BaseTestCase,
                            ImageCacheTestCase):
 
     """Tests image caching when SQLite is used in cache"""
 
     def setUp(self):
         """
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_manage.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_manage.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_misc.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_misc.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_notifier.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_notifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -698,17 +698,17 @@
             timeutils.isotime(self.task.created_at),
             output_log['payload']['created_at']
         )
         if 'location' in output_log['payload']:
             self.fail('Notification contained location field.')
         # Verify newly added fields 'image_id', 'user_id' and
         # 'request_id' are not part of notification yet
-        self.assertTrue('image_id' not in output_log['payload'])
-        self.assertTrue('user_id' not in output_log['payload'])
-        self.assertTrue('request_id' not in output_log['payload'])
+        self.assertNotIn('image_id', output_log['payload'])
+        self.assertNotIn('user_id', output_log['payload'])
+        self.assertNotIn('request_id', output_log['payload'])
 
     def test_task_create_notification_disabled(self):
         self.config(disabled_notifications=['task.create'])
         self.task_repo_proxy.add(self.task_stub_proxy)
         output_logs = self.notifier.get_logs()
         self.assertEqual(0, len(output_logs))
 
@@ -733,17 +733,17 @@
             now,
             output_log['payload']['deleted_at']
         )
         if 'location' in output_log['payload']:
             self.fail('Notification contained location field.')
         # Verify newly added fields 'image_id', 'user_id' and
         # 'request_id' are not part of notification yet
-        self.assertTrue('image_id' not in output_log['payload'])
-        self.assertTrue('user_id' not in output_log['payload'])
-        self.assertTrue('request_id' not in output_log['payload'])
+        self.assertNotIn('image_id', output_log['payload'])
+        self.assertNotIn('user_id', output_log['payload'])
+        self.assertNotIn('request_id', output_log['payload'])
 
     def test_task_delete_notification_disabled(self):
         self.config(disabled_notifications=['task.delete'])
         self.task_repo_proxy.remove(self.task_stub_proxy)
         output_logs = self.notifier.get_logs()
         self.assertEqual(0, len(output_logs))
 
@@ -754,23 +754,17 @@
             self.task_proxy.run(executor=mock_executor)
         output_logs = self.notifier.get_logs()
         self.assertEqual(1, len(output_logs))
         output_log = output_logs[0]
         self.assertEqual('INFO', output_log['notification_type'])
         self.assertEqual('task.run', output_log['event_type'])
         self.assertEqual(self.task.task_id, output_log['payload']['id'])
-        self.assertFalse(
-            self.task.image_id in output_log['payload']
-        )
-        self.assertFalse(
-            self.task.user_id in output_log['payload']
-        )
-        self.assertFalse(
-            self.task.request_id in output_log['payload']
-        )
+        self.assertNotIn(self.task.image_id, output_log['payload'])
+        self.assertNotIn(self.task.user_id, output_log['payload'])
+        self.assertNotIn(self.task.request_id, output_log['payload'])
 
     def test_task_run_notification_disabled(self):
         self.config(disabled_notifications=['task.run'])
         with mock.patch('glance.async_.TaskExecutor') as mock_executor:
             executor = mock_executor.return_value
             executor._run.return_value = mock.Mock()
             self.task_proxy.run(executor=mock_executor)
@@ -783,17 +777,17 @@
         self.assertEqual(1, len(output_logs))
         output_log = output_logs[0]
         self.assertEqual('INFO', output_log['notification_type'])
         self.assertEqual('task.processing', output_log['event_type'])
         self.assertEqual(self.task.task_id, output_log['payload']['id'])
         # Verify newly added fields 'image_id', 'user_id' and
         # 'request_id' are not part of notification yet
-        self.assertTrue('image_id' not in output_log['payload'])
-        self.assertTrue('user_id' not in output_log['payload'])
-        self.assertTrue('request_id' not in output_log['payload'])
+        self.assertNotIn('image_id', output_log['payload'])
+        self.assertNotIn('user_id', output_log['payload'])
+        self.assertNotIn('request_id', output_log['payload'])
 
     def test_task_processing_notification_disabled(self):
         self.config(disabled_notifications=['task.processing'])
         self.task_proxy.begin_processing()
         output_logs = self.notifier.get_logs()
         self.assertEqual(0, len(output_logs))
 
@@ -804,17 +798,17 @@
         self.assertEqual(2, len(output_logs))
         output_log = output_logs[1]
         self.assertEqual('INFO', output_log['notification_type'])
         self.assertEqual('task.success', output_log['event_type'])
         self.assertEqual(self.task.task_id, output_log['payload']['id'])
         # Verify newly added fields 'image_id', 'user_id' and
         # 'request_id' are not part of notification yet
-        self.assertTrue('image_id' not in output_log['payload'])
-        self.assertTrue('user_id' not in output_log['payload'])
-        self.assertTrue('request_id' not in output_log['payload'])
+        self.assertNotIn('image_id', output_log['payload'])
+        self.assertNotIn('user_id', output_log['payload'])
+        self.assertNotIn('request_id', output_log['payload'])
 
     def test_task_success_notification_disabled(self):
         self.config(disabled_notifications=['task.processing', 'task.success'])
         self.task_proxy.begin_processing()
         self.task_proxy.succeed(result=None)
         output_logs = self.notifier.get_logs()
         self.assertEqual(0, len(output_logs))
@@ -825,16 +819,16 @@
         self.assertEqual(1, len(output_logs))
         output_log = output_logs[0]
         self.assertEqual('INFO', output_log['notification_type'])
         self.assertEqual('task.failure', output_log['event_type'])
         self.assertEqual(self.task.task_id, output_log['payload']['id'])
         # Verify newly added fields 'image_id', 'user_id' and
         # 'request_id' are not part of notification yet
-        self.assertTrue('image_id' not in output_log['payload'])
-        self.assertTrue('user_id' not in output_log['payload'])
-        self.assertTrue('request_id' not in output_log['payload'])
+        self.assertNotIn('image_id', output_log['payload'])
+        self.assertNotIn('user_id', output_log['payload'])
+        self.assertNotIn('request_id', output_log['payload'])
 
     def test_task_failure_notification_disabled(self):
         self.config(disabled_notifications=['task.failure'])
         self.task_proxy.fail(message=None)
         output_logs = self.notifier.get_logs()
         self.assertEqual(0, len(output_logs))
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_policy.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_quota.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_quota.py`

 * *Files 4% similar despite different names*

```diff
@@ -198,14 +198,15 @@
         self.assertRaises(exception.StorageQuotaFull,
                           image.set_data,
                           data,
                           size=len(data))
 
         # If we turn on keystone quotas, the global limit gets ignored
         # so the same image no longer fails.
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         image.set_data(data, size=len(data))
 
     def test_append_location(self):
         new_location = {'url': 'file:///a/path', 'metadata': {},
                         'status': 'active'}
         image = self._get_image()
@@ -790,63 +791,69 @@
                         'status': 'active', 'size': size * units.Mi,
                         'locations': locations}
         self.db_api.image_create(context, image_values)
 
     def test_enforce_overquota(self):
         # Check that a single large image with multiple locations will
         # trip the quota check.
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         self._create_fake_image(context, 300)
         exc = self.assertRaises(exception.LimitExceeded,
                                 ks_quota.enforce_image_size_total,
                                 context, context.owner)
         self.assertIn('image_size_total is over limit of 500', str(exc))
 
     def test_enforce_overquota_with_delta(self):
         # Check that delta is honored, if used.
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         self._create_fake_image(context, 200)
         ks_quota.enforce_image_size_total(context, context.owner)
         ks_quota.enforce_image_size_total(context, context.owner,
                                           delta=50)
         self.assertRaises(exception.LimitExceeded,
                           ks_quota.enforce_image_size_total,
                           context, context.owner, delta=200)
 
     def test_enforce_overquota_disabled(self):
         # Just like the overquota case above, but without being enabled,
         # so no failure
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=False)
         context = FakeContext()
         self._create_fake_image(context, 300)
         # Does not raise because keystone limits are disabled
         ks_quota.enforce_image_size_total(context, context.owner)
 
     def test_enforce_overquota_multiple(self):
         # Check that multiple images with a combined amount
         # (2*2*150=600) over the quota will trip the quota check.
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         self._create_fake_image(context, 150)
         self._create_fake_image(context, 150)
         exc = self.assertRaises(exception.LimitExceeded,
                                 ks_quota.enforce_image_size_total,
                                 context, context.owner)
         self.assertIn('image_size_total is over limit of 500', str(exc))
 
     def test_enforce_underquota(self):
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         self._create_fake_image(context, 100)
         # We are under quota, so no exception expected
         ks_quota.enforce_image_size_total(context, context.owner)
 
     def test_enforce_underquota_with_others_over_quota(self):
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         # Put the first tenant over quota
         context = FakeContext()
         self._create_fake_image(context, 300)
         self._create_fake_image(context, 300)
 
         # Create an image for another tenant that is not over quota
@@ -854,38 +861,41 @@
         other_context.owner = 'someone_else'
         self._create_fake_image(other_context, 100)
         # This tenant should pass the quota check, because it is under quota,
         # even though the other is over.
         ks_quota.enforce_image_size_total(other_context, other_context.owner)
 
     def test_enforce_multiple_limits_under_quota(self):
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         # Make sure that we can call the multi-limit handler and pass when
         # we are under quota.
         ks_quota._enforce_some(context, context.owner,
                                {ks_quota.QUOTA_IMAGE_SIZE_TOTAL: lambda: 200,
                                 'another_limit': lambda: 1},
                                {'another_limit': 1})
 
     def test_enforce_multiple_limits_over_quota(self):
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         context = FakeContext()
         # Make sure that even if one of a multi-limit call is over
         # quota, we get the exception.
         self.assertRaises(exception.LimitExceeded,
                           ks_quota._enforce_some,
                           context, context.owner,
                           {ks_quota.QUOTA_IMAGE_SIZE_TOTAL: lambda: 200,
                            'another_limit': lambda: 1},
                           {'another_limit': 5})
 
     @mock.patch('oslo_limit.limit.Enforcer')
     @mock.patch.object(ks_quota, 'LOG')
     def test_oslo_limit_config_fail(self, mock_LOG, mock_enforcer):
+        self.config(endpoint_id='ENDPOINT_ID', group='oslo_limit')
         self.config(use_keystone_limits=True)
         mock_enforcer.return_value.enforce.side_effect = (
             ol_exc.SessionInitError('test'))
         context = FakeContext()
         self._create_fake_image(context, 100)
         self.assertRaises(ol_exc.SessionInitError,
                           ks_quota.enforce_image_size_total,
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_schema.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_scrubber.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_store_image.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_store_image.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_store_location.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_store_location.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_test_utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/test_versions.py` & `glance-28.0.0.0rc1/glance/tests/unit/test_versions.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/utils.py` & `glance-28.0.0.0rc1/glance/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_cache_management_api.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_cache_management_api.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_discovery_image_import.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_discovery_image_import.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_discovery_stores.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_discovery_stores.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_image_actions_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_actions_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_image_data_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_data_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_image_members_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_members_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_image_tags_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_image_tags_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_images_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_images_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -3873,15 +3873,15 @@
             UUID2, name='image-2', owner=TENANT2,
             checksum='ca425b88f047ce8ec45ee90e813ada91',
             os_hash_algo=FAKEHASHALGO, os_hash_value=MULTIHASH1,
             created_at=DATETIME, updated_at=DATETIME, size=1024,
             virtual_size=3072, extra_properties=props)
         self.controller._delete_encryption_key(request.context, image)
         # Make sure the encryption key is gone
-        self.assertRaises(KeyError,
+        self.assertRaises(castellan_exception.ManagedObjectNotFoundError,
                           self.controller._key_manager.get,
                           request.context, fake_encryption_key)
 
     def test_delete_no_encryption_key_id(self):
         request = unit_test_utils.get_fake_request()
         extra_props = {
             'cinder_encryption_key_deletion_policy': 'on_image_deletion',
```

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_metadef_resources.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_metadef_resources.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_schemas_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_schemas_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_tasks_resource.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_tasks_resource.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/unit/v2/test_v2_policy.py` & `glance-28.0.0.0rc1/glance/tests/unit/v2/test_v2_policy.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/utils.py` & `glance-28.0.0.0rc1/glance/tests/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import subprocess
 import threading
 import time
 from unittest import mock
 
 from alembic import command as alembic_command
 import fixtures
+from oslo_concurrency import lockutils
 from oslo_config import cfg
 from oslo_config import fixture as cfg_fixture
 from oslo_log.fixture import logging_error as log_fixture
 from oslo_log import log
 from oslo_utils import timeutils
 from oslo_utils import units
 import testtools
@@ -82,14 +83,17 @@
         config.parse_args(args=[])
         self.addCleanup(CONF.reset)
         self.mock_object(exception, '_FATAL_EXCEPTION_FORMAT_ERRORS', True)
         self.test_dir = self.useFixture(fixtures.TempDir()).path
         self.test_dir2 = self.useFixture(fixtures.TempDir()).path
         self.conf_dir = os.path.join(self.test_dir, 'etc')
         utils.safe_mkdirs(self.conf_dir)
+        self.lock_dir = os.path.join(self.test_dir, 'locks')
+        utils.safe_mkdirs(self.lock_dir)
+        lockutils.set_defaults(self.lock_dir)
         self.set_policy()
 
         # Limit the amount of DeprecationWarning messages in the unit test logs
         self.useFixture(glance_fixtures.WarningsFixture())
 
         # Make sure logging output is limited but still test debug formatting
         self.useFixture(log_fixture.get_logging_handle_error_fixture())
```

### Comparing `glance-28.0.0.0b2/glance/tests/var/ca.crt` & `glance-28.0.0.0rc1/glance/tests/var/ca.crt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/ca.key` & `glance-28.0.0.0rc1/glance/tests/var/ca.key`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/certificate.crt` & `glance-28.0.0.0rc1/glance/tests/var/certificate.crt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/privatekey.key` & `glance-28.0.0.0rc1/glance/tests/var/privatekey.key`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/testserver-bad-ovf.ova` & `glance-28.0.0.0rc1/glance/tests/var/testserver-bad-ovf.ova`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/testserver-no-disk.ova` & `glance-28.0.0.0rc1/glance/tests/var/testserver-no-disk.ova`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/testserver-no-ovf.ova` & `glance-28.0.0.0rc1/glance/tests/var/testserver-no-ovf.ova`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/testserver-not-tar.ova` & `glance-28.0.0.0rc1/glance/tests/var/testserver-not-tar.ova`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/tests/var/testserver.ova` & `glance-28.0.0.0rc1/glance/tests/var/testserver.ova`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance/version.py` & `glance-28.0.0.0rc1/glance/version.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance.egg-info/PKG-INFO` & `glance-28.0.0.0rc1/glance.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: glance
-Version: 28.0.0.0b2
+Version: 28.0.0.0rc1
 Summary: OpenStack Image Service
 Home-page: https://docs.openstack.org/glance/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ================
         OpenStack Glance
@@ -80,8 +80,10 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `glance-28.0.0.0b2/glance.egg-info/SOURCES.txt` & `glance-28.0.0.0rc1/glance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,15 @@
 glance/housekeeping.py
 glance/i18n.py
 glance/location.py
 glance/notifier.py
 glance/opts.py
 glance/schema.py
 glance/scrubber.py
+glance/sqlite_migration.py
 glance/version.py
 glance.egg-info/PKG-INFO
 glance.egg-info/SOURCES.txt
 glance.egg-info/dependency_links.txt
 glance.egg-info/entry_points.txt
 glance.egg-info/not-zip-safe
 glance.egg-info/pbr.json
@@ -409,28 +410,31 @@
 glance/db/sqlalchemy/alembic_migrations/add_metadefs_tables.py
 glance/db/sqlalchemy/alembic_migrations/add_tasks_tables.py
 glance/db/sqlalchemy/alembic_migrations/alembic.ini
 glance/db/sqlalchemy/alembic_migrations/env.py
 glance/db/sqlalchemy/alembic_migrations/migrate.cfg
 glance/db/sqlalchemy/alembic_migrations/script.py.mako
 glance/db/sqlalchemy/alembic_migrations/data_migrations/2023_1_migrate01_empty.py
+glance/db/sqlalchemy/alembic_migrations/data_migrations/2024_1_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/__init__.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/ocata_migrate01_community_images.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/pike_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/queens_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/rocky_migrate02_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/train_migrate01_backend_to_store.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/ussuri_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/wallaby_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/xena_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/yoga_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/data_migrations/zed_migrate01_empty.py
 glance/db/sqlalchemy/alembic_migrations/versions/2023_1_contract01_empty.py
 glance/db/sqlalchemy/alembic_migrations/versions/2023_1_expand01_empty.py
+glance/db/sqlalchemy/alembic_migrations/versions/2024_1_contract01_empty.py
+glance/db/sqlalchemy/alembic_migrations/versions/2024_1_expand01_add_cache_tables.py
 glance/db/sqlalchemy/alembic_migrations/versions/__init__.py
 glance/db/sqlalchemy/alembic_migrations/versions/liberty_initial.py
 glance/db/sqlalchemy/alembic_migrations/versions/mitaka01_add_image_created_updated_idx.py
 glance/db/sqlalchemy/alembic_migrations/versions/mitaka02_update_metadef_os_nova_server.py
 glance/db/sqlalchemy/alembic_migrations/versions/ocata_contract01_drop_is_public.py
 glance/db/sqlalchemy/alembic_migrations/versions/ocata_expand01_add_visibility.py
 glance/db/sqlalchemy/alembic_migrations/versions/pike_contract01_drop_artifacts_tables.py
@@ -469,14 +473,16 @@
 glance/image_cache/base.py
 glance/image_cache/cleaner.py
 glance/image_cache/client.py
 glance/image_cache/prefetcher.py
 glance/image_cache/pruner.py
 glance/image_cache/drivers/__init__.py
 glance/image_cache/drivers/base.py
+glance/image_cache/drivers/centralized_db.py
+glance/image_cache/drivers/common.py
 glance/image_cache/drivers/sqlite.py
 glance/image_cache/drivers/xattr.py
 glance/locale/de/LC_MESSAGES/glance.po
 glance/locale/en_GB/LC_MESSAGES/glance.po
 glance/locale/es/LC_MESSAGES/glance.po
 glance/locale/fr/LC_MESSAGES/glance.po
 glance/locale/it/LC_MESSAGES/glance.po
@@ -522,26 +528,30 @@
 glance/tests/functional/test_wsgi.py
 glance/tests/functional/db/__init__.py
 glance/tests/functional/db/base.py
 glance/tests/functional/db/base_metadef.py
 glance/tests/functional/db/test_migrations.py
 glance/tests/functional/db/test_sqlalchemy.py
 glance/tests/functional/db/migrations/__init__.py
+glance/tests/functional/db/migrations/test_2024_1_expand01.py
 glance/tests/functional/db/migrations/test_mitaka01.py
 glance/tests/functional/db/migrations/test_mitaka02.py
 glance/tests/functional/db/migrations/test_ocata_contract01.py
 glance/tests/functional/db/migrations/test_ocata_expand01.py
 glance/tests/functional/db/migrations/test_ocata_migrate01.py
 glance/tests/functional/db/migrations/test_pike_contract01.py
 glance/tests/functional/db/migrations/test_pike_expand01.py
 glance/tests/functional/db/migrations/test_pike_migrate01.py
 glance/tests/functional/db/migrations/test_rocky_expand01.py
 glance/tests/functional/db/migrations/test_rocky_expand02.py
 glance/tests/functional/db/migrations/test_train_migrate01.py
 glance/tests/functional/db/migrations/test_wallaby_expand01.py
+glance/tests/functional/image_cache/__init__.py
+glance/tests/functional/image_cache/drivers/__init__.py
+glance/tests/functional/image_cache/drivers/test_centralized_db.py
 glance/tests/functional/serial/__init__.py
 glance/tests/functional/serial/test_scrubber.py
 glance/tests/functional/v2/__init__.py
 glance/tests/functional/v2/metadef_base.py
 glance/tests/functional/v2/test_cache_api.py
 glance/tests/functional/v2/test_cache_api_policy.py
 glance/tests/functional/v2/test_discovery.py
@@ -591,14 +601,15 @@
 glance/tests/unit/test_manage.py
 glance/tests/unit/test_misc.py
 glance/tests/unit/test_notifier.py
 glance/tests/unit/test_policy.py
 glance/tests/unit/test_quota.py
 glance/tests/unit/test_schema.py
 glance/tests/unit/test_scrubber.py
+glance/tests/unit/test_sqlite_migration.py
 glance/tests/unit/test_store_image.py
 glance/tests/unit/test_store_location.py
 glance/tests/unit/test_test_utils.py
 glance/tests/unit/test_versions.py
 glance/tests/unit/utils.py
 glance/tests/unit/api/__init__.py
 glance/tests/unit/api/test_cmd.py
@@ -715,31 +726,36 @@
 releasenotes/notes/bug-1719252-name-validation-443a2e2a36be2cec.yaml
 releasenotes/notes/bug-1861334-ebc2026b85675d47.yaml
 releasenotes/notes/bug-1881958-d0e16538f3c0ffaa.yaml
 releasenotes/notes/bug-1979699-70182ec2aead0383.yaml
 releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml
 releasenotes/notes/bump-api-2-4-efa266aef0928e04.yaml
 releasenotes/notes/cache-api-b806ccfb8c5d9bb6.yaml
+releasenotes/notes/caracal-milestone-3-releasenotes-534b1daa3e1f254c.yaml
 releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml
 releasenotes/notes/clean-up-acceptable-values-store_type_preference-39081e4045894731.yaml
 releasenotes/notes/cleanout_registry_data-api-9d91368aed83497e.yaml
 releasenotes/notes/cleanup-enable_v2_api-9b9b467f4ae8c3b1.yaml
 releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml
 releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml
 releasenotes/notes/delete_from_store-a1d9b9bd5cf27546.yaml
 releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml
 releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml
 releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml
 releasenotes/notes/deprecate-glance-api-opts-23bdbd1ad7625999.yaml
+releasenotes/notes/deprecate-glance-cache-manage-c88f07d33fcc7ca5.yaml
 releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml
+releasenotes/notes/deprecate-location_strategy-f658e69700204bbf.yaml
 releasenotes/notes/deprecate-owner_is_tenant-ec8ea36a3f7e9268.yaml
 releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml
+releasenotes/notes/deprecate-scrubber-862c38e0d65557f3.yaml
 releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml
 releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml
 releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml
+releasenotes/notes/deprecate-sqlite-cache-driver-1f5f67862f56e0ba.yaml
 releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml
 releasenotes/notes/deprecate-windows-support-557481e4d45912ee.yaml
 releasenotes/notes/distributed-image-import-82cff4426731beac.yaml
 releasenotes/notes/drop-py-2-7-863871c7bc047146.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-c6f051d5b2b40329.yaml
 releasenotes/notes/drop-sheepdog-b55aae84807d31d9.yaml
 releasenotes/notes/drop-support-for-sqlalchemy-migrate-4bcbe7b200697586.yaml
```

### Comparing `glance-28.0.0.0b2/glance.egg-info/entry_points.txt` & `glance-28.0.0.0rc1/glance.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/glance.egg-info/requires.txt` & `glance-28.0.0.0rc1/glance.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/playbooks/post-check-metadata-injection.yaml` & `glance-28.0.0.0rc1/playbooks/post-check-metadata-injection.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/rally-jobs/README.rst` & `glance-28.0.0.0rc1/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/rally-jobs/glance.yaml` & `glance-28.0.0.0rc1/rally-jobs/glance.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/Stein-reno-rc1-0a03f8394934a2e7.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/Train-milestone3-be5520106a182fa0.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/add-compressed-format-185e537187a202bd.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/add_policy_enforcement_for_metadef_delete_apis-95d2b16cc444840a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/alembic-migrations-902b31edae7a5d7d.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/antelope-milestone-2-d89e39412f9c0334.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/antelope-milestone-3-b9a4f7fdba31f628.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/api-2-6-current-9eeb83b7ecc0a562.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/api-2.16-8417b1e23322fedb.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/api-minor-ver-bump-2-6-aa3591fc58f08055.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/api-minor-version-bump-bbd69dc457fc731c.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/bp-barbican-secret-deletion-support-40cffa5ffa33447e.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/bp-inject-image-metadata-0a08af539bcce7f2.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/bug-1537903-54b2822eac6cfc09.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/bug-1980049-623d2eb0fa074136.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/cinder-store-migration-non-owner-80a2a8114d8602aa.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/consistent-store-names-57374b9505d530d0.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/copy-existing-image-94fd0b8d24bc16a0.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-admin_role-2f9d33ed0785d082.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-allow_additional_image_props-0e3b2f1ffa4e55e1.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-checksum-a602853403e1c4a8.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-5cb692fe889eb52b.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-registry-ff286df90df793f0.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-9890a1e961def2f6.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-continued-646f91b21cd771f7.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-show-multiple-location-continued-ussuri-16e8d9d8a59da1bc.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/deprecate-v1-api-6c7dbefb90fd8772.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/distributed-image-import-82cff4426731beac.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/experimental-multi-store-d2c26f9dbb9c835b.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/glare-ectomy-72a1f80f306f2e3b.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/image-tasks-api-f21b42eab91c2079.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/image-visibility-changes-fa5aa18dc67244c4.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/implement-lite-spec-db-sync-check-3e2e147aec0ae82b.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/import-locking-behavior-901c691f3839fe0a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/import-multi-stores-3e781f2878b3134d.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/improved-config-options-221c58a8c37602ba.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/location-add-status-checks-b70db66100bc96b7.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/make-task-api-admin-only-by-default-7def996262e18f7a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/multihash-081466a98601da20.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/multihash-081466a98601da20.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/mutistore-support-for-scrubber-6b360394ef32774a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/new_image_filters-c888361e6ecf495c.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/newton-1-release-065334d464f78fc5.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/newton-bugs-06ed3727b973c271.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/oslo-log-use-stderr-changes-07f5daf3e6abdcd6.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/pike-metadefs-changes-95b54e0bf8bbefd6.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/pike-rc-1-a5d3f6e8877b52c6.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/pike-rc-2-acc173005045e16a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/policy-in-code-7e0c6c070d32d136.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/policy-in-code-implications-438449a73af2893c.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/policy-refactor-xena-0cddb7f2d492cb3a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/queens-metadefs-changes-daf02bef18d049f4.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/queens-uwsgi-issues-4cee9e4fdf62c646.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/range-header-request-83cf11eebf865fb1.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/rbac-updates-ba0fcb886fe4085c.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/remove-enforce-secure-rbac-ec9a0249870460c2.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/remove-osprofiler-paste-ini-options-c620dedc8f9728ff.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/remove_native_ssl-c16d5a127b57583d.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/reordered-store-config-opts-newton-3a6575b5908c0e0f.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/restrict_location_updates-05454bb765a8c92c.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/rethinking-filesystem-access-120bc46064b3d40a.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/rocky-rc-b0ea7628b7a74c96.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/secure-rbac-project-personas-fb0d9792b9dc3783.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/train-metadefs-changes-c4380754cdd13a19.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/use-cursive-c6b15d94845232da.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/use-cursive-c6b15d94845232da.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/use-webob-1.8.1-5c3cd1b1382f063e.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/ussuri-final-b377a21508ada060.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/ussuri-final-b377a21508ada060.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/victoria-m2-release-notes-8a6ae2fdb3d29dae.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/victoria-m3-releasenotes-9209cea98a29abc4.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/victoria-rc1-release-notes-d928355cf90d608d.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/wsgi-containerization-369880238a5e793d.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/xena-m3-releasenotes-a92d55d29eecc8f6.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/xena-rc1-release-notes-12dbe0ac528ce483.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/yoga-rc1-release-notes-153932161f52a038.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-1-592415040e67924e.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-2-a782e75cdbd8fe13.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml` & `glance-28.0.0.0rc1/releasenotes/notes/zed-milestone-3-3e38697ae4677a81.yaml`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/source/conf.py` & `glance-28.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `glance-28.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `glance-28.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `glance-28.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `glance-28.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/requirements.txt` & `glance-28.0.0.0rc1/requirements.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# The order of packages is significant, because pip processes them in the order
-# of appearance. Changing the order has an impact on the overall integration
-# process, which may cause wedges in the gate later.
-
 pbr>=3.1.1 # Apache-2.0
 defusedxml>=0.6.0 # PSF
 
 # < 0.8.0/0.8 does not work, see https://bugs.launchpad.net/bugs/1153983
 SQLAlchemy>=1.3.14 # MIT
 eventlet>=0.33.3 # MIT
 PasteDeploy>=1.5.0 # MIT
```

### Comparing `glance-28.0.0.0b2/setup.cfg` & `glance-28.0.0.0rc1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 data_files = 
 	etc/glance =
 	etc/glance-api.conf
 	etc/glance-cache.conf
 	etc/glance-manage.conf
```

### Comparing `glance-28.0.0.0b2/setup.py` & `glance-28.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/test-requirements.txt` & `glance-28.0.0.0rc1/test-requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-# The order of packages is significant, because pip processes them in the order
-# of appearance. Changing the order has an impact on the overall integration
-# process, which may cause wedges in the gate later.
-
 # Hacking already pins down pep8, pyflakes and flake8
-hacking>=3.0.1,<3.1.0 # Apache-2.0
+hacking>=6.1.0,<6.2.0 # Apache-2.0
 
 # Needed for testing
 coverage!=4.4,>=4.0 # Apache-2.0
 ddt>=1.0.1 # MIT
 fixtures>=3.0.0 # Apache-2.0/BSD
 requests>=2.18.0 # Apache-2.0
 testrepository>=0.0.18 # Apache-2.0/BSD
```

### Comparing `glance-28.0.0.0b2/tools/test-setup.sh` & `glance-28.0.0.0rc1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/tools/test_format_inspector.py` & `glance-28.0.0.0rc1/tools/test_format_inspector.py`

 * *Files identical despite different names*

### Comparing `glance-28.0.0.0b2/tox.ini` & `glance-28.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

