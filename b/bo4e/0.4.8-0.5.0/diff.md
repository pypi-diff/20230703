# Comparing `tmp/bo4e-0.4.8.tar.gz` & `tmp/bo4e-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bo4e-0.4.8.tar", last modified: Mon Jul  3 04:53:41 2023, max compression
+gzip compressed data, was "bo4e-0.5.0.tar", last modified: Mon Jul  3 11:38:36 2023, max compression
```

## Comparing `bo4e-0.4.8.tar` & `bo4e-0.5.0.tar`

### file list

```diff
@@ -1,444 +1,447 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/formatting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-03 04:53:29.000000 bo4e-0.4.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-03 04:53:29.000000 bo4e-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 04:53:29.000000 bo4e-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-03 04:53:29.000000 bo4e-0.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 04:53:29.000000 bo4e-0.4.8/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 04:53:29.000000 bo4e-0.4.8/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 04:53:29.000000 bo4e-0.4.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 04:53:29.000000 bo4e-0.4.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-03 04:53:29.000000 bo4e-0.4.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 04:53:29.000000 bo4e-0.4.8/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:29.000000 bo4e-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 04:53:41.790287 bo4e-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-03 04:53:29.000000 bo4e-0.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/_static/bo4e-python-logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.bo.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.com.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.enum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/bo4e.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/test_uml.py
--rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-07-03 04:53:29.000000 bo4e-0.4.8/docs/uml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.750287 bo4e-0.4.8/json_schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.754287 bo4e-0.4.8/json_schemas/bo/
--rw-r--r--   0 runner    (1001) docker     (123)    52157 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Angebot.json
--rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Ansprechpartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Ausschreibung.json
--rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Buendelvertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Energiemenge.json
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Fremdkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Geschaeftsobjekt.json
--rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Geschaeftspartner.json
--rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Kosten.json
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Lastgang.json
--rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/LastgangKompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)    24945 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Marktlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Marktteilnehmer.json
--rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Messlokation.json
--rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Netznutzungsrechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Preisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    39186 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattDienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)    39843 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattHardware.json
--rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattKonzessionsabgabe.json
--rw-r--r--   0 runner    (1001) docker     (123)    39860 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattMessung.json
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/PreisblattNetznutzung.json
--rw-r--r--   0 runner    (1001) docker     (123)    36100 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Rechnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Region.json
--rw-r--r--   0 runner    (1001) docker     (123)    61951 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Regionaltarif.json
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Standorteigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)    59198 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarif.json
--rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifinfo.json
--rw-r--r--   0 runner    (1001) docker     (123)    44628 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifkosten.json
--rw-r--r--   0 runner    (1001) docker     (123)    56245 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Tarifpreisblatt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26552 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Vertrag.json
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Zaehler.json
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/Zeitreihe.json
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/bo/_LastgangBody.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.758287 bo4e-0.4.8/json_schemas/com/
--rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Adresse.json
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Angebotsvariante.json
--rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagRegional.json
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/AufAbschlagstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Ausschreibungsdetail.json
--rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Ausschreibungslos.json
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Betrag.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/COM.json
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Dienstleistung.json
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Energieherkunft.json
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Energiemix.json
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/ExterneReferenz.json
--rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Fremdkostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Fremdkostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geokoordinaten.json
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geraet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Geraeteeigenschaften.json
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Hardware.json
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Katasteradresse.json
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Kostenblock.json
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Kostenposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/KriteriumWert.json
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/MarktgebietInfo.json
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Menge.json
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Messlokationszuordnung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/PositionsAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preis.json
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Preisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Rechnungsposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionaleGueltigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalePreisgarantie.json
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalePreisstaffel.json
--rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionaleTarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/RegionalerAufAbschlag.json
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Regionskriterium.json
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Rufnummer.json
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Sigmoidparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenAllgemein.json
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenGas.json
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/StandorteigenschaftenStrom.json
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Steuerbetrag.json
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tagesvektor.json
--rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifberechnungsparameter.json
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifeinschraenkung.json
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifpreis.json
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Tarifpreisposition.json
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/TarifpreispositionProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/TarifpreisstaffelProOrt.json
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Unterschrift.json
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Verbrauch.json
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Vertragskonditionen.json
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Vertragsteil.json
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zaehlwerk.json
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitintervall.json
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitraum.json
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitreihenwert.json
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zeitreihenwertkompakt.json
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/com/Zustaendigkeit.json
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-03 04:53:29.000000 bo4e-0.4.8/json_schemas/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-03 04:53:29.000000 bo4e-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 04:53:29.000000 bo4e-0.4.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-03 04:53:29.000000 bo4e-0.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 04:53:41.790287 bo4e-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 04:53:29.000000 bo4e-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.746287 bo4e-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e/bo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3373 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5915 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/bo/zeitreihe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.774287 bo4e-0.4.8/src/bo4e/com/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/com.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/externereferenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/rufnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/com/zustaendigkeit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.782287 bo4e-0.4.8/src/bo4e/enum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/anrede.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/artikelid.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/botyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/energierichtung.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geraetemerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kontaktart.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/kundentyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/landescode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/marktrolle.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/medium.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messart.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messgroesse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/netzebene.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/nnrechnungsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/nnrechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/oekolabel.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preismodell.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preisstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/preistyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/rufnummernart.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/sparte.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/strenum.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifart.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tariftyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/themengebiet.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/titel.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsart.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsform.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/enum/zeiteinheit.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-07-03 04:53:29.000000 bo4e-0.4.8/src/bo4e/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.762287 bo4e-0.4.8/src/bo4e.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13354 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 04:53:41.000000 bo4e-0.4.8/src/bo4e.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/serialization_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_adresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_angebotsvariante.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ansprechpartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagproort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10190 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagregional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibung.py
--rw-r--r--   0 runner    (1001) docker     (123)     6516 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibungsdetail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_ausschreibungslos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_betrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_buendelvertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_bypassing_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.746287 bo4e-0.4.8/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 04:53:41.790287 bo4e-0.4.8/tests/test_data/test_data_adresse/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energieherkunft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energiemenge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_energiemix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_externe_referenz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_fremdkostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geokoordinaten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geraet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geraeteeigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geschaeftsobjekt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_geschaeftspartner.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_katasteradresse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kostenblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kostenposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_kriteriumswert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_lastgang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_lastgangkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktgebietinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_marktteilnehmer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_menge.py
--rw-r--r--   0 runner    (1001) docker     (123)     9715 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_messlokation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_messlokationszuordnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_netznutzungsrechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_positionsaufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblatt_messung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisblattnetznutzung.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_preisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_rechnung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_rechnungsposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalegueltigkeit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalepreisgarantie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionalepreisstaffel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaleraufabschlag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionaltarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_regionskriterium.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_sigmoidparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaften.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaftengas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_steuerbetrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tagesvektor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifeinschraenkung.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifkosten.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisblatt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreispositionproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_unterschrift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_verbrauch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertrag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertragskonditionen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_vertragsteil.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zaehler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitintervall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitraum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihenwert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-03 04:53:29.000000 bo4e-0.4.8/tests/test_zeitreihenwertkompakt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-03 04:53:29.000000 bo4e-0.4.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/formatting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-03 11:38:22.000000 bo4e-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-03 11:38:22.000000 bo4e-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-03 11:38:22.000000 bo4e-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-03 11:38:22.000000 bo4e-0.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-03 11:38:22.000000 bo4e-0.5.0/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-03 11:38:22.000000 bo4e-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-07-03 11:38:22.000000 bo4e-0.5.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 11:38:22.000000 bo4e-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-03 11:38:22.000000 bo4e-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-03 11:38:22.000000 bo4e-0.5.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:22.000000 bo4e-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 11:38:36.862871 bo4e-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-03 11:38:22.000000 bo4e-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.818870 bo4e-0.5.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26543 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/_static/bo4e-python-logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.822870 bo4e-0.5.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.bo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.com.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12407 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.enum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/bo4e.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/test_uml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29341 2023-07-03 11:38:22.000000 bo4e-0.5.0/docs/uml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.822870 bo4e-0.5.0/json_schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.826870 bo4e-0.5.0/json_schemas/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)    52157 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Angebot.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21807 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Ansprechpartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30100 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Ausschreibung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30522 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Buendelvertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Energiemenge.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Fremdkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Geschaeftsobjekt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13958 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Geschaeftspartner.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18391 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Kosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Lastgang.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/LastgangKompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24945 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Marktlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15569 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Marktteilnehmer.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32380 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Messlokation.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38378 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Netznutzungsrechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Preisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39186 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattDienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39843 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattHardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33150 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattKonzessionsabgabe.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39860 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattMessung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/PreisblattNetznutzung.json
+-rw-r--r--   0 runner    (1001) docker     (123)    36100 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Rechnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Region.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61951 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Regionaltarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Standorteigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)    59198 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarif.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30455 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifinfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    44628 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifkosten.json
+-rw-r--r--   0 runner    (1001) docker     (123)    56245 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Tarifpreisblatt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26552 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Vertrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Zaehler.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/Zeitreihe.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/bo/_LastgangBody.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.830870 bo4e-0.5.0/json_schemas/com/
+-rw-r--r--   0 runner    (1001) docker     (123)     7148 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Adresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39348 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)    41486 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Angebotsvariante.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7234 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26998 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagRegional.json
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/AufAbschlagstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Ausschreibungsdetail.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18473 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Ausschreibungslos.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Betrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/COM.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Dienstleistung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Energieherkunft.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Energiemix.json
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/ExterneReferenz.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11847 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Fremdkostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Fremdkostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geokoordinaten.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geraet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Geraeteeigenschaften.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Hardware.json
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Katasteradresse.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Kostenblock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Kostenposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/KriteriumWert.json
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/MarktgebietInfo.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Menge.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Messlokationszuordnung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/PositionsAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Preisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14694 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Rechnungsposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionaleGueltigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalePreisgarantie.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalePreisstaffel.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionaleTarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/RegionalerAufAbschlag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Regionskriterium.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Rufnummer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Sigmoidparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenAllgemein.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenGas.json
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/StandorteigenschaftenStrom.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Steuerbetrag.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tagesvektor.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7469 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifberechnungsparameter.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifeinschraenkung.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifpreis.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Tarifpreisposition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/TarifpreispositionProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/TarifpreisstaffelProOrt.json
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Unterschrift.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Verbrauch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Vertragskonditionen.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Vertragsteil.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zaehlwerk.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitintervall.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitraum.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitreihenwert.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zeitreihenwertkompakt.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/com/Zustaendigkeit.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-03 11:38:22.000000 bo4e-0.5.0/json_schemas/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-03 11:38:22.000000 bo4e-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 11:38:22.000000 bo4e-0.5.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-03 11:38:22.000000 bo4e-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-03 11:38:36.862871 bo4e-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-03 11:38:22.000000 bo4e-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.814869 bo4e-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e/bo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/bo/zeitreihe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.842871 bo4e-0.5.0/src/bo4e/com/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/com.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/externereferenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/rufnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/com/zustaendigkeit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.850871 bo4e-0.5.0/src/bo4e/enum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/anrede.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/artikelid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/botyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geraetemerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/landescode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/medium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/netzebene.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/nnrechnungsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/nnrechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preismodell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/preistyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/rufnummernart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/sparte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/strenum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/titel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/enum/zeiteinheit.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.850871 bo4e-0.5.0/src/bo4e/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-03 11:38:22.000000 bo4e-0.5.0/src/bo4e/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.834870 bo4e-0.5.0/src/bo4e.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13405 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-03 11:38:36.000000 bo4e-0.5.0/src/bo4e.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/serialization_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_adresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_angebotsvariante.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ansprechpartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10162 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagregional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_ausschreibungslos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_betrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_buendelvertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_bypassing_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.814869 bo4e-0.5.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:38:36.862871 bo4e-0.5.0/tests/test_data/test_data_adresse/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energieherkunft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energiemenge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_energiemix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_externe_referenz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_fremdkostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geokoordinaten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geraet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geraeteeigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_geschaeftspartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_katasteradresse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kostenblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kostenposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_kriteriumswert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_lastgang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_lastgangkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktgebietinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_marktteilnehmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_menge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_messlokation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_messlokationszuordnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_netznutzungsrechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_positionsaufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblatt_messung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_preisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_rechnung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_rechnungsposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionaltarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_regionskriterium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_sigmoidparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaften.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_steuerbetrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tagesvektor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifkosten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisblatt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_unterschrift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_verbrauch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12093 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertrag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertragskonditionen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_vertragsteil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zaehler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitintervall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitraum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihenwert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 11:38:22.000000 bo4e-0.5.0/tests/test_zeitreihenwertkompakt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-03 11:38:22.000000 bo4e-0.5.0/tox.ini
```

### Comparing `bo4e-0.4.8/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-0.5.0/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-0.5.0/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/dependabot.yml` & `bo4e-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/codeql-analysis.yml` & `bo4e-0.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/coverage.yml` & `bo4e-0.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/docs.yml` & `bo4e-0.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/formatting.yml` & `bo4e-0.5.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/linting.yml` & `bo4e-0.5.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/python-publish.yml` & `bo4e-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.github/workflows/tests.yml` & `bo4e-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.gitignore` & `bo4e-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.pre-commit-config.yaml` & `bo4e-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.pylintrc` & `bo4e-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/.readthedocs.yaml` & `bo4e-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/CONTRIBUTING.md` & `bo4e-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/LICENSE.rst` & `bo4e-0.5.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/PKG-INFO` & `bo4e-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.4.8/README.rst` & `bo4e-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/Makefile` & `bo4e-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/_static/bo4e-python-favicon.png` & `bo4e-0.5.0/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/_static/bo4e-python-favicon.svg` & `bo4e-0.5.0/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/_static/bo4e-python-logo.png` & `bo4e-0.5.0/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/_static/bo4e-python-logo.svg` & `bo4e-0.5.0/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/api/bo4e.bo.rst` & `bo4e-0.5.0/docs/api/bo4e.bo.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/api/bo4e.com.rst` & `bo4e-0.5.0/docs/api/bo4e.com.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/api/bo4e.enum.rst` & `bo4e-0.5.0/docs/api/bo4e.enum.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/conf.py` & `bo4e-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/index.rst` & `bo4e-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/docs/requirements.txt` & `bo4e-0.5.0/docs/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via requests
 charset-normalizer==2.1.0
     # via requests
 idna==3.3
     # via requests
 iso3166==2.1.1
     # via -r docs/requirements.in
-networkx==3.0
+networkx==3.1
     # via -r docs/requirements.in
 pydantic==1.10.5
     # via -r docs/requirements.in
 pyhumps==3.8.0
     # via -r docs/requirements.in
 requests==2.31.0
     # via -r docs/requirements.in
```

### Comparing `bo4e-0.4.8/docs/uml.py` & `bo4e-0.5.0/docs/uml.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,33 +10,21 @@
 import os
 import pkgutil
 import re
 import shlex
 import subprocess
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
-from re import Pattern
 from typing import Any, Dict, List, Optional, Tuple, Type, cast
 
 import networkx as nx  # type: ignore[import]
 import requests  # type: ignore[import]
-
-# pylint: disable=no-name-in-module
-from pydantic import ConstrainedStr
-from pydantic.fields import (
-    MAPPING_LIKE_SHAPES,
-    SHAPE_GENERIC,
-    SHAPE_LIST,
-    SHAPE_NAME_LOOKUP,
-    SHAPE_SINGLETON,
-    SHAPE_TUPLE,
-    ModelField,
-)
-from pydantic.main import ModelMetaclass
-from pydantic.typing import display_as_type
+from pydantic._internal._model_construction import ModelMetaclass
+from pydantic._internal._repr import display_as_type
+from pydantic.fields import FieldInfo
 
 
 # pylint: disable=too-few-public-methods
 class _Package:
     """
     Encapsulates scope and color options into a class to make linter and type checker happier
     """
@@ -139,15 +127,15 @@
         list(map(self.nodes[node1]["fields"].__delitem__, self.nodes[node2]["fields"].keys()))
 
     # pylint: disable=too-many-arguments
     def add_association(
         self,
         node1: str,
         node2: str,
-        through_field: ModelField,
+        through_field: FieldInfo,
         card1: Optional[Cardinality] = None,
         card2: Optional[Cardinality] = None,
     ) -> None:
         """
         Adds an association-relation. `node1` references `node2` in its field `through_field`. Additionally, you can
         provide information relating to the cardinality of the association.
         """
@@ -224,45 +212,47 @@
         if card:
             if card[0] == card[1]:
                 return f"{card[0]}"
             return f"{card[0]}..{card[1]}"
         return None
 
     @staticmethod
-    def model_field_str(model_field: ModelField, card: Optional[Cardinality] = None) -> str:
-        """
-        Parse the type of the ModelField to a printable string. Copied from pydantic.field.ModelField._type_display()
+    def model_field_str(model_field: FieldInfo, card: Optional[Cardinality] = None) -> str:
         """
-        result_str = display_as_type(model_field.type_)
-
+        Parse the type of the ModelField to a printable string. Copied from
+        pydantic._internal._repr.display_as_type
+        https://github.com/pydantic/pydantic/blob/58ae1ef77a4bf4276aaa6214aaaaf59455f5e587/pydantic/_internal/_repr.py#L85
+        """
+        result_str = display_as_type(model_field.annotation)
+        # todo: check if this is still necessary
+        # https://github.com/bo4e/BO4E-python/issues/478
         # have to do this since display_as_type(self.outer_type_) is different (and wrong) on python 3.6
-        if model_field.shape in MAPPING_LIKE_SHAPES:
-            result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
-        elif model_field.shape == SHAPE_TUPLE:
-            result_str = "Tuple[" + ", ".join(
-                display_as_type(
-                    sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
-                )
-            )
-            result_str += "]"
-        elif model_field.shape == SHAPE_GENERIC:
-            assert model_field.sub_fields
-            result_str = (
-                f"{display_as_type(model_field.type_)}["
-                f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
-            )
-        elif model_field.shape not in (SHAPE_SINGLETON, SHAPE_LIST):
-            result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
-
-        if isinstance(model_field.outer_type_, type) and issubclass(model_field.outer_type_, ConstrainedStr):
-            if isinstance(model_field.outer_type_.regex, Pattern):
-                result_str = f"str<{model_field.outer_type_.regex.pattern}>"
-            elif isinstance(model_field.outer_type_.regex, str):
-                result_str = f"str<{model_field.outer_type_.regex}>"
-
+        # if model_field.shape in MAPPING_LIKE_SHAPES:
+        #    result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
+        # elif model_field.shape == SHAPE_TUPLE:
+        #    result_str = "Tuple[" + ", ".join(
+        #        display_as_type(
+        #            sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
+        #        )
+        #    )
+        #    result_str += "]"
+        # elif model_field.shape == SHAPE_GENERIC:
+        #    assert model_field.sub_fields
+        #    result_str = (
+        #        f"{display_as_type(model_field.type_)}["
+        #        f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
+        #    )
+        # elif model_field.shape not in (SHAPE_SINGLETON, SHAPE_LIST):
+        #    result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
+        #
+        # if is_constrained_str(model_field):
+        #    if isinstance(model_field.outer_type_.regex, Pattern):
+        #        result_str = f"str<{model_field.outer_type_.regex.pattern}>"
+        #    elif isinstance(model_field.outer_type_.regex, str):
+        #        result_str = f"str<{model_field.outer_type_.regex}>"
         assert card is not None
         return f"{result_str} [{_UMLNetworkABC.get_cardinality_string(card)}]"
 
     @staticmethod
     def _remove_last_package_name(namespace: str) -> str:
         """
         E.g. `_remove_last_package_name('bo4e.bo.angebot.Angebot')` -> `bo4e.bo.Angebot`. The only use of this function
@@ -287,21 +277,22 @@
         cls_str = (
             f'class "[[{LINK_URI_BASE}/api/bo4e.{node.split(".")[1]}.html#{node}'
             f' {node.split(".")[-1]}]]\\n<size:10>{".".join(node.split(".")[0:-1])}" as {node.split(".")[-1]}'
         )
         if detailed:
             cls_str += " {\n"
             for field_dict in self.nodes[node]["fields"].values():
-                model_field = field_dict["model_field"]
-                type_modl_namespace = f"{model_field.type_.__module__}.{model_field.type_.__name__}"
+                model_field: FieldInfo = field_dict["model_field"]
+                assert model_field.annotation is not None
+                type_modl_namespace = f"{model_field.annotation.__module__}.{model_field.annotation.__name__}"
                 if type_modl_namespace in self[node]:
                     # Skip the fields which will appear as references in the graph
                     continue
                 type_str = _UMLNetworkABC.model_field_str(model_field, field_dict["card"])
