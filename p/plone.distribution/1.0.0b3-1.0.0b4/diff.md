# Comparing `tmp/plone.distribution-1.0.0b3.tar.gz` & `tmp/plone.distribution-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0b3.tar", last modified: Fri Mar  8 12:20:47 2024, max compression
+gzip compressed data, was "plone.distribution-1.0.0b4.tar", last modified: Wed Apr  3 10:04:16 2024, max compression
```

## Comparing `plone.distribution-1.0.0b3.tar` & `plone.distribution-1.0.0b4.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.096521 plone.distribution-1.0.0b3/
--rw-r--r--   0 maurits    (501) staff       (20)     1365 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      538 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      709 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      740 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     2024 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)     2846 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/CHANGES.md
--rw-r--r--   0 maurits    (501) staff       (20)       95 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/CONTRIBUTING.md
--rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/LICENSE
--rw-r--r--   0 maurits    (501) staff       (20)      299 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     5109 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/Makefile
--rw-r--r--   0 maurits    (501) staff       (20)    12869 2024-03-08 12:20:47.095826 plone.distribution-1.0.0b3/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8816 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/README.md
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/constraints.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.061379 plone.distribution-1.0.0b3/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     7078 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/Makefile
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.062478 plone.distribution-1.0.0b3/docs/_static/
--rw-r--r--   0 maurits    (501) staff       (20)     5430 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/_static/favicon.ico
--rw-r--r--   0 maurits    (501) staff       (20)     3775 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/_static/logo.svg
--rw-r--r--   0 maurits    (501) staff       (20)       30 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/_static/print.css
--rw-r--r--   0 maurits    (501) staff       (20)     7814 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/_static/styles.css
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.063406 plone.distribution-1.0.0b3/docs/api/
--rw-r--r--   0 maurits    (501) staff       (20)      469 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/api/distribution.md
--rw-r--r--   0 maurits    (501) staff       (20)      709 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/api/index.md
--rw-r--r--   0 maurits    (501) staff       (20)      439 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/api/site.md
--rw-r--r--   0 maurits    (501) staff       (20)     2813 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/conf.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.063700 plone.distribution-1.0.0b3/docs/development/
--rw-r--r--   0 maurits    (501) staff       (20)       26 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/development/index.md
--rw-r--r--   0 maurits    (501) staff       (20)     1329 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/index.md
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.064859 plone.distribution-1.0.0b3/docs/usage/
--rw-r--r--   0 maurits    (501) staff       (20)     2560 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/usage/code-examples.md
--rw-r--r--   0 maurits    (501) staff       (20)     2528 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/usage/index.md
--rw-r--r--   0 maurits    (501) staff       (20)     5886 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/usage/package-structure.md
--rw-r--r--   0 maurits    (501) staff       (20)     2683 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/docs/usage/zcml.md
--rw-r--r--   0 maurits    (501) staff       (20)      172 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/instance.yaml
--rw-r--r--   0 maurits    (501) staff       (20)      251 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/mx.ini
--rw-r--r--   0 maurits    (501) staff       (20)     4578 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      393 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/requirements-docs.txt
--rw-r--r--   0 maurits    (501) staff       (20)       33 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/requirements.txt
--rw-r--r--   0 maurits    (501) staff       (20)       38 2024-03-08 12:20:47.096612 plone.distribution-1.0.0b3/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2448 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.050865 plone.distribution-1.0.0b3/src/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.065124 plone.distribution-1.0.0b3/src/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.071064 plone.distribution-1.0.0b3/src/plone/distribution/
--rw-r--r--   0 maurits    (501) staff       (20)      221 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.071813 plone.distribution-1.0.0b3/src/plone/distribution/api/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/api/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1912 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/api/distribution.py
--rw-r--r--   0 maurits    (501) staff       (20)     6617 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/api/site.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.073274 plone.distribution-1.0.0b3/src/plone/distribution/browser/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2547 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/admin.py
--rw-r--r--   0 maurits    (501) staff       (20)      970 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1286 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/image.py
--rw-r--r--   0 maurits    (501) staff       (20)     1055 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.074994 plone.distribution-1.0.0b3/src/plone/distribution/browser/static/
--rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-logo.png
--rw-r--r--   0 maurits    (501) staff       (20)     2240 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-overview.min.css
--rw-r--r--   0 maurits    (501) staff       (20)   581628 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-overview.min.js
--rw-r--r--   0 maurits    (501) staff       (20)      812 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone.svg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.075262 plone.distribution-1.0.0b3/src/plone/distribution/browser/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     1431 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/browser/templates/plone-overview.pt
--rw-r--r--   0 maurits    (501) staff       (20)      446 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3892 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/core.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.052397 plone.distribution-1.0.0b3/src/plone/distribution/distributions/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.076455 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.077486 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/
--rw-r--r--   0 maurits    (501) staff       (20)      336 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/defaultpages.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.079635 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/
--rw-r--r--   0 maurits    (501) staff       (20)     5166 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/1.json
--rw-r--r--   0 maurits    (501) staff       (20)     1324 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/2.json
--rw-r--r--   0 maurits    (501) staff       (20)     1885 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/3.json
--rw-r--r--   0 maurits    (501) staff       (20)     2261 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/4.json
--rw-r--r--   0 maurits    (501) staff       (20)     1881 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/5.json
--rw-r--r--   0 maurits    (501) staff       (20)     2256 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/6.json
--rw-r--r--   0 maurits    (501) staff       (20)      425 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/ordering.json
--rw-r--r--   0 maurits    (501) staff       (20)     2799 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/portlets.json
--rw-r--r--   0 maurits    (501) staff       (20)   293282 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/image.png
--rw-r--r--   0 maurits    (501) staff       (20)      148 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/profiles.json
--rw-r--r--   0 maurits    (501) staff       (20)     1280 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/schema.json
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.081247 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.052624 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/content/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.081553 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/content/items/
--rw-r--r--   0 maurits    (501) staff       (20)      712 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/content/items/1.json
--rw-r--r--   0 maurits    (501) staff       (20)   218233 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/image.png
--rw-r--r--   0 maurits    (501) staff       (20)      175 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/profiles.json
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/schema.json
--rw-r--r--   0 maurits    (501) staff       (20)      514 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/distributions.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.083389 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1266 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5172 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/dist_export.py
--rw-r--r--   0 maurits    (501) staff       (20)     4696 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/dist_import.py
--rw-r--r--   0 maurits    (501) staff       (20)     2762 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/helpers.py
--rw-r--r--   0 maurits    (501) staff       (20)      522 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     2735 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/serializer.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.084016 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/templates/
--rw-r--r--   0 maurits    (501) staff       (20)     3756 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/templates/export_all.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1241 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/exportimport/templates/import_all.pt
--rw-r--r--   0 maurits    (501) staff       (20)     1457 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/handler.py
--rw-r--r--   0 maurits    (501) staff       (20)      698 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)      391 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/meta.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     3531 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/metaconfigure.py
--rw-r--r--   0 maurits    (501) staff       (20)     4174 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/registry.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.084763 plone.distribution-1.0.0b3/src/plone/distribution/services/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.085543 plone.distribution-1.0.0b3/src/plone/distribution/services/auth/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/auth/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      348 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/auth/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1301 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/auth/login.py
--rw-r--r--   0 maurits    (501) staff       (20)      412 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)      582 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/overrides.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.086844 plone.distribution-1.0.0b3/src/plone/distribution/services/sites/
--rw-r--r--   0 maurits    (501) staff       (20)       77 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/sites/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     2105 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/sites/add.py
--rw-r--r--   0 maurits    (501) staff       (20)      895 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/sites/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     4882 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/sites/get.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.087568 plone.distribution-1.0.0b3/src/plone/distribution/services/system/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/system/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      332 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/system/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     1112 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/services/system/get.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.088343 plone.distribution-1.0.0b3/src/plone/distribution/testing/
--rw-r--r--   0 maurits    (501) staff       (20)      149 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/testing/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3129 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/testing/layer.py
--rw-r--r--   0 maurits    (501) staff       (20)     1017 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/testing/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.089352 plone.distribution-1.0.0b3/src/plone/distribution/utils/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      914 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/utils/request.py
--rw-r--r--   0 maurits    (501) staff       (20)     5065 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/utils/schema.py
--rw-r--r--   0 maurits    (501) staff       (20)      870 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/src/plone/distribution/utils/validation.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.067553 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    12869 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     5018 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      365 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2024-03-08 12:20:47.000000 plone.distribution-1.0.0b3/src/plone.distribution.egg-info/top_level.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.089797 plone.distribution-1.0.0b3/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.090372 plone.distribution-1.0.0b3/tests/api/
--rw-r--r--   0 maurits    (501) staff       (20)     1524 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/api/test_api_distribution.py
--rw-r--r--   0 maurits    (501) staff       (20)     2152 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/api/test_api_site.py
--rw-r--r--   0 maurits    (501) staff       (20)      363 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/conftest.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.091332 plone.distribution-1.0.0b3/tests/distributions/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/distributions/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      322 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/distributions/conftest.py
--rw-r--r--   0 maurits    (501) staff       (20)     1895 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/distributions/test_distributions_classic.py
--rw-r--r--   0 maurits    (501) staff       (20)     1765 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/distributions/test_distributions_default.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.091889 plone.distribution-1.0.0b3/tests/exportimport/
--rw-r--r--   0 maurits    (501) staff       (20)    12736 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/exportimport/portal.json
--rw-r--r--   0 maurits    (501) staff       (20)     2344 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/exportimport/test_exportimport_helpers.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.092911 plone.distribution-1.0.0b3/tests/services/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/services/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      243 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/services/conftest.py
--rw-r--r--   0 maurits    (501) staff       (20)     4839 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/services/test_services_site.py
--rw-r--r--   0 maurits    (501) staff       (20)     2445 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/services/test_services_system.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.094205 plone.distribution-1.0.0b3/tests/utils/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      519 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/conftest.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-03-08 12:20:47.095297 plone.distribution-1.0.0b3/tests/utils/data/
--rw-r--r--   0 maurits    (501) staff       (20)      969 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/data/invalid.json
--rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/data/valid.json
--rw-r--r--   0 maurits    (501) staff       (20)     1328 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/data/with_default_language.json
--rw-r--r--   0 maurits    (501) staff       (20)     1205 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/test_utils_request.py
--rw-r--r--   0 maurits    (501) staff       (20)     2907 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/test_utils_schema.py
--rw-r--r--   0 maurits    (501) staff       (20)     1692 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tests/utils/test_utils_validation.py
--rw-r--r--   0 maurits    (501) staff       (20)     4885 2024-03-08 12:20:46.000000 plone.distribution-1.0.0b3/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.773026 plone.distribution-1.0.0b4/
+-rw-r--r--   0 maurits    (501) staff       (20)     1365 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      538 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      740 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     2024 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)     2927 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/CHANGES.md
+-rw-r--r--   0 maurits    (501) staff       (20)       95 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/CONTRIBUTING.md
+-rw-r--r--   0 maurits    (501) staff       (20)    18092 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/LICENSE
+-rw-r--r--   0 maurits    (501) staff       (20)      299 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5109 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/Makefile
+-rw-r--r--   0 maurits    (501) staff       (20)    12950 2024-04-03 10:04:16.772569 plone.distribution-1.0.0b4/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     8816 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/README.md
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/constraints.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.740184 plone.distribution-1.0.0b4/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     7078 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/Makefile
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.741349 plone.distribution-1.0.0b4/docs/_static/
+-rw-r--r--   0 maurits    (501) staff       (20)     5430 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/favicon.ico
+-rw-r--r--   0 maurits    (501) staff       (20)     3775 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/logo.svg
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/print.css
+-rw-r--r--   0 maurits    (501) staff       (20)     7814 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/_static/styles.css
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.742224 plone.distribution-1.0.0b4/docs/api/
+-rw-r--r--   0 maurits    (501) staff       (20)      469 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/distribution.md
+-rw-r--r--   0 maurits    (501) staff       (20)      709 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)      439 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/api/site.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2813 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/conf.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.742515 plone.distribution-1.0.0b4/docs/development/
+-rw-r--r--   0 maurits    (501) staff       (20)       26 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/development/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)     1329 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/index.md
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.743664 plone.distribution-1.0.0b4/docs/usage/
+-rw-r--r--   0 maurits    (501) staff       (20)     2560 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/code-examples.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2528 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/index.md
+-rw-r--r--   0 maurits    (501) staff       (20)     5886 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/package-structure.md
+-rw-r--r--   0 maurits    (501) staff       (20)     2683 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/docs/usage/zcml.md
+-rw-r--r--   0 maurits    (501) staff       (20)      172 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/instance.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)      251 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/mx.ini
+-rw-r--r--   0 maurits    (501) staff       (20)     4578 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      393 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/requirements-docs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       33 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/requirements.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-03 10:04:16.773104 plone.distribution-1.0.0b4/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2448 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.729261 plone.distribution-1.0.0b4/src/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.743964 plone.distribution-1.0.0b4/src/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.748906 plone.distribution-1.0.0b4/src/plone/distribution/
+-rw-r--r--   0 maurits    (501) staff       (20)      221 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.749722 plone.distribution-1.0.0b4/src/plone/distribution/api/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1912 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/distribution.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6617 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/api/site.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.751053 plone.distribution-1.0.0b4/src/plone/distribution/browser/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2547 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/admin.py
+-rw-r--r--   0 maurits    (501) staff       (20)      970 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1286 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/image.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1055 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.752952 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/
+-rw-r--r--   0 maurits    (501) staff       (20)     1185 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-logo.png
+-rw-r--r--   0 maurits    (501) staff       (20)     2240 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.css
+-rw-r--r--   0 maurits    (501) staff       (20)   581628 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.js
+-rw-r--r--   0 maurits    (501) staff       (20)      812 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone.svg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.753240 plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     1431 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/plone-overview.pt
+-rw-r--r--   0 maurits    (501) staff       (20)      446 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3892 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/core.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.730780 plone.distribution-1.0.0b4/src/plone/distribution/distributions/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.754442 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.755259 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/
+-rw-r--r--   0 maurits    (501) staff       (20)      336 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/defaultpages.json
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.756848 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/
+-rw-r--r--   0 maurits    (501) staff       (20)     5166 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/1.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1324 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/2.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1885 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/3.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2261 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/4.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1881 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/5.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2256 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/6.json
+-rw-r--r--   0 maurits    (501) staff       (20)      425 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/ordering.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2799 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/portlets.json
+-rw-r--r--   0 maurits    (501) staff       (20)   293282 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/profiles.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1280 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/schema.json
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.757941 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.731065 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.758191 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/items/
+-rw-r--r--   0 maurits    (501) staff       (20)      712 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/items/1.json
+-rw-r--r--   0 maurits    (501) staff       (20)   218233 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/image.png
+-rw-r--r--   0 maurits    (501) staff       (20)      175 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/profiles.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/schema.json
+-rw-r--r--   0 maurits    (501) staff       (20)      514 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/distributions.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.760076 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1415 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5172 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_export.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4696 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_import.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2762 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/helpers.py
+-rw-r--r--   0 maurits    (501) staff       (20)      522 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3345 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/serializer.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.760557 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/
+-rw-r--r--   0 maurits    (501) staff       (20)     3756 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/export_all.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1241 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/import_all.pt
+-rw-r--r--   0 maurits    (501) staff       (20)     1457 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/handler.py
+-rw-r--r--   0 maurits    (501) staff       (20)      698 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)      391 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/meta.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     3531 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/metaconfigure.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4174 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/registry.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.761435 plone.distribution-1.0.0b4/src/plone/distribution/services/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.762317 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      348 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1301 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/auth/login.py
+-rw-r--r--   0 maurits    (501) staff       (20)      412 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)      582 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/overrides.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.763397 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/
+-rw-r--r--   0 maurits    (501) staff       (20)       77 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2105 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/add.py
+-rw-r--r--   0 maurits    (501) staff       (20)      895 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     4882 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/sites/get.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.764201 plone.distribution-1.0.0b4/src/plone/distribution/services/system/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      332 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     1112 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/services/system/get.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.765060 plone.distribution-1.0.0b4/src/plone/distribution/testing/
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3129 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/layer.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1017 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/testing/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.766119 plone.distribution-1.0.0b4/src/plone/distribution/utils/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      914 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/request.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5065 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)      870 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone/distribution/utils/validation.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.746327 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    12950 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     5018 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      365 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/src/plone.distribution.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.766553 plone.distribution-1.0.0b4/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.767027 plone.distribution-1.0.0b4/tests/api/
+-rw-r--r--   0 maurits    (501) staff       (20)     1524 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/api/test_api_distribution.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2152 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/api/test_api_site.py
+-rw-r--r--   0 maurits    (501) staff       (20)      363 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/conftest.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.768329 plone.distribution-1.0.0b4/tests/distributions/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      322 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/conftest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1895 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/test_distributions_classic.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1765 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/distributions/test_distributions_default.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.769022 plone.distribution-1.0.0b4/tests/exportimport/
+-rw-r--r--   0 maurits    (501) staff       (20)    12736 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/exportimport/portal.json
+-rw-r--r--   0 maurits    (501) staff       (20)     2344 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/exportimport/test_exportimport_helpers.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.770071 plone.distribution-1.0.0b4/tests/services/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      243 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/conftest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4839 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/test_services_site.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2445 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/services/test_services_system.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.771480 plone.distribution-1.0.0b4/tests/utils/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      519 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/conftest.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-03 10:04:16.772176 plone.distribution-1.0.0b4/tests/utils/data/
+-rw-r--r--   0 maurits    (501) staff       (20)      969 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/invalid.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1267 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/valid.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1328 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/data/with_default_language.json
+-rw-r--r--   0 maurits    (501) staff       (20)     1205 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_request.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2907 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_schema.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1692 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tests/utils/test_utils_validation.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4885 2024-04-03 10:04:16.000000 plone.distribution-1.0.0b4/tox.ini
```

### Comparing `plone.distribution-1.0.0b3/.editorconfig` & `plone.distribution-1.0.0b4/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/.flake8` & `plone.distribution-1.0.0b4/.flake8`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/.gitignore` & `plone.distribution-1.0.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/.meta.toml` & `plone.distribution-1.0.0b4/.meta.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/.pre-commit-config.yaml` & `plone.distribution-1.0.0b4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/CHANGES.md` & `plone.distribution-1.0.0b4/CHANGES.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0b4 (2024-04-03)
+
+
+### Bug fixes:
+
+- Fix exporting files.
+  [pbauer] #58
+
 ## 1.0.0b3 (2024-03-08)
 
 
 ### Bug fixes:
 
 - Fix importing blocks on the site-root.
   [pbauer] #56
```

