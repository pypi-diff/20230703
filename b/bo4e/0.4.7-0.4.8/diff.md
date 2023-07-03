# Comparing `tmp/bo4e-0.4.7.tar.gz` & `tmp/bo4e-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo4e-0.4.7.tar", last modified: Wed Feb 15 08:21:09 2023, max compression
+gzip compressed data, was "bo4e-0.4.8.tar", last modified: Mon Jul  3 04:53:41 2023, max compression
```

## Comparing `bo4e-0.4.7.tar` & `bo4e-0.4.8.tar`

### file list

```diff
@@ -1,444 +1,444 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.222538 bo4e-0.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.154536 bo4e-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.154536 bo4e-0.4.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.154536 bo4e-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-15 08:20:56.000000 bo4e-0.4.7/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-02-15 08:20:56.000000 bo4e-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-15 08:20:56.000000 bo4e-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-02-15 08:20:56.000000 bo4e-0.4.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-02-15 08:20:56.000000 bo4e-0.4.7/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.158536 bo4e-0.4.7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-15 08:20:56.000000 bo4e-0.4.7/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-15 08:20:56.000000 bo4e-0.4.7/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-15 08:20:56.000000 bo4e-0.4.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-02-15 08:20:56.000000 bo4e-0.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-02-15 08:20:56.000000 bo4e-0.4.7/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 08:20:56.000000 bo4e-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-02-15 08:21:09.222538 bo4e-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-15 08:20:56.000000 bo4e-0.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.158536 bo4e-0.4.7/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.158536 bo4e-0.4.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/_static/bo4e-python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/_static/bo4e-python-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.158536 bo4e-0.4.7/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/api/bo4e.bo.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/api/bo4e.com.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/api/bo4e.enum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/api/bo4e.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/test_uml.py
--rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-02-15 08:20:56.000000 bo4e-0.4.7/docs/uml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.158536 bo4e-0.4.7/json_schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.166536 bo4e-0.4.7/json_schemas/bo/
--rw-r--r--   0 runner    (1001) docker     (123)    52031 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Angebot.json
--rw-r--r--   0 runner    (1001) docker     (123)    21681 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Ansprechpartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    29974 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Ausschreibung.json
--rw-r--r--   0 runner    (1001) docker     (123)    30396 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Buendelvertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Energiemenge.json
--rw-r--r--   0 runner    (1001) docker     (123)    18311 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Fremdkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Geschaeftsobjekt.json
--rw-r--r--   0 runner    (1001) docker     (123)    13832 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Geschaeftspartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Kosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Lastgang.json
--rw-r--r--   0 runner    (1001) docker     (123)    11722 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/LastgangKompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)    24819 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Marktlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Marktteilnehmer.json
--rw-r--r--   0 runner    (1001) docker     (123)    32254 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Messlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    38252 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Netznutzungsrechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)    32201 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Preisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    39060 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/PreisblattDienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)    39717 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/PreisblattHardware.json
--rw-r--r--   0 runner    (1001) docker     (123)    33024 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/PreisblattKonzessionsabgabe.json
--rw-r--r--   0 runner    (1001) docker     (123)    39734 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/PreisblattMessung.json
--rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/PreisblattNetznutzung.json
--rw-r--r--   0 runner    (1001) docker     (123)    35974 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Rechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Region.json
--rw-r--r--   0 runner    (1001) docker     (123)    61825 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Regionaltarif.json
--rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Standorteigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)    59072 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Tarif.json
--rw-r--r--   0 runner    (1001) docker     (123)    30329 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Tarifinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)    44502 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Tarifkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Tarifpreisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26426 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Vertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)    21175 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Zaehler.json
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/Zeitreihe.json
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/bo/_LastgangBody.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.178537 bo4e-0.4.7/json_schemas/com/
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Adresse.json
--rw-r--r--   0 runner    (1001) docker     (123)     9529 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Angebotsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    39222 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Angebotsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)    41360 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Angebotsvariante.json
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/AufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/AufAbschlagProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26999 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/AufAbschlagRegional.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/AufAbschlagstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Ausschreibungsdetail.json
--rw-r--r--   0 runner    (1001) docker     (123)    18347 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Ausschreibungslos.json
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Betrag.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/COM.json
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Dienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Energieherkunft.json
--rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Energiemix.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/ExterneReferenz.json
--rw-r--r--   0 runner    (1001) docker     (123)    11848 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Fremdkostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Fremdkostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Geokoordinaten.json
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Geraet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Geraeteeigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Hardware.json
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Katasteradresse.json
--rw-r--r--   0 runner    (1001) docker     (123)    11282 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Kostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Kostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/KriteriumWert.json
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/MarktgebietInfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Menge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Messlokationszuordnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/PositionsAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Preis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Preisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)    11261 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Preisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Preisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Rechnungsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/RegionaleGueltigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/RegionalePreisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/RegionalePreisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/RegionaleTarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    29831 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/RegionalerAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Regionskriterium.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Rufnummer.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Sigmoidparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/StandorteigenschaftenAllgemein.json
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/StandorteigenschaftenGas.json
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/StandorteigenschaftenStrom.json
--rw-r--r--   0 runner    (1001) docker     (123)     5783 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Steuerbetrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Tagesvektor.json
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Tarifberechnungsparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Tarifeinschraenkung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Tarifpreis.json
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Tarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/TarifpreispositionProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/TarifpreisstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Unterschrift.json
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Verbrauch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Vertragskonditionen.json
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Vertragsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zaehlwerk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zeitintervall.json
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zeitraum.json
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zeitreihenwert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zeitreihenwertkompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/com/Zustaendigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-15 08:20:56.000000 bo4e-0.4.7/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-15 08:20:56.000000 bo4e-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 08:20:56.000000 bo4e-0.4.7/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-02-15 08:20:56.000000 bo4e-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-02-15 08:21:09.222538 bo4e-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-02-15 08:20:56.000000 bo4e-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.150535 bo4e-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.178537 bo4e-0.4.7/src/bo4e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.182537 bo4e-0.4.7/src/bo4e/bo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/bo/zeitreihe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.194537 bo4e-0.4.7/src/bo4e/com/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/com.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/externereferenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/rufnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/com/zustaendigkeit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.206538 bo4e-0.4.7/src/bo4e/enum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/anrede.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/artikelid.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/botyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/energierichtung.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/geraetemerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kontaktart.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/kundentyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/landescode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/marktrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/messart.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/messgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/netzebene.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/nnrechnungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/nnrechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/oekolabel.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/preismodell.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/preisstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/preistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/rufnummernart.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/sparte.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tarifart.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tariftyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/themengebiet.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/titel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/vertragsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/vertragsform.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/enum/zeiteinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-15 08:20:56.000000 bo4e-0.4.7/src/bo4e/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.178537 bo4e-0.4.7/src/bo4e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 08:21:09.000000 bo4e-0.4.7/src/bo4e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.222538 bo4e-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/serialization_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_bypassing_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.154536 bo4e-0.4.7/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 08:21:09.222538 bo4e-0.4.7/tests/test_data/test_data_adresse/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_externe_referenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_kriteriumswert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_lastgangkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblatt_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblatt_messung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zeitreihe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-02-15 08:20:56.000000 bo4e-0.4.7/tests/test_zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-02-15 08:20:56.000000 bo4e-0.4.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-03 04:53:29.000000 bo4e-0.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 04:53:29.000000 bo4e-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-03 04:53:29.000000 bo4e-0.4.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 04:53:29.000000 bo4e-0.4.8/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 04:53:29.000000 bo4e-0.4.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 04:53:29.000000 bo4e-0.4.8/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 04:53:29.000000 bo4e-0.4.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-03 04:53:29.000000 bo4e-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 04:53:29.000000 bo4e-0.4.8/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:29.000000 bo4e-0.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 04:53:41.790287 bo4e-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-03 04:53:29.000000 bo4e-0.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.bo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.com.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.enum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/test_uml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/uml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/json_schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.754287 bo4e-0.4.8/json_schemas/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)    52157 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Angebot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Ansprechpartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Ausschreibung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Buendelvertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Energiemenge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Fremdkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Geschaeftsobjekt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Geschaeftspartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Kosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Lastgang.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/LastgangKompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24945 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Marktlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Marktteilnehmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Messlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Netznutzungsrechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Preisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39186 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattDienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39843 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattHardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattKonzessionsabgabe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39860 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattMessung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattNetznutzung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36100 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Rechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Region.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61951 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Regionaltarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Standorteigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59198 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44628 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56245 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifpreisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26552 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Vertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Zaehler.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Zeitreihe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/_LastgangBody.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.758287 bo4e-0.4.8/json_schemas/com/
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Adresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsvariante.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagRegional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Ausschreibungsdetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Ausschreibungslos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Betrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/COM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Dienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Energieherkunft.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Energiemix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/ExterneReferenz.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Fremdkostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Fremdkostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geokoordinaten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geraet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geraeteeigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Hardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Katasteradresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Kostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Kostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/KriteriumWert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/MarktgebietInfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Menge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Messlokationszuordnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/PositionsAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Rechnungsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionaleGueltigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalePreisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalePreisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionaleTarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalerAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Regionskriterium.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Rufnummer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Sigmoidparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenAllgemein.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenGas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenStrom.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Steuerbetrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tagesvektor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifberechnungsparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifeinschraenkung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifpreis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/TarifpreispositionProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/TarifpreisstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Unterschrift.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Verbrauch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Vertragskonditionen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Vertragsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zaehlwerk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitintervall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitraum.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitreihenwert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitreihenwertkompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zustaendigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-03 04:53:29.000000 bo4e-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 04:53:29.000000 bo4e-0.4.8/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 04:53:29.000000 bo4e-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 04:53:41.790287 bo4e-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 04:53:29.000000 bo4e-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.746287 bo4e-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/zeitreihe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.774287 bo4e-0.4.8/src/bo4e/com/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/externereferenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/rufnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zustaendigkeit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.782287 bo4e-0.4.8/src/bo4e/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/anrede.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/artikelid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/botyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geraetemerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/landescode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/netzebene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/nnrechnungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/nnrechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preismodell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rufnummernart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/sparte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/titel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zeiteinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/serialization_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_bypassing_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.746287 bo4e-0.4.8/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/tests/test_data/test_data_adresse/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_externe_referenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kriteriumswert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_lastgangkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_messung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-03 04:53:29.000000 bo4e-0.4.8/tox.ini
```

### Comparing `bo4e-0.4.7/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-0.4.8/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-0.4.8/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/dependabot.yml` & `bo4e-0.4.8/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/codeql-analysis.yml` & `bo4e-0.4.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/coverage.yml` & `bo4e-0.4.8/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/docs.yml` & `bo4e-0.4.8/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/formatting.yml` & `bo4e-0.4.8/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/linting.yml` & `bo4e-0.4.8/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/python-publish.yml` & `bo4e-0.4.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.github/workflows/tests.yml` & `bo4e-0.4.8/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.gitignore` & `bo4e-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.pre-commit-config.yaml` & `bo4e-0.4.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.pylintrc` & `bo4e-0.4.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/.readthedocs.yaml` & `bo4e-0.4.8/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/CONTRIBUTING.md` & `bo4e-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/LICENSE.rst` & `bo4e-0.4.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/PKG-INFO` & `bo4e-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.4.7/README.rst` & `bo4e-0.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/Makefile` & `bo4e-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/_static/bo4e-python-favicon.png` & `bo4e-0.4.8/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/_static/bo4e-python-favicon.svg` & `bo4e-0.4.8/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/_static/bo4e-python-logo.png` & `bo4e-0.4.8/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/_static/bo4e-python-logo.svg` & `bo4e-0.4.8/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/api/bo4e.bo.rst` & `bo4e-0.4.8/docs/api/bo4e.bo.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/api/bo4e.com.rst` & `bo4e-0.4.8/docs/api/bo4e.com.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/api/bo4e.enum.rst` & `bo4e-0.4.8/docs/api/bo4e.enum.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/conf.py` & `bo4e-0.4.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/index.rst` & `bo4e-0.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/docs/uml.py` & `bo4e-0.4.8/docs/uml.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/json_schemas/bo/Angebot.json` & `bo4e-0.4.8/json_schemas/bo/Angebot.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999884259259259%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Ansprechpartner.json` & `bo4e-0.4.8/json_schemas/bo/Ansprechpartner.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999643874643874%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Ausschreibung.json` & `bo4e-0.4.8/json_schemas/bo/Ausschreibung.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999789562289562%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Buendelvertrag.json` & `bo4e-0.4.8/json_schemas/bo/Buendelvertrag.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999756335282651%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Energiemenge.json` & `bo4e-0.4.8/json_schemas/bo/Energiemenge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/json_schemas/bo/Fremdkosten.json` & `bo4e-0.4.8/json_schemas/bo/Fremdkosten.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1138,8 +1138,8 @@
 00004710: 6e67 220a 2020 2020 2020 2020 7d0a 2020  ng".        }.  
 00004720: 2020 7d2c 0a20 2020 2022 7265 7175 6972    },.    "requir
 00004730: 6564 223a 205b 0a20 2020 2020 2020 2022  ed": [.        "
 00004740: 6775 656c 7469 676b 6569 7422 0a20 2020  gueltigkeit".   
 00004750: 205d 2c0a 2020 2020 2274 6974 6c65 223a   ],.    "title":
 00004760: 2022 4672 656d 646b 6f73 7465 6e22 2c0a   "Fremdkosten",.
 00004770: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00004780: 6563 7422 0a7d 0a                        ect".}.