-                if model_field.required:
+                if model_field.is_required():
                     cls_str += f"\t{model_field.alias} : {type_str}\n"
                 else:
                     cls_str += f"\t{model_field.alias} : {type_str} = {model_field.default}\n"
             cls_str += "}"
 
         return cls_str
 
@@ -453,61 +444,63 @@
         with open(file_path / file_name, "w+", encoding="utf-8") as uml_file:
             uml_file.write(file_content)
             path_list.append(file_path / file_name)
 
     return path_list
 
 
-def model_field_str(model_field: ModelField) -> str:
+def model_field_str(model_field: FieldInfo) -> str:
     """
     Parse the type of the ModelField to a printable string. Copied from pydantic.field.ModelField._type_display()
     """
-    result_str = display_as_type(model_field.type_)
-
+    result_str = display_as_type(model_field.annotation)
+    # todo: check if this is still necessary
+    # https://github.com/bo4e/BO4E-python/issues/478
     # have to do this since display_as_type(self.outer_type_) is different (and wrong) on python 3.6
-    if model_field.shape in MAPPING_LIKE_SHAPES:
-        result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
-    elif model_field.shape == SHAPE_TUPLE:
-        result_str = "Tuple[" + ", ".join(
-            display_as_type(
-                sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
-            )
-        )
-        result_str += "]"
-    elif model_field.shape == SHAPE_GENERIC:
-        assert model_field.sub_fields
-        result_str = (
-            f"{display_as_type(model_field.type_)}["
-            f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
-        )
-    elif model_field.shape != SHAPE_SINGLETON:
-        result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
-
-    if model_field.allow_none and (model_field.shape != SHAPE_SINGLETON or not model_field.sub_fields):
-        result_str = f"Optional[{result_str}]"
+    # if model_field.shape in MAPPING_LIKE_SHAPES:
+    #    result_str = f"Mapping[{display_as_type(cast(ModelField, model_field.key_field).type_)}, {result_str}]"
+    # elif model_field.shape == SHAPE_TUPLE:
+    #    result_str = "Tuple[" + ", ".join(
+    #        display_as_type(
+    #            sub_field.type_ for sub_field in model_field.sub_fields  # type:ignore[arg-type,union-attr]
+    #        )
+    #    )
+    #    result_str += "]"
+    # elif model_field.shape == SHAPE_GENERIC:
+    #    assert model_field.sub_fields
+    #    result_str = (
+    #        f"{display_as_type(model_field.type_)}["
+    #        f"{', '.join(display_as_type(sub_field.type_) for sub_field in model_field.sub_fields)}]"
+    #    )
+    # elif model_field.shape != SHAPE_SINGLETON:
+    #    result_str = SHAPE_NAME_LOOKUP[model_field.shape].format(result_str)
+    # if model_field.allow_none and (model_field.shape != SHAPE_SINGLETON or not model_field.sub_fields):
+    #    result_str = f"Optional[{result_str}]"
     return result_str
 
 
-def get_cardinality(model_field: ModelField) -> Cardinality:
+def get_cardinality(model_field: FieldInfo) -> Cardinality:
     """
     Determines the cardinality of a field. This field can either contain a reference to another node in the graph or
     be of another arbitrary type.
     """
     type_str = model_field_str(model_field)
     card1: str = "1"
     card2: str = "1"
     if type_str.startswith("Optional["):
         card1 = "0"
     if type_str.startswith("List[") or type_str.startswith("Optional[List["):
         card1 = "0"
         card2 = "*"
-        if hasattr(model_field.outer_type_, "max_items") and model_field.outer_type_.max_items:
-            card2 = str(model_field.outer_type_.max_items)
-        if hasattr(model_field.outer_type_, "min_items") and model_field.outer_type_.min_items:
-            card1 = str(model_field.outer_type_.min_items)
+        # todo: re-add min_length / max_length interpretation
+        # https://github.com/bo4e/BO4E-python/issues/477
+        # if hasattr(model_field.outer_type_, "max_items") and model_field.outer_type_.max_items:
+        #    card2 = str(model_field.outer_type_.max_items)
+        # if hasattr(model_field.outer_type_, "min_items") and model_field.outer_type_.min_items:
+        #    card1 = str(model_field.outer_type_.min_items)
     return card1, card2
 
 
 def build_network(module_dir: Path, parser: Type[_UMLNetworkABC]) -> Tuple[_UMLNetworkABC, List[str]]:
     """
     Build a network of the relationships of all classes found in bo4e packages defined by `pkgs` and all classes
     referenced by any class in these packages. Referenced classes will be added only if `regex_incl_network` matches and
@@ -554,22 +547,23 @@
             uml_network.add_extension(
                 modl_namespace,
                 type_modl_namespace,
             )
     # ------------------------------------------------------------------------------------------------------------------
     # ------ determine references in fields which pass `regex_incl_network` and `regex_excl_network` -------------------
     for field_dict in uml_network.nodes[modl_namespace]["fields"].values():
-        model_field: ModelField = field_dict["model_field"]
+        model_field: FieldInfo = field_dict["model_field"]
         # Add cardinality information to the field
         field_card = get_cardinality(model_field)
         field_dict["card"] = field_card
-        type_modl_namespace = f"{model_field.type_.__module__}.{model_field.type_.__name__}"
+        assert model_field.annotation is not None
+        type_modl_namespace = f"{model_field.annotation.__module__}.{model_field.annotation.__name__}"
         if re.match(regex_incl_network, type_modl_namespace) and not re.match(regex_excl_network, type_modl_namespace):
             if not uml_network.has_node(type_modl_namespace):
-                _recursive_add_class(model_field.type_, type_modl_namespace, uml_network)
+                _recursive_add_class(model_field.annotation, type_modl_namespace, uml_network)  # type:ignore[arg-type]
 
             uml_network.add_association(
                 modl_namespace,
                 type_modl_namespace,
                 through_field=model_field,
                 card1=None,
                 card2=field_card,
```

### Comparing `bo4e-0.4.8/json_schemas/bo/Angebot.json` & `bo4e-0.5.0/json_schemas/bo/Angebot.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Ansprechpartner.json` & `bo4e-0.5.0/json_schemas/bo/Ansprechpartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Ausschreibung.json` & `bo4e-0.5.0/json_schemas/bo/Ausschreibung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Buendelvertrag.json` & `bo4e-0.5.0/json_schemas/bo/Buendelvertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Energiemenge.json` & `bo4e-0.5.0/json_schemas/bo/Energiemenge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Fremdkosten.json` & `bo4e-0.5.0/json_schemas/bo/Fremdkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Geschaeftsobjekt.json` & `bo4e-0.5.0/json_schemas/bo/Geschaeftsobjekt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Geschaeftspartner.json` & `bo4e-0.5.0/json_schemas/bo/Geschaeftspartner.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Kosten.json` & `bo4e-0.5.0/json_schemas/bo/Kosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Lastgang.json` & `bo4e-0.5.0/json_schemas/bo/Lastgang.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/LastgangKompakt.json` & `bo4e-0.5.0/json_schemas/bo/LastgangKompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Marktlokation.json` & `bo4e-0.5.0/json_schemas/bo/Marktlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Marktteilnehmer.json` & `bo4e-0.5.0/json_schemas/bo/Marktteilnehmer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Messlokation.json` & `bo4e-0.5.0/json_schemas/bo/Messlokation.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Netznutzungsrechnung.json` & `bo4e-0.5.0/json_schemas/bo/Netznutzungsrechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Preisblatt.json` & `bo4e-0.5.0/json_schemas/bo/Preisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/PreisblattDienstleistung.json` & `bo4e-0.5.0/json_schemas/bo/PreisblattDienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/PreisblattHardware.json` & `bo4e-0.5.0/json_schemas/bo/PreisblattHardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/PreisblattKonzessionsabgabe.json` & `bo4e-0.5.0/json_schemas/bo/PreisblattKonzessionsabgabe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/PreisblattMessung.json` & `bo4e-0.5.0/json_schemas/bo/PreisblattMessung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/PreisblattNetznutzung.json` & `bo4e-0.5.0/json_schemas/bo/PreisblattNetznutzung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Rechnung.json` & `bo4e-0.5.0/json_schemas/bo/Rechnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Region.json` & `bo4e-0.5.0/json_schemas/bo/Region.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Regionaltarif.json` & `bo4e-0.5.0/json_schemas/bo/Regionaltarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Standorteigenschaften.json` & `bo4e-0.5.0/json_schemas/bo/Standorteigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Tarif.json` & `bo4e-0.5.0/json_schemas/bo/Tarif.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Tarifinfo.json` & `bo4e-0.5.0/json_schemas/bo/Tarifinfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Tarifkosten.json` & `bo4e-0.5.0/json_schemas/bo/Tarifkosten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Tarifpreisblatt.json` & `bo4e-0.5.0/json_schemas/bo/Tarifpreisblatt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Vertrag.json` & `bo4e-0.5.0/json_schemas/bo/Vertrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Zaehler.json` & `bo4e-0.5.0/json_schemas/bo/Zaehler.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/Zeitreihe.json` & `bo4e-0.5.0/json_schemas/bo/Zeitreihe.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/bo/_LastgangBody.json` & `bo4e-0.5.0/json_schemas/bo/_LastgangBody.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Adresse.json` & `bo4e-0.5.0/json_schemas/com/Adresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Angebotsposition.json` & `bo4e-0.5.0/json_schemas/com/Angebotsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Angebotsteil.json` & `bo4e-0.5.0/json_schemas/com/Angebotsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Angebotsvariante.json` & `bo4e-0.5.0/json_schemas/com/Angebotsvariante.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/AufAbschlag.json` & `bo4e-0.5.0/json_schemas/com/AufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/AufAbschlagProOrt.json` & `bo4e-0.5.0/json_schemas/com/AufAbschlagProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/AufAbschlagRegional.json` & `bo4e-0.5.0/json_schemas/com/AufAbschlagRegional.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/AufAbschlagstaffelProOrt.json` & `bo4e-0.5.0/json_schemas/com/AufAbschlagstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Ausschreibungsdetail.json` & `bo4e-0.5.0/json_schemas/com/Ausschreibungsdetail.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Ausschreibungslos.json` & `bo4e-0.5.0/json_schemas/com/Ausschreibungslos.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Betrag.json` & `bo4e-0.5.0/json_schemas/com/Betrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Dienstleistung.json` & `bo4e-0.5.0/json_schemas/com/Dienstleistung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Energieherkunft.json` & `bo4e-0.5.0/json_schemas/com/Energieherkunft.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Energiemix.json` & `bo4e-0.5.0/json_schemas/com/Energiemix.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/ExterneReferenz.json` & `bo4e-0.5.0/json_schemas/com/ExterneReferenz.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Fremdkostenblock.json` & `bo4e-0.5.0/json_schemas/com/Fremdkostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Fremdkostenposition.json` & `bo4e-0.5.0/json_schemas/com/Fremdkostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Geokoordinaten.json` & `bo4e-0.5.0/json_schemas/com/Geokoordinaten.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Geraet.json` & `bo4e-0.5.0/json_schemas/com/Geraet.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Geraeteeigenschaften.json` & `bo4e-0.5.0/json_schemas/com/Geraeteeigenschaften.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Hardware.json` & `bo4e-0.5.0/json_schemas/com/Hardware.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Katasteradresse.json` & `bo4e-0.5.0/json_schemas/com/Katasteradresse.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Kostenblock.json` & `bo4e-0.5.0/json_schemas/com/Kostenblock.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Kostenposition.json` & `bo4e-0.5.0/json_schemas/com/Kostenposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/KriteriumWert.json` & `bo4e-0.5.0/json_schemas/com/KriteriumWert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/MarktgebietInfo.json` & `bo4e-0.5.0/json_schemas/com/MarktgebietInfo.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Menge.json` & `bo4e-0.5.0/json_schemas/com/Menge.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Messlokationszuordnung.json` & `bo4e-0.5.0/json_schemas/com/Messlokationszuordnung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/PositionsAufAbschlag.json` & `bo4e-0.5.0/json_schemas/com/PositionsAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Preis.json` & `bo4e-0.5.0/json_schemas/com/Preis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Preisgarantie.json` & `bo4e-0.5.0/json_schemas/com/Preisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Preisposition.json` & `bo4e-0.5.0/json_schemas/com/Preisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Preisstaffel.json` & `bo4e-0.5.0/json_schemas/com/Preisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Rechnungsposition.json` & `bo4e-0.5.0/json_schemas/com/Rechnungsposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/RegionaleGueltigkeit.json` & `bo4e-0.5.0/json_schemas/com/RegionaleGueltigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/RegionalePreisgarantie.json` & `bo4e-0.5.0/json_schemas/com/RegionalePreisgarantie.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/RegionalePreisstaffel.json` & `bo4e-0.5.0/json_schemas/com/RegionalePreisstaffel.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/RegionaleTarifpreisposition.json` & `bo4e-0.5.0/json_schemas/com/RegionaleTarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/RegionalerAufAbschlag.json` & `bo4e-0.5.0/json_schemas/com/RegionalerAufAbschlag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Regionskriterium.json` & `bo4e-0.5.0/json_schemas/com/Regionskriterium.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Rufnummer.json` & `bo4e-0.5.0/json_schemas/com/Rufnummer.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Sigmoidparameter.json` & `bo4e-0.5.0/json_schemas/com/Sigmoidparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenAllgemein.json` & `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenAllgemein.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenGas.json` & `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenGas.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/StandorteigenschaftenStrom.json` & `bo4e-0.5.0/json_schemas/com/StandorteigenschaftenStrom.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Steuerbetrag.json` & `bo4e-0.5.0/json_schemas/com/Steuerbetrag.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Tagesvektor.json` & `bo4e-0.5.0/json_schemas/com/Tagesvektor.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Tarifberechnungsparameter.json` & `bo4e-0.5.0/json_schemas/com/Tarifberechnungsparameter.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Tarifeinschraenkung.json` & `bo4e-0.5.0/json_schemas/com/Tarifeinschraenkung.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Tarifpreis.json` & `bo4e-0.5.0/json_schemas/com/Tarifpreis.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Tarifpreisposition.json` & `bo4e-0.5.0/json_schemas/com/Tarifpreisposition.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/TarifpreispositionProOrt.json` & `bo4e-0.5.0/json_schemas/com/TarifpreispositionProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/TarifpreisstaffelProOrt.json` & `bo4e-0.5.0/json_schemas/com/TarifpreisstaffelProOrt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Unterschrift.json` & `bo4e-0.5.0/json_schemas/com/Unterschrift.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Verbrauch.json` & `bo4e-0.5.0/json_schemas/com/Verbrauch.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Vertragskonditionen.json` & `bo4e-0.5.0/json_schemas/com/Vertragskonditionen.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Vertragsteil.json` & `bo4e-0.5.0/json_schemas/com/Vertragsteil.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zaehlwerk.json` & `bo4e-0.5.0/json_schemas/com/Zaehlwerk.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zeitintervall.json` & `bo4e-0.5.0/json_schemas/com/Zeitintervall.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zeitraum.json` & `bo4e-0.5.0/json_schemas/com/Zeitraum.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zeitreihenwert.json` & `bo4e-0.5.0/json_schemas/com/Zeitreihenwert.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zeitreihenwertkompakt.json` & `bo4e-0.5.0/json_schemas/com/Zeitreihenwertkompakt.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/com/Zustaendigkeit.json` & `bo4e-0.5.0/json_schemas/com/Zustaendigkeit.json`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/json_schemas/generate_json_schemas.py` & `bo4e-0.5.0/json_schemas/generate_json_schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,8 @@
             file_path = this_directory / pkg / (name + ".json")  # pylint:disable=invalid-name
             schema_json_dict = json.loads(cls.schema_json(ensure_ascii=False, sort_keys=True, indent=4))
             if "definitions" in schema_json_dict:
                 for definition in schema_json_dict["definitions"].values():
                     # this sanitizing step is necessary since python 3.11
                     definition["description"] = definition["description"].strip()
             with open(file_path, "w+", encoding="utf-8") as json_schema_file:
-                json_schema_file.write(json.dumps(schema_json_dict, ensure_ascii=False, indent=4))
+                json_schema_file.write(json.dumps(schema_json_dict, indent=4))
```

### Comparing `bo4e-0.4.8/pyproject.toml` & `bo4e-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/setup.cfg` & `bo4e-0.5.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 zip_safe = False
 packages = find:
 package_dir = = src
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	iso3166
-	pydantic==1.*
+	pydantic>=2.0.0
 	pyhumps
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/angebot.py` & `bo4e-0.5.0/src/bo4e/bo/angebot.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,25 +34,25 @@
 
 
     """
 
     bo_typ: BoTyp = BoTyp.ANGEBOT
     # required attributes
     #: Eindeutige Nummer des Angebotes
-    angebotsnummer: constr(strict=True, regex=r"^\d+$")  # type: ignore[valid-type]
+    angebotsnummer: constr(strict=True, pattern=r"^\d+$")  # type: ignore[valid-type]
     #: Erstellungsdatum des Angebots
     angebotsdatum: datetime
     #: Sparte, für die das Angebot abgegeben wird (Strom/Gas)
     sparte: Sparte
     #: Ersteller des Angebots
     angebotsgeber: Geschaeftspartner
     #: Empfänger des Angebots
     angebotsnehmer: Geschaeftspartner
 
-    varianten: conlist(Angebotsvariante, min_items=1)  # type: ignore[valid-type]
+    varianten: conlist(Angebotsvariante, min_length=1)  # type: ignore[valid-type]
     """ Eine oder mehrere Varianten des Angebots mit den Angebotsteilen;
     Ein Angebot besteht mindestens aus einer Variante."""
 
     # optional attributes
     anfragereferenz: Optional[str] = None
     """	Referenz auf eine Anfrage oder Ausschreibung;
     Kann dem Empfänger des Angebotes bei Zuordnung des Angebotes zur Anfrage bzw. Ausschreibung helfen."""
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/ansprechpartner.py` & `bo4e-0.5.0/src/bo4e/bo/ansprechpartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/ausschreibung.py` & `bo4e-0.5.0/src/bo4e/bo/ausschreibung.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,14 @@
     """
     bindefrist: Zeitraum
     """
     Diese Komponente wird zur Abbildung von Zeiträumen in Form von Dauern oder der Angabe von Start und Ende verwendet.
     Es muss daher entweder eine Dauer oder ein Zeitraum in Form von Start und Ende angegeben sein
     """
     #: Die einzelnen Lose, aus denen sich die Ausschreibung zusammensetzt
-    lose: conlist(Ausschreibungslos, min_items=1)  # type: ignore[valid-type]
+    lose: conlist(Ausschreibungslos, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Aufzählung der unterstützten Ausschreibungsportale
     ausschreibungportal: Optional[Ausschreibungsportal] = None
     #: Internetseite, auf der die Ausschreibung veröffentlicht wurde (falls vorhanden)
     webseite: Optional[str] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/buendelvertrag.py` & `bo4e-0.5.0/src/bo4e/bo/buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/energiemenge.py` & `bo4e-0.5.0/src/bo4e/bo/energiemenge.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     #: Eindeutige Nummer der Marktlokation bzw. der Messlokation, zu der die Energiemenge gehört
     lokations_id: str
     # todo: add validator such that only mess- or marktlokations IDs are accepted + cross check with lokationstyp
     #: Gibt an, ob es sich um eine Markt- oder Messlokation handelt
     lokationstyp: Lokationstyp
 
     #: Gibt den Verbrauch in einer Zeiteinheit an
-    energieverbrauch: conlist(Verbrauch, min_items=1)  # type: ignore[valid-type]
+    energieverbrauch: conlist(Verbrauch, min_length=1)  # type: ignore[valid-type]
     # there are no optional attributes
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/fremdkosten.py` & `bo4e-0.5.0/src/bo4e/bo/fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-0.5.0/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,10 +39,10 @@
     # pylint:disable=duplicate-code
     class Config:
         """
         basic configuration for pydantic's behaviour
         """
 
         alias_generator = camelize
-        allow_population_by_field_name = True
+        populate_by_name = True
         extra = "allow"
         json_encoders = {Decimal: str}
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/geschaeftspartner.py` & `bo4e-0.5.0/src/bo4e/bo/geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/kosten.py` & `bo4e-0.5.0/src/bo4e/bo/kosten.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     # required attributes
     bo_typ: BoTyp = BoTyp.KOSTEN
     #: Klasse der Kosten, beispielsweise Fremdkosten
     kostenklasse: Kostenklasse
     #: Für diesen Zeitraum wurden die Kosten ermittelt
     gueltigkeit: Zeitraum
     #: In Kostenblöcken werden Kostenpositionen zusammengefasst. Beispiele: Netzkosten, Umlagen, Steuern etc
-    kostenbloecke: conlist(Kostenblock, min_items=1)  # type: ignore[valid-type]
+    kostenbloecke: conlist(Kostenblock, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Die Gesamtsumme über alle Kostenblöcke und -positionen
     summe_kosten: Optional[List[Betrag]] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/lastgang.py` & `bo4e-0.5.0/src/bo4e/bo/lastgang.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     #: Definition der gemessenen Größe anhand ihrer Einheit
     messgroesse: Mengeneinheit
 
     # optional attributes
     #: Versionsnummer des Lastgangs
     version: Optional[str] = None
     #: Die OBIS-Kennzahl für den Wert, die festlegt, welche Größe mit dem Stand gemeldet wird, z.B. '1-0:1.8.1'
-    obis_kennzahl: Optional[constr(strict=True, regex=OBIS_PATTERN)] = None  # type: ignore[valid-type]
+    obis_kennzahl: Optional[constr(strict=True, pattern=OBIS_PATTERN)] = None  # type: ignore[valid-type]
 
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 class LastgangKompakt(_LastgangBody):
     """
