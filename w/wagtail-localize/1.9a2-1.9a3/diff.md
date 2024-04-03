# Comparing `tmp/wagtail_localize-1.9a2.tar.gz` & `tmp/wagtail_localize-1.9a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_localize-1.9a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wagtail_localize-1.9a3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wagtail_localize-1.9a2.tar` & `wagtail_localize-1.9a3.tar`

### file list

```diff
@@ -1,356 +1,356 @@
--rw-r--r--   0        0        0    16417 2024-02-25 14:09:53.425002 wagtail_localize-1.9a2/CHANGELOG.md
--rw-r--r--   0        0        0     1539 2022-07-01 10:57:34.575741 wagtail_localize-1.9a2/LICENSE
--rw-r--r--   0        0        0     3834 2024-02-20 16:47:39.204573 wagtail_localize-1.9a2/README.md
--rw-r--r--   0        0        0     2407 2024-02-11 10:57:08.667732 wagtail_localize-1.9a2/pyproject.toml
--rw-r--r--   0        0        0        4 2023-02-15 19:30:49.157059 wagtail_localize-1.9a2/runtime.txt
--rw-r--r--   0        0        0      154 2024-02-25 14:09:30.920347 wagtail_localize-1.9a2/wagtail_localize/__init__.py
--rw-r--r--   0        0        0      367 2022-07-01 10:57:34.552360 wagtail_localize-1.9a2/wagtail_localize/apps.py
--rw-r--r--   0        0        0      260 2023-02-15 19:30:42.626257 wagtail_localize-1.9a2/wagtail_localize/compat.py
--rw-r--r--   0        0        0     6999 2023-10-06 14:18:16.429671 wagtail_localize-1.9a2/wagtail_localize/components.py
--rw-r--r--   0        0        0    11173 2023-10-01 16:27:10.927412 wagtail_localize-1.9a2/wagtail_localize/fields.py
--rw-r--r--   0        0        0      355 2024-02-20 16:53:27.053809 wagtail_localize-1.9a2/wagtail_localize/locale/af/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      452 2024-02-20 16:52:38.778445 wagtail_localize-1.9a2/wagtail_localize/locale/af/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      332 2024-02-20 16:53:27.051349 wagtail_localize-1.9a2/wagtail_localize/locale/af/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      380 2024-02-20 16:52:38.773213 wagtail_localize-1.9a2/wagtail_localize/locale/af/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      866 2024-02-20 16:53:26.966138 wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1107 2024-02-20 16:52:38.711173 wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1260 2024-02-20 16:53:26.964028 wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1400 2024-02-20 16:52:38.705768 wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      504 2024-02-20 16:53:27.002450 wagtail_localize-1.9a2/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      602 2024-02-20 16:52:38.428885 wagtail_localize-1.9a2/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      435 2024-02-20 16:53:27.000774 wagtail_localize-1.9a2/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      490 2024-02-20 16:52:38.423410 wagtail_localize-1.9a2/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    11279 2024-02-20 16:53:27.080746 wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11803 2024-02-20 16:52:38.386170 wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4119 2024-02-20 16:53:27.081397 wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     4085 2024-02-20 16:52:38.379035 wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      423 2024-02-20 16:53:26.909803 wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      568 2024-02-20 16:52:38.757557 wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      825 2024-02-20 16:53:26.914315 wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      901 2024-02-20 16:52:38.752241 wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      604 2024-02-20 16:53:27.104938 wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      722 2024-02-20 16:52:38.768052 wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      723 2024-02-20 16:53:27.102579 wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      796 2024-02-20 16:52:38.762832 wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8759 2024-02-20 16:53:27.097058 wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9272 2024-02-20 16:52:38.506865 wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3131 2024-02-20 16:53:27.093656 wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3064 2024-02-20 16:52:38.500374 wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5670 2024-02-20 16:53:27.015735 wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5993 2024-02-20 16:52:38.518344 wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2628 2024-02-20 16:53:27.016786 wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2552 2024-02-20 16:52:38.512372 wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8553 2024-02-20 16:53:27.030460 wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9096 2024-02-20 16:52:38.924733 wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3066 2024-02-20 16:53:27.028164 wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2974 2024-02-20 16:52:38.918259 wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      519 2024-02-20 16:53:26.960040 wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      642 2024-02-20 16:52:38.396946 wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      797 2024-02-20 16:53:26.957622 wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      952 2024-02-20 16:52:38.391502 wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8909 2024-02-20 16:53:27.076295 wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9655 2024-02-20 16:52:38.821391 wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3181 2024-02-20 16:53:27.077595 wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3208 2024-02-20 16:52:38.815104 wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1651 2024-02-20 16:53:26.990796 wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1677 2024-02-20 16:52:38.667864 wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1402 2024-02-20 16:53:26.988714 wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1356 2024-02-20 16:52:38.661911 wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      741 2024-02-20 16:53:27.060502 wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1021 2024-02-20 16:52:38.472519 wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1460 2024-02-20 16:53:27.059094 wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1590 2024-02-20 16:52:38.467136 wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      210 2024-02-25 14:51:48.916196 wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8715 2024-02-25 14:51:21.984311 wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0       98 2024-02-25 14:51:48.914728 wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     8047 2024-02-25 14:51:21.213354 wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      369 2024-02-20 16:53:26.982381 wagtail_localize-1.9a2/wagtail_localize/locale/en_IN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      435 2024-02-20 16:52:38.607630 wagtail_localize-1.9a2/wagtail_localize/locale/en_IN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      310 2024-02-20 16:53:26.980391 wagtail_localize-1.9a2/wagtail_localize/locale/en_IN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      325 2024-02-20 16:52:38.602340 wagtail_localize-1.9a2/wagtail_localize/locale/en_IN/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8872 2024-02-20 16:53:27.110123 wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9593 2024-02-20 16:52:38.878783 wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3155 2024-02-20 16:53:27.107002 wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3108 2024-02-20 16:52:38.871902 wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      624 2024-02-20 16:53:26.883691 wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      683 2024-02-20 16:52:38.689776 wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      540 2024-02-20 16:53:26.883223 wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      546 2024-02-20 16:52:38.684522 wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      422 2024-02-20 16:53:27.068691 wagtail_localize-1.9a2/wagtail_localize/locale/es_VE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      495 2024-02-20 16:52:38.656551 wagtail_localize-1.9a2/wagtail_localize/locale/es_VE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      398 2024-02-20 16:53:27.066900 wagtail_localize-1.9a2/wagtail_localize/locale/es_VE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      422 2024-02-20 16:52:38.651256 wagtail_localize-1.9a2/wagtail_localize/locale/es_VE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      709 2024-02-20 16:53:26.944537 wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      808 2024-02-20 16:52:38.889581 wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1086 2024-02-20 16:53:26.942259 wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1060 2024-02-20 16:52:38.884335 wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      425 2024-02-20 16:53:26.994818 wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      563 2024-02-20 16:52:38.935183 wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2024-02-20 16:53:26.992897 wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      603 2024-02-20 16:52:38.930024 wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      775 2024-02-20 16:53:27.006341 wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      942 2024-02-20 16:52:38.899917 wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1509 2024-02-20 16:53:27.008581 wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1628 2024-02-20 16:52:38.894760 wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2818 2024-02-20 16:53:26.888412 wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2979 2024-02-20 16:52:38.854484 wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2646 2024-02-20 16:53:26.886727 wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2617 2024-02-20 16:52:38.848995 wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     9199 2024-02-20 16:53:26.956534 wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9760 2024-02-20 16:52:38.866253 wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3318 2024-02-20 16:53:26.954046 wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3213 2024-02-20 16:52:38.859838 wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8623 2024-02-20 16:53:27.115324 wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9177 2024-02-20 16:52:38.723120 wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3105 2024-02-20 16:53:27.114020 wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3024 2024-02-20 16:52:38.716675 wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      730 2024-02-20 16:53:26.879776 wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      959 2024-02-20 16:52:38.585371 wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1008 2024-02-20 16:53:26.878495 wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1092 2024-02-20 16:52:38.580075 wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2024-02-20 16:53:26.895238 wagtail_localize-1.9a2/wagtail_localize/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      432 2024-02-20 16:52:38.799135 wagtail_localize-1.9a2/wagtail_localize/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      302 2024-02-20 16:53:26.890129 wagtail_localize-1.9a2/wagtail_localize/locale/hi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      322 2024-02-20 16:52:38.793941 wagtail_localize-1.9a2/wagtail_localize/locale/hi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1377 2024-02-20 16:53:27.064299 wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1458 2024-02-20 16:52:38.564590 wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1203 2024-02-20 16:53:27.062416 wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1235 2024-02-20 16:52:38.559170 wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      410 2024-02-20 16:53:26.951809 wagtail_localize-1.9a2/wagtail_localize/locale/ht/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      501 2024-02-20 16:52:38.678886 wagtail_localize-1.9a2/wagtail_localize/locale/ht/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2024-02-20 16:53:26.949575 wagtail_localize-1.9a2/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      415 2024-02-20 16:52:38.673076 wagtail_localize-1.9a2/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8938 2024-02-20 16:53:27.116325 wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9494 2024-02-20 16:52:38.735060 wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3220 2024-02-20 16:53:27.111857 wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3113 2024-02-20 16:52:38.728448 wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      592 2024-02-20 16:53:27.037531 wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      827 2024-02-20 16:52:38.439227 wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1150 2024-02-20 16:53:27.033462 wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2024-02-20 16:52:38.434016 wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8679 2024-02-20 16:53:26.932636 wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9181 2024-02-20 16:52:38.843657 wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3082 2024-02-20 16:53:26.930068 wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3018 2024-02-20 16:52:38.837353 wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8402 2024-02-20 16:53:27.049752 wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8946 2024-02-20 16:52:38.494864 wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3171 2024-02-20 16:53:27.047198 wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3255 2024-02-20 16:52:38.488545 wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      787 2024-02-20 16:53:27.041469 wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      957 2024-02-20 16:52:38.461745 wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1259 2024-02-20 16:53:27.039142 wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1448 2024-02-20 16:52:38.456117 wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      499 2024-02-20 16:53:26.923754 wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      581 2024-02-20 16:52:38.809542 wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      767 2024-02-20 16:53:26.922004 wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      788 2024-02-20 16:52:38.804234 wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1337 2024-02-20 16:53:27.011995 wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1481 2024-02-20 16:52:38.831965 wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1248 2024-02-20 16:53:27.013902 wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1289 2024-02-20 16:52:38.826561 wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5593 2024-02-20 16:53:26.898860 wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5952 2024-02-20 16:52:38.912696 wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2690 2024-02-20 16:53:26.904514 wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2643 2024-02-20 16:52:38.906149 wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      670 2024-02-20 16:53:27.021293 wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      792 2024-02-20 16:52:38.483263 wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1162 2024-02-20 16:53:27.019374 wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1189 2024-02-20 16:52:38.477913 wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     1058 2024-02-20 16:53:26.907967 wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1140 2024-02-20 16:52:38.418197 wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      985 2024-02-20 16:53:26.910378 wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      975 2024-02-20 16:52:38.412738 wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      815 2024-02-20 16:53:27.025093 wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      902 2024-02-20 16:52:38.407643 wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1100 2024-02-20 16:53:27.025668 wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1176 2024-02-20 16:52:38.402191 wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      628 2024-02-20 16:53:27.089519 wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      704 2024-02-20 16:52:38.700562 wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      455 2024-02-20 16:53:27.087082 wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      502 2024-02-20 16:52:38.695206 wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      732 2024-02-20 16:53:27.073184 wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      909 2024-02-20 16:52:38.788814 wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1211 2024-02-20 16:53:27.071070 wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1371 2024-02-20 16:52:38.783427 wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8739 2024-02-20 16:53:26.918876 wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9426 2024-02-20 16:52:38.746943 wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3124 2024-02-20 16:53:26.919983 wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3176 2024-02-20 16:52:38.740482 wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     5303 2022-07-01 10:57:34.469976 wagtail_localize-1.9a2/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2838 2022-07-01 10:57:34.470220 wagtail_localize-1.9a2/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     9036 2024-02-20 16:53:27.046118 wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9748 2024-02-20 16:52:38.330700 wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3217 2024-02-20 16:53:27.043483 wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3176 2024-02-20 16:52:38.318112 wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8233 2024-02-20 16:53:26.974591 wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8956 2024-02-20 16:52:38.450903 wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3183 2024-02-20 16:53:26.971994 wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3173 2024-02-20 16:52:38.444612 wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8704 2024-02-20 16:53:26.987130 wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9309 2024-02-20 16:52:38.530037 wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3166 2024-02-20 16:53:26.984573 wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3102 2024-02-20 16:52:38.523567 wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     8710 2024-02-20 16:53:27.084331 wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9179 2024-02-20 16:52:38.597203 wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3152 2024-02-20 16:53:27.088755 wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3011 2024-02-20 16:52:38.590733 wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    11197 2024-02-20 16:53:26.969226 wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11947 2024-02-20 16:52:38.554054 wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4192 2024-02-20 16:53:26.969910 wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     4189 2024-02-20 16:52:38.547045 wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      674 2024-02-20 16:53:27.100492 wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      828 2024-02-20 16:52:38.360064 wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1096 2024-02-20 16:53:27.098108 wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1132 2024-02-20 16:52:38.353891 wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     7327 2024-02-20 16:53:27.057500 wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7776 2024-02-20 16:52:38.305192 wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3078 2024-02-20 16:53:27.055013 wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3004 2024-02-20 16:52:38.272608 wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      434 2024-02-20 16:53:26.962524 wagtail_localize-1.9a2/wagtail_localize/locale/sr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      527 2024-02-20 16:52:38.645786 wagtail_localize-1.9a2/wagtail_localize/locale/sr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8646 2024-02-20 16:53:26.936968 wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9257 2024-02-20 16:52:38.373106 wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3031 2024-02-20 16:53:26.934717 wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     3015 2024-02-20 16:52:38.366227 wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      433 2024-02-20 16:53:26.904943 wagtail_localize-1.9a2/wagtail_localize/locale/ta/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      515 2024-02-20 16:52:38.945506 wagtail_localize-1.9a2/wagtail_localize/locale/ta/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      343 2024-02-20 16:53:26.897352 wagtail_localize-1.9a2/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      374 2024-02-20 16:52:38.940221 wagtail_localize-1.9a2/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      550 2024-02-20 16:53:27.091867 wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      717 2024-02-20 16:52:38.617956 wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      880 2024-02-20 16:53:27.085491 wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1031 2024-02-20 16:52:38.612636 wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      810 2024-02-20 16:53:26.978562 wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      934 2024-02-20 16:52:38.955960 wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1218 2024-02-20 16:53:26.976433 wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1261 2024-02-20 16:52:38.950603 wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      622 2024-02-20 16:53:26.901528 wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      834 2024-02-20 16:52:38.966432 wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1149 2024-02-20 16:53:26.892158 wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1293 2024-02-20 16:52:38.961080 wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      680 2024-02-20 16:53:26.946694 wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      887 2024-02-20 16:52:38.976736 wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1108 2024-02-20 16:53:26.948028 wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1218 2024-02-20 16:52:38.971525 wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     9342 2024-02-20 16:53:27.010350 wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9983 2024-02-20 16:52:38.640299 wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3990 2024-02-20 16:53:27.005238 wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     4175 2024-02-20 16:52:38.633687 wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      686 2024-02-20 16:53:27.031017 wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      857 2024-02-20 16:52:38.347414 wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1424 2024-02-20 16:53:27.035478 wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1450 2024-02-20 16:52:38.339357 wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      495 2024-02-20 16:53:26.927598 wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      691 2024-02-20 16:52:38.628218 wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      736 2024-02-20 16:53:26.925808 wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      907 2024-02-20 16:52:38.623074 wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     7043 2024-02-20 16:53:26.916842 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7589 2024-02-20 16:52:38.541525 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2916 2024-02-20 16:53:26.911839 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     2952 2024-02-20 16:52:38.535358 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      828 2024-02-20 16:53:26.940327 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      919 2024-02-20 16:52:38.575094 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1114 2024-02-20 16:53:26.938060 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1184 2024-02-20 16:52:38.569605 wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922735 wagtail_localize-1.9a2/wagtail_localize/locales/__init__.py
--rw-r--r--   0        0        0      267 2022-07-01 10:57:34.513956 wagtail_localize-1.9a2/wagtail_localize/locales/apps.py
--rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515898 wagtail_localize-1.9a2/wagtail_localize/locales/components.py
--rw-r--r--   0        0        0     1315 2023-02-15 19:30:42.626580 wagtail_localize-1.9a2/wagtail_localize/locales/forms.py
--rw-r--r--   0        0        0      337 2024-02-25 14:51:48.904233 wagtail_localize-1.9a2/wagtail_localize/locales/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2456 2024-02-25 14:51:21.971408 wagtail_localize-1.9a2/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      710 2022-07-01 10:57:34.510343 wagtail_localize-1.9a2/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1979 2022-07-01 10:57:34.509539 wagtail_localize-1.9a2/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1981 2022-07-01 10:57:34.509928 wagtail_localize-1.9a2/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2023 2022-07-01 10:57:34.507986 wagtail_localize-1.9a2/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2053 2022-07-01 10:57:34.509174 wagtail_localize-1.9a2/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2010 2022-07-01 10:57:34.508810 wagtail_localize-1.9a2/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1986 2022-07-01 10:57:34.506765 wagtail_localize-1.9a2/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2453 2022-07-01 10:57:34.507498 wagtail_localize-1.9a2/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2026 2022-07-01 10:57:34.506256 wagtail_localize-1.9a2/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1927 2022-07-01 10:57:34.507136 wagtail_localize-1.9a2/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0      559 2022-07-01 10:57:34.508337 wagtail_localize-1.9a2/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0       92 2024-02-10 10:59:03.987422 wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/_icon.html
--rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515715 wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html
--rw-r--r--   0        0        0      207 2022-07-01 10:57:34.515314 wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/create.html
--rw-r--r--   0        0        0     2765 2023-11-15 20:07:31.817770 wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/edit.html
--rw-r--r--   0        0        0     2150 2024-02-11 10:57:08.668215 wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/index.html
--rw-r--r--   0        0        0    22849 2024-02-10 12:59:11.548528 wagtail_localize-1.9a2/wagtail_localize/locales/tests.py
--rw-r--r--   0        0        0      462 2023-02-15 19:30:42.626782 wagtail_localize-1.9a2/wagtail_localize/locales/utils.py
--rw-r--r--   0        0        0     7140 2024-02-10 10:59:03.988016 wagtail_localize-1.9a2/wagtail_localize/locales/views.py
--rw-r--r--   0        0        0     1052 2023-02-15 19:30:42.626987 wagtail_localize-1.9a2/wagtail_localize/locales/wagtail_hooks.py
--rw-r--r--   0        0        0      385 2022-07-01 10:57:34.538728 wagtail_localize-1.9a2/wagtail_localize/machine_translators/__init__.py
--rw-r--r--   0        0        0      303 2022-09-12 13:15:14.646119 wagtail_localize-1.9a2/wagtail_localize/machine_translators/base.py
--rw-r--r--   0        0        0     1717 2023-11-15 20:20:30.451831 wagtail_localize-1.9a2/wagtail_localize/machine_translators/deepl.py
--rw-r--r--   0        0        0     1678 2024-02-11 10:57:08.668507 wagtail_localize-1.9a2/wagtail_localize/machine_translators/dummy.py
--rw-r--r--   0        0        0     1957 2023-01-22 13:17:54.447370 wagtail_localize-1.9a2/wagtail_localize/machine_translators/google.py
--rw-r--r--   0        0        0     1562 2024-02-10 10:59:03.988239 wagtail_localize-1.9a2/wagtail_localize/machine_translators/libretranslate.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.540801 wagtail_localize-1.9a2/wagtail_localize/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.541279 wagtail_localize-1.9a2/wagtail_localize/management/commands/__init__.py
--rw-r--r--   0        0        0      550 2022-07-01 10:57:34.541517 wagtail_localize-1.9a2/wagtail_localize/management/commands/sync_locale_trees.py
--rw-r--r--   0        0        0    14672 2022-11-04 12:29:12.963230 wagtail_localize-1.9a2/wagtail_localize/migrations/0001_initial.py
--rw-r--r--   0        0        0     2248 2023-10-06 14:18:16.431518 wagtail_localize-1.9a2/wagtail_localize/migrations/0002_translation.py
--rw-r--r--   0        0        0     1027 2023-10-06 14:18:16.432643 wagtail_localize-1.9a2/wagtail_localize/migrations/0003_delete_translation_sources.py
--rw-r--r--   0        0        0      860 2023-10-06 14:18:16.432859 wagtail_localize-1.9a2/wagtail_localize/migrations/0004_one_source_per_objectlocale.py
--rw-r--r--   0        0        0      552 2023-10-06 14:18:16.433222 wagtail_localize-1.9a2/wagtail_localize/migrations/0005_remove_translationsource_object.py
--rw-r--r--   0        0        0     1790 2023-10-06 14:18:16.433514 wagtail_localize-1.9a2/wagtail_localize/migrations/0006_create_submit_translation_permission.py
--rw-r--r--   0        0        0      782 2023-10-06 14:18:16.433897 wagtail_localize-1.9a2/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py
--rw-r--r--   0        0        0      764 2023-10-06 14:18:16.434185 wagtail_localize-1.9a2/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py
--rw-r--r--   0        0        0      591 2023-10-06 14:18:16.434441 wagtail_localize-1.9a2/wagtail_localize/migrations/0009_stringtranslation_errors.py
--rw-r--r--   0        0        0     1399 2023-10-06 14:18:16.435554 wagtail_localize-1.9a2/wagtail_localize/migrations/0010_overridablesegment.py
--rw-r--r--   0        0        0     2226 2023-10-06 14:18:16.435752 wagtail_localize-1.9a2/wagtail_localize/migrations/0011_segmentoverride.py
--rw-r--r--   0        0        0     1329 2023-10-06 14:18:16.435966 wagtail_localize-1.9a2/wagtail_localize/migrations/0012_localesynchronization.py
--rw-r--r--   0        0        0      427 2023-10-06 14:18:16.436143 wagtail_localize-1.9a2/wagtail_localize/migrations/0013_translationsource_schema_version.py
--rw-r--r--   0        0        0      371 2023-10-06 14:18:16.436320 wagtail_localize-1.9a2/wagtail_localize/migrations/0014_remove_translation_source_last_updated_at.py
--rw-r--r--   0        0        0      464 2023-10-06 14:18:16.436494 wagtail_localize-1.9a2/wagtail_localize/migrations/0015_translationcontext_field_path.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.427580 wagtail_localize-1.9a2/wagtail_localize/migrations/__init__.py
--rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922854 wagtail_localize-1.9a2/wagtail_localize/modeladmin/__init__.py
--rw-r--r--   0        0        0      221 2022-07-01 10:57:34.554873 wagtail_localize-1.9a2/wagtail_localize/modeladmin/apps.py
--rw-r--r--   0        0        0     3299 2023-11-07 09:07:15.665670 wagtail_localize-1.9a2/wagtail_localize/modeladmin/helpers.py
--rw-r--r--   0        0        0     2282 2023-11-07 09:07:15.665930 wagtail_localize-1.9a2/wagtail_localize/modeladmin/options.py
--rw-r--r--   0        0        0      421 2024-02-11 10:57:08.668826 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/button.html
--rw-r--r--   0        0        0      162 2022-07-01 10:57:34.556094 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/header_with_breadcrumb.html
--rw-r--r--   0        0        0       46 2022-07-01 10:57:34.557049 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_choose_parent.html
--rw-r--r--   0        0        0      309 2023-02-15 19:30:42.627410 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_create.html
--rw-r--r--   0        0        0       39 2022-07-01 10:57:34.556233 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_delete.html
--rw-r--r--   0        0        0      660 2024-02-11 10:57:08.669096 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html
--rw-r--r--   0        0        0       40 2022-07-01 10:57:34.556386 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_history.html
--rw-r--r--   0        0        0      638 2024-02-11 10:57:08.669491 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html
--rw-r--r--   0        0        0      245 2022-08-31 18:34:50.710573 wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_inspect.html
--rw-r--r--   0        0        0    27666 2024-02-11 10:56:57.587331 wagtail_localize-1.9a2/wagtail_localize/modeladmin/tests.py
--rw-r--r--   0        0        0     7741 2024-02-11 10:57:08.669749 wagtail_localize-1.9a2/wagtail_localize/modeladmin/views.py
--rw-r--r--   0        0        0      616 2023-11-13 20:55:45.204387 wagtail_localize-1.9a2/wagtail_localize/modeladmin/wagtail_hooks.py
--rw-r--r--   0        0        0    86565 2024-02-25 14:05:04.494169 wagtail_localize-1.9a2/wagtail_localize/models.py
--rw-r--r--   0        0        0     4984 2024-02-10 10:59:03.989916 wagtail_localize-1.9a2/wagtail_localize/operations.py
--rw-r--r--   0        0        0      147 2023-10-06 14:18:16.438575 wagtail_localize-1.9a2/wagtail_localize/segments/__init__.py
--rw-r--r--   0        0        0    13186 2023-02-15 19:30:42.628385 wagtail_localize-1.9a2/wagtail_localize/segments/extract.py
--rw-r--r--   0        0        0    12985 2023-10-06 14:18:16.438831 wagtail_localize-1.9a2/wagtail_localize/segments/ingest.py
--rw-r--r--   0        0        0    12328 2023-02-15 19:31:17.389809 wagtail_localize-1.9a2/wagtail_localize/segments/types.py
--rw-r--r--   0        0        0      880 2024-02-25 14:54:34.920595 wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css
--rw-r--r--   0        0        0      906 2024-02-25 14:54:34.920616 wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/css/wagtail-localize-editor-form.css
--rw-r--r--   0        0        0     1501 2024-02-25 14:54:34.920253 wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js
--rw-r--r--   0        0        0    91140 2024-02-25 14:54:34.920271 wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js
--rw-r--r--   0        0        0    14658 2023-02-15 19:31:17.389857 wagtail_localize-1.9a2/wagtail_localize/strings.py
--rw-r--r--   0        0        0     7028 2023-10-06 14:18:16.439067 wagtail_localize-1.9a2/wagtail_localize/synctree.py
--rw-r--r--   0        0        0     1377 2022-07-01 10:57:34.504798 wagtail_localize-1.9a2/wagtail_localize/tasks.py
--rw-r--r--   0        0        0     1267 2023-11-15 20:07:31.818718 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/_components.html
--rw-r--r--   0        0        0     1349 2022-07-01 10:57:34.560800 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html
--rw-r--r--   0        0        0      893 2022-07-01 10:57:34.561400 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html
--rw-r--r--   0        0        0     3814 2024-02-11 10:57:08.672084 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html
--rw-r--r--   0        0        0      742 2022-09-13 08:26:04.349160 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html
--rw-r--r--   0        0        0     2465 2023-11-15 20:07:31.818982 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html
--rw-r--r--   0        0        0     1947 2022-07-01 10:57:34.562358 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/translations_report.html
--rw-r--r--   0        0        0     4228 2023-11-15 20:07:31.819263 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/update_translations.html
--rw-r--r--   0        0        0      501 2022-07-01 10:57:34.563064 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-convert.svg
--rw-r--r--   0        0        0      918 2022-10-12 20:12:40.316546 wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.425464 wagtail_localize-1.9a2/wagtail_localize/templatetags/__init__.py
--rw-r--r--   0        0        0      324 2022-07-01 10:57:34.426417 wagtail_localize-1.9a2/wagtail_localize/templatetags/wagtail_localize_admin_tags.py
--rw-r--r--   0        0        0     1453 2023-10-06 14:18:16.441489 wagtail_localize-1.9a2/wagtail_localize/version.py
--rw-r--r--   0        0        0        0 2022-07-01 10:57:34.565383 wagtail_localize-1.9a2/wagtail_localize/views/__init__.py
--rw-r--r--   0        0        0     6490 2023-10-06 14:18:16.441714 wagtail_localize-1.9a2/wagtail_localize/views/convert.py
--rw-r--r--   0        0        0    54587 2024-02-25 14:05:04.496053 wagtail_localize-1.9a2/wagtail_localize/views/edit_translation.py
--rw-r--r--   0        0        0     4676 2023-10-01 16:27:10.930943 wagtail_localize-1.9a2/wagtail_localize/views/report.py
--rw-r--r--   0        0        0     1350 2023-02-15 19:30:42.632653 wagtail_localize-1.9a2/wagtail_localize/views/snippets_api.py
--rw-r--r--   0        0        0     8968 2023-02-15 19:30:42.632802 wagtail_localize-1.9a2/wagtail_localize/views/submit_translations.py
--rw-r--r--   0        0        0     6591 2024-02-10 10:44:26.184662 wagtail_localize-1.9a2/wagtail_localize/views/update_translations.py
--rw-r--r--   0        0        0    15341 2024-02-11 10:57:08.674343 wagtail_localize-1.9a2/wagtail_localize/wagtail_hooks.py
--rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 wagtail_localize-1.9a2/PKG-INFO
+-rw-r--r--   0        0        0    16417 2024-02-29 19:30:57.184908 wagtail_localize-1.9a3/CHANGELOG.md
+-rw-r--r--   0        0        0     1539 2022-07-01 10:57:34.575741 wagtail_localize-1.9a3/LICENSE
+-rw-r--r--   0        0        0     3834 2024-02-29 19:30:57.185268 wagtail_localize-1.9a3/README.md
+-rw-r--r--   0        0        0     2407 2024-02-29 19:30:57.190589 wagtail_localize-1.9a3/pyproject.toml
+-rw-r--r--   0        0        0        4 2023-02-15 19:30:49.157059 wagtail_localize-1.9a3/runtime.txt
+-rw-r--r--   0        0        0      154 2024-03-02 13:36:52.565155 wagtail_localize-1.9a3/wagtail_localize/__init__.py
+-rw-r--r--   0        0        0      367 2022-07-01 10:57:34.552360 wagtail_localize-1.9a3/wagtail_localize/apps.py
+-rw-r--r--   0        0        0      260 2023-02-15 19:30:42.626257 wagtail_localize-1.9a3/wagtail_localize/compat.py
+-rw-r--r--   0        0        0     6999 2023-10-06 14:18:16.429671 wagtail_localize-1.9a3/wagtail_localize/components.py
+-rw-r--r--   0        0        0    11173 2023-10-01 16:27:10.927412 wagtail_localize-1.9a3/wagtail_localize/fields.py
+-rw-r--r--   0        0        0      355 2024-02-25 14:59:21.587598 wagtail_localize-1.9a3/wagtail_localize/locale/af/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      452 2024-02-29 19:30:57.192715 wagtail_localize-1.9a3/wagtail_localize/locale/af/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      332 2024-02-20 16:53:27.051349 wagtail_localize-1.9a3/wagtail_localize/locale/af/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      380 2024-02-20 16:52:38.773213 wagtail_localize-1.9a3/wagtail_localize/locale/af/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      866 2024-02-25 14:59:21.662510 wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1107 2024-02-29 19:30:57.193116 wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1260 2024-02-20 16:53:26.964028 wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1400 2024-02-20 16:52:38.705768 wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      504 2024-02-25 14:59:21.566377 wagtail_localize-1.9a3/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      602 2024-02-29 19:30:57.193706 wagtail_localize-1.9a3/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      435 2024-02-20 16:53:27.000774 wagtail_localize-1.9a3/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      490 2024-02-20 16:52:38.423410 wagtail_localize-1.9a3/wagtail_localize/locale/az_AZ/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    11279 2024-02-25 14:59:21.665288 wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11803 2024-02-29 19:30:57.195003 wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4119 2024-02-20 16:53:27.081397 wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     4085 2024-02-20 16:52:38.379035 wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      423 2024-02-25 14:59:21.590294 wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      568 2024-02-29 19:30:57.195333 wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      825 2024-02-20 16:53:26.914315 wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      901 2024-02-20 16:52:38.752241 wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      604 2024-02-25 14:59:21.688160 wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      722 2024-02-29 19:30:57.195813 wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      723 2024-02-20 16:53:27.102579 wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      796 2024-02-20 16:52:38.762832 wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8759 2024-02-25 14:59:21.614624 wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9272 2024-02-29 19:30:57.196343 wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3131 2024-02-20 16:53:27.093656 wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3064 2024-02-20 16:52:38.500374 wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5670 2024-02-25 14:59:21.682230 wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5993 2024-02-29 19:30:57.196751 wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2628 2024-02-20 16:53:27.016786 wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2552 2024-02-20 16:52:38.512372 wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8553 2024-02-25 14:59:21.582113 wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9096 2024-02-29 19:30:57.197491 wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3066 2024-02-20 16:53:27.028164 wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2974 2024-02-20 16:52:38.918259 wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      519 2024-02-25 14:59:21.679484 wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      642 2024-02-29 19:30:57.198082 wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      797 2024-02-20 16:53:26.957622 wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      952 2024-02-20 16:52:38.391502 wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8909 2024-02-25 14:59:21.612383 wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9655 2024-02-29 19:30:57.198646 wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3181 2024-02-20 16:53:27.077595 wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3208 2024-02-20 16:52:38.815104 wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1651 2024-02-25 14:59:21.686049 wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1677 2024-02-29 19:30:57.199070 wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1402 2024-02-20 16:53:26.988714 wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1356 2024-02-20 16:52:38.661911 wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      741 2024-02-25 14:59:21.575966 wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1021 2024-02-29 19:30:57.199549 wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1460 2024-02-20 16:53:27.059094 wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1590 2024-02-20 16:52:38.467136 wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      210 2024-02-25 15:00:08.323068 wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8715 2024-02-29 19:30:57.200253 wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0       98 2024-02-25 15:00:08.321150 wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     8047 2024-02-29 19:30:57.201520 wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      369 2024-02-25 14:59:21.584839 wagtail_localize-1.9a3/wagtail_localize/locale/en_IN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      435 2024-02-29 19:30:57.202215 wagtail_localize-1.9a3/wagtail_localize/locale/en_IN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      310 2024-02-20 16:53:26.980391 wagtail_localize-1.9a3/wagtail_localize/locale/en_IN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      325 2024-02-20 16:52:38.602340 wagtail_localize-1.9a3/wagtail_localize/locale/en_IN/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8872 2024-02-25 14:59:21.697910 wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9593 2024-02-29 19:30:57.202678 wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3155 2024-02-20 16:53:27.107002 wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3108 2024-02-20 16:52:38.871902 wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      624 2024-02-25 14:59:21.703276 wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      683 2024-02-29 19:30:57.203101 wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      540 2024-02-20 16:53:26.883223 wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      546 2024-02-20 16:52:38.684522 wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      422 2024-02-25 14:59:21.638337 wagtail_localize-1.9a3/wagtail_localize/locale/es_VE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      495 2024-02-29 19:30:57.203824 wagtail_localize-1.9a3/wagtail_localize/locale/es_VE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      398 2024-02-20 16:53:27.066900 wagtail_localize-1.9a3/wagtail_localize/locale/es_VE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      422 2024-02-20 16:52:38.651256 wagtail_localize-1.9a3/wagtail_localize/locale/es_VE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      709 2024-02-29 19:30:57.204428 wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      808 2024-02-29 19:30:57.204810 wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1086 2024-02-29 19:30:57.205047 wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1060 2024-02-29 19:30:57.205320 wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      425 2024-02-25 14:59:21.705263 wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      563 2024-02-29 19:30:57.205681 wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2024-02-20 16:53:26.992897 wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      603 2024-02-20 16:52:38.930024 wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      775 2024-02-25 14:59:21.692923 wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      942 2024-02-29 19:30:57.206063 wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1509 2024-02-20 16:53:27.008581 wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1628 2024-02-20 16:52:38.894760 wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2818 2024-02-25 14:59:21.569240 wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2979 2024-02-29 19:30:57.206430 wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2646 2024-02-20 16:53:26.886727 wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2617 2024-02-20 16:52:38.848995 wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     9199 2024-02-25 14:59:21.603629 wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9760 2024-02-29 19:30:57.206847 wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3318 2024-02-20 16:53:26.954046 wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3213 2024-02-20 16:52:38.859838 wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8623 2024-02-25 14:59:21.599671 wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9177 2024-02-29 19:30:57.208071 wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3105 2024-02-20 16:53:27.114020 wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3024 2024-02-20 16:52:38.716675 wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      730 2024-02-29 19:30:57.208548 wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      959 2024-02-29 19:30:57.208755 wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1008 2024-02-20 16:53:26.878495 wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1092 2024-02-20 16:52:38.580075 wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2024-02-25 14:59:21.566792 wagtail_localize-1.9a3/wagtail_localize/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      432 2024-02-29 19:30:57.208955 wagtail_localize-1.9a3/wagtail_localize/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      302 2024-02-20 16:53:26.890129 wagtail_localize-1.9a3/wagtail_localize/locale/hi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      322 2024-02-20 16:52:38.793941 wagtail_localize-1.9a3/wagtail_localize/locale/hi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1377 2024-02-25 14:59:21.659884 wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1458 2024-02-29 19:30:57.209251 wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1203 2024-02-20 16:53:27.062416 wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1235 2024-02-20 16:52:38.559170 wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      410 2024-02-25 14:59:21.618368 wagtail_localize-1.9a3/wagtail_localize/locale/ht/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      501 2024-02-29 19:30:57.209559 wagtail_localize-1.9a3/wagtail_localize/locale/ht/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2024-02-20 16:53:26.949575 wagtail_localize-1.9a3/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      415 2024-02-20 16:52:38.673076 wagtail_localize-1.9a3/wagtail_localize/locale/ht/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8938 2024-02-25 14:59:21.616296 wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9494 2024-02-29 19:30:57.210779 wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3220 2024-02-20 16:53:27.111857 wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3113 2024-02-20 16:52:38.728448 wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      592 2024-02-25 14:59:21.645905 wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      827 2024-02-29 19:30:57.211085 wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1150 2024-02-20 16:53:27.033462 wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2024-02-20 16:52:38.434016 wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8679 2024-02-25 14:59:21.567051 wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9181 2024-02-29 19:30:57.211555 wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3082 2024-02-20 16:53:26.930068 wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3018 2024-02-20 16:52:38.837353 wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8402 2024-02-29 19:30:57.212053 wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8946 2024-02-29 19:30:57.212885 wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3171 2024-02-20 16:53:27.047198 wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3255 2024-02-20 16:52:38.488545 wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      787 2024-02-25 14:59:21.644369 wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      957 2024-02-29 19:30:57.213219 wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1259 2024-02-20 16:53:27.039142 wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1448 2024-02-20 16:52:38.456117 wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      499 2024-02-25 14:59:21.701367 wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      581 2024-02-29 19:30:57.213547 wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      767 2024-02-20 16:53:26.922004 wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      788 2024-02-20 16:52:38.804234 wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1337 2024-02-25 14:59:21.625010 wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1481 2024-02-29 19:30:57.213964 wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1248 2024-02-20 16:53:27.013902 wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1289 2024-02-20 16:52:38.826561 wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5593 2024-02-25 14:59:21.649262 wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5952 2024-02-29 19:30:57.214292 wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2690 2024-02-20 16:53:26.904514 wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2643 2024-02-20 16:52:38.906149 wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      670 2024-02-25 14:59:21.631511 wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      792 2024-02-29 19:30:57.215149 wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1162 2024-02-20 16:53:27.019374 wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1189 2024-02-20 16:52:38.477913 wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     1058 2024-02-25 14:59:21.655542 wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1140 2024-02-29 19:30:57.215549 wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      985 2024-02-20 16:53:26.910378 wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      975 2024-02-20 16:52:38.412738 wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      815 2024-02-25 14:59:21.671129 wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      902 2024-02-29 19:30:57.215756 wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1100 2024-02-20 16:53:27.025668 wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1176 2024-02-20 16:52:38.402191 wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      628 2024-02-25 14:59:21.601106 wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      704 2024-02-29 19:30:57.216121 wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      455 2024-02-20 16:53:27.087082 wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      502 2024-02-20 16:52:38.695206 wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      732 2024-02-25 14:59:21.694899 wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      909 2024-02-29 19:30:57.216612 wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1211 2024-02-20 16:53:27.071070 wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1371 2024-02-20 16:52:38.783427 wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8739 2024-02-25 14:59:21.642594 wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9426 2024-02-29 19:30:57.217249 wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3124 2024-02-20 16:53:26.919983 wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3176 2024-02-20 16:52:38.740482 wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     5303 2022-07-01 10:57:34.469976 wagtail_localize-1.9a3/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2838 2022-07-01 10:57:34.470220 wagtail_localize-1.9a3/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     9036 2024-02-25 14:59:21.572234 wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9748 2024-02-29 19:30:57.217633 wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3217 2024-02-20 16:53:27.043483 wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3176 2024-02-20 16:52:38.318112 wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8233 2024-02-25 14:59:21.636423 wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8956 2024-02-29 19:30:57.218614 wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3183 2024-02-20 16:53:26.971994 wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3173 2024-02-20 16:52:38.444612 wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8704 2024-02-25 14:59:21.621123 wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9309 2024-02-29 19:30:57.219235 wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3166 2024-02-20 16:53:26.984573 wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3102 2024-02-20 16:52:38.523567 wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     8710 2024-02-25 14:59:21.634068 wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9179 2024-02-29 19:30:57.219527 wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3152 2024-02-20 16:53:27.088755 wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3011 2024-02-20 16:52:38.590733 wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    11197 2024-02-25 14:59:21.609799 wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11947 2024-02-29 19:30:57.220318 wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4192 2024-02-20 16:53:26.969910 wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     4189 2024-02-20 16:52:38.547045 wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      674 2024-02-25 14:59:21.651177 wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      828 2024-02-29 19:30:57.220528 wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1096 2024-02-20 16:53:27.098108 wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1132 2024-02-20 16:52:38.353891 wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     7327 2024-02-25 14:59:21.684434 wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7776 2024-02-29 19:30:57.220787 wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3078 2024-02-20 16:53:27.055013 wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3004 2024-02-20 16:52:38.272608 wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      434 2024-02-25 14:59:21.629827 wagtail_localize-1.9a3/wagtail_localize/locale/sr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      527 2024-02-29 19:30:57.220999 wagtail_localize-1.9a3/wagtail_localize/locale/sr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8646 2024-02-25 14:59:21.674104 wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9257 2024-02-29 19:30:57.221251 wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3031 2024-02-20 16:53:26.934717 wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     3015 2024-02-20 16:52:38.366227 wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      433 2024-02-25 14:59:21.653215 wagtail_localize-1.9a3/wagtail_localize/locale/ta/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      515 2024-02-29 19:30:57.221439 wagtail_localize-1.9a3/wagtail_localize/locale/ta/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      343 2024-02-20 16:53:26.897352 wagtail_localize-1.9a3/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      374 2024-02-20 16:52:38.940221 wagtail_localize-1.9a3/wagtail_localize/locale/ta/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      550 2024-02-25 14:59:21.668930 wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      717 2024-02-29 19:30:57.221631 wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      880 2024-02-20 16:53:27.085491 wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1031 2024-02-20 16:52:38.612636 wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      810 2024-02-25 14:59:21.592718 wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      934 2024-02-29 19:30:57.221823 wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1218 2024-02-20 16:53:26.976433 wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1261 2024-02-20 16:52:38.950603 wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      622 2024-02-25 14:59:21.675284 wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      834 2024-02-29 19:30:57.223562 wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1149 2024-02-20 16:53:26.892158 wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1293 2024-02-20 16:52:38.961080 wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      680 2024-02-25 14:59:21.690253 wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      887 2024-02-29 19:30:57.223748 wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1108 2024-02-20 16:53:26.948028 wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1218 2024-02-20 16:52:38.971525 wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     9342 2024-02-25 14:59:21.627736 wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9983 2024-02-29 19:30:57.224001 wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3990 2024-02-20 16:53:27.005238 wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     4175 2024-02-20 16:52:38.633687 wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      686 2024-02-25 14:59:21.657888 wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      857 2024-02-29 19:30:57.224186 wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1424 2024-02-20 16:53:27.035478 wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1450 2024-02-20 16:52:38.339357 wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      495 2024-02-25 14:59:21.623060 wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      691 2024-02-29 19:30:57.224364 wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      736 2024-02-20 16:53:26.925808 wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      907 2024-02-20 16:52:38.623074 wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     7043 2024-02-25 14:59:21.677946 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7589 2024-02-29 19:30:57.224563 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2916 2024-02-20 16:53:26.911839 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     2952 2024-02-20 16:52:38.535358 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      828 2024-02-25 14:59:21.667249 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      919 2024-02-29 19:30:57.224743 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1114 2024-02-20 16:53:26.938060 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1184 2024-02-20 16:52:38.569605 wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922735 wagtail_localize-1.9a3/wagtail_localize/locales/__init__.py
+-rw-r--r--   0        0        0      267 2022-07-01 10:57:34.513956 wagtail_localize-1.9a3/wagtail_localize/locales/apps.py
+-rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515898 wagtail_localize-1.9a3/wagtail_localize/locales/components.py
+-rw-r--r--   0        0        0     1315 2023-02-15 19:30:42.626580 wagtail_localize-1.9a3/wagtail_localize/locales/forms.py
+-rw-r--r--   0        0        0      337 2024-02-25 15:00:08.310040 wagtail_localize-1.9a3/wagtail_localize/locales/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2456 2024-02-25 14:59:50.951957 wagtail_localize-1.9a3/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      710 2022-07-01 10:57:34.510343 wagtail_localize-1.9a3/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1979 2022-07-01 10:57:34.509539 wagtail_localize-1.9a3/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1981 2022-07-01 10:57:34.509928 wagtail_localize-1.9a3/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2023 2022-07-01 10:57:34.507986 wagtail_localize-1.9a3/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2053 2022-07-01 10:57:34.509174 wagtail_localize-1.9a3/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2010 2022-07-01 10:57:34.508810 wagtail_localize-1.9a3/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1986 2022-07-01 10:57:34.506765 wagtail_localize-1.9a3/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2453 2022-07-01 10:57:34.507498 wagtail_localize-1.9a3/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2026 2022-07-01 10:57:34.506256 wagtail_localize-1.9a3/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1927 2022-07-01 10:57:34.507136 wagtail_localize-1.9a3/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0      559 2022-07-01 10:57:34.508337 wagtail_localize-1.9a3/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0       92 2024-02-10 10:59:03.987422 wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/_icon.html
+-rw-r--r--   0        0        0      917 2022-07-01 10:57:34.515715 wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html
+-rw-r--r--   0        0        0      207 2022-07-01 10:57:34.515314 wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/create.html
+-rw-r--r--   0        0        0     2765 2023-11-15 20:07:31.817770 wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/edit.html
+-rw-r--r--   0        0        0     2150 2024-02-29 19:30:57.225007 wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/index.html
+-rw-r--r--   0        0        0    22849 2024-02-10 12:59:11.548528 wagtail_localize-1.9a3/wagtail_localize/locales/tests.py
+-rw-r--r--   0        0        0      462 2023-02-15 19:30:42.626782 wagtail_localize-1.9a3/wagtail_localize/locales/utils.py
+-rw-r--r--   0        0        0     7140 2024-02-10 10:59:03.988016 wagtail_localize-1.9a3/wagtail_localize/locales/views.py
+-rw-r--r--   0        0        0     1052 2023-02-15 19:30:42.626987 wagtail_localize-1.9a3/wagtail_localize/locales/wagtail_hooks.py
+-rw-r--r--   0        0        0      385 2022-07-01 10:57:34.538728 wagtail_localize-1.9a3/wagtail_localize/machine_translators/__init__.py
+-rw-r--r--   0        0        0      303 2022-09-12 13:15:14.646119 wagtail_localize-1.9a3/wagtail_localize/machine_translators/base.py
+-rw-r--r--   0        0        0     1717 2023-11-15 20:20:30.451831 wagtail_localize-1.9a3/wagtail_localize/machine_translators/deepl.py
+-rw-r--r--   0        0        0     1678 2024-02-29 19:30:57.225380 wagtail_localize-1.9a3/wagtail_localize/machine_translators/dummy.py
+-rw-r--r--   0        0        0     1957 2023-01-22 13:17:54.447370 wagtail_localize-1.9a3/wagtail_localize/machine_translators/google.py
+-rw-r--r--   0        0        0     1562 2024-02-10 10:59:03.988239 wagtail_localize-1.9a3/wagtail_localize/machine_translators/libretranslate.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.540801 wagtail_localize-1.9a3/wagtail_localize/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.541279 wagtail_localize-1.9a3/wagtail_localize/management/commands/__init__.py
+-rw-r--r--   0        0        0      550 2022-07-01 10:57:34.541517 wagtail_localize-1.9a3/wagtail_localize/management/commands/sync_locale_trees.py
+-rw-r--r--   0        0        0    14672 2022-11-04 12:29:12.963230 wagtail_localize-1.9a3/wagtail_localize/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2248 2023-10-06 14:18:16.431518 wagtail_localize-1.9a3/wagtail_localize/migrations/0002_translation.py
+-rw-r--r--   0        0        0     1027 2023-10-06 14:18:16.432643 wagtail_localize-1.9a3/wagtail_localize/migrations/0003_delete_translation_sources.py
+-rw-r--r--   0        0        0      860 2023-10-06 14:18:16.432859 wagtail_localize-1.9a3/wagtail_localize/migrations/0004_one_source_per_objectlocale.py
+-rw-r--r--   0        0        0      552 2023-10-06 14:18:16.433222 wagtail_localize-1.9a3/wagtail_localize/migrations/0005_remove_translationsource_object.py
+-rw-r--r--   0        0        0     1790 2023-10-06 14:18:16.433514 wagtail_localize-1.9a3/wagtail_localize/migrations/0006_create_submit_translation_permission.py
+-rw-r--r--   0        0        0      782 2023-10-06 14:18:16.433897 wagtail_localize-1.9a3/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py
+-rw-r--r--   0        0        0      764 2023-10-06 14:18:16.434185 wagtail_localize-1.9a3/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py
+-rw-r--r--   0        0        0      591 2023-10-06 14:18:16.434441 wagtail_localize-1.9a3/wagtail_localize/migrations/0009_stringtranslation_errors.py
+-rw-r--r--   0        0        0     1399 2023-10-06 14:18:16.435554 wagtail_localize-1.9a3/wagtail_localize/migrations/0010_overridablesegment.py
+-rw-r--r--   0        0        0     2226 2023-10-06 14:18:16.435752 wagtail_localize-1.9a3/wagtail_localize/migrations/0011_segmentoverride.py
+-rw-r--r--   0        0        0     1329 2023-10-06 14:18:16.435966 wagtail_localize-1.9a3/wagtail_localize/migrations/0012_localesynchronization.py
+-rw-r--r--   0        0        0      427 2023-10-06 14:18:16.436143 wagtail_localize-1.9a3/wagtail_localize/migrations/0013_translationsource_schema_version.py
+-rw-r--r--   0        0        0      371 2023-10-06 14:18:16.436320 wagtail_localize-1.9a3/wagtail_localize/migrations/0014_remove_translation_source_last_updated_at.py
+-rw-r--r--   0        0        0      464 2023-10-06 14:18:16.436494 wagtail_localize-1.9a3/wagtail_localize/migrations/0015_translationcontext_field_path.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.427580 wagtail_localize-1.9a3/wagtail_localize/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-23 10:15:38.922854 wagtail_localize-1.9a3/wagtail_localize/modeladmin/__init__.py
+-rw-r--r--   0        0        0      221 2022-07-01 10:57:34.554873 wagtail_localize-1.9a3/wagtail_localize/modeladmin/apps.py
+-rw-r--r--   0        0        0     3299 2023-11-07 09:07:15.665670 wagtail_localize-1.9a3/wagtail_localize/modeladmin/helpers.py
+-rw-r--r--   0        0        0     2282 2023-11-07 09:07:15.665930 wagtail_localize-1.9a3/wagtail_localize/modeladmin/options.py
+-rw-r--r--   0        0        0      421 2024-02-29 19:30:57.225744 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/button.html
+-rw-r--r--   0        0        0      162 2022-07-01 10:57:34.556094 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/includes/header_with_breadcrumb.html
+-rw-r--r--   0        0        0       46 2022-07-01 10:57:34.557049 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_choose_parent.html
+-rw-r--r--   0        0        0      309 2023-02-15 19:30:42.627410 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_create.html
+-rw-r--r--   0        0        0       39 2022-07-01 10:57:34.556233 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_delete.html
+-rw-r--r--   0        0        0      660 2024-02-29 19:30:57.226192 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html
+-rw-r--r--   0        0        0       40 2022-07-01 10:57:34.556386 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_history.html
+-rw-r--r--   0        0        0      638 2024-02-29 19:30:57.226531 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html
+-rw-r--r--   0        0        0      245 2022-08-31 18:34:50.710573 wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_inspect.html
+-rw-r--r--   0        0        0    27666 2024-02-11 10:56:57.587331 wagtail_localize-1.9a3/wagtail_localize/modeladmin/tests.py
+-rw-r--r--   0        0        0     7741 2024-02-29 19:30:57.226885 wagtail_localize-1.9a3/wagtail_localize/modeladmin/views.py
+-rw-r--r--   0        0        0      616 2023-11-13 20:55:45.204387 wagtail_localize-1.9a3/wagtail_localize/modeladmin/wagtail_hooks.py
+-rw-r--r--   0        0        0    86565 2024-02-25 14:56:17.401641 wagtail_localize-1.9a3/wagtail_localize/models.py
+-rw-r--r--   0        0        0     4984 2024-02-10 10:59:03.989916 wagtail_localize-1.9a3/wagtail_localize/operations.py
+-rw-r--r--   0        0        0      147 2023-10-06 14:18:16.438575 wagtail_localize-1.9a3/wagtail_localize/segments/__init__.py
+-rw-r--r--   0        0        0    13186 2023-02-15 19:30:42.628385 wagtail_localize-1.9a3/wagtail_localize/segments/extract.py
+-rw-r--r--   0        0        0    12985 2023-10-06 14:18:16.438831 wagtail_localize-1.9a3/wagtail_localize/segments/ingest.py
+-rw-r--r--   0        0        0    12328 2023-02-15 19:31:17.389809 wagtail_localize-1.9a3/wagtail_localize/segments/types.py
+-rw-r--r--   0        0        0      880 2024-03-02 13:37:35.535049 wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css
+-rw-r--r--   0        0        0      906 2024-03-02 13:37:35.534859 wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/css/wagtail-localize-editor-form.css
+-rw-r--r--   0        0        0     1501 2024-03-02 13:37:35.534648 wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js
+-rw-r--r--   0        0        0    91125 2024-03-02 13:37:35.534680 wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js
+-rw-r--r--   0        0        0    14658 2023-02-15 19:31:17.389857 wagtail_localize-1.9a3/wagtail_localize/strings.py
+-rw-r--r--   0        0        0     7028 2023-10-06 14:18:16.439067 wagtail_localize-1.9a3/wagtail_localize/synctree.py
+-rw-r--r--   0        0        0     1377 2022-07-01 10:57:34.504798 wagtail_localize-1.9a3/wagtail_localize/tasks.py
+-rw-r--r--   0        0        0     1267 2023-11-15 20:07:31.818718 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/_components.html
+-rw-r--r--   0        0        0     1349 2022-07-01 10:57:34.560800 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html
+-rw-r--r--   0        0        0      893 2022-07-01 10:57:34.561400 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html
+-rw-r--r--   0        0        0     3814 2024-02-29 19:30:57.229339 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html
+-rw-r--r--   0        0        0      742 2022-09-13 08:26:04.349160 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html
+-rw-r--r--   0        0        0     2465 2023-11-15 20:07:31.818982 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html
+-rw-r--r--   0        0        0     1947 2022-07-01 10:57:34.562358 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/translations_report.html
+-rw-r--r--   0        0        0     4228 2023-11-15 20:07:31.819263 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/update_translations.html
+-rw-r--r--   0        0        0      501 2022-07-01 10:57:34.563064 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-convert.svg
+-rw-r--r--   0        0        0      918 2022-10-12 20:12:40.316546 wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.425464 wagtail_localize-1.9a3/wagtail_localize/templatetags/__init__.py
+-rw-r--r--   0        0        0      324 2022-07-01 10:57:34.426417 wagtail_localize-1.9a3/wagtail_localize/templatetags/wagtail_localize_admin_tags.py
+-rw-r--r--   0        0        0     1453 2023-10-06 14:18:16.441489 wagtail_localize-1.9a3/wagtail_localize/version.py
+-rw-r--r--   0        0        0        0 2022-07-01 10:57:34.565383 wagtail_localize-1.9a3/wagtail_localize/views/__init__.py
+-rw-r--r--   0        0        0     6490 2023-10-06 14:18:16.441714 wagtail_localize-1.9a3/wagtail_localize/views/convert.py
+-rw-r--r--   0        0        0    54587 2024-02-29 19:30:57.233254 wagtail_localize-1.9a3/wagtail_localize/views/edit_translation.py
+-rw-r--r--   0        0        0     4676 2023-10-01 16:27:10.930943 wagtail_localize-1.9a3/wagtail_localize/views/report.py
+-rw-r--r--   0        0        0     1350 2023-02-15 19:30:42.632653 wagtail_localize-1.9a3/wagtail_localize/views/snippets_api.py
+-rw-r--r--   0        0        0     8968 2023-02-15 19:30:42.632802 wagtail_localize-1.9a3/wagtail_localize/views/submit_translations.py
+-rw-r--r--   0        0        0     6591 2024-02-10 10:44:26.184662 wagtail_localize-1.9a3/wagtail_localize/views/update_translations.py
+-rw-r--r--   0        0        0    15341 2024-02-29 19:30:57.233703 wagtail_localize-1.9a3/wagtail_localize/wagtail_hooks.py
+-rw-r--r--   0        0        0     6165 1970-01-01 00:00:00.000000 wagtail_localize-1.9a3/PKG-INFO
```

