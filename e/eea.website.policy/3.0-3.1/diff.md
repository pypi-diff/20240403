# Comparing `tmp/eea.website.policy-3.0.zip` & `tmp/eea.website.policy-3.1.zip`

## zipinfo {}

```diff
@@ -1,257 +1,257 @@
-Zip file size: 97227 bytes, number of entries: 255
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/
--rw-r--r--  2.0 unx       38 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/setup.cfg
--rw-r--r--  2.0 unx     2288 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/CONTRIBUTING.md
--rw-r--r--  2.0 unx     4965 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/PKG-INFO
--rw-r--r--  2.0 unx     3027 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/README.rst
--rw-r--r--  2.0 unx     1989 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/setup.py
--rw-r--r--  2.0 unx      126 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/MANIFEST.in
--rw-r--r--  2.0 unx     1038 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/docs/HISTORY.txt
--rw-r--r--  2.0 unx      917 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/docs/LICENSE.GPL
--rw-r--r--  2.0 unx       53 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     4965 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/not-zip-safe
--rw-r--r--  2.0 unx      238 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/top_level.txt
--rw-r--r--  2.0 unx     8165 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea.website.policy.egg-info/SOURCES.txt
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/behaviors/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/
--rw-r--r--  2.0 unx        4 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/version.txt
--rw-r--r--  2.0 unx      502 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/configure.zcml
--rw-r--r--  2.0 unx      714 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/setuphandlers.py
--rw-r--r--  2.0 unx      242 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/interfaces.py
--rw-r--r--  2.0 unx      352 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/README.txt
--rw-r--r--  2.0 unx     1339 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles.zcml
--rw-r--r--  2.0 unx      221 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx      767 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/upgrades/configure.zcml
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/upgrades/__init__.py
--rw-r--r--  2.0 unx     2018 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/tests/base.py
--rw-r--r--  2.0 unx      676 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/tests/__init__.py
--rw-r--r--  2.0 unx      234 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/behaviors/configure.zcml
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/behaviors/__init__.py
--rw-r--r--  2.0 unx      419 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/browser/configure.zcml
--rw-r--r--  2.0 unx      480 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/browser/view.pt
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/browser/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/languages/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/
--rw-r--r--  2.0 unx       87 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/languages/metadata.xml
--rw-r--r--  2.0 unx      572 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/languages/registry.xml
--rw-r--r--  2.0 unx      128 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/
--rw-r--r--  2.0 unx      368 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types.xml
--rw-r--r--  2.0 unx      719 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/metadata.xml
--rw-r--r--  2.0 unx    11397 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/actions.xml
--rw-r--r--  2.0 unx      553 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/repositorytool.xml
--rw-r--r--  2.0 unx      179 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx   139757 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/topic_page.xml
--rw-r--r--  2.0 unx    13612 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/landing_page.xml
--rw-r--r--  2.0 unx      323 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/LRF.xml
--rw-r--r--  2.0 unx     7717 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/faq.xml
--rw-r--r--  2.0 unx     7085 b- defN 23-Jun-01 13:04 eea.website.policy-3.0/eea/website/policy/profiles/default/types/article.xml
-255 files, 238588 bytes uncompressed, 44819 bytes compressed:  81.2%
+Zip file size: 97267 bytes, number of entries: 255
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/setup.cfg
+-rw-r--r--  2.0 unx     2288 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     5031 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/PKG-INFO
+-rw-r--r--  2.0 unx     3027 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/README.rst
+-rw-r--r--  2.0 unx     1989 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/MANIFEST.in
+-rw-r--r--  2.0 unx     1124 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/docs/LICENSE.GPL
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5031 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx      238 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     8165 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea.website.policy.egg-info/SOURCES.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/behaviors/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/version.txt
+-rw-r--r--  2.0 unx      502 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/configure.zcml
+-rw-r--r--  2.0 unx      714 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/setuphandlers.py
+-rw-r--r--  2.0 unx      242 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/interfaces.py
+-rw-r--r--  2.0 unx      352 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/README.txt
+-rw-r--r--  2.0 unx     1339 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles.zcml
+-rw-r--r--  2.0 unx      221 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--  2.0 unx      767 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/upgrades/configure.zcml
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/upgrades/__init__.py
+-rw-r--r--  2.0 unx     2018 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/tests/base.py
+-rw-r--r--  2.0 unx      676 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/tests/__init__.py
+-rw-r--r--  2.0 unx      234 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/behaviors/configure.zcml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/behaviors/__init__.py
+-rw-r--r--  2.0 unx      419 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/browser/configure.zcml
+-rw-r--r--  2.0 unx      480 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/browser/view.pt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/browser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/languages/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/
+-rw-r--r--  2.0 unx       87 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/languages/metadata.xml
+-rw-r--r--  2.0 unx      572 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/languages/registry.xml
+-rw-r--r--  2.0 unx      128 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/uninstall/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/
+-rw-r--r--  2.0 unx      368 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types.xml
+-rw-r--r--  2.0 unx      719 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx    11397 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/actions.xml
+-rw-r--r--  2.0 unx      553 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/repositorytool.xml
+-rw-r--r--  2.0 unx      179 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx   139757 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/topic_page.xml
+-rw-r--r--  2.0 unx    13612 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/landing_page.xml
+-rw-r--r--  2.0 unx      323 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/LRF.xml
+-rw-r--r--  2.0 unx     7717 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/faq.xml
+-rw-r--r--  2.0 unx     7085 b- defN 24-Apr-03 15:07 eea.website.policy-3.1/eea/website/policy/profiles/default/types/article.xml
+255 files, 238793 bytes uncompressed, 44859 bytes compressed:  81.2%
```