@@ -85,8 +85,8 @@
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.LASTGANG
 
     #: Die im Lastgang enthaltenen Messwerte
-    werte: conlist(Zeitreihenwert, min_items=1)  # type: ignore[valid-type]
+    werte: conlist(Zeitreihenwert, min_length=1)  # type: ignore[valid-type]
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/marktlokation.py` & `bo4e-0.5.0/src/bo4e/bo/marktlokation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Contains Marktlokation class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
-from typing import Any, Dict, Optional
+from typing import Optional
 
 # pylint: disable=no-name-in-module
-from pydantic import conlist, validator
+from pydantic import conlist, field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.bo.geschaeftsobjekt import Geschaeftsobjekt
 from bo4e.bo.geschaeftspartner import Geschaeftspartner
 from bo4e.com.adresse import Adresse
 from bo4e.com.geokoordinaten import Geokoordinaten
 from bo4e.com.katasteradresse import Katasteradresse
 from bo4e.com.messlokationszuordnung import Messlokationszuordnung
@@ -40,15 +41,15 @@
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.MARKTLOKATION
     #: Identifikationsnummer einer Marktlokation, an der Energie entweder verbraucht, oder erzeugt wird.
     marktlokations_id: str
-    _marktlokations_id_check = validator("marktlokations_id", allow_reuse=True)(validate_marktlokations_id)
+    _marktlokations_id_check = field_validator("marktlokations_id")(validate_marktlokations_id)
     #: Sparte der Marktlokation, z.B. Gas oder Strom
     sparte: Sparte
     #: Kennzeichnung, ob Energie eingespeist oder entnommen (ausgespeist) wird
     energierichtung: Energierichtung
     #: Die Bilanzierungsmethode, RLM oder SLP
     bilanzierungsmethode: Bilanzierungsmethode
     netzebene: Netzebene
@@ -110,23 +111,24 @@
     """
     katasterinformation: Optional[Katasteradresse] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
-    kundengruppen: conlist(Kundentyp, min_items=0) = None  # type: ignore[valid-type]
+    kundengruppen: Optional[conlist(Kundentyp, min_length=0)] = None  # type: ignore[valid-type]
     #: Kundengruppen der Marktlokation
 
     # pylint:disable=unused-argument, no-self-argument
-    @validator("katasterinformation", always=True)
+    @field_validator("katasterinformation")
     def validate_address_info(
-        cls, katasterinformation: Optional[Katasteradresse], values: Dict[str, Any]
+        cls, katasterinformation: Optional[Katasteradresse], validation_info: ValidationInfo
     ) -> Optional[Katasteradresse]:
         """Checks that there is one and only one valid adress given."""
+        values = validation_info.data  # type:ignore[attr-defined]
         all_address_attributes = [
             values["lokationsadresse"],
             values["geoadresse"],
             katasterinformation,
         ]
         amount_of_given_address_infos = len([i for i in all_address_attributes if i is not None])
         if amount_of_given_address_infos != 1:
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/marktteilnehmer.py` & `bo4e-0.5.0/src/bo4e/bo/marktteilnehmer.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.MARKTTEILNEHMER
     #: Gibt im Klartext die Bezeichnung der Marktrolle an
     marktrolle: Marktrolle
     #: Gibt die Codenummer der Marktrolle an
-    rollencodenummer: constr(strict=True, regex=r"^\d{13}$")  # type: ignore[valid-type]
+    rollencodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
     #: Gibt den Typ des Codes an
     rollencodetyp: Rollencodetyp
     #: Sparte des Marktteilnehmers, z.B. Gas oder Strom
     sparte: Sparte
 
     # optional attributes
     #: Die 1:1-Kommunikationsadresse des Marktteilnehmers; Diese wird in der Marktkommunikation verwendet.
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/messlokation.py` & `bo4e-0.5.0/src/bo4e/bo/messlokation.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,26 +90,26 @@
     katasterinformation: Optional[Katasteradresse] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
     # pylint: disable=unused-argument, no-self-argument
-    @validator("messlokations_id", always=True)
+    @validator("messlokations_id")
     def _validate_messlokations_id(cls, messlokations_id: str) -> str:
         if not messlokations_id:
             raise ValueError("The messlokations_id must not be empty.")
         if not _melo_id_pattern.match(messlokations_id):
             raise ValueError(f"The messlokations_id '{messlokations_id}' does not match {_melo_id_pattern.pattern}")
         if not messlokations_id[0:2] in countries:
             raise ValueError(f"The country code '{messlokations_id[0:2]}' is not a valid country code")
         return messlokations_id
 
     # pylint: disable=no-self-argument
-    @validator("katasterinformation", always=True)
+    @validator("katasterinformation")
     def validate_address_info(
         cls, katasterinformation: Optional[Katasteradresse], values: Dict[str, Any]
     ) -> Optional[Katasteradresse]:
         """Checks that if an address is given, that there is only one valid address given"""
         all_address_attributes = [
             values["messadresse"],
             values["geoadresse"],
@@ -117,15 +117,15 @@
         ]
         amount_of_given_address_infos = len([i for i in all_address_attributes if i is not None])
         if amount_of_given_address_infos > 1:
             raise ValueError("More than one address information is given.")
         return katasterinformation
 
     # pylint: disable=no-self-argument
-    @validator("grundzustaendiger_msbim_codenr", always=True)
+    @validator("grundzustaendiger_msbim_codenr")
     def validate_grundzustaendiger_x_codenr(
         cls, grundzustaendiger_msbim_codenr: Optional[str], values: Dict[str, Any]
     ) -> Optional[str]:
         """Checks that if a codenr is given, that there is only one valid codenr given."""
         all_grundzustaendiger_x_codenr_attributes = [
             values["grundzustaendiger_msb_codenr"],
             grundzustaendiger_msbim_codenr,
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/netznutzungsrechnung.py` & `bo4e-0.5.0/src/bo4e/bo/netznutzungsrechnung.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.NETZNUTZUNGSRECHNUNG
     #: Sparte (Strom, Gas ...) für die die Rechnung ausgestellt ist
     sparte: Sparte
-    absendercodenummer: constr(strict=True, regex=r"^\d{13}$")  # type: ignore[valid-type]
+    absendercodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
     """
     Die Rollencodenummer des Absenders (siehe :class:`Marktteilnehmer`).
     Über die Nummer können weitere Informationen zum Marktteilnehmer ermittelt werden.
     """
-    empfaengercodenummer: constr(strict=True, regex=r"^\d{13}$")  # type: ignore[valid-type]
+    empfaengercodenummer: constr(strict=True, pattern=r"^\d{13}$")  # type: ignore[valid-type]
     """
     Die Rollencodenummer des Empfängers (siehe :class:`Marktteilnehmer`).
     Über die Nummer können weitere Informationen zum Marktteilnehmer ermittelt werden.
     """
     #: Aus der INVOIC entnommen
     nnrechnungsart: NNRechnungsart
     #: Aus der INVOIC entnommen
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblatt.py` & `bo4e-0.5.0/src/bo4e/bo/preisblatt.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,11 +43,11 @@
     #: Preisblatt gilt für angegebene Sparte
     sparte: Sparte
     #: Merkmal, das anzeigt, ob es sich um vorläufige oder endgültige Preise handelt
     preisstatus: Preisstatus
     #: Der Zeitraum für den der Preis festgelegt ist
     gueltigkeit: Zeitraum
     #: Die einzelnen Positionen, die mit dem Preisblatt abgerechnet werden können. Z.B. Arbeitspreis, Grundpreis etc
-    preispositionen: conlist(Preisposition, min_items=1)  # type: ignore[valid-type]
+    preispositionen: conlist(Preisposition, min_length=1)  # type: ignore[valid-type]
     # optional attributes
     #: Der Netzbetreiber, der die Preise veröffentlicht hat
     herausgeber: Optional[Marktteilnehmer] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-0.5.0/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblatthardware.py` & `bo4e-0.5.0/src/bo4e/bo/preisblatthardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-0.5.0/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblattmessung.py` & `bo4e-0.5.0/src/bo4e/bo/preisblattmessung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-0.5.0/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/rechnung.py` & `bo4e-0.5.0/src/bo4e/bo/rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/region.py` & `bo4e-0.5.0/src/bo4e/bo/region.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,12 @@
 
     # required attributes
     bo_typ: BoTyp = BoTyp.REGION
     #: Bezeichnung der Region
     bezeichnung: str
 
     #: Positivliste der Kriterien zur Definition der Region
-    positiv_liste: conlist(Regionskriterium, min_items=1)  # type: ignore[valid-type]
+    positiv_liste: conlist(Regionskriterium, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Negativliste der Kriterien zur Definition der Region
     negativ_liste: Optional[List[Regionskriterium]] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/regionaltarif.py` & `bo4e-0.5.0/src/bo4e/bo/regionaltarif.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     bo_typ: BoTyp = BoTyp.REGIONALTARIF
     # required attributes
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
     #: Die festgelegten Preise mit regionaler Eingrenzung, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(RegionaleTarifpreisposition, min_items=1)  # type: ignore[valid-type]
+    tarifpreise: conlist(RegionaleTarifpreisposition, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
     tarif_auf_abschlaege: Optional[List[RegionalerAufAbschlag]] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
     preisgarantien: Optional[List[RegionalePreisgarantie]] = None
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/standorteigenschaften.py` & `bo4e-0.5.0/src/bo4e/bo/standorteigenschaften.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,12 +27,12 @@
         `Standorteigenschaften JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/bo/Standorteigenschaften.json>`_
 
     """
 
     # required attributes
     bo_typ: BoTyp = BoTyp.STANDORTEIGENSCHAFTEN
     #: Eigenschaften zur Sparte Strom