### Comparing `plone.distribution-1.0.0b3/LICENSE` & `plone.distribution-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/Makefile` & `plone.distribution-1.0.0b4/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/PKG-INFO` & `plone.distribution-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -350,14 +350,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0b4 (2024-04-03)
+
+
+### Bug fixes:
+
+- Fix exporting files.
+  [pbauer] #58
+
 ## 1.0.0b3 (2024-03-08)
 
 
 ### Bug fixes:
 
 - Fix importing blocks on the site-root.
   [pbauer] #56
```

### Comparing `plone.distribution-1.0.0b3/README.md` & `plone.distribution-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/Makefile` & `plone.distribution-1.0.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/_static/favicon.ico` & `plone.distribution-1.0.0b4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/_static/logo.svg` & `plone.distribution-1.0.0b4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/_static/styles.css` & `plone.distribution-1.0.0b4/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/api/index.md` & `plone.distribution-1.0.0b4/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/conf.py` & `plone.distribution-1.0.0b4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/index.md` & `plone.distribution-1.0.0b4/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/usage/code-examples.md` & `plone.distribution-1.0.0b4/docs/usage/code-examples.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/usage/index.md` & `plone.distribution-1.0.0b4/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/usage/package-structure.md` & `plone.distribution-1.0.0b4/docs/usage/package-structure.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/docs/usage/zcml.md` & `plone.distribution-1.0.0b4/docs/usage/zcml.md`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/pyproject.toml` & `plone.distribution-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/setup.py` & `plone.distribution-1.0.0b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.distribution",
-    version="1.0.0b3",
+    version="1.0.0b4",
     description="Plone distribution support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/api/distribution.py` & `plone.distribution-1.0.0b4/src/plone/distribution/api/distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/api/site.py` & `plone.distribution-1.0.0b4/src/plone/distribution/api/site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/admin.py` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/admin.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/configure.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/image.py` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/image.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/overrides.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-logo.png` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-logo.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-overview.min.css` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.css`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone-overview.min.js` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone-overview.min.js`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/static/plone.svg` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/static/plone.svg`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/browser/templates/plone-overview.pt` & `plone.distribution-1.0.0b4/src/plone/distribution/browser/templates/plone-overview.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/core.py` & `plone.distribution-1.0.0b4/src/plone/distribution/core.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/1.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/1.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/2.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/2.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/3.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/3.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/4.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/4.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/5.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/5.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/items/6.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/items/6.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/content/portlets.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/content/portlets.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/image.png` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/classic/schema.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/classic/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/content/items/1.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/content/items/1.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/image.png` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/image.png`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions/default/schema.json` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions/default/schema.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/distributions.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/distributions.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/configure.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/configure.zcml`

 * *Files 13% similar despite different names*

```diff
@@ -39,9 +39,11 @@
       class=".dist_import.ImportContent"
       permission="cmf.ManagePortal"
       />
 
   <!-- Serializers -->
   <adapter factory=".serializer.DistributionFileFieldSerializer" />
   <adapter factory=".serializer.DistributionImageFieldSerializer" />
