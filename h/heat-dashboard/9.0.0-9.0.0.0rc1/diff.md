# Comparing `tmp/heat-dashboard-9.0.0.tar.gz` & `tmp/heat-dashboard-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heat-dashboard-9.0.0.tar", last modified: Wed Mar 22 12:20:30 2023, max compression
+gzip compressed data, was "heat-dashboard-9.0.0.0rc1.tar", last modified: Thu Mar  2 11:37:48 2023, max compression
```

## Comparing `heat-dashboard-9.0.0.tar` & `heat-dashboard-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,639 +1,639 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/.eslintignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8434 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/.eslintrc.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7275 2023-03-22 12:20:29.000000 heat-dashboard-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29430 2023-03-22 12:20:29.000000 heat-dashboard-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3189 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/configuration/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/contributor/devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7280 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/user/stacks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1883 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/doc/source/user/template_generator.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.332453 heat-dashboard-9.0.0/heat_dashboard/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8937 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/api/heat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/api/rest/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/api/rest/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/api/rest/heat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/conf/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/conf/default_policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37275 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/conf/default_policies/heat.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9380 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/conf/heat_policy.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/templates/resource_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/templates/resource_types/_details.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/templates/stacks.resource_types/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/templates/stacks.resource_types/_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2866 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/resource_types/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.340458 heat-dashboard-9.0.0/heat_dashboard/content/stacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20603 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14244 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/mappings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/sro.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15443 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6671 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.344460 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_change_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_detail_events.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_detail_resources.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_detail_topology.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_preview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_preview_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_preview_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_resource_info.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_resource_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_select_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_stack_info.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_stack_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/change_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/create.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/preview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/preview_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/preview_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/select_template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12948 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/stacks/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.344460 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8672 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.344460 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/templates/template_generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/templates/template_generator/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_generator/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.344460 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/stacks.template_versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/stacks.template_versions/_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/stacks.template_versions/index.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/template_versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/template_versions/_details.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/templates/template_versions/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/content/template_versions/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/_1610_project_orchestration_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/_1620_project_stacks_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/_1630_project_resource_types_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/_1640_project_template_versions_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3610 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/_1650_project_template_generator_panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/local_settings.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/local_settings.d/_1699_orchestration_settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/local_settings.d/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10900 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/cs/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14964 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/de/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/de/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/locale/en_AU/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/en_AU/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10181 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/en_AU/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13933 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.316444 heat-dashboard-9.0.0/heat_dashboard/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10249 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/es/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14551 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/fr/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/fr/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.348463 heat-dashboard-9.0.0/heat_dashboard/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13815 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/id/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/id/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10007 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/it/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15380 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ja/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3057 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ja/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18231 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/ne/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21599 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ne/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4512 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ne/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/pl_PL/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/pl_PL/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10003 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/pl_PL/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3285 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18916 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ru/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/ru/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10735 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/tr_TR/LC_MESSAGES/django.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.352465 heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13228 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.368474 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/apple-touch-icon.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11458 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/drag.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10174 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/favicon.ico
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6291 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2512 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5388 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5912 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7411 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2479 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5927 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo-splash.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5718 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6345 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6532 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5110 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2023-03-22 12:20:06.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/safari-pinned-tab.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5258 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6380 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2824 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2844 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2824 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/spinner.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13372 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4595 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5811 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10026 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5760 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8461 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.gif
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-red.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.368474 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/actions-checked-selected.template.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4245 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/check.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/create.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/delete.service.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.372476 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   540294 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-material.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-notify.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen-main.scss
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3761 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.372476 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/file-text-o.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/floppy-o.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/ic_close_24px.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/ic_help_outline_24px.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/spinner.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/trash.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27924 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/vis.scss
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.320446 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.380481 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2104 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3858 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3919 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4510 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4287 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7405 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8986 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11955 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8943 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4165 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9559 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10672 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10575 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8408 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.spec.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.380481 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)  1242315 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-material.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7461 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-notify.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)  1398089 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/vis.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.384483 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2953 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.388486 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3094 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5707 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.388486 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3519 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4203 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.388486 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.392488 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2432 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2495 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8554 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5655 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.392488 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5957 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5516 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5152 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10323 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.396490 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2644 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5441 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4059 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2632 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.396490 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5224 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7137 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.396490 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3033 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingassociation.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5653 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3618 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.400493 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5497 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.400493 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10313 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9820 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.400493 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6405 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6999 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.404495 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6221 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3163 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.404495 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5730 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3001 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.408497 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3156 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9238 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.408497 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3152 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3152 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.408497 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2043 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27869 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27200 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13288 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-blue.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1949 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-gray.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-green.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-red.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3830 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2843 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.spec.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.svg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/depends_on.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_draft.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_edge.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_resource.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_template.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15760 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/test/integration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/horizon.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.412500 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/resourcetypespage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/stackspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/templategeneratorpage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/templateversionspage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/integration/test_basic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.416502 heat-dashboard-9.0.0/heat_dashboard/test/test_data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8610 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/cinder_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15960 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/glance_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16876 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/heat_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13127 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/keystone_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7877 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/neutron_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7521 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/nova_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4311 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/test_data/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.416502 heat-dashboard-9.0.0/heat_dashboard/test/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.416502 heat-dashboard-9.0.0/heat_dashboard/test/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13904 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/api/test_heat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/api/test_heat_rest.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.416502 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_resource_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38379 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_stacks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5292 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_template_generator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_template_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.336456 heat-dashboard-9.0.0/heat_dashboard.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42850 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2023-03-22 12:20:30.000000 heat-dashboard-9.0.0/heat_dashboard.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/karma.conf.js
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/package.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/drop-py-2-7-3dafc6e9e6f29bda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/drop-python-3-6-and-3-7-b7319859be66ed72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/enabled_file_for_tmplgen-71432805cbfe4176.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/policy-in-code-support-42c02d6b73e770ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/split-out-from-horizon-1d1eabed58eb885e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/notes/template-generator-panel-decc3ec172bfa1dd.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8961 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/cs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5019 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6180 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.324449 heat-dashboard-9.0.0/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.420504 heat-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4116 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2524 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4335 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/ne/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/ne/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/ne/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4093 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.328451 heat-dashboard-9.0.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-03-22 12:20:30.424507 heat-dashboard-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2970 2023-03-22 12:20:07.000000 heat-dashboard-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/.eslintignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8434 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/.eslintrc.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7275 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29440 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.415708 heat-dashboard-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.415708 heat-dashboard-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3189 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/configuration/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/contributor/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7280 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/user/stacks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1883 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/doc/source/user/template_generator.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/heat_dashboard/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1540 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8937 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/heat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/rest/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/rest/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/api/rest/heat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/default_policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37275 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/default_policies/heat.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9380 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/heat_policy.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1162 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/templates/resource_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/templates/resource_types/_details.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/templates/stacks.resource_types/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/templates/stacks.resource_types/_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2866 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.423709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20603 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14244 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/sro.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15443 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6671 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.427709 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_change_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      214 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_detail_events.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_detail_resources.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_detail_topology.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_preview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1582 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_preview_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_preview_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_resource_info.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_resource_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_select_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_stack_info.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_stack_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/change_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/create.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/preview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/preview_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/preview_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/select_template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12948 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8672 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/templates/template_generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/templates/template_generator/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1115 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1778 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/stacks.template_versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/stacks.template_versions/_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/stacks.template_versions/index.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/template_versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/template_versions/_details.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/templates/template_versions/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2212 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.431710 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1152 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1610_project_orchestration_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1620_project_stacks_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1630_project_resource_types_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1070 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1640_project_template_versions_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3610 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1650_project_template_generator_panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      757 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/local_settings.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1312 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/local_settings.d/_1699_orchestration_settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/local_settings.d/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10900 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/cs/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14964 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_AU/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_AU/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10181 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_AU/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13933 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2987 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10249 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14551 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3497 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13815 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10007 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/it/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15380 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3057 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18231 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21599 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4512 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pl_PL/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pl_PL/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10003 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pl_PL/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.403707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.435710 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14621 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3285 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.439711 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18916 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.439711 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10735 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/tr_TR/LC_MESSAGES/django.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.439711 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13228 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2600 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.455712 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4465 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2277 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      923 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/apple-touch-icon.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5665 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11458 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/drag.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10174 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/favicon.ico
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6291 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3085 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5596 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2512 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5388 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5912 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7210 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3073 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7411 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2479 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5927 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo-splash.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5718 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6345 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6532 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5110 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3122 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/safari-pinned-tab.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5258 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6380 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2824 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2844 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2824 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/spinner.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13372 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4595 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4903 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5811 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10026 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5760 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8461 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.gif
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2916 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-red.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.455712 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/actions-checked-selected.template.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4245 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/check.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/create.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4333 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/delete.service.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.455712 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   540294 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-material.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-notify.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen-main.scss
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3761 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.459713 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/file-text-o.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/floppy-o.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/ic_close_24px.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/ic_help_outline_24px.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/spinner.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1045 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/trash.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2302 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27924 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/vis.scss
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.463714 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2104 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3858 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      897 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2690 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3919 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1565 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      707 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1053 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3550 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4510 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4287 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7405 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8986 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11955 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8943 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6920 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5618 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4165 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      836 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9559 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10672 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10575 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8408 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.spec.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.467714 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)  1242315 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-material.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7461 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-notify.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)  1398089 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/vis.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.407707 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.471714 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2804 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7753 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2953 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.471714 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5713 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2211 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6085 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3094 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5707 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.475715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1110 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3519 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4203 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1783 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.475715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1007 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1011 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1998 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.475715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2432 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2495 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8554 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5655 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4642 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.479715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10339 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10357 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5957 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5516 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5152 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10323 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.479715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2644 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2627 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2637 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3259 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5441 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4059 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2632 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.479715 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2186 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5224 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7137 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.483716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3033 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingassociation.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3611 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3619 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5653 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3618 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.483716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5497 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1538 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.483716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2242 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10313 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9820 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5424 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.487716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1354 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6405 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6999 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3923 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.487716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2995 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3005 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1925 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6221 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3163 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3006 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.491716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5730 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3001 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2184 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.491716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3156 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9238 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5535 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.491716 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3152 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3152 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3151 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2740 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3147 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.495717 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2043 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27869 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27200 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13288 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2045 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.495717 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-blue.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1949 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-gray.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-green.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-red.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3608 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3830 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2843 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.spec.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.svg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.495717 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      747 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/depends_on.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1149 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_draft.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2092 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_edge.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_resource.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_template.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.495717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15760 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.495717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/horizon.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/resourcetypespage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/stackspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/templategeneratorpage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/templateversionspage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/test_basic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8610 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/cinder_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15960 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/glance_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16876 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/heat_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13127 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/keystone_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7877 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/neutron_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7521 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/nova_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4311 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.499717 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13904 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/test_heat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2641 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/test_heat_rest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.503718 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1841 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_resource_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38379 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_stacks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5292 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_template_generator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_template_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.419709 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42850 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       15 2023-03-02 11:37:48.000000 heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/karma.conf.js
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      830 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/package.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.503718 heat-dashboard-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-3dafc6e9e6f29bda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-b7319859be66ed72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/enabled_file_for_tmplgen-71432805cbfe4176.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/policy-in-code-support-42c02d6b73e770ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/split-out-from-horizon-1d1eabed58eb885e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/notes/template-generator-panel-decc3ec172bfa1dd.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.503718 heat-dashboard-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.503718 heat-dashboard-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8961 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5019 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6180 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4116 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2524 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4335 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ne/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ne/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ne/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4093 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7352 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.411707 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4025 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-03-02 11:37:48.507718 heat-dashboard-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2970 2023-03-02 11:37:20.000000 heat-dashboard-9.0.0.0rc1/tox.ini
```

### Comparing `heat-dashboard-9.0.0/.eslintrc.js` & `heat-dashboard-9.0.0.0rc1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/.zuul.yaml` & `heat-dashboard-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/AUTHORS` & `heat-dashboard-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/CONTRIBUTING.rst` & `heat-dashboard-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/ChangeLog` & `heat-dashboard-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Update \`\`bindep.txt\`\` to sync with the horizon
 * Imported Translations from Zanata
 * Imported Translations from Zanata
 * Imported Translations from Zanata
 * Switch to 2023.1 Python3 unit tests and generic template name
 * Update master for stable/zed
```

