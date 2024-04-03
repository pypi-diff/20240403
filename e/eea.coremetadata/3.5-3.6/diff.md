# Comparing `tmp/eea.coremetadata-3.5.zip` & `tmp/eea.coremetadata-3.6.zip`

## zipinfo {}

```diff
@@ -1,257 +1,257 @@
-Zip file size: 86141 bytes, number of entries: 255
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/docs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/setup.cfg
--rw-r--r--  2.0 unx     2286 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/CONTRIBUTING.md
--rw-r--r--  2.0 unx     6570 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/PKG-INFO
--rw-r--r--  2.0 unx     2989 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/README.rst
--rw-r--r--  2.0 unx     1661 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/setup.py
--rw-r--r--  2.0 unx      126 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/MANIFEST.in
--rw-r--r--  2.0 unx       40 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6570 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/PKG-INFO
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/namespace_packages.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/not-zip-safe
--rw-r--r--  2.0 unx       57 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/requires.txt
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/top_level.txt
--rw-r--r--  2.0 unx     7931 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea.coremetadata.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     2718 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/docs/HISTORY.txt
--rw-r--r--  2.0 unx      915 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/docs/LICENSE.txt
--rw-r--r--  2.0 unx    18092 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/docs/LICENSE.GPL
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/
--rw-r--r--  2.0 unx       93 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/upgrades/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/tests/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/behaviors/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/browser/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/
--rw-r--r--  2.0 unx        4 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/version.txt
--rw-r--r--  2.0 unx      647 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/configure.zcml
--rw-r--r--  2.0 unx      668 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/setuphandlers.py
--rw-r--r--  2.0 unx     7270 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/interfaces.py
--rw-r--r--  2.0 unx      917 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/indexer.py
--rw-r--r--  2.0 unx      346 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/README.txt
--rw-r--r--  2.0 unx    23389 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/metadata.py
--rw-r--r--  2.0 unx      991 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles.zcml
--rw-r--r--  2.0 unx      221 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eea.pot
--rwxr-xr-x  2.0 unx      218 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/update.sh
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/plone-manual.pot
--rw-r--r--  2.0 unx       13 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
--rw-r--r--  2.0 unx     2071 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/upgrades/configure.zcml
--rw-r--r--  2.0 unx     5469 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/upgrades/to_24.py
--rw-r--r--  2.0 unx      822 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/upgrades/to_20.py
--rw-r--r--  2.0 unx       17 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/upgrades/__init__.py
--rw-r--r--  2.0 unx     1716 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/tests/base.py
--rw-r--r--  2.0 unx      672 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/tests/test_doctests.py
--rw-r--r--  2.0 unx       14 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/tests/__init__.py
--rw-r--r--  2.0 unx     1586 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/behaviors/configure.zcml
--rw-r--r--  2.0 unx     5039 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/behaviors/vocabulary.py
--rw-r--r--  2.0 unx     3244 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/behaviors/metadata.py
--rw-r--r--  2.0 unx       18 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/behaviors/__init__.py
--rw-r--r--  2.0 unx      141 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/browser/configure.zcml
--rw-r--r--  2.0 unx       16 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/browser/__init__.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/uninstall/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/
--rw-r--r--  2.0 unx      126 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/uninstall/browserlayer.xml
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/
--rw-r--r--  2.0 unx      187 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/metadata.xml
--rw-r--r--  2.0 unx      981 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/catalog.xml
--rw-r--r--  2.0 unx     3086 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/registry.xml
--rw-r--r--  2.0 unx      174 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/browserlayer.xml
--rw-r--r--  2.0 unx      209 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/topics.cfg
--rw-r--r--  2.0 unx      194 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
--rw-r--r--  2.0 unx     6611 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/topics.xml
--rw-r--r--  2.0 unx     3664 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.xml
--rw-r--r--  2.0 unx     3656 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/publisher.xml
--rw-r--r--  2.0 unx      182 b- defN 24-Mar-05 12:48 eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
-255 files, 126411 bytes uncompressed, 35607 bytes compressed:  71.8%
+Zip file size: 86180 bytes, number of entries: 255
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/docs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/setup.cfg
+-rw-r--r--  2.0 unx     2286 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/CONTRIBUTING.md
+-rw-r--r--  2.0 unx     6650 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/PKG-INFO
+-rw-r--r--  2.0 unx     2989 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/README.rst
+-rw-r--r--  2.0 unx     1661 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/setup.py
+-rw-r--r--  2.0 unx      126 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/MANIFEST.in
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6650 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/not-zip-safe
+-rw-r--r--  2.0 unx       57 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/requires.txt
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     7931 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea.coremetadata.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     2798 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/docs/HISTORY.txt
+-rw-r--r--  2.0 unx      915 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/docs/LICENSE.txt
+-rw-r--r--  2.0 unx    18092 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/docs/LICENSE.GPL
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/upgrades/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/tests/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/behaviors/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/browser/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/
+-rw-r--r--  2.0 unx        4 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/version.txt
+-rw-r--r--  2.0 unx      647 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/configure.zcml
+-rw-r--r--  2.0 unx      668 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/setuphandlers.py
+-rw-r--r--  2.0 unx     7270 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/interfaces.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/indexer.py
+-rw-r--r--  2.0 unx      346 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/README.txt
+-rw-r--r--  2.0 unx    23389 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/metadata.py
+-rw-r--r--  2.0 unx      991 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles.zcml
+-rw-r--r--  2.0 unx      221 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eea.pot
+-rwxr-xr-x  2.0 unx      218 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/update.sh
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/plone-manual.pot
+-rw-r--r--  2.0 unx       13 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
+-rw-r--r--  2.0 unx       28 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
+-rw-r--r--  2.0 unx     2071 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/upgrades/configure.zcml
+-rw-r--r--  2.0 unx     5469 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/upgrades/to_24.py
+-rw-r--r--  2.0 unx      822 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/upgrades/to_20.py
+-rw-r--r--  2.0 unx       17 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/upgrades/__init__.py
+-rw-r--r--  2.0 unx     1716 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/tests/base.py
+-rw-r--r--  2.0 unx      672 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/tests/test_doctests.py
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/tests/__init__.py
+-rw-r--r--  2.0 unx     1586 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/behaviors/configure.zcml
+-rw-r--r--  2.0 unx     5039 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/behaviors/vocabulary.py
+-rw-r--r--  2.0 unx     3244 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/behaviors/metadata.py
+-rw-r--r--  2.0 unx       18 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/behaviors/__init__.py
+-rw-r--r--  2.0 unx      141 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/browser/configure.zcml
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/browser/__init__.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/uninstall/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/
+-rw-r--r--  2.0 unx      126 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/uninstall/browserlayer.xml
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/metadata.xml
+-rw-r--r--  2.0 unx      981 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/catalog.xml
+-rw-r--r--  2.0 unx     3086 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/registry.xml
+-rw-r--r--  2.0 unx      174 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/browserlayer.xml
+-rw-r--r--  2.0 unx      209 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/topics.cfg
+-rw-r--r--  2.0 unx      194 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
+-rw-r--r--  2.0 unx     6611 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/topics.xml
+-rw-r--r--  2.0 unx     3665 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.xml
+-rw-r--r--  2.0 unx     3656 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/publisher.xml
+-rw-r--r--  2.0 unx      182 b- defN 24-Apr-03 12:35 eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
+255 files, 126652 bytes uncompressed, 35646 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,766 +1,766 @@
-Filename: eea.coremetadata-3.5/
+Filename: eea.coremetadata-3.6/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/
 Comment: 
 
-Filename: eea.coremetadata-3.5/docs/
+Filename: eea.coremetadata-3.6/docs/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/
+Filename: eea.coremetadata-3.6/eea/
 Comment: 
 
-Filename: eea.coremetadata-3.5/setup.cfg
+Filename: eea.coremetadata-3.6/setup.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.5/CONTRIBUTING.md
+Filename: eea.coremetadata-3.6/CONTRIBUTING.md
 Comment: 
 
-Filename: eea.coremetadata-3.5/PKG-INFO
+Filename: eea.coremetadata-3.6/PKG-INFO
 Comment: 
 
-Filename: eea.coremetadata-3.5/README.rst
+Filename: eea.coremetadata-3.6/README.rst
 Comment: 
 
-Filename: eea.coremetadata-3.5/setup.py
+Filename: eea.coremetadata-3.6/setup.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/MANIFEST.in
+Filename: eea.coremetadata-3.6/MANIFEST.in
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/entry_points.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/entry_points.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/dependency_links.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/dependency_links.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/PKG-INFO
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/PKG-INFO
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/namespace_packages.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/namespace_packages.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/not-zip-safe
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/not-zip-safe
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/requires.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/requires.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/top_level.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/top_level.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea.coremetadata.egg-info/SOURCES.txt
+Filename: eea.coremetadata-3.6/eea.coremetadata.egg-info/SOURCES.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/docs/HISTORY.txt
+Filename: eea.coremetadata-3.6/docs/HISTORY.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/docs/LICENSE.txt
+Filename: eea.coremetadata-3.6/docs/LICENSE.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/docs/LICENSE.GPL
+Filename: eea.coremetadata-3.6/docs/LICENSE.GPL
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/
+Filename: eea.coremetadata-3.6/eea/coremetadata/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/__init__.py
+Filename: eea.coremetadata-3.6/eea/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/upgrades/
+Filename: eea.coremetadata-3.6/eea/coremetadata/upgrades/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/tests/
+Filename: eea.coremetadata-3.6/eea/coremetadata/tests/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/behaviors/
+Filename: eea.coremetadata-3.6/eea/coremetadata/behaviors/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/browser/
+Filename: eea.coremetadata-3.6/eea/coremetadata/browser/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/version.txt
+Filename: eea.coremetadata-3.6/eea/coremetadata/version.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/configure.zcml
+Filename: eea.coremetadata-3.6/eea/coremetadata/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/setuphandlers.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/setuphandlers.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/interfaces.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/interfaces.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/indexer.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/indexer.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/README.txt
+Filename: eea.coremetadata-3.6/eea/coremetadata/README.txt
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/metadata.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/metadata.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles.zcml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eea.pot
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eea.pot
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/update.sh
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/update.sh
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/plone-manual.pot
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/plone-manual.pot
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/zh_TW/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/en/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/es/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt_BR/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ro/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/eu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/el/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/it/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/ru/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/is/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/hu/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/nl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fi/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/lv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/mt/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/tr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/no/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sv/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/bg/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/kl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/et/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/sk/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/pl/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/cs/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/da/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/fr/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/plone.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/eea.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/eea.mo
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
+Filename: eea.coremetadata-3.6/eea/coremetadata/locales/de/LC_MESSAGES/plone.po
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/upgrades/configure.zcml
+Filename: eea.coremetadata-3.6/eea/coremetadata/upgrades/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/upgrades/to_24.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/upgrades/to_24.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/upgrades/to_20.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/upgrades/to_20.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/upgrades/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/upgrades/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/tests/base.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/tests/base.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/tests/test_doctests.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/tests/test_doctests.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/tests/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/tests/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/behaviors/configure.zcml
+Filename: eea.coremetadata-3.6/eea/coremetadata/behaviors/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/behaviors/vocabulary.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/behaviors/vocabulary.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/behaviors/metadata.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/behaviors/metadata.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/behaviors/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/behaviors/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/browser/configure.zcml
+Filename: eea.coremetadata-3.6/eea/coremetadata/browser/configure.zcml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/browser/__init__.py
+Filename: eea.coremetadata-3.6/eea/coremetadata/browser/__init__.py
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/uninstall/
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/uninstall/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/uninstall/browserlayer.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/uninstall/browserlayer.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/metadata.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/metadata.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/catalog.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/catalog.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/registry.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/registry.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/browserlayer.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/browserlayer.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/topics.cfg
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/topics.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.cfg
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/topics.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/topics.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/publisher.xml
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/publisher.xml
 Comment: 
 
-Filename: eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
+Filename: eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/publisher.cfg
 Comment: 
 
 Zip file comment:
```