+00004780: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Geschaeftsobjekt.json` & `bo4e-0.4.8/json_schemas/bo/Geschaeftsobjekt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -217,8 +217,8 @@
 00000d80: 6974 6c65 223a 2022 5665 7273 696f 6e73  itle": "Versions
 00000d90: 7472 756b 7475 7222 2c0a 2020 2020 2020  truktur",.      
 00000da0: 2020 2020 2020 2274 7970 6522 3a20 2273        "type": "s
 00000db0: 7472 696e 6722 0a20 2020 2020 2020 207d  tring".        }
 00000dc0: 0a20 2020 207d 2c0a 2020 2020 2274 6974  .    },.    "tit
 00000dd0: 6c65 223a 2022 4765 7363 6861 6566 7473  le": "Geschaefts
 00000de0: 6f62 6a65 6b74 222c 0a20 2020 2022 7479  objekt",.    "ty
-00000df0: 7065 223a 2022 6f62 6a65 6374 220a 7d0a  pe": "object".}.
+00000df0: 7065 223a 2022 6f62 6a65 6374 220a 7d    pe": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Geschaeftspartner.json` & `bo4e-0.4.8/json_schemas/bo/Geschaeftspartner.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999338624338625%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Kosten.json` & `bo4e-0.4.8/json_schemas/bo/Kosten.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1143,8 +1143,8 @@
 00004760: 2020 2020 226b 6f73 7465 6e6b 6c61 7373      "kostenklass
 00004770: 6522 2c0a 2020 2020 2020 2020 2267 7565  e",.        "gue
 00004780: 6c74 6967 6b65 6974 222c 0a20 2020 2020  ltigkeit",.     
 00004790: 2020 2022 6b6f 7374 656e 626c 6f65 636b     "kostenbloeck
 000047a0: 6522 0a20 2020 205d 2c0a 2020 2020 2274  e".    ],.    "t
 000047b0: 6974 6c65 223a 2022 4b6f 7374 656e 222c  itle": "Kosten",
 000047c0: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-000047d0: 6a65 6374 220a 7d0a                      ject".}.
+000047d0: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Lastgang.json` & `bo4e-0.4.8/json_schemas/bo/Lastgang.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -601,8 +601,8 @@
 00002580: 2020 2020 226c 6f6b 6174 696f 6e73 7479      "lokationsty
 00002590: 7022 2c0a 2020 2020 2020 2020 226d 6573  p",.        "mes
 000025a0: 7367 726f 6573 7365 222c 0a20 2020 2020  sgroesse",.     
 000025b0: 2020 2022 7765 7274 6522 0a20 2020 205d     "werte".    ]
 000025c0: 2c0a 2020 2020 2274 6974 6c65 223a 2022  ,.    "title": "
 000025d0: 4c61 7374 6761 6e67 222c 0a20 2020 2022  Lastgang",.    "
 000025e0: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-000025f0: 7d0a                                     }.
+000025f0: 7d                                       }
```

### Comparing `bo4e-0.4.7/json_schemas/bo/LastgangKompakt.json` & `bo4e-0.4.8/json_schemas/bo/LastgangKompakt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -726,8 +726,8 @@
 00002d50: 7367 726f 6573 7365 222c 0a20 2020 2020  sgroesse",.     
 00002d60: 2020 2022 7a65 6974 696e 7465 7276 616c     "zeitinterval
 00002d70: 6c22 2c0a 2020 2020 2020 2020 2274 6167  l",.        "tag
 00002d80: 6573 7665 6b74 6f72 656e 220a 2020 2020  esvektoren".    
 00002d90: 5d2c 0a20 2020 2022 7469 746c 6522 3a20  ],.    "title": 
 00002da0: 224c 6173 7467 616e 674b 6f6d 7061 6b74  "LastgangKompakt
 00002db0: 222c 0a20 2020 2022 7479 7065 223a 2022  ",.    "type": "
-00002dc0: 6f62 6a65 6374 220a 7d0a                 object".}.
+00002dc0: 6f62 6a65 6374 220a 7d                   object".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Marktlokation.json` & `bo4e-0.4.8/json_schemas/bo/Marktlokation.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999768518518518%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Marktteilnehmer.json` & `bo4e-0.4.8/json_schemas/bo/Marktteilnehmer.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999537037037037%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Messlokation.json` & `bo4e-0.4.8/json_schemas/bo/Messlokation.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999798711755233%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Netznutzungsrechnung.json` & `bo4e-0.4.8/json_schemas/bo/Netznutzungsrechnung.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999821937321937%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Preisblatt.json` & `bo4e-0.4.8/json_schemas/bo/Preisblatt.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999807098765432%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/PreisblattDienstleistung.json` & `bo4e-0.4.8/json_schemas/bo/PreisblattDienstleistung.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999840357598978%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/PreisblattHardware.json` & `bo4e-0.4.8/json_schemas/bo/PreisblattHardware.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999845679012346%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/PreisblattKonzessionsabgabe.json` & `bo4e-0.4.8/json_schemas/bo/PreisblattKonzessionsabgabe.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999814814814815%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/PreisblattMessung.json` & `bo4e-0.4.8/json_schemas/bo/PreisblattMessung.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999845679012346%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/PreisblattNetznutzung.json` & `bo4e-0.4.8/json_schemas/bo/PreisblattNetznutzung.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999982853223594%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Rechnung.json` & `bo4e-0.4.8/json_schemas/bo/Rechnung.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999798711755233%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Region.json` & `bo4e-0.4.8/json_schemas/bo/Region.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -425,8 +425,8 @@
 00001a80: 207d 2c0a 2020 2020 2272 6571 7569 7265   },.    "require
 00001a90: 6422 3a20 5b0a 2020 2020 2020 2020 2262  d": [.        "b
 00001aa0: 657a 6569 6368 6e75 6e67 222c 0a20 2020  ezeichnung",.   
 00001ab0: 2020 2020 2022 706f 7369 7469 764c 6973       "positivLis
 00001ac0: 7465 220a 2020 2020 5d2c 0a20 2020 2022  te".    ],.    "
 00001ad0: 7469 746c 6522 3a20 2252 6567 696f 6e22  title": "Region"
 00001ae0: 2c0a 2020 2020 2274 7970 6522 3a20 226f  ,.    "type": "o
-00001af0: 626a 6563 7422 0a7d 0a                   bject".}.
+00001af0: 626a 6563 7422 0a7d                      bject".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Regionaltarif.json` & `bo4e-0.4.8/json_schemas/bo/Regionaltarif.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999910968660969%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Standorteigenschaften.json` & `bo4e-0.4.8/json_schemas/bo/Standorteigenschaften.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -446,8 +446,8 @@
 00001bd0: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
 00001be0: 2022 7265 7175 6972 6564 223a 205b 0a20   "required": [. 
 00001bf0: 2020 2020 2020 2022 6569 6765 6e73 6368         "eigensch
 00001c00: 6166 7465 6e53 7472 6f6d 220a 2020 2020  aftenStrom".    
 00001c10: 5d2c 0a20 2020 2022 7469 746c 6522 3a20  ],.    "title": 
 00001c20: 2253 7461 6e64 6f72 7465 6967 656e 7363  "Standorteigensc
 00001c30: 6861 6674 656e 222c 0a20 2020 2022 7479  haften",.    "ty
-00001c40: 7065 223a 2022 6f62 6a65 6374 220a 7d0a  pe": "object".}.
+00001c40: 7065 223a 2022 6f62 6a65 6374 220a 7d    pe": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Tarif.json` & `bo4e-0.4.8/json_schemas/bo/Tarif.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999903549382716%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Tarifinfo.json` & `bo4e-0.4.8/json_schemas/bo/Tarifinfo.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999798711755233%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Tarifkosten.json` & `bo4e-0.4.8/json_schemas/bo/Tarifkosten.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999863834422658%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Tarifpreisblatt.json` & `bo4e-0.4.8/json_schemas/bo/Tarifpreisblatt.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999901497241922%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Vertrag.json` & `bo4e-0.4.8/json_schemas/bo/Vertrag.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999742798353909%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Zaehler.json` & `bo4e-0.4.8/json_schemas/bo/Zaehler.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999969135802469%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/bo/Zeitreihe.json` & `bo4e-0.4.8/json_schemas/bo/Zeitreihe.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -666,8 +666,8 @@
 00002990: 7274 222c 0a20 2020 2020 2020 2022 6d65  rt",.        "me
 000029a0: 6469 756d 222c 0a20 2020 2020 2020 2022  dium",.        "
 000029b0: 6569 6e68 6569 7422 2c0a 2020 2020 2020  einheit",.      
 000029c0: 2020 2277 6572 7465 220a 2020 2020 5d2c    "werte".    ],
 000029d0: 0a20 2020 2022 7469 746c 6522 3a20 225a  .    "title": "Z
 000029e0: 6569 7472 6569 6865 222c 0a20 2020 2022  eitreihe",.    "
 000029f0: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-00002a00: 7d0a                                     }.
+00002a00: 7d                                       }
```

### Comparing `bo4e-0.4.7/json_schemas/bo/_LastgangBody.json` & `bo4e-0.4.8/json_schemas/bo/_LastgangBody.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -312,8 +312,8 @@
 00001370: 2020 2020 2022 6c6f 6b61 7469 6f6e 7349       "lokationsI
 00001380: 6422 2c0a 2020 2020 2020 2020 226c 6f6b  d",.        "lok
 00001390: 6174 696f 6e73 7479 7022 2c0a 2020 2020  ationstyp",.    
 000013a0: 2020 2020 226d 6573 7367 726f 6573 7365      "messgroesse
 000013b0: 220a 2020 2020 5d2c 0a20 2020 2022 7469  ".    ],.    "ti
 000013c0: 746c 6522 3a20 225f 4c61 7374 6761 6e67  tle": "_Lastgang
 000013d0: 426f 6479 222c 0a20 2020 2022 7479 7065  Body",.    "type