## zipnote {}

```diff
@@ -1,766 +1,766 @@
-Filename: eea.website.policy-3.0/
+Filename: eea.website.policy-3.1/
 Comment: 
 
-Filename: eea.website.policy-3.0/docs/
+Filename: eea.website.policy-3.1/docs/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/
+Filename: eea.website.policy-3.1/eea/
 Comment: 
 
-Filename: eea.website.policy-3.0/setup.cfg
+Filename: eea.website.policy-3.1/setup.cfg
 Comment: 
 
-Filename: eea.website.policy-3.0/CONTRIBUTING.md
+Filename: eea.website.policy-3.1/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.website.policy-3.0/PKG-INFO
+Filename: eea.website.policy-3.1/PKG-INFO
 Comment: 
 
-Filename: eea.website.policy-3.0/README.rst
+Filename: eea.website.policy-3.1/README.rst
 Comment: 
 
-Filename: eea.website.policy-3.0/setup.py
+Filename: eea.website.policy-3.1/setup.py
 Comment: 
 
-Filename: eea.website.policy-3.0/MANIFEST.in
+Filename: eea.website.policy-3.1/MANIFEST.in
 Comment: 
 
-Filename: eea.website.policy-3.0/docs/HISTORY.txt
+Filename: eea.website.policy-3.1/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/docs/LICENSE.txt
+Filename: eea.website.policy-3.1/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/docs/LICENSE.GPL
+Filename: eea.website.policy-3.1/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/entry_points.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/dependency_links.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/PKG-INFO
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/namespace_packages.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/not-zip-safe
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/requires.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/requires.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/top_level.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea.website.policy.egg-info/SOURCES.txt
+Filename: eea.website.policy-3.1/eea.website.policy.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/
+Filename: eea.website.policy-3.1/eea/website/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/__init__.py
+Filename: eea.website.policy-3.1/eea/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/
+Filename: eea.website.policy-3.1/eea/website/policy/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/__init__.py
+Filename: eea.website.policy-3.1/eea/website/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/upgrades/
+Filename: eea.website.policy-3.1/eea/website/policy/upgrades/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/tests/
+Filename: eea.website.policy-3.1/eea/website/policy/tests/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/behaviors/
+Filename: eea.website.policy-3.1/eea/website/policy/behaviors/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/browser/
+Filename: eea.website.policy-3.1/eea/website/policy/browser/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/version.txt
+Filename: eea.website.policy-3.1/eea/website/policy/version.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/configure.zcml
+Filename: eea.website.policy-3.1/eea/website/policy/configure.zcml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/setuphandlers.py
+Filename: eea.website.policy-3.1/eea/website/policy/setuphandlers.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/interfaces.py
+Filename: eea.website.policy-3.1/eea/website/policy/interfaces.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/README.txt
+Filename: eea.website.policy-3.1/eea/website/policy/README.txt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles.zcml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles.zcml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eea.pot
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eea.pot
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/update.sh
+Filename: eea.website.policy-3.1/eea/website/policy/locales/update.sh
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/plone-manual.pot
+Filename: eea.website.policy-3.1/eea/website/policy/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/locales/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/en/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/es/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/el/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/it/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/is/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/no/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/et/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/da/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/eea.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/locales/de/LC_MESSAGES/plone.po
+Filename: eea.website.policy-3.1/eea/website/policy/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/upgrades/configure.zcml
+Filename: eea.website.policy-3.1/eea/website/policy/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/upgrades/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/upgrades/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/tests/base.py
+Filename: eea.website.policy-3.1/eea/website/policy/tests/base.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/tests/test_doctests.py
+Filename: eea.website.policy-3.1/eea/website/policy/tests/test_doctests.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/tests/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/tests/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/behaviors/configure.zcml
+Filename: eea.website.policy-3.1/eea/website/policy/behaviors/configure.zcml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/behaviors/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/behaviors/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/browser/configure.zcml
+Filename: eea.website.policy-3.1/eea/website/policy/browser/configure.zcml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/browser/view.pt
+Filename: eea.website.policy-3.1/eea/website/policy/browser/view.pt
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/browser/__init__.py
+Filename: eea.website.policy-3.1/eea/website/policy/browser/__init__.py
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/languages/
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/languages/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/uninstall/
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/uninstall/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/languages/metadata.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/languages/metadata.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/languages/registry.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/languages/registry.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/uninstall/browserlayer.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/metadata.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/actions.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/actions.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/repositorytool.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/repositorytool.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/browserlayer.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/topic_page.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/topic_page.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/landing_page.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/landing_page.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/LRF.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/LRF.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/faq.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/faq.xml
 Comment: 
 
-Filename: eea.website.policy-3.0/eea/website/policy/profiles/default/types/article.xml
+Filename: eea.website.policy-3.1/eea/website/policy/profiles/default/types/article.xml
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.website.policy-3.0/CONTRIBUTING.md` & `eea.website.policy-3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/PKG-INFO` & `eea.website.policy-3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eea.website.policy
-Version: 3.0
+Version: 3.1
 Summary: EEA Website Plone backend policy
 Home-page: https://github.com/eea/eea.website.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -125,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.1 - (2024-04-03)
+---------------------------
+* Change: dummy release
+  [alecghica]
+
 3.0 - (2023-06-01)
 ---------------------------
 * Change: Persist EEA WWW GenericSetup profile
   [avoinea - refs #145772]
 * Feature: Add dependencies: 
   eea.progress.editing, eea.api.dataconnector, collective.volto.subsites
   [avoinea - refs #145772]
@@ -161,9 +165,7 @@
 * Change: Add EEA supported languages [avoinea]
 
 1.0 - (2022-03-18)
 -----------------------
 
 * Initial release.
   [eea]
-
-
```