-    eigenschaften_strom: conlist(StandorteigenschaftenStrom, min_items=1)  # type: ignore[valid-type]
+    eigenschaften_strom: conlist(StandorteigenschaftenStrom, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Eigenschaften zur Sparte Gas
     eigenschaften_gas: Optional[StandorteigenschaftenGas] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/tarif.py` & `bo4e-0.5.0/src/bo4e/bo/tarif.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     bo_typ: BoTyp = BoTyp.TARIF
     # required attributes
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
     #: Die festgelegten Preise mit regionaler Eingrenzung z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(TarifpreispositionProOrt, min_items=1)  # type: ignore[valid-type]
+    tarifpreise: conlist(TarifpreispositionProOrt, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
     tarif_auf_abschlaege: Optional[List[AufAbschlagRegional]] = None
     # todo: fix inconsistency: RegionalerAufAbschlag vs. AufAbschlagRegional
     # https://github.com/Hochfrequenz/BO4E-python/issues/345
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/tarifinfo.py` & `bo4e-0.5.0/src/bo4e/bo/tarifinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
     #: Name des Tarifs
     bezeichnung: str
     #: Der Name des Marktpartners, der den Tarif anbietet
     anbietername: str
     #: Strom oder Gas, etc.
     sparte: Sparte
     #: Kundentypen für den der Tarif gilt, z.B. Privatkunden
-    kundentypen: conlist(Kundentyp, min_items=1)  # type: ignore[valid-type]
+    kundentypen: conlist(Kundentyp, min_length=1)  # type: ignore[valid-type]
     #: Die Art des Tarifes, z.B. Eintarif oder Mehrtarif
     tarifart: Tarifart
     #: Hinweis auf den Tariftyp, z.B. Grundversorgung oder Sondertarif
     tariftyp: Tariftyp
     #: Weitere Merkmale des Tarifs, z.B. Festpreis oder Vorkasse
-    tarifmerkmale: conlist(Tarifmerkmal, min_items=1)  # type: ignore[valid-type]
+    tarifmerkmale: conlist(Tarifmerkmal, min_length=1)  # type: ignore[valid-type]
     #: Der Marktteilnehmer (Lieferant), der diesen Tarif anbietet
     anbieter: Marktteilnehmer
 
     # optional attributes
     #: Internetseite auf dem der Tarif zu finden ist
     website: Optional[str] = None
     #: Freitext
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/tarifkosten.py` & `bo4e-0.5.0/src/bo4e/bo/tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-0.5.0/src/bo4e/bo/tarifpreisblatt.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
 
     bo_typ: BoTyp = BoTyp.TARIFPREISBLATT
     # required attributes (additional to those of Tarifinfo)
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: datetime
     #: Die festgelegten Preise, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: conlist(Tarifpreisposition, min_items=1)  # type: ignore[valid-type]
+    tarifpreise: conlist(Tarifpreisposition, min_length=1)  # type: ignore[valid-type]
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
     berechnungsparameter: Tarifberechnungsparameter
 
     # optional attributes
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
     tarifeinschraenkung: Optional[Tarifeinschraenkung] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/vertrag.py` & `bo4e-0.5.0/src/bo4e/bo/vertrag.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """
     vertragspartner2: Geschaeftspartner
     """
     Der "zweitgenannte" Vertragspartner.
     In der Regel der Empfänger des Vertrags.
     Beispiel "Vertrag zwischen Vertragspartner 1 und Vertragspartner 2".
     """
-    vertragsteile: conlist(Vertragsteil, min_items=1)  # type: ignore[valid-type]
+    vertragsteile: conlist(Vertragsteil, min_length=1)  # type: ignore[valid-type]
     """
     Der Vertragsteil wird dazu verwendet, eine vertragliche Leistung in Bezug zu einer Lokation
     (Markt- oder Messlokation) festzulegen.
     """
 
     # optional attributes
     #: Beschreibung zum Vertrag
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/zaehler.py` & `bo4e-0.5.0/src/bo4e/bo/zaehler.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     # required attributes
     bo_typ: BoTyp = BoTyp.ZAEHLER
     zaehlernummer: str  #: Nummerierung des Zählers,vergeben durch den Messstellenbetreiber
     sparte: Sparte  #: Strom oder Gas
     zaehlerauspraegung: Zaehlerauspraegung  #: Spezifikation die Richtung des Zählers betreffend
     zaehlertyp: Zaehlertyp  #: Typisierung des Zählers
-    zaehlwerke: conlist(Zaehlwerk, min_items=1)  # type: ignore[valid-type]  #: Die Zählwerke des Zählers
+    zaehlwerke: conlist(Zaehlwerk, min_length=1)  # type: ignore[valid-type]  #: Die Zählwerke des Zählers
     tarifart: Tarifart  #: Spezifikation bezüglich unterstützter Tarifarten
 
     # optional attributes
     zaehlerkonstante: Optional[Decimal] = None  #: Zählerkonstante auf dem Zähler
     eichung_bis: Optional[datetime] = None  #: Bis zu diesem Datum (exklusiv) ist der Zähler geeicht.
     letzte_eichung: Optional[datetime] = None  #: Zu diesem Datum fand die letzte Eichprüfung des Zählers statt.
     zaehlerhersteller: Optional[Geschaeftspartner] = None  #: Der Hersteller des Zählers
```

### Comparing `bo4e-0.4.8/src/bo4e/bo/zeitreihe.py` & `bo4e-0.5.0/src/bo4e/bo/zeitreihe.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     #: Beschreibt die Art der Messung (z.B. aktueller Wert, mittlerer Wert, maximaler Wert)
     messart: Messart
     #: Medium, das gemessen wurde (z.B. Wasser, Dampf, Strom, Gas)
     medium: Medium
     #: Alle Werte in der Tabelle haben die Einheit, die hier angegeben ist
     einheit: Mengeneinheit
     #: Hier liegen jeweils die Werte
-    werte: conlist(Zeitreihenwert, min_items=1)  # type: ignore[valid-type]
+    werte: conlist(Zeitreihenwert, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Beschreibt die Verwendung der Zeitreihe
     beschreibung: Optional[str] = None
     #: Version der Zeitreihe
     version: Optional[str] = None
     #: Kennzeichnung, wie die Werte entstanden sind, z.B. durch Messung
```

### Comparing `bo4e-0.4.8/src/bo4e/com/adresse.py` & `bo4e-0.5.0/src/bo4e/com/adresse.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     adresszusatz: Optional[str] = None
     #: Im Falle einer c/o-Adresse steht in diesem Attribut die Anrede. Z.B. "c/o Veronica Hauptmieterin"
     co_ergaenzung: Optional[str] = None
     #: Offizieller ISO-Landescode
     landescode: Landescode = Landescode.DE  # type:ignore
 
     # pylint: disable=no-self-argument
-    @validator("postfach", always=True)
+    @validator("postfach")
     def strasse_xor_postfach(cls, postfach: Optional[str], values: Dict[str, Any]) -> Optional[str]:
         """
         An address is valid if it contains a postfach XOR (a strasse AND hausnummer).
         This functions checks for these conditions of a valid address.
 
         Nur folgende Angabekombinationen sind (nach der Abfrage) möglich:
         Straße           w   f   f
```

### Comparing `bo4e-0.4.8/src/bo4e/com/angebotsposition.py` & `bo4e-0.5.0/src/bo4e/com/angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/angebotsteil.py` & `bo4e-0.5.0/src/bo4e/com/angebotsteil.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     .. HINT::
         `Angebotsteil JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Angebotsteil.json>`_
 
     """
 
     # required attributes
     #: Einzelne Positionen, die zu diesem Angebotsteil gehören
-    positionen: conlist(Angebotsposition, min_items=1)  # type: ignore[valid-type]
+    positionen: conlist(Angebotsposition, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Identifizierung eines Subkapitels einer Anfrage, beispielsweise das Los einer Ausschreibung
     anfrage_subreferenz: Optional[str] = None
     lieferstellenangebotsteil: Optional[List[Marktlokation]] = None
     """
     Marktlokationen, für die dieses Angebotsteil gilt, falls vorhanden.
```

### Comparing `bo4e-0.4.8/src/bo4e/com/angebotsvariante.py` & `bo4e-0.5.0/src/bo4e/com/angebotsvariante.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     #: Datum der Erstellung der Angebotsvariante
     erstellungsdatum: datetime
 
     #: Bis zu diesem Zeitpunkt gilt die Angebotsvariante
     bindefrist: datetime
 
-    teile: conlist(Angebotsteil, min_items=1)  # type: ignore[valid-type]
+    teile: conlist(Angebotsteil, min_length=1)  # type: ignore[valid-type]
     """
     Angebotsteile werden im einfachsten Fall für eine Marktlokation oder Lieferstellenadresse erzeugt.
     Hier werden die Mengen und Gesamtkosten aller Angebotspositionen zusammengefasst.
     Eine Variante besteht mindestens aus einem Angebotsteil.
     """
 
     # optional attributes
```

### Comparing `bo4e-0.4.8/src/bo4e/com/aufabschlag.py` & `bo4e-0.5.0/src/bo4e/com/aufabschlag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Contains AufAbschlag class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from typing import List, Optional
 
-from pydantic import validator
+from pydantic import field_validator
 
 from bo4e.com.com import COM
 from bo4e.com.preisstaffel import Preisstaffel
 from bo4e.com.zeitraum import Zeitraum
 from bo4e.enum.aufabschlagstyp import AufAbschlagstyp
 from bo4e.enum.aufabschlagsziel import AufAbschlagsziel
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
@@ -42,14 +42,14 @@
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #: Typ des Aufabschlages (z.B. absolut oder prozentual).
     auf_abschlagstyp: Optional[AufAbschlagstyp] = None
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc..
     auf_abschlagsziel: Optional[AufAbschlagsziel] = None
     einheit: Optional[Waehrungseinheit] = None
-    _einheit_check = validator("einheit", allow_reuse=True)(einheit_only_for_abschlagstyp_absolut)
+    _einheit_check = field_validator("einheit")(einheit_only_for_abschlagstyp_absolut)
     """ Gibt an in welcher Währungseinheit der Auf/Abschlag berechnet wird. Euro oder Ct..
     (Nur im Falle absoluter Aufschlagstypen). """
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind.
     website: Optional[str] = None
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind.
     gueltigkeitszeitraum: Optional[Zeitraum] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/com/aufabschlagproort.py` & `bo4e-0.5.0/src/bo4e/com/aufabschlagproort.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     #: Die Postleitzahl des Ortes für den der Aufschlag gilt.
     postleitzahl: str
     #: Der Ort für den der Aufschlag gilt.
     ort: str
     #: Die ene't-Netznummer des Netzes in dem der Aufschlag gilt.
     netznr: str
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung.
-    staffeln: conlist(AufAbschlagstaffelProOrt, min_items=1)  # type: ignore[valid-type]
+    staffeln: conlist(AufAbschlagstaffelProOrt, min_length=1)  # type: ignore[valid-type]
```

### Comparing `bo4e-0.4.8/src/bo4e/com/aufabschlagregional.py` & `bo4e-0.5.0/src/bo4e/com/aufabschlagregional.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     """
 
     # required attributess
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: str
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    betraege: conlist(AufAbschlagProOrt, min_items=1)  # type: ignore[valid-type]
+    betraege: conlist(AufAbschlagProOrt, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #:Typ des Aufabschlages (z.B. absolut oder prozentual)
     auf_abschlagstyp: Optional[AufAbschlagstyp] = None
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc.
```

### Comparing `bo4e-0.4.8/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-0.5.0/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-0.5.0/src/bo4e/com/ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/ausschreibungslos.py` & `bo4e-0.5.0/src/bo4e/com/ausschreibungslos.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     wunsch_vertragsform: Vertragsform
     #: Name des Lizenzpartners
     betreut_durch: str
     #: Anzahl der Lieferstellen in dieser Ausschreibung
     anzahl_lieferstellen: int
 
     #: Die ausgeschriebenen Lieferstellen
-    lieferstellen: conlist(Ausschreibungsdetail, min_items=1)  # type: ignore[valid-type]
+    lieferstellen: conlist(Ausschreibungsdetail, min_length=1)  # type: ignore[valid-type]
 
     #: Zeitraum, für den die in diesem Los enthaltenen Lieferstellen beliefert werden sollen
     lieferzeitraum: Zeitraum
 
     # optional attributes
     #: Bemerkung des Kunden zum Los
     bemerkung: Optional[str] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/com/betrag.py` & `bo4e-0.5.0/src/bo4e/com/betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/com.py` & `bo4e-0.5.0/src/bo4e/com/com.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     # pylint:disable=duplicate-code
     class Config:
         """
         basic configuration for pydantic's behaviour
         """
 
         alias_generator = camelize
-        allow_population_by_field_name = True
+        populate_by_name = True
         extra = "allow"
         json_encoders = {Decimal: str}
 
 
 # pylint: disable=invalid-name
 #: Any type derived from COM including those that do not directly inherit from COM
 TCom = TypeVar("TCom", bound=Type[COM])
```

### Comparing `bo4e-0.4.8/src/bo4e/com/dienstleistung.py` & `bo4e-0.5.0/src/bo4e/com/dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/energieherkunft.py` & `bo4e-0.5.0/src/bo4e/com/energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/energiemix.py` & `bo4e-0.5.0/src/bo4e/com/energiemix.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     #: Strom oder Gas etc.
     energieart: Sparte
     #: Bezeichnung des Energiemix
     bezeichnung: str
     #: Jahr, für das der Energiemix gilt
     gueltigkeitsjahr: int
     #: Anteile der jeweiligen Erzeugungsart
-    anteil: conlist(Energieherkunft, min_items=1)  # type: ignore[valid-type]
+    anteil: conlist(Energieherkunft, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Bemerkung zum Energiemix
     bemerkung: Optional[str] = None
     #: Höhe des erzeugten CO2-Ausstosses in g/kWh
     co2_emission: Optional[Decimal] = None
     #: Höhe des erzeugten Atommülls in g/kWh
```

### Comparing `bo4e-0.4.8/src/bo4e/com/externereferenz.py` & `bo4e-0.5.0/src/bo4e/com/externereferenz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/fremdkostenblock.py` & `bo4e-0.5.0/src/bo4e/com/fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/fremdkostenposition.py` & `bo4e-0.5.0/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/geokoordinaten.py` & `bo4e-0.5.0/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/geraet.py` & `bo4e-0.5.0/src/bo4e/com/geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/geraeteeigenschaften.py` & `bo4e-0.5.0/src/bo4e/com/geraeteeigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/hardware.py` & `bo4e-0.5.0/src/bo4e/com/hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/katasteradresse.py` & `bo4e-0.5.0/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/kostenblock.py` & `bo4e-0.5.0/src/bo4e/com/kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/kostenposition.py` & `bo4e-0.5.0/src/bo4e/com/kostenposition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Contains Kostenposition and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
-from typing import Any, Dict, Optional
+from typing import Optional
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
-from pydantic import validator
+from pydantic import field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.com.betrag import Betrag
 from bo4e.com.com import COM
 from bo4e.com.menge import Menge
 from bo4e.com.preis import Preis
 from bo4e.validators import check_bis_is_later_than_von
 
@@ -43,28 +44,28 @@
     einzelpreis: Preis
 
     # optional attributes
     #: inklusiver von-Zeitpunkt der Kostenzeitscheibe
     von: Optional[datetime] = None
     #: exklusiver bis-Zeitpunkt der Kostenzeitscheibe
     bis: Optional[datetime] = None
-    _bis_check = validator("bis", always=True, allow_reuse=True)(check_bis_is_later_than_von)
+    _bis_check = field_validator("bis")(check_bis_is_later_than_von)
 
     #: Die Menge, die in die Kostenberechnung eingeflossen ist. Beispiel: 3.660 kWh
     menge: Optional[Menge] = None
 
     zeitmenge: Optional[Menge] = None
     """
     Wenn es einen zeitbasierten Preis gibt (z.B. €/Jahr), dann ist hier die Menge angegeben mit der die Kosten berechnet
     wurden. Z.B. 138 Tage.
     """
 
     #: Detaillierung des Artikels (optional). Beispiel: 'Drehstromzähler'
     artikeldetail: Optional[str] = None
 
     @staticmethod
-    def _get_inclusive_start(values: Dict[str, Any]) -> Optional[datetime]:
-        return values["von"]
+    def _get_inclusive_start(values: ValidationInfo) -> Optional[datetime]:
+        return values.data["von"]  # type:ignore[attr-defined]
 
     # @staticmethod
     # def _get_exclusive_end(values) -> Optional[datetime]:
     #     return values['bis']
```

### Comparing `bo4e-0.4.8/src/bo4e/com/kriteriumwert.py` & `bo4e-0.5.0/src/bo4e/com/kriteriumwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/marktgebietinfo.py` & `bo4e-0.5.0/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/menge.py` & `bo4e-0.5.0/src/bo4e/com/menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/messlokationszuordnung.py` & `bo4e-0.5.0/src/bo4e/com/messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/positionsaufabschlag.py` & `bo4e-0.5.0/src/bo4e/com/positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/preis.py` & `bo4e-0.5.0/src/bo4e/com/preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/preisgarantie.py` & `bo4e-0.5.0/src/bo4e/com/preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/preisposition.py` & `bo4e-0.5.0/src/bo4e/com/preisposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     #: Bezeichnung für die in der Position abgebildete Leistungserbringung
     leistungsbezeichnung: str
     #: Festlegung, mit welcher Preiseinheit abgerechnet wird, z.B. Ct. oder €
     preiseinheit: Waehrungseinheit
     #: Hier wird festgelegt, auf welche Bezugsgrösse sich der Preis bezieht, z.B. kWh oder Stück
     bezugsgroesse: Mengeneinheit
     #: Preisstaffeln, die zu dieser Preisposition gehören
-    preisstaffeln: conlist(Preisstaffel, min_items=1)  # type: ignore[valid-type]
+    preisstaffeln: conlist(Preisstaffel, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     zeitbasis: Optional[Zeiteinheit] = None
     """
     Die Zeit(dauer) auf die sich der Preis bezieht.
     Z.B. ein Jahr für einen Leistungspreis der in €/kW/Jahr ausgegeben wird
     """
```

### Comparing `bo4e-0.4.8/src/bo4e/com/preisstaffel.py` & `bo4e-0.5.0/src/bo4e/com/preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/rechnungsposition.py` & `bo4e-0.5.0/src/bo4e/com/rechnungsposition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Contains Rechnungsposition class and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
-from typing import Any, Dict, Optional
+from typing import Optional
 
-from pydantic import validator
+from pydantic import field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.com.betrag import Betrag
 from bo4e.com.com import COM
 from bo4e.com.menge import Menge
 from bo4e.com.preis import Preis
 from bo4e.com.steuerbetrag import Steuerbetrag
 from bo4e.enum.bdewartikelnummer import BDEWArtikelnummer
@@ -34,15 +35,15 @@
 
     # required attributes
     #: Fortlaufende Nummer für die Rechnungsposition
     positionsnummer: int
 
     lieferung_von: datetime  #: Start der Lieferung für die abgerechnete Leistung (inklusiv)
     lieferung_bis: datetime  #: Ende der Lieferung für die abgerechnete Leistung (exklusiv)
-    _bis_check = validator("lieferung_bis", always=True, allow_reuse=True)(check_bis_is_later_than_von)
+    _bis_check = field_validator("lieferung_bis")(check_bis_is_later_than_von)
 
     #: Bezeichung für die abgerechnete Position
     positionstext: str
 
     #: Die abgerechnete Menge mit Einheit
     positions_menge: Menge
     #: Der Preis für eine Einheit der energetischen Menge
@@ -77,14 +78,14 @@
     #: Nettobetrag für den Rabatt dieser Position
     teilrabatt_netto: Optional[Betrag] = None
 
     #: Standardisierte vom BDEW herausgegebene Liste, welche im Strommarkt die BDEW-Artikelnummer ablöst
     artikel_id: Optional[str] = None
 
     @staticmethod
-    def _get_inclusive_start(values: Dict[str, Any]) -> datetime:
+    def _get_inclusive_start(values: ValidationInfo) -> datetime:
         """return the inclusive start (used in the validator)"""
-        return values["lieferung_von"]
+        return values.data["lieferung_von"]  # type:ignore[attr-defined]
 
     # def _get_exclusive_end(self) -> datetime:
     #     """return the exclusive end (used in the validator)"""
     #     return self.lieferung_bis
```

### Comparing `bo4e-0.4.8/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-0.5.0/src/bo4e/com/regionalegueltigkeit.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,9 +24,9 @@
         `RegionaleGueltigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/RegionaleGueltigkeit.json>`_
 
     """
 
     # required attributes
     gueltigkeitstyp: Gueltigkeitstyp  #: Unterscheidung ob Positivliste oder Negativliste übertragen wird
     kriteriums_werte: conlist(  # type: ignore[valid-type]
-        KriteriumWert, min_items=1
+        KriteriumWert, min_length=1
     )  #: Hier stehen die Kriterien, die die regionale Gültigkeit festlegen
```

### Comparing `bo4e-0.4.8/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-0.5.0/src/bo4e/com/regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-0.5.0/src/bo4e/com/regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-0.5.0/src/bo4e/com/regionaleraufabschlag.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
 
     # required attributes
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: str
 
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    staffeln: conlist(RegionalePreisstaffel, min_items=1)  # type: ignore[valid-type]
+    staffeln: conlist(RegionalePreisstaffel, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Beschreibung des Auf-/Abschlags
     beschreibung: Optional[str] = None
 
     #: Typ des Aufabschlages (z.B. absolut oder prozentual)
     auf_abschlagstyp: Optional[AufAbschlagstyp] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-0.5.0/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     #: Angabe des Preistypes (z.B. Grundpreis)
     preistyp: Preistyp
     #: Einheit des Preises (z.B. EURO)
     einheit: Waehrungseinheit
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
     bezugseinheit: Mengeneinheit
     #: Hier sind die Staffeln mit ihren Preisangaben und regionalen Gültigkeiten definiert
-    preisstaffeln: conlist(RegionalePreisstaffel, min_items=1)  # type: ignore[valid-type]
+    preisstaffeln: conlist(RegionalePreisstaffel, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
     mengeneinheitstaffel: Optional[Mengeneinheit] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/com/regionskriterium.py` & `bo4e-0.5.0/src/bo4e/com/regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/rufnummer.py` & `bo4e-0.5.0/src/bo4e/com/rufnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/sigmoidparameter.py` & `bo4e-0.5.0/src/bo4e/com/sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-0.5.0/src/bo4e/com/standorteigenschaftengas.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
     .. HINT::
         `StandorteigenschaftenGas JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/StandorteigenschaftenGas.json>`_
 
     """
 
     # required attributes
-    netzkontonummern: conlist(str, min_items=1, max_items=2)  # type: ignore[valid-type]  #: Netzkontonummern der Gasnetze
+    netzkontonummern: conlist(str, min_length=1, max_length=2)  # type: ignore[valid-type]  #: Netzkontonummern der Gasnetze
     marktgebiete: List[MarktgebietInfo]  #: Die Informationen zu Marktgebieten in dem Netz.
```

### Comparing `bo4e-0.4.8/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-0.5.0/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/steuerbetrag.py` & `bo4e-0.5.0/src/bo4e/com/steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/tagesvektor.py` & `bo4e-0.5.0/src/bo4e/com/tagesvektor.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,12 +29,12 @@
     tag: datetime.datetime
     """
     Der Zeitpunkt ab dem die Werte ermittelt wurden.
     Es kann entweder der Beginn des Strom- oder Gastages verwendet werden.
     Der Zeitpunkt sollte eindeutig sein, d.h. sowohl Datum+Uhrzeit als auch den UTC-Offset spezifizieren.
     """
     # for the validator see also https://github.com/Hochfrequenz/BO4E-python/issues/262
-    werte: conlist(Zeitreihenwertkompakt, min_items=1)  # type: ignore[valid-type]
+    werte: conlist(Zeitreihenwertkompakt, min_length=1)  # type: ignore[valid-type]
     """
     Die Werte am angegebenen Tag;
     In Kombination aus Zeitintervall und Tag lassen sich die Zeiten der Werte eindeutig konstruieren.
     """
```

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-0.5.0/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-0.5.0/src/bo4e/com/tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifpreis.py` & `bo4e-0.5.0/src/bo4e/com/tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifpreisposition.py` & `bo4e-0.5.0/src/bo4e/com/tarifpreisposition.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,12 @@
     #: Angabe des Preistypes (z.B. Grundpreis)
     preistyp: Preistyp
     #: Einheit des Preises (z.B. EURO)
     einheit: Waehrungseinheit
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
     bezugseinheit: Mengeneinheit
     #: Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: conlist(Preisstaffel, min_items=1)  # type: ignore[valid-type]
+    preisstaffeln: conlist(Preisstaffel, min_length=1)  # type: ignore[valid-type]
 
     # optional attributes
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
     mengeneinheitstaffel: Optional[Mengeneinheit] = None
```

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-0.5.0/src/bo4e/com/tarifpreispositionproort.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     .. HINT::
         `TarifpreispositionProOrt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/TarifpreispositionProOrt.json>`_
 
     """
 
     # required attributes
     #: Postleitzahl des Ortes für den der Preis gilt
-    postleitzahl: constr(strict=True, regex=r"^\d{5}$")  # type: ignore[valid-type]
+    postleitzahl: constr(strict=True, pattern=r"^\d{5}$")  # type: ignore[valid-type]
     #: Ort für den der Preis gilt
     ort: str
     #: ene't-Netznummer des Netzes in dem der Preis gilt
     netznr: str
     # Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: conlist(TarifpreisstaffelProOrt, min_items=1)  # type: ignore[valid-type]
+    preisstaffeln: conlist(TarifpreisstaffelProOrt, min_length=1)  # type: ignore[valid-type]
     # there are no optional attributes
```

### Comparing `bo4e-0.4.8/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-0.5.0/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/unterschrift.py` & `bo4e-0.5.0/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/verbrauch.py` & `bo4e-0.5.0/src/bo4e/com/verbrauch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 Contains Verbrauch and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
 from decimal import Decimal
-from typing import Any, Dict, Optional
+from typing import Optional
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from pydantic import constr, validator
+from pydantic import constr, field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.com.com import COM
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.wertermittlungsverfahren import Wertermittlungsverfahren
 from bo4e.validators import OBIS_PATTERN, check_bis_is_later_than_von
 
 
@@ -28,28 +29,28 @@
 
     """
 
     # required attributes
     #: Gibt an, ob es sich um eine PROGNOSE oder eine MESSUNG handelt
     wertermittlungsverfahren: Wertermittlungsverfahren
     #: Die OBIS-Kennzahl für den Wert, die festlegt, welche Größe mit dem Stand gemeldet wird, z.B. '1-0:
-    obis_kennzahl: constr(strict=True, regex=OBIS_PATTERN)  # type: ignore[valid-type]  # type: ignore[valid-type]
+    obis_kennzahl: constr(strict=True, pattern=OBIS_PATTERN)  # type: ignore[valid-type]  # type: ignore[valid-type]
     #: Gibt den absoluten Wert der Menge an
     wert: Decimal
     #: Gibt die Einheit zum jeweiligen Wert an
     einheit: Mengeneinheit
 
     # optional attributes
     #: Inklusiver Beginn des Zeitraumes, für den der Verbrauch angegeben wird
     startdatum: Optional[datetime] = None
     #: Exklusives Ende des Zeitraumes, für den der Verbrauch angegeben wird
     enddatum: Optional[datetime] = None
-    _bis_check = validator("enddatum", always=True, allow_reuse=True)(check_bis_is_later_than_von)
+    _bis_check = field_validator("enddatum")(check_bis_is_later_than_von)
 
     @staticmethod
-    def _get_inclusive_start(values: Dict[str, Any]) -> Optional[datetime]:
+    def _get_inclusive_start(values: ValidationInfo) -> Optional[datetime]:
         """a method for easier usage of the check_bis_is_later_than_von validator"""
-        return values["startdatum"]
+        return values.data["startdatum"]  # type:ignore[attr-defined]
 
     # def _get_exclusive_end(self) -> Optional[datetime]:
     #     """a method for easier usage of the check_bis_is_later_than_von validator"""
     #     return self.enddatum
```

### Comparing `bo4e-0.4.8/src/bo4e/com/vertragskonditionen.py` & `bo4e-0.5.0/src/bo4e/com/vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/vertragsteil.py` & `bo4e-0.5.0/src/bo4e/com/vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/zaehlwerk.py` & `bo4e-0.5.0/src/bo4e/com/zaehlwerk.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,14 @@
 
     zaehlwerk_id: str  # Identifikation des Zählwerks (Registers) innerhalb des Zählers.
     # Oftmals eine laufende Nummer hinter der Zählernummer. Z.B. 47110815_1
     bezeichnung: str  # Zusätzliche Bezeichnung, z.B. Zählwerk_Wirkarbeit.
     richtung: Energierichtung  # Die Energierichtung, Einspeisung oder Ausspeisung.
     obis_kennzahl: constr(  # type: ignore[valid-type]
         strict=True,
-        regex=r"(?:(1)-((?:[0-5]?[0-9])|(?:6[0-5])):((?:[1-8]|99))\.((?:6|8|9|29))\.([0-9]{1,2}))|"
+        pattern=r"(?:(1)-((?:[0-5]?[0-9])|(?:6[0-5])):((?:[1-8]|99))\.((?:6|8|9|29))\.([0-9]{1,2}))|"
         r"(?:(7)-((?:[0-5]?[0-9])|(?:6[0-5])):(.{1,2})\.(.{1,2})\.([0-9]{1,2}))",
     )  # Die OBIS-Kennzahl für das Zählwerk, die festlegt, welche auf die gemessene Größe mit dem Stand gemeldet wird.
     # Nur Zählwerkstände mit dieser OBIS-Kennzahl werden an diesem Zählwerk registriert.
     wandlerfaktor: Decimal  # Mit diesem Faktor wird eine Zählerstandsdifferenz multipliziert, um zum eigentlichen Verbrauch im Zeitraum
     # zu kommen.
     einheit: Mengeneinheit  # Die Einheit der gemessenen Größe, z.B. kWh
```

### Comparing `bo4e-0.4.8/src/bo4e/com/zeitintervall.py` & `bo4e-0.5.0/src/bo4e/com/zeitintervall.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/zeitreihenwert.py` & `bo4e-0.5.0/src/bo4e/com/zeitreihenwert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Contains Zeitreihenwert class
 and corresponding marshmallow schema for de-/serialization
 """
 from datetime import datetime
-from typing import Any, Dict
 
-from pydantic import validator
+from pydantic import field_validator
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.com.zeitreihenwertkompakt import Zeitreihenwertkompakt
 from bo4e.validators import check_bis_is_later_than_von
 
 # pylint: disable=too-few-public-methods
 
 
@@ -25,17 +25,17 @@
         `Zeitreihenwert JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/Hochfrequenz/BO4E-python/main/json_schemas/com/Zeitreihenwert.json>`_
 
     """
 
     # required attributes
     datum_uhrzeit_von: datetime  #: Datum Uhrzeit mit Auflösung Sekunden an dem das Messintervall begonnen wurde (inklusiv)
     datum_uhrzeit_bis: datetime  #: Datum Uhrzeit mit Auflösung Sekunden an dem das Messintervall endet (exklusiv)
-    _bis_check = validator("datum_uhrzeit_bis", allow_reuse=True)(check_bis_is_later_than_von)
+    _bis_check = field_validator("datum_uhrzeit_bis")(check_bis_is_later_than_von)
 
     @staticmethod
-    def _get_inclusive_start(values: Dict[str, Any]) -> datetime:
+    def _get_inclusive_start(values: ValidationInfo) -> datetime:
         """return the inclusive start (used in the validator)"""
-        return values["datum_uhrzeit_von"]
+        return values.data["datum_uhrzeit_von"]  # type:ignore[attr-defined]
 
     # def _get_exclusive_end(self) -> datetime:
     #     """return the exclusive end (used in the validator)"""
     #     return self.datum_uhrzeit_bis
```

### Comparing `bo4e-0.4.8/src/bo4e/com/zeitreihenwertkompakt.py` & `bo4e-0.5.0/src/bo4e/com/zeitreihenwertkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/com/zustaendigkeit.py` & `bo4e-0.5.0/src/bo4e/com/zustaendigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/angebotsstatus.py` & `bo4e-0.5.0/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/artikelid.py` & `bo4e-0.5.0/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-0.5.0/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-0.5.0/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-0.5.0/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-0.5.0/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-0.5.0/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/botyp.py` & `bo4e-0.5.0/src/bo4e/enum/botyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-0.5.0/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/erzeugungsart.py` & `bo4e-0.5.0/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/gebiettyp.py` & `bo4e-0.5.0/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/geraetemerkmal.py` & `bo4e-0.5.0/src/bo4e/enum/geraetemerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/geraetetyp.py` & `bo4e-0.5.0/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-0.5.0/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-0.5.0/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/kostenklasse.py` & `bo4e-0.5.0/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/kundengruppe.py` & `bo4e-0.5.0/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/kundengruppeka.py` & `bo4e-0.5.0/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/kundentyp.py` & `bo4e-0.5.0/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/leistungstyp.py` & `bo4e-0.5.0/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/marktrolle.py` & `bo4e-0.5.0/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/mengeneinheit.py` & `bo4e-0.5.0/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/messgroesse.py` & `bo4e-0.5.0/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/messpreistyp.py` & `bo4e-0.5.0/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/messwertstatus.py` & `bo4e-0.5.0/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-0.5.0/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/netzebene.py` & `bo4e-0.5.0/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/nnrechnungstyp.py` & `bo4e-0.5.0/src/bo4e/enum/nnrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/oekolabel.py` & `bo4e-0.5.0/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/oekozertifikat.py` & `bo4e-0.5.0/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/preisgarantietyp.py` & `bo4e-0.5.0/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/preistyp.py` & `bo4e-0.5.0/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/rechnungslegung.py` & `bo4e-0.5.0/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/rechnungsstatus.py` & `bo4e-0.5.0/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/rechnungstyp.py` & `bo4e-0.5.0/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-0.5.0/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/rufnummernart.py` & `bo4e-0.5.0/src/bo4e/enum/rufnummernart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-0.5.0/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-0.5.0/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/tarifmerkmal.py` & `bo4e-0.5.0/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/themengebiet.py` & `bo4e-0.5.0/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/vertragsart.py` & `bo4e-0.5.0/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/vertragsstatus.py` & `bo4e-0.5.0/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/voraussetzungen.py` & `bo4e-0.5.0/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/waehrungscode.py` & `bo4e-0.5.0/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/zaehlertyp.py` & `bo4e-0.5.0/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/enum/zeiteinheit.py` & `bo4e-0.5.0/src/bo4e/enum/zeiteinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/src/bo4e/validators.py` & `bo4e-0.5.0/src/bo4e/validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 """
 Contains validators for BO s and COM s classes.
 """
 import re
 from datetime import datetime
-from typing import Any, Dict, Optional, Protocol
+from typing import Optional, Protocol
+
+from pydantic_core.core_schema import ValidationInfo
 
 from bo4e.enum.aufabschlagstyp import AufAbschlagstyp
 
 # pylint: disable=unused-argument
 from bo4e.enum.waehrungseinheit import Waehrungseinheit
 
 
-def einheit_only_for_abschlagstyp_absolut(cls, value: Waehrungseinheit, values: Dict[str, Any]) -> Waehrungseinheit:  # type: ignore[no-untyped-def]
+def einheit_only_for_abschlagstyp_absolut(cls, value: Waehrungseinheit, validation_info: ValidationInfo) -> Waehrungseinheit:  # type: ignore[no-untyped-def]
     """
     Check that einheit is only there if abschlagstyp is absolut.
     Currently, (2021-12-15) only used in COM AufAbschlag.
     """
+    values = validation_info.data  # type:ignore[attr-defined]
     if value and (not values["auf_abschlagstyp"] or (values["auf_abschlagstyp"] != AufAbschlagstyp.ABSOLUT)):
         raise ValueError("Only state einheit if auf_abschlagstyp is absolute.")
     return value
 
 
 # pylint:disable=too-few-public-methods
 class _VonBisType(Protocol):
     """
     a protocol for all classes that have an inclusive start and exclusive end
     """
 
     @staticmethod
-    def _get_inclusive_start(values: Dict[str, Any]) -> Optional[datetime]:
+    def _get_inclusive_start(values: ValidationInfo) -> Optional[datetime]:
         """
         should return the inclusive start of the timeslice
         """
 
     # def _get_exclusive_end(self) -> Optional[datetime]:
     #     """
     #     should return the exclusive end of the timeslice
     #     """
 
 
-def check_bis_is_later_than_von(cls, value: datetime, values: Dict[str, Any]):  # type: ignore[no-untyped-def]
+def check_bis_is_later_than_von(cls, value: datetime, values: ValidationInfo):  # type: ignore[no-untyped-def]
     """
     assert that 'bis' is later than 'von'
     """
     # we want access to private methods here because these helper methods should be "hidden"
     start = cls._get_inclusive_start(values)  # pylint: disable=protected-access
     end = value
     if start and end and not end >= start:
@@ -56,15 +59,15 @@
 OBIS_PATTERN = r"((1)-((?:[0-5]?[0-9])|(?:6[0-5])):((?:[1-8]|99))\.((?:6|8|9|29))\.([0-9]{1,2})|(7)-((?:[0-5]?[0-9])|(?:6[0-5])):(.{1,2})\.(.{1,2})\.([0-9]{1,2}))"
 # TODO: Maybe create custom data type for OBIS. See https://pydantic-docs.helpmanual.io/usage/types/#custom-data-types
 
 _malo_id_pattern = re.compile(r"^[1-9]\d{10}$")
 
 
 # pylint: disable=unused-argument
-def validate_marktlokations_id(cls, marktlokations_id: str, values: Dict[str, Any]) -> str:  # type: ignore[no-untyped-def]
+def validate_marktlokations_id(cls, marktlokations_id: str, values: ValidationInfo) -> str:  # type: ignore[no-untyped-def]
     """
     A validator for marktlokations IDs
     """
     if not marktlokations_id:
         raise ValueError("The marktlokations_id must not be empty.")
     if not _malo_id_pattern.match(marktlokations_id):
         raise ValueError(f"The Marktlokations-ID '{marktlokations_id}' does not match {_malo_id_pattern.pattern}")
```

### Comparing `bo4e-0.4.8/src/bo4e.egg-info/PKG-INFO` & `bo4e-0.5.0/src/bo4e.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bo4e
-Version: 0.4.8
+Version: 0.5.0
 Summary: Python Library that implements the BO4E Standard.
 Home-page: https://github.com/Hochfrequenz/BO4E-python
 Author: Kevin Krechan
 Author-email: kevin.krechan@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Project-URL: Code, https://github.com/Hochfrequenz/BO4E-python
```

### Comparing `bo4e-0.4.8/src/bo4e.egg-info/SOURCES.txt` & `bo4e-0.5.0/src/bo4e.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,15 @@
 src/bo4e/enum/voraussetzungen.py
 src/bo4e/enum/waehrungscode.py
 src/bo4e/enum/waehrungseinheit.py
 src/bo4e/enum/wertermittlungsverfahren.py
 src/bo4e/enum/zaehlerauspraegung.py
 src/bo4e/enum/zaehlertyp.py
 src/bo4e/enum/zeiteinheit.py
+src/bo4e/utils/__init__.py
 tests/__init__.py
 tests/serialization_helper.py
 tests/test_adresse.py
 tests/test_angebot.py
 tests/test_angebotsposition.py
 tests/test_angebotsteil.py
 tests/test_angebotsvariante.py
@@ -339,14 +340,15 @@
 tests/test_aufabschlagstaffelproort.py
 tests/test_ausschreibung.py
 tests/test_ausschreibungsdetail.py
 tests/test_ausschreibungslos.py
 tests/test_betrag.py
 tests/test_buendelvertrag.py
 tests/test_bypassing_validation.py
+tests/test_doc_utils.py
 tests/test_energieherkunft.py
 tests/test_energiemenge.py
 tests/test_energiemix.py
 tests/test_enums.py
 tests/test_externe_referenz.py
 tests/test_fremdkosten.py
 tests/test_fremdkostenblock.py
```

### Comparing `bo4e-0.4.8/tests/serialization_helper.py` & `bo4e-0.5.0/tests/serialization_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 def assert_serialization_roundtrip(serializable_object: T, expected_json_dict: Optional[Dict[str, Any]] = None) -> T:
     """
     Serializes the serializable_object using the provided schema,
     then asserts, that the result is equal to the expected_json_dict (if given),
     then deserializes the dictionary again and asserts the equality with the original serializable_object
     :returns the deserialized_object
     """
-    json_string = serializable_object.json(by_alias=True, ensure_ascii=False)  # type: ignore[attr-defined]
+    json_string = serializable_object.model_dump_json(by_alias=True)  # type: ignore[attr-defined]
     assert json_string is not None
-    actual_json_dict = serializable_object.dict(by_alias=True)  # type: ignore[attr-defined]
+    actual_json_dict = serializable_object.model_dump(by_alias=True)  # type: ignore[attr-defined]
     assert actual_json_dict is not None
     # TODO: serializable_object.dict()
     if expected_json_dict is not None:
         assert all([(k in json_string) for k in expected_json_dict.keys()])
         assert actual_json_dict == expected_json_dict, (
             f"actual_json_dict != expected_json_dict\n\t" f"diff = {list(diff(expected_json_dict, actual_json_dict))}"
         )
         # this (diff(...)) contains the difference between two dicts -> just for easier debugging
 
-    deserialized_object = type(serializable_object).parse_raw(json_string)  # type: ignore[attr-defined]
+    deserialized_object = type(serializable_object).model_validate_json(json_string)  # type: ignore[attr-defined]
     assert isinstance(deserialized_object, type(serializable_object))
     assert deserialized_object == serializable_object
     return deserialized_object
```

### Comparing `bo4e-0.4.8/tests/test_adresse.py` & `bo4e-0.5.0/tests/test_adresse.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,22 +28,22 @@
         """
 
         address_test_data = Adresse.parse_file(
             "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json",
             encoding="utf-8",
         )
 
-        address_dict = address_test_data.json(by_alias=True, ensure_ascii=False)
+        address_dict = address_test_data.model_dump_json(by_alias=True)
 
         assert "Nördliche Münchner Straße" in address_dict
         assert "27A" in address_dict
         assert "82031" in address_dict
         assert "DE" in address_dict
 
-        deserialized_address = Adresse.parse_raw(address_dict)
+        deserialized_address = Adresse.model_validate_json(address_dict)
 
         assert isinstance(deserialized_address, Adresse)
         assert deserialized_address.strasse == "Nördliche Münchner Straße"
         assert deserialized_address.hausnummer == "27A"
         assert deserialized_address.postleitzahl == "82031"
         assert deserialized_address.landescode == Landescode.DE  # type: ignore[attr-defined]
 
@@ -57,21 +57,21 @@
 
         a = Adresse(
             postleitzahl=address_test_data["postleitzahl"],
             ort=address_test_data["ort"],
             postfach=address_test_data["postfach"],
         )
 
-        address_json = a.json(by_alias=True, ensure_ascii=False)
+        address_json = a.model_dump_json(by_alias=True)
 
         assert "10 64 38" in address_json
         assert "82031" in address_json
         assert "DE" in address_json
 
-        deserialized_address = Adresse.parse_raw(address_json)
+        deserialized_address = Adresse.model_validate_json(address_json)
 
         assert isinstance(deserialized_address, Adresse)
         assert deserialized_address.postfach == "10 64 38"
         assert deserialized_address.postleitzahl == "82031"
         assert deserialized_address.landescode == Landescode.DE  # type: ignore[attr-defined]
 
     def test_serialization_only_required_fields(self) -> None:
@@ -82,45 +82,45 @@
         }
 
         a = Adresse(
             postleitzahl=address_test_data["postleitzahl"],
             ort=address_test_data["ort"],
         )
 
-        address_json = a.json(by_alias=True, ensure_ascii=False)
+        address_json = a.model_dump_json(by_alias=True)
 
         assert "Grünwald" in address_json
         assert "82031" in address_json
 
-        deserialized_address = Adresse.parse_raw(address_json)
+        deserialized_address = Adresse.model_validate_json(address_json)
 
         assert isinstance(deserialized_address, Adresse)
         assert deserialized_address.ort == "Grünwald"
         assert deserialized_address.postleitzahl == "82031"
 
     def test_serialization_only_required_fields_landescode_AT(self) -> None:
         address_test_data = Adresse.parse_file(
             "./tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json",
             encoding="utf-8",
         )
         address_test_data.landescode = Landescode.AT  # type: ignore[attr-defined]
 
-        address_json = address_test_data.json(by_alias=True, ensure_ascii=False)
-        deserialized_address = Adresse.parse_raw(address_json)
+        address_json = address_test_data.model_dump_json(by_alias=True)
+        deserialized_address = Adresse.model_validate_json(address_json)
 
         assert deserialized_address.landescode == Landescode.AT  # type: ignore[attr-defined]
 
     def test_deserialization(self) -> None:
         json_string = r"""{"strasse":"Getreidegasse",
                  "hausnummer":"9",
                  "ort":"Salzburg",
                  "postleitzahl":"5020",
                  "landescode":"AT"}"""
 
-        a: Adresse = Adresse.parse_raw(json_string)
+        a: Adresse = Adresse.model_validate_json(json_string)
         assert a.landescode is Landescode.AT  # type: ignore[attr-defined]
 
     @pytest.mark.datafiles("./tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json")
     def test_missing_required_attribute(self, datafiles: Path) -> None:
         """
         Test for getting an error message if a required attribute is missing
         """
@@ -195,17 +195,17 @@
         Minimal working example
         :return:
         """
         a = Adresse(
             postleitzahl="6413", ort="Wildermieming", strasse="Gerhardhof", hausnummer="1", landescode=Landescode.AT  # type: ignore[attr-defined]
         )
         assert a.landescode == Landescode.AT  # type: ignore[attr-defined]
-        serialized_address = a.json(by_alias=True, ensure_ascii=False)
+        serialized_address = a.model_dump_json(by_alias=True)
         assert '"AT"' in serialized_address
-        deserialized_address = Adresse.parse_raw(serialized_address)
+        deserialized_address = Adresse.model_validate_json(serialized_address)
         assert deserialized_address.landescode == Landescode.AT  # type: ignore[attr-defined]
 
     @pytest.mark.parametrize(
         "address_json, adresse",
         [
             pytest.param(
                 r"""{"postleitzahl": "12345", 
@@ -230,21 +230,21 @@
         ],
     )
     def test_serialization_with_all_possible_fields(self, address_json: str, adresse: Adresse) -> None:
         """
         Test serialization with all required and optional attributes
         """
 
-        serialized_address = adresse.json(by_alias=True, ensure_ascii=False)
+        serialized_address = adresse.model_dump_json(by_alias=True)
 
         assert "ISS spacestation" in serialized_address
         assert "12345" in serialized_address
         assert "Milky Way" in serialized_address
         assert "42" in serialized_address
         assert "FR" in serialized_address
         assert "to whom it may concern" in serialized_address
         assert "you will find me" in serialized_address
         assert "Mitte" in serialized_address
 
-        deserialized_address = Adresse.parse_raw(address_json)
+        deserialized_address = Adresse.model_validate_json(address_json)
 
         assert deserialized_address == adresse
```

### Comparing `bo4e-0.4.8/tests/test_angebot.py` & `bo4e-0.5.0/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_angebotsposition.py` & `bo4e-0.5.0/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_angebotsteil.py` & `bo4e-0.5.0/tests/test_angebotsteil.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,13 +184,13 @@
         assert_serialization_roundtrip(angebotsteil, expected_json_dict)
 
     def test_angebotsteil_positionen_required(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Angebotsteil(positionen=[])
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Angebotsteil()  # type: ignore[call-arg]
         assert "1 validation error" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_angebotsvariante.py` & `bo4e-0.5.0/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_ansprechpartner.py` & `bo4e-0.5.0/tests/test_ansprechpartner.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,20 +41,20 @@
                     hausnummer="540a",
                 ),
             ),
         )
         assert ansprechpartner.versionstruktur == "2", "versionstruktur was not automatically set"
         assert ansprechpartner.bo_typ is BoTyp.ANSPRECHPARTNER, "boTyp was not automatically set"
 
-        json_string = ansprechpartner.json(by_alias=True, ensure_ascii=False)
+        json_string = ansprechpartner.model_dump_json(by_alias=True)
         assert "Müller-Schmidt" in json_string
         assert "Mühlenweg" in json_string
         assert '"FRAU"' in json_string
 
-        deserialized_ansprechpartner = Ansprechpartner.parse_raw(json_string)
+        deserialized_ansprechpartner = Ansprechpartner.model_validate_json(json_string)
 
         assert isinstance(deserialized_ansprechpartner, Ansprechpartner)
         assert isinstance(deserialized_ansprechpartner.geschaeftspartner, Geschaeftspartner)
         assert deserialized_ansprechpartner == ansprechpartner
 
     def test_de_serialisation_maximal_attributes(self) -> None:
         """
@@ -101,20 +101,20 @@
             zustaendigkeit=Zustaendigkeit(
                 themengebiet=Themengebiet.MARKTKOMMUNIKATION, jobtitel="Schatzmeister", abteilung="unten rechts"
             ),
         )
         assert ansprechpartner.versionstruktur == "2", "versionstruktur was not automatically set"
         assert ansprechpartner.bo_typ is BoTyp.ANSPRECHPARTNER, "boTyp was not automatically set"
 
-        json_string = ansprechpartner.json(by_alias=True, ensure_ascii=False)
+        json_string = ansprechpartner.model_dump_json(by_alias=True)
         assert "Müller-Schmidt" in json_string
         assert "Mühlenweg" in json_string
         assert "PROF_DR" in json_string
 
-        deserialized_ansprechpartner = Ansprechpartner.parse_raw(json_string)
+        deserialized_ansprechpartner = Ansprechpartner.model_validate_json(json_string)
 
         assert isinstance(deserialized_ansprechpartner, Ansprechpartner)
         assert isinstance(deserialized_ansprechpartner.geschaeftspartner, Geschaeftspartner)
         assert isinstance(deserialized_ansprechpartner.adresse, Adresse)
         assert isinstance(deserialized_ansprechpartner.rufnummer, Rufnummer)
         assert isinstance(deserialized_ansprechpartner.zustaendigkeit, Zustaendigkeit)
         assert deserialized_ansprechpartner == ansprechpartner
```

### Comparing `bo4e-0.4.8/tests/test_aufabschlag.py` & `bo4e-0.5.0/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_aufabschlagproort.py` & `bo4e-0.5.0/tests/test_aufabschlagproort.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,8 +61,8 @@
                 postleitzahl="01187",
                 ort="Dresden",
                 netznr="2",
                 staffeln=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_aufabschlagregional.py` & `bo4e-0.5.0/tests/test_aufabschlagregional.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,8 +232,8 @@
                 AufAbschlagRegional(
                     bezeichnung="foo",
                     betraege=[],
                 ),
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_aufabschlagstaffelproort.py` & `bo4e-0.5.0/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_ausschreibung.py` & `bo4e-0.5.0/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_ausschreibungsdetail.py` & `bo4e-0.5.0/tests/test_ausschreibungsdetail.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from bo4e.enum.landescode import Landescode
 from bo4e.enum.mengeneinheit import Mengeneinheit
 from bo4e.enum.netzebene import Netzebene
 from bo4e.enum.zaehlertyp import Zaehlertyp
 from bo4e.enum.zeiteinheit import Zeiteinheit
 from tests.serialization_helper import assert_serialization_roundtrip
 from tests.test_adresse import example_adresse
-from tests.test_menge import example_menge
 from tests.test_zeitraum import example_zeitraum
 
 example_ausschreibungsdetail = Ausschreibungsdetail(
     marktlokations_id="56789012345",
     netzebene_lieferung=Netzebene.MSP,
     netzebene_messung=Netzebene.NSP,
     marktlokationsadresse=example_adresse,
```

### Comparing `bo4e-0.4.8/tests/test_ausschreibungslos.py` & `bo4e-0.5.0/tests/test_ausschreibungslos.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,13 +85,13 @@
                 anzahl_lieferstellen=17,
                 lieferzeitraum=example_zeitraum,
                 ## ^^ above is just clutter
                 lieferstellen=[],  # the important line
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Ausschreibungslos()  # type: ignore[call-arg]
         assert "10 validation errors" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_betrag.py` & `bo4e-0.5.0/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_buendelvertrag.py` & `bo4e-0.5.0/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_bypassing_validation.py` & `bo4e-0.5.0/tests/test_bypassing_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import inspect
-import json
 
 import pytest
 from pydantic import ValidationError
 
 from bo4e.bo.marktlokation import Marktlokation
 from bo4e.com.adresse import Adresse
 from bo4e.enum.bilanzierungsmethode import Bilanzierungsmethode
@@ -33,22 +32,22 @@
             )
             return malo
 
         # now, instantiation will fail:
         with pytest.raises(ValidationError) as validation_error:
             instantiate_with_constructor()
         error_msg = str(validation_error.value).replace("\n", " ").replace("\r", " ").replace("  ", " ")
-        assert "1 validation error for Marktlokation netzebene  field required" in error_msg
+        assert "1 validation error for Marktlokation netzebene  Field required" in error_msg
 
         # You're in a dilemma:
         # - either you cannot instantiate the BO, although you'd like to use BO4E
         # - or you have to guess values/enter dummy data which you cannot distinguish from real data later on.
         # The workaround is to use construct:
         def instantiate_with_construct() -> Marktlokation:
-            malo = Marktlokation.construct(  # type:ignore[call-arg] # silence mypy complaints about the netzebene
+            malo = Marktlokation.model_construct(  # type:ignore[call-arg] # silence mypy complaints about the netzebene
                 marktlokations_id="51238696781",
                 sparte=Sparte.GAS,
                 lokationsadresse=Adresse(
                     postleitzahl="04109", ort="Leipzig", hausnummer="15", strasse="Thomaskirchhof"
                 ),
                 energierichtung=Energierichtung.EINSP,
                 bilanzierungsmethode=Bilanzierungsmethode.PAUSCHAL,
@@ -61,12 +60,12 @@
         assert isinstance(marktlokation, Marktlokation)  # Now the object is still a Marktlokation
         # but it has no member netzebene
         assert not any(m for m in inspect.getmembers(marktlokation) if m[0] == "netzebene")
         # and trying to access the missing netzebene raises an AttributeError:
         with pytest.raises(AttributeError):
             _ = marktlokation.netzebene
         # you can still serialize the invalid malo
-        malo_json_str = marktlokation.json()  # works
+        malo_json_str = marktlokation.model_dump_json()  # works
         assert malo_json_str is not None
         # but deserializing raises an error:
         with pytest.raises(ValidationError):
-            Marktlokation.parse_raw(malo_json_str)
+            Marktlokation.model_validate_json(malo_json_str)
```

### Comparing `bo4e-0.4.8/tests/test_energieherkunft.py` & `bo4e-0.5.0/tests/test_energieherkunft.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,10 +47,8 @@
         ],
     )
     def test_energieherkunft_failing_validation(self, failing_percentage: float) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = (Energieherkunft(erzeugungsart=Erzeugungsart.BIOMASSE, anteil_prozent=Decimal(failing_percentage)),)
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value is less than 100" in str(
-            excinfo.value
-        ) or "ensure this value is greater than 0" in str(excinfo.value)
+        assert "should be less than 100" in str(excinfo.value) or "should be greater than 0" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_energiemenge.py` & `bo4e-0.5.0/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_energiemix.py` & `bo4e-0.5.0/tests/test_energiemix.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,8 +128,8 @@
                 energieart=Sparte.STROM,
                 bezeichnung="foo",
                 gueltigkeitsjahr=2021,
                 anteil=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_enums.py` & `bo4e-0.5.0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_externe_referenz.py` & `bo4e-0.5.0/tests/test_externe_referenz.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from bo4e.enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
 
 
 class TestExterneReferenz:
     def test_serialization(self) -> None:
         er = ExterneReferenz(ex_ref_name="HOCHFREQUENZ_HFSAP_100", ex_ref_wert="12345")
 
-        er_json = er.json(by_alias=True, ensure_ascii=False)
+        er_json = er.model_dump_json(by_alias=True)
 
         assert "exRefName" in er_json
 
-        deserialized_er: ExterneReferenz = ExterneReferenz.parse_raw(er_json)
+        deserialized_er: ExterneReferenz = ExterneReferenz.model_validate_json(er_json)
         assert isinstance(deserialized_er, ExterneReferenz)
         assert deserialized_er == er
 
     def test_list_of_externe_referenz(self) -> None:
         gp = Geschaeftspartner(
             externe_referenzen=[
                 ExterneReferenz(ex_ref_name="SAP GP Nummer", ex_ref_wert="0123456789"),
@@ -33,17 +33,17 @@
                 strasse="Am Geldspeicher",
                 hausnummer="17",
                 postleitzahl="88101",
                 ort="Entenhausen",
             ),
         )
 
-        gp_json = gp.json(by_alias=True, ensure_ascii=False)
+        gp_json = gp.model_dump_json(by_alias=True)
 
-        deserialized_gp: Geschaeftspartner = Geschaeftspartner.parse_raw(gp_json)
+        deserialized_gp: Geschaeftspartner = Geschaeftspartner.model_validate_json(gp_json)
         assert len(deserialized_gp.externe_referenzen) == 2  # type: ignore[arg-type]
         assert deserialized_gp.externe_referenzen[0].ex_ref_name == "SAP GP Nummer"  # type: ignore[index]
 
     def test_geschaeftspartner_with_no_externe_referenz(self) -> None:
         gp = Geschaeftspartner(
             # just some dummy data to make the GP valid
             name1="Duck",
@@ -54,23 +54,23 @@
                 strasse="Am Geldspeicher",
                 hausnummer="17",
                 postleitzahl="88101",
                 ort="Entenhausen",
             ),
         )
 
-        gp_json = gp.json(by_alias=True, ensure_ascii=False)
+        gp_json = gp.model_dump_json(by_alias=True)
 
-        deserialized_gp: Geschaeftspartner = Geschaeftspartner.parse_raw(gp_json)
+        deserialized_gp: Geschaeftspartner = Geschaeftspartner.model_validate_json(gp_json)
 
         assert deserialized_gp.externe_referenzen == []
 
     def test_extension_data(self) -> None:
         """
         tests the behaviour of the json extension data (`extra="allow"`)
         """
         er = ExterneReferenz(ex_ref_name="foo.bar", ex_ref_wert="12345")
-        er_json: Dict[str, Any] = er.dict()
+        er_json: Dict[str, Any] = er.model_dump()
         er_json["additional_key"] = "additional_value"
         deserialized_er: ExterneReferenz = ExterneReferenz.parse_obj(er_json)
         assert isinstance(deserialized_er, ExterneReferenz)
         assert deserialized_er.additional_key == "additional_value"  # type:ignore[attr-defined]
```

### Comparing `bo4e-0.4.8/tests/test_fremdkosten.py` & `bo4e-0.5.0/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_fremdkostenblock.py` & `bo4e-0.5.0/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_fremdkostenposition.py` & `bo4e-0.5.0/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_geokoordinaten.py` & `bo4e-0.5.0/tests/test_geokoordinaten.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 class TestGeokoordinaten:
     def test_serialization(self) -> None:
         geo = Geokoordinaten(
             breitengrad=Decimal(52.52149200439453),
             laengengrad=Decimal(13.404866218566895),
         )
 
-        json_string = geo.json(by_alias=True, ensure_ascii=False)
+        json_string = geo.model_dump_json(by_alias=True)
 
         assert "breitengrad" in json_string
         assert str(geo.breitengrad) in json_string
 
-        deserialized_geo: Geokoordinaten = Geokoordinaten.parse_raw(json_string)
+        deserialized_geo: Geokoordinaten = Geokoordinaten.model_validate_json(json_string)
 
         assert isinstance(deserialized_geo.breitengrad, Decimal)
         assert isinstance(deserialized_geo.laengengrad, Decimal)
         assert geo.breitengrad == deserialized_geo.breitengrad
 
     def test_wrong_datatype(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
```

### Comparing `bo4e-0.4.8/tests/test_geraet.py` & `bo4e-0.5.0/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_geraeteeigenschaften.py` & `bo4e-0.5.0/tests/test_geraeteeigenschaften.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,8 +45,8 @@
         ],
     )
     def test_failing_validation(self, not_a_geraetetyp: Any) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Geraeteeigenschaften(geraetemerkmal=Geraetemerkmal.GAS_G1000, geraetetyp=not_a_geraetetyp)
 
         assert "1 validation error" in str(excinfo.value)
-        assert "value is not a valid enumeration member" in str(excinfo.value)
+        assert "string_type" in str(excinfo.value) or "type=enum" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_geschaeftsobjekt.py` & `bo4e-0.5.0/tests/test_geschaeftsobjekt.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,19 +34,19 @@
         go = Geschaeftsobjekt(
             bo_typ=bo_typ,
             versionstruktur=versionstruktur,
             externe_referenzen=externe_referenzen,
         )
         assert isinstance(go, Geschaeftsobjekt)
 
-        go_json = go.json(by_alias=True, ensure_ascii=False)
+        go_json = go.model_dump_json(by_alias=True)
 
         assert str(versionstruktur) in go_json
 
-        go_deserialized = Geschaeftsobjekt.parse_raw(go_json)
+        go_deserialized = Geschaeftsobjekt.model_validate_json(go_json)
 
         assert go_deserialized.bo_typ is bo_typ
         assert go_deserialized.versionstruktur == versionstruktur
         assert go_deserialized.externe_referenzen == externe_referenzen
 
     def test_initialization_with_minimal_attributs(self) -> None:
         go = Geschaeftsobjekt(bo_typ=BoTyp.ANSPRECHPARTNER)
@@ -56,9 +56,9 @@
 
     def test_no_list_in_externen_referenzen(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Geschaeftsobjekt(
                 bo_typ=BoTyp.ENERGIEMENGE,
                 externe_referenzen=ExterneReferenz(ex_ref_name="Schufa-ID", ex_ref_wert="aksdlakoeuhn"),  # type: ignore[arg-type]
             )
-        assert "1 validation error" in str(excinfo.value)
-        assert "value is not a valid list" in str(excinfo.value)
+        assert "2 validation error" in str(excinfo.value)
+        assert "type=model_type" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_geschaeftspartner.py` & `bo4e-0.5.0/tests/test_geschaeftspartner.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,19 +40,19 @@
                 hausnummer=address_test_data["hausnummer"],
             ),
         )
 
         # test default value for bo_typ in Geschaeftspartner
         assert gp.bo_typ == BoTyp.GESCHAEFTSPARTNER
 
-        gp_json = gp.json(by_alias=True, ensure_ascii=False)
+        gp_json = gp.model_dump_json(by_alias=True)
 
         assert "Helga" in gp_json
 
-        gp_deserialized = Geschaeftspartner.parse_raw(gp_json)
+        gp_deserialized = Geschaeftspartner.model_validate_json(gp_json)
 
         assert gp_deserialized.bo_typ == gp.bo_typ
         assert type(gp_deserialized.partneradresse) == Adresse
 
     def test_optional_attribute_partneradresse(self) -> None:
         """
         The BO4E standard does not yet define whether the partneradresse is mandatory or not.
@@ -73,16 +73,16 @@
             umsatzsteuer_id="DE267311963",
             glaeubiger_id="DE98ZZZ09999999999",
             e_mail_adresse="test@bo4e.de",
             website="bo4e.de",
             geschaeftspartnerrolle=[Geschaeftspartnerrolle.DIENSTLEISTER],
         )
 
-        gp_json = gp.json(by_alias=True, ensure_ascii=False)
-        gp_deserialized = Geschaeftspartner.parse_raw(gp_json)
+        gp_json = gp.model_dump_json(by_alias=True)
+        gp_deserialized = Geschaeftspartner.model_validate_json(gp_json)
 
         assert gp_deserialized.partneradresse is None
 
     def test_list_validation_of_geschaeftspartnerrolle(self) -> None:
         """
         Tests that if the geschaeftspartnerrolle of Geschaeftspartner is not a list, an error is raised.
 
@@ -111,15 +111,15 @@
                     ort="Dresden",
                     strasse="Goethestraße",
                     hausnummer="1",
                 ),
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "value is not a valid list" in str(excinfo.value)
+        assert "type=list_type" in str(excinfo.value)
 
     def test_serialization_of_non_german_address(self) -> None:
         """
         Test that partneradresses with a Landescode!=DE (default) are (de)serialized correctly.
         """
         gp = Geschaeftspartner(
             anrede=Anrede.FRAU,
@@ -132,10 +132,10 @@
             kontaktweg=[Kontaktart.E_MAIL],
             umsatzsteuer_id="AT12345",
             geschaeftspartnerrolle=[Geschaeftspartnerrolle.DIENSTLEISTER],
             partneradresse=Adresse(
                 postleitzahl="1014", ort="Wien 1", strasse="Ballhausplatz", hausnummer="2", landescode=Landescode.AT  # type: ignore[attr-defined]
             ),
         )
-        gp_json = gp.json(by_alias=True, ensure_ascii=False)
-        gp_deserialized = Geschaeftspartner.parse_raw(gp_json)
+        gp_json = gp.model_dump_json(by_alias=True)
+        gp_deserialized = Geschaeftspartner.model_validate_json(gp_json)
         assert gp_deserialized.partneradresse.landescode == Landescode.AT  # type: ignore[attr-defined, union-attr]
```

### Comparing `bo4e-0.4.8/tests/test_kosten.py` & `bo4e-0.5.0/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_kostenblock.py` & `bo4e-0.5.0/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_kostenposition.py` & `bo4e-0.5.0/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_kriteriumswert.py` & `bo4e-0.5.0/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_lastgang.py` & `bo4e-0.5.0/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_lastgangkompakt.py` & `bo4e-0.5.0/tests/test_lastgangkompakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_marktlokation.py` & `bo4e-0.5.0/tests/test_marktlokation.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,20 +31,20 @@
             energierichtung=Energierichtung.EINSP,
             bilanzierungsmethode=Bilanzierungsmethode.PAUSCHAL,
             netzebene=Netzebene.NSP,
         )
         assert malo.versionstruktur == "2", "versionstruktur was not automatically set"
         assert malo.bo_typ is BoTyp.MARKTLOKATION, "boTyp was not automatically set"
 
