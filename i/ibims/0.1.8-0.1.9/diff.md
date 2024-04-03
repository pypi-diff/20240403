# Comparing `tmp/ibims-0.1.8.tar.gz` & `tmp/ibims-0.1.9.tar.gz`

## Comparing `ibims-0.1.8.tar` & `ibims-0.1.9.tar`

### file list

```diff
@@ -1,307 +1,306 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ibims-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 ibims-0.1.8/.readthedocs.yml
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ibims-0.1.8/README.md
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ibims-0.1.8/domain-language.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ibims-0.1.8/requirements.in
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ibims-0.1.8/requirements.txt
--rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 ibims-0.1.8/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/docs.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/unittests.yml
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ibims-0.1.8/.github/workflows/updater.yml
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/bo4e_config.json
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/bo4e_updater.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/tox.env
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Bilanzierung.json
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Dokument.json
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/File.json
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Geschaeftspartner_extension.json
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Hinweis.json
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Kampagne.json
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Marktlokation_extension.json
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Rechnung_extension.json
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/ZaehlerGas.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/bo/Zaehler_extension.json
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Adresse_extension.json
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Bankverbindung.json
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/ConcessionFee.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Lastprofil.json
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Preisgarantie_extension.json
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Preisposition_extension.json
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Rechnungsposition_extension.json
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/SepaInfo.json
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Steuerbetrag_extension.json
--rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Verbrauch_extension.json
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Vertragskonto.json
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/VertragskontoCBA.json
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/VertragskontoMBA.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Zaehlpunkt.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/com/Zaehlwerk_extension.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Abgabeart.json
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/AblesendeRolle.json
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Ablesungsstatus.json
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Aggregationsverantwortung.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/HinweisThema.json
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Marktgebiet.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/MesstechnischeEinordnung.json
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Messwerterfassung.json
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Messwertstatus.json
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Profiltyp.json
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Prognosegrundlage.json
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Regelzone.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ibims-0.1.8/bo4e/models/enum/Variant.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-docs.in
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-docs.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-generate-bo4e.in
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-generate-bo4e.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-spellcheck.in
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-spellcheck.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ibims-0.1.8/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/.gitignore
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/Makefile
--rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/conf.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/index.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.8/docs/_static/.gitkeep
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ibims-0.1.8/src/_ibims_version.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/py.typed
--rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/__init__.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/__version__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/__init__.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/angebot.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/ansprechpartner.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/ausschreibung.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/bilanzierung.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/buendelvertrag.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/dokument.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/energiemenge.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/file.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/fremdkosten.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/hinweis.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/kampagne.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/kosten.py
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/lastgang.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/lastgang_kompakt.py
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/marktlokation.py
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/messlokation.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/netznutzungsrechnung.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt.py
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_dienstleistung.py
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_hardware.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_konzessionsabgabe.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_messung.py
--rw-r--r--   0        0        0     1908 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_netznutzung.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/rechnung.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/region.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/regionaltarif.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/tarif.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/tarifinfo.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/tarifkosten.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/vertrag.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/zaehler.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/zaehler_gas.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/bo/zeitreihe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/adresse.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/angebotsposition.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/angebotsteil.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/angebotsvariante.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag_pro_ort.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag_regional.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/auf_abschlagstaffel_pro_ort.py
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/ausschreibungslos.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/bankverbindung.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/betrag.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/com.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/concession_fee.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/dienstleistung.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/energieherkunft.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/energiemix.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/externe_referenz.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/fremdkostenblock.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/fremdkostenposition.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/geokoordinaten.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/geraet.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/geraeteeigenschaften.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/hardware.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/katasteradresse.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/kostenblock.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/kostenposition.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/kriterium_wert.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/lastprofil.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/marktgebiet_info.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/menge.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/positions_auf_abschlag.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/preis.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/preisgarantie.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/preisposition.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/preisstaffel.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/rechnungsposition.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionale_gueltigkeit.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionale_preisgarantie.py
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionale_preisstaffel.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionale_tarifpreisposition.py
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionaler_auf_abschlag.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/regionskriterium.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/rufnummer.py
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/sepa_info.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/sigmoidparameter.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/standorteigenschaften_gas.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/standorteigenschaften_strom.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/steuerbetrag.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tagesvektor.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifpreis.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifpreisposition.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifpreisposition_pro_ort.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/tarifpreisstaffel_pro_ort.py
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/unterschrift.py
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/verbrauch.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/vertragskonditionen.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/vertragskonto.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/vertragskonto_cba.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/vertragskonto_mba.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/vertragsteil.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zaehlpunkt.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zaehlwerk.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zeitintervall.py
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zeitraum.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zeitreihenwert.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zeitreihenwertkompakt.py
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/com/zustaendigkeit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/abgabeart.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/ablesende_rolle.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/ablesungsstatus.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/aggregationsverantwortung.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/angebotsstatus.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/anrede.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/artikel_id.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/auf_abschlagstyp.py
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/auf_abschlagsziel.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/bdew_artikelnummer.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/bo_typ.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/energierichtung.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/erzeugungsart.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/gasqualitaet.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/gebiettyp.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/geraetemerkmal.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/geraetetyp.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/hinweis_thema.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kontaktart.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kostenklasse.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kundengruppe.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kundengruppe_ka.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/kundentyp.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/landescode.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/leistungstyp.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/lokationstyp.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/marktgebiet.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/marktrolle.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/medium.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/mengeneinheit.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/mengenoperator.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messart.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messgroesse.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messpreistyp.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messtechnische_einordnung.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messwerterfassung.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messwertstatus.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/netzebene.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/nn_rechnungsart.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/nn_rechnungstyp.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/oekolabel.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/oekozertifikat.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/preismodell.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/preisstatus.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/preistyp.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/profiltyp.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/prognosegrundlage.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/rechnungslegung.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/rechnungstyp.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/regelzone.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/rollencodetyp.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/rufnummernart.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/sparte.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tarifart.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tariftyp.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/tarifzeit.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/themengebiet.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/titel.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/variant.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/verbrauchsart.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/vertragsart.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/vertragsform.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/vertragsstatus.py
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/voraussetzungen.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/waehrungscode.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/zaehlertyp.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/bo4e/enum/zeiteinheit.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/__init__.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/agent_hint_loader.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/base.py
--rw-r--r--   0        0        0     2820 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/customer_loader.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/document_loader.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/invoice_loader.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/network_loader.py
--rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/product_loader.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/quantities_loader.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/resource_loader.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/datasets/usage_loader.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/meta/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/targetmodels/__init__.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 ibims-0.1.8/src/ibims/targetmodels/transactiondata.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ibims-0.1.8/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ibims-0.1.8/LICENSE
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ibims-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 ibims-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 ibims-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 ibims-0.1.9/.readthedocs.yml
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 ibims-0.1.9/README.md
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ibims-0.1.9/domain-language.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ibims-0.1.9/requirements.in
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ibims-0.1.9/requirements.txt
+-rw-r--r--   0        0        0     3476 2020-02-02 00:00:00.000000 ibims-0.1.9/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ibims-0.1.9/.github/workflows/updater.yml
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/bo4e_config.json
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/bo4e_updater.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/tox.env
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Bilanzierung.json
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Dokument.json
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/File.json
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Geschaeftspartner_extension.json
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Hinweis.json
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Kampagne.json
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Marktlokation_extension.json
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Rechnung_extension.json
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/ZaehlerGas.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/bo/Zaehler_extension.json
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Adresse_extension.json
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Bankverbindung.json
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/ConcessionFee.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Lastprofil.json
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Preisgarantie_extension.json
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Preisposition_extension.json
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Rechnungsposition_extension.json
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/SepaInfo.json
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Steuerbetrag_extension.json
+-rw-r--r--   0        0        0     3978 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Verbrauch_extension.json
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/VertragskontoCBA.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/VertragskontoMBA.json
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Zaehlpunkt.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/com/Zaehlwerk_extension.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Abgabeart.json
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/AblesendeRolle.json
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Ablesungsstatus.json
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Aggregationsverantwortung.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/HinweisThema.json
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Marktgebiet.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/MesstechnischeEinordnung.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Messwerterfassung.json
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Messwertstatus.json
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Profiltyp.json
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Prognosegrundlage.json
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Regelzone.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ibims-0.1.9/bo4e/models/enum/Variant.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-docs.in
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-docs.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-generate-bo4e.in
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-generate-bo4e.txt
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-spellcheck.in
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-spellcheck.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 ibims-0.1.9/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/Makefile
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/conf.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/index.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.9/docs/_static/.gitkeep
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 ibims-0.1.9/src/_ibims_version.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/py.typed
+-rw-r--r--   0        0        0    13954 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/__init__.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/__version__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/__init__.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/angebot.py
+-rw-r--r--   0        0        0     1956 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/ansprechpartner.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/ausschreibung.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/bilanzierung.py
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/dokument.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/energiemenge.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/file.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/fremdkosten.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/hinweis.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/kampagne.py
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/kosten.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/lastgang.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/lastgang_kompakt.py
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/marktlokation.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/messlokation.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/netznutzungsrechnung.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt.py
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_dienstleistung.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_hardware.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_konzessionsabgabe.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_messung.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_netznutzung.py
+-rw-r--r--   0        0        0     2995 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/rechnung.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/region.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/regionaltarif.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/tarif.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/tarifinfo.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/tarifkosten.py
+-rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0        0        0     2385 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/vertrag.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/zaehler.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/zaehler_gas.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/bo/zeitreihe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/__init__.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/adresse.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/angebotsposition.py
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/angebotsteil.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/angebotsvariante.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag_pro_ort.py
+-rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag_regional.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/auf_abschlagstaffel_pro_ort.py
+-rw-r--r--   0        0        0     2155 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/bankverbindung.py
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/betrag.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/com.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/concession_fee.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/dienstleistung.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/energieherkunft.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/energiemix.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/externe_referenz.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/geokoordinaten.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/geraet.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/geraeteeigenschaften.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/hardware.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/katasteradresse.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/kostenblock.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/kostenposition.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/kriterium_wert.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/lastprofil.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/marktgebiet_info.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/menge.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/positions_auf_abschlag.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/preis.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/preisgarantie.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/preisposition.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/preisstaffel.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/rechnungsposition.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionale_gueltigkeit.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionale_preisgarantie.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionale_preisstaffel.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionale_tarifpreisposition.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionaler_auf_abschlag.py
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/regionskriterium.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/rufnummer.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/sepa_info.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/standorteigenschaften_gas.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/standorteigenschaften_strom.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/steuerbetrag.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tagesvektor.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifpreis.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifpreisposition_pro_ort.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/tarifpreisstaffel_pro_ort.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/unterschrift.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/verbrauch.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/vertragskonto.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/vertragskonto_cba.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/vertragskonto_mba.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/vertragsteil.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zaehlpunkt.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zaehlwerk.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zeitintervall.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zeitraum.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zeitreihenwertkompakt.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/com/zustaendigkeit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/abgabeart.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/ablesende_rolle.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/ablesungsstatus.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/aggregationsverantwortung.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/anrede.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/artikel_id.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/auf_abschlagstyp.py
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/auf_abschlagsziel.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/bdew_artikelnummer.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/bo_typ.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/energierichtung.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/gebiettyp.py
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/geraetemerkmal.py
+-rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/geraetetyp.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/hinweis_thema.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kontaktart.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kostenklasse.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kundengruppe.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kundengruppe_ka.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/kundentyp.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/landescode.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/leistungstyp.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/lokationstyp.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/marktgebiet.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/marktrolle.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/medium.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/mengenoperator.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messart.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messgroesse.py
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messpreistyp.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messtechnische_einordnung.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messwerterfassung.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messwertstatus.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/netzebene.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/nn_rechnungsart.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/nn_rechnungstyp.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/oekolabel.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/preismodell.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/preisstatus.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/preistyp.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/profiltyp.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/prognosegrundlage.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/regelzone.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/rufnummernart.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/sparte.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tarifart.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tariftyp.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/tarifzeit.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/themengebiet.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/titel.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/variant.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/vertragsart.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/vertragsform.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/waehrungscode.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/bo4e/enum/zeiteinheit.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/__init__.py
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/agent_hint_loader.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/base.py
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/customer_loader.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/document_loader.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/invoice_loader.py
+-rw-r--r--   0        0        0     3004 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/network_loader.py
+-rw-r--r--   0        0        0     2920 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/product_loader.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/quantities_loader.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/resource_loader.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/datasets/usage_loader.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/meta/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/targetmodels/__init__.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 ibims-0.1.9/src/ibims/targetmodels/transactiondata.py
+-rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 ibims-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 ibims-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 ibims-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 ibims-0.1.9/PKG-INFO
```