-000013e0: 223a 2022 6f62 6a65 6374 220a 7d0a       ": "object".}.
+000013e0: 223a 2022 6f62 6a65 6374 220a 7d         ": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Adresse.json` & `bo4e-0.4.8/json_schemas/com/Adresse.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9907407407407408%*

 * *Differences: {"'properties'": "{'ortsteil': OrderedDict([('title', 'Ortsteil'), ('type', 'string')])}"}*

```diff
@@ -279,14 +279,18 @@
             ],
             "default": "DE"
         },
         "ort": {
             "title": "Ort",
             "type": "string"
         },
+        "ortsteil": {
+            "title": "Ortsteil",
+            "type": "string"
+        },
         "postfach": {
             "title": "Postfach",
             "type": "string"
         },
         "postleitzahl": {
             "title": "Postleitzahl",
             "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/com/Angebotsposition.json` & `bo4e-0.4.8/json_schemas/com/Angebotsposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -589,8 +589,8 @@
 000024c0: 0a20 2020 2020 2020 2022 706f 7369 7469  .        "positi
 000024d0: 6f6e 7362 657a 6569 6368 6e75 6e67 222c  onsbezeichnung",
 000024e0: 0a20 2020 2020 2020 2022 706f 7369 7469  .        "positi
 000024f0: 6f6e 7370 7265 6973 220a 2020 2020 5d2c  onspreis".    ],
 00002500: 0a20 2020 2022 7469 746c 6522 3a20 2241  .    "title": "A
 00002510: 6e67 6562 6f74 7370 6f73 6974 696f 6e22  ngebotsposition"
 00002520: 2c0a 2020 2020 2274 7970 6522 3a20 226f  ,.    "type": "o
-00002530: 626a 6563 7422 0a7d 0a                   bject".}.
+00002530: 626a 6563 7422 0a7d                      bject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Angebotsteil.json` & `bo4e-0.4.8/json_schemas/com/Angebotsteil.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999850657108721%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/com/Angebotsvariante.json` & `bo4e-0.4.8/json_schemas/com/Angebotsvariante.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999859708193042%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/com/AufAbschlag.json` & `bo4e-0.4.8/json_schemas/com/AufAbschlag.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -446,8 +446,8 @@
 00001bd0: 2022 7265 7175 6972 6564 223a 205b 0a20   "required": [. 
 00001be0: 2020 2020 2020 2022 6265 7a65 6963 686e         "bezeichn
 00001bf0: 756e 6722 2c0a 2020 2020 2020 2020 2273  ung",.        "s
 00001c00: 7461 6666 656c 6e22 0a20 2020 205d 2c0a  taffeln".    ],.
 00001c10: 2020 2020 2274 6974 6c65 223a 2022 4175      "title": "Au
 00001c20: 6641 6273 6368 6c61 6722 2c0a 2020 2020  fAbschlag",.    
 00001c30: 2274 7970 6522 3a20 226f 626a 6563 7422  "type": "object"
-00001c40: 0a7d 0a                                  .}.
+00001c40: 0a7d                                     .}
```

### Comparing `bo4e-0.4.7/json_schemas/com/AufAbschlagProOrt.json` & `bo4e-0.4.8/json_schemas/com/AufAbschlagProOrt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
 000008b0: 2020 2020 2022 6f72 7422 2c0a 2020 2020       "ort",.    
 000008c0: 2020 2020 226e 6574 7a6e 7222 2c0a 2020      "netznr",.  
 000008d0: 2020 2020 2020 2273 7461 6666 656c 6e22        "staffeln"
 000008e0: 0a20 2020 205d 2c0a 2020 2020 2274 6974  .    ],.    "tit
 000008f0: 6c65 223a 2022 4175 6641 6273 6368 6c61  le": "AufAbschla
 00000900: 6750 726f 4f72 7422 2c0a 2020 2020 2274  gProOrt",.    "t
 00000910: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-00000920: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/AufAbschlagRegional.json` & `bo4e-0.4.8/json_schemas/com/AufAbschlagRegional.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1681,8 +1681,8 @@
 00006900: 7175 6972 6564 223a 205b 0a20 2020 2020  quired": [.     
 00006910: 2020 2022 6265 7a65 6963 686e 756e 6722     "bezeichnung"
 00006920: 2c0a 2020 2020 2020 2020 2262 6574 7261  ,.        "betra
 00006930: 6567 6522 0a20 2020 205d 2c0a 2020 2020  ege".    ],.    
 00006940: 2274 6974 6c65 223a 2022 4175 6641 6273  "title": "AufAbs
 00006950: 6368 6c61 6752 6567 696f 6e61 6c22 2c0a  chlagRegional",.
 00006960: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00006970: 6563 7422 0a7d 0a                        ect".}.
+00006970: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/AufAbschlagstaffelProOrt.json` & `bo4e-0.4.8/json_schemas/com/AufAbschlagstaffelProOrt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 12% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 00000320: 2020 2020 2020 2020 2273 7461 6666 656c          "staffel
 00000330: 6772 656e 7a65 566f 6e22 2c0a 2020 2020  grenzeVon",.    
 00000340: 2020 2020 2273 7461 6666 656c 6772 656e      "staffelgren
 00000350: 7a65 4269 7322 0a20 2020 205d 2c0a 2020  zeBis".    ],.  
 00000360: 2020 2274 6974 6c65 223a 2022 4175 6641    "title": "AufA
 00000370: 6273 6368 6c61 6773 7461 6666 656c 5072  bschlagstaffelPr
 00000380: 6f4f 7274 222c 0a20 2020 2022 7479 7065  oOrt",.    "type
-00000390: 223a 2022 6f62 6a65 6374 220a 7d0a       ": "object".}.
+00000390: 223a 2022 6f62 6a65 6374 220a 7d         ": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Ausschreibungsdetail.json` & `bo4e-0.4.8/json_schemas/com/Ausschreibungsdetail.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999338624338625%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/com/Ausschreibungslos.json` & `bo4e-0.4.8/json_schemas/com/Ausschreibungslos.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999614197530864%*

 * *Differences: {"'definitions'": "{'Adresse': {'properties': {'ortsteil': OrderedDict([('title', 'Ortsteil'), "*

 * *                  "('type', 'string')])}}}"}*

```diff
@@ -23,14 +23,18 @@
                     ],
                     "default": "DE"
                 },
                 "ort": {
                     "title": "Ort",
                     "type": "string"
                 },
+                "ortsteil": {
+                    "title": "Ortsteil",
+                    "type": "string"
+                },
                 "postfach": {
                     "title": "Postfach",
                     "type": "string"
                 },
                 "postleitzahl": {
                     "title": "Postleitzahl",
                     "type": "string"
```

### Comparing `bo4e-0.4.7/json_schemas/com/Betrag.json` & `bo4e-0.4.8/json_schemas/com/Betrag.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -320,8 +320,8 @@
 000013f0: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
 00001400: 2022 7265 7175 6972 6564 223a 205b 0a20   "required": [. 
 00001410: 2020 2020 2020 2022 7765 7274 222c 0a20         "wert",. 
 00001420: 2020 2020 2020 2022 7761 6568 7275 6e67         "waehrung
 00001430: 220a 2020 2020 5d2c 0a20 2020 2022 7469  ".    ],.    "ti
 00001440: 746c 6522 3a20 2242 6574 7261 6722 2c0a  tle": "Betrag",.
 00001450: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00001460: 6563 7422 0a7d 0a                        ect".}.
+00001460: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Dienstleistung.json` & `bo4e-0.4.8/json_schemas/com/Dienstleistung.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -158,8 +158,8 @@
 000009d0: 6422 3a20 5b0a 2020 2020 2020 2020 2264  d": [.        "d
 000009e0: 6965 6e73 746c 6569 7374 756e 6773 7479  ienstleistungsty
 000009f0: 7022 2c0a 2020 2020 2020 2020 2262 657a  p",.        "bez
 00000a00: 6569 6368 6e75 6e67 220a 2020 2020 5d2c  eichnung".    ],
 00000a10: 0a20 2020 2022 7469 746c 6522 3a20 2244  .    "title": "D
 00000a20: 6965 6e73 746c 6569 7374 756e 6722 2c0a  ienstleistung",.
 00000a30: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000a40: 6563 7422 0a7d 0a                        ect".}.
+00000a40: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Energieherkunft.json` & `bo4e-0.4.8/json_schemas/com/Energieherkunft.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 00000510: 223a 205b 0a20 2020 2020 2020 2022 6572  ": [.        "er
 00000520: 7a65 7567 756e 6773 6172 7422 2c0a 2020  zeugungsart",.  
 00000530: 2020 2020 2020 2261 6e74 6569 6c50 726f        "anteilPro
 00000540: 7a65 6e74 220a 2020 2020 5d2c 0a20 2020  zent".    ],.   
 00000550: 2022 7469 746c 6522 3a20 2245 6e65 7267   "title": "Energ
 00000560: 6965 6865 726b 756e 6674 222c 0a20 2020  ieherkunft",.   
 00000570: 2022 7479 7065 223a 2022 6f62 6a65 6374   "type": "object
-00000580: 220a 7d0a                                ".}.
+00000580: 220a 7d                                  ".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Energiemix.json` & `bo4e-0.4.8/json_schemas/com/Energiemix.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -333,8 +333,8 @@
 000014c0: 2020 2022 6265 7a65 6963 686e 756e 6722     "bezeichnung"
 000014d0: 2c0a 2020 2020 2020 2020 2267 7565 6c74  ,.        "guelt
 000014e0: 6967 6b65 6974 736a 6168 7222 2c0a 2020  igkeitsjahr",.  
 000014f0: 2020 2020 2020 2261 6e74 6569 6c22 0a20        "anteil". 
 00001500: 2020 205d 2c0a 2020 2020 2274 6974 6c65     ],.    "title
 00001510: 223a 2022 456e 6572 6769 656d 6978 222c  ": "Energiemix",
 00001520: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00001530: 6a65 6374 220a 7d0a                      ject".}.
+00001530: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/ExterneReferenz.json` & `bo4e-0.4.8/json_schemas/com/ExterneReferenz.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 00000330: 7d2c 0a20 2020 2022 7265 7175 6972 6564  },.    "required
 00000340: 223a 205b 0a20 2020 2020 2020 2022 6578  ": [.        "ex
 00000350: 5265 664e 616d 6522 2c0a 2020 2020 2020  RefName",.      
 00000360: 2020 2265 7852 6566 5765 7274 220a 2020    "exRefWert".  
 00000370: 2020 5d2c 0a20 2020 2022 7469 746c 6522    ],.    "title"
 00000380: 3a20 2245 7874 6572 6e65 5265 6665 7265  : "ExterneRefere
 00000390: 6e7a 222c 0a20 2020 2022 7479 7065 223a  nz",.    "type":
-000003a0: 2022 6f62 6a65 6374 220a 7d0a             "object".}.
+000003a0: 2022 6f62 6a65 6374 220a 7d               "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Fremdkostenblock.json` & `bo4e-0.4.8/json_schemas/com/Fremdkostenblock.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -734,8 +734,8 @@
 00002dd0: 2020 207d 2c0a 2020 2020 2272 6571 7569     },.    "requi
 00002de0: 7265 6422 3a20 5b0a 2020 2020 2020 2020  red": [.        
 00002df0: 226b 6f73 7465 6e62 6c6f 636b 6265 7a65  "kostenblockbeze
 00002e00: 6963 686e 756e 6722 0a20 2020 205d 2c0a  ichnung".    ],.
 00002e10: 2020 2020 2274 6974 6c65 223a 2022 4672      "title": "Fr
 00002e20: 656d 646b 6f73 7465 6e62 6c6f 636b 222c  emdkostenblock",
 00002e30: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00002e40: 6a65 6374 220a 7d0a                      ject".}.