-        json_string = malo.json(by_alias=True, ensure_ascii=False)
+        json_string = malo.model_dump_json(by_alias=True)
 
         assert "boTyp" in json_string, "No camel case serialization"
         assert "marktlokationsId" in json_string, "No camel case serialization"
 
-        deserialized_malo: Marktlokation = Marktlokation.parse_raw(json_string)
+        deserialized_malo: Marktlokation = Marktlokation.model_validate_json(json_string)
 
         # check that `deserialized_malo.marktlokations_id` and `malo.marktlokations_id` have the same value
         # but are **not** the same object.
         assert deserialized_malo.marktlokations_id == malo.marktlokations_id
         assert deserialized_malo.marktlokations_id is not malo.marktlokations_id
         assert deserialized_malo.bo_typ is BoTyp.MARKTLOKATION
 
@@ -83,20 +83,20 @@
             netzebene=Netzebene.NSP,
             endkunde=gp,
             kundengruppen=[Kundentyp.GEWERBE, Kundentyp.PRIVAT],
         )
         assert malo.versionstruktur == "2", "versionstruktur was not automatically set"
         assert malo.bo_typ == BoTyp.MARKTLOKATION, "boTyp was not automatically set"
 
-        json_string = malo.json(by_alias=True, ensure_ascii=False)
+        json_string = malo.model_dump_json(by_alias=True)
 
         assert "boTyp" in json_string, "No camel case serialization"
         assert "marktlokationsId" in json_string, "No camel case serialization"
 
