# Comparing `tmp/django-508-plugins-3.0.0.tar.gz` & `tmp/django-508-plugins-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-508-plugins-3.0.0.tar", last modified: Wed Mar 20 20:23:28 2024, max compression
+gzip compressed data, was "django-508-plugins-3.0.1.tar", last modified: Wed Apr  3 14:30:41 2024, max compression
```

## Comparing `django-508-plugins-3.0.0.tar` & `django-508-plugins-3.0.1.tar`

### file list

```diff
@@ -1,102 +1,104 @@
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:28.067871 django-508-plugins-3.0.0/
--rw-r--r--   0 ruttenb   (1328) ims        (100)      136 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/MANIFEST.in
--rw-r--r--   0 ruttenb   (1328) ims        (100)      550 2024-03-20 20:23:28.067851 django-508-plugins-3.0.0/PKG-INFO
--rw-r--r--   0 ruttenb   (1328) ims        (100)     2854 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/README.md
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.888873 django-508-plugins-3.0.0/django_508_plugins.egg-info/
--rw-rw----   0 ruttenb   (1328) ims        (100)      550 2024-03-20 20:23:25.000000 django-508-plugins-3.0.0/django_508_plugins.egg-info/PKG-INFO
--rw-rw----   0 ruttenb   (1328) ims        (100)     4136 2024-03-20 20:23:26.000000 django-508-plugins-3.0.0/django_508_plugins.egg-info/SOURCES.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        1 2024-03-20 20:23:25.000000 django-508-plugins-3.0.0/django_508_plugins.egg-info/dependency_links.txt
--rw-rw----   0 ruttenb   (1328) ims        (100)        8 2024-03-20 20:23:25.000000 django-508-plugins-3.0.0/django_508_plugins.egg-info/top_level.txt
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.891891 django-508-plugins-3.0.0/plugins/
--rw-r--r--   0 ruttenb   (1328) ims        (100)       88 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/plugins/__init__.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.895861 django-508-plugins-3.0.0/plugins/datepicker/
--rw-rw----   0 ruttenb   (1328) ims        (100)       65 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/datepicker/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      259 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/datepicker/apps.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.869856 django-508-plugins-3.0.0/plugins/datepicker/static/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.897855 django-508-plugins-3.0.0/plugins/datepicker/static/datepicker/
--rw-r--r--   0 ruttenb   (1328) ims        (100)    25244 2022-07-01 19:40:52.000000 django-508-plugins-3.0.0/plugins/datepicker/static/datepicker/jqueryui_datepicker_508.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.909855 django-508-plugins-3.0.0/plugins/datepicker/static/images/
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7090 2022-07-01 19:40:52.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_444444_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7074 2022-07-01 19:40:52.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_555555_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2022-07-01 19:40:52.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_777620_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7111 2022-07-01 19:40:53.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_777777_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2022-07-01 19:40:53.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     6487 2022-07-01 19:40:53.000000 django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_ffffff_256x240.png
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.913853 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.927855 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7090 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_444444_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7074 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_555555_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_777620_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     7111 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_777777_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)     6487 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 ruttenb   (1328) ims        (100)    30801 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/jquery-ui.min.css
--rw-r--r--   0 ruttenb   (1328) ims        (100)   255079 2023-02-22 15:33:48.000000 django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/jquery-ui.min.js
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.930871 django-508-plugins-3.0.0/plugins/select2/
--rw-rw----   0 ruttenb   (1328) ims        (100)       59 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/__init__.py
--rw-rw----   0 ruttenb   (1328) ims        (100)      240 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/apps.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.872856 django-508-plugins-3.0.0/plugins/select2/static/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:28.056851 django-508-plugins-3.0.0/plugins/select2/static/select2/
--rw-rw----   0 ruttenb   (1328) ims        (100)     3347 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2-bootstrap.css
--rw-rw----   0 ruttenb   (1328) ims        (100)     1849 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2-spinner.gif
--rw-rw----   0 ruttenb   (1328) ims        (100)    19210 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2.css
--rw-rw----   0 ruttenb   (1328) ims        (100)   159709 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      613 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2.png
--rw-rw----   0 ruttenb   (1328) ims        (100)     1389 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ar.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1003 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_az.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1081 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_bg.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      952 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ca.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1988 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_cs.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      853 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_da.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1014 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_de.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1128 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_el.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1102 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_en.js.template
--rw-rw----   0 ruttenb   (1328) ims        (100)     1177 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_es.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      886 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_et.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1313 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_eu.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1207 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fa.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      940 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fi.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1077 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fr.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1339 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_gl.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      885 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_he.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1002 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_hr.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      802 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_hu.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1111 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_id.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      855 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_is.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      866 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_it.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      812 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ja.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1078 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ka.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      871 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ko.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1144 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_lt.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      999 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_lv.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1064 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_mk.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1122 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ms.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1145 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_nb.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      846 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_nl.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     2015 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pl.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      969 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pt-BR.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      891 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pt-PT.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      902 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ro.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1058 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_rs.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1171 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ru.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1948 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_sk.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      847 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_sv.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1063 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_th.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1070 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_tr.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      904 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ug-CN.js
--rw-rw----   0 ruttenb   (1328) ims        (100)     1415 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_uk.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      910 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_vi.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      762 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_zh-CN.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      774 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_zh-TW.js
--rw-rw----   0 ruttenb   (1328) ims        (100)      845 2019-07-23 20:26:00.000000 django-508-plugins-3.0.0/plugins/select2/static/select2/select2x2.png
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:28.059854 django-508-plugins-3.0.0/plugins/selectcn/
--rw-r--r--   0 ruttenb   (1328) ims        (100)       60 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/plugins/selectcn/__init__.py
--rw-r--r--   0 ruttenb   (1328) ims        (100)      255 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/plugins/selectcn/apps.py
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.874856 django-508-plugins-3.0.0/plugins/selectcn/static/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:27.875863 django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:28.061858 django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/css/
--rw-r--r--   0 ruttenb   (1328) ims        (100)    19160 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/css/selectcn.css
-drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-03-20 20:23:28.064851 django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/js/
--rw-r--r--   0 ruttenb   (1328) ims        (100)   159097 2024-03-20 20:22:55.000000 django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/js/selectcn.js
--rw-r--r--   0 ruttenb   (1328) ims        (100)       38 2024-03-20 20:23:28.068884 django-508-plugins-3.0.0/setup.cfg
--rw-rw----   0 ruttenb   (1328) ims        (100)      722 2019-07-23 20:26:01.000000 django-508-plugins-3.0.0/setup.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.743028 django-508-plugins-3.0.1/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      136 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/MANIFEST.in
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      550 2024-04-03 14:30:41.742995 django-508-plugins-3.0.1/PKG-INFO
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     2854 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/README.md
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.553035 django-508-plugins-3.0.1/django_508_plugins.egg-info/
+-rw-rw----   0 ruttenb   (1328) ims        (100)      550 2024-04-03 14:30:37.000000 django-508-plugins-3.0.1/django_508_plugins.egg-info/PKG-INFO
+-rw-rw----   0 ruttenb   (1328) ims        (100)     4235 2024-04-03 14:30:37.000000 django-508-plugins-3.0.1/django_508_plugins.egg-info/SOURCES.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        1 2024-04-03 14:30:37.000000 django-508-plugins-3.0.1/django_508_plugins.egg-info/dependency_links.txt
+-rw-rw----   0 ruttenb   (1328) ims        (100)        8 2024-04-03 14:30:37.000000 django-508-plugins-3.0.1/django_508_plugins.egg-info/top_level.txt
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.555042 django-508-plugins-3.0.1/plugins/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)       88 2024-04-03 14:29:59.000000 django-508-plugins-3.0.1/plugins/__init__.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.560019 django-508-plugins-3.0.1/plugins/datepicker/
+-rw-rw----   0 ruttenb   (1328) ims        (100)       65 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/datepicker/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      259 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/datepicker/apps.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.527995 django-508-plugins-3.0.1/plugins/datepicker/static/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.562056 django-508-plugins-3.0.1/plugins/datepicker/static/datepicker/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    25244 2022-07-01 19:40:52.000000 django-508-plugins-3.0.1/plugins/datepicker/static/datepicker/jqueryui_datepicker_508.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.578071 django-508-plugins-3.0.1/plugins/datepicker/static/images/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7090 2022-07-01 19:40:52.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7074 2022-07-01 19:40:52.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2022-07-01 19:40:52.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7111 2022-07-01 19:40:53.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2022-07-01 19:40:53.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     6487 2022-07-01 19:40:53.000000 django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_ffffff_256x240.png
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.590001 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.603036 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7090 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7074 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     7111 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     4618 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)     6487 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    37452 2024-04-03 14:29:59.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   529159 2024-04-03 14:29:59.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    30801 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.min.css
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   255079 2023-02-22 15:33:48.000000 django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.min.js
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.607036 django-508-plugins-3.0.1/plugins/select2/
+-rw-rw----   0 ruttenb   (1328) ims        (100)       59 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/__init__.py
+-rw-rw----   0 ruttenb   (1328) ims        (100)      240 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/apps.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.531050 django-508-plugins-3.0.1/plugins/select2/static/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.730998 django-508-plugins-3.0.1/plugins/select2/static/select2/
+-rw-rw----   0 ruttenb   (1328) ims        (100)     3347 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2-bootstrap.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1849 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2-spinner.gif
+-rw-rw----   0 ruttenb   (1328) ims        (100)    19210 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2.css
+-rw-rw----   0 ruttenb   (1328) ims        (100)   159709 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      613 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2.png
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1389 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ar.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1003 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_az.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1081 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_bg.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      952 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ca.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1988 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_cs.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      853 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_da.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1014 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_de.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1128 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_el.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1102 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_en.js.template
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1177 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_es.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      886 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_et.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1313 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_eu.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1207 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fa.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      940 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fi.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1077 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fr.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1339 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_gl.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      885 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_he.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1002 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_hr.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      802 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_hu.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1111 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_id.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      855 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_is.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      866 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_it.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      812 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ja.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1078 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ka.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      871 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ko.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1144 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_lt.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      999 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_lv.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1064 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_mk.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1122 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ms.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1145 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_nb.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      846 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_nl.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     2015 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pl.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      969 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pt-BR.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      891 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pt-PT.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      902 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ro.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1058 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_rs.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1171 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ru.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1948 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_sk.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      847 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_sv.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1063 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_th.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1070 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_tr.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      904 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ug-CN.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)     1415 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_uk.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      910 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_vi.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      762 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_zh-CN.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      774 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_zh-TW.js
+-rw-rw----   0 ruttenb   (1328) ims        (100)      845 2019-07-23 20:26:00.000000 django-508-plugins-3.0.1/plugins/select2/static/select2/select2x2.png
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.734987 django-508-plugins-3.0.1/plugins/selectcn/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)       60 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/plugins/selectcn/__init__.py
+-rw-r--r--   0 ruttenb   (1328) ims        (100)      255 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/plugins/selectcn/apps.py
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.534018 django-508-plugins-3.0.1/plugins/selectcn/static/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.535031 django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.737017 django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/css/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)    19160 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/css/selectcn.css
+drwxr-sr-x   0 ruttenb   (1328) ims        (100)        0 2024-04-03 14:30:41.739023 django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/js/
+-rw-r--r--   0 ruttenb   (1328) ims        (100)   159097 2024-03-20 20:22:55.000000 django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/js/selectcn.js
+-rw-r--r--   0 ruttenb   (1328) ims        (100)       38 2024-04-03 14:30:41.744010 django-508-plugins-3.0.1/setup.cfg
+-rw-rw----   0 ruttenb   (1328) ims        (100)      722 2019-07-23 20:26:01.000000 django-508-plugins-3.0.1/setup.py
```

### Comparing `django-508-plugins-3.0.0/PKG-INFO` & `django-508-plugins-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-508-plugins
-Version: 3.0.0
+Version: 3.0.1
 Summary: Installable Django app containing 508-compliant plugins.
 Home-page: https://github.com/imsweb/django-508-plugins
 Author: Brad Rutten
 Author-email: ruttenb@imsweb.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-508-plugins-3.0.0/README.md` & `django-508-plugins-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/django_508_plugins.egg-info/PKG-INFO` & `django-508-plugins-3.0.1/django_508_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-508-plugins