+00002e40: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Fremdkostenposition.json` & `bo4e-0.4.8/json_schemas/com/Fremdkostenposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -641,8 +641,8 @@
 00002800: 696f 6e22 2c0a 2020 2020 2020 2020 2261  ion",.        "a
 00002810: 7274 696b 656c 6265 7a65 6963 686e 756e  rtikelbezeichnun
 00002820: 6722 2c0a 2020 2020 2020 2020 2265 696e  g",.        "ein
 00002830: 7a65 6c70 7265 6973 220a 2020 2020 5d2c  zelpreis".    ],
 00002840: 0a20 2020 2022 7469 746c 6522 3a20 2246  .    "title": "F
 00002850: 7265 6d64 6b6f 7374 656e 706f 7369 7469  remdkostenpositi
 00002860: 6f6e 222c 0a20 2020 2022 7479 7065 223a  on",.    "type":
-00002870: 2022 6f62 6a65 6374 220a 7d0a             "object".}.
+00002870: 2022 6f62 6a65 6374 220a 7d               "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Geokoordinaten.json` & `bo4e-0.4.8/json_schemas/com/Geokoordinaten.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 00000270: 2272 6571 7569 7265 6422 3a20 5b0a 2020  "required": [.  
 00000280: 2020 2020 2020 2262 7265 6974 656e 6772        "breitengr
 00000290: 6164 222c 0a20 2020 2020 2020 2022 6c61  ad",.        "la
 000002a0: 656e 6765 6e67 7261 6422 0a20 2020 205d  engengrad".    ]
 000002b0: 2c0a 2020 2020 2274 6974 6c65 223a 2022  ,.    "title": "
 000002c0: 4765 6f6b 6f6f 7264 696e 6174 656e 222c  Geokoordinaten",
 000002d0: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-000002e0: 6a65 6374 220a 7d0a                      ject".}.
+000002e0: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Geraet.json` & `bo4e-0.4.8/json_schemas/com/Geraet.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -300,8 +300,8 @@
 000012b0: 2020 2020 2020 2020 2020 2274 6974 6c65            "title
 000012c0: 223a 2022 4765 7261 6574 656e 756d 6d65  ": "Geraetenumme
 000012d0: 7222 2c0a 2020 2020 2020 2020 2020 2020  r",.            
 000012e0: 2274 7970 6522 3a20 2273 7472 696e 6722  "type": "string"
 000012f0: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
 00001300: 2c0a 2020 2020 2274 6974 6c65 223a 2022  ,.    "title": "
 00001310: 4765 7261 6574 222c 0a20 2020 2022 7479  Geraet",.    "ty
-00001320: 7065 223a 2022 6f62 6a65 6374 220a 7d0a  pe": "object".}.
+00001320: 7065 223a 2022 6f62 6a65 6374 220a 7d    pe": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Geraeteeigenschaften.json` & `bo4e-0.4.8/json_schemas/com/Geraeteeigenschaften.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -249,8 +249,8 @@
 00000f80: 7022 0a20 2020 2020 2020 207d 0a20 2020  p".        }.   
 00000f90: 207d 2c0a 2020 2020 2272 6571 7569 7265   },.    "require
 00000fa0: 6422 3a20 5b0a 2020 2020 2020 2020 2267  d": [.        "g
 00000fb0: 6572 6165 7465 7479 7022 0a20 2020 205d  eraetetyp".    ]
 00000fc0: 2c0a 2020 2020 2274 6974 6c65 223a 2022  ,.    "title": "
 00000fd0: 4765 7261 6574 6565 6967 656e 7363 6861  Geraeteeigenscha
 00000fe0: 6674 656e 222c 0a20 2020 2022 7479 7065  ften",.    "type
-00000ff0: 223a 2022 6f62 6a65 6374 220a 7d0a       ": "object".}.
+00000ff0: 223a 2022 6f62 6a65 6374 220a 7d         ": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Hardware.json` & `bo4e-0.4.8/json_schemas/com/Hardware.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -159,8 +159,8 @@
 000009e0: 207d 2c0a 2020 2020 2272 6571 7569 7265   },.    "require
 000009f0: 6422 3a20 5b0a 2020 2020 2020 2020 2267  d": [.        "g
 00000a00: 6572 6165 7465 7479 7022 2c0a 2020 2020  eraetetyp",.    
 00000a10: 2020 2020 2262 657a 6569 6368 6e75 6e67      "bezeichnung
 00000a20: 220a 2020 2020 5d2c 0a20 2020 2022 7469  ".    ],.    "ti
 00000a30: 746c 6522 3a20 2248 6172 6477 6172 6522  tle": "Hardware"
 00000a40: 2c0a 2020 2020 2274 7970 6522 3a20 226f  ,.    "type": "o
-00000a50: 626a 6563 7422 0a7d 0a                   bject".}.
+00000a50: 626a 6563 7422 0a7d                      bject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Katasteradresse.json` & `bo4e-0.4.8/json_schemas/com/Katasteradresse.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 00000270: 0a20 2020 2022 7265 7175 6972 6564 223a  .    "required":
 00000280: 205b 0a20 2020 2020 2020 2022 6765 6d61   [.        "gema
 00000290: 726b 756e 6746 6c75 7222 2c0a 2020 2020  rkungFlur",.    
 000002a0: 2020 2020 2266 6c75 7273 7475 6563 6b22      "flurstueck"
 000002b0: 0a20 2020 205d 2c0a 2020 2020 2274 6974  .    ],.    "tit
 000002c0: 6c65 223a 2022 4b61 7461 7374 6572 6164  le": "Katasterad
 000002d0: 7265 7373 6522 2c0a 2020 2020 2274 7970  resse",.    "typ
-000002e0: 6522 3a20 226f 626a 6563 7422 0a7d 0a    e": "object".}.
+000002e0: 6522 3a20 226f 626a 6563 7422 0a7d       e": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Kostenblock.json` & `bo4e-0.4.8/json_schemas/com/Kostenblock.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -699,8 +699,8 @@
 00002ba0: 2020 7d2c 0a20 2020 2022 7265 7175 6972    },.    "requir
 00002bb0: 6564 223a 205b 0a20 2020 2020 2020 2022  ed": [.        "
 00002bc0: 6b6f 7374 656e 626c 6f63 6b62 657a 6569  kostenblockbezei
 00002bd0: 6368 6e75 6e67 220a 2020 2020 5d2c 0a20  chnung".    ],. 
 00002be0: 2020 2022 7469 746c 6522 3a20 224b 6f73     "title": "Kos
 00002bf0: 7465 6e62 6c6f 636b 222c 0a20 2020 2022  tenblock",.    "
 00002c00: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-00002c10: 7d0a                                     }.
+00002c10: 7d                                       }
```

### Comparing `bo4e-0.4.7/json_schemas/com/Kostenposition.json` & `bo4e-0.4.8/json_schemas/com/Kostenposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -615,8 +615,8 @@
 00002660: 706f 7369 7469 6f6e 222c 0a20 2020 2020  position",.     
 00002670: 2020 2022 6172 7469 6b65 6c62 657a 6569     "artikelbezei
 00002680: 6368 6e75 6e67 222c 0a20 2020 2020 2020  chnung",.       
 00002690: 2022 6569 6e7a 656c 7072 6569 7322 0a20   "einzelpreis". 
 000026a0: 2020 205d 2c0a 2020 2020 2274 6974 6c65     ],.    "title
 000026b0: 223a 2022 4b6f 7374 656e 706f 7369 7469  ": "Kostenpositi
 000026c0: 6f6e 222c 0a20 2020 2022 7479 7065 223a  on",.    "type":
-000026d0: 2022 6f62 6a65 6374 220a 7d0a             "object".}.
+000026d0: 2022 6f62 6a65 6374 220a 7d               "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/KriteriumWert.json` & `bo4e-0.4.8/json_schemas/com/KriteriumWert.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 00000410: 2020 2020 2272 6571 7569 7265 6422 3a20      "required": 
 00000420: 5b0a 2020 2020 2020 2020 226b 7269 7465  [.        "krite
 00000430: 7269 756d 222c 0a20 2020 2020 2020 2022  rium",.        "
 00000440: 7765 7274 220a 2020 2020 5d2c 0a20 2020  wert".    ],.   
 00000450: 2022 7469 746c 6522 3a20 224b 7269 7465   "title": "Krite
 00000460: 7269 756d 5765 7274 222c 0a20 2020 2022  riumWert",.    "
 00000470: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-00000480: 7d0a                                     }.
+00000480: 7d                                       }
```

### Comparing `bo4e-0.4.7/json_schemas/com/MarktgebietInfo.json` & `bo4e-0.4.8/json_schemas/com/MarktgebietInfo.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 00000270: 205b 0a20 2020 2020 2020 2022 6d61 726b   [.        "mark
 00000280: 7467 6562 6965 7422 2c0a 2020 2020 2020  tgebiet",.      
 00000290: 2020 226d 6172 6b74 6765 6269 6574 636f    "marktgebietco
 000002a0: 6465 220a 2020 2020 5d2c 0a20 2020 2022  de".    ],.    "
 000002b0: 7469 746c 6522 3a20 224d 6172 6b74 6765  title": "Marktge
 000002c0: 6269 6574 496e 666f 222c 0a20 2020 2022  bietInfo",.    "
 000002d0: 7479 7065 223a 2022 6f62 6a65 6374 220a  type": "object".
-000002e0: 7d0a                                     }.
+000002e0: 7d                                       }
```

### Comparing `bo4e-0.4.7/json_schemas/com/Menge.json` & `bo4e-0.4.8/json_schemas/com/Menge.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -72,8 +72,8 @@
 00000470: 6d62 6572 220a 2020 2020 2020 2020 7d0a  mber".        }.
 00000480: 2020 2020 7d2c 0a20 2020 2022 7265 7175      },.    "requ
 00000490: 6972 6564 223a 205b 0a20 2020 2020 2020  ired": [.       
 000004a0: 2022 7765 7274 222c 0a20 2020 2020 2020   "wert",.       
 000004b0: 2022 6569 6e68 6569 7422 0a20 2020 205d   "einheit".    ]
 000004c0: 2c0a 2020 2020 2274 6974 6c65 223a 2022  ,.    "title": "
 000004d0: 4d65 6e67 6522 2c0a 2020 2020 2274 7970  Menge",.    "typ