-        deserialized_malo: Marktlokation = Marktlokation.parse_raw(json_string)
+        deserialized_malo: Marktlokation = Marktlokation.model_validate_json(json_string)
 
         assert deserialized_malo.marktlokations_id == malo.marktlokations_id
         assert deserialized_malo.marktlokations_id is not malo.marktlokations_id
         assert deserialized_malo.bo_typ is BoTyp.MARKTLOKATION
         assert deserialized_malo.endkunde == gp
 
     def test_missing_required_fields(self) -> None:
@@ -133,19 +133,19 @@
             "geoadresse": null,
             "bilanzierungsmethode": "PAUSCHAL",
             "versionstruktur": "2",
             "energierichtung": "EINSP"
             }"""
 
         with pytest.raises(ValidationError) as excinfo:
-            Marktlokation.parse_raw(invalid_json_string)
+            Marktlokation.model_validate_json(invalid_json_string)
 
         assert "1 validation error" in str(excinfo.value)
         assert "marktlokationsId" in str(excinfo.value)
-        assert "field required" in str(excinfo.value)
+        assert "Field required" in str(excinfo.value)
 
     def test_address_validation(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Marktlokation(
                 marktlokations_id="51238696781",
                 sparte=Sparte.GAS,
                 lokationsadresse=Adresse(
```

### Comparing `bo4e-0.4.8/tests/test_marktteilnehmer.py` & `bo4e-0.5.0/tests/test_marktteilnehmer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 class TestMarktteilnehmer:
     def test_serialization(self) -> None:
         mt = example_marktteilnehmer
 
         assert mt.versionstruktur == "2", "versionstruktur was not automatically set"
         assert mt.bo_typ == BoTyp.MARKTTEILNEHMER, "boTyp was not automatically set"
 
-        json_string = mt.json(by_alias=True, ensure_ascii=False)
+        json_string = mt.model_dump_json(by_alias=True)
         json_dict = json.loads(json_string)
 
         # Test camelcase
         assert "boTyp" in json_dict
         assert "marktrolle" in json_dict
 
-        deserialized_mt: Marktteilnehmer = Marktteilnehmer.parse_raw(json_string)
+        deserialized_mt: Marktteilnehmer = Marktteilnehmer.model_validate_json(json_string)
 
         assert mt.marktrolle is deserialized_mt.marktrolle
         # Test snakecase
         assert deserialized_mt.bo_typ is BoTyp.MARKTTEILNEHMER
```

### Comparing `bo4e-0.4.8/tests/test_menge.py` & `bo4e-0.5.0/tests/test_menge.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 class TestMenge:
     def test_menge(self) -> None:
         """
         Test de-/serialisation of Menge (only has required attributes).
         """
 
-        json_string = example_menge.json(by_alias=True, ensure_ascii=False)
+        json_string = example_menge.model_dump_json(by_alias=True)
 
         assert "3.41" in json_string
         assert "MWH" in json_string
 
-        menge_deserialized = Menge.parse_raw(json_string)
+        menge_deserialized = Menge.model_validate_json(json_string)
 
         assert isinstance(menge_deserialized.wert, Decimal)
         assert menge_deserialized.wert == Decimal(3.41)
         assert isinstance(menge_deserialized.einheit, Mengeneinheit)
         assert menge_deserialized.einheit == Mengeneinheit.MWH
 
     def test_wrong_datatype(self) -> None:
```

### Comparing `bo4e-0.4.8/tests/test_messlokation.py` & `bo4e-0.5.0/tests/test_messlokation.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,21 @@
         melo = Messlokation(
             messlokations_id="DE00056266802AO6G56M11SN51G21M24S",
             sparte=Sparte.STROM,
         )
         assert melo.versionstruktur == "2", "versionstruktur was not automatically set"
         assert melo.bo_typ is BoTyp.MESSLOKATION, "boTyp was not automatically set"
 
-        json_string = melo.json(by_alias=True, ensure_ascii=False)
+        json_string = melo.model_dump_json(by_alias=True)
         json_dict = json.loads(json_string)
 
         assert "boTyp" in json_dict, "No camel case serialization"
         assert "messlokationsId" in json_dict, "No camel case serialization"
 
-        deserialized_melo: Messlokation = Messlokation.parse_raw(json_string)
+        deserialized_melo: Messlokation = Messlokation.model_validate_json(json_string)
 
         # check that `deserialized_malo.marktlokations_id` and `malo.marktlokations_id` have the same value
         # but are **not** the same object.
         assert deserialized_melo.messlokations_id == melo.messlokations_id
         assert deserialized_melo.messlokations_id is not melo.messlokations_id
         assert deserialized_melo.bo_typ is BoTyp.MESSLOKATION
 
@@ -104,21 +104,21 @@
             ],
             grundzustaendiger_msb_codenr="9910125000002",
             messadresse=Adresse(postleitzahl="04177", ort="Leipzig", hausnummer="1", strasse="Jahnalle"),
         )
         assert melo.versionstruktur == "2", "versionstruktur was not automatically set"
         assert melo.bo_typ == BoTyp.MESSLOKATION, "boTyp was not automatically set"
 
-        json_string = melo.json(by_alias=True, ensure_ascii=False)
+        json_string = melo.model_dump_json(by_alias=True)
         json_dict = json.loads(json_string)
 
         assert "boTyp" in json_dict, "No camel case serialization"
         assert "messlokationsId" in json_dict, "No camel case serialization"
 
-        deserialized_melo: Messlokation = Messlokation.parse_raw(json_string)
+        deserialized_melo: Messlokation = Messlokation.model_validate_json(json_string)
 
         assert deserialized_melo.messlokations_id == melo.messlokations_id
         assert deserialized_melo.messlokations_id is not melo.messlokations_id
         assert deserialized_melo.bo_typ is BoTyp.MESSLOKATION
 
     def test_missing_required_fields(self) -> None:
         """