### Comparing `ibims-0.1.8/.pre-commit-config.yaml` & `ibims-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.readthedocs.yml` & `ibims-0.1.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/README.md` & `ibims-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/requirements.txt` & `ibims-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/tox.ini` & `ibims-0.1.9/tox.ini`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/dependabot.yml` & `ibims-0.1.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/codeql-analysis.yml` & `ibims-0.1.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/coverage.yml` & `ibims-0.1.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/dependabot_automerge.yml` & `ibims-0.1.9/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/docs.yml` & `ibims-0.1.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/formatting.yml` & `ibims-0.1.9/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/packaging_test.yml` & `ibims-0.1.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/python-publish.yml` & `ibims-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/pythonlint.yml` & `ibims-0.1.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/unittests.yml` & `ibims-0.1.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.github/workflows/updater.yml` & `ibims-0.1.9/.github/workflows/updater.yml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/bo4e_config.json` & `ibims-0.1.9/bo4e/bo4e_config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953703703703703%*

 * *Differences: {"'additionalModels'": '{delete: [10]}'}*

```diff
@@ -142,20 +142,14 @@
             "schema": {
                 "$ref": "models/com/SepaInfo.json"
             }
         },
         {
             "module": "com",
             "schema": {
-                "$ref": "models/com/Vertragskonto.json"
-            }
-        },
-        {
-            "module": "com",
-            "schema": {
                 "$ref": "models/com/VertragskontoCBA.json"
             }
         },
         {
             "module": "com",
             "schema": {
                 "$ref": "models/com/VertragskontoMBA.json"
```

### Comparing `ibims-0.1.8/bo4e/bo4e_updater.py` & `ibims-0.1.9/bo4e/bo4e_updater.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Bilanzierung.json` & `ibims-0.1.9/bo4e/models/bo/Bilanzierung.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Dokument.json` & `ibims-0.1.9/bo4e/models/bo/Dokument.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/File.json` & `ibims-0.1.9/bo4e/models/bo/File.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Geschaeftspartner_extension.json` & `ibims-0.1.9/bo4e/models/bo/Geschaeftspartner_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Hinweis.json` & `ibims-0.1.9/bo4e/models/bo/Hinweis.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Kampagne.json` & `ibims-0.1.9/bo4e/models/bo/Kampagne.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Marktlokation_extension.json` & `ibims-0.1.9/bo4e/models/bo/Marktlokation_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Rechnung_extension.json` & `ibims-0.1.9/bo4e/models/bo/Rechnung_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/ZaehlerGas.json` & `ibims-0.1.9/bo4e/models/bo/ZaehlerGas.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/bo/Zaehler_extension.json` & `ibims-0.1.9/bo4e/models/bo/Zaehler_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/Bankverbindung.json` & `ibims-0.1.9/bo4e/models/com/Bankverbindung.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/ConcessionFee.json` & `ibims-0.1.9/bo4e/models/com/ConcessionFee.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/Lastprofil.json` & `ibims-0.1.9/bo4e/models/com/Lastprofil.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/SepaInfo.json` & `ibims-0.1.9/bo4e/models/com/SepaInfo.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/Verbrauch_extension.json` & `ibims-0.1.9/bo4e/models/com/Verbrauch_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/VertragskontoCBA.json` & `ibims-0.1.9/bo4e/models/com/VertragskontoCBA.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/VertragskontoMBA.json` & `ibims-0.1.9/bo4e/models/com/VertragskontoMBA.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/Zaehlpunkt.json` & `ibims-0.1.9/bo4e/models/com/Zaehlpunkt.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/com/Zaehlwerk_extension.json` & `ibims-0.1.9/bo4e/models/com/Zaehlwerk_extension.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/enum/Aggregationsverantwortung.json` & `ibims-0.1.9/bo4e/models/enum/Aggregationsverantwortung.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/enum/HinweisThema.json` & `ibims-0.1.9/bo4e/models/enum/HinweisThema.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/bo4e/models/enum/Messwertstatus.json` & `ibims-0.1.9/bo4e/models/enum/Messwertstatus.json`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/dev_requirements/requirements-docs.txt` & `ibims-0.1.9/dev_requirements/requirements-docs.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,34 +16,34 @@
     # via
     #   sphinx
     #   sphinx-rtd-theme
 idna==3.4
     # via requests
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.2
+jinja2==3.1.3
     # via sphinx
 markupsafe==2.1.2
     # via jinja2
 packaging==23.0
     # via sphinx
 pygments==2.15.0
     # via sphinx
 requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
 sphinx==7.2.6
     # via
-    #   -r dev_requirements/requirements-docs.in
+    #   -r requirements-docs.in
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
     #   sphinxcontrib-serializinghtml
 sphinx-rtd-theme==2.0.0
-    # via -r dev_requirements/requirements-docs.in
+    # via -r requirements-docs.in
 sphinxcontrib-applehelp==1.0.4
     # via sphinx
 sphinxcontrib-devhelp==1.0.2
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.1
     # via sphinx
 sphinxcontrib-jquery==4.1
```

### Comparing `ibims-0.1.8/dev_requirements/requirements-generate-bo4e.txt` & `ibims-0.1.9/dev_requirements/requirements-generate-bo4e.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 #
 annotated-types==0.5.0
     # via pydantic
 argcomplete==3.1.6
     # via datamodel-code-generator
 black==23.12.1
     # via datamodel-code-generator
-bo4e-python-generator==0.0.3
-    # via -r dev_requirements/requirements-generate-bo4e.in
+bo4e-python-generator==0.0.4
+    # via -r requirements-generate-bo4e.in
 bo4e-schema-tool==0.0.2
-    # via -r dev_requirements/requirements-generate-bo4e.in
+    # via -r requirements-generate-bo4e.in
 certifi==2023.7.22
     # via requests
 charset-normalizer==3.1.0
     # via requests
 click==8.1.3
     # via
     #   black
@@ -35,15 +35,15 @@
     # via
     #   email-validator
     #   requests
 inflect==5.6.2
     # via datamodel-code-generator
 isort==5.13.2
     # via datamodel-code-generator
-jinja2==3.1.2
+jinja2==3.1.3
     # via datamodel-code-generator
 markupsafe==2.1.2
     # via jinja2
 more-itertools==10.1.0
     # via bo4e-schema-tool
 mypy-extensions==1.0.0
     # via black
@@ -58,20 +58,20 @@
 pydantic[email]==2.3.0
     # via
     #   bo4e-schema-tool
     #   datamodel-code-generator
 pydantic-core==2.6.3
     # via pydantic
 python-dotenv==1.0.0
-    # via -r dev_requirements/requirements-generate-bo4e.in
+    # via -r requirements-generate-bo4e.in
 pyyaml==6.0.1
     # via datamodel-code-generator
 requests==2.31.0
     # via
-    #   -r dev_requirements/requirements-generate-bo4e.in
+    #   -r requirements-generate-bo4e.in
     #   bo4e-schema-tool
 typing-extensions==4.7.1
     # via
     #   pydantic
     #   pydantic-core
 urllib3==2.1.0
     # via requests
```

### Comparing `ibims-0.1.8/dev_requirements/requirements-packaging.txt` & `ibims-0.1.9/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/docs/Makefile` & `ibims-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/docs/conf.py` & `ibims-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/docs/make.bat` & `ibims-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/__init__.py` & `ibims-0.1.9/src/ibims/bo4e/__init__.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/angebot.py` & `ibims-0.1.9/src/ibims/bo4e/bo/angebot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.angebotsvariante import Angebotsvariante
 from ..com.externe_referenz import ExterneReferenz
 from ..enum.bo_typ import BoTyp
 from ..enum.sparte import Sparte
 from .ansprechpartner import Ansprechpartner
@@ -22,22 +24,23 @@
 
     .. HINT::
         `Angebot JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Angebot.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anfragereferenz: Annotated[str | None, Field(None, title="Anfragereferenz")]
-    angebotsdatum: Annotated[AwareDatetime | None, Field(None, title="Angebotsdatum")]
+    angebotsdatum: Annotated[datetime | None, Field(None, title="Angebotsdatum")]
     angebotsgeber: Geschaeftspartner | None = None
     angebotsnehmer: Geschaeftspartner | None = None
     angebotsnummer: Annotated[str | None, Field(None, title="Angebotsnummer")]
-    bindefrist: Annotated[AwareDatetime | None, Field(None, title="Bindefrist")]
+    bindefrist: Annotated[datetime | None, Field(None, title="Bindefrist")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ANGEBOT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     sparte: Sparte | None = None
     unterzeichner_angebotsgeber: Annotated[Ansprechpartner | None, Field(None, alias="unterzeichnerAngebotsgeber")]
     unterzeichner_angebotsnehmer: Annotated[Ansprechpartner | None, Field(None, alias="unterzeichnerAngebotsnehmer")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/ansprechpartner.py` & `ibims-0.1.9/src/ibims/bo4e/bo/ansprechpartner.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     .. HINT::
         `Ansprechpartner JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Ansprechpartner.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     adresse: Adresse | None = None
     anrede: Anrede | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ANSPRECHPARTNER, alias="boTyp")]
     e_mail_adresse: Annotated[str | None, Field(None, alias="eMailAdresse", title="Emailadresse")]
     externe_referenzen: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/ausschreibung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/ausschreibung.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.ausschreibungslos import Ausschreibungslos
 from ..com.externe_referenz import ExterneReferenz
 from ..com.zeitraum import Zeitraum
 from ..enum.ausschreibungsportal import Ausschreibungsportal
 from ..enum.ausschreibungsstatus import Ausschreibungsstatus