+  <adapter factory=".serializer.DistributionSimpleFileFieldSerializer" />
+  <adapter factory=".serializer.DistributionSimpleImageFieldSerializer" />
 
 </configure>
```

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/dist_export.py` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_export.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/dist_import.py` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/dist_import.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/helpers.py` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/interfaces.py` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/serializer.py` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/serializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 from plone.dexterity.interfaces import IDexterityContent
 from plone.distribution.exportimport.interfaces import IDistributionBlobsMarker
+from plone.namedfile.interfaces import INamedBlobFileField
+from plone.namedfile.interfaces import INamedBlobImageField
 from plone.namedfile.interfaces import INamedFileField
 from plone.namedfile.interfaces import INamedImageField
 from plone.restapi.interfaces import IFieldSerializer
 from plone.restapi.serializer.converters import json_compatible
 from plone.restapi.serializer.dxfields import DefaultFieldSerializer
 from zope.component import adapter
 from zope.globalrequest import getRequest
@@ -12,15 +14,15 @@
 
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-@adapter(INamedFileField, IDexterityContent, IDistributionBlobsMarker)
+@adapter(INamedBlobFileField, IDexterityContent, IDistributionBlobsMarker)
 @implementer(IFieldSerializer)
 class DistributionFileFieldSerializer(DefaultFieldSerializer):
     def __call__(self):
         namedfile = self.field.get(self.context)
         if namedfile is None:
             return None
         blob_path = export_blob(
@@ -31,15 +33,21 @@
             "content-type": namedfile.contentType,
             "size": namedfile.getSize(),
             "blob_path": blob_path,
         }
         return json_compatible(result)
 
 