@@ -151,15 +151,15 @@
                 "geoadresse": null,
                 "versionstruktur": "2",
                 "grundzustaendigerMsbimCodenr": null
                 }
                 """
 
         with pytest.raises(ValidationError) as excinfo:
-            Messlokation.parse_raw(invalid_json_string)
+            Messlokation.model_validate_json(invalid_json_string)
 
         assert "messlokationsId" in str(excinfo.value)
 
     def test_address_validation(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Messlokation(
                 messlokations_id="DE00056266802AO6G56M11SN51G21M24S",
@@ -220,12 +220,12 @@
         """
         tests the behaviour of the json extension data (`extra="allow"`)
         """
         melo = Messlokation(
             messlokations_id="DE00056266802AO6G56M11SN51G21M24S",
             sparte=Sparte.STROM,
         )
-        melo_json: Dict[str, Any] = melo.dict()
+        melo_json: Dict[str, Any] = melo.model_dump()
         melo_json["additional_key"] = "additional_value"
         deserialized_melo: Messlokation = Messlokation.parse_obj(melo_json)
         assert isinstance(deserialized_melo, Messlokation)
         assert deserialized_melo.additional_key == "additional_value"  # type:ignore[attr-defined]
```

### Comparing `bo4e-0.4.8/tests/test_messlokationszuordnung.py` & `bo4e-0.5.0/tests/test_messlokationszuordnung.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,20 +12,20 @@
         messlokations_id = "DE0010688516810000000000000012345"
 
         mlz = Messlokationszuordnung(
             messlokations_id=messlokations_id,
             arithmetik=ArithmetischeOperation.ADDITION,
         )
 
-        json_string = mlz.json(by_alias=True, ensure_ascii=False)
+        json_string = mlz.model_dump_json(by_alias=True)
 
         assert messlokations_id in json_string
         assert "ADDITION" in json_string
 
-        mlz_deserialized = Messlokationszuordnung.parse_raw(json_string)
+        mlz_deserialized = Messlokationszuordnung.model_validate_json(json_string)
 
         assert mlz_deserialized.messlokations_id == messlokations_id
         assert mlz_deserialized.arithmetik == ArithmetischeOperation.ADDITION
 
     def test_serialisation_required_and_optional_attributes(self) -> None:
         """
         Test serialisation of Messlokationszuordnung with required and optional attributes
@@ -35,24 +35,24 @@
         mlz = Messlokationszuordnung(
             messlokations_id=messlokations_id,
             arithmetik=ArithmetischeOperation.ADDITION,
             gueltig_seit=datetime(year=2021, month=1, day=13),
             gueltig_bis=datetime(year=2021, month=5, day=4),
         )
 
-        mlz_json = mlz.json(by_alias=True, ensure_ascii=False)
+        mlz_json = mlz.model_dump_json(by_alias=True)
 
         # CamelCase keys are made because they will put into JSON strings
         # to send them to the frontend (= JavaScript land)
         assert "messlokationsId" in mlz_json
         assert messlokations_id in mlz_json
         assert "arithmetik" in mlz_json
         assert "ADDITION" in mlz_json
         assert "gueltigSeit" in mlz_json
         assert "2021-01-13T00:00:00" in mlz_json
 
-        mlz_deserialized = Messlokationszuordnung.parse_raw(mlz_json)
+        mlz_deserialized = Messlokationszuordnung.model_validate_json(mlz_json)
 
         assert mlz_deserialized.messlokations_id == messlokations_id
         assert mlz_deserialized.arithmetik == ArithmetischeOperation.ADDITION
         assert mlz_deserialized.gueltig_seit == datetime(year=2021, month=1, day=13)
         assert mlz_deserialized.gueltig_bis == datetime(year=2021, month=5, day=4)
```

### Comparing `bo4e-0.4.8/tests/test_netznutzungsrechnung.py` & `bo4e-0.5.0/tests/test_netznutzungsrechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_positionsaufabschlag.py` & `bo4e-0.5.0/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preis.py` & `bo4e-0.5.0/tests/test_preis.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,35 +14,35 @@
 class TestPreis:
     def test_preis_only_required(self) -> None:
         """
         Test de-/serialisation of Preis (only has required attributes).
         """
         preis = example_preis
 
-        json_string = preis.json(by_alias=True, ensure_ascii=False)
+        json_string = preis.model_dump_json(by_alias=True)
 
         assert "KWH" in json_string
         assert "EUR" in json_string
         assert "null" in json_string
 