-Version: 3.0.0
+Version: 3.0.1
 Summary: Installable Django app containing 508-compliant plugins.
 Home-page: https://github.com/imsweb/django-508-plugins
 Author: Brad Rutten
 Author-email: ruttenb@imsweb.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-508-plugins-3.0.0/django_508_plugins.egg-info/SOURCES.txt` & `django-508-plugins-3.0.1/django_508_plugins.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 plugins/datepicker/static/datepicker/jqueryui_datepicker_508.js
 plugins/datepicker/static/images/ui-icons_444444_256x240.png
 plugins/datepicker/static/images/ui-icons_555555_256x240.png
 plugins/datepicker/static/images/ui-icons_777620_256x240.png
 plugins/datepicker/static/images/ui-icons_777777_256x240.png
 plugins/datepicker/static/images/ui-icons_cc0000_256x240.png
 plugins/datepicker/static/images/ui-icons_ffffff_256x240.png
+plugins/datepicker/static/jquery-ui/jquery-ui.css
+plugins/datepicker/static/jquery-ui/jquery-ui.js
 plugins/datepicker/static/jquery-ui/jquery-ui.min.css
 plugins/datepicker/static/jquery-ui/jquery-ui.min.js
 plugins/datepicker/static/jquery-ui/images/ui-icons_444444_256x240.png
 plugins/datepicker/static/jquery-ui/images/ui-icons_555555_256x240.png
 plugins/datepicker/static/jquery-ui/images/ui-icons_777620_256x240.png
 plugins/datepicker/static/jquery-ui/images/ui-icons_777777_256x240.png
 plugins/datepicker/static/jquery-ui/images/ui-icons_cc0000_256x240.png