-000004e0: 6522 3a20 226f 626a 6563 7422 0a7d 0a    e": "object".}.
+000004e0: 6522 3a20 226f 626a 6563 7422 0a7d       e": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Messlokationszuordnung.json` & `bo4e-0.4.8/json_schemas/com/Messlokationszuordnung.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,8 @@
 00000600: 205b 0a20 2020 2020 2020 2022 6d65 7373   [.        "mess
 00000610: 6c6f 6b61 7469 6f6e 7349 6422 2c0a 2020  lokationsId",.  
 00000620: 2020 2020 2020 2261 7269 7468 6d65 7469        "arithmeti
 00000630: 6b22 0a20 2020 205d 2c0a 2020 2020 2274  k".    ],.    "t
 00000640: 6974 6c65 223a 2022 4d65 7373 6c6f 6b61  itle": "Messloka
 00000650: 7469 6f6e 737a 756f 7264 6e75 6e67 222c  tionszuordnung",
 00000660: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00000670: 6a65 6374 220a 7d0a                      ject".}.
+00000670: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/PositionsAufAbschlag.json` & `bo4e-0.4.8/json_schemas/com/PositionsAufAbschlag.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,8 @@
 00000790: 2020 2020 2020 2022 6175 6641 6273 6368         "aufAbsch
 000007a0: 6c61 6773 7765 7274 222c 0a20 2020 2020  lagswert",.     
 000007b0: 2020 2022 6175 6641 6273 6368 6c61 6773     "aufAbschlags
 000007c0: 7761 6568 7275 6e67 220a 2020 2020 5d2c  waehrung".    ],
 000007d0: 0a20 2020 2022 7469 746c 6522 3a20 2250  .    "title": "P
 000007e0: 6f73 6974 696f 6e73 4175 6641 6273 6368  ositionsAufAbsch
 000007f0: 6c61 6722 2c0a 2020 2020 2274 7970 6522  lag",.    "type"
-00000800: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+00000800: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Preis.json` & `bo4e-0.4.8/json_schemas/com/Preis.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -123,8 +123,8 @@
 000007a0: 6571 7569 7265 6422 3a20 5b0a 2020 2020  equired": [.    
 000007b0: 2020 2020 2277 6572 7422 2c0a 2020 2020      "wert",.    
 000007c0: 2020 2020 2265 696e 6865 6974 222c 0a20      "einheit",. 
 000007d0: 2020 2020 2020 2022 6265 7a75 6773 7765         "bezugswe
 000007e0: 7274 220a 2020 2020 5d2c 0a20 2020 2022  rt".    ],.    "
 000007f0: 7469 746c 6522 3a20 2250 7265 6973 222c  title": "Preis",
 00000800: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00000810: 6a65 6374 220a 7d0a                      ject".}.
+00000810: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Preisgarantie.json` & `bo4e-0.4.8/json_schemas/com/Preisgarantie.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 4% similar despite different names*

```diff
@@ -215,8 +215,8 @@
 00000d60: 2020 2020 2270 7265 6973 6761 7261 6e74      "preisgarant
 00000d70: 6965 7479 7022 2c0a 2020 2020 2020 2020  ietyp",.        
 00000d80: 227a 6569 746c 6963 6865 4775 656c 7469  "zeitlicheGuelti
 00000d90: 676b 6569 7422 0a20 2020 205d 2c0a 2020  gkeit".    ],.  
 00000da0: 2020 2274 6974 6c65 223a 2022 5072 6569    "title": "Prei
 00000db0: 7367 6172 616e 7469 6522 2c0a 2020 2020  sgarantie",.    
 00000dc0: 2274 7970 6522 3a20 226f 626a 6563 7422  "type": "object"
-00000dd0: 0a7d 0a                                  .}.
+00000dd0: 0a7d                                     .}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Preisposition.json` & `bo4e-0.4.8/json_schemas/com/Preisposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -697,8 +697,8 @@
 00002b80: 2270 7265 6973 6569 6e68 6569 7422 2c0a  "preiseinheit",.
 00002b90: 2020 2020 2020 2020 2262 657a 7567 7367          "bezugsg
 00002ba0: 726f 6573 7365 222c 0a20 2020 2020 2020  roesse",.       
 00002bb0: 2022 7072 6569 7373 7461 6666 656c 6e22   "preisstaffeln"
 00002bc0: 0a20 2020 205d 2c0a 2020 2020 2274 6974  .    ],.    "tit
 00002bd0: 6c65 223a 2022 5072 6569 7370 6f73 6974  le": "Preisposit
 00002be0: 696f 6e22 2c0a 2020 2020 2274 7970 6522  ion",.    "type"
-00002bf0: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+00002bf0: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Preisstaffel.json` & `bo4e-0.4.8/json_schemas/com/Preisstaffel.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,8 @@
 00000810: 7473 7072 6569 7322 2c0a 2020 2020 2020  tspreis",.      
 00000820: 2020 2273 7461 6666 656c 6772 656e 7a65    "staffelgrenze
 00000830: 566f 6e22 2c0a 2020 2020 2020 2020 2273  Von",.        "s
 00000840: 7461 6666 656c 6772 656e 7a65 4269 7322  taffelgrenzeBis"
 00000850: 0a20 2020 205d 2c0a 2020 2020 2274 6974  .    ],.    "tit
 00000860: 6c65 223a 2022 5072 6569 7373 7461 6666  le": "Preisstaff
 00000870: 656c 222c 0a20 2020 2022 7479 7065 223a  el",.    "type":
-00000880: 2022 6f62 6a65 6374 220a 7d0a             "object".}.
+00000880: 2022 6f62 6a65 6374 220a 7d               "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Rechnungsposition.json` & `bo4e-0.4.8/json_schemas/com/Rechnungsposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -912,8 +912,8 @@
 000038f0: 222c 0a20 2020 2020 2020 2022 7465 696c  ",.        "teil
 00003900: 7375 6d6d 654e 6574 746f 222c 0a20 2020  summeNetto",.   
 00003910: 2020 2020 2022 7465 696c 7375 6d6d 6553       "teilsummeS
 00003920: 7465 7565 7222 0a20 2020 205d 2c0a 2020  teuer".    ],.  
 00003930: 2020 2274 6974 6c65 223a 2022 5265 6368    "title": "Rech
 00003940: 6e75 6e67 7370 6f73 6974 696f 6e22 2c0a  nungsposition",.
 00003950: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00003960: 6563 7422 0a7d 0a                        ect".}.
+00003960: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/RegionaleGueltigkeit.json` & `bo4e-0.4.8/json_schemas/com/RegionaleGueltigkeit.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -158,8 +158,8 @@
 000009d0: 2020 2020 2020 2022 6775 656c 7469 676b         "gueltigk
 000009e0: 6569 7473 7479 7022 2c0a 2020 2020 2020  eitstyp",.      
 000009f0: 2020 226b 7269 7465 7269 756d 7357 6572    "kriteriumsWer
 00000a00: 7465 220a 2020 2020 5d2c 0a20 2020 2022  te".    ],.    "
 00000a10: 7469 746c 6522 3a20 2252 6567 696f 6e61  title": "Regiona
 00000a20: 6c65 4775 656c 7469 676b 6569 7422 2c0a  leGueltigkeit",.
 00000a30: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000a40: 6563 7422 0a7d 0a                        ect".}.
+00000a40: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/RegionalePreisgarantie.json` & `bo4e-0.4.8/json_schemas/com/RegionalePreisgarantie.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,8 @@
 000018e0: 6368 6547 7565 6c74 6967 6b65 6974 222c  cheGueltigkeit",
 000018f0: 0a20 2020 2020 2020 2022 7265 6769 6f6e  .        "region
 00001900: 616c 6547 7565 6c74 6967 6b65 6974 220a  aleGueltigkeit".
 00001910: 2020 2020 5d2c 0a20 2020 2022 7469 746c      ],.    "titl
 00001920: 6522 3a20 2252 6567 696f 6e61 6c65 5072  e": "RegionalePr
 00001930: 6569 7367 6172 616e 7469 6522 2c0a 2020  eisgarantie",.  
 00001940: 2020 2274 7970 6522 3a20 226f 626a 6563    "type": "objec
-00001950: 7422 0a7d 0a                             t".}.
+00001950: 7422 0a7d                                t".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/RegionalePreisstaffel.json` & `bo4e-0.4.8/json_schemas/com/RegionalePreisstaffel.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -317,8 +317,7 @@
 000013c0: 656c 6772 656e 7a65 4269 7322 2c0a 2020  elgrenzeBis",.  
 000013d0: 2020 2020 2020 2272 6567 696f 6e61 6c65        "regionale
 000013e0: 4775 656c 7469 676b 6569 7422 0a20 2020  Gueltigkeit".   
 000013f0: 205d 2c0a 2020 2020 2274 6974 6c65 223a   ],.    "title":
 00001400: 2022 5265 6769 6f6e 616c 6550 7265 6973   "RegionalePreis
 00001410: 7374 6166 6665 6c22 2c0a 2020 2020 2274  staffel",.    "t
 00001420: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-00001430: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/RegionaleTarifpreisposition.json` & `bo4e-0.4.8/json_schemas/com/RegionaleTarifpreisposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -506,8 +506,8 @@
 00001f90: 2022 6265 7a75 6773 6569 6e68 6569 7422   "bezugseinheit"
 00001fa0: 2c0a 2020 2020 2020 2020 2270 7265 6973  ,.        "preis
 00001fb0: 7374 6166 6665 6c6e 220a 2020 2020 5d2c  staffeln".    ],
 00001fc0: 0a20 2020 2022 7469 746c 6522 3a20 2252  .    "title": "R
 00001fd0: 6567 696f 6e61 6c65 5461 7269 6670 7265  egionaleTarifpre
 00001fe0: 6973 706f 7369 7469 6f6e 222c 0a20 2020  isposition",.   
 00001ff0: 2022 7479 7065 223a 2022 6f62 6a65 6374   "type": "object
-00002000: 220a 7d0a                                ".}.
+00002000: 220a 7d                                  ".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/RegionalerAufAbschlag.json` & `bo4e-0.4.8/json_schemas/com/RegionalerAufAbschlag.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -1858,8 +1858,8 @@
 00007410: 6972 6564 223a 205b 0a20 2020 2020 2020  ired": [.       
 00007420: 2022 6265 7a65 6963 686e 756e 6722 2c0a   "bezeichnung",.
 00007430: 2020 2020 2020 2020 2273 7461 6666 656c          "staffel
 00007440: 6e22 0a20 2020 205d 2c0a 2020 2020 2274  n".    ],.    "t
 00007450: 6974 6c65 223a 2022 5265 6769 6f6e 616c  itle": "Regional
 00007460: 6572 4175 6641 6273 6368 6c61 6722 2c0a  erAufAbschlag",.
 00007470: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00007480: 6563 7422 0a7d 0a                        ect".}.
+00007480: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Regionskriterium.json` & `bo4e-0.4.8/json_schemas/com/Regionskriterium.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -161,8 +161,8 @@
 00000a00: 6b65 6974 7374 7970 222c 0a20 2020 2020  keitstyp",.     
 00000a10: 2020 2022 7265 6769 6f6e 736b 7269 7465     "regionskrite
 00000a20: 7269 756d 7479 7022 2c0a 2020 2020 2020  riumtyp",.      
 00000a30: 2020 2277 6572 7422 0a20 2020 205d 2c0a    "wert".    ],.
 00000a40: 2020 2020 2274 6974 6c65 223a 2022 5265      "title": "Re
 00000a50: 6769 6f6e 736b 7269 7465 7269 756d 222c  gionskriterium",
 00000a60: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00000a70: 6a65 6374 220a 7d0a                      ject".}.
+00000a70: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Rufnummer.json` & `bo4e-0.4.8/json_schemas/com/Rufnummer.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,8 @@
 00000440: 207d 2c0a 2020 2020 2272 6571 7569 7265   },.    "require
 00000450: 6422 3a20 5b0a 2020 2020 2020 2020 226e  d": [.        "n
 00000460: 756d 6d65 726e 7479 7022 2c0a 2020 2020  ummerntyp",.    
 00000470: 2020 2020 2272 7566 6e75 6d6d 6572 220a      "rufnummer".
 00000480: 2020 2020 5d2c 0a20 2020 2022 7469 746c      ],.    "titl
 00000490: 6522 3a20 2252 7566 6e75 6d6d 6572 222c  e": "Rufnummer",
 000004a0: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-000004b0: 6a65 6374 220a 7d0a                      ject".}.
+000004b0: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Sigmoidparameter.json` & `bo4e-0.4.8/json_schemas/com/Sigmoidparameter.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,7 @@
 00000330: 2020 2020 2020 2022 4122 2c0a 2020 2020         "A",.    
 00000340: 2020 2020 2242 222c 0a20 2020 2020 2020      "B",.       
 00000350: 2022 4322 2c0a 2020 2020 2020 2020 2244   "C",.        "D
 00000360: 220a 2020 2020 5d2c 0a20 2020 2022 7469  ".    ],.    "ti
 00000370: 746c 6522 3a20 2253 6967 6d6f 6964 7061  tle": "Sigmoidpa
 00000380: 7261 6d65 7465 7222 2c0a 2020 2020 2274  rameter",.    "t
 00000390: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-000003a0: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/StandorteigenschaftenAllgemein.json` & `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenAllgemein.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/json_schemas/com/StandorteigenschaftenGas.json` & `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenGas.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,8 @@
 00000710: 205b 0a20 2020 2020 2020 2022 6e65 747a   [.        "netz
 00000720: 6b6f 6e74 6f6e 756d 6d65 726e 222c 0a20  kontonummern",. 
 00000730: 2020 2020 2020 2022 6d61 726b 7467 6562         "marktgeb
 00000740: 6965 7465 220a 2020 2020 5d2c 0a20 2020  iete".    ],.   
 00000750: 2022 7469 746c 6522 3a20 2253 7461 6e64   "title": "Stand
 00000760: 6f72 7465 6967 656e 7363 6861 6674 656e  orteigenschaften
 00000770: 4761 7322 2c0a 2020 2020 2274 7970 6522  Gas",.    "type"
-00000780: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+00000780: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/StandorteigenschaftenStrom.json` & `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenStrom.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 00000320: 6574 4569 6322 2c0a 2020 2020 2020 2020  etEic",.        
 00000330: 2272 6567 656c 7a6f 6e65 222c 0a20 2020  "regelzone",.   
 00000340: 2020 2020 2022 7265 6765 6c7a 6f6e 6545       "regelzoneE
 00000350: 6963 220a 2020 2020 5d2c 0a20 2020 2022  ic".    ],.    "
 00000360: 7469 746c 6522 3a20 2253 7461 6e64 6f72  title": "Standor
 00000370: 7465 6967 656e 7363 6861 6674 656e 5374  teigenschaftenSt
 00000380: 726f 6d22 2c0a 2020 2020 2274 7970 6522  rom",.    "type"
-00000390: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+00000390: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Steuerbetrag.json` & `bo4e-0.4.8/json_schemas/com/Steuerbetrag.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -355,8 +355,8 @@
 00001620: 2020 2020 2020 2262 6173 6973 7765 7274        "basiswert
 00001630: 222c 0a20 2020 2020 2020 2022 7374 6575  ",.        "steu
 00001640: 6572 7765 7274 222c 0a20 2020 2020 2020  erwert",.       
 00001650: 2022 7761 6568 7275 6e67 220a 2020 2020   "waehrung".    
 00001660: 5d2c 0a20 2020 2022 7469 746c 6522 3a20  ],.    "title": 
 00001670: 2253 7465 7565 7262 6574 7261 6722 2c0a  "Steuerbetrag",.
 00001680: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00001690: 6563 7422 0a7d 0a                        ect".}.
+00001690: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Tagesvektor.json` & `bo4e-0.4.8/json_schemas/com/Tagesvektor.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -277,8 +277,7 @@
 00001140: 2020 207d 2c0a 2020 2020 2272 6571 7569     },.    "requi
 00001150: 7265 6422 3a20 5b0a 2020 2020 2020 2020  red": [.        
 00001160: 2274 6167 222c 0a20 2020 2020 2020 2022  "tag",.        "
 00001170: 7765 7274 6522 0a20 2020 205d 2c0a 2020  werte".    ],.  
 00001180: 2020 2274 6974 6c65 223a 2022 5461 6765    "title": "Tage
 00001190: 7376 656b 746f 7222 2c0a 2020 2020 2274  svektor",.    "t
 000011a0: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-000011b0: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/Tarifberechnungsparameter.json` & `bo4e-0.4.8/json_schemas/com/Tarifberechnungsparameter.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -460,8 +460,8 @@
 00001cb0: 225a 7573 6174 7a70 7265 6973 6522 2c0a  "Zusatzpreise",.
 00001cc0: 2020 2020 2020 2020 2020 2020 2274 7970              "typ
 00001cd0: 6522 3a20 2261 7272 6179 220a 2020 2020  e": "array".    
 00001ce0: 2020 2020 7d0a 2020 2020 7d2c 0a20 2020      }.    },.   
 00001cf0: 2022 7469 746c 6522 3a20 2254 6172 6966   "title": "Tarif
 00001d00: 6265 7265 6368 6e75 6e67 7370 6172 616d  berechnungsparam
 00001d10: 6574 6572 222c 0a20 2020 2022 7479 7065  eter",.    "type
-00001d20: 223a 2022 6f62 6a65 6374 220a 7d0a       ": "object".}.
+00001d20: 223a 2022 6f62 6a65 6374 220a 7d         ": "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Tarifeinschraenkung.json` & `bo4e-0.4.8/json_schemas/com/Tarifeinschraenkung.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 1% similar despite different names*

```diff
@@ -585,8 +585,8 @@
 00002480: 5a75 7361 747a 7072 6f64 756b 7465 222c  Zusatzprodukte",
 00002490: 0a20 2020 2020 2020 2020 2020 2022 7479  .            "ty
 000024a0: 7065 223a 2022 6172 7261 7922 0a20 2020  pe": "array".   
 000024b0: 2020 2020 207d 0a20 2020 207d 2c0a 2020       }.    },.  
 000024c0: 2020 2274 6974 6c65 223a 2022 5461 7269    "title": "Tari
 000024d0: 6665 696e 7363 6872 6165 6e6b 756e 6722  feinschraenkung"
 000024e0: 2c0a 2020 2020 2274 7970 6522 3a20 226f  ,.    "type": "o