## Comparing `eea.coremetadata-3.5/CONTRIBUTING.md` & `eea.coremetadata-3.6/CONTRIBUTING.md`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/PKG-INFO` & `eea.coremetadata-3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.coremetadata
-Version: 3.5
+Version: 3.6
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.coremetadata
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -124,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.6 - (2024-04-03)
+---------------------------
+* Change: Develop
+  [alecghica]
+
 3.5 - (2024-03-05)
 ---------------------------
 * Feature: Expose rights field as metadata
   [dobri1408 - refs #159551]
 
 3.4 - (2023-10-16)
 ---------------------------
```

## Comparing `eea.coremetadata-3.5/README.rst` & `eea.coremetadata-3.6/README.rst`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/setup.py` & `eea.coremetadata-3.6/setup.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea.coremetadata.egg-info/PKG-INFO` & `eea.coremetadata-3.6/eea.coremetadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eea.coremetadata
-Version: 3.5
+Version: 3.6
 Summary: An add-on for Plone
 Home-page: https://github.com/eea/eea.coremetadata
 Author: European Environment Agency: IDM2 A-Team
 Author-email: eea-edw-a-team-alerts@googlegroups.com
 License: GPL version 2
 Keywords: EEA Add-ons Plone Zope
 Classifier: Environment :: Web Environment
@@ -124,14 +124,19 @@
 
 .. _EEA: https://www.eea.europa.eu/
 .. _`EEA Web Systems Training`: http://www.youtube.com/user/eeacms/videos?view=1
 
 Changelog
 =========
 
+3.6 - (2024-04-03)
+---------------------------
+* Change: Develop
+  [alecghica]
+
 3.5 - (2024-03-05)
 ---------------------------
 * Feature: Expose rights field as metadata
   [dobri1408 - refs #159551]
 
 3.4 - (2023-10-16)
 ---------------------------
```

## Comparing `eea.coremetadata-3.5/eea.coremetadata.egg-info/SOURCES.txt` & `eea.coremetadata-3.6/eea.coremetadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/docs/HISTORY.txt` & `eea.coremetadata-3.6/docs/HISTORY.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+3.6 - (2024-04-03)
+---------------------------
+* Change: Develop
+  [alecghica]
+
 3.5 - (2024-03-05)
 ---------------------------
 * Feature: Expose rights field as metadata
   [dobri1408 - refs #159551]
 
 3.4 - (2023-10-16)
 ---------------------------
```

## Comparing `eea.coremetadata-3.5/docs/LICENSE.txt` & `eea.coremetadata-3.6/docs/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/docs/LICENSE.GPL` & `eea.coremetadata-3.6/docs/LICENSE.GPL`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/configure.zcml` & `eea.coremetadata-3.6/eea/coremetadata/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/setuphandlers.py` & `eea.coremetadata-3.6/eea/coremetadata/setuphandlers.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/interfaces.py` & `eea.coremetadata-3.6/eea/coremetadata/interfaces.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/indexer.py` & `eea.coremetadata-3.6/eea/coremetadata/indexer.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/metadata.py` & `eea.coremetadata-3.6/eea/coremetadata/metadata.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles.zcml` & `eea.coremetadata-3.6/eea/coremetadata/profiles.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/upgrades/configure.zcml` & `eea.coremetadata-3.6/eea/coremetadata/upgrades/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/upgrades/to_24.py` & `eea.coremetadata-3.6/eea/coremetadata/upgrades/to_24.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/upgrades/to_20.py` & `eea.coremetadata-3.6/eea/coremetadata/upgrades/to_20.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/tests/base.py` & `eea.coremetadata-3.6/eea/coremetadata/tests/base.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/tests/test_doctests.py` & `eea.coremetadata-3.6/eea/coremetadata/tests/test_doctests.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/behaviors/configure.zcml` & `eea.coremetadata-3.6/eea/coremetadata/behaviors/configure.zcml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/behaviors/vocabulary.py` & `eea.coremetadata-3.6/eea/coremetadata/behaviors/vocabulary.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/behaviors/metadata.py` & `eea.coremetadata-3.6/eea/coremetadata/behaviors/metadata.py`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/catalog.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/catalog.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/registry.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/registry.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/topics.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/topics.xml`

 * *Files identical despite different names*

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.xml`

 * *Files 0% similar despite different names*

### Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/organisations.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/organisations.xml`

```diff
@@ -39,15 +39,15 @@
     <caption>
       <langstring language="en">European Food Safety Authority</langstring>
     </caption>
   </term>
   <term>
     <termIdentifier>ECHA</termIdentifier>
     <caption>
-      <langstring language="en">European Chemical Agency</langstring>
+      <langstring language="en">European Chemicals Agency</langstring>
     </caption>
   </term>
   <term>
     <termIdentifier>C3S</termIdentifier>
     <caption>
       <langstring language="en">Copernicus Climate Change Service (implemented by ECMWF)</langstring>
     </caption>
```

## Comparing `eea.coremetadata-3.5/eea/coremetadata/profiles/default/taxonomies/publisher.xml` & `eea.coremetadata-3.6/eea/coremetadata/profiles/default/taxonomies/publisher.xml`

 * *Files identical despite different names*