-@adapter(INamedImageField, IDexterityContent, IDistributionBlobsMarker)
+@adapter(INamedFileField, IDexterityContent, IDistributionBlobsMarker)
+@implementer(IFieldSerializer)
+class DistributionSimpleFileFieldSerializer(DistributionFileFieldSerializer):
+    """Same as above but less specific field interface"""
+
+
+@adapter(INamedBlobImageField, IDexterityContent, IDistributionBlobsMarker)
 @implementer(IFieldSerializer)
 class DistributionImageFieldSerializer(DefaultFieldSerializer):
     def __call__(self):
         namedfile = self.field.get(self.context)
         if namedfile is None:
             return None
         blob_path = export_blob(
@@ -53,14 +61,20 @@
             "width": width,
             "height": height,
             "blob_path": blob_path,
         }
         return json_compatible(result)
 
 
+@adapter(INamedImageField, IDexterityContent, IDistributionBlobsMarker)
+@implementer(IFieldSerializer)
+class DistributionSimpleImageFieldSerializer(DistributionImageFieldSerializer):
+    """Same as above but less specific field interface"""
+
+
 def export_blob(uid, fieldname, filename, data):
     """Store blob data in a way that makes it easier to edit by hand:
     <distribution>/content/blobs/<uid>-<fieldname>/<filename>"""
     unique_dir_name_for_file = f"{uid}-{fieldname}"
     request = getRequest()
     distribution_directory = Path(request["distribution_directory"])
     target_directory = distribution_directory / "blobs" / unique_dir_name_for_file