@@ -21,14 +23,15 @@
 
     .. HINT::
         `Ausschreibung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Ausschreibung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     abgabefrist: Zeitraum | None = None
     ausschreibender: Geschaeftspartner | None = None
     ausschreibungportal: Ausschreibungsportal | None = None
     ausschreibungsnummer: Annotated[str | None, Field(None, title="Ausschreibungsnummer")]
     ausschreibungsstatus: Ausschreibungsstatus | None = None
@@ -36,10 +39,10 @@
     bindefrist: Zeitraum | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.AUSSCHREIUNG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     kostenpflichtig: Annotated[bool | None, Field(None, title="Kostenpflichtig")]
     lose: Annotated[list[Ausschreibungslos] | None, Field(None, title="Lose")]
-    veroeffentlichungszeitpunkt: Annotated[AwareDatetime | None, Field(None, title="Veroeffentlichungszeitpunkt")]
+    veroeffentlichungszeitpunkt: Annotated[datetime | None, Field(None, title="Veroeffentlichungszeitpunkt")]
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     webseite: Annotated[str | None, Field(None, title="Webseite")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/bilanzierung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/bilanzierung.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..com.lastprofil import Lastprofil
 from ..enum.aggregationsverantwortung import Aggregationsverantwortung
 from ..enum.bo_typ import BoTyp
 from ..enum.profiltyp import Profiltyp
@@ -14,21 +16,22 @@
     Bilanzierung is a business object used for balancing. This object is no BO4E standard and a complete go
     implementation can be found at
     https://github.com/Hochfrequenz/go-bo4e/blob/3414a1eac741542628df796d6beb43eaa27b0b3e/bo/bilanzierung.go
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     bo_typ: Annotated[BoTyp | None, Field("BILANZIERUNG", alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    bilanzierungsbeginn: Annotated[AwareDatetime, Field(title="Bilanzierungsbeginn")]
-    bilanzierungsende: Annotated[AwareDatetime, Field(title="Bilanzierungsende")]
+    bilanzierungsbeginn: Annotated[datetime, Field(title="Bilanzierungsbeginn")]
+    bilanzierungsende: Annotated[datetime, Field(title="Bilanzierungsende")]
     bilanzkreis: Annotated[str | None, Field(None, title="Bilanzkreis")]
     aggregationsverantwortung: Aggregationsverantwortung | None = None
     lastprofile: Annotated[list[Lastprofil] | None, Field(None, title="Lastprofile")]
     prognosegrundlage: Prognosegrundlage | None = None
     details_prognosegrundlage: Annotated[Profiltyp | None, Field(None, alias="detailsPrognosegrundlage")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/buendelvertrag.py` & `ibims-0.1.9/src/ibims/bo4e/bo/buendelvertrag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..com.unterschrift import Unterschrift
 from ..com.vertragskonditionen import Vertragskonditionen
 from ..enum.bo_typ import BoTyp
 from ..enum.sparte import Sparte
@@ -23,27 +25,28 @@
 
     .. HINT::
         `Buendelvertrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Buendelvertrag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.BUENDELVERTRAG, alias="boTyp")]
     einzelvertraege: Annotated[list[Vertrag] | None, Field(None, title="Einzelvertraege")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     sparte: Sparte | None = None
     unterzeichnervp1: Annotated[list[Unterschrift] | None, Field(None, title="Unterzeichnervp1")]
     unterzeichnervp2: Annotated[list[Unterschrift] | None, Field(None, title="Unterzeichnervp2")]
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     vertragsart: Vertragsart | None = None
-    vertragsbeginn: Annotated[AwareDatetime | None, Field(None, title="Vertragsbeginn")]
-    vertragsende: Annotated[AwareDatetime | None, Field(None, title="Vertragsende")]
+    vertragsbeginn: Annotated[datetime | None, Field(None, title="Vertragsbeginn")]
+    vertragsende: Annotated[datetime | None, Field(None, title="Vertragsende")]
     vertragskonditionen: Annotated[list[Vertragskonditionen] | None, Field(None, title="Vertragskonditionen")]
     vertragsnummer: Annotated[str | None, Field(None, title="Vertragsnummer")]
     vertragspartner1: Geschaeftspartner | None = None
     vertragspartner2: Geschaeftspartner | None = None
     vertragsstatus: Vertragsstatus | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/dokument.py` & `ibims-0.1.9/src/ibims/bo4e/bo/kampagne.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..enum.bo_typ import BoTyp
 
 
-class Dokument(BaseModel):
+class Kampagne(BaseModel):
     """
-    A generic document reference like for bills, order confirmations and cancellations
+    A "Kampagne"/campaign models which marketing activities led customers to a product/tariff.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.GESCHAEFTSOBJEKT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
-    id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    erstellungsdatum: Annotated[AwareDatetime, Field(title="Erstellungsdatum")]
-    has_been_sent: Annotated[bool, Field(alias="hasBeenSent", title="Hasbeensent")]
-    dokumentenname: Annotated[str, Field(title="Dokumentenname")]
-    vorlagenname: Annotated[str, Field(title="Vorlagenname")]
+    id: Annotated[str, Field(title="Id")]
+    name: Annotated[str, Field(title="Name")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/energiemenge.py` & `ibims-0.1.9/src/ibims/bo4e/bo/energiemenge.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     .. HINT::
         `Energiemenge JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Energiemenge.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ENERGIEMENGE, alias="boTyp")]
     energieverbrauch: Annotated[list[Verbrauch] | None, Field(None, title="Energieverbrauch")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/fremdkosten.py` & `ibims-0.1.9/src/ibims/bo4e/bo/fremdkosten.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     .. HINT::
         `Fremdkosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Fremdkosten.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.FREMDKOSTEN, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     gueltigkeit: Zeitraum | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/geschaeftsobjekt.py` & `ibims-0.1.9/src/ibims/bo4e/bo/geschaeftsobjekt.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     .. HINT::
         `Geschaeftsobjekt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Geschaeftsobjekt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.GESCHAEFTSOBJEKT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/geschaeftspartner.py` & `ibims-0.1.9/src/ibims/bo4e/bo/geschaeftspartner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.adresse import Adresse
 from ..com.externe_referenz import ExterneReferenz
 from ..enum.anrede import Anrede
 from ..enum.bo_typ import BoTyp
 from ..enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
@@ -22,14 +24,15 @@
 
     .. HINT::
         `Geschaeftspartner JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Geschaeftspartner.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     amtsgericht: Annotated[str | None, Field(None, title="Amtsgericht")]
     anrede: Anrede | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.GESCHAEFTSPARTNER, alias="boTyp")]
     e_mail_adresse: Annotated[str | None, Field(None, alias="eMailAdresse", title="Emailadresse")]
     externe_referenzen: Annotated[
@@ -43,16 +46,16 @@
     name1: Annotated[str | None, Field(None, title="Name1")]
     name2: Annotated[str | None, Field(None, title="Name2")]
     name3: Annotated[str | None, Field(None, title="Name3")]
     partneradresse: Adresse | None = None
     umsatzsteuer_id: Annotated[str | None, Field(None, alias="umsatzsteuerId", title="Umsatzsteuerid")]
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     website: Annotated[str | None, Field(None, title="Website")]
-    erstellungsdatum: Annotated[AwareDatetime | None, Field(None, title="Erstellungsdatum")]
-    geburtstag: Annotated[AwareDatetime | None, Field(None, title="Geburtstag")]
+    erstellungsdatum: Annotated[datetime | None, Field(None, title="Erstellungsdatum")]
+    geburtstag: Annotated[datetime | None, Field(None, title="Geburtstag")]
     telefonnummer_mobil: Annotated[str | None, Field(None, alias="telefonnummerMobil", title="Telefonnummermobil")]
     telefonnummer_privat: Annotated[str | None, Field(None, alias="telefonnummerPrivat", title="Telefonnummerprivat")]
     telefonnummer_geschaeft: Annotated[
         str | None, Field(None, alias="telefonnummerGeschaeft", title="Telefonnummergeschaeft")
     ]
     firmenname: Annotated[str | None, Field(None, title="Firmenname")]
     hausbesitzer: Annotated[bool | None, Field(None, title="Hausbesitzer")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/hinweis.py` & `ibims-0.1.9/src/ibims/bo4e/bo/hinweis.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..enum.bo_typ import BoTyp
 from ..enum.hinweis_thema import HinweisThema
 
 
@@ -10,17 +12,18 @@
     """
     Contains specific hints for the handling of contracts and customers.
     Hints are meant to be read and written by agents or customer service employees.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.GESCHAEFTSOBJEKT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    erstellungsdatum: Annotated[AwareDatetime, Field(title="Erstellungsdatum")]
+    erstellungsdatum: Annotated[datetime, Field(title="Erstellungsdatum")]
     thema: Annotated[HinweisThema | str, Field(title="Thema")]
     nachricht: Annotated[str, Field(title="Nachricht")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/kosten.py` & `ibims-0.1.9/src/ibims/bo4e/bo/kosten.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     .. HINT::
         `Kosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Kosten.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.KOSTEN, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     gueltigkeit: Zeitraum | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/lastgang.py` & `ibims-0.1.9/src/ibims/bo4e/bo/lastgang.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     .. HINT::
         `Lastgang JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Lastgang.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.LASTGANG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     lokations_id: Annotated[str | None, Field(None, alias="lokationsId", title="Lokationsid")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/lastgang_kompakt.py` & `ibims-0.1.9/src/ibims/bo4e/bo/lastgang_kompakt.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Modell zur Abbildung eines kompakten Lastganges.
     In diesem Modell werden die Messwerte in Form von Tagesvektoren mit fester Anzahl von Werten übertragen.
     Daher ist dieses BO nur zur Übertragung von äquidistanten Messwertverläufen geeignet.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.LASTGANG_KOMPAKT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     lokations_id: Annotated[str | None, Field(None, alias="lokationsId", title="Lokationsid")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/marktlokation.py` & `ibims-0.1.9/src/ibims/bo4e/bo/marktlokation.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 
     .. HINT::
         `Marktlokation JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Marktlokation.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bilanzierungsgebiet: Annotated[str | None, Field(None, title="Bilanzierungsgebiet")]
     bilanzierungsmethode: Bilanzierungsmethode | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.MARKTLOKATION, alias="boTyp")]
     endkunde: Geschaeftspartner | None = None
     energierichtung: Energierichtung | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/marktteilnehmer.py` & `ibims-0.1.9/src/ibims/bo4e/bo/marktteilnehmer.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     .. HINT::
         `Marktteilnehmer JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Marktteilnehmer.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     amtsgericht: Annotated[str | None, Field(None, title="Amtsgericht")]
     anrede: Anrede | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.MARKTTEILNEHMER, alias="boTyp")]
     e_mail_adresse: Annotated[str | None, Field(None, alias="eMailAdresse", title="Emailadresse")]
     externe_referenzen: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/messlokation.py` & `ibims-0.1.9/src/ibims/bo4e/bo/messlokation.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     .. HINT::
         `Messlokation JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Messlokation.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.MESSLOKATION, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     geoadresse: Geokoordinaten | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/netznutzungsrechnung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/netznutzungsrechnung.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.betrag import Betrag
 from ..com.externe_referenz import ExterneReferenz
 from ..com.rechnungsposition import Rechnungsposition
 from ..com.steuerbetrag import Steuerbetrag
 from ..com.zeitraum import Zeitraum
@@ -25,35 +27,36 @@
 
     .. HINT::
         `Netznutzungsrechnung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Netznutzungsrechnung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     absendercodenummer: Annotated[str | None, Field(None, title="Absendercodenummer")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.NETZNUTZUNGSRECHNUNG, alias="boTyp")]
     empfaengercodenummer: Annotated[str | None, Field(None, title="Empfaengercodenummer")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
-    faelligkeitsdatum: Annotated[AwareDatetime | None, Field(None, title="Faelligkeitsdatum")]
+    faelligkeitsdatum: Annotated[datetime | None, Field(None, title="Faelligkeitsdatum")]
     gesamtbrutto: Betrag | None = None
     gesamtnetto: Betrag | None = None
     gesamtsteuer: Betrag | None = None
     lokations_id: Annotated[str | None, Field(None, alias="lokationsId", title="Lokationsid")]
     nnrechnungsart: NNRechnungsart | None = None
     nnrechnungstyp: NNRechnungstyp | None = None
     original: Annotated[bool | None, Field(None, title="Original")]
     original_rechnungsnummer: Annotated[
         str | None, Field(None, alias="originalRechnungsnummer", title="Originalrechnungsnummer")
     ]
     rabatt_brutto: Annotated[Betrag | None, Field(None, alias="rabattBrutto")]
-    rechnungsdatum: Annotated[AwareDatetime | None, Field(None, title="Rechnungsdatum")]
+    rechnungsdatum: Annotated[datetime | None, Field(None, title="Rechnungsdatum")]
     rechnungsempfaenger: Geschaeftspartner | None = None
     rechnungsersteller: Geschaeftspartner | None = None
     rechnungsnummer: Annotated[str | None, Field(None, title="Rechnungsnummer")]
     rechnungsperiode: Zeitraum | None = None
     rechnungspositionen: Annotated[list[Rechnungsposition] | None, Field(None, title="Rechnungspositionen")]
     rechnungsstatus: Rechnungsstatus | None = None
     rechnungstitel: Annotated[str | None, Field(None, title="Rechnungstitel")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     .. HINT::
         `Preisblatt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Preisblatt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATT, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_dienstleistung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_dienstleistung.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     .. HINT::
         `PreisblattDienstleistung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/PreisblattDienstleistung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     basisdienstleistung: Dienstleistungstyp | None = None
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bilanzierungsmethode: Bilanzierungsmethode | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATTDIENSTLEISTUNG, alias="boTyp")]
     externe_referenzen: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_hardware.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_hardware.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     .. HINT::
         `PreisblattHardware JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/PreisblattHardware.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     basisgeraet: Geraeteeigenschaften | None = None
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bilanzierungsmethode: Bilanzierungsmethode | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATTHARDWARE, alias="boTyp")]
     externe_referenzen: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_konzessionsabgabe.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_konzessionsabgabe.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
     .. HINT::
         `PreisblattKonzessionsabgabe JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/PreisblattKonzessionsabgabe.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATTKONZESSIONSABGABE, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_messung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_messung.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
     .. HINT::
         `PreisblattMessung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/PreisblattMessung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bilanzierungsmethode: Bilanzierungsmethode | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATTMESSUNG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/preisblatt_netznutzung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/preisblatt_netznutzung.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     .. HINT::
         `PreisblattNetznutzung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/PreisblattNetznutzung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bilanzierungsmethode: Bilanzierungsmethode | None = None
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.PREISBLATTNETZNUTZUNG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/rechnung.py` & `ibims-0.1.9/src/ibims/bo4e/bo/rechnung.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.betrag import Betrag
 from ..com.externe_referenz import ExterneReferenz
 from ..com.rechnungsposition import Rechnungsposition
 from ..com.steuerbetrag import Steuerbetrag
 from ..com.zeitraum import Zeitraum
@@ -23,29 +25,30 @@
 
     .. HINT::
         `Rechnung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Rechnung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.RECHNUNG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
-    faelligkeitsdatum: Annotated[AwareDatetime | None, Field(None, title="Faelligkeitsdatum")]
+    faelligkeitsdatum: Annotated[datetime | None, Field(None, title="Faelligkeitsdatum")]
     gesamtbrutto: Betrag | None = None
     gesamtnetto: Betrag | None = None
     gesamtsteuer: Betrag | None = None
     original_rechnungsnummer: Annotated[
         str | None, Field(None, alias="originalRechnungsnummer", title="Originalrechnungsnummer")
     ]
     rabatt_brutto: Annotated[Betrag | None, Field(None, alias="rabattBrutto")]
-    rechnungsdatum: Annotated[AwareDatetime | None, Field(None, title="Rechnungsdatum")]
+    rechnungsdatum: Annotated[datetime | None, Field(None, title="Rechnungsdatum")]
     rechnungsempfaenger: Geschaeftspartner | None = None
     rechnungsersteller: Geschaeftspartner | None = None
     rechnungsnummer: Annotated[str | None, Field(None, title="Rechnungsnummer")]
     rechnungsperiode: Zeitraum | None = None
     rechnungspositionen: Annotated[list[Rechnungsposition] | None, Field(None, title="Rechnungspositionen")]
     rechnungsstatus: Rechnungsstatus | None = None
     rechnungstitel: Annotated[str | None, Field(None, title="Rechnungstitel")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/region.py` & `ibims-0.1.9/src/ibims/bo4e/bo/region.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     .. HINT::
         `Region JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Region.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.REGION, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/regionaltarif.py` & `ibims-0.1.9/src/ibims/bo4e/bo/regionaltarif.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.energiemix import Energiemix
 from ..com.externe_referenz import ExterneReferenz
 from ..com.regionale_preisgarantie import RegionalePreisgarantie
 from ..com.regionale_tarifpreisposition import RegionaleTarifpreisposition
 from ..com.regionaler_auf_abschlag import RegionalerAufAbschlag
@@ -27,30 +29,31 @@
 
     .. HINT::
         `Regionaltarif JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Regionaltarif.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anbieter: Marktteilnehmer | None = None
     anbietername: Annotated[str | None, Field(None, title="Anbietername")]
-    anwendung_von: Annotated[AwareDatetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
+    anwendung_von: Annotated[datetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     berechnungsparameter: Tarifberechnungsparameter | None = None
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.REGIONALTARIF, alias="boTyp")]
     energiemix: Energiemix | None = None
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     kundentypen: Annotated[list[Kundentyp] | None, Field(None, title="Kundentypen")]
     preisgarantien: Annotated[list[RegionalePreisgarantie] | None, Field(None, title="Preisgarantien")]
-    preisstand: Annotated[AwareDatetime | None, Field(None, title="Preisstand")]
+    preisstand: Annotated[datetime | None, Field(None, title="Preisstand")]
     sparte: Sparte | None = None
     tarif_auf_abschlaege: Annotated[
         list[RegionalerAufAbschlag] | None, Field(None, alias="tarifAufAbschlaege", title="Tarifaufabschlaege")
     ]
     tarifart: Tarifart | None = None
     tarifeinschraenkung: Tarifeinschraenkung | None = None
     tarifmerkmale: Annotated[list[Tarifmerkmal] | None, Field(None, title="Tarifmerkmale")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/standorteigenschaften.py` & `ibims-0.1.9/src/ibims/bo4e/bo/standorteigenschaften.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     .. HINT::
         `Standorteigenschaften JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Standorteigenschaften.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.STANDORTEIGENSCHAFTEN, alias="boTyp")]
     eigenschaften_gas: Annotated[StandorteigenschaftenGas | None, Field(None, alias="eigenschaftenGas")]
     eigenschaften_strom: Annotated[
         list[StandorteigenschaftenStrom] | None, Field(None, alias="eigenschaftenStrom", title="Eigenschaftenstrom")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/tarif.py` & `ibims-0.1.9/src/ibims/bo4e/bo/tarif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.auf_abschlag_regional import AufAbschlagRegional
 from ..com.energiemix import Energiemix
 from ..com.externe_referenz import ExterneReferenz
 from ..com.preisgarantie import Preisgarantie
 from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
@@ -29,30 +31,31 @@
 
     .. HINT::
         `Tarif JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Tarif.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anbieter: Marktteilnehmer | None = None
     anbietername: Annotated[str | None, Field(None, title="Anbietername")]
-    anwendung_von: Annotated[AwareDatetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
+    anwendung_von: Annotated[datetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     berechnungsparameter: Tarifberechnungsparameter | None = None
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.TARIF, alias="boTyp")]
     energiemix: Energiemix | None = None
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     kundentypen: Annotated[list[Kundentyp] | None, Field(None, title="Kundentypen")]
     preisgarantie: Preisgarantie | None = None
-    preisstand: Annotated[AwareDatetime | None, Field(None, title="Preisstand")]
+    preisstand: Annotated[datetime | None, Field(None, title="Preisstand")]
     sparte: Sparte | None = None
     tarif_auf_abschlaege: Annotated[
         list[AufAbschlagRegional] | None, Field(None, alias="tarifAufAbschlaege", title="Tarifaufabschlaege")
     ]
     tarifart: Tarifart | None = None
     tarifeinschraenkung: Tarifeinschraenkung | None = None
     tarifmerkmale: Annotated[list[Tarifmerkmal] | None, Field(None, title="Tarifmerkmale")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/tarifinfo.py` & `ibims-0.1.9/src/ibims/bo4e/bo/tarifinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.energiemix import Energiemix
 from ..com.externe_referenz import ExterneReferenz
 from ..com.vertragskonditionen import Vertragskonditionen
 from ..com.zeitraum import Zeitraum
 from ..enum.bo_typ import BoTyp
@@ -25,19 +27,20 @@
 
     .. HINT::
         `Tarifinfo JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Tarifinfo.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anbieter: Marktteilnehmer | None = None
     anbietername: Annotated[str | None, Field(None, title="Anbietername")]
-    anwendung_von: Annotated[AwareDatetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
+    anwendung_von: Annotated[datetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.TARIFINFO, alias="boTyp")]
     energiemix: Energiemix | None = None
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/tarifkosten.py` & `ibims-0.1.9/src/ibims/bo4e/bo/tarifkosten.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.energiemix import Energiemix
 from ..com.externe_referenz import ExterneReferenz
 from ..com.vertragskonditionen import Vertragskonditionen
 from ..com.zeitraum import Zeitraum
 from ..enum.bo_typ import BoTyp
@@ -25,19 +27,20 @@
 
     .. HINT::
         `Tarifkosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Tarifkosten.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anbieter: Marktteilnehmer | None = None
     anbietername: Annotated[str | None, Field(None, title="Anbietername")]
-    anwendung_von: Annotated[AwareDatetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
+    anwendung_von: Annotated[datetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.TARIFKOSTEN, alias="boTyp")]
     energiemix: Energiemix | None = None
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/tarifpreisblatt.py` & `ibims-0.1.9/src/ibims/bo4e/bo/tarifpreisblatt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.auf_abschlag import AufAbschlag
 from ..com.energiemix import Energiemix
 from ..com.externe_referenz import ExterneReferenz
 from ..com.preisgarantie import Preisgarantie
 from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
@@ -29,30 +31,31 @@
 
     .. HINT::
         `Tarifpreisblatt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Tarifpreisblatt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anbieter: Marktteilnehmer | None = None
     anbietername: Annotated[str | None, Field(None, title="Anbietername")]
-    anwendung_von: Annotated[AwareDatetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
+    anwendung_von: Annotated[datetime | None, Field(None, alias="anwendungVon", title="Anwendungvon")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     berechnungsparameter: Tarifberechnungsparameter | None = None
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.TARIFPREISBLATT, alias="boTyp")]
     energiemix: Energiemix | None = None
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     kundentypen: Annotated[list[Kundentyp] | None, Field(None, title="Kundentypen")]
     preisgarantie: Preisgarantie | None = None
-    preisstand: Annotated[AwareDatetime | None, Field(None, title="Preisstand")]
+    preisstand: Annotated[datetime | None, Field(None, title="Preisstand")]
     sparte: Sparte | None = None
     tarif_auf_abschlaege: Annotated[
         list[AufAbschlag] | None, Field(None, alias="tarifAufAbschlaege", title="Tarifaufabschlaege")
     ]
     tarifart: Tarifart | None = None
     tarifeinschraenkung: Tarifeinschraenkung | None = None
     tarifmerkmale: Annotated[list[Tarifmerkmal] | None, Field(None, title="Tarifmerkmale")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/vertrag.py` & `ibims-0.1.9/src/ibims/bo4e/bo/vertrag.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..com.unterschrift import Unterschrift
 from ..com.vertragskonditionen import Vertragskonditionen
 from ..com.vertragsteil import Vertragsteil
 from ..enum.bo_typ import BoTyp
@@ -23,27 +25,28 @@
 
     .. HINT::
         `Vertrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Vertrag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.VERTRAG, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     sparte: Sparte | None = None
     unterzeichnervp1: Annotated[list[Unterschrift] | None, Field(None, title="Unterzeichnervp1")]
     unterzeichnervp2: Annotated[list[Unterschrift] | None, Field(None, title="Unterzeichnervp2")]
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     vertragsart: Vertragsart | None = None
-    vertragsbeginn: Annotated[AwareDatetime | None, Field(None, title="Vertragsbeginn")]
-    vertragsende: Annotated[AwareDatetime | None, Field(None, title="Vertragsende")]
+    vertragsbeginn: Annotated[datetime | None, Field(None, title="Vertragsbeginn")]
+    vertragsende: Annotated[datetime | None, Field(None, title="Vertragsende")]
     vertragskonditionen: Vertragskonditionen | None = None
     vertragsnummer: Annotated[str | None, Field(None, title="Vertragsnummer")]
     vertragspartner1: Geschaeftspartner | None = None
     vertragspartner2: Geschaeftspartner | None = None
     vertragsstatus: Vertragsstatus | None = None
     vertragsteile: Annotated[list[Vertragsteil] | None, Field(None, title="Vertragsteile")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/zaehler.py` & `ibims-0.1.9/src/ibims/bo4e/bo/zaehler.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..com.zaehlwerk import Zaehlwerk
 from ..com.zeitraum import Zeitraum
 from ..enum.bo_typ import BoTyp
 from ..enum.messwerterfassung import Messwerterfassung
@@ -23,29 +25,30 @@
 
     .. HINT::
         `Zaehler JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Zaehler.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ZAEHLER, alias="boTyp")]
