# Comparing `tmp/aiohttp_admin2-0.0.4.tar.gz` & `tmp/aiohttp_admin2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_admin2-0.0.4.tar", max compression
+gzip compressed data, was "aiohttp_admin2-0.0.5.tar", max compression
```

## Comparing `aiohttp_admin2-0.0.4.tar` & `aiohttp_admin2-0.0.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     1075 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/LICENSE
--rw-r--r--   0        0        0     1154 2021-07-01 20:43:24.196491 aiohttp_admin2-0.0.4/README_BUILD.rst
--rw-r--r--   0        0        0      185 2021-07-01 20:43:26.232504 aiohttp_admin2-0.0.4/aiohttp_admin2/__init__.py
--rw-r--r--   0        0        0     1054 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/connection_injectors.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/__init__.py
--rw-r--r--   0        0        0    14520 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/controller.py
--rw-r--r--   0        0        0      178 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/exceptions.py
--rw-r--r--   0        0        0      428 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/mongo_controller.py
--rw-r--r--   0        0        0      762 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/mysql_controller.py
--rw-r--r--   0        0        0      783 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/postgres_controller.py
--rw-r--r--   0        0        0      876 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/relations.py
--rw-r--r--   0        0        0      444 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/types.py
--rw-r--r--   0        0        0       98 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/exceptions.py
--rw-r--r--   0        0        0       91 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/__init__.py
--rw-r--r--   0        0        0     4795 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/base.py
--rw-r--r--   0        0        0      321 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/exceptions.py
--rw-r--r--   0        0        0      916 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/__init__.py
--rw-r--r--   0        0        0     3354 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/abc.py
--rw-r--r--   0        0        0     1721 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/array_field.py
--rw-r--r--   0        0        0      379 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/bolean_field.py
--rw-r--r--   0        0        0     2992 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/choice_field.py
--rw-r--r--   0        0        0      637 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/date_field.py
--rw-r--r--   0        0        0      550 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/float_field.py
--rw-r--r--   0        0        0     1042 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/int_field.py
--rw-r--r--   0        0        0     1082 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/json_field.py
--rw-r--r--   0        0        0      410 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/mongo_fields.py
--rw-r--r--   0        0        0      376 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/string_field.py
--rw-r--r--   0        0        0     1553 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/url_field.py
--rw-r--r--   0        0        0     3748 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/generics.py
--rw-r--r--   0        0        0      124 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/validators/__init__.py
--rw-r--r--   0        0        0      900 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/validators/length.py
--rw-r--r--   0        0        0      578 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/validators/required.py
--rw-r--r--   0        0        0      386 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/__init__.py
--rw-r--r--   0        0        0     5964 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/abc.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/dict_resource/__init__.py
--rw-r--r--   0        0        0     5613 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/dict_resource/dict_resource.py
--rw-r--r--   0        0        0     2205 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/dict_resource/filters.py
--rw-r--r--   0        0        0      692 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/exceptions.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mongo_resource/__init__.py
--rw-r--r--   0        0        0     2677 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mongo_resource/filters.py
--rw-r--r--   0        0        0     5772 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mongo_resource/mongo_resource.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mysql_resource/__init__.py
--rw-r--r--   0        0        0     1465 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mysql_resource/mysql_resource.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/__init__.py
--rw-r--r--   0        0        0     4678 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/filters.py
--rw-r--r--   0        0        0     9322 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/postgres_resource.py
--rw-r--r--   0        0        0      542 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/utils.py
--rw-r--r--   0        0        0      228 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/resources/types.py
--rw-r--r--   0        0        0      688 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/__init__.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/__init__.py
--rw-r--r--   0        0        0     5307 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/admin.py
--rw-r--r--   0        0        0      916 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/exceptions.py
--rw-r--r--   0        0        0      745 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/setup.py
--rw-r--r--   0        0        0     4023 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/css/base.css
--rw-r--r--   0        0        0   160268 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/css/theme.css
--rw-r--r--   0        0        0     1217 2021-07-01 20:43:07.292384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/js/main.js
--rw-r--r--   0        0        0      508 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/cursor_pagination.html
--rw-r--r--   0        0        0      610 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/boolean_filter.html
--rw-r--r--   0        0        0      620 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/choice_filter.html
--rw-r--r--   0        0        0     2989 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/datetime_filter.html
--rw-r--r--   0        0        0      880 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/search_filter.html
--rw-r--r--   0        0        0      811 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/single_value_filter.html
--rw-r--r--   0        0        0      202 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/field_errors.html
--rw-r--r--   0        0        0      108 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/field_title.html
--rw-r--r--   0        0        0      686 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/array_field.html
--rw-r--r--   0        0        0      886 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/autocomplete_field.html
--rw-r--r--   0        0        0      549 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/boolean_field.html
--rw-r--r--   0        0        0      896 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/choice_field.html
--rw-r--r--   0        0        0      522 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/ck_editor_field.html
--rw-r--r--   0        0        0      298 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/date_field.html
--rw-r--r--   0        0        0     1143 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/datetime_field.html
--rw-r--r--   0        0        0      436 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/field.html
--rw-r--r--   0        0        0      620 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/file_field.html
--rw-r--r--   0        0        0     2474 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/image_field.html
--rw-r--r--   0        0        0     1393 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/json_field.html
--rw-r--r--   0        0        0      601 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/long_string_field.html
--rw-r--r--   0        0        0      605 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/string_field.html
--rw-r--r--   0        0        0     1788 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/form.html
--rw-r--r--   0        0        0      359 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/header.html
--rw-r--r--   0        0        0      402 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_action_buttons.html
--rw-r--r--   0        0        0      271 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_cell.html
--rw-r--r--   0        0        0     1306 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_block.html
--rw-r--r--   0        0        0     1135 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_header_block.html
--rw-r--r--   0        0        0      141 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/messages.html
--rw-r--r--   0        0        0     1094 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/nav_aside.html
--rw-r--r--   0        0        0     2705 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/pagination.html
--rw-r--r--   0        0        0      491 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/tabs_bar.html
--rw-r--r--   0        0        0     1671 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/base.html
--rw-r--r--   0        0        0      909 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/create_page.html
--rw-r--r--   0        0        0      207 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/custom_page.html
--rw-r--r--   0        0        0      173 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/custom_tab_page.html
--rw-r--r--   0        0        0      937 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/delete_page.html
--rw-r--r--   0        0        0     1488 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_edit_page.html
--rw-r--r--   0        0        0      347 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_view_page.html
--rw-r--r--   0        0        0      587 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_cursor_page.html
--rw-r--r--   0        0        0     1574 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_page.html
--rw-r--r--   0        0        0     1085 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/utils.py
--rw-r--r--   0        0        0        0 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/__init__.py
--rw-r--r--   0        0        0    14819 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/base.py
--rw-r--r--   0        0        0     8617 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/controller_view.py
--rw-r--r--   0        0        0      335 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/dashboard.py
--rw-r--r--   0        0        0     9391 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/many_to_many_tab_view.py
--rw-r--r--   0        0        0     1046 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/tab_base_view.py
--rw-r--r--   0        0        0      865 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/tab_template_view.py
--rw-r--r--   0        0        0      632 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/template_view.py
--rw-r--r--   0        0        0     2236 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/utils.py
--rw-r--r--   0        0        0     4272 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/filters.py
--rw-r--r--   0        0        0     3810 2021-07-01 20:43:07.296384 aiohttp_admin2-0.0.4/aiohttp_admin2/views/widgets.py
--rw-r--r--   0        0        0     1074 2021-07-01 20:43:26.228504 aiohttp_admin2-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     3038 2021-07-01 20:43:27.135065 aiohttp_admin2-0.0.4/setup.py
--rw-r--r--   0        0        0     2328 2021-07-01 20:43:27.135610 aiohttp_admin2-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1692 2021-10-09 20:31:07.238186 aiohttp_admin2-0.0.5/README_BUILD.rst
+-rw-r--r--   0        0        0      185 2021-10-09 20:31:09.054091 aiohttp_admin2-0.0.5/aiohttp_admin2/__init__.py
+-rw-r--r--   0        0        0     1054 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/connection_injectors.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/__init__.py
+-rw-r--r--   0        0        0    14520 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/controller.py
+-rw-r--r--   0        0        0      178 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/exceptions.py
+-rw-r--r--   0        0        0     1095 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/mongo_controller.py
+-rw-r--r--   0        0        0      630 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/mysql_controller.py
+-rw-r--r--   0        0        0     1413 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/postgres_controller.py
+-rw-r--r--   0        0        0      876 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/relations.py
+-rw-r--r--   0        0        0      444 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/types.py
+-rw-r--r--   0        0        0       98 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/exceptions.py
+-rw-r--r--   0        0        0       91 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/__init__.py
+-rw-r--r--   0        0        0     4903 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/base.py
+-rw-r--r--   0        0        0      321 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/exceptions.py
+-rw-r--r--   0        0        0      916 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/__init__.py
+-rw-r--r--   0        0        0     3357 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/abc.py
+-rw-r--r--   0        0        0     2807 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/array_field.py
+-rw-r--r--   0        0        0      750 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/bolean_field.py
+-rw-r--r--   0        0        0     3352 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/choice_field.py
+-rw-r--r--   0        0        0     1477 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/date_field.py
+-rw-r--r--   0        0        0      607 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/float_field.py
+-rw-r--r--   0        0        0     1259 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/int_field.py
+-rw-r--r--   0        0        0     1098 2021-10-09 20:30:48.858005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/json_field.py
+-rw-r--r--   0        0        0      464 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/mongo_fields.py
+-rw-r--r--   0        0        0      593 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/string_field.py
+-rw-r--r--   0        0        0     1923 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/url_field.py
+-rw-r--r--   0        0        0     4529 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/generics.py
+-rw-r--r--   0        0        0      124 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/validators/__init__.py
+-rw-r--r--   0        0        0      900 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/validators/length.py
+-rw-r--r--   0        0        0      578 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/validators/required.py
+-rw-r--r--   0        0        0      386 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/__init__.py
+-rw-r--r--   0        0        0     5964 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/abc.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/dict_resource/__init__.py
+-rw-r--r--   0        0        0     5733 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/dict_resource/dict_resource.py
+-rw-r--r--   0        0        0     2205 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/dict_resource/filters.py
+-rw-r--r--   0        0        0      692 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/exceptions.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mongo_resource/__init__.py
+-rw-r--r--   0        0        0     2677 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mongo_resource/filters.py
+-rw-r--r--   0        0        0     5829 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mongo_resource/mongo_resource.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mysql_resource/__init__.py
+-rw-r--r--   0        0        0     1931 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mysql_resource/mysql_resource.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/__init__.py
+-rw-r--r--   0        0        0     4678 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/filters.py
+-rw-r--r--   0        0        0     9998 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/postgres_resource.py
+-rw-r--r--   0        0        0      542 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/utils.py
+-rw-r--r--   0        0        0      228 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/resources/types.py
+-rw-r--r--   0        0        0      688 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/__init__.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/__init__.py
+-rw-r--r--   0        0        0     5307 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/admin.py
+-rw-r--r--   0        0        0      916 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/exceptions.py
+-rw-r--r--   0        0        0      745 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/setup.py
+-rw-r--r--   0        0        0     4023 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/css/base.css
+-rw-r--r--   0        0        0   160268 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/css/theme.css
+-rw-r--r--   0        0        0     1217 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/js/main.js
+-rw-r--r--   0        0        0      508 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/cursor_pagination.html
+-rw-r--r--   0        0        0      610 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/boolean_filter.html
+-rw-r--r--   0        0        0      620 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/choice_filter.html
+-rw-r--r--   0        0        0     2989 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/datetime_filter.html
+-rw-r--r--   0        0        0      880 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/search_filter.html
+-rw-r--r--   0        0        0      811 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/single_value_filter.html
+-rw-r--r--   0        0        0      202 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/field_errors.html
+-rw-r--r--   0        0        0      108 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/field_title.html
+-rw-r--r--   0        0        0      686 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/array_field.html
+-rw-r--r--   0        0        0      886 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/autocomplete_field.html
+-rw-r--r--   0        0        0      549 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/boolean_field.html
+-rw-r--r--   0        0        0      896 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/choice_field.html
+-rw-r--r--   0        0        0      522 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/ck_editor_field.html
+-rw-r--r--   0        0        0      298 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/date_field.html
+-rw-r--r--   0        0        0     1143 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/datetime_field.html
+-rw-r--r--   0        0        0      436 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/field.html
+-rw-r--r--   0        0        0      620 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/file_field.html
+-rw-r--r--   0        0        0     2474 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/image_field.html
+-rw-r--r--   0        0        0     1393 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/json_field.html
+-rw-r--r--   0        0        0      601 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/long_string_field.html
+-rw-r--r--   0        0        0      605 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/string_field.html
+-rw-r--r--   0        0        0     1788 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/form.html
+-rw-r--r--   0        0        0      359 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/header.html
+-rw-r--r--   0        0        0      402 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_action_buttons.html
+-rw-r--r--   0        0        0      197 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_cell.html
+-rw-r--r--   0        0        0     1306 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_block.html
+-rw-r--r--   0        0        0     1135 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_header_block.html
+-rw-r--r--   0        0        0      141 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/messages.html
+-rw-r--r--   0        0        0     1094 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/nav_aside.html
+-rw-r--r--   0        0        0     2705 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/pagination.html
+-rw-r--r--   0        0        0      491 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/tabs_bar.html
+-rw-r--r--   0        0        0     1671 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/base.html
+-rw-r--r--   0        0        0      909 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/create_page.html
+-rw-r--r--   0        0        0      207 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/custom_page.html
+-rw-r--r--   0        0        0      173 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/custom_tab_page.html
+-rw-r--r--   0        0        0      937 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/delete_page.html
+-rw-r--r--   0        0        0     1488 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_edit_page.html
+-rw-r--r--   0        0        0      347 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_view_page.html
+-rw-r--r--   0        0        0      587 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_cursor_page.html
+-rw-r--r--   0        0        0     1574 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_page.html
+-rw-r--r--   0        0        0     1085 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/utils.py
+-rw-r--r--   0        0        0        0 2021-10-09 20:30:48.862005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/__init__.py
+-rw-r--r--   0        0        0    14819 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/base.py
+-rw-r--r--   0        0        0     8617 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/controller_view.py
+-rw-r--r--   0        0        0      335 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/dashboard.py
+-rw-r--r--   0        0        0     9391 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/many_to_many_tab_view.py
+-rw-r--r--   0        0        0     1046 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/tab_base_view.py
+-rw-r--r--   0        0        0      865 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/tab_template_view.py
+-rw-r--r--   0        0        0      632 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/template_view.py
+-rw-r--r--   0        0        0     2236 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/utils.py
+-rw-r--r--   0        0        0     4272 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/filters.py
+-rw-r--r--   0        0        0     3810 2021-10-09 20:30:48.866005 aiohttp_admin2-0.0.5/aiohttp_admin2/views/widgets.py
+-rw-r--r--   0        0        0     1076 2021-10-09 20:31:09.054091 aiohttp_admin2-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3605 2021-10-09 20:31:09.922739 aiohttp_admin2-0.0.5/setup.py
+-rw-r--r--   0        0        0     2931 2021-10-09 20:31:09.923204 aiohttp_admin2-0.0.5/PKG-INFO
```

### Comparing `aiohttp_admin2-0.0.4/LICENSE` & `aiohttp_admin2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/connection_injectors.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/connection_injectors.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/controller.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/controller.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/controllers/relations.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/controllers/relations.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/base.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,45 +34,38 @@
         new_attrs = {**new_attrs, "_fields_cls": _fields_cls}
 
         return super().__new__(mcs, name, bases, new_attrs, **kwargs)
 
 
 class Mapper(metaclass=MapperMeta):
 