```

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/templates/export_all.pt` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/export_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/exportimport/templates/import_all.pt` & `plone.distribution-1.0.0b4/src/plone/distribution/exportimport/templates/import_all.pt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/handler.py` & `plone.distribution-1.0.0b4/src/plone/distribution/handler.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/interfaces.py` & `plone.distribution-1.0.0b4/src/plone/distribution/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/metaconfigure.py` & `plone.distribution-1.0.0b4/src/plone/distribution/metaconfigure.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/registry.py` & `plone.distribution-1.0.0b4/src/plone/distribution/registry.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/auth/login.py` & `plone.distribution-1.0.0b4/src/plone/distribution/services/auth/login.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/overrides.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/services/overrides.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/sites/add.py` & `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/add.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/sites/configure.zcml` & `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/sites/get.py` & `plone.distribution-1.0.0b4/src/plone/distribution/services/sites/get.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/services/system/get.py` & `plone.distribution-1.0.0b4/src/plone/distribution/services/system/get.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/testing/layer.py` & `plone.distribution-1.0.0b4/src/plone/distribution/testing/layer.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/testing/testing.py` & `plone.distribution-1.0.0b4/src/plone/distribution/testing/testing.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/utils/request.py` & `plone.distribution-1.0.0b4/src/plone/distribution/utils/request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/utils/schema.py` & `plone.distribution-1.0.0b4/src/plone/distribution/utils/schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone/distribution/utils/validation.py` & `plone.distribution-1.0.0b4/src/plone/distribution/utils/validation.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/src/plone.distribution.egg-info/PKG-INFO` & `plone.distribution-1.0.0b4/src/plone.distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.distribution
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Plone distribution support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -350,14 +350,22 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0b4 (2024-04-03)
+
+
+### Bug fixes:
+
+- Fix exporting files.
+  [pbauer] #58
+
 ## 1.0.0b3 (2024-03-08)
 
 
 ### Bug fixes:
 
 - Fix importing blocks on the site-root.
   [pbauer] #56