### Comparing `heat-dashboard-9.0.0/LICENSE` & `heat-dashboard-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/PKG-INFO` & `heat-dashboard-9.0.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Heat Management Dashboard
 Home-page: https://docs.openstack.org/heat-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========================
         Welcome to Heat Dashboard!
```

### Comparing `heat-dashboard-9.0.0/README.rst` & `heat-dashboard-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/devstack/plugin.sh` & `heat-dashboard-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/conf.py` & `heat-dashboard-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/configuration/configuration.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/configuration/configuration.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/contributor/contributing.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/index.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/install/index.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/user/stacks.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/user/stacks.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/doc/source/user/template_generator.rst` & `heat-dashboard-9.0.0.0rc1/doc/source/user/template_generator.rst`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/api/__init__.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/api/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/api/heat.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/api/heat.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/api/rest/__init__.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/api/rest/heat.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/api/rest/heat.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/conf/default_policies/heat.yaml` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/default_policies/heat.yaml`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/conf/heat_policy.yaml` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/conf/heat_policy.yaml`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/resource_types/panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/resource_types/tables.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/tables.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/resource_types/tabs.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/tabs.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/resource_types/urls.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/urls.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/resource_types/views.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/resource_types/views.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/api.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/api.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/forms.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/forms.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/mappings.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/mappings.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/sro.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/sro.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/tables.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/tables.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/tabs.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/tabs.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_detail_overview.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_detail_overview.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_preview_details.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_preview_details.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_resource_overview.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_resource_overview.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/_select_template.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/_select_template.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/templates/stacks/index.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/templates/stacks/index.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/urls.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/urls.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/stacks/views.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/stacks/views.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_generator/api.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/api.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_generator/panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_generator/templates/template_generator/index.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/templates/template_generator/index.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_generator/urls.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/urls.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_generator/views.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_generator/views.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_versions/panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_versions/tables.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/tables.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_versions/tabs.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/tabs.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_versions/urls.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/urls.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/content/template_versions/views.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/content/template_versions/views.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/enabled/_1610_project_orchestration_panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1610_project_orchestration_panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/enabled/_1620_project_stacks_panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1620_project_stacks_panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/enabled/_1630_project_resource_types_panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1630_project_resource_types_panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/enabled/_1640_project_template_versions_panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1640_project_template_versions_panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/enabled/_1650_project_template_generator_panel.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/enabled/_1650_project_template_generator_panel.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/exceptions.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/exceptions.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/local_settings.d/_1699_orchestration_settings.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/local_settings.d/_1699_orchestration_settings.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/cs/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/de/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/de/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/en_AU/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_AU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/en_GB/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/es/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/fr/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/fr/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/id/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/id/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/it/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ja/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ja/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ko_KR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ne/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ne/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ne/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/pl_PL/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/pt_BR/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ru/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/ru/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/tr_TR/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/LC_MESSAGES/django.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/alarm-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/apple-touch-icon.png` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/config-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/db-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/favicon.ico` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/firewall-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/flavor-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/floatingip-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/image-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/keypair-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/lb-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo-splash.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo-splash.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/logo.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/network-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/policy-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/port-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/router-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/safari-pinned-tab.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/safari-pinned-tab.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/securitygroup-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/server-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/spinner.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/spinner.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/stack-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/unknown-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/volume-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/vpn.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.gif` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.gif`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/img/wait-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/check.service.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/check.service.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/create.service.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/create.service.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/delete.service.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/stacks/actions/delete.service.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-material.scss` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-material.scss`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-notify.scss` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/angular-notify.scss`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen.scss` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/hotgen.scss`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/file-text-o.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/file-text-o.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/floppy-o.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/floppy-o.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/spinner.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/spinner.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/trash.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/trash.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/img/icons/unknown.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/vis.scss` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/css/vis.scss`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/agent.module.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/compile.directive.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/dependson.directive.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/draggable.directive.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/droppable.directive.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/globals.service.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/icons.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/loading.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/menu.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-draft.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-edge.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-node.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/modal-template.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/states.service.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/template-generator.module.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/utils.module.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/components/vis-network.controller.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-material.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-material.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-notify.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/angular-notify.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/vis.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/libs/vis.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volume/os__cinder__volume.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__cinder__volumeattachment/os__cinder__volumeattachment.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__recordset/os__designate__recordset.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__designate__zone/os__designate__zone.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__autoscalinggroup/os__heat__autoscalinggroup.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__resourcegroup/os__heat__resourcegroup.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__heat__scalingpolicy/os__heat__scalingpolicy.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingip/os__neutron__floatingip.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingassociation.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingassociation.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__floatingipassociation/os__neutron__floatingipassociation.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__net/os__neutron__net.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__port/os__neutron__port.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__router/os__neutron__router.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__routerinterface/os__neutron__routerinterface.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__securitygroup/os__neutron__securitygroup.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__neutron__subnet/os__neutron__subnet.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__keypair/os__nova__keypair.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__nova__server/os__nova__server.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-blue.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-blue.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-gray.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-gray.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-green.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-green.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-red.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container-red.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.spec.js` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.spec.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.svg` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/js/resources/os__swift__container/os__swift__container.svg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/depends_on.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/depends_on.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_draft.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_draft.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_edge.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_edge.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_resource.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_resource.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_template.html` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/static/dashboard/project/heat_dashboard/template_generator/templates/modal_template.html`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/helpers.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/helpers.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/resourcetypespage.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/resourcetypespage.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/stackspage.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/stackspage.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/templategeneratorpage.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/templategeneratorpage.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/integration/pages/project/orchestration/templateversionspage.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/pages/project/orchestration/templateversionspage.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/integration/test_basic.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/integration/test_basic.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/settings.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/settings.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/cinder_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/cinder_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/exceptions.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/exceptions.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/glance_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/glance_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/heat_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/heat_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/keystone_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/keystone_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/neutron_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/neutron_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/nova_data.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/nova_data.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/test_data/utils.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/test_data/utils.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/api/test_heat.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/test_heat.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/api/test_heat_rest.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/api/test_heat_rest.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_resource_types.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_resource_types.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_stacks.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_stacks.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_template_generator.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_template_generator.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard/test/tests/content/test_template_versions.py` & `heat-dashboard-9.0.0.0rc1/heat_dashboard/test/tests/content/test_template_versions.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/heat_dashboard.egg-info/PKG-INFO` & `heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: heat-dashboard
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Heat Management Dashboard
 Home-page: https://docs.openstack.org/heat-dashboard/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==========================
         Welcome to Heat Dashboard!
```

### Comparing `heat-dashboard-9.0.0/heat_dashboard.egg-info/SOURCES.txt` & `heat-dashboard-9.0.0.0rc1/heat_dashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/karma.conf.js` & `heat-dashboard-9.0.0.0rc1/karma.conf.js`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/manage.py` & `heat-dashboard-9.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/package.json` & `heat-dashboard-9.0.0.0rc1/package.json`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/notes/enabled_file_for_tmplgen-71432805cbfe4176.yaml` & `heat-dashboard-9.0.0.0rc1/releasenotes/notes/enabled_file_for_tmplgen-71432805cbfe4176.yaml`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/conf.py` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/cs/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/ne/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ne/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/pt_BR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/ru/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `heat-dashboard-9.0.0.0rc1/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/requirements.txt` & `heat-dashboard-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/setup.cfg` & `heat-dashboard-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/setup.py` & `heat-dashboard-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/test-requirements.txt` & `heat-dashboard-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `heat-dashboard-9.0.0/tox.ini` & `heat-dashboard-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