-000024f0: 626a 6563 7422 0a7d 0a                   bject".}.
+000024f0: 626a 6563 7422 0a7d                      bject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Tarifpreis.json` & `bo4e-0.4.8/json_schemas/com/Tarifpreis.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -172,8 +172,8 @@
 00000ab0: 2c0a 2020 2020 2020 2020 2265 696e 6865  ,.        "einhe
 00000ac0: 6974 222c 0a20 2020 2020 2020 2022 6265  it",.        "be
 00000ad0: 7a75 6773 7765 7274 222c 0a20 2020 2020  zugswert",.     
 00000ae0: 2020 2022 7072 6569 7374 7970 220a 2020     "preistyp".  
 00000af0: 2020 5d2c 0a20 2020 2022 7469 746c 6522    ],.    "title"
 00000b00: 3a20 2254 6172 6966 7072 6569 7322 2c0a  : "Tarifpreis",.
 00000b10: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000b20: 6563 7422 0a7d 0a                        ect".}.
+00000b20: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Tarifpreisposition.json` & `bo4e-0.4.8/json_schemas/com/Tarifpreisposition.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -311,8 +311,8 @@
 00001360: 696e 6865 6974 222c 0a20 2020 2020 2020  inheit",.       
 00001370: 2022 6265 7a75 6773 6569 6e68 6569 7422   "bezugseinheit"
 00001380: 2c0a 2020 2020 2020 2020 2270 7265 6973  ,.        "preis
 00001390: 7374 6166 6665 6c6e 220a 2020 2020 5d2c  staffeln".    ],
 000013a0: 0a20 2020 2022 7469 746c 6522 3a20 2254  .    "title": "T
 000013b0: 6172 6966 7072 6569 7370 6f73 6974 696f  arifpreispositio
 000013c0: 6e22 2c0a 2020 2020 2274 7970 6522 3a20  n",.    "type": 
-000013d0: 226f 626a 6563 7422 0a7d 0a              "object".}.
+000013d0: 226f 626a 6563 7422 0a7d                 "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/TarifpreispositionProOrt.json` & `bo4e-0.4.8/json_schemas/com/TarifpreispositionProOrt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -162,8 +162,8 @@
 00000a10: 222c 0a20 2020 2020 2020 2022 6e65 747a  ",.        "netz
 00000a20: 6e72 222c 0a20 2020 2020 2020 2022 7072  nr",.        "pr
 00000a30: 6569 7373 7461 6666 656c 6e22 0a20 2020  eisstaffeln".   
 00000a40: 205d 2c0a 2020 2020 2274 6974 6c65 223a   ],.    "title":
 00000a50: 2022 5461 7269 6670 7265 6973 706f 7369   "Tarifpreisposi
 00000a60: 7469 6f6e 5072 6f4f 7274 222c 0a20 2020  tionProOrt",.   
 00000a70: 2022 7479 7065 223a 2022 6f62 6a65 6374   "type": "object
-00000a80: 220a 7d0a                                ".}.
+00000a80: 220a 7d                                  ".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/TarifpreisstaffelProOrt.json` & `bo4e-0.4.8/json_schemas/com/TarifpreisstaffelProOrt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
 00000420: 2020 2020 2020 2022 7374 6166 6665 6c67         "staffelg
 00000430: 7265 6e7a 6556 6f6e 222c 0a20 2020 2020  renzeVon",.     
 00000440: 2020 2022 7374 6166 6665 6c67 7265 6e7a     "staffelgrenz
 00000450: 6542 6973 220a 2020 2020 5d2c 0a20 2020  eBis".    ],.   
 00000460: 2022 7469 746c 6522 3a20 2254 6172 6966   "title": "Tarif
 00000470: 7072 6569 7373 7461 6666 656c 5072 6f4f  preisstaffelProO
 00000480: 7274 222c 0a20 2020 2022 7479 7065 223a  rt",.    "type":
-00000490: 2022 6f62 6a65 6374 220a 7d0a             "object".}.
+00000490: 2022 6f62 6a65 6374 220a 7d               "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Unterschrift.json` & `bo4e-0.4.8/json_schemas/com/Unterschrift.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -44,8 +44,8 @@
 000002b0: 3a20 2273 7472 696e 6722 0a20 2020 2020  : "string".     
 000002c0: 2020 207d 0a20 2020 207d 2c0a 2020 2020     }.    },.    
 000002d0: 2272 6571 7569 7265 6422 3a20 5b0a 2020  "required": [.  
 000002e0: 2020 2020 2020 226e 616d 6522 0a20 2020        "name".   
 000002f0: 205d 2c0a 2020 2020 2274 6974 6c65 223a   ],.    "title":
 00000300: 2022 556e 7465 7273 6368 7269 6674 222c   "Unterschrift",
 00000310: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00000320: 6a65 6374 220a 7d0a                      ject".}.
+00000320: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Verbrauch.json` & `bo4e-0.4.8/json_schemas/com/Verbrauch.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -141,8 +141,8 @@
 000008c0: 7265 6e22 2c0a 2020 2020 2020 2020 226f  ren",.        "o
 000008d0: 6269 734b 656e 6e7a 6168 6c22 2c0a 2020  bisKennzahl",.  
 000008e0: 2020 2020 2020 2277 6572 7422 2c0a 2020        "wert",.  
 000008f0: 2020 2020 2020 2265 696e 6865 6974 220a        "einheit".
 00000900: 2020 2020 5d2c 0a20 2020 2022 7469 746c      ],.    "titl
 00000910: 6522 3a20 2256 6572 6272 6175 6368 222c  e": "Verbrauch",
 00000920: 0a20 2020 2022 7479 7065 223a 2022 6f62  .    "type": "ob
-00000930: 6a65 6374 220a 7d0a                      ject".}.
+00000930: 6a65 6374 220a 7d                        ject".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Vertragskonditionen.json` & `bo4e-0.4.8/json_schemas/com/Vertragskonditionen.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -203,8 +203,7 @@
 00000ca0: 2020 2020 2224 7265 6622 3a20 2223 2f64      "$ref": "#/d
 00000cb0: 6566 696e 6974 696f 6e73 2f5a 6569 7472  efinitions/Zeitr
 00000cc0: 6175 6d22 0a20 2020 2020 2020 207d 0a20  aum".        }. 
 00000cd0: 2020 207d 2c0a 2020 2020 2274 6974 6c65     },.    "title
 00000ce0: 223a 2022 5665 7274 7261 6773 6b6f 6e64  ": "Vertragskond
 00000cf0: 6974 696f 6e65 6e22 2c0a 2020 2020 2274  itionen",.    "t
 00000d00: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-00000d10: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/Vertragsteil.json` & `bo4e-0.4.8/json_schemas/com/Vertragsteil.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -164,8 +164,8 @@
 00000a30: 205b 0a20 2020 2020 2020 2022 7665 7274   [.        "vert
 00000a40: 7261 6773 7465 696c 6265 6769 6e6e 222c  ragsteilbeginn",
 00000a50: 0a20 2020 2020 2020 2022 7665 7274 7261  .        "vertra
 00000a60: 6773 7465 696c 656e 6465 220a 2020 2020  gsteilende".    
 00000a70: 5d2c 0a20 2020 2022 7469 746c 6522 3a20  ],.    "title": 
 00000a80: 2256 6572 7472 6167 7374 6569 6c22 2c0a  "Vertragsteil",.
 00000a90: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000aa0: 6563 7422 0a7d 0a                        ect".}.