```

### Comparing `plone.distribution-1.0.0b3/src/plone.distribution.egg-info/SOURCES.txt` & `plone.distribution-1.0.0b4/src/plone.distribution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/api/test_api_distribution.py` & `plone.distribution-1.0.0b4/tests/api/test_api_distribution.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/api/test_api_site.py` & `plone.distribution-1.0.0b4/tests/api/test_api_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/distributions/test_distributions_classic.py` & `plone.distribution-1.0.0b4/tests/distributions/test_distributions_classic.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/distributions/test_distributions_default.py` & `plone.distribution-1.0.0b4/tests/distributions/test_distributions_default.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/exportimport/portal.json` & `plone.distribution-1.0.0b4/tests/exportimport/portal.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/exportimport/test_exportimport_helpers.py` & `plone.distribution-1.0.0b4/tests/exportimport/test_exportimport_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/services/test_services_site.py` & `plone.distribution-1.0.0b4/tests/services/test_services_site.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/services/test_services_system.py` & `plone.distribution-1.0.0b4/tests/services/test_services_system.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/conftest.py` & `plone.distribution-1.0.0b4/tests/utils/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/data/invalid.json` & `plone.distribution-1.0.0b4/tests/utils/data/invalid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/data/valid.json` & `plone.distribution-1.0.0b4/tests/utils/data/valid.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/data/with_default_language.json` & `plone.distribution-1.0.0b4/tests/utils/data/with_default_language.json`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/test_utils_request.py` & `plone.distribution-1.0.0b4/tests/utils/test_utils_request.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/test_utils_schema.py` & `plone.distribution-1.0.0b4/tests/utils/test_utils_schema.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tests/utils/test_utils_validation.py` & `plone.distribution-1.0.0b4/tests/utils/test_utils_validation.py`

 * *Files identical despite different names*

### Comparing `plone.distribution-1.0.0b3/tox.ini` & `plone.distribution-1.0.0b4/tox.ini`

 * *Files identical despite different names*