-    # todo: add itter
-
     _data: t.Dict[str, t.Any] = None
     _fields: t.Dict[str, AbstractField] = None
 
     def __init__(self, data: t.Dict[str, t.Any]) -> None:
-        self.pass_validation = False
+        self._pass_validation = False
         self.with_errors = False
         self.error: t.Optional[str] = None
         self._data = data
         self._fields = self._fields or {}
         self._fields_after_validation = []
         for field in self._fields_cls:
             new_field = field(data.get(field.name))
             new_field.name = field.name
             self._fields[field.name] = new_field
 
     @property
     def raw_data(self):
         """Getter for raw mapper data"""
-        if not self.pass_validation:
-            raise MapperError(
-                "Try to get data from mapper before call the `is_valid` "
-                "method."
-            )
         return self._data
 
     @property
     def data(self) -> t.Dict[str, t.Any]:
         """Return serialize data"""
-        if not self.pass_validation:
+        if not self._pass_validation:
             raise MapperError(
                 "Try to get data from mapper before call the `is_valid` "
                 "method."
             )
         return {
             f.name: f.to_python()
             for f in self._fields_after_validation
@@ -114,14 +107,22 @@
         if it is invalid.
 
         If we set `skip_primary` to `True` then a mapper will not to check the
         primary key field.
         """
         is_valid = True
 
+        if self._pass_validation:
+            # if we'll call is_valid method more than once with wrong data
+            # than errors will duplicate
+            raise MapperError(
+                "`is_valid` method have to call only once per life cycle of "
+                "the mapper object"
+            )
+
         for f in self.fields.values():
 
             if skip_primary and f.primary_key:
                 continue
 
             self._fields_after_validation.append(f)
 
@@ -145,13 +146,13 @@
             if len(e.args):
                 self.error = e.args[0]
             else:
                 if not self.error:
                     self.error = 'Invalid'
 
         self.with_errors = not is_valid
-        self.pass_validation = True
+        self._pass_validation = True
 
         return is_valid
 
     def __repr__(self):
         return f'{self.__class__.__name__}()'
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/__init__.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/abc.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/abc.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     def __init__(
         self,
         *,
         required: bool = False,
         validators: t.List[t.Callable[[t.Any], None]] = None,
         value: t.Optional[str] = None,
-        default: t.Optional[str] = None,
+        default: t.Optional[t.Any] = None,
         primary_key: bool = False,
         **kwargs: t.Any,
     ) -> None:
         self.default: t.Optional[str] = default
         self._value: t.Optional[str] = value
         self.errors: t.List[t.Optional[str]] = []
         self.required = required
@@ -115,8 +115,8 @@
             value=value
         )
 
     def __repr__(self):
         return \
             f"{self.__class__.__name__}(name={self.type_name}," \
             f" value={self._value}), required={self.required}" \
-            f" primary_key={self.primary_key}"
+            f" primary_key={self.primary_key})"
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/choice_field.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/choice_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,26 @@
 
     choices = [
         (1, 'select'),
         (2, 'unselect'),
         (3, 'delete'),
     ]
 
+    >>> from aiohttp_admin2.mappers import fields
+    >>>
+    >>> choices = [(1, 'select'), (2, 'unselect'), ]
+    >>>
+    >>> class Mapper(Mapper):
+    >>>     field = type = fields.ChoicesField(
+    >>>         field_cls=fields.StringField,
+    >>>         choices=choices,
+    >>>     )
+
+    you need to specify `field_cls` which describe type of field. By default
+    it's a `StringField`.
     """
     type_name: str = 'choice'
     empty_value: str = '-- empty --'
     field: AbstractField
 
     def __init__(
         self,
@@ -53,15 +65,14 @@
 
         return value
 
     def to_storage(self) -> str:
         return self.field.to_storage()
 
     def is_valid(self) -> bool:
-        # todo: move to validator
         is_valid = self.field.is_valid()
 
         if not self.required and self.value is None:
             return is_valid
 
         if self.value in [str(value) for value, _ in self.choices]:
             return is_valid
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/float_field.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/float_field.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 from aiohttp_admin2.mappers.fields.abc import AbstractField
 from aiohttp_admin2.mappers.exceptions import ValidationError
 
 __all__ = ["FloatField", ]
 
 
 class FloatField(AbstractField):
+    """
+    Simple representation of float type.
+    """
     type_name: str = 'float'
 
     def to_python(self) -> t.Optional[float]:
         try:
             return (
                 float(self._value) if self._value is not None else self._value
             )
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/int_field.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/int_field.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 from aiohttp_admin2.mappers.exceptions import ValidationError
 from aiohttp_admin2.mappers.fields.abc import AbstractField
 
 __all__ = ["IntField", "SmallIntField", ]
 
 
 class IntField(AbstractField):
+    """
+    Simple representation of float type.
+    """
     type_name: str = 'int'
 
     def to_python(self) -> t.Optional[int]:
         if self._value == '':
             return None
         try:
             return int(self._value) if self._value is not None else self._value
         except ValueError:
             raise ValidationError(
                 f"Incorrect value for Int field. {self._value}"
             )
 
 
 class SmallIntField(IntField):
+    """
+    Simple representation of float type but with additional validation related
+    with long of integer (only for int from MIN_INT to MAX_INT).
+    """
     type_name: str = 'small_int'
     MAX_INT = 32_767
     MIN_INT = -32_768
 
     def to_python(self) -> t.Optional[int]:
         value = super().to_python()
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/fields/json_field.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/fields/json_field.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 __all__ = ["JsonField", ]
 
 
 class JsonField(AbstractField):
     type_name: str = 'json'
 
     def to_python(self) -> t.Optional[t.Dict[str, t.Any]]:
-        if self._value.strip():
+        if self._value and self._value.strip():
             try:
                 return json.loads(self._value)
             except json.decoder.JSONDecodeError:
                 raise ValidationError(
                     "Incorrect format for json field.")
 
         return self._value
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/generics.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/generics.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import sqlalchemy as sa
 import umongo
 
+from marshmallow import EXCLUDE
+from marshmallow.exceptions import ValidationError as MarshmallowValidationErr
 from aiohttp_admin2.mappers.base import Mapper
 from aiohttp_admin2.mappers import fields
 from aiohttp_admin2.mappers.fields import mongo_fields
 from aiohttp_admin2.mappers.exceptions import ValidationError
 
 
 __all__ = [
@@ -14,35 +16,36 @@
 
 
 class PostgresMapperGeneric(Mapper):
     """
     This class need for generate Mapper from sqlAlchemy's model.
     """
 
-    # todo: added types
     FIELDS_MAPPER = {
         sa.Integer: fields.IntField,
+        sa.BigInteger: fields.IntField,
         sa.SmallInteger: fields.SmallIntField,
+        sa.Float: fields.FloatField,
         sa.String: fields.StringField,
         sa.Text: fields.LongStringField,
         sa.Enum: fields.ChoicesField,
         sa.Boolean: fields.BooleanField,
         sa.ARRAY: fields.ArrayField,
         sa.DateTime: fields.DateTimeField,
         sa.Date: fields.DateField,
         sa.JSON: fields.JsonField,
     }
     DEFAULT_FIELD = fields.StringField
 
     def __init_subclass__(cls, table: sa.Table) -> None:
+        super().__init_subclass__()
         cls._fields = {}
 
         existing_fields = [field.name for field in cls._fields_cls]
 
-        # todo: add tests
         for name, column in table.columns.items():
             field_cls = \
                 cls.FIELDS_MAPPER.get(type(column.type), cls.DEFAULT_FIELD)
 
             max_length = hasattr(column.type, 'length') and column.type.length
             field_kwargs = {
                 "max_length": max_length,
@@ -98,23 +101,33 @@
             field.name = name
             if name not in existing_fields:
                 cls._fields_cls.append(field)
                 cls._fields[name] = field
 
     def validation(self):
         """
-        In current method we cover marshmallow validation.
+        In the current method we cover marshmallow validation. We create/update
+        instances via umongo which use marshmallow validation for it. We can't
+        to copy all validation from marshmallow to our mapper because user can
+        to set custom validation. So we just check twice that data is valid for
+        the our mapper and for the marshmallow schema.
         """
         is_valid = True
+        errors = {}
 
-        errors = self.table\
-            .schema\
-            .as_marshmallow_schema()()\
-            .load(self.raw_data)\
-            .errors
+        try:
+            # mapper may have additional fields which are not specify in the
+            # schema so we need to skip validation of fields which are not
+            # exist in the schema
+            self.table.schema.as_marshmallow_schema()().load(
+                self.raw_data,
+                unknown=EXCLUDE,
+            )
+        except MarshmallowValidationErr as e:
+            errors = e.messages
 
         # validation for each field
         for f in self.fields.values():
             if errors.get(f.name):
                 f.errors.append(errors.get(f.name)[0])
                 is_valid = False
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/validators/length.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/validators/length.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/mappers/validators/required.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/mappers/validators/required.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/abc.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/abc.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/dict_resource/dict_resource.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/dict_resource/dict_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,25 @@
 
         if not instance:
             raise InstanceDoesNotExist
 
         return self._row_to_instance(instance)
 
     async def get_many(self, pks: t.List[PK]) -> InstanceMapper:
-        return {
+        relations = {
             pk: self._row_to_instance(self.engine.get(pk))
             for pk in pks
             if pk in self.engine
         }
 
+        return {
+            _id: relations.get(_id, None)
+            for _id in pks
+        }
+
     async def get_list(
         self,
         limit: int = 50,
         page: int = 1,
         cursor: t.Optional[int] = None,
         order_by: t.Optional[str] = None,
         filters: t.Optional[FiltersType] = None,
@@ -144,27 +149,27 @@
             raise InstanceDoesNotExist
 
         del self.engine[pk]
 
     async def create(self, instance: Instance) -> Instance:
         pk = self._get_pk()
         instance.data.id = pk
-        self.engine[pk] = {"id": pk, **instance.data}
+        self.engine[pk] = {"id": pk, **instance.data.__dict__}
 
         return instance
 
     async def update(self, pk: PK, instance: Instance) -> Instance:
         if pk not in self.engine:
             raise InstanceDoesNotExist
 
         self.engine[pk] = instance.data
 
         return self._row_to_instance({
             "id": pk,
-            **instance.data
+            **instance.data.__dict__
         })
 
     def _get_pk(self) -> PK:
         """Return a unique pk for new instance."""
         pk = self._pk
 
         while pk in self.engine:
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/dict_resource/filters.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/dict_resource/filters.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/exceptions.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mongo_resource/filters.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mongo_resource/filters.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mongo_resource/mongo_resource.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mongo_resource/mongo_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,24 @@
         return self._row_to_instance(data)
 
     async def get_many(self, pks: t.List[PK]) -> InstanceMapper:
         data = await self.table\
             .find({"_id": {"$in": [ObjectId(pk) for pk in pks]}})\
             .to_list(length=len(pks))
 
-        return {
+        relations = {
             str(r["id"]): self._row_to_instance(r)
             for r in data
         }
 
+        return {
+            _id: relations.get(_id, None)
+            for _id in pks
+        }
+
     async def get_list(
         self,
         *,
         limit=50,
         page=1,
         cursor=None,
         order_by: t.Optional[str] = None,
@@ -120,23 +125,22 @@
 
     async def create(self, instance: Instance) -> Instance:
         res = await self.table(**instance.data.to_dict()).commit()
 
         return await self.get_one(res.inserted_id)
 
     async def update(self, pk: PK, instance: Instance) -> Instance:
-        if hasattr(instance.data, 'id'):
-            del instance.data.id
+        data = instance.data.to_dict()
+
+        if data.get('id'):
+            del data['id']
 
         await self.table\
             .collection\
-            .update_one(
-                {"_id": ObjectId(pk)},
-                {"$set": instance.data.to_dict()}
-            )
+            .update_one({"_id": ObjectId(pk)}, {"$set": data})
 
         return await self.get_one(pk)
 
     def get_order(self, order_by: str) -> SortType:
         """
         Return received order or default order if order_by was not provide.
         """
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/mysql_resource/mysql_resource.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/mysql_resource/mysql_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+from sqlalchemy.dialects import mysql
+
 from aiohttp_admin2.resources.postgres_resource.postgres_resource import \
     PostgresResource
 from aiohttp_admin2.resources.abc import Instance
 from aiohttp_admin2.resources.types import PK
 
 
 __all__ = ['MySqlResource', ]
 
 
 class MySqlResource(PostgresResource):
 
+    _dialect = mysql.dialect()
+
+    async def _execute(self, conn, query):
+        if not isinstance(query, str):
+            # fixed problem with post compile in aio-mysql
+            query = str(
+                query.compile(
+                    compile_kwargs={"literal_binds": True},
+                    dialect=self._dialect,
+                )
+            )
+
+        return await conn.execute(query)
+
     async def create(self, instance: Instance) -> Instance:
-        data = instance.data
+        data = instance.data.to_dict()
         async with self.engine.acquire() as conn:
             query = self.table\
                 .insert()\
                 .values([data])
 
             result = await conn.execute(query)
 
@@ -26,15 +42,15 @@
             data = await cursor.fetchone()
 
             await conn.execute('commit;')
 
             return self._row_to_instance(data)
 
     async def update(self, pk: PK, instance: Instance) -> Instance:
-        data = instance.data
+        data = instance.data.to_dict()
         async with self.engine.acquire() as conn:
             query = self.table\
                 .update()\
                 .where(self._primary_key == pk)\
                 .values(**data)
 
             await conn.execute(query)
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/filters.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/filters.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/postgres_resource.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/postgres_resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import typing as t
+import logging
 
 import sqlalchemy as sa
 from sqlalchemy import func
-from sqlalchemy.engine.result import RowProxy
+from sqlalchemy.engine.row import RowProxy
 from sqlalchemy.sql.elements import UnaryExpression
 from aiopg.sa import Engine
 
 from aiohttp_admin2.resources.abc import AbstractResource
 from aiohttp_admin2.resources.abc import Instance
 from aiohttp_admin2.resources.abc import InstanceMapper
 from aiohttp_admin2.resources.abc import Paginator
@@ -22,14 +23,15 @@
 from aiohttp_admin2.resources.postgres_resource.filters import default_filter_mapper  # noqa
 
 
 __all__ = ['PostgresResource', 'SortType', ]
 
 
 SortType = t.Union[sa.Column, UnaryExpression]
+logger = logging.getLogger('aiohttp_admin.resource')
 
 
 class PostgresResource(AbstractResource):
     engine: Engine
     table: sa.Table
     limit: int = 50
     name: str
@@ -44,57 +46,73 @@
         custom_sort_list: t.Dict[str, t.Callable] = None,
     ) -> None:
         self.engine = engine
         self.table = table
         self.name = table.name.lower()
         self.custom_sort_list = custom_sort_list or {}
 
+
+    async def _execute(self, conn, query):
+        return await conn.execute(query)
+
+    async def _execute_scalar(self, conn, query):
+        res = await self._execute(conn, query)
+        return await res.scalar()
+
     def get_one_select(self) -> sa.sql.Select:
         """
         In this place you can redefine query.
         """
         return self.table.select()
 
     async def get_one(self, pk: PK) -> Instance:
         async with self.engine.acquire() as conn:
             query = self.get_one_select()\
                 .where(self._primary_key == pk)
 
-            cursor = await conn.execute(query)
+            cursor = await self._execute(conn, query)
 
             res = await cursor.fetchone()
 
             if not res:
                 raise InstanceDoesNotExist
 
             return self._row_to_instance(res)
 
     async def get_many(self, pks: t.List[PK], field: str = None) -> InstanceMapper:
         column = sa.column(field) if field else self._primary_key
         async with self.engine.acquire() as conn:
             query = self.table.select().where(column.in_(pks))
-
-            cursor = await conn.execute(query)
-
-            # todo: validation for return many instance for single id
+            cursor = await self._execute(conn, query)
 
             relations = {}
             relations_list = []
+            multiple_instances_per_key = False
 
             for r in await cursor.fetchall():
                 instance = self._row_to_instance(r, relations_list)
 
                 if field:
                     pk = getattr(instance, field)
                 else:
                     pk = instance.get_pk()
 
                 relations_list.append(instance)
+
+                if relations.get(pk):
+                    multiple_instances_per_key = True
+
                 relations[pk] = instance
 
+            if multiple_instances_per_key:
+                logger.warning(
+                    "`get_many` function return multiple instances for "
+                    "single pk"
+                )
+
             return {_id: relations.get(_id, None) for _id in pks}
 
     def get_list_select(self) -> sa.sql.Select:
         """
         In this place you can redefine query.
         """
         return self.table.select()
@@ -119,41 +137,43 @@
 
         async with self.engine.acquire() as conn:
             query = self.get_list_select()\
                 .limit(limit + 1)
 
             if cursor is not None:
                 if order_by == id_orders[0]:
-                    query = query.where(self._primary_key >= cursor)
+                    query = query.where(self._primary_key > cursor)
                 else:
-                    query = query.where(self._primary_key <= cursor)
+                    query = query.where(self._primary_key < cursor)
             else:
                 query = query.offset(offset)
 
             if filters:
                 query = self.apply_filters(query=query, filters=filters)
 
-            cursor_query = await conn\
-                .execute(query.order_by(self.get_order(order_by)))
+            cursor_query = await self\
+                ._execute(conn, query.order_by(self.get_order(order_by)))
 
             res = []
 
             for r in await cursor_query.fetchall():
                 res.append(self._row_to_instance(r, res))
 
             if cursor is None:
                 if filters:
-                    count: int = await conn.scalar(
+                    count: int = await self._execute_scalar(
+                        conn,
                         self.apply_filters(
                             query=sa.select([func.count(self._primary_key)]),
                             filters=filters,
                         )
                     )
                 else:
-                    count: int = await conn.scalar(
+                    count: int = await self._execute_scalar(
+                        conn,
                         sa.select([func.count(self._primary_key)])
                     )
                 return self.create_paginator(
                     instances=res,
                     limit=limit,
                     offset=offset,
                     count=count,
@@ -167,44 +187,44 @@
 
     async def delete(self, pk: PK) -> None:
         async with self.engine.acquire() as conn:
             query = self.table\
                 .delete()\
                 .where(self._primary_key == pk)
 
-            cursor = await conn.execute(query)
-            await conn.execute('commit;')
+            cursor = await self._execute(conn, query)
+            await self._execute(conn, 'commit;')
 
             if not cursor.rowcount:
                 raise InstanceDoesNotExist
 
     async def create(self, instance: Instance) -> Instance:
         data = instance.data.to_dict()
         async with self.engine.acquire() as conn:
             query = self.table\
                 .insert()\
                 .values([data])\
                 .returning(*self.table.c)
 
-            cursor = await conn.execute(query)
+            cursor = await self._execute(conn, query)
             data = await cursor.fetchone()
 
             return self._row_to_instance(data)
 
     async def update(self, pk: PK, instance: Instance) -> Instance:
         data = instance.data.to_dict()
 
         async with self.engine.acquire() as conn:
             query = self.table\
                 .update()\
                 .where(self._primary_key == pk)\
                 .values(**data)\
                 .returning(*self.table.c)
 
-            cursor = await conn.execute(query)
+            cursor = await self._execute(conn, query)
             data = await cursor.fetchone()
 
             return self._row_to_instance(data)
 
     @property
     def _primary_key(self) -> sa.Column:
         """
```

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/resources/postgres_resource/utils.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/resources/postgres_resource/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/__init__.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/__init__.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/admin.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/admin.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/exceptions.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/setup.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/setup.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/css/base.css` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/css/base.css`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/css/theme.css` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/css/theme.css`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/static/js/main.js` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/boolean_filter.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/boolean_filter.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/choice_filter.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/choice_filter.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/datetime_filter.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/datetime_filter.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/search_filter.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/search_filter.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/single_value_filter.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/filters/single_value_filter.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/array_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/array_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/autocomplete_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/autocomplete_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/boolean_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/boolean_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/choice_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/choice_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/ck_editor_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/ck_editor_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/datetime_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/datetime_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/file_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/file_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/image_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/image_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/json_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/json_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/long_string_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/long_string_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/string_field.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/fields/string_field.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/form.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/form/form.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_block.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_block.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_header_block.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/list_objects_header_block.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/nav_aside.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/nav_aside.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/pagination.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/blocks/pagination.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/base.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/base.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/create_page.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/create_page.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/delete_page.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/delete_page.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_edit_page.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/detail_edit_page.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_cursor_page.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_cursor_page.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_page.html` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/templates/aiohttp_admin/layouts/list_page.html`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/utils.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/base.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/base.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/controller_view.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/controller_view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/many_to_many_tab_view.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/many_to_many_tab_view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/tab_base_view.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/tab_base_view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/tab_template_view.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/tab_template_view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/template_view.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/template_view.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/aiohttp/views/utils.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/aiohttp/views/utils.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/filters.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/filters.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/aiohttp_admin2/views/widgets.py` & `aiohttp_admin2-0.0.5/aiohttp_admin2/views/widgets.py`

 * *Files identical despite different names*

### Comparing `aiohttp_admin2-0.0.4/pyproject.toml` & `aiohttp_admin2-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiohttp_admin2"
-version = "0.0.4"
+version = "0.0.5"
 description = "Generator an admin interface based on aiohttp."
 authors = ["Mykhailo Havelia <misha.gavela@gmail.com>"]
 maintainers = ["Mykhailo Havelia <misha.gavela@gmail.com>"]
 license = "MIT"
 readme = 'README_BUILD.rst'
 homepage = "https://github.com/arfey/aiohttp_admin2"
 repository = "https://github.com/arfey/aiohttp_admin2"
@@ -14,18 +14,18 @@
     { include = "aiohttp_admin2" },
     { include = "aiohttp_admin2/**/*" },
 ]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-aiohttp = "3.6.3"
+aiohttp = "^3.6.3"
 aiohttp-jinja2 = "^1.4.2"
 aiopg = "^1.3.0"
-SQLAlchemy = "1.3.24"
+SQLAlchemy = "^1.4.20"
 sqlalchemy-stubs = "^0.4"
 aiomysql = "^0.0.21"
 motor = "^2.4.0"
 umongo = "^3.0.0"
 python-dateutil = "^2.8.1"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `aiohttp_admin2-0.0.4/setup.py` & `aiohttp_admin2-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,29 +23,29 @@
                                   'templates/aiohttp_admin/blocks/*',
                                   'templates/aiohttp_admin/blocks/filters/*',
                                   'templates/aiohttp_admin/blocks/form/*',
                                   'templates/aiohttp_admin/blocks/form/fields/*',
                                   'templates/aiohttp_admin/layouts/*']}
 
 install_requires = \
-['SQLAlchemy==1.3.24',
+['SQLAlchemy>=1.4.20,<2.0.0',
  'aiohttp-jinja2>=1.4.2,<2.0.0',
- 'aiohttp==3.6.3',
+ 'aiohttp>=3.6.3,<4.0.0',
  'aiomysql>=0.0.21,<0.0.22',
  'aiopg>=1.3.0,<2.0.0',
  'motor>=2.4.0,<3.0.0',
  'python-dateutil>=2.8.1,<3.0.0',
  'sqlalchemy-stubs>=0.4,<0.5',
  'umongo>=3.0.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'aiohttp-admin2',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Generator an admin interface based on aiohttp.',
-    'long_description': '===============\nAiohttp admin 2\n===============\n\n`Demo site\n<https://shrouded-stream-28595.herokuapp.com/>`_ | `Demo source code\n<https://github.com/Arfey/aiohttp_admin2/tree/master/aiohttp_admin2/demo/>`_.\n\nThe aiohttp admin is library for generate admin interface for your data based\non aiohttp. This interface support multiple data storages and can combine them\ntogether.\n\n.. image:: https://img.shields.io/pypi/v/aiohttp_admin2.svg\n        :target: https://pypi.python.org/pypi/aiohttp_admin2\n\n.. image:: https://img.shields.io/travis/arfey/aiohttp_admin2.svg\n        :target: https://travis-ci.com/arfey/aiohttp_admin2\n\n.. image:: https://readthedocs.org/projects/aiohttp-admin2/badge/?version=latest\n        :target: https://aiohttp-admin2.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n\n\n.. image:: https://pyup.io/repos/github/arfey/aiohttp_admin2/shield.svg\n     :target: https://pyup.io/repos/github/arfey/aiohttp_admin2/\n     :alt: Updates\n\n* Free software: MIT license\n* Documentation: https://aiohttp-admin2.readthedocs.io.\n\n=======\nHistory\n=======\n\n0.1.0 (2020-04-28)\n------------------\n\n* First release on PyPI.\n',
+    'long_description': '.. image:: https://img.shields.io/pypi/v/aiohttp_admin2.svg\n        :target: https://pypi.python.org/pypi/aiohttp_admin2\n\n.. image:: https://github.com/Arfey/aiohttp_admin2/actions/workflows/tests.yaml/badge.svg?branch=master\n        :target: https://github.com/Arfey/aiohttp_admin2/actions/workflows/tests.yaml\n\n.. image:: https://readthedocs.org/projects/aiohttp-admin2/badge/?version=latest\n        :target: https://aiohttp-admin2.readthedocs.io/en/latest/?badge=latest\n        :alt: Documentation Status\n\n.. image:: https://pyup.io/repos/github/arfey/aiohttp_admin2/shield.svg\n     :target: https://pyup.io/repos/github/arfey/aiohttp_admin2/\n     :alt: Updates\n\n.. image:: https://img.shields.io/badge/PRs-welcome-green.svg\n     :target: https://github.com/Arfey/aiohttp_admin2/issues\n     :alt: PRs Welcome\n\n=============\nAiohttp admin\n=============\n\n`Demo site\n<https://shrouded-stream-28595.herokuapp.com/>`_ | `Demo source code\n<https://github.com/Arfey/aiohttp_admin2/tree/master/demo/main>`_.\n\nThe aiohttp admin is a library for build admin interface for applications based\non the aiohttp. With this library you can ease to generate CRUD views for your\ndata (for data storages which support by aiohttp admin) and flexibly customize\nrepresentation and access to these.\n\n* Free software: MIT license\n* Documentation: https://aiohttp-admin2.readthedocs.io.\n\nInstallation\n------------\n\nThe first step which you need to do it’s installing library\n\n.. code-block:: bash\n\n   pip install aiohttp_admin2\n\n.. image:: https://github.com/Arfey/aiohttp_admin2/blob/master/docs/images/index.png?raw=true\n\n=======\nHistory\n=======\n\n0.1.0 (2020-04-28)\n------------------\n\n* First release on PyPI.\n',
     'author': 'Mykhailo Havelia',
     'author_email': 'misha.gavela@gmail.com',
     'maintainer': 'Mykhailo Havelia',
     'maintainer_email': 'misha.gavela@gmail.com',
     'url': 'https://github.com/arfey/aiohttp_admin2',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiohttp_admin2-0.0.4/PKG-INFO` & `aiohttp_admin2-0.0.5/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 Metadata-Version: 2.1
 Name: aiohttp-admin2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Generator an admin interface based on aiohttp.
 Home-page: https://github.com/arfey/aiohttp_admin2
 License: MIT
 Keywords: aiohttp_admin2,admin interface,aiohttp
 Author: Mykhailo Havelia
 Author-email: misha.gavela@gmail.com
 Maintainer: Mykhailo Havelia
 Maintainer-email: misha.gavela@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: SQLAlchemy (==1.3.24)
-Requires-Dist: aiohttp (==3.6.3)
+Requires-Dist: SQLAlchemy (>=1.4.20,<2.0.0)
+Requires-Dist: aiohttp (>=3.6.3,<4.0.0)
 Requires-Dist: aiohttp-jinja2 (>=1.4.2,<2.0.0)
 Requires-Dist: aiomysql (>=0.0.21,<0.0.22)
 Requires-Dist: aiopg (>=1.3.0,<2.0.0)
 Requires-Dist: motor (>=2.4.0,<3.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
 Requires-Dist: sqlalchemy-stubs (>=0.4,<0.5)
 Requires-Dist: umongo (>=3.0.0,<4.0.0)
 Project-URL: Documentation, https://aiohttp-admin2.readthedocs.io
 Project-URL: Repository, https://github.com/arfey/aiohttp_admin2
 Description-Content-Type: text/x-rst
 
-===============
-Aiohttp admin 2
-===============
-
-`Demo site
-<https://shrouded-stream-28595.herokuapp.com/>`_ | `Demo source code
-<https://github.com/Arfey/aiohttp_admin2/tree/master/aiohttp_admin2/demo/>`_.
-
-The aiohttp admin is library for generate admin interface for your data based
-on aiohttp. This interface support multiple data storages and can combine them
-together.
-
 .. image:: https://img.shields.io/pypi/v/aiohttp_admin2.svg
         :target: https://pypi.python.org/pypi/aiohttp_admin2
 
-.. image:: https://img.shields.io/travis/arfey/aiohttp_admin2.svg
-        :target: https://travis-ci.com/arfey/aiohttp_admin2
+.. image:: https://github.com/Arfey/aiohttp_admin2/actions/workflows/tests.yaml/badge.svg?branch=master
+        :target: https://github.com/Arfey/aiohttp_admin2/actions/workflows/tests.yaml
 
 .. image:: https://readthedocs.org/projects/aiohttp-admin2/badge/?version=latest
         :target: https://aiohttp-admin2.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
-
 .. image:: https://pyup.io/repos/github/arfey/aiohttp_admin2/shield.svg
      :target: https://pyup.io/repos/github/arfey/aiohttp_admin2/
      :alt: Updates
 
+.. image:: https://img.shields.io/badge/PRs-welcome-green.svg
+     :target: https://github.com/Arfey/aiohttp_admin2/issues
+     :alt: PRs Welcome
+
+=============
+Aiohttp admin
+=============
+
+`Demo site
+<https://shrouded-stream-28595.herokuapp.com/>`_ | `Demo source code
+<https://github.com/Arfey/aiohttp_admin2/tree/master/demo/main>`_.
+
+The aiohttp admin is a library for build admin interface for applications based
+on the aiohttp. With this library you can ease to generate CRUD views for your
+data (for data storages which support by aiohttp admin) and flexibly customize
+representation and access to these.
+
 * Free software: MIT license
 * Documentation: https://aiohttp-admin2.readthedocs.io.
 
+Installation
+------------
+
+The first step which you need to do it’s installing library
+
+.. code-block:: bash
+
+   pip install aiohttp_admin2
+
+.. image:: https://github.com/Arfey/aiohttp_admin2/blob/master/docs/images/index.png?raw=true
+
 =======
 History
 =======
 
 0.1.0 (2020-04-28)
 ------------------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