+00000aa0: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zaehlwerk.json` & `bo4e-0.4.8/json_schemas/com/Zaehlwerk.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
 00000860: 2c0a 2020 2020 2020 2020 226f 6269 734b  ,.        "obisK
 00000870: 656e 6e7a 6168 6c22 2c0a 2020 2020 2020  ennzahl",.      
 00000880: 2020 2277 616e 646c 6572 6661 6b74 6f72    "wandlerfaktor
 00000890: 222c 0a20 2020 2020 2020 2022 6569 6e68  ",.        "einh
 000008a0: 6569 7422 0a20 2020 205d 2c0a 2020 2020  eit".    ],.    
 000008b0: 2274 6974 6c65 223a 2022 5a61 6568 6c77  "title": "Zaehlw
 000008c0: 6572 6b22 2c0a 2020 2020 2274 7970 6522  erk",.    "type"
-000008d0: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+000008d0: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zeitintervall.json` & `bo4e-0.4.8/json_schemas/com/Zeitintervall.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,7 @@
 000004d0: 2022 7265 7175 6972 6564 223a 205b 0a20   "required": [. 
 000004e0: 2020 2020 2020 2022 7765 7274 222c 0a20         "wert",. 
 000004f0: 2020 2020 2020 2022 7a65 6974 6569 6e68         "zeiteinh
 00000500: 6569 7422 0a20 2020 205d 2c0a 2020 2020  eit".    ],.    
 00000510: 2274 6974 6c65 223a 2022 5a65 6974 696e  "title": "Zeitin
 00000520: 7465 7276 616c 6c22 2c0a 2020 2020 2274  tervall",.    "t
 00000530: 7970 6522 3a20 226f 626a 6563 7422 0a7d  ype": "object".}
-00000540: 0a                                       .
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zeitraum.json` & `bo4e-0.4.8/json_schemas/com/Zeitraum.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,8 @@
 00000730: 2020 2274 6974 6c65 223a 2022 5374 6172    "title": "Star
 00000740: 747a 6569 7470 756e 6b74 222c 0a20 2020  tzeitpunkt",.   
 00000750: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
 00000760: 2022 7374 7269 6e67 220a 2020 2020 2020   "string".      
 00000770: 2020 7d0a 2020 2020 7d2c 0a20 2020 2022    }.    },.    "
 00000780: 7469 746c 6522 3a20 225a 6569 7472 6175  title": "Zeitrau
 00000790: 6d22 2c0a 2020 2020 2274 7970 6522 3a20  m",.    "type": 
-000007a0: 226f 626a 6563 7422 0a7d 0a              "object".}.
+000007a0: 226f 626a 6563 7422 0a7d                 "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zeitreihenwert.json` & `bo4e-0.4.8/json_schemas/com/Zeitreihenwert.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -229,8 +229,8 @@
 00000e40: 2020 2022 7765 7274 222c 0a20 2020 2020     "wert",.     
 00000e50: 2020 2022 6461 7475 6d55 6872 7a65 6974     "datumUhrzeit
 00000e60: 566f 6e22 2c0a 2020 2020 2020 2020 2264  Von",.        "d
 00000e70: 6174 756d 5568 727a 6569 7442 6973 220a  atumUhrzeitBis".
 00000e80: 2020 2020 5d2c 0a20 2020 2022 7469 746c      ],.    "titl
 00000e90: 6522 3a20 225a 6569 7472 6569 6865 6e77  e": "Zeitreihenw
 00000ea0: 6572 7422 2c0a 2020 2020 2274 7970 6522  ert",.    "type"