-        preis_deserialized = Preis.parse_raw(json_string)
+        preis_deserialized = Preis.model_validate_json(json_string)
 
         assert isinstance(preis_deserialized.wert, Decimal)
         assert isinstance(preis_deserialized.einheit, Waehrungseinheit)
         assert isinstance(preis_deserialized.bezugswert, Mengeneinheit)
         assert preis_deserialized.status is None
         assert preis == preis_deserialized
 
     def test_wrong_datatype(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Preis(wert="lululululu", einheit=Waehrungseinheit.EUR, bezugswert=Mengeneinheit.KWH)  # type: ignore[arg-type]
 
         assert "1 validation error" in str(excinfo.value)
         assert "wert" in str(excinfo.value)
-        assert "value is not a valid decimal" in str(excinfo.value)
+        assert "type=decimal_parsing" in str(excinfo.value)
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Preis(wert=Decimal(3.50), einheit=Waehrungseinheit.EUR, status=Preisstatus.ENDGUELTIG)  # type: ignore[call-arg]
 
         assert "1 validation error" in str(excinfo.value)
 
@@ -50,14 +50,14 @@
         preis = Preis(
             wert=Decimal(3.50),
             einheit=Waehrungseinheit.EUR,
             bezugswert=Mengeneinheit.KWH,
             status=Preisstatus.ENDGUELTIG,
         )
 
-        json_string = preis.json(by_alias=True, ensure_ascii=False)
+        json_string = preis.model_dump_json(by_alias=True)
 
         assert "ENDGUELTIG" in json_string
 
-        preis_deserialized = Preis.parse_raw(json_string)
+        preis_deserialized = Preis.model_validate_json(json_string)
 
         assert isinstance(preis_deserialized.status, Preisstatus)
```

### Comparing `bo4e-0.4.8/tests/test_preisblatt.py` & `bo4e-0.5.0/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisblatt_dienstleistung.py` & `bo4e-0.5.0/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisblatt_hardware.py` & `bo4e-0.5.0/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-0.5.0/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisblatt_messung.py` & `bo4e-0.5.0/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisblattnetznutzung.py` & `bo4e-0.5.0/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisgarantie.py` & `bo4e-0.5.0/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisposition.py` & `bo4e-0.5.0/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_preisstaffel.py` & `bo4e-0.5.0/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_rechnung.py` & `bo4e-0.5.0/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_rechnungsposition.py` & `bo4e-0.5.0/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_region.py` & `bo4e-0.5.0/tests/test_region.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,8 @@
             _ = Region(
                 bezeichnung="Bikini Bottom",
                 positiv_liste=[],
                 negativ_liste=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_regionalegueltigkeit.py` & `bo4e-0.5.0/tests/test_regionalegueltigkeit.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,8 +55,8 @@
         with pytest.raises(ValidationError) as excinfo:
             _ = RegionaleGueltigkeit(
                 gueltigkeitstyp=Gueltigkeitstyp.NUR_IN,
                 kriteriums_werte=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_regionalepreisgarantie.py` & `bo4e-0.5.0/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_regionalepreisstaffel.py` & `bo4e-0.5.0/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_regionaleraufabschlag.py` & `bo4e-0.5.0/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_regionaletarifpreisposition.py` & `bo4e-0.5.0/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_regionaltarif.py` & `bo4e-0.5.0/tests/test_regionaltarif.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,8 +95,8 @@
                 tarifart=Tarifart.MEHRTARIF,
                 tariftyp=Tariftyp.GRUND_ERSATZVERSORGUNG,
                 tarifmerkmale=[Tarifmerkmal.HEIZSTROM],
                 anbieter=example_marktteilnehmer,
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_regionskriterium.py` & `bo4e-0.5.0/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_sigmoidparameter.py` & `bo4e-0.5.0/tests/test_sigmoidparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_standorteigenschaften.py` & `bo4e-0.5.0/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_standorteigenschaftengas.py` & `bo4e-0.5.0/tests/test_standorteigenschaftengas.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,19 +38,19 @@
         assert "2 validation errors" in str(excinfo.value)
 
     @pytest.mark.parametrize(
         "wrong_netzkontonummern, expected_error_message",
         [
             pytest.param(
                 [],
-                "ensure this value has at least 1 item",
+                "too_short",
             ),
             pytest.param(
                 ["1", "2", "3"],
-                "ensure this value has at most 2 items",
+                "should have at most 2 items",
             ),
         ],
     )
     def test_standorteigenschaftengas_list_lenght_validation(
         self, wrong_netzkontonummern: List[str], expected_error_message: str
     ) -> None:
         with pytest.raises(ValidationError) as excinfo:
```

### Comparing `bo4e-0.4.8/tests/test_standorteigenschaftenstrom.py` & `bo4e-0.5.0/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_steuerbetrag.py` & `bo4e-0.5.0/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tagesvektor.py` & `bo4e-0.5.0/tests/test_tagesvektor.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,10 +53,10 @@
         assert "2 validation errors" in str(excinfo.value)
 
     def test_list_not_long_enough_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Tagesvektor(tag=datetime(2021, 12, 15, 5, 0, tzinfo=timezone.utc), werte=[])
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
 
     # add tests for issues 261 and 262 here
```

### Comparing `bo4e-0.4.8/tests/test_tarif.py` & `bo4e-0.5.0/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifberechnungsparameter.py` & `bo4e-0.5.0/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifeinschraenkung.py` & `bo4e-0.5.0/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifinfo.py` & `bo4e-0.5.0/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifkosten.py` & `bo4e-0.5.0/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifpreis.py` & `bo4e-0.5.0/tests/test_tarifpreis.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 class TestTarifpreis:
     def test_tarifpreis_only_required(self) -> None:
         """
         Test de-/serialisation of Tarifpreis (only has required attributes).
         """
         tarifpreis = example_tarifpreis
 
-        json_string = tarifpreis.json(by_alias=True, ensure_ascii=False)
+        json_string = tarifpreis.model_dump_json(by_alias=True)
 
         assert "ARBEITSPREIS_HT" in json_string
         assert "null" in json_string
 
-        tarifpreis_deserialized = Tarifpreis.parse_raw(json_string)
+        tarifpreis_deserialized = Tarifpreis.model_validate_json(json_string)
 
         assert isinstance(tarifpreis_deserialized.wert, Decimal)
         assert isinstance(tarifpreis_deserialized.einheit, Waehrungseinheit)
         assert isinstance(tarifpreis_deserialized.bezugswert, Mengeneinheit)
         assert isinstance(tarifpreis_deserialized.preistyp, Preistyp)
         assert tarifpreis_deserialized.beschreibung is None
         assert tarifpreis == tarifpreis_deserialized
@@ -45,15 +45,15 @@
                 einheit=Waehrungseinheit.EUR,
                 bezugswert=Mengeneinheit.KWH,
                 preistyp=Preistyp.ARBEITSPREIS_HT,
             )
 
         assert "1 validation error" in str(excinfo.value)
         assert "wert" in str(excinfo.value)
-        assert "value is not a valid decimal" in str(excinfo.value)
+        assert "should be a valid decimal" in str(excinfo.value)
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Tarifpreis(  # type: ignore[call-arg]
                 wert=Decimal(3.50),
                 einheit=Waehrungseinheit.EUR,
                 status=Preisstatus.ENDGUELTIG,
@@ -68,16 +68,16 @@
             einheit=Waehrungseinheit.EUR,
             bezugswert=Mengeneinheit.KWH,
             status=Preisstatus.ENDGUELTIG,
             preistyp=Preistyp.ARBEITSPREIS_HT,
             beschreibung="Das ist ein HT Arbeitspreis",
         )
 
-        json_string = tarifpreis.json(by_alias=True, ensure_ascii=False)
+        json_string = tarifpreis.model_dump_json(by_alias=True)
 
         assert "Das ist ein HT Arbeitspreis" in json_string
 
-        tarifpreis_deserialized = Tarifpreis.parse_raw(json_string)
+        tarifpreis_deserialized = Tarifpreis.model_validate_json(json_string)
 
         assert isinstance(tarifpreis_deserialized.beschreibung, str)
         assert tarifpreis_deserialized.beschreibung == "Das ist ein HT Arbeitspreis"
         assert tarifpreis_deserialized == tarifpreis
```

### Comparing `bo4e-0.4.8/tests/test_tarifpreisblatt.py` & `bo4e-0.5.0/tests/test_tarifpreisblatt.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,16 @@
 from bo4e.enum.sparte import Sparte
 from bo4e.enum.tarifart import Tarifart
 from bo4e.enum.tarifmerkmal import Tarifmerkmal
 from bo4e.enum.tariftyp import Tariftyp
 from tests.serialization_helper import assert_serialization_roundtrip
 from tests.test_aufabschlag import example_aufabschlag
 from tests.test_energiemix import example_energiemix
-from tests.test_geraeteeigenschaften import example_geraeteeigenschaften
 from tests.test_marktteilnehmer import example_marktteilnehmer
 from tests.test_preisgarantie import example_preisgarantie
-from tests.test_preisposition import example_preisposition
 from tests.test_tarifpreisposition import example_tarifpreisposition
 from tests.test_vertragskonditionen import example_vertragskonditionen
 from tests.test_zeitraum import example_zeitraum
 
 
 class TestTarifpreisblatt:
     @pytest.mark.parametrize(
```

### Comparing `bo4e-0.4.8/tests/test_tarifpreisposition.py` & `bo4e-0.5.0/tests/test_tarifpreisposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,8 +99,8 @@
                 preistyp=Preistyp.ENTGELT_ABLESUNG,
                 einheit=Waehrungseinheit.EUR,
                 bezugseinheit=Mengeneinheit.KWH,
                 preisstaffeln=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_tarifpreispositionproort.py` & `bo4e-0.5.0/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_tarifpreisstaffelproort.py` & `bo4e-0.5.0/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_unterschrift.py` & `bo4e-0.5.0/tests/test_unterschrift.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,36 +9,36 @@
 class TestUnterschrift:
     def test_unterschrift_only_required_attributes(self) -> None:
         """
         Test de-/serialisation of Unterschrift with minimal attributes.
         """
         unterschrift = Unterschrift(name="Foo")
 
-        json_string = unterschrift.json(by_alias=True, ensure_ascii=False)
+        json_string = unterschrift.model_dump_json(by_alias=True)
 
         assert "Foo" in json_string
 
-        unterschrift_deserialized = Unterschrift.parse_raw(json_string)
+        unterschrift_deserialized = Unterschrift.model_validate_json(json_string)
 
         assert isinstance(unterschrift_deserialized.name, str)
         assert unterschrift_deserialized.name == "Foo"
 
     def test_unterschrift_required_and_optional_attributes(self) -> None:
         """
         Test de-/serialisation of Unterschrift with maximal attributes.
         """
         unterschrift = Unterschrift(name="Foo", ort="Grünwald", datum=datetime(2019, 6, 7, tzinfo=timezone.utc))
 
-        json_string = unterschrift.json(by_alias=True, ensure_ascii=False)
+        json_string = unterschrift.model_dump_json(by_alias=True)
 
         assert "Foo" in json_string
         assert "Grünwald" in json_string
-        assert "2019-06-07T00:00:00+00:00" in json_string
+        assert "2019-06-07T00:00:00Z" in json_string
 
-        unterschrift_deserialized = Unterschrift.parse_raw(json_string)
+        unterschrift_deserialized = Unterschrift.model_validate_json(json_string)
 
         assert isinstance(unterschrift_deserialized.name, str)
         assert unterschrift_deserialized.name == "Foo"
         assert isinstance(unterschrift_deserialized.ort, str)
         assert unterschrift_deserialized.ort == "Grünwald"
         assert isinstance(unterschrift_deserialized.datum, datetime)
         assert unterschrift_deserialized.datum == datetime(2019, 6, 7, tzinfo=timezone.utc)
```

### Comparing `bo4e-0.4.8/tests/test_verbrauch.py` & `bo4e-0.5.0/tests/test_verbrauch.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
                 startdatum=datetime(2021, 12, 1, 0, 0, 0).replace(tzinfo=timezone.utc),
                 enddatum=datetime(2021, 12, 2, 0, 0, 0).replace(tzinfo=timezone.utc),
                 einheit=Mengeneinheit.KWH,
                 wertermittlungsverfahren=Wertermittlungsverfahren.MESSUNG,
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "obisKennzahl" in str(excinfo.value)
-        assert "string does not match regex" in str(excinfo.value)
+        assert "obis_kennzahl" in str(excinfo.value)
+        assert "should match pattern" in str(excinfo.value)
 
     def test_failing_validation_end_later_than_start(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Verbrauch(
                 obis_kennzahl="1-0:1.8.1",
                 wert=Decimal(40),
                 startdatum=datetime(2021, 12, 2, 0, 0, 0).replace(tzinfo=timezone.utc),
```

### Comparing `bo4e-0.4.8/tests/test_vertrag.py` & `bo4e-0.5.0/tests/test_vertrag.py`

 * *Files 4% similar despite different names*

```diff
@@ -168,28 +168,28 @@
 
     def test_serialisation_only_required_attributes(self) -> None:
         """
         Test de-/serialisation of Vertrag with minimal attributes.
         """
         vertrag = self.get_example_vertrag()
 
-        json_string = vertrag.json(by_alias=True, ensure_ascii=False)
+        json_string = vertrag.model_dump_json(by_alias=True)
 
         assert vertrag.bo_typ is BoTyp.VERTRAG, "boTyp was not automatically set"
         assert self._vertragsnummer in json_string
         assert "BILANZIERUNGSVERTRAG" in json_string
         assert "AKTIV" in json_string
         assert "STROM" in json_string
-        assert "2021-04-30T13:45:00+00:00" in json_string
-        assert "2021-06-05T16:30:00+00:00" in json_string
+        assert "2021-04-30T13:45:00Z" in json_string
+        assert "2021-06-05T16:30:00Z" in json_string
         assert "von Sinnen" in json_string
         assert "Preetz" in json_string
-        assert "2021-06-05T00:00:00+00:00" in json_string
+        assert "2021-06-05T00:00:00Z" in json_string
 
-        vertrag_deserialized = Vertrag.parse_raw(json_string)
+        vertrag_deserialized = Vertrag.model_validate_json(json_string)
 
         assert vertrag_deserialized.vertragsnummer == self._vertragsnummer
         assert vertrag_deserialized.vertragsart == self._vertragsart
         assert vertrag_deserialized.vertragsstatus == self._vertragsstatus
         assert vertrag_deserialized.sparte == self._sparte
         assert vertrag_deserialized.vertragsbeginn == self._vertragsbeginn
         assert vertrag_deserialized.vertragsende == self._vertragsende
@@ -223,34 +223,34 @@
             ],
             beschreibung="Hello Vertrag",
             vertragskonditionen=Vertragskonditionen(beschreibung="Beschreibung"),
             unterzeichnervp1=[Unterschrift(name="Foo")],
             unterzeichnervp2=[Unterschrift(name="Bar"), Unterschrift(name="Dr.No")],
         )
 
-        json_string = vertrag.json(by_alias=True, ensure_ascii=False)
+        json_string = vertrag.model_dump_json(by_alias=True)
 
         assert vertrag.bo_typ is BoTyp.VERTRAG, "boTyp was not automatically set"
         assert self._vertragsnummer in json_string
         assert "BILANZIERUNGSVERTRAG" in json_string
         assert "AKTIV" in json_string
         assert "STROM" in json_string
-        assert "2021-04-30T13:45:00+00:00" in json_string
-        assert "2021-06-05T16:30:00+00:00" in json_string
+        assert "2021-04-30T13:45:00Z" in json_string
+        assert "2021-06-05T16:30:00Z" in json_string
         assert "von Sinnen" in json_string
         assert "Preetz" in json_string
-        assert "2021-06-05T00:00:00+00:00" in json_string
-        assert "2002-12-03T00:00:00+00:00" in json_string
+        assert "2021-06-05T00:00:00Z" in json_string
+        assert "2002-12-03T00:00:00Z" in json_string
         assert "Hello Vertrag" in json_string
         assert "Beschreibung" in json_string
         assert "Foo" in json_string
         assert "Bar" in json_string
         assert "Dr.No" in json_string
 
-        vertrag_deserialized = Vertrag.parse_raw(json_string)
+        vertrag_deserialized = Vertrag.model_validate_json(json_string)
 
         assert vertrag_deserialized.vertragsnummer == self._vertragsnummer
         assert vertrag_deserialized.vertragsart == self._vertragsart
         assert vertrag_deserialized.vertragsstatus == self._vertragsstatus
         assert vertrag_deserialized.sparte == self._sparte
         assert vertrag_deserialized.vertragsbeginn == self._vertragsbeginn
         assert vertrag_deserialized.vertragsende == self._vertragsende
@@ -291,8 +291,8 @@
                 vertragsende=self._vertragsende,
                 vertragspartner1=self._vertragspartner1,
                 vertragspartner2=self._vertragspartner2,
                 vertragsteile=[],
             )
 
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_vertragskonditionen.py` & `bo4e-0.5.0/tests/test_vertragskonditionen.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,24 +21,24 @@
 class TestVertragskonditionen:
     def test_vertragskonditionen_with_optional_attributes(self) -> None:
         """
         Test de-/serialisation of Vertragskonditionen (only has optional attributes).
         """
         vertragskonditionen = example_vertragskonditionen
 
-        json_string = vertragskonditionen.json(by_alias=True, ensure_ascii=False)
+        json_string = vertragskonditionen.model_dump_json(by_alias=True)
 
         assert "Foobar" in json_string
         assert "3" in json_string
-        assert "2013-10-11T00:00:00+00:00" in json_string
+        assert "2013-10-11T00:00:00Z" in json_string
         assert "WOCHE" in json_string
         assert "TAG" in json_string
         assert "14" in json_string
 
-        vertragskonditionen_deserialized = Vertragskonditionen.parse_raw(json_string)
+        vertragskonditionen_deserialized = Vertragskonditionen.model_validate_json(json_string)
 
         assert isinstance(vertragskonditionen_deserialized.beschreibung, str)
         assert vertragskonditionen_deserialized.beschreibung == "Foobar"
         assert isinstance(vertragskonditionen_deserialized.anzahl_abschlaege, Decimal)
         assert vertragskonditionen_deserialized.anzahl_abschlaege == Decimal(3)
         assert isinstance(vertragskonditionen_deserialized.vertragslaufzeit, Zeitraum)
         assert vertragskonditionen_deserialized.vertragslaufzeit == Zeitraum(
```

### Comparing `bo4e-0.4.8/tests/test_vertragsteil.py` & `bo4e-0.5.0/tests/test_vertragsteil.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,20 @@
         Test de-/serialisation of Vertragsteil with minimal attributes.
         """
         vertragsteil = Vertragsteil(
             vertragsteilbeginn=datetime(2001, 3, 15, tzinfo=timezone.utc),
             vertragsteilende=datetime(2007, 11, 27, tzinfo=timezone.utc),
         )
 
-        json_string = vertragsteil.json(by_alias=True, ensure_ascii=False)
+        json_string = vertragsteil.model_dump_json(by_alias=True)
 
-        assert "2001-03-15T00:00:00+00:00" in json_string
-        assert "2007-11-27T00:00:00+00:00" in json_string
+        assert "2001-03-15T00:00:00Z" in json_string
+        assert "2007-11-27T00:00:00Z" in json_string
 
-        vertragsteil_deserialized = Vertragsteil.parse_raw(json_string)
+        vertragsteil_deserialized = Vertragsteil.model_validate_json(json_string)
 
         assert isinstance(vertragsteil_deserialized.vertragsteilbeginn, datetime)
         assert vertragsteil_deserialized.vertragsteilbeginn == datetime(2001, 3, 15, tzinfo=timezone.utc)
         assert isinstance(vertragsteil_deserialized.vertragsteilende, datetime)
         assert vertragsteil_deserialized.vertragsteilende == datetime(2007, 11, 27, tzinfo=timezone.utc)
 
     def test_vertragsteil_required_and_optional_attributes(self) -> None:
@@ -40,23 +40,23 @@
             vertragsteilende=datetime(2007, 11, 27, tzinfo=timezone.utc),
             lokation="Bar",
             vertraglich_fixierte_menge=Menge(wert=Decimal(3.1), einheit=Mengeneinheit.KWH),
             minimale_abnahmemenge=Menge(wert=Decimal(2000), einheit=Mengeneinheit.KWH),
             maximale_abnahmemenge=Menge(wert=Decimal(0.111111), einheit=Mengeneinheit.KWH),
         )
 
-        json_string = vertragsteil.json(by_alias=True, ensure_ascii=False)
+        json_string = vertragsteil.model_dump_json(by_alias=True)
 
-        assert "2001-03-15T00:00:00+00:00" in json_string
-        assert "2007-11-27T00:00:00+00:00" in json_string
+        assert "2001-03-15T00:00:00Z" in json_string
+        assert "2007-11-27T00:00:00Z" in json_string
         assert "Bar" in json_string
         assert "KWH" in json_string
         assert "0.111111" in json_string
 
-        vertragsteil_deserialized = Vertragsteil.parse_raw(json_string)
+        vertragsteil_deserialized = Vertragsteil.model_validate_json(json_string)
 
         assert isinstance(vertragsteil_deserialized.vertragsteilbeginn, datetime)
         assert vertragsteil_deserialized.vertragsteilbeginn == datetime(2001, 3, 15, tzinfo=timezone.utc)
         assert isinstance(vertragsteil_deserialized.vertragsteilende, datetime)
         assert vertragsteil_deserialized.vertragsteilende == datetime(2007, 11, 27, tzinfo=timezone.utc)
         assert isinstance(vertragsteil_deserialized.lokation, str)
         assert vertragsteil_deserialized.lokation == "Bar"
```

### Comparing `bo4e-0.4.8/tests/test_zaehler.py` & `bo4e-0.5.0/tests/test_zaehler.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,18 +42,18 @@
             externe_referenzen=[ExterneReferenz(ex_ref_name="zaehler im anderen system", ex_ref_wert="7890")],
             letzte_eichung=datetime(2019, 6, 30, 0, 0, 0),
         )
         assert zaehler.versionstruktur == "2", "versionstruktur was not automatically set"
         assert zaehler.bo_typ is BoTyp.ZAEHLER, "boTyp was not automatically set"
         assert zaehler.zaehlwerke[0].richtung == Energierichtung.EINSP
         assert zaehler.zaehlwerke[0].einheit == Mengeneinheit.KW
-        json_string = zaehler.json(by_alias=True, ensure_ascii=False)
+        json_string = zaehler.model_dump_json(by_alias=True)
         assert "richtung" in json_string, "Zaehlwerk->richtung was not serialized"
         assert "einheit" in json_string, "Zaehlwerk->einheit was not serialized"
-        deserialized_zaehler = Zaehler.parse_raw(json_string)
+        deserialized_zaehler = Zaehler.model_validate_json(json_string)
         assert deserialized_zaehler == zaehler
 
     def test_serialization_fails_for_invalid_obis(self) -> None:
         """
         Test serialisation of Zaehler fails if OBIS is wrong.
         """
         with pytest.raises(ValidationError) as excinfo:
@@ -71,16 +71,16 @@
                         wandlerfaktor=Decimal(0.95),
                     )
                 ],
                 zaehlertyp=Zaehlertyp.DREHSTROMZAEHLER,
                 tarifart=Tarifart.ZWEITARIF,
             )
         assert "1 validation error" in str(excinfo.value)
-        assert "obisKennzahl" in str(excinfo.value)
-        assert "string does not match regex" in str(excinfo.value)
+        assert "obis_kennzahl" in str(excinfo.value)
+        assert "should match pattern" in str(excinfo.value)
 
     def test_serialization_fails_for_empty_zaehlwerke(self) -> None:
         """
         Test serialisation of Zaehler fails if there are no zaehlwerke.
         """
         with pytest.raises(ValidationError) as excinfo:
             _ = Zaehler(
@@ -88,8 +88,8 @@
                 sparte=Sparte.STROM,
                 zaehlerauspraegung=Zaehlerauspraegung.EINRICHTUNGSZAEHLER,
                 zaehlwerke=[],
                 zaehlertyp=Zaehlertyp.DREHSTROMZAEHLER,
                 tarifart=Tarifart.ZWEITARIF,
             )
         assert "1 validation error" in str(excinfo.value)
-        assert "ensure this value has at least 1 item" in str(excinfo.value)
+        assert "too_short" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_zeitintervall.py` & `bo4e-0.5.0/tests/test_zeitintervall.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 class TestZeitintervall:
     def test_zeitintervall_daten(self) -> None:
         """
         Test de-/serialisation of Zeitintervall (only has optional attributes) with option startdatum and enddatum.
         """
         zeitintervall = Zeitintervall(wert=2, zeiteinheit=Zeiteinheit.VIERTEL_STUNDE)
 
-        json_string = zeitintervall.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitintervall.model_dump_json(by_alias=True)
 
         assert "2" in json_string
         assert "VIERTEL_STUNDE" in json_string
 
-        zeitintervall_deserialized = Zeitintervall.parse_raw(json_string)
+        zeitintervall_deserialized = Zeitintervall.model_validate_json(json_string)
 
         assert isinstance(zeitintervall_deserialized.wert, int)
         assert zeitintervall_deserialized.wert == 2
         assert isinstance(zeitintervall_deserialized.zeiteinheit, Zeiteinheit)
         assert zeitintervall_deserialized.zeiteinheit == Zeiteinheit.VIERTEL_STUNDE
 
     def test_wrong_datatype(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Zeitintervall(wert="errrrrror", zeiteinheit=Zeiteinheit.TAG)  # type: ignore[arg-type]
 
         assert "1 validation error" in str(excinfo.value)
         assert "wert" in str(excinfo.value)
-        assert "value is not a valid integer" in str(excinfo.value)
+        assert "should be a valid integer" in str(excinfo.value)
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Zeitintervall(wert=3)  # type: ignore[call-arg]
 
         assert "1 validation error" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_zeitraum.py` & `bo4e-0.5.0/tests/test_zeitraum.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,40 +25,40 @@
 class TestZeitraum:
     def test_zeitraum_dauer(self) -> None:
         """
         Test de-/serialisation of Zeitraum (only has optional attributes) with option dauer and einheit.
         """
         zeitraum = Zeitraum(einheit=Zeiteinheit.TAG, dauer=Decimal(21))
 
-        json_string = zeitraum.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitraum.model_dump_json(by_alias=True)
 
         assert "21" in json_string
         assert "TAG" in json_string
 
-        zeitraum_deserialized = Zeitraum.parse_raw(json_string)
+        zeitraum_deserialized = Zeitraum.model_validate_json(json_string)
 
         assert isinstance(zeitraum_deserialized.einheit, Zeiteinheit)
         assert zeitraum_deserialized.einheit == Zeiteinheit.TAG
         assert isinstance(zeitraum_deserialized.dauer, Decimal)
         assert zeitraum_deserialized.dauer == Decimal(21)
 
     def test_zeitraum_daten(self) -> None:
         """
         Test de-/serialisation of Zeitraum (only has optional attributes) with option startdatum and enddatum.
         """
         zeitraum = Zeitraum(
             startdatum=datetime(2013, 5, 1, tzinfo=timezone.utc), enddatum=datetime(2022, 1, 28, tzinfo=timezone.utc)
         )
 
-        json_string = zeitraum.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitraum.model_dump_json(by_alias=True)
 
-        assert "2013-05-01T00:00:00+00:00" in json_string
-        assert "2022-01-28T00:00:00+00:00" in json_string
+        assert "2013-05-01T00:00:00Z" in json_string
+        assert "2022-01-28T00:00:00Z" in json_string
 
-        zeitraum_deserialized = Zeitraum.parse_raw(json_string)
+        zeitraum_deserialized = Zeitraum.model_validate_json(json_string)
 
         assert isinstance(zeitraum_deserialized.startdatum, datetime)
         assert zeitraum_deserialized.startdatum == datetime(2013, 5, 1, tzinfo=timezone.utc)
         assert isinstance(zeitraum_deserialized.enddatum, datetime)
         assert zeitraum_deserialized.enddatum == datetime(2022, 1, 28, tzinfo=timezone.utc)
 
     def test_zeitraum_zeitpunkte(self) -> None:
@@ -66,20 +66,20 @@
         Test de-/serialisation of Zeitraum (only has optional attributes) with option startzeitpunkt and endzeitpunkt.
         """
         zeitraum = Zeitraum(
             startzeitpunkt=datetime(2011, 2, 5, 16, 43, tzinfo=timezone.utc),
             endzeitpunkt=datetime(2021, 7, 30, tzinfo=timezone.utc),
         )
 
-        json_string = zeitraum.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitraum.model_dump_json(by_alias=True)
 
-        assert "2011-02-05T16:43:00+00:00" in json_string
-        assert "2021-07-30T00:00:00+00:00" in json_string
+        assert "2011-02-05T16:43:00Z" in json_string
+        assert "2021-07-30T00:00:00Z" in json_string
 
-        zeitraum_deserialized = Zeitraum.parse_raw(json_string)
+        zeitraum_deserialized = Zeitraum.model_validate_json(json_string)
 
         assert isinstance(zeitraum_deserialized.startzeitpunkt, datetime)
         assert zeitraum_deserialized.startzeitpunkt == datetime(2011, 2, 5, 16, 43, tzinfo=timezone.utc)
         assert isinstance(zeitraum_deserialized.endzeitpunkt, datetime)
         assert zeitraum_deserialized.endzeitpunkt == datetime(2021, 7, 30, tzinfo=timezone.utc)
 
     @pytest.mark.parametrize(
```

### Comparing `bo4e-0.4.8/tests/test_zeitreihe.py` & `bo4e-0.5.0/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-0.4.8/tests/test_zeitreihenwert.py` & `bo4e-0.5.0/tests/test_zeitreihenwert.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,43 +18,43 @@
 class TestZeitreihenwert:
     def test_zeitreihenwert_only_required_attributes(self) -> None:
         """
         Test de-/serialisation of Zeitreihenwert with minimal attributes.
         """
         zeitreihenwert = example_zeitreihenwert
 
-        json_string = zeitreihenwert.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitreihenwert.model_dump_json(by_alias=True)
 
-        assert "2001-03-15T00:00:00+00:00" in json_string
-        assert "2007-11-27T00:00:00+00:00" in json_string
+        assert "2001-03-15T00:00:00Z" in json_string
+        assert "2007-11-27T00:00:00Z" in json_string
 
-        zeitreihenwert_deserialized: Zeitreihenwert = Zeitreihenwert.parse_raw(json_string)
+        zeitreihenwert_deserialized: Zeitreihenwert = Zeitreihenwert.model_validate_json(json_string)
         assert zeitreihenwert_deserialized == zeitreihenwert
 
     def test_zeitreihenwert_required_and_optional_attributes(self) -> None:
         """
         Test de-/serialisation of Zeitreihenwert with maximal attributes.
         """
         zeitreihenwert = Zeitreihenwert(
             datum_uhrzeit_von=datetime(2001, 3, 15, tzinfo=timezone.utc),
             datum_uhrzeit_bis=datetime(2007, 11, 27, tzinfo=timezone.utc),
             wert=Decimal(2.5),
             status=Messwertstatus.ABGELESEN,
             statuszusatz=Messwertstatuszusatz.Z78_GERAETEWECHSEL,
         )
 
-        json_string = zeitreihenwert.json(by_alias=True, ensure_ascii=False)
+        json_string = zeitreihenwert.model_dump_json(by_alias=True)
 
         assert "2.5" in json_string
-        assert "2001-03-15T00:00:00+00:00" in json_string
-        assert "2007-11-27T00:00:00+00:00" in json_string
+        assert "2001-03-15T00:00:00Z" in json_string
+        assert "2007-11-27T00:00:00Z" in json_string
         assert "ABGELESEN" in json_string
         assert "Z78_GERAETEWECHSEL" in json_string
 
-        zeitreihenwert_deserialized: Zeitreihenwert = Zeitreihenwert.parse_raw(json_string)
+        zeitreihenwert_deserialized: Zeitreihenwert = Zeitreihenwert.model_validate_json(json_string)
         assert zeitreihenwert_deserialized == zeitreihenwert
 
     def test_missing_required_attribute(self) -> None:
         with pytest.raises(ValidationError) as excinfo:
             _ = Zeitreihenwert(datum_uhrzeit_von=datetime(2007, 11, 27, tzinfo=timezone.utc), wert=Decimal(1.5))  # type: ignore[call-arg]
 
         assert "1 validation error" in str(excinfo.value)
```

### Comparing `bo4e-0.4.8/tests/test_zeitreihenwertkompakt.py` & `bo4e-0.5.0/tests/test_zeitreihenwertkompakt.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 
 class TestZeitreihenwertkompakt:
     def test_serialization(self) -> None:
         zrwk = Zeitreihenwertkompakt(
             wert=Decimal(1.5), status=Messwertstatus.ABGELESEN, statuszusatz=Messwertstatuszusatz.Z78_GERAETEWECHSEL
         )
 
-        json_string = zrwk.json(by_alias=True, ensure_ascii=False)
+        json_string = zrwk.model_dump_json(by_alias=True)
 
         assert "1.5" in json_string
         assert "ABGELESEN" in json_string
         assert "Z78_GERAETEWECHSEL" in json_string
-        deserialized_zrwk: Zeitreihenwertkompakt = Zeitreihenwertkompakt.parse_raw(json_string)
+        deserialized_zrwk: Zeitreihenwertkompakt = Zeitreihenwertkompakt.model_validate_json(json_string)
 
         assert isinstance(deserialized_zrwk.wert, Decimal)
         assert deserialized_zrwk.wert == Decimal(1.5)
         assert isinstance(deserialized_zrwk.status, Messwertstatus)
         assert deserialized_zrwk.status == Messwertstatus.ABGELESEN
         assert isinstance(deserialized_zrwk.statuszusatz, Messwertstatuszusatz)
         assert deserialized_zrwk.statuszusatz == Messwertstatuszusatz.Z78_GERAETEWECHSEL
@@ -42,14 +42,14 @@
         assert "1 validation error" in str(excinfo.value)
 
     def test_only_required(self) -> None:
         zrwk = Zeitreihenwertkompakt(
             wert=Decimal(1.5),
         )
 
-        json_string = zrwk.json(by_alias=True, ensure_ascii=False)
+        json_string = zrwk.model_dump_json(by_alias=True)
 
         assert "1.5" in json_string
 
-        deserialized_zrwk: Zeitreihenwertkompakt = Zeitreihenwertkompakt.parse_raw(json_string)
+        deserialized_zrwk: Zeitreihenwertkompakt = Zeitreihenwertkompakt.model_validate_json(json_string)
 
         assert deserialized_zrwk == zrwk
```

### Comparing `bo4e-0.4.8/tox.ini` & `bo4e-0.5.0/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pylint json_schemas/generate_json_schemas.py
 
 [testenv:type_check]
 usedevelop = True
 # the type_check environment checks the type hints using mypy
 deps =
     -rrequirements.txt
-    mypy==1.3.0
+    mypy
     pytest
 commands =
     mypy --show-error-codes src/bo4e
     mypy --show-error-codes tests
     mypy --show-error-codes docs/uml.py
     mypy --show-error-codes json_schemas/generate_json_schemas.py
     # add single files (ending with .py) or packages here
```