### Comparing `wagtail_localize-1.9a2/CHANGELOG.md` & `wagtail_localize-1.9a3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/LICENSE` & `wagtail_localize-1.9a3/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/README.md` & `wagtail_localize-1.9a3/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/pyproject.toml` & `wagtail_localize-1.9a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/components.py` & `wagtail_localize-1.9a3/wagtail_localize/components.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/fields.py` & `wagtail_localize-1.9a3/wagtail_localize/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/az_AZ/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/be/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/bg/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/bn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ca/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/cs/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/cy/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/da/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/de/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/dv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/es/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/et/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/eu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fa/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/gl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/he_IL/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/hr_HR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/hu/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/id_ID/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/is_IS/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/it/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ja/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ko/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/lt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/mi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/my/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/my/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/nl_NL/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sk_SK/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sr/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/sv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/ta/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/ta/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tet/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/th/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hans/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po` & `wagtail_localize-1.9a3/wagtail_localize/locale/zh_Hant/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/components.py` & `wagtail_localize-1.9a3/wagtail_localize/locales/components.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/forms.py` & `wagtail_localize-1.9a3/wagtail_localize/locales/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/hr_HR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/is_IS/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo` & `wagtail_localize-1.9a3/wagtail_localize/locales/locale/zh_Hant/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html` & `wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/confirm_delete.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/edit.html` & `wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/edit.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/templates/wagtaillocales/index.html` & `wagtail_localize-1.9a3/wagtail_localize/locales/templates/wagtaillocales/index.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/tests.py` & `wagtail_localize-1.9a3/wagtail_localize/locales/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/views.py` & `wagtail_localize-1.9a3/wagtail_localize/locales/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/locales/wagtail_hooks.py` & `wagtail_localize-1.9a3/wagtail_localize/locales/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/machine_translators/deepl.py` & `wagtail_localize-1.9a3/wagtail_localize/machine_translators/deepl.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/machine_translators/dummy.py` & `wagtail_localize-1.9a3/wagtail_localize/machine_translators/dummy.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/machine_translators/google.py` & `wagtail_localize-1.9a3/wagtail_localize/machine_translators/google.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/machine_translators/libretranslate.py` & `wagtail_localize-1.9a3/wagtail_localize/machine_translators/libretranslate.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/management/commands/sync_locale_trees.py` & `wagtail_localize-1.9a3/wagtail_localize/management/commands/sync_locale_trees.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0001_initial.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0002_translation.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0002_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0003_delete_translation_sources.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0003_delete_translation_sources.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0004_one_source_per_objectlocale.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0004_one_source_per_objectlocale.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0005_remove_translationsource_object.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0005_remove_translationsource_object.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0006_create_submit_translation_permission.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0006_create_submit_translation_permission.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0007_stringtranslation_type_and_tool_name.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0008_stringtranslation_last_translated_by.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0009_stringtranslation_errors.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0009_stringtranslation_errors.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0010_overridablesegment.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0010_overridablesegment.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0011_segmentoverride.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0011_segmentoverride.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/migrations/0012_localesynchronization.py` & `wagtail_localize-1.9a3/wagtail_localize/migrations/0012_localesynchronization.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/helpers.py` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/helpers.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/options.py` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/options.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_edit.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/templates/wagtail_localize/modeladmin/translatable_index.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/tests.py` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/tests.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/views.py` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/modeladmin/wagtail_hooks.py` & `wagtail_localize-1.9a3/wagtail_localize/modeladmin/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/models.py` & `wagtail_localize-1.9a3/wagtail_localize/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/operations.py` & `wagtail_localize-1.9a3/wagtail_localize/operations.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/segments/extract.py` & `wagtail_localize-1.9a3/wagtail_localize/segments/extract.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/segments/ingest.py` & `wagtail_localize-1.9a3/wagtail_localize/segments/ingest.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/segments/types.py` & `wagtail_localize-1.9a3/wagtail_localize/segments/types.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css` & `wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/css/wagtail-localize-component-form.css`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/css/wagtail-localize-editor-form.css` & `wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/css/wagtail-localize-editor-form.css`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js` & `wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/js/wagtail-localize-component-form.js`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js` & `wagtail_localize-1.9a3/wagtail_localize/static/wagtail_localize/js/wagtail-localize.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2163,16 +2163,16 @@
             value: t
         }), a.default.createElement("input", {
             type: "hidden",
             name: "next",
             value: window.location.href
         }), a.default.createElement("button", {
             type: "submit",
-            name: "action-publish",
-            value: "action-publish",
+            name: "action",
+            value: "publish",
             className: "button button-longrunning",
             "data-clicked-text": o.default("Publishing..."),
             "data-controller": "w-progress",
             "data-action": "w-progress#activate",
             "data-w-progress-active-value": o.default("Publishing...")
         }, a.default.createElement(l.default, {
             name: "upload",
```

### Comparing `wagtail_localize-1.9a2/wagtail_localize/strings.py` & `wagtail_localize-1.9a3/wagtail_localize/strings.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/synctree.py` & `wagtail_localize-1.9a3/wagtail_localize/synctree.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/tasks.py` & `wagtail_localize-1.9a3/wagtail_localize/tasks.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/_components.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/_components.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/confirm_convert_to_alias.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/edit_translatable_alias.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/edit_translation.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/includes/generic_header.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/submit_translation.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/translations_report.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/translations_report.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/admin/update_translations.html` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/admin/update_translations.html`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg` & `wagtail_localize-1.9a3/wagtail_localize/templates/wagtail_localize/icons/wagtail-localize-language.svg`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/version.py` & `wagtail_localize-1.9a3/wagtail_localize/version.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/convert.py` & `wagtail_localize-1.9a3/wagtail_localize/views/convert.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/edit_translation.py` & `wagtail_localize-1.9a3/wagtail_localize/views/edit_translation.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/report.py` & `wagtail_localize-1.9a3/wagtail_localize/views/report.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/snippets_api.py` & `wagtail_localize-1.9a3/wagtail_localize/views/snippets_api.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/submit_translations.py` & `wagtail_localize-1.9a3/wagtail_localize/views/submit_translations.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/views/update_translations.py` & `wagtail_localize-1.9a3/wagtail_localize/views/update_translations.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/wagtail_localize/wagtail_hooks.py` & `wagtail_localize-1.9a3/wagtail_localize/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_localize-1.9a2/PKG-INFO` & `wagtail_localize-1.9a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-localize
-Version: 1.9a2
+Version: 1.9a3
 Summary: Translation plugin for Wagtail CMS
 Author-email: Karl Hobley <karl@torchbox.com>
 Maintainer-email: Dan Braghis <dan.braghis@torchbox.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