-00000eb0: 3a20 226f 626a 6563 7422 0a7d 0a         : "object".}.
+00000eb0: 3a20 226f 626a 6563 7422 0a7d            : "object".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zeitreihenwertkompakt.json` & `bo4e-0.4.8/json_schemas/com/Zeitreihenwertkompakt.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -211,8 +211,8 @@
 00000d20: 0a20 2020 2020 2020 207d 0a20 2020 207d  .        }.    }
 00000d30: 2c0a 2020 2020 2272 6571 7569 7265 6422  ,.    "required"
 00000d40: 3a20 5b0a 2020 2020 2020 2020 2277 6572  : [.        "wer
 00000d50: 7422 0a20 2020 205d 2c0a 2020 2020 2274  t".    ],.    "t
 00000d60: 6974 6c65 223a 2022 5a65 6974 7265 6968  itle": "Zeitreih
 00000d70: 656e 7765 7274 6b6f 6d70 616b 7422 2c0a  enwertkompakt",.
 00000d80: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000d90: 6563 7422 0a7d 0a                        ect".}.
+00000d90: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/com/Zustaendigkeit.json` & `bo4e-0.4.8/json_schemas/com/Zustaendigkeit.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 00000c10: 2020 2020 2020 2020 7d0a 2020 2020 7d2c          }.    },
 00000c20: 0a20 2020 2022 7265 7175 6972 6564 223a  .    "required":
 00000c30: 205b 0a20 2020 2020 2020 2022 7468 656d   [.        "them
 00000c40: 656e 6765 6269 6574 220a 2020 2020 5d2c  engebiet".    ],
 00000c50: 0a20 2020 2022 7469 746c 6522 3a20 225a  .    "title": "Z
 00000c60: 7573 7461 656e 6469 676b 6569 7422 2c0a  ustaendigkeit",.
 00000c70: 2020 2020 2274 7970 6522 3a20 226f 626a      "type": "obj
-00000c80: 6563 7422 0a7d 0a                        ect".}.
+00000c80: 6563 7422 0a7d                           ect".}
```

### Comparing `bo4e-0.4.7/json_schemas/generate_json_schemas.py` & `bo4e-0.4.8/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/pyproject.toml` & `bo4e-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/setup.cfg` & `bo4e-0.4.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 zip_safe = False
 packages = find:
 package_dir = = src
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	iso3166
-	pydantic
+	pydantic==1.*
 	pyhumps
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `bo4e-0.4.7/src/bo4e/bo/angebot.py` & `bo4e-0.4.8/src/bo4e/bo/angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/ansprechpartner.py` & `bo4e-0.4.8/src/bo4e/bo/ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/ausschreibung.py` & `bo4e-0.4.8/src/bo4e/bo/ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/buendelvertrag.py` & `bo4e-0.4.8/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/energiemenge.py` & `bo4e-0.4.8/src/bo4e/bo/energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/fremdkosten.py` & `bo4e-0.4.8/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-0.4.8/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/geschaeftspartner.py` & `bo4e-0.4.8/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/kosten.py` & `bo4e-0.4.8/src/bo4e/bo/kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/lastgang.py` & `bo4e-0.4.8/src/bo4e/bo/lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/marktlokation.py` & `bo4e-0.4.8/src/bo4e/bo/marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/marktteilnehmer.py` & `bo4e-0.4.8/src/bo4e/bo/marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/messlokation.py` & `bo4e-0.4.8/src/bo4e/bo/messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/netznutzungsrechnung.py` & `bo4e-0.4.8/src/bo4e/bo/netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblatt.py` & `bo4e-0.4.8/src/bo4e/bo/preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-0.4.8/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblatthardware.py` & `bo4e-0.4.8/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-0.4.8/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblattmessung.py` & `bo4e-0.4.8/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-0.4.8/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/rechnung.py` & `bo4e-0.4.8/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/region.py` & `bo4e-0.4.8/src/bo4e/bo/region.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/regionaltarif.py` & `bo4e-0.4.8/src/bo4e/bo/regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/standorteigenschaften.py` & `bo4e-0.4.8/src/bo4e/bo/standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/tarif.py` & `bo4e-0.4.8/src/bo4e/bo/tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/tarifinfo.py` & `bo4e-0.4.8/src/bo4e/bo/tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/tarifkosten.py` & `bo4e-0.4.8/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-0.4.8/src/bo4e/bo/tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/vertrag.py` & `bo4e-0.4.8/src/bo4e/bo/vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/zaehler.py` & `bo4e-0.4.8/src/bo4e/bo/zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/bo/zeitreihe.py` & `bo4e-0.4.8/src/bo4e/bo/zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/adresse.py` & `bo4e-0.4.8/src/bo4e/com/adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/angebotsposition.py` & `bo4e-0.4.8/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/angebotsteil.py` & `bo4e-0.4.8/src/bo4e/com/angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/angebotsvariante.py` & `bo4e-0.4.8/src/bo4e/com/angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/aufabschlag.py` & `bo4e-0.4.8/src/bo4e/com/aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/aufabschlagproort.py` & `bo4e-0.4.8/src/bo4e/com/aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/aufabschlagregional.py` & `bo4e-0.4.8/src/bo4e/com/aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-0.4.8/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-0.4.8/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/ausschreibungslos.py` & `bo4e-0.4.8/src/bo4e/com/ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/betrag.py` & `bo4e-0.4.8/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/com.py` & `bo4e-0.4.8/src/bo4e/com/com.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/dienstleistung.py` & `bo4e-0.4.8/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/energieherkunft.py` & `bo4e-0.4.8/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/energiemix.py` & `bo4e-0.4.8/src/bo4e/com/energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/externereferenz.py` & `bo4e-0.4.8/src/bo4e/com/externereferenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/fremdkostenblock.py` & `bo4e-0.4.8/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/fremdkostenposition.py` & `bo4e-0.4.8/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/geokoordinaten.py` & `bo4e-0.4.8/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/geraet.py` & `bo4e-0.4.8/src/bo4e/com/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/geraeteeigenschaften.py` & `bo4e-0.4.8/src/bo4e/com/geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/hardware.py` & `bo4e-0.4.8/src/bo4e/com/hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/katasteradresse.py` & `bo4e-0.4.8/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/kostenblock.py` & `bo4e-0.4.8/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/kostenposition.py` & `bo4e-0.4.8/src/bo4e/com/kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/kriteriumwert.py` & `bo4e-0.4.8/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/marktgebietinfo.py` & `bo4e-0.4.8/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/menge.py` & `bo4e-0.4.8/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/messlokationszuordnung.py` & `bo4e-0.4.8/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/positionsaufabschlag.py` & `bo4e-0.4.8/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/preis.py` & `bo4e-0.4.8/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/preisgarantie.py` & `bo4e-0.4.8/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/preisposition.py` & `bo4e-0.4.8/src/bo4e/com/preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/preisstaffel.py` & `bo4e-0.4.8/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/rechnungsposition.py` & `bo4e-0.4.8/src/bo4e/com/rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-0.4.8/src/bo4e/com/regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-0.4.8/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-0.4.8/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-0.4.8/src/bo4e/com/regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-0.4.8/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/regionskriterium.py` & `bo4e-0.4.8/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/rufnummer.py` & `bo4e-0.4.8/src/bo4e/com/rufnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/sigmoidparameter.py` & `bo4e-0.4.8/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-0.4.8/src/bo4e/com/standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-0.4.8/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/steuerbetrag.py` & `bo4e-0.4.8/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tagesvektor.py` & `bo4e-0.4.8/src/bo4e/com/tagesvektor.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-0.4.8/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-0.4.8/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifpreis.py` & `bo4e-0.4.8/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifpreisposition.py` & `bo4e-0.4.8/src/bo4e/com/tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-0.4.8/src/bo4e/com/tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-0.4.8/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/unterschrift.py` & `bo4e-0.4.8/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/verbrauch.py` & `bo4e-0.4.8/src/bo4e/com/verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/vertragskonditionen.py` & `bo4e-0.4.8/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/vertragsteil.py` & `bo4e-0.4.8/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zaehlwerk.py` & `bo4e-0.4.8/src/bo4e/com/zaehlwerk.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zeitintervall.py` & `bo4e-0.4.8/src/bo4e/com/zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zeitraum.py` & `bo4e-0.4.8/src/bo4e/com/zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zeitreihenwert.py` & `bo4e-0.4.8/src/bo4e/com/zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zeitreihenwertkompakt.py` & `bo4e-0.4.8/src/bo4e/com/zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/com/zustaendigkeit.py` & `bo4e-0.4.8/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/angebotsstatus.py` & `bo4e-0.4.8/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/artikelid.py` & `bo4e-0.4.8/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-0.4.8/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-0.4.8/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-0.4.8/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-0.4.8/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-0.4.8/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/botyp.py` & `bo4e-0.4.8/src/bo4e/enum/botyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-0.4.8/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/erzeugungsart.py` & `bo4e-0.4.8/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/gebiettyp.py` & `bo4e-0.4.8/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/geraetemerkmal.py` & `bo4e-0.4.8/src/bo4e/enum/geraetemerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/geraetetyp.py` & `bo4e-0.4.8/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-0.4.8/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-0.4.8/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/kostenklasse.py` & `bo4e-0.4.8/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/kundengruppe.py` & `bo4e-0.4.8/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/kundengruppeka.py` & `bo4e-0.4.8/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/kundentyp.py` & `bo4e-0.4.8/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/leistungstyp.py` & `bo4e-0.4.8/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/marktrolle.py` & `bo4e-0.4.8/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/mengeneinheit.py` & `bo4e-0.4.8/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/messgroesse.py` & `bo4e-0.4.8/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/messpreistyp.py` & `bo4e-0.4.8/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/messwertstatus.py` & `bo4e-0.4.8/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-0.4.8/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/netzebene.py` & `bo4e-0.4.8/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/nnrechnungstyp.py` & `bo4e-0.4.8/src/bo4e/enum/nnrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/oekolabel.py` & `bo4e-0.4.8/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/oekozertifikat.py` & `bo4e-0.4.8/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/preisgarantietyp.py` & `bo4e-0.4.8/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/preistyp.py` & `bo4e-0.4.8/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/rechnungslegung.py` & `bo4e-0.4.8/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/rechnungsstatus.py` & `bo4e-0.4.8/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/rechnungstyp.py` & `bo4e-0.4.8/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-0.4.8/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/rufnummernart.py` & `bo4e-0.4.8/src/bo4e/enum/rufnummernart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-0.4.8/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-0.4.8/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/tarifmerkmal.py` & `bo4e-0.4.8/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/themengebiet.py` & `bo4e-0.4.8/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/vertragsart.py` & `bo4e-0.4.8/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/vertragsstatus.py` & `bo4e-0.4.8/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/voraussetzungen.py` & `bo4e-0.4.8/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/waehrungscode.py` & `bo4e-0.4.8/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/zaehlertyp.py` & `bo4e-0.4.8/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/enum/zeiteinheit.py` & `bo4e-0.4.8/src/bo4e/enum/zeiteinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e/validators.py` & `bo4e-0.4.8/src/bo4e/validators.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/src/bo4e.egg-info/PKG-INFO` & `bo4e-0.4.8/src/bo4e.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.4.7/src/bo4e.egg-info/SOURCES.txt` & `bo4e-0.4.8/src/bo4e.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/serialization_helper.py` & `bo4e-0.4.8/tests/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_adresse.py` & `bo4e-0.4.8/tests/test_adresse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from pathlib import Path
 from typing import Dict, Optional
 
 import pytest
-from py._path.local import LocalPath  # type:ignore[import]
 from pydantic import ValidationError
 
 from bo4e.com.adresse import Adresse
 from bo4e.enum import landescode
 from bo4e.enum.landescode import Landescode
 
 # import pydantic
@@ -116,15 +116,15 @@
                  "postleitzahl":"5020",
                  "landescode":"AT"}"""
 
         a: Adresse = Adresse.parse_raw(json_string)
         assert a.landescode is Landescode.AT  # type: ignore[attr-defined]
 
     @pytest.mark.datafiles("./tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json")
-    def test_missing_required_attribute(self, datafiles: LocalPath) -> None:
+    def test_missing_required_attribute(self, datafiles: Path) -> None:
         """
         Test for getting an error message if a required attribute is missing
         """
 
         with pytest.raises(ValidationError) as excinfo:
             _ = Adresse.parse_file(datafiles / "test_data_adresse_missing_plz.json", encoding="utf-8")
```

### Comparing `bo4e-0.4.7/tests/test_angebot.py` & `bo4e-0.4.8/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_angebotsposition.py` & `bo4e-0.4.8/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_angebotsteil.py` & `bo4e-0.4.8/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_angebotsvariante.py` & `bo4e-0.4.8/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_ansprechpartner.py` & `bo4e-0.4.8/tests/test_ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_aufabschlag.py` & `bo4e-0.4.8/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_aufabschlagproort.py` & `bo4e-0.4.8/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_aufabschlagregional.py` & `bo4e-0.4.8/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_aufabschlagstaffelproort.py` & `bo4e-0.4.8/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_ausschreibung.py` & `bo4e-0.4.8/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_ausschreibungsdetail.py` & `bo4e-0.4.8/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_ausschreibungslos.py` & `bo4e-0.4.8/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_betrag.py` & `bo4e-0.4.8/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_buendelvertrag.py` & `bo4e-0.4.8/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_bypassing_validation.py` & `bo4e-0.4.8/tests/test_bypassing_validation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_energieherkunft.py` & `bo4e-0.4.8/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_energiemenge.py` & `bo4e-0.4.8/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_energiemix.py` & `bo4e-0.4.8/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_enums.py` & `bo4e-0.4.8/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_externe_referenz.py` & `bo4e-0.4.8/tests/test_externe_referenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_fremdkosten.py` & `bo4e-0.4.8/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_fremdkostenblock.py` & `bo4e-0.4.8/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_fremdkostenposition.py` & `bo4e-0.4.8/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_geokoordinaten.py` & `bo4e-0.4.8/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_geraet.py` & `bo4e-0.4.8/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_geraeteeigenschaften.py` & `bo4e-0.4.8/tests/test_geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_geschaeftsobjekt.py` & `bo4e-0.4.8/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_geschaeftspartner.py` & `bo4e-0.4.8/tests/test_geschaeftspartner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
+from pathlib import Path
 
 import pytest
-from py._path.local import LocalPath  # type:ignore[import]
 from pydantic import ValidationError
 
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.adresse import Adresse
 from bo4e.enum.anrede import Anrede
 from bo4e.enum.botyp import BoTyp
 from bo4e.enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
 from bo4e.enum.kontaktart import Kontaktart
 from bo4e.enum.landescode import Landescode
 
 
 class TestGeschaeftspartner:
     @pytest.mark.datafiles("./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json")
-    def test_serializable(self, datafiles: LocalPath) -> None:
+    def test_serializable(self, datafiles: Path) -> None:
         with open(datafiles / "test_data_adresse_only_required_fields.json", encoding="utf-8") as json_file:
             address_test_data = json.load(json_file)
 
         gp = Geschaeftspartner(
             anrede=Anrede.FRAU,
             name1="von Sinnen",
             name2="Helga",
```

### Comparing `bo4e-0.4.7/tests/test_kosten.py` & `bo4e-0.4.8/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_kostenblock.py` & `bo4e-0.4.8/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_kostenposition.py` & `bo4e-0.4.8/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_kriteriumswert.py` & `bo4e-0.4.8/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_lastgang.py` & `bo4e-0.4.8/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_lastgangkompakt.py` & `bo4e-0.4.8/tests/test_lastgangkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_marktlokation.py` & `bo4e-0.4.8/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_marktteilnehmer.py` & `bo4e-0.4.8/tests/test_marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_menge.py` & `bo4e-0.4.8/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_messlokation.py` & `bo4e-0.4.8/tests/test_messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_messlokationszuordnung.py` & `bo4e-0.4.8/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_netznutzungsrechnung.py` & `bo4e-0.4.8/tests/test_netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_positionsaufabschlag.py` & `bo4e-0.4.8/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preis.py` & `bo4e-0.4.8/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblatt.py` & `bo4e-0.4.8/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblatt_dienstleistung.py` & `bo4e-0.4.8/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblatt_hardware.py` & `bo4e-0.4.8/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-0.4.8/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblatt_messung.py` & `bo4e-0.4.8/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisblattnetznutzung.py` & `bo4e-0.4.8/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisgarantie.py` & `bo4e-0.4.8/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisposition.py` & `bo4e-0.4.8/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_preisstaffel.py` & `bo4e-0.4.8/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_rechnung.py` & `bo4e-0.4.8/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_rechnungsposition.py` & `bo4e-0.4.8/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_region.py` & `bo4e-0.4.8/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionalegueltigkeit.py` & `bo4e-0.4.8/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionalepreisgarantie.py` & `bo4e-0.4.8/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionalepreisstaffel.py` & `bo4e-0.4.8/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionaleraufabschlag.py` & `bo4e-0.4.8/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionaletarifpreisposition.py` & `bo4e-0.4.8/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionaltarif.py` & `bo4e-0.4.8/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_regionskriterium.py` & `bo4e-0.4.8/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_sigmoidparameter.py` & `bo4e-0.4.8/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_standorteigenschaften.py` & `bo4e-0.4.8/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_standorteigenschaftengas.py` & `bo4e-0.4.8/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_standorteigenschaftenstrom.py` & `bo4e-0.4.8/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_steuerbetrag.py` & `bo4e-0.4.8/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tagesvektor.py` & `bo4e-0.4.8/tests/test_tagesvektor.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarif.py` & `bo4e-0.4.8/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifberechnungsparameter.py` & `bo4e-0.4.8/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifeinschraenkung.py` & `bo4e-0.4.8/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifinfo.py` & `bo4e-0.4.8/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifkosten.py` & `bo4e-0.4.8/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifpreis.py` & `bo4e-0.4.8/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifpreisblatt.py` & `bo4e-0.4.8/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifpreisposition.py` & `bo4e-0.4.8/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifpreispositionproort.py` & `bo4e-0.4.8/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_tarifpreisstaffelproort.py` & `bo4e-0.4.8/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_unterschrift.py` & `bo4e-0.4.8/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_verbrauch.py` & `bo4e-0.4.8/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_vertrag.py` & `bo4e-0.4.8/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_vertragskonditionen.py` & `bo4e-0.4.8/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_vertragsteil.py` & `bo4e-0.4.8/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zaehler.py` & `bo4e-0.4.8/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zeitintervall.py` & `bo4e-0.4.8/tests/test_zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zeitraum.py` & `bo4e-0.4.8/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zeitreihe.py` & `bo4e-0.4.8/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zeitreihenwert.py` & `bo4e-0.4.8/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tests/test_zeitreihenwertkompakt.py` & `bo4e-0.4.8/tests/test_zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.7/tox.ini` & `bo4e-0.4.8/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pylint json_schemas/generate_json_schemas.py
 
 [testenv:type_check]
 usedevelop = True
 # the type_check environment checks the type hints using mypy
 deps =
     -rrequirements.txt
-    mypy
+    mypy==1.3.0
     pytest
 commands =
     mypy --show-error-codes src/bo4e
     mypy --show-error-codes tests
     mypy --show-error-codes docs/uml.py
     mypy --show-error-codes json_schemas/generate_json_schemas.py
     # add single files (ending with .py) or packages here
```