-    eichung_bis: Annotated[AwareDatetime | None, Field(None, alias="eichungBis", title="Eichungbis")]
+    eichung_bis: Annotated[datetime | None, Field(None, alias="eichungBis", title="Eichungbis")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
-    letzte_eichung: Annotated[AwareDatetime | None, Field(None, alias="letzteEichung", title="Letzteeichung")]
+    letzte_eichung: Annotated[datetime | None, Field(None, alias="letzteEichung", title="Letzteeichung")]
     sparte: Sparte | None = None
     tarifart: Tarifart | None = None
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     zaehlerauspraegung: Zaehlerauspraegung | None = None
     zaehlerhersteller: Geschaeftspartner | None = None
     zaehlerkonstante: Annotated[float | str | None, Field(None, title="Zaehlerkonstante")]
     zaehlernummer: Annotated[str | None, Field(None, title="Zaehlernummer")]
     zaehlertyp: Zaehlertyp | None = None
     zaehlwerke: Annotated[list[Zaehlwerk] | None, Field(None, title="Zaehlwerke")]
     messwerterfassung: Messwerterfassung
     nachstes_ablesedatum: Annotated[
-        AwareDatetime | None, Field(None, alias="nachstesAblesedatum", title="Nachstesablesedatum")
+        datetime | None, Field(None, alias="nachstesAblesedatum", title="Nachstesablesedatum")
     ]
     aktiver_zeitraum: Annotated[Zeitraum | None, Field(None, alias="aktiverZeitraum")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/zaehler_gas.py` & `ibims-0.1.9/src/ibims/bo4e/bo/zaehler_gas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..com.externe_referenz import ExterneReferenz
 from ..com.zaehlwerk import Zaehlwerk
 from ..com.zeitraum import Zeitraum
 from ..enum.bo_typ import BoTyp
 from ..enum.geraetemerkmal import Geraetemerkmal
@@ -18,31 +20,32 @@
 class ZaehlerGas(BaseModel):
     """
     Resolve some ambiguity of `Strom` and `Gas`
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     versionstruktur: Annotated[str | None, Field("2", title="Versionstruktur")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ZAEHLER, alias="boTyp")]
     externe_referenzen: Annotated[
         list[ExterneReferenz] | None, Field(None, alias="externeReferenzen", title="Externereferenzen")
     ]
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     zaehlernummer: Annotated[str | None, Field(None, title="Zaehlernummer")]
     sparte: Sparte | None = None
     zaehlerauspraegung: Zaehlerauspraegung | None = None
     zaehlertyp: Zaehlertyp
     zaehlwerke: Annotated[list[Zaehlwerk] | None, Field(None, title="Zaehlwerke")]
     tarifart: Tarifart | None = None
     zaehlerkonstante: Annotated[float | str | None, Field(None, title="Zaehlerkonstante")]
-    eichung_bis: Annotated[AwareDatetime | None, Field(None, alias="eichungBis", title="Eichungbis")]
-    letzte_eichung: Annotated[AwareDatetime | None, Field(None, alias="letzteEichung", title="Letzteeichung")]
+    eichung_bis: Annotated[datetime | None, Field(None, alias="eichungBis", title="Eichungbis")]
+    letzte_eichung: Annotated[datetime | None, Field(None, alias="letzteEichung", title="Letzteeichung")]
     zaehlerhersteller: Geschaeftspartner | None = None
     messwerterfassung: Messwerterfassung
     nachstes_ablesedatum: Annotated[
-        AwareDatetime | None, Field(None, alias="nachstesAblesedatum", title="Nachstesablesedatum")
+        datetime | None, Field(None, alias="nachstesAblesedatum", title="Nachstesablesedatum")
     ]
     aktiver_zeitraum: Annotated[Zeitraum | None, Field(None, alias="aktiverZeitraum")]
     zaehlergroesse: Geraetemerkmal
     druckniveau: Netzebene
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/bo/zeitreihe.py` & `ibims-0.1.9/src/ibims/bo4e/bo/zeitreihe.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     .. HINT::
         `Zeitreihe JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Zeitreihe.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     bo_typ: Annotated[BoTyp | None, Field(BoTyp.ZEITREIHE, alias="boTyp")]
     einheit: Mengeneinheit | None = None
     externe_referenzen: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/adresse.py` & `ibims-0.1.9/src/ibims/bo4e/com/adresse.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     .. HINT::
         `Adresse JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Adresse.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     adresszusatz: Annotated[str | None, Field(None, title="Adresszusatz")]
     co_ergaenzung: Annotated[str | None, Field(None, alias="coErgaenzung", title="Coergaenzung")]
     hausnummer: Annotated[str | None, Field(None, title="Hausnummer")]
     landescode: Landescode | None = Landescode.DE
     ort: Annotated[str | None, Field(None, title="Ort")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/angebotsposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/angebotsposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,13 +20,14 @@
 
     .. HINT::
         `Angebotsposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Angebotsposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     positionsbezeichnung: Annotated[str | None, Field(None, title="Positionsbezeichnung")]
     positionskosten: Betrag | None = None
     positionsmenge: Menge | None = None
     positionspreis: Preis | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/angebotsteil.py` & `ibims-0.1.9/src/ibims/bo4e/com/angebotsteil.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     .. HINT::
         `Angebotsteil JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Angebotsteil.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anfrage_subreferenz: Annotated[str | None, Field(None, alias="anfrageSubreferenz", title="Anfragesubreferenz")]
     gesamtkostenangebotsteil: Betrag | None = None
     gesamtmengeangebotsteil: Menge | None = None
     lieferstellenangebotsteil: Annotated[list[Marktlokation] | None, Field(None, title="Lieferstellenangebotsteil")]
     lieferzeitraum: Zeitraum | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/angebotsvariante.py` & `ibims-0.1.9/src/ibims/bo4e/com/angebotsvariante.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.angebotsstatus import Angebotsstatus
 from .angebotsteil import Angebotsteil
 from .betrag import Betrag
 from .menge import Menge
 
@@ -17,15 +19,16 @@
 
     .. HINT::
         `Angebotsvariante JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Angebotsvariante.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     angebotsstatus: Angebotsstatus | None = None
-    bindefrist: Annotated[AwareDatetime | None, Field(None, title="Bindefrist")]
-    erstellungsdatum: Annotated[AwareDatetime | None, Field(None, title="Erstellungsdatum")]
+    bindefrist: Annotated[datetime | None, Field(None, title="Bindefrist")]
+    erstellungsdatum: Annotated[datetime | None, Field(None, title="Erstellungsdatum")]
     gesamtkosten: Betrag | None = None
     gesamtmenge: Menge | None = None
     teile: Annotated[list[Angebotsteil] | None, Field(None, title="Teile")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag.py` & `ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     .. HINT::
         `AufAbschlag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/AufAbschlag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     auf_abschlagstyp: Annotated[AufAbschlagstyp | None, Field(None, alias="aufAbschlagstyp")]
     auf_abschlagsziel: Annotated[AufAbschlagsziel | None, Field(None, alias="aufAbschlagsziel")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     einheit: Waehrungseinheit | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag_pro_ort.py` & `ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag_pro_ort.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 
     .. HINT::
         `AufAbschlagProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/AufAbschlagProOrt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     netznr: Annotated[str | None, Field(None, title="Netznr")]
     ort: Annotated[str | None, Field(None, title="Ort")]
     postleitzahl: Annotated[str | None, Field(None, title="Postleitzahl")]
     staffeln: Annotated[list[AufAbschlagstaffelProOrt] | None, Field(None, title="Staffeln")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/auf_abschlag_regional.py` & `ibims-0.1.9/src/ibims/bo4e/com/auf_abschlag_regional.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     .. HINT::
         `AufAbschlagRegional JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/AufAbschlagRegional.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     auf_abschlagstyp: Annotated[AufAbschlagstyp | None, Field(None, alias="aufAbschlagstyp")]
     auf_abschlagsziel: Annotated[AufAbschlagsziel | None, Field(None, alias="aufAbschlagsziel")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     betraege: Annotated[list[AufAbschlagProOrt] | None, Field(None, title="Betraege")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/auf_abschlagstaffel_pro_ort.py` & `ibims-0.1.9/src/ibims/bo4e/com/auf_abschlagstaffel_pro_ort.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 
     .. HINT::
         `AufAbschlagstaffelProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/AufAbschlagstaffelProOrt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     staffelgrenze_bis: Annotated[float | str | None, Field(None, alias="staffelgrenzeBis", title="Staffelgrenzebis")]
     staffelgrenze_von: Annotated[float | str | None, Field(None, alias="staffelgrenzeVon", title="Staffelgrenzevon")]
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/ausschreibungsdetail.py` & `ibims-0.1.9/src/ibims/bo4e/com/ausschreibungsdetail.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     .. HINT::
         `Ausschreibungsdetail JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Ausschreibungsdetail.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     kunde: Annotated[str | None, Field(None, title="Kunde")]
     lastgang_vorhanden: Annotated[bool | None, Field(None, alias="lastgangVorhanden", title="Lastgangvorhanden")]
     lieferzeitraum: Zeitraum | None = None
     marktlokations_id: Annotated[str | None, Field(None, alias="marktlokationsId", title="Marktlokationsid")]
     marktlokationsadresse: Adresse | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/ausschreibungslos.py` & `ibims-0.1.9/src/ibims/bo4e/com/ausschreibungslos.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     .. HINT::
         `Ausschreibungslos JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Ausschreibungslos.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anzahl_lieferstellen: Annotated[int | None, Field(None, alias="anzahlLieferstellen", title="Anzahllieferstellen")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     betreut_durch: Annotated[str | None, Field(None, alias="betreutDurch", title="Betreutdurch")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     energieart: Sparte | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/bankverbindung.py` & `ibims-0.1.9/src/ibims/bo4e/com/bankverbindung.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from .sepa_info import SepaInfo
 
 
 class Bankverbindung(BaseModel):
     """
     This component contains bank connection information.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     iban: Annotated[str | None, Field(None, title="Iban")]
     bic: Annotated[str | None, Field(None, title="Bic")]
-    gueltig_seit: Annotated[AwareDatetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
-    gueltig_bis: Annotated[AwareDatetime | None, Field(None, alias="gueltigBis", title="Gueltigbis")]
+    gueltig_seit: Annotated[datetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
+    gueltig_bis: Annotated[datetime | None, Field(None, alias="gueltigBis", title="Gueltigbis")]
     bankname: Annotated[str | None, Field(None, title="Bankname")]
     sepa_info: Annotated[SepaInfo | None, Field(None, alias="sepaInfo")]
     kontoinhaber: Annotated[str | None, Field(None, title="Kontoinhaber")]
     ouid: Annotated[int, Field(title="Ouid")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/betrag.py` & `ibims-0.1.9/src/ibims/bo4e/com/betrag.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 
     .. HINT::
         `Betrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Betrag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     waehrung: Waehrungscode | None = None
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/com.py` & `ibims-0.1.9/src/ibims/bo4e/com/com.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 
     .. HINT::
         `COM JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/COM.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/dienstleistung.py` & `ibims-0.1.9/src/ibims/bo4e/com/dienstleistung.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `Dienstleistung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Dienstleistung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     dienstleistungstyp: Dienstleistungstyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/energieherkunft.py` & `ibims-0.1.9/src/ibims/bo4e/com/energieherkunft.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `Energieherkunft JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Energieherkunft.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anteil_prozent: Annotated[float | str | None, Field(None, alias="anteilProzent", title="Anteilprozent")]
     erzeugungsart: Erzeugungsart | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/energiemix.py` & `ibims-0.1.9/src/ibims/bo4e/com/energiemix.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     .. HINT::
         `Energiemix JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Energiemix.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     anteil: Annotated[list[Energieherkunft] | None, Field(None, title="Anteil")]
     atommuell: Annotated[float | str | None, Field(None, title="Atommuell")]
     bemerkung: Annotated[str | None, Field(None, title="Bemerkung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     co2_emission: Annotated[float | str | None, Field(None, alias="co2Emission", title="Co2Emission")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/externe_referenz.py` & `ibims-0.1.9/src/ibims/bo4e/com/externe_referenz.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `ExterneReferenz JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/ExterneReferenz.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     ex_ref_name: Annotated[str | None, Field(None, alias="exRefName", title="Exrefname")]
     ex_ref_wert: Annotated[str | None, Field(None, alias="exRefWert", title="Exrefwert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/fremdkostenblock.py` & `ibims-0.1.9/src/ibims/bo4e/com/fremdkostenblock.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 
     .. HINT::
         `Fremdkostenblock JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Fremdkostenblock.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     kostenblockbezeichnung: Annotated[str | None, Field(None, title="Kostenblockbezeichnung")]
     kostenpositionen: Annotated[list[Fremdkostenposition] | None, Field(None, title="Kostenpositionen")]
     summe_kostenblock: Annotated[Betrag | None, Field(None, alias="summeKostenblock")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/fremdkostenposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/fremdkostenposition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from .betrag import Betrag
 from .menge import Menge
 from .preis import Preis
 
 
@@ -16,22 +18,23 @@
 
     .. HINT::
         `Fremdkostenposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Fremdkostenposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     artikelbezeichnung: Annotated[str | None, Field(None, title="Artikelbezeichnung")]
     artikeldetail: Annotated[str | None, Field(None, title="Artikeldetail")]
     betrag_kostenposition: Annotated[Betrag | None, Field(None, alias="betragKostenposition")]
-    bis: Annotated[AwareDatetime | None, Field(None, title="Bis")]
+    bis: Annotated[datetime | None, Field(None, title="Bis")]
     einzelpreis: Preis | None = None
     gebietcode_eic: Annotated[str | None, Field(None, alias="gebietcodeEic", title="Gebietcodeeic")]
     link_preisblatt: Annotated[str | None, Field(None, alias="linkPreisblatt", title="Linkpreisblatt")]
     marktpartnercode: Annotated[str | None, Field(None, title="Marktpartnercode")]
     marktpartnername: Annotated[str | None, Field(None, title="Marktpartnername")]
     menge: Menge | None = None
     positionstitel: Annotated[str | None, Field(None, title="Positionstitel")]
-    von: Annotated[AwareDatetime | None, Field(None, title="Von")]
+    von: Annotated[datetime | None, Field(None, title="Von")]
     zeitmenge: Menge | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/geokoordinaten.py` & `ibims-0.1.9/src/ibims/bo4e/com/unterschrift.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+from datetime import datetime
+
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 
-class Geokoordinaten(BaseModel):
+class Unterschrift(BaseModel):
     """
-    This component provides the geo-coordinates for a location.
+    Modellierung einer Unterschrift, z.B. für Verträge, Angebote etc.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/Geokoordinaten.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/Unterschrift.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Geokoordinaten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Geokoordinaten.json>`_
+        `Unterschrift JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Unterschrift.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    breitengrad: Annotated[float | str | None, Field(None, title="Breitengrad")]
-    laengengrad: Annotated[float | str | None, Field(None, title="Laengengrad")]
+    datum: Annotated[datetime | None, Field(None, title="Datum")]
+    name: Annotated[str | None, Field(None, title="Name")]
+    ort: Annotated[str | None, Field(None, title="Ort")]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/geraet.py` & `ibims-0.1.9/src/ibims/bo4e/com/geraeteeigenschaften.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
-from .geraeteeigenschaften import Geraeteeigenschaften
+from ..enum.geraetemerkmal import Geraetemerkmal
+from ..enum.geraetetyp import Geraetetyp
 
 
-class Geraet(BaseModel):
+class Geraeteeigenschaften(BaseModel):
     """
-    Mit dieser Komponente werden alle Geräte modelliert, die keine Zähler sind.
+    Mit dieser Komponente werden die Eigenschaften eines Gerätes in Bezug auf den Typ und weitere Merkmale modelliert
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/Geraet.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/Geraeteeigenschaften.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Geraet JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Geraet.json>`_
+        `Geraeteeigenschaften JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Geraeteeigenschaften.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    geraeteeigenschaften: Geraeteeigenschaften | None = None
-    geraetenummer: Annotated[str | None, Field(None, title="Geraetenummer")]
+    geraetemerkmal: Geraetemerkmal | None = None
+    geraetetyp: Geraetetyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/hardware.py` & `ibims-0.1.9/src/ibims/bo4e/com/hardware.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `Hardware JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Hardware.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     geraetetyp: Geraetetyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/katasteradresse.py` & `ibims-0.1.9/src/ibims/bo4e/com/katasteradresse.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 
     .. HINT::
         `Katasteradresse JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Katasteradresse.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     flurstueck: Annotated[str | None, Field(None, title="Flurstueck")]
     gemarkung_flur: Annotated[str | None, Field(None, alias="gemarkungFlur", title="Gemarkungflur")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/kostenblock.py` & `ibims-0.1.9/src/ibims/bo4e/com/kostenblock.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 
     .. HINT::
         `Kostenblock JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Kostenblock.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     kostenblockbezeichnung: Annotated[str | None, Field(None, title="Kostenblockbezeichnung")]
     kostenpositionen: Annotated[list[Kostenposition] | None, Field(None, title="Kostenpositionen")]
     summe_kostenblock: Annotated[Betrag | None, Field(None, alias="summeKostenblock")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/kostenposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/kostenposition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from .betrag import Betrag
 from .menge import Menge
 from .preis import Preis
 
 
@@ -16,18 +18,19 @@
 
     .. HINT::
         `Kostenposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Kostenposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     artikelbezeichnung: Annotated[str | None, Field(None, title="Artikelbezeichnung")]
     artikeldetail: Annotated[str | None, Field(None, title="Artikeldetail")]
     betrag_kostenposition: Annotated[Betrag | None, Field(None, alias="betragKostenposition")]
-    bis: Annotated[AwareDatetime | None, Field(None, title="Bis")]
+    bis: Annotated[datetime | None, Field(None, title="Bis")]
     einzelpreis: Preis | None = None
     menge: Menge | None = None
     positionstitel: Annotated[str | None, Field(None, title="Positionstitel")]
-    von: Annotated[AwareDatetime | None, Field(None, title="Von")]
+    von: Annotated[datetime | None, Field(None, title="Von")]
     zeitmenge: Menge | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/kriterium_wert.py` & `ibims-0.1.9/src/ibims/bo4e/com/kriterium_wert.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `KriteriumWert JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/KriteriumWert.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     kriterium: Tarifregionskriterium | None = None
     wert: Annotated[str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/lastprofil.py` & `ibims-0.1.9/src/ibims/bo4e/com/lastprofil.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,12 +10,13 @@
     https://github.com/Hochfrequenz/BO4E-dotnet/blob/9bdc151170ddba5c9d7535e863d5a396fe7fec52/BO4E/COM/Lastprofil.cs
     https://github.com/Hochfrequenz/go-bo4e/blob/708b39de0dcea8a9448ed4e7341a2687f6bf7c11/com/lastprofil.go
     Fields, which are not needed for migrations, are omitted and the field "profilart" is modelled as Profiltyp ENUM.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     einspeisung: Annotated[bool | None, Field(False, title="Einspeisung")]
     profilart: Profiltyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/marktgebiet_info.py` & `ibims-0.1.9/src/ibims/bo4e/com/marktgebiet_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 
     .. HINT::
         `MarktgebietInfo JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/MarktgebietInfo.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     marktgebiet: Annotated[str | None, Field(None, title="Marktgebiet")]
     marktgebietcode: Annotated[str | None, Field(None, title="Marktgebietcode")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/menge.py` & `ibims-0.1.9/src/ibims/bo4e/com/menge.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `Menge JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Menge.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     einheit: Mengeneinheit | None = None
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/messlokationszuordnung.py` & `ibims-0.1.9/src/ibims/bo4e/com/messlokationszuordnung.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.arithmetische_operation import ArithmetischeOperation
 
 
 class Messlokationszuordnung(BaseModel):
     """
@@ -16,13 +18,14 @@
 
     .. HINT::
         `Messlokationszuordnung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Messlokationszuordnung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     arithmetik: ArithmetischeOperation | None = None
-    gueltig_bis: Annotated[AwareDatetime | None, Field(None, alias="gueltigBis", title="Gueltigbis")]
-    gueltig_seit: Annotated[AwareDatetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
+    gueltig_bis: Annotated[datetime | None, Field(None, alias="gueltigBis", title="Gueltigbis")]
+    gueltig_seit: Annotated[datetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
     messlokations_id: Annotated[str | None, Field(None, alias="messlokationsId", title="Messlokationsid")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/positions_auf_abschlag.py` & `ibims-0.1.9/src/ibims/bo4e/com/positions_auf_abschlag.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
     .. HINT::
         `PositionsAufAbschlag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/PositionsAufAbschlag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     auf_abschlagstyp: Annotated[AufAbschlagstyp | None, Field(None, alias="aufAbschlagstyp")]
     auf_abschlagswaehrung: Annotated[Waehrungseinheit | None, Field(None, alias="aufAbschlagswaehrung")]
     auf_abschlagswert: Annotated[float | str | None, Field(None, alias="aufAbschlagswert", title="Aufabschlagswert")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/preis.py` & `ibims-0.1.9/src/ibims/bo4e/com/preis.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 
     .. HINT::
         `Preis JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Preis.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezugswert: Mengeneinheit | None = None
     einheit: Waehrungseinheit | None = None
     status: Preisstatus | None = None
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/preisgarantie.py` & `ibims-0.1.9/src/ibims/bo4e/com/preisgarantie.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.preisgarantietyp import Preisgarantietyp
 from .zeitraum import Zeitraum
 
 
 class Preisgarantie(BaseModel):
@@ -15,13 +17,14 @@
 
     .. HINT::
         `Preisgarantie JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Preisgarantie.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     preisgarantietyp: Preisgarantietyp | None = None
     zeitliche_gueltigkeit: Annotated[Zeitraum | None, Field(None, alias="zeitlicheGueltigkeit")]
-    creation_date: Annotated[AwareDatetime | None, Field(None, alias="creationDate", title="Creationdate")]
+    creation_date: Annotated[datetime | None, Field(None, alias="creationDate", title="Creationdate")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/preisposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/preisposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     .. HINT::
         `Preisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Preisposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bdew_artikelnummer: Annotated[BDEWArtikelnummer | None, Field(None, alias="bdewArtikelnummer")]
     berechnungsmethode: Kalkulationsmethode | None = None
     bezugsgroesse: Mengeneinheit | None = None
     freimenge_blindarbeit: Annotated[
         float | str | None, Field(None, alias="freimengeBlindarbeit", title="Freimengeblindarbeit")
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/preisstaffel.py` & `ibims-0.1.9/src/ibims/bo4e/com/preisstaffel.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 
     .. HINT::
         `Preisstaffel JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Preisstaffel.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     einheitspreis: Annotated[float | str | None, Field(None, title="Einheitspreis")]
     sigmoidparameter: Sigmoidparameter | None = None
     staffelgrenze_bis: Annotated[float | str | None, Field(None, alias="staffelgrenzeBis", title="Staffelgrenzebis")]
     staffelgrenze_von: Annotated[float | str | None, Field(None, alias="staffelgrenzeVon", title="Staffelgrenzevon")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/rechnungsposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/rechnungsposition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.bdew_artikelnummer import BDEWArtikelnummer
 from ..enum.zeiteinheit import Zeiteinheit
 from .betrag import Betrag
 from .menge import Menge
 from .preis import Preis
@@ -20,21 +22,22 @@
 
     .. HINT::
         `Rechnungsposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Rechnungsposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     artikel_id: Annotated[str | None, Field(None, alias="artikelId", title="Artikelid")]
     artikelnummer: BDEWArtikelnummer | None = None
     einzelpreis: Preis | None = None
-    lieferung_bis: Annotated[AwareDatetime | None, Field(None, alias="lieferungBis", title="Lieferungbis")]
-    lieferung_von: Annotated[AwareDatetime | None, Field(None, alias="lieferungVon", title="Lieferungvon")]
+    lieferung_bis: Annotated[datetime | None, Field(None, alias="lieferungBis", title="Lieferungbis")]
+    lieferung_von: Annotated[datetime | None, Field(None, alias="lieferungVon", title="Lieferungvon")]
     lokations_id: Annotated[str | None, Field(None, alias="lokationsId", title="Lokationsid")]
     positions_menge: Annotated[Menge | None, Field(None, alias="positionsMenge")]
     positionsnummer: Annotated[int | None, Field(None, title="Positionsnummer")]
     positionstext: Annotated[str | None, Field(None, title="Positionstext")]
     teilrabatt_netto: Annotated[Betrag | None, Field(None, alias="teilrabattNetto")]
     teilsumme_netto: Annotated[Betrag | None, Field(None, alias="teilsummeNetto")]
     teilsumme_steuer: Annotated[Steuerbetrag | None, Field(None, alias="teilsummeSteuer")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionale_gueltigkeit.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionale_gueltigkeit.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,13 +15,14 @@
 
     .. HINT::
         `RegionaleGueltigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionaleGueltigkeit.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     gueltigkeitstyp: Gueltigkeitstyp | None = None
     kriteriums_werte: Annotated[
         list[KriteriumWert] | None, Field(None, alias="kriteriumsWerte", title="Kriteriumswerte")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionale_preisgarantie.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionale_preisgarantie.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 
     .. HINT::
         `RegionalePreisgarantie JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionalePreisgarantie.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     preisgarantietyp: Preisgarantietyp | None = None
     regionale_gueltigkeit: Annotated[RegionaleGueltigkeit | None, Field(None, alias="regionaleGueltigkeit")]
     zeitliche_gueltigkeit: Annotated[Zeitraum | None, Field(None, alias="zeitlicheGueltigkeit")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionale_preisstaffel.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionale_preisstaffel.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     .. HINT::
         `RegionalePreisstaffel JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionalePreisstaffel.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     einheitspreis: Annotated[float | str | None, Field(None, title="Einheitspreis")]
     regionale_gueltigkeit: Annotated[RegionaleGueltigkeit | None, Field(None, alias="regionaleGueltigkeit")]
     sigmoidparameter: Sigmoidparameter | None = None
     staffelgrenze_bis: Annotated[float | str | None, Field(None, alias="staffelgrenzeBis", title="Staffelgrenzebis")]
     staffelgrenze_von: Annotated[float | str | None, Field(None, alias="staffelgrenzeVon", title="Staffelgrenzevon")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionale_tarifpreisposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifpreisposition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.mengeneinheit import Mengeneinheit
 from ..enum.preistyp import Preistyp
 from ..enum.waehrungseinheit import Waehrungseinheit
-from .regionale_preisstaffel import RegionalePreisstaffel
+from .preisstaffel import Preisstaffel
 
 
-class RegionaleTarifpreisposition(BaseModel):
+class Tarifpreisposition(BaseModel):
     """
-    Mit dieser Komponente können Tarifpreise verschiedener Typen im Zusammenhang mit regionalen Gültigkeiten abgebildet
-    werden.
+    Mit dieser Komponente können Tarifpreise verschiedener Typen abgebildet werden.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/RegionaleTarifpreisposition.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/Tarifpreisposition.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `RegionaleTarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionaleTarifpreisposition.json>`_
+        `Tarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tarifpreisposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezugseinheit: Mengeneinheit | None = None
     einheit: Waehrungseinheit | None = None
     mengeneinheitstaffel: Mengeneinheit | None = None
-    preisstaffeln: Annotated[list[RegionalePreisstaffel] | None, Field(None, title="Preisstaffeln")]
+    preisstaffeln: Annotated[list[Preisstaffel] | None, Field(None, title="Preisstaffeln")]
     preistyp: Preistyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionaler_auf_abschlag.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionaler_auf_abschlag.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
     .. HINT::
         `RegionalerAufAbschlag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionalerAufAbschlag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     auf_abschlagstyp: Annotated[AufAbschlagstyp | None, Field(None, alias="aufAbschlagstyp")]
     auf_abschlagsziel: Annotated[AufAbschlagsziel | None, Field(None, alias="aufAbschlagsziel")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     einheit: Waehrungseinheit | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/regionskriterium.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionskriterium.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 
     .. HINT::
         `Regionskriterium JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Regionskriterium.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     gueltigkeitstyp: Gueltigkeitstyp | None = None
     regionskriteriumtyp: Regionskriteriumtyp | None = None
     wert: Annotated[str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/rufnummer.py` & `ibims-0.1.9/src/ibims/bo4e/com/rufnummer.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `Rufnummer JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Rufnummer.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     nummerntyp: Rufnummernart | None = None
     rufnummer: Annotated[str | None, Field(None, title="Rufnummer")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/sepa_info.py` & `ibims-0.1.9/src/ibims/bo4e/com/sepa_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 
 class SepaInfo(BaseModel):
     """
     This class includes details about the sepa mandates.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     sepa_id: Annotated[str, Field(alias="sepaId", title="Sepaid")]
     sepa_zahler: Annotated[bool, Field(alias="sepaZahler", title="Sepazahler")]
     creditor_identifier: Annotated[str | None, Field(None, alias="creditorIdentifier", title="Creditoridentifier")]
-    gueltig_seit: Annotated[AwareDatetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
+    gueltig_seit: Annotated[datetime | None, Field(None, alias="gueltigSeit", title="Gueltigseit")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/sigmoidparameter.py` & `ibims-0.1.9/src/ibims/bo4e/com/sigmoidparameter.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,13 +13,14 @@
 
     .. HINT::
         `Sigmoidparameter JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Sigmoidparameter.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     a: Annotated[float | str | None, Field(None, alias="A", title="A")]
     b: Annotated[float | str | None, Field(None, alias="B", title="B")]
     c: Annotated[float | str | None, Field(None, alias="C", title="C")]
     d: Annotated[float | str | None, Field(None, alias="D", title="D")]
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/standorteigenschaften_gas.py` & `ibims-0.1.9/src/ibims/bo4e/com/standorteigenschaften_gas.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,11 +14,12 @@
 
     .. HINT::
         `StandorteigenschaftenGas JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/StandorteigenschaftenGas.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     marktgebiete: Annotated[list[MarktgebietInfo] | None, Field(None, title="Marktgebiete")]
     netzkontonummern: Annotated[list[str] | None, Field(None, title="Netzkontonummern")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/standorteigenschaften_strom.py` & `ibims-0.1.9/src/ibims/bo4e/com/standorteigenschaften_strom.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     .. HINT::
         `StandorteigenschaftenStrom JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/StandorteigenschaftenStrom.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bilanzierungsgebiet_eic: Annotated[
         str | None, Field(None, alias="bilanzierungsgebietEic", title="Bilanzierungsgebieteic")
     ]
     regelzone: Annotated[str | None, Field(None, title="Regelzone")]
     regelzone_eic: Annotated[str | None, Field(None, alias="regelzoneEic", title="Regelzoneeic")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/steuerbetrag.py` & `ibims-0.1.9/src/ibims/bo4e/com/steuerbetrag.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     .. HINT::
         `Steuerbetrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Steuerbetrag.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     basiswert: Annotated[float | str | None, Field(None, title="Basiswert")]
     steuerkennzeichen: Steuerkennzeichen | None = None
     steuerwert: Annotated[float | str | None, Field(None, title="Steuerwert")]
     waehrung: Waehrungscode | None = None
     steuerwert_vorausgezahlt: Annotated[
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tagesvektor.py` & `ibims-0.1.9/src/ibims/bo4e/com/tagesvektor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from .zeitreihenwertkompakt import Zeitreihenwertkompakt
 
 
 class Tagesvektor(BaseModel):
     """
@@ -14,11 +16,12 @@
 
     .. HINT::
         `Tagesvektor JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tagesvektor.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    tag: Annotated[AwareDatetime | None, Field(None, title="Tag")]
+    tag: Annotated[datetime | None, Field(None, title="Tag")]
     werte: Annotated[list[Zeitreihenwertkompakt] | None, Field(None, title="Werte")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifberechnungsparameter.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifberechnungsparameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     .. HINT::
         `Tarifberechnungsparameter JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tarifberechnungsparameter.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     berechnungsmethode: Tarifkalkulationsmethode | None = None
     hoechstpreis_ht: Annotated[Preis | None, Field(None, alias="hoechstpreisHT")]
     hoechstpreis_nt: Annotated[Preis | None, Field(None, alias="hoechstpreisNT")]
     kw_inklusive: Annotated[float | str | None, Field(None, alias="kwInklusive", title="Kwinklusive")]
     kw_weitere_mengen: Annotated[float | str | None, Field(None, alias="kwWeitereMengen", title="Kwweiteremengen")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifeinschraenkung.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifeinschraenkung.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,13 +16,14 @@
 
     .. HINT::
         `Tarifeinschraenkung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tarifeinschraenkung.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     einschraenkungleistung: Annotated[list[Menge] | None, Field(None, title="Einschraenkungleistung")]
     einschraenkungzaehler: Annotated[list[Geraet] | None, Field(None, title="Einschraenkungzaehler")]
     voraussetzungen: Annotated[list[Voraussetzungen] | None, Field(None, title="Voraussetzungen")]
     zusatzprodukte: Annotated[list[str] | None, Field(None, title="Zusatzprodukte")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifpreis.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifpreis.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
     .. HINT::
         `Tarifpreis JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tarifpreis.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     bezugswert: Mengeneinheit | None = None
     einheit: Waehrungseinheit | None = None
     preistyp: Preistyp | None = None
     status: Preisstatus | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifpreisposition.py` & `ibims-0.1.9/src/ibims/bo4e/com/regionale_tarifpreisposition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.mengeneinheit import Mengeneinheit
 from ..enum.preistyp import Preistyp
 from ..enum.waehrungseinheit import Waehrungseinheit
-from .preisstaffel import Preisstaffel
+from .regionale_preisstaffel import RegionalePreisstaffel
 
 
-class Tarifpreisposition(BaseModel):
+class RegionaleTarifpreisposition(BaseModel):
     """
-    Mit dieser Komponente können Tarifpreise verschiedener Typen abgebildet werden.
+    Mit dieser Komponente können Tarifpreise verschiedener Typen im Zusammenhang mit regionalen Gültigkeiten abgebildet
+    werden.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/Tarifpreisposition.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/RegionaleTarifpreisposition.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Tarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Tarifpreisposition.json>`_
+        `RegionaleTarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionaleTarifpreisposition.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezugseinheit: Mengeneinheit | None = None
     einheit: Waehrungseinheit | None = None
     mengeneinheitstaffel: Mengeneinheit | None = None
-    preisstaffeln: Annotated[list[Preisstaffel] | None, Field(None, title="Preisstaffeln")]
+    preisstaffeln: Annotated[list[RegionalePreisstaffel] | None, Field(None, title="Preisstaffeln")]
     preistyp: Preistyp | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifpreisposition_pro_ort.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifpreisposition_pro_ort.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,13 +14,14 @@
 
     .. HINT::
         `TarifpreispositionProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/TarifpreispositionProOrt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     netznr: Annotated[str | None, Field(None, title="Netznr")]
     ort: Annotated[str | None, Field(None, title="Ort")]
     postleitzahl: Annotated[str | None, Field(None, title="Postleitzahl")]
     preisstaffeln: Annotated[list[TarifpreisstaffelProOrt] | None, Field(None, title="Preisstaffeln")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/tarifpreisstaffel_pro_ort.py` & `ibims-0.1.9/src/ibims/bo4e/com/tarifpreisstaffel_pro_ort.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
     .. HINT::
         `TarifpreisstaffelProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/TarifpreisstaffelProOrt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     arbeitspreis: Annotated[float | str | None, Field(None, title="Arbeitspreis")]
     arbeitspreis_nt: Annotated[float | str | None, Field(None, alias="arbeitspreisNT", title="Arbeitspreisnt")]
     grundpreis: Annotated[float | str | None, Field(None, title="Grundpreis")]
     staffelgrenze_bis: Annotated[float | str | None, Field(None, alias="staffelgrenzeBis", title="Staffelgrenzebis")]
     staffelgrenze_von: Annotated[float | str | None, Field(None, alias="staffelgrenzeVon", title="Staffelgrenzevon")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/unterschrift.py` & `ibims-0.1.9/src/ibims/bo4e/com/geraet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
+from .geraeteeigenschaften import Geraeteeigenschaften
 
-class Unterschrift(BaseModel):
+
+class Geraet(BaseModel):
     """
-    Modellierung einer Unterschrift, z.B. für Verträge, Angebote etc.
+    Mit dieser Komponente werden alle Geräte modelliert, die keine Zähler sind.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/Unterschrift.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/Geraet.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Unterschrift JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Unterschrift.json>`_
+        `Geraet JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Geraet.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    datum: Annotated[AwareDatetime | None, Field(None, title="Datum")]
-    name: Annotated[str | None, Field(None, title="Name")]
-    ort: Annotated[str | None, Field(None, title="Ort")]
+    geraeteeigenschaften: Geraeteeigenschaften | None = None
+    geraetenummer: Annotated[str | None, Field(None, title="Geraetenummer")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/verbrauch.py` & `ibims-0.1.9/src/ibims/bo4e/com/verbrauch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.ablesende_rolle import AblesendeRolle
 from ..enum.ablesungsstatus import Ablesungsstatus
 from ..enum.mengeneinheit import Mengeneinheit
 from ..enum.messwertstatus import Messwertstatus
 from ..enum.wertermittlungsverfahren import Wertermittlungsverfahren
@@ -18,42 +20,41 @@
 
     .. HINT::
         `Verbrauch JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Verbrauch.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     einheit: Mengeneinheit | None = None
-    enddatum: Annotated[AwareDatetime | None, Field(None, title="Enddatum")]
+    enddatum: Annotated[datetime | None, Field(None, title="Enddatum")]
     obis_kennzahl: Annotated[str | None, Field(None, alias="obisKennzahl", title="Obiskennzahl")]
-    startdatum: Annotated[AwareDatetime | None, Field(None, title="Startdatum")]
+    startdatum: Annotated[datetime | None, Field(None, title="Startdatum")]
     wert: Annotated[float | str | None, Field(None, title="Wert")]
     wertermittlungsverfahren: Wertermittlungsverfahren | None = None
     ablesegrund: Annotated[str | None, Field(None, title="Ablesegrund")]
     ablesebeschreibung: Annotated[str | None, Field(None, title="Ablesebeschreibung")]
     periodenverbrauch: Annotated[float | str | None, Field(None, title="Periodenverbrauch")]
     periodenverbrauch_ursprung: Annotated[
         str | None, Field(None, alias="periodenverbrauchUrsprung", title="Periodenverbrauchursprung")
     ]
     ableser: AblesendeRolle | None = None
     status: Ablesungsstatus | None = None
     energiegehalt_gas: Annotated[float | str | None, Field(None, alias="energiegehaltGas", title="Energiegehaltgas")]
     energiegehalt_gas_gueltig_von: Annotated[
-        AwareDatetime | None, Field(None, alias="energiegehaltGasGueltigVon", title="Energiegehaltgasgueltigvon")
+        datetime | None, Field(None, alias="energiegehaltGasGueltigVon", title="Energiegehaltgasgueltigvon")
     ]
     energiegehalt_gas_gueltig_bis: Annotated[
-        AwareDatetime | None, Field(None, alias="energiegehaltGasGueltigBis", title="Energiegehaltgasgueltigbis")
+        datetime | None, Field(None, alias="energiegehaltGasGueltigBis", title="Energiegehaltgasgueltigbis")
     ]
     umwandlungsfaktor_gas: Annotated[
         float | str | None, Field(None, alias="umwandlungsfaktorGas", title="Umwandlungsfaktorgas")
     ]
     umwandlungsfaktor_gas_gueltig_von: Annotated[
-        AwareDatetime | None,
-        Field(None, alias="umwandlungsfaktorGasGueltigVon", title="Umwandlungsfaktorgasgueltigvon"),
+        datetime | None, Field(None, alias="umwandlungsfaktorGasGueltigVon", title="Umwandlungsfaktorgasgueltigvon")
     ]
     umwandlungsfaktor_gas_gueltig_bis: Annotated[
-        AwareDatetime | None,
-        Field(None, alias="umwandlungsfaktorGasGueltigBis", title="Umwandlungsfaktorgasgueltigbis"),
+        datetime | None, Field(None, alias="umwandlungsfaktorGasGueltigBis", title="Umwandlungsfaktorgasgueltigbis")
     ]
     messwertstatus: Messwertstatus | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/vertragskonditionen.py` & `ibims-0.1.9/src/ibims/bo4e/com/vertragskonditionen.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
     .. HINT::
         `Vertragskonditionen JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Vertragskonditionen.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     abschlagszyklus: Zeitraum | None = None
     anzahl_abschlaege: Annotated[float | str | None, Field(None, alias="anzahlAbschlaege", title="Anzahlabschlaege")]
     beschreibung: Annotated[str | None, Field(None, title="Beschreibung")]
     kuendigungsfrist: Zeitraum | None = None
     vertragslaufzeit: Zeitraum | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/vertragskonto.py` & `ibims-0.1.9/src/ibims/bo4e/com/vertragskonto.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,13 +8,14 @@
 class Vertragskonto(BaseModel):
     """
     Bundle common attributes of MBA and CBA.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     ouid: Annotated[int, Field(title="Ouid")]
     vertrags_adresse: Annotated[Adresse, Field(alias="vertragsAdresse")]
     vertragskontonummer: Annotated[str, Field(title="Vertragskontonummer")]
     rechnungsstellung: Kontaktart
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/vertragskonto_cba.py` & `ibims-0.1.9/src/ibims/bo4e/com/vertragskonto_cba.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..bo.vertrag import Vertrag
 from ..enum.kontaktart import Kontaktart
 from .adresse import Adresse
 
 
@@ -12,19 +14,20 @@
     locks and billing dates. But in the first place, CBAs will be grouped together by the address in their contracts.
     For each group of CBAs with a common address there will be created an MBA (master billing
     account) to support that the invoices for the CBAs can be bundled into a single invoice for the MBA.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     ouid: Annotated[int, Field(title="Ouid")]
     vertrags_adresse: Annotated[Adresse, Field(alias="vertragsAdresse")]
     vertragskontonummer: Annotated[str, Field(title="Vertragskontonummer")]
     rechnungsstellung: Kontaktart
     vertrag: Vertrag
-    erstellungsdatum: Annotated[AwareDatetime, Field(title="Erstellungsdatum")]
-    rechnungsdatum_start: Annotated[AwareDatetime, Field(alias="rechnungsdatumStart", title="Rechnungsdatumstart")]
+    erstellungsdatum: Annotated[datetime, Field(title="Erstellungsdatum")]
+    rechnungsdatum_start: Annotated[datetime, Field(alias="rechnungsdatumStart", title="Rechnungsdatumstart")]
     rechnungsdatum_naechstes: Annotated[
-        AwareDatetime, Field(alias="rechnungsdatumNaechstes", title="Rechnungsdatumnaechstes")
+        datetime, Field(alias="rechnungsdatumNaechstes", title="Rechnungsdatumnaechstes")
     ]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/vertragskonto_mba.py` & `ibims-0.1.9/src/ibims/bo4e/com/vertragskonto_mba.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     Models an MBA (master billing account). Its main purpose is to bundle CBAs together having the same address in
     their related contracts. This feature supports a single invoice for all CBAs instead of several
     invoices for each.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     ouid: Annotated[int, Field(title="Ouid")]
     vertrags_adresse: Annotated[Adresse, Field(alias="vertragsAdresse")]
     vertragskontonummer: Annotated[str, Field(title="Vertragskontonummer")]
     rechnungsstellung: Kontaktart
     cbas: Annotated[list[VertragskontoCBA], Field(title="Cbas")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/vertragsteil.py` & `ibims-0.1.9/src/ibims/bo4e/com/vertragsteil.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from .menge import Menge
 
 
 class Vertragsteil(BaseModel):
     """
@@ -15,15 +17,16 @@
 
     .. HINT::
         `Vertragsteil JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Vertragsteil.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     lokation: Annotated[str | None, Field(None, title="Lokation")]
     maximale_abnahmemenge: Annotated[Menge | None, Field(None, alias="maximaleAbnahmemenge")]
     minimale_abnahmemenge: Annotated[Menge | None, Field(None, alias="minimaleAbnahmemenge")]
     vertraglich_fixierte_menge: Annotated[Menge | None, Field(None, alias="vertraglichFixierteMenge")]
-    vertragsteilbeginn: Annotated[AwareDatetime | None, Field(None, title="Vertragsteilbeginn")]
-    vertragsteilende: Annotated[AwareDatetime | None, Field(None, title="Vertragsteilende")]
+    vertragsteilbeginn: Annotated[datetime | None, Field(None, title="Vertragsteilbeginn")]
+    vertragsteilende: Annotated[datetime | None, Field(None, title="Vertragsteilende")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zaehlpunkt.py` & `ibims-0.1.9/src/ibims/bo4e/com/zaehlpunkt.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     """
     The zaehlpunkt object was created during a migration project.
     It contains attributes needed for metering mapping.
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     periodenverbrauch_vorhersage: Annotated[
         float | str, Field(alias="periodenverbrauchVorhersage", title="Periodenverbrauchvorhersage")
     ]
     einheit_vorhersage: Annotated[Mengeneinheit | None, Field(Mengeneinheit.KWH, alias="einheitVorhersage")]
     zeitreihentyp: Annotated[str | None, Field("Z21", title="Zeitreihentyp")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zaehlwerk.py` & `ibims-0.1.9/src/ibims/bo4e/com/zaehlwerk.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.abgabeart import Abgabeart
 from ..enum.energierichtung import Energierichtung
 from ..enum.mengeneinheit import Mengeneinheit
 
 
@@ -16,23 +18,24 @@
 
     .. HINT::
         `Zaehlwerk JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zaehlwerk.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     bezeichnung: Annotated[str | None, Field(None, title="Bezeichnung")]
     einheit: Mengeneinheit | None = None
     obis_kennzahl: Annotated[str | None, Field(None, alias="obisKennzahl", title="Obiskennzahl")]
     richtung: Energierichtung | None = None
     wandlerfaktor: Annotated[float | str | None, Field(None, title="Wandlerfaktor")]
     zaehlwerk_id: Annotated[str | None, Field(None, alias="zaehlwerkId", title="Zaehlwerkid")]
     vorkommastellen: Annotated[int, Field(title="Vorkommastellen")]
     nachkommastellen: Annotated[int, Field(title="Nachkommastellen")]
     schwachlastfaehig: Annotated[bool, Field(title="Schwachlastfaehig")]
     konzessionsabgaben_typ: Annotated[Abgabeart | None, Field(None, alias="konzessionsabgabenTyp")]
-    active_from: Annotated[AwareDatetime, Field(alias="activeFrom", title="Activefrom")]
-    active_until: Annotated[AwareDatetime | None, Field(None, alias="activeUntil", title="Activeuntil")]
+    active_from: Annotated[datetime, Field(alias="activeFrom", title="Activefrom")]
+    active_until: Annotated[datetime | None, Field(None, alias="activeUntil", title="Activeuntil")]
     description: Annotated[str | None, Field(None, title="Description")]
     verbrauchsart: Annotated[str | None, Field(None, title="Verbrauchsart")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zeitraum.py` & `ibims-0.1.9/src/ibims/bo4e/com/zeitraum.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.zeiteinheit import Zeiteinheit
 
 
 class Zeitraum(BaseModel):
     """
@@ -18,15 +20,16 @@
 
     .. HINT::
         `Zeitraum JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zeitraum.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     dauer: Annotated[float | str | None, Field(None, title="Dauer")]
     einheit: Zeiteinheit | None = None
-    enddatum: Annotated[AwareDatetime | None, Field(None, title="Enddatum")]
-    endzeitpunkt: Annotated[AwareDatetime | None, Field(None, title="Endzeitpunkt")]
-    startdatum: Annotated[AwareDatetime | None, Field(None, title="Startdatum")]
-    startzeitpunkt: Annotated[AwareDatetime | None, Field(None, title="Startzeitpunkt")]
+    enddatum: Annotated[datetime | None, Field(None, title="Enddatum")]
+    endzeitpunkt: Annotated[datetime | None, Field(None, title="Endzeitpunkt")]
+    startdatum: Annotated[datetime | None, Field(None, title="Startdatum")]
+    startzeitpunkt: Annotated[datetime | None, Field(None, title="Startzeitpunkt")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zeitreihenwert.py` & `ibims-0.1.9/src/ibims/bo4e/com/zeitreihenwert.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
+from datetime import datetime
+
+from pydantic import BaseModel, ConfigDict, Field
 from typing_extensions import Annotated
 
 from ..enum.messwertstatus import Messwertstatus
 from ..enum.messwertstatuszusatz import Messwertstatuszusatz
 
 
 class Zeitreihenwert(BaseModel):
@@ -15,14 +17,15 @@
 
     .. HINT::
         `Zeitreihenwert JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zeitreihenwert.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
-    datum_uhrzeit_bis: Annotated[AwareDatetime | None, Field(None, alias="datumUhrzeitBis", title="Datumuhrzeitbis")]
-    datum_uhrzeit_von: Annotated[AwareDatetime | None, Field(None, alias="datumUhrzeitVon", title="Datumuhrzeitvon")]
+    datum_uhrzeit_bis: Annotated[datetime | None, Field(None, alias="datumUhrzeitBis", title="Datumuhrzeitbis")]
+    datum_uhrzeit_von: Annotated[datetime | None, Field(None, alias="datumUhrzeitVon", title="Datumuhrzeitvon")]
     status: Messwertstatus | None = None
     statuszusatz: Messwertstatuszusatz | None = None
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zeitreihenwertkompakt.py` & `ibims-0.1.9/src/ibims/bo4e/com/zeitreihenwertkompakt.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 
     .. HINT::
         `Zeitreihenwertkompakt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zeitreihenwertkompakt.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     status: Messwertstatus | None = None
     statuszusatz: Messwertstatuszusatz | None = None
     wert: Annotated[float | str | None, Field(None, title="Wert")]
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/com/zustaendigkeit.py` & `ibims-0.1.9/src/ibims/bo4e/com/zustaendigkeit.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,12 +14,13 @@
 
     .. HINT::
         `Zustaendigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zustaendigkeit.json>`_
     """
 
     model_config = ConfigDict(
         extra="allow",
+        populate_by_name=True,
     )
     id: Annotated[str | None, Field(None, alias="_id", title=" Id")]
     abteilung: Annotated[str | None, Field(None, title="Abteilung")]
     jobtitel: Annotated[str | None, Field(None, title="Jobtitel")]
     themengebiet: Themengebiet | None = None
```

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/aggregationsverantwortung.py` & `ibims-0.1.9/src/ibims/bo4e/enum/aggregationsverantwortung.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/bdew_artikelnummer.py` & `ibims-0.1.9/src/ibims/bo4e/enum/bdew_artikelnummer.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/bemessungsgroesse.py` & `ibims-0.1.9/src/ibims/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/bo_typ.py` & `ibims-0.1.9/src/ibims/bo4e/enum/bo_typ.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/dienstleistungstyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/geraetemerkmal.py` & `ibims-0.1.9/src/ibims/bo4e/enum/geraetemerkmal.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/geraetetyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/hinweis_thema.py` & `ibims-0.1.9/src/ibims/bo4e/enum/hinweis_thema.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/kalkulationsmethode.py` & `ibims-0.1.9/src/ibims/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/kundengruppe.py` & `ibims-0.1.9/src/ibims/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/kundengruppe_ka.py` & `ibims-0.1.9/src/ibims/bo4e/enum/kundengruppe_ka.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/kundentyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/landescode.py` & `ibims-0.1.9/src/ibims/bo4e/enum/landescode.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/leistungstyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/messpreistyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/messwertstatus.py` & `ibims-0.1.9/src/ibims/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/messwertstatuszusatz.py` & `ibims-0.1.9/src/ibims/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/nn_rechnungstyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/nn_rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/oekolabel.py` & `ibims-0.1.9/src/ibims/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/oekozertifikat.py` & `ibims-0.1.9/src/ibims/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/rechnungstyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/regionskriteriumtyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/themengebiet.py` & `ibims-0.1.9/src/ibims/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/voraussetzungen.py` & `ibims-0.1.9/src/ibims/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/waehrungscode.py` & `ibims-0.1.9/src/ibims/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/bo4e/enum/zaehlertyp.py` & `ibims-0.1.9/src/ibims/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/__init__.py` & `ibims-0.1.9/src/ibims/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/agent_hint_loader.py` & `ibims-0.1.9/src/ibims/datasets/agent_hint_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     This is a bo4e data set that consists of
     * a GeschaeftspartnerErweitert
     * a Vertrag
     * a hint
     In the context of this package is may be used to create ED$ AgentHint Data.
     """
 
-    geschaeftspartner_erw: Geschaeftspartner
+    geschaeftspartner: Geschaeftspartner
     """
     The following attribute needs to be filled for this DataSet:
     - externe_referenzen
     - customerID
     """
 
     vertrag: Vertrag
```

### Comparing `ibims-0.1.8/src/ibims/datasets/base.py` & `ibims-0.1.9/src/ibims/datasets/base.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/customer_loader.py` & `ibims-0.1.9/src/ibims/datasets/customer_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     In the context of this package is may be used to create Tripica Customer Data.
     """
 
     powercloud_customer_id: str  #: the powercloud customer id that was used to create this data set
     # this allows us to track a customer from its source up the target
     # https://github.com/Hochfrequenz/bo4e_migration_framework/blob/6f091b76ff4e7a72bb0ff6ecb46a8477d35b5bf8/src/bomf/model/__init__.py#L70
 
-    geschaeftspartner_erw: Geschaeftspartner
+    geschaeftspartner: Geschaeftspartner
     """
     The following attributes need to be filled for this DataSet:
     - name1 (Surname)
     - name2 (Firstname)
     - name3 (Title e.g. Dr.)
     - erstellungsdatum
     - geburtstag
```

### Comparing `ibims-0.1.8/src/ibims/datasets/document_loader.py` & `ibims-0.1.9/src/ibims/datasets/document_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     doc_id: str
     """
     a unique id identifying a document in the tripica data loader set (typically a filename)
     """
 
-    geschaeftspartner_erw: Geschaeftspartner
+    geschaeftspartner: Geschaeftspartner
     """
     The following attribute needs to be filled for this DataSet:
     - externe_referenzen
     especially the customerID
     """
 
     vertrag: Vertrag
```

### Comparing `ibims-0.1.8/src/ibims/datasets/invoice_loader.py` & `ibims-0.1.9/src/ibims/datasets/invoice_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
     The following attributes need to be filled for this DataSet:
     - lokationsadresse
     - marktlokations_id
     - sparte
     """
 
-    rechnung_erweitert: Rechnung
+    rechnung: Rechnung
     """
     The following attributes need to be filled for this Dataset:
     - rechungstyp
     - rechungsnummer
     - rechungsdatum
     - faelligkeitsdatum
     - rechungsperiode
```

### Comparing `ibims-0.1.8/src/ibims/datasets/network_loader.py` & `ibims-0.1.9/src/ibims/datasets/network_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     - name3 (Title e.g. Dr.)
     - gewerbekennzeichnung
     - partneradresse
     """
 
     liefer_adresse: Adresse
 
-    geschaeftspartner_mit_rechnungs_adresse: Geschaeftspartner
+    geschaeftspartner: Geschaeftspartner
     """
     This information is used for the customerMeterReadings part and
     is not a real business partner, so not all information of this object arte needed:
     - name1 (Surname)
     - name2 (Firstname)
     - partneradresse
     """
```

### Comparing `ibims-0.1.8/src/ibims/datasets/product_loader.py` & `ibims-0.1.9/src/ibims/datasets/product_loader.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/quantities_loader.py` & `ibims-0.1.9/src/ibims/datasets/quantities_loader.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/resource_loader.py` & `ibims-0.1.9/src/ibims/datasets/resource_loader.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/datasets/usage_loader.py` & `ibims-0.1.9/src/ibims/datasets/usage_loader.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/src/ibims/targetmodels/transactiondata.py` & `ibims-0.1.9/src/ibims/targetmodels/transactiondata.py`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/.gitignore` & `ibims-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/LICENSE` & `ibims-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/pyproject.toml` & `ibims-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibims-0.1.8/PKG-INFO` & `ibims-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibims
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Pydantic based BO4E data model that is inteded to be used in data migrations from one system to another
 Project-URL: Changelog, https://github.com/Hochfrequenz/intermediate-bo4e-migration-models/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/intermediate-bo4e-migration-models
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
 Keywords: bo4e,migration,pydantic
```