## Comparing `eea.website.policy-3.0/README.rst` & `eea.website.policy-3.1/README.rst`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/setup.py` & `eea.website.policy-3.1/setup.py`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/docs/HISTORY.txt` & `eea.website.policy-3.1/docs/HISTORY.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+3.1 - (2024-04-03)
+---------------------------
+* Change: dummy release
+  [alecghica]
+
 3.0 - (2023-06-01)
 ---------------------------
 * Change: Persist EEA WWW GenericSetup profile
   [avoinea - refs #145772]
 * Feature: Add dependencies: 
   eea.progress.editing, eea.api.dataconnector, collective.volto.subsites
   [avoinea - refs #145772]
```

## Comparing `eea.website.policy-3.0/docs/LICENSE.txt` & `eea.website.policy-3.1/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/docs/LICENSE.GPL` & `eea.website.policy-3.1/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea.website.policy.egg-info/PKG-INFO` & `eea.website.policy-3.1/eea.website.policy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eea.website.policy
-Version: 3.0
+Version: 3.1
 Summary: EEA Website Plone backend policy
 Home-page: https://github.com/eea/eea.website.policy
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
 Classifier: Framework :: Plone :: Addon
 Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -125,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.1 - (2024-04-03)
+---------------------------
+* Change: dummy release
+  [alecghica]
+
 3.0 - (2023-06-01)
 ---------------------------
 * Change: Persist EEA WWW GenericSetup profile
   [avoinea - refs #145772]
 * Feature: Add dependencies: 
   eea.progress.editing, eea.api.dataconnector, collective.volto.subsites
   [avoinea - refs #145772]
@@ -161,9 +165,7 @@
 * Change: Add EEA supported languages [avoinea]
 
 1.0 - (2022-03-18)
 -----------------------
 
 * Initial release.
   [eea]
-
-
```

## Comparing `eea.website.policy-3.0/eea.website.policy.egg-info/SOURCES.txt` & `eea.website.policy-3.1/eea.website.policy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/setuphandlers.py` & `eea.website.policy-3.1/eea/website/policy/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles.zcml` & `eea.website.policy-3.1/eea/website/policy/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/upgrades/configure.zcml` & `eea.website.policy-3.1/eea/website/policy/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/tests/base.py` & `eea.website.policy-3.1/eea/website/policy/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/tests/test_doctests.py` & `eea.website.policy-3.1/eea/website/policy/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/languages/registry.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/languages/registry.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/metadata.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/metadata.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/actions.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/repositorytool.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/repositorytool.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/types/topic_page.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/types/topic_page.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/types/landing_page.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/types/landing_page.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/types/faq.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/types/faq.xml`

 * *Files identical despite different names*

## Comparing `eea.website.policy-3.0/eea/website/policy/profiles/default/types/article.xml` & `eea.website.policy-3.1/eea/website/policy/profiles/default/types/article.xml`

 * *Files identical despite different names*