```

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/datepicker/jqueryui_datepicker_508.js` & `django-508-plugins-3.0.1/plugins/datepicker/static/datepicker/jqueryui_datepicker_508.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_444444_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_555555_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_777620_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_777777_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_cc0000_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/images/ui-icons_ffffff_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_444444_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_555555_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_777620_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_777777_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_cc0000_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/images/ui-icons_ffffff_256x240.png` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/jquery-ui.min.css` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/datepicker/static/jquery-ui/jquery-ui.min.js` & `django-508-plugins-3.0.1/plugins/datepicker/static/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2-bootstrap.css` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2-bootstrap.css`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2-spinner.gif` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2.css` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2.css`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2.png` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ar.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ar.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_az.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_az.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_bg.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_bg.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ca.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ca.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_cs.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_cs.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_da.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_da.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_de.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_de.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_el.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_el.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_en.js.template` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_en.js.template`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_es.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_es.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_et.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_et.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_eu.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_eu.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fa.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fa.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fi.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fi.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_fr.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_fr.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_gl.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_gl.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_he.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_he.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_hr.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_hr.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_hu.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_hu.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_id.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_id.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_is.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_is.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_it.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_it.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ja.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ja.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ka.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ka.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ko.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ko.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_lt.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_lt.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_lv.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_lv.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_mk.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_mk.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ms.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ms.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_nb.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_nb.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_nl.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_nl.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pl.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pl.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pt-BR.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_pt-PT.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ro.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ro.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_rs.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_rs.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ru.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ru.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_sk.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_sk.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_sv.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_sv.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_th.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_th.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_tr.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_tr.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_ug-CN.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_ug-CN.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_uk.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_uk.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_vi.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_vi.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_zh-CN.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2_locale_zh-TW.js` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2_locale_zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/select2/static/select2/select2x2.png` & `django-508-plugins-3.0.1/plugins/select2/static/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/css/selectcn.css` & `django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/css/selectcn.css`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/plugins/selectcn/static/selectcn/js/selectcn.js` & `django-508-plugins-3.0.1/plugins/selectcn/static/selectcn/js/selectcn.js`

 * *Files identical despite different names*

### Comparing `django-508-plugins-3.0.0/setup.py` & `django-508-plugins-3.0.1/setup.py`

 * *Files identical despite different names*

