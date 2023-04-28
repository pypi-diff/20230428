# Comparing `tmp/teritorio-2023.2.1.tar.gz` & `tmp/teritorio-2023.4.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teritorio-2023.2.1.tar", max compression
+gzip compressed data, was "teritorio-2023.4.28.tar", max compression
```

## Comparing `teritorio-2023.2.1.tar` & `teritorio-2023.4.28.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.2.1/LICENSE.txt
--rw-r--r--   0        0        0     2188 2023-01-28 23:28:39.058992 teritorio-2023.2.1/README.rst
--rw-r--r--   0        0        0     2199 2023-02-01 22:09:59.173629 teritorio-2023.2.1/pyproject.toml
--rw-r--r--   0        0        0      115 2023-01-28 23:28:39.059785 teritorio-2023.2.1/src/teritorio/__init__.py
--rw-r--r--   0        0        0    46659 2023-01-28 23:28:39.060035 teritorio-2023.2.1/src/teritorio/_data/country.json
--rw-r--r--   0        0        0    36064 2023-02-01 19:33:08.179310 teritorio-2023.2.1/src/teritorio/_data/currency.json
--rw-r--r--   0        0        0     2001 2023-01-28 23:28:39.060341 teritorio-2023.2.1/src/teritorio/main.py
--rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.2.1/src/teritorio/py.typed
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 teritorio-2023.2.1/setup.py
--rw-r--r--   0        0        0     3146 1970-01-01 00:00:00.000000 teritorio-2023.2.1/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:39.058913 teritorio-2023.4.28/LICENSE.txt
+-rw-r--r--   0        0        0     2377 2023-03-12 00:03:02.409875 teritorio-2023.4.28/README.rst
+-rw-r--r--   0        0        0     2845 2023-04-28 14:54:20.747121 teritorio-2023.4.28/pyproject.toml
+-rw-r--r--   0        0        0      115 2023-01-28 23:28:39.059785 teritorio-2023.4.28/src/teritorio/__init__.py
+-rw-r--r--   0        0        0    48421 2023-04-28 14:44:19.353103 teritorio-2023.4.28/src/teritorio/_data/country.json
+-rw-r--r--   0        0        0    37324 2023-04-28 13:07:47.892608 teritorio-2023.4.28/src/teritorio/_data/currency.json
+-rw-r--r--   0        0        0     2219 2023-04-28 11:59:18.006870 teritorio-2023.4.28/src/teritorio/main.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:39.060375 teritorio-2023.4.28/src/teritorio/py.typed
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 teritorio-2023.4.28/PKG-INFO
```

### Comparing `teritorio-2023.2.1/LICENSE.txt` & `teritorio-2023.4.28/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `teritorio-2023.2.1/README.rst` & `teritorio-2023.4.28/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 =================================================
 teritorio: ISO codes for countries and currencies
 =================================================
 
-.. image:: https://github.com/spapanik/teritorio/actions/workflows/build.yml/badge.svg
-  :alt: Build
-  :target: https://github.com/spapanik/teritorio/actions/workflows/build.yml
-.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/teritorio.svg
-  :alt: Total alerts
-  :target: https://lgtm.com/projects/g/spapanik/teritorio/alerts/
+.. image:: https://github.com/spapanik/teritorio/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/teritorio/actions/workflows/tests.yml
 .. image:: https://img.shields.io/github/license/spapanik/teritorio
   :alt: License
   :target: https://github.com/spapanik/teritorio/blob/main/LICENSE.txt
 .. image:: https://img.shields.io/pypi/v/teritorio
   :alt: PyPI
   :target: https://pypi.org/project/teritorio
 .. image:: https://pepy.tech/badge/teritorio
   :alt: Downloads
   :target: https://pepy.tech/project/teritorio
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: Code style
+  :alt: code style: black
   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
 
 ``teritorio`` two iterable singletons that ``Countries`` and ``Currencies``, that contain all the
 relevant ISO information about countries and currencies, respectively.
 
 In a nutshell
 -------------
```

### Comparing `teritorio-2023.2.1/src/teritorio/_data/country.json` & `teritorio-2023.4.28/src/teritorio/_data/country.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('ABW', OrderedDict([('alpha_2_code', 'AW'), ('alpha_3_code', 'ABW'), "*

 * *            "('english_name', 'Aruba'), ('french_name', 'Aruba'), ('numeric_code', 533)])), "*

 * *            "('AFG', OrderedDict([('alpha_2_code', 'AF'), ('alpha_3_code', 'AFG'), "*

 * *            '(\'english_name\', \'Afghanistan\'), (\'french_name\', "Afghanistan (l\')"), '*

 * *            "('numeric_code', 4)])), ('AGO', OrderedDict([('alpha_2_code', 'AO'), ('alpha_3_code', "*

 * *            '\'AGO\'), (\'english_name\',  […]*

```diff
@@ -1,1745 +1,1745 @@
-[
-    {
+{
+    "ABW": {
         "alpha_2_code": "AW",
         "alpha_3_code": "ABW",
         "english_name": "Aruba",
         "french_name": "Aruba",
         "numeric_code": 533
     },
-    {
+    "AFG": {
         "alpha_2_code": "AF",
         "alpha_3_code": "AFG",
         "english_name": "Afghanistan",
         "french_name": "Afghanistan (l')",
         "numeric_code": 4
     },
-    {
+    "AGO": {
         "alpha_2_code": "AO",
         "alpha_3_code": "AGO",
         "english_name": "Angola",
         "french_name": "Angola (l')",
         "numeric_code": 24
     },
-    {
+    "AIA": {
         "alpha_2_code": "AI",
         "alpha_3_code": "AIA",
         "english_name": "Anguilla",
         "french_name": "Anguilla",
         "numeric_code": 660
     },
-    {
+    "ALA": {
         "alpha_2_code": "AX",
         "alpha_3_code": "ALA",
         "english_name": "\u00c5land Islands",
         "french_name": "\u00c5land(les \u00celes)",
         "numeric_code": 248
     },
-    {
+    "ALB": {
         "alpha_2_code": "AL",
         "alpha_3_code": "ALB",
         "english_name": "Albania",
         "french_name": "Albanie (l')",
         "numeric_code": 8
     },
-    {
+    "AND": {
         "alpha_2_code": "AD",
         "alpha_3_code": "AND",
         "english_name": "Andorra",
         "french_name": "Andorre (l')",
         "numeric_code": 20
     },
-    {
+    "ARE": {
         "alpha_2_code": "AE",
         "alpha_3_code": "ARE",
         "english_name": "United Arab Emirates (the)",
         "french_name": "\u00c9mirats arabes unis (les)",
         "numeric_code": 784
     },
-    {
+    "ARG": {
         "alpha_2_code": "AR",
         "alpha_3_code": "ARG",
         "english_name": "Argentina",
         "french_name": "Argentine (l')",
         "numeric_code": 32
     },
-    {
+    "ARM": {
         "alpha_2_code": "AM",
         "alpha_3_code": "ARM",
         "english_name": "Armenia",
         "french_name": "Arm\u00e9nie (l')",
         "numeric_code": 51
     },
-    {
+    "ASM": {
         "alpha_2_code": "AS",
         "alpha_3_code": "ASM",
         "english_name": "American Samoa",
         "french_name": "Samoa am\u00e9ricaines (les)",
         "numeric_code": 16
     },
-    {
+    "ATA": {
         "alpha_2_code": "AQ",
         "alpha_3_code": "ATA",
         "english_name": "Antarctica",
         "french_name": "Antarctique (l')",
         "numeric_code": 10
     },
-    {
+    "ATF": {
         "alpha_2_code": "TF",
         "alpha_3_code": "ATF",
         "english_name": "French Southern Territories (the)",
         "french_name": "Terres australes fran\u00e7aises (les)",
         "numeric_code": 260
     },
-    {
+    "ATG": {
         "alpha_2_code": "AG",
         "alpha_3_code": "ATG",
         "english_name": "Antigua and Barbuda",
         "french_name": "Antigua-et-Barbuda",
         "numeric_code": 28
     },
-    {
+    "AUS": {
         "alpha_2_code": "AU",
         "alpha_3_code": "AUS",
         "english_name": "Australia",
         "french_name": "Australie (l')",
         "numeric_code": 36
     },
-    {
+    "AUT": {
         "alpha_2_code": "AT",
         "alpha_3_code": "AUT",
         "english_name": "Austria",
         "french_name": "Autriche (l')",
         "numeric_code": 40
     },
-    {
+    "AZE": {
         "alpha_2_code": "AZ",
         "alpha_3_code": "AZE",
         "english_name": "Azerbaijan",
         "french_name": "Azerba\u00efdjan (l')",
         "numeric_code": 31
     },
-    {
+    "BDI": {
         "alpha_2_code": "BI",
         "alpha_3_code": "BDI",
         "english_name": "Burundi",
         "french_name": "Burundi (le)",
         "numeric_code": 108
     },
-    {
+    "BEL": {
         "alpha_2_code": "BE",
         "alpha_3_code": "BEL",
         "english_name": "Belgium",
         "french_name": "Belgique (la)",
         "numeric_code": 56
     },
-    {
+    "BEN": {
         "alpha_2_code": "BJ",
         "alpha_3_code": "BEN",
         "english_name": "Benin",
         "french_name": "B\u00e9nin (le)",
         "numeric_code": 204
     },
-    {
+    "BES": {
         "alpha_2_code": "BQ",
         "alpha_3_code": "BES",
         "english_name": "Bonaire, Sint Eustatius and Saba",
         "french_name": "Bonaire, Saint-Eustache et Saba",
         "numeric_code": 535
     },
-    {
+    "BFA": {
         "alpha_2_code": "BF",
         "alpha_3_code": "BFA",
         "english_name": "Burkina Faso",
         "french_name": "Burkina Faso (le)",
         "numeric_code": 854
     },
-    {
+    "BGD": {
         "alpha_2_code": "BD",
         "alpha_3_code": "BGD",
         "english_name": "Bangladesh",
         "french_name": "Bangladesh (le)",
         "numeric_code": 50
     },
-    {
+    "BGR": {
         "alpha_2_code": "BG",
         "alpha_3_code": "BGR",
         "english_name": "Bulgaria",
         "french_name": "Bulgarie (la)",
         "numeric_code": 100
     },
-    {
+    "BHR": {
         "alpha_2_code": "BH",
         "alpha_3_code": "BHR",
         "english_name": "Bahrain",
         "french_name": "Bahre\u00efn",
         "numeric_code": 48
     },
-    {
+    "BHS": {
         "alpha_2_code": "BS",
         "alpha_3_code": "BHS",
         "english_name": "Bahamas (the)",
         "french_name": "Bahamas (les)",
         "numeric_code": 44
     },
-    {
+    "BIH": {
         "alpha_2_code": "BA",
         "alpha_3_code": "BIH",
         "english_name": "Bosnia and Herzegovina",
         "french_name": "Bosnie-Herz\u00e9govine (la)",
         "numeric_code": 70
     },
-    {
+    "BLM": {
         "alpha_2_code": "BL",
         "alpha_3_code": "BLM",
         "english_name": "Saint Barth\u00e9lemy",
         "french_name": "Saint-Barth\u00e9lemy",
         "numeric_code": 652
     },
-    {
+    "BLR": {
         "alpha_2_code": "BY",
         "alpha_3_code": "BLR",
         "english_name": "Belarus",
         "french_name": "B\u00e9larus (le)",
         "numeric_code": 112
     },
-    {
+    "BLZ": {
         "alpha_2_code": "BZ",
         "alpha_3_code": "BLZ",
         "english_name": "Belize",
         "french_name": "Belize (le)",
         "numeric_code": 84
     },
-    {
+    "BMU": {
         "alpha_2_code": "BM",
         "alpha_3_code": "BMU",
         "english_name": "Bermuda",
         "french_name": "Bermudes (les)",
         "numeric_code": 60
     },
-    {
+    "BOL": {
         "alpha_2_code": "BO",
         "alpha_3_code": "BOL",
         "english_name": "Bolivia (Plurinational State of)",
         "french_name": "Bolivie (\u00c9tat plurinational de)",
         "numeric_code": 68
     },
-    {
+    "BRA": {
         "alpha_2_code": "BR",
         "alpha_3_code": "BRA",
         "english_name": "Brazil",
         "french_name": "Br\u00e9sil (le)",
         "numeric_code": 76
     },
-    {
+    "BRB": {
         "alpha_2_code": "BB",
         "alpha_3_code": "BRB",
         "english_name": "Barbados",
         "french_name": "Barbade (la)",
         "numeric_code": 52
     },
-    {
+    "BRN": {
         "alpha_2_code": "BN",
         "alpha_3_code": "BRN",
         "english_name": "Brunei Darussalam",
         "french_name": "Brun\u00e9i Darussalam (le)",
         "numeric_code": 96
     },
-    {
+    "BTN": {
         "alpha_2_code": "BT",
         "alpha_3_code": "BTN",
         "english_name": "Bhutan",
         "french_name": "Bhoutan (le)",
         "numeric_code": 64
     },
-    {
+    "BVT": {
         "alpha_2_code": "BV",
         "alpha_3_code": "BVT",
         "english_name": "Bouvet Island",
         "french_name": "Bouvet (l'\u00cele)",
         "numeric_code": 74
     },
-    {
+    "BWA": {
         "alpha_2_code": "BW",
         "alpha_3_code": "BWA",
         "english_name": "Botswana",
         "french_name": "Botswana (le)",
         "numeric_code": 72
     },
-    {
+    "CAF": {
         "alpha_2_code": "CF",
         "alpha_3_code": "CAF",
         "english_name": "Central African Republic (the)",
         "french_name": "R\u00e9publique centrafricaine (la)",
         "numeric_code": 140
     },
-    {
+    "CAN": {
         "alpha_2_code": "CA",
         "alpha_3_code": "CAN",
         "english_name": "Canada",
         "french_name": "Canada (le)",
         "numeric_code": 124
     },
-    {
+    "CCK": {
         "alpha_2_code": "CC",
         "alpha_3_code": "CCK",
         "english_name": "Cocos (Keeling) Islands (the)",
         "french_name": "Cocos (les \u00celes)/ Keeling (les \u00celes)",
         "numeric_code": 166
     },
-    {
+    "CHE": {
         "alpha_2_code": "CH",
         "alpha_3_code": "CHE",
         "english_name": "Switzerland",
         "french_name": "Suisse (la)",
         "numeric_code": 756
     },
-    {
+    "CHL": {
         "alpha_2_code": "CL",
         "alpha_3_code": "CHL",
         "english_name": "Chile",
         "french_name": "Chili (le)",
         "numeric_code": 152
     },
-    {
+    "CHN": {
         "alpha_2_code": "CN",
         "alpha_3_code": "CHN",
         "english_name": "China",
         "french_name": "Chine (la)",
         "numeric_code": 156
     },
-    {
+    "CIV": {
         "alpha_2_code": "CI",
         "alpha_3_code": "CIV",
         "english_name": "C\u00f4te d'Ivoire",
         "french_name": "C\u00f4te d'Ivoire (la)",
         "numeric_code": 384
     },
-    {
+    "CMR": {
         "alpha_2_code": "CM",
         "alpha_3_code": "CMR",
         "english_name": "Cameroon",
         "french_name": "Cameroun (le)",
         "numeric_code": 120
     },
-    {
+    "COD": {
         "alpha_2_code": "CD",
         "alpha_3_code": "COD",
         "english_name": "Congo (the Democratic Republic of the)",
         "french_name": "Congo (la R\u00e9publique d\u00e9mocratique du)",
         "numeric_code": 180
     },
-    {
+    "COG": {
         "alpha_2_code": "CG",
         "alpha_3_code": "COG",
         "english_name": "Congo (the)",
         "french_name": "Congo (le)",
         "numeric_code": 178
     },
-    {
+    "COK": {
         "alpha_2_code": "CK",
         "alpha_3_code": "COK",
         "english_name": "Cook Islands (the)",
         "french_name": "Cook (les \u00celes)",
         "numeric_code": 184
     },
-    {
+    "COL": {
         "alpha_2_code": "CO",
         "alpha_3_code": "COL",
         "english_name": "Colombia",
         "french_name": "Colombie (la)",
         "numeric_code": 170
     },
-    {
+    "COM": {
         "alpha_2_code": "KM",
         "alpha_3_code": "COM",
         "english_name": "Comoros (the)",
         "french_name": "Comores (les)",
         "numeric_code": 174
     },
-    {
+    "CPV": {
         "alpha_2_code": "CV",
         "alpha_3_code": "CPV",
         "english_name": "Cabo Verde",
         "french_name": "Cabo Verde",
         "numeric_code": 132
     },
-    {
+    "CRI": {
         "alpha_2_code": "CR",
         "alpha_3_code": "CRI",
         "english_name": "Costa Rica",
         "french_name": "Costa Rica (le)",
         "numeric_code": 188
     },
-    {
+    "CUB": {
         "alpha_2_code": "CU",
         "alpha_3_code": "CUB",
         "english_name": "Cuba",
         "french_name": "Cuba",
         "numeric_code": 192
     },
-    {
+    "CUW": {
         "alpha_2_code": "CW",
         "alpha_3_code": "CUW",
         "english_name": "Cura\u00e7ao",
         "french_name": "Cura\u00e7ao",
         "numeric_code": 531
     },
-    {
+    "CXR": {
         "alpha_2_code": "CX",
         "alpha_3_code": "CXR",
         "english_name": "Christmas Island",
         "french_name": "Christmas (l'\u00cele)",
         "numeric_code": 162
     },
-    {
+    "CYM": {
         "alpha_2_code": "KY",
         "alpha_3_code": "CYM",
         "english_name": "Cayman Islands (the)",
         "french_name": "Ca\u00efmans (les \u00celes)",
         "numeric_code": 136
     },
-    {
+    "CYP": {
         "alpha_2_code": "CY",
         "alpha_3_code": "CYP",
         "english_name": "Cyprus",
         "french_name": "Chypre",
         "numeric_code": 196
     },
-    {
+    "CZE": {
         "alpha_2_code": "CZ",
         "alpha_3_code": "CZE",
         "english_name": "Czechia",
         "french_name": "Tch\u00e9quie (la)",
         "numeric_code": 203
     },
-    {
+    "DEU": {
         "alpha_2_code": "DE",
         "alpha_3_code": "DEU",
         "english_name": "Germany",
         "french_name": "Allemagne (l')",
         "numeric_code": 276
     },
-    {
+    "DJI": {
         "alpha_2_code": "DJ",
         "alpha_3_code": "DJI",
         "english_name": "Djibouti",
         "french_name": "Djibouti",
         "numeric_code": 262
     },
-    {
+    "DMA": {
         "alpha_2_code": "DM",
         "alpha_3_code": "DMA",
         "english_name": "Dominica",
         "french_name": "Dominique (la)",
         "numeric_code": 212
     },
-    {
+    "DNK": {
         "alpha_2_code": "DK",
         "alpha_3_code": "DNK",
         "english_name": "Denmark",
         "french_name": "Danemark (le)",
         "numeric_code": 208
     },
-    {
+    "DOM": {
         "alpha_2_code": "DO",
         "alpha_3_code": "DOM",
         "english_name": "Dominican Republic (the)",
         "french_name": "dominicaine (la R\u00e9publique)",
         "numeric_code": 214
     },
-    {
+    "DZA": {
         "alpha_2_code": "DZ",
         "alpha_3_code": "DZA",
         "english_name": "Algeria",
         "french_name": "Alg\u00e9rie (l')",
         "numeric_code": 12
     },
-    {
+    "ECU": {
         "alpha_2_code": "EC",
         "alpha_3_code": "ECU",
         "english_name": "Ecuador",
         "french_name": "\u00c9quateur (l')",
         "numeric_code": 218
     },
-    {
+    "EGY": {
         "alpha_2_code": "EG",
         "alpha_3_code": "EGY",
         "english_name": "Egypt",
         "french_name": "\u00c9gypte (l')",
         "numeric_code": 818
     },
-    {
+    "ERI": {
         "alpha_2_code": "ER",
         "alpha_3_code": "ERI",
         "english_name": "Eritrea",
         "french_name": "\u00c9rythr\u00e9e (l')",
         "numeric_code": 232
     },
-    {
+    "ESH": {
         "alpha_2_code": "EH",
         "alpha_3_code": "ESH",
         "english_name": "Western Sahara*",
         "french_name": "Sahara occidental (le)*",
         "numeric_code": 732
     },
-    {
+    "ESP": {
         "alpha_2_code": "ES",
         "alpha_3_code": "ESP",
         "english_name": "Spain",
         "french_name": "Espagne (l')",
         "numeric_code": 724
     },
-    {
+    "EST": {
         "alpha_2_code": "EE",
         "alpha_3_code": "EST",
         "english_name": "Estonia",
         "french_name": "Estonie (l')",
         "numeric_code": 233
     },
-    {
+    "ETH": {
         "alpha_2_code": "ET",
         "alpha_3_code": "ETH",
         "english_name": "Ethiopia",
         "french_name": "\u00c9thiopie (l')",
         "numeric_code": 231
     },
-    {
+    "FIN": {
         "alpha_2_code": "FI",
         "alpha_3_code": "FIN",
         "english_name": "Finland",
         "french_name": "Finlande (la)",
         "numeric_code": 246
     },
-    {
+    "FJI": {
         "alpha_2_code": "FJ",
         "alpha_3_code": "FJI",
         "english_name": "Fiji",
         "french_name": "Fidji (les)",
         "numeric_code": 242
     },
-    {
+    "FLK": {
         "alpha_2_code": "FK",
         "alpha_3_code": "FLK",
         "english_name": "Falkland Islands (the) [Malvinas]",
         "french_name": "Falkland (les \u00celes)/Malouines (les \u00celes)",
         "numeric_code": 238
     },
-    {
+    "FRA": {
         "alpha_2_code": "FR",
         "alpha_3_code": "FRA",
         "english_name": "France",
         "french_name": "France (la)",
         "numeric_code": 250
     },
-    {
+    "FRO": {
         "alpha_2_code": "FO",
         "alpha_3_code": "FRO",
         "english_name": "Faroe Islands (the)",
         "french_name": "F\u00e9ro\u00e9 (les \u00celes)",
         "numeric_code": 234
     },
-    {
+    "FSM": {
         "alpha_2_code": "FM",
         "alpha_3_code": "FSM",
         "english_name": "Micronesia (Federated States of)",
         "french_name": "Micron\u00e9sie (\u00c9tats f\u00e9d\u00e9r\u00e9s de)",
         "numeric_code": 583
     },
-    {
+    "GAB": {
         "alpha_2_code": "GA",
         "alpha_3_code": "GAB",
         "english_name": "Gabon",
         "french_name": "Gabon (le)",
         "numeric_code": 266
     },
-    {
+    "GBR": {
         "alpha_2_code": "GB",
         "alpha_3_code": "GBR",
         "english_name": "United Kingdom of Great Britain and Northern Ireland (the)",
         "french_name": "Royaume-Uni de Grande-Bretagne et d'Irlande du Nord (le)",
         "numeric_code": 826
     },
-    {
+    "GEO": {
         "alpha_2_code": "GE",
         "alpha_3_code": "GEO",
         "english_name": "Georgia",
         "french_name": "G\u00e9orgie (la)",
         "numeric_code": 268
     },
-    {
+    "GGY": {
         "alpha_2_code": "GG",
         "alpha_3_code": "GGY",
         "english_name": "Guernsey",
         "french_name": "Guernesey",
         "numeric_code": 831
     },
-    {
+    "GHA": {
         "alpha_2_code": "GH",
         "alpha_3_code": "GHA",
         "english_name": "Ghana",
         "french_name": "Ghana (le)",
         "numeric_code": 288
     },
-    {
+    "GIB": {
         "alpha_2_code": "GI",
         "alpha_3_code": "GIB",
         "english_name": "Gibraltar",
         "french_name": "Gibraltar",
         "numeric_code": 292
     },
-    {
+    "GIN": {
         "alpha_2_code": "GN",
         "alpha_3_code": "GIN",
         "english_name": "Guinea",
         "french_name": "Guin\u00e9e (la)",
         "numeric_code": 324
     },
-    {
+    "GLP": {
         "alpha_2_code": "GP",
         "alpha_3_code": "GLP",
         "english_name": "Guadeloupe",
         "french_name": "Guadeloupe (la)",
         "numeric_code": 312
     },
-    {
+    "GMB": {
         "alpha_2_code": "GM",
         "alpha_3_code": "GMB",
         "english_name": "Gambia (the)",
         "french_name": "Gambie (la)",
         "numeric_code": 270
     },
-    {
+    "GNB": {
         "alpha_2_code": "GW",
         "alpha_3_code": "GNB",
         "english_name": "Guinea-Bissau",
         "french_name": "Guin\u00e9e-Bissau (la)",
         "numeric_code": 624
     },
-    {
+    "GNQ": {
         "alpha_2_code": "GQ",
         "alpha_3_code": "GNQ",
         "english_name": "Equatorial Guinea",
         "french_name": "Guin\u00e9e \u00e9quatoriale (la)",
         "numeric_code": 226
     },
-    {
+    "GRC": {
         "alpha_2_code": "GR",
         "alpha_3_code": "GRC",
         "english_name": "Greece",
         "french_name": "Gr\u00e8ce (la)",
         "numeric_code": 300
     },
-    {
+    "GRD": {
         "alpha_2_code": "GD",
         "alpha_3_code": "GRD",
         "english_name": "Grenada",
         "french_name": "Grenade (la)",
         "numeric_code": 308
     },
-    {
+    "GRL": {
         "alpha_2_code": "GL",
         "alpha_3_code": "GRL",
         "english_name": "Greenland",
         "french_name": "Groenland (le)",
         "numeric_code": 304
     },
-    {
+    "GTM": {
         "alpha_2_code": "GT",
         "alpha_3_code": "GTM",
         "english_name": "Guatemala",
         "french_name": "Guatemala (le)",
         "numeric_code": 320
     },
-    {
+    "GUF": {
         "alpha_2_code": "GF",
         "alpha_3_code": "GUF",
         "english_name": "French Guiana",
         "french_name": "Guyane fran\u00e7aise (la )",
         "numeric_code": 254
     },
-    {
+    "GUM": {
         "alpha_2_code": "GU",
         "alpha_3_code": "GUM",
         "english_name": "Guam",
         "french_name": "Guam",
         "numeric_code": 316
     },
-    {
+    "GUY": {
         "alpha_2_code": "GY",
         "alpha_3_code": "GUY",
         "english_name": "Guyana",
         "french_name": "Guyana (le)",
         "numeric_code": 328
     },
-    {
+    "HKG": {
         "alpha_2_code": "HK",
         "alpha_3_code": "HKG",
         "english_name": "Hong Kong",
         "french_name": "Hong Kong",
         "numeric_code": 344
     },
-    {
+    "HMD": {
         "alpha_2_code": "HM",
         "alpha_3_code": "HMD",
         "english_name": "Heard Island and McDonald Islands",
         "french_name": "Heard-et-\u00celes MacDonald (l'\u00cele)",
         "numeric_code": 334
     },
-    {
+    "HND": {
         "alpha_2_code": "HN",
         "alpha_3_code": "HND",
         "english_name": "Honduras",
         "french_name": "Honduras (le)",
         "numeric_code": 340
     },
-    {
+    "HRV": {
         "alpha_2_code": "HR",
         "alpha_3_code": "HRV",
         "english_name": "Croatia",
         "french_name": "Croatie (la)",
         "numeric_code": 191
     },
-    {
+    "HTI": {
         "alpha_2_code": "HT",
         "alpha_3_code": "HTI",
         "english_name": "Haiti",
         "french_name": "Ha\u00efti",
         "numeric_code": 332
     },
-    {
+    "HUN": {
         "alpha_2_code": "HU",
         "alpha_3_code": "HUN",
         "english_name": "Hungary",
         "french_name": "Hongrie (la)",
         "numeric_code": 348
     },
-    {
+    "IDN": {
         "alpha_2_code": "ID",
         "alpha_3_code": "IDN",
         "english_name": "Indonesia",
         "french_name": "Indon\u00e9sie (l')",
         "numeric_code": 360
     },
-    {
+    "IMN": {
         "alpha_2_code": "IM",
         "alpha_3_code": "IMN",
         "english_name": "Isle of Man",
         "french_name": "\u00cele de Man",
         "numeric_code": 833
     },
-    {
+    "IND": {
         "alpha_2_code": "IN",
         "alpha_3_code": "IND",
         "english_name": "India",
         "french_name": "Inde (l')",
         "numeric_code": 356
     },
-    {
+    "IOT": {
         "alpha_2_code": "IO",
         "alpha_3_code": "IOT",
         "english_name": "British Indian Ocean Territory (the)",
         "french_name": "Indien (le Territoire britannique de l'oc\u00e9an)",
         "numeric_code": 86
     },
-    {
+    "IRL": {
         "alpha_2_code": "IE",
         "alpha_3_code": "IRL",
         "english_name": "Ireland",
         "french_name": "Irlande (l')",
         "numeric_code": 372
     },
-    {
+    "IRN": {
         "alpha_2_code": "IR",
         "alpha_3_code": "IRN",
         "english_name": "Iran (Islamic Republic of)",
         "french_name": "Iran (R\u00e9publique Islamique d')",
         "numeric_code": 364
     },
-    {
+    "IRQ": {
         "alpha_2_code": "IQ",
         "alpha_3_code": "IRQ",
         "english_name": "Iraq",
         "french_name": "Iraq (l')",
         "numeric_code": 368
     },
-    {
+    "ISL": {
         "alpha_2_code": "IS",
         "alpha_3_code": "ISL",
         "english_name": "Iceland",
         "french_name": "Islande (l')",
         "numeric_code": 352
     },
-    {
+    "ISR": {
         "alpha_2_code": "IL",
         "alpha_3_code": "ISR",
         "english_name": "Israel",
         "french_name": "Isra\u00ebl",
         "numeric_code": 376
     },
-    {
+    "ITA": {
         "alpha_2_code": "IT",
         "alpha_3_code": "ITA",
         "english_name": "Italy",
         "french_name": "Italie (l')",
         "numeric_code": 380
     },
-    {
+    "JAM": {
         "alpha_2_code": "JM",
         "alpha_3_code": "JAM",
         "english_name": "Jamaica",
         "french_name": "Jama\u00efque (la)",
         "numeric_code": 388
     },
-    {
+    "JEY": {
         "alpha_2_code": "JE",
         "alpha_3_code": "JEY",
         "english_name": "Jersey",
         "french_name": "Jersey",
         "numeric_code": 832
     },
-    {
+    "JOR": {
         "alpha_2_code": "JO",
         "alpha_3_code": "JOR",
         "english_name": "Jordan",
         "french_name": "Jordanie (la)",
         "numeric_code": 400
     },
-    {
+    "JPN": {
         "alpha_2_code": "JP",
         "alpha_3_code": "JPN",
         "english_name": "Japan",
         "french_name": "Japon (le)",
         "numeric_code": 392
     },
-    {
+    "KAZ": {
         "alpha_2_code": "KZ",
         "alpha_3_code": "KAZ",
         "english_name": "Kazakhstan",
         "french_name": "Kazakhstan (le)",
         "numeric_code": 398
     },
-    {
+    "KEN": {
         "alpha_2_code": "KE",
         "alpha_3_code": "KEN",
         "english_name": "Kenya",
         "french_name": "Kenya (le)",
         "numeric_code": 404
     },
-    {
+    "KGZ": {
         "alpha_2_code": "KG",
         "alpha_3_code": "KGZ",
         "english_name": "Kyrgyzstan",
         "french_name": "Kirghizistan (le)",
         "numeric_code": 417
     },
-    {
+    "KHM": {
         "alpha_2_code": "KH",
         "alpha_3_code": "KHM",
         "english_name": "Cambodia",
         "french_name": "Cambodge (le)",
         "numeric_code": 116
     },
-    {
+    "KIR": {
         "alpha_2_code": "KI",
         "alpha_3_code": "KIR",
         "english_name": "Kiribati",
         "french_name": "Kiribati",
         "numeric_code": 296
     },
-    {
+    "KNA": {
         "alpha_2_code": "KN",
         "alpha_3_code": "KNA",
         "english_name": "Saint Kitts and Nevis",
         "french_name": "Saint-Kitts-et-Nevis",
         "numeric_code": 659
     },
-    {
+    "KOR": {
         "alpha_2_code": "KR",
         "alpha_3_code": "KOR",
         "english_name": "Korea (the Republic of)",
         "french_name": "Cor\u00e9e (la R\u00e9publique de)",
         "numeric_code": 410
     },
-    {
+    "KWT": {
         "alpha_2_code": "KW",
         "alpha_3_code": "KWT",
         "english_name": "Kuwait",
         "french_name": "Kowe\u00eft (le)",
         "numeric_code": 414
     },
-    {
+    "LAO": {
         "alpha_2_code": "LA",
         "alpha_3_code": "LAO",
         "english_name": "Lao People's Democratic Republic (the)",
         "french_name": "Lao (la R\u00e9publique d\u00e9mocratique populaire)",
         "numeric_code": 418
     },
-    {
+    "LBN": {
         "alpha_2_code": "LB",
         "alpha_3_code": "LBN",
         "english_name": "Lebanon",
         "french_name": "Liban (le)",
         "numeric_code": 422
     },
-    {
+    "LBR": {
         "alpha_2_code": "LR",
         "alpha_3_code": "LBR",
         "english_name": "Liberia",
         "french_name": "Lib\u00e9ria (le)",
         "numeric_code": 430
     },
-    {
+    "LBY": {
         "alpha_2_code": "LY",
         "alpha_3_code": "LBY",
         "english_name": "Libya",
         "french_name": "Libye (la)",
         "numeric_code": 434
     },
-    {
+    "LCA": {
         "alpha_2_code": "LC",
         "alpha_3_code": "LCA",
         "english_name": "Saint Lucia",
         "french_name": "Sainte-Lucie",
         "numeric_code": 662
     },
-    {
+    "LIE": {
         "alpha_2_code": "LI",
         "alpha_3_code": "LIE",
         "english_name": "Liechtenstein",
         "french_name": "Liechtenstein (le)",
         "numeric_code": 438
     },
-    {
+    "LKA": {
         "alpha_2_code": "LK",
         "alpha_3_code": "LKA",
         "english_name": "Sri Lanka",
         "french_name": "Sri Lanka",
         "numeric_code": 144
     },
-    {
+    "LSO": {
         "alpha_2_code": "LS",
         "alpha_3_code": "LSO",
         "english_name": "Lesotho",
         "french_name": "Lesotho (le)",
         "numeric_code": 426
     },
-    {
+    "LTU": {
         "alpha_2_code": "LT",
         "alpha_3_code": "LTU",
         "english_name": "Lithuania",
         "french_name": "Lituanie (la)",
         "numeric_code": 440
     },
-    {
+    "LUX": {
         "alpha_2_code": "LU",
         "alpha_3_code": "LUX",
         "english_name": "Luxembourg",
         "french_name": "Luxembourg (le)",
         "numeric_code": 442
     },
-    {
+    "LVA": {
         "alpha_2_code": "LV",
         "alpha_3_code": "LVA",
         "english_name": "Latvia",
         "french_name": "Lettonie (la)",
         "numeric_code": 428
     },
-    {
+    "MAC": {
         "alpha_2_code": "MO",
         "alpha_3_code": "MAC",
         "english_name": "Macao",
         "french_name": "Macao",
         "numeric_code": 446
     },
-    {
+    "MAF": {
         "alpha_2_code": "MF",
         "alpha_3_code": "MAF",
         "english_name": "Saint Martin (French part)",
         "french_name": "Saint-Martin (partie fran\u00e7aise)",
         "numeric_code": 663
     },
-    {
+    "MAR": {
         "alpha_2_code": "MA",
         "alpha_3_code": "MAR",
         "english_name": "Morocco",
         "french_name": "Maroc (le)",
         "numeric_code": 504
     },
-    {
+    "MCO": {
         "alpha_2_code": "MC",
         "alpha_3_code": "MCO",
         "english_name": "Monaco",
         "french_name": "Monaco",
         "numeric_code": 492
     },
-    {
+    "MDA": {
         "alpha_2_code": "MD",
         "alpha_3_code": "MDA",
         "english_name": "Moldova (the Republic of)",
         "french_name": "Moldova (la R\u00e9publique de)",
         "numeric_code": 498
     },
-    {
+    "MDG": {
         "alpha_2_code": "MG",
         "alpha_3_code": "MDG",
         "english_name": "Madagascar",
         "french_name": "Madagascar",
         "numeric_code": 450
     },
-    {
+    "MDV": {
         "alpha_2_code": "MV",
         "alpha_3_code": "MDV",
         "english_name": "Maldives",
         "french_name": "Maldives (les)",
         "numeric_code": 462
     },
-    {
+    "MEX": {
         "alpha_2_code": "MX",
         "alpha_3_code": "MEX",
         "english_name": "Mexico",
         "french_name": "Mexique (le)",
         "numeric_code": 484
     },
-    {
+    "MHL": {
         "alpha_2_code": "MH",
         "alpha_3_code": "MHL",
         "english_name": "Marshall Islands (the)",
         "french_name": "Marshall (les \u00celes)",
         "numeric_code": 584
     },
-    {
+    "MKD": {
         "alpha_2_code": "MK",
         "alpha_3_code": "MKD",
         "english_name": "North Macedonia",
         "french_name": "Mac\u00e9doine du Nord (la)",
         "numeric_code": 807
     },
-    {
+    "MLI": {
         "alpha_2_code": "ML",
         "alpha_3_code": "MLI",
         "english_name": "Mali",
         "french_name": "Mali (le)",
         "numeric_code": 466
     },
-    {
+    "MLT": {
         "alpha_2_code": "MT",
         "alpha_3_code": "MLT",
         "english_name": "Malta",
         "french_name": "Malte",
         "numeric_code": 470
     },
-    {
+    "MMR": {
         "alpha_2_code": "MM",
         "alpha_3_code": "MMR",
         "english_name": "Myanmar",
         "french_name": "Myanmar (le)",
         "numeric_code": 104
     },
-    {
+    "MNE": {
         "alpha_2_code": "ME",
         "alpha_3_code": "MNE",
         "english_name": "Montenegro",
         "french_name": "Mont\u00e9n\u00e9gro (le)",
         "numeric_code": 499
     },
-    {
+    "MNG": {
         "alpha_2_code": "MN",
         "alpha_3_code": "MNG",
         "english_name": "Mongolia",
         "french_name": "Mongolie (la)",
         "numeric_code": 496
     },
-    {
+    "MNP": {
         "alpha_2_code": "MP",
         "alpha_3_code": "MNP",
         "english_name": "Northern Mariana Islands (the)",
         "french_name": "Mariannes du Nord (les \u00celes)",
         "numeric_code": 580
     },
-    {
+    "MOZ": {
         "alpha_2_code": "MZ",
         "alpha_3_code": "MOZ",
         "english_name": "Mozambique",
         "french_name": "Mozambique (le)",
         "numeric_code": 508
     },
-    {
+    "MRT": {
         "alpha_2_code": "MR",
         "alpha_3_code": "MRT",
         "english_name": "Mauritania",
         "french_name": "Mauritanie (la)",
         "numeric_code": 478
     },
-    {
+    "MSR": {
         "alpha_2_code": "MS",
         "alpha_3_code": "MSR",
         "english_name": "Montserrat",
         "french_name": "Montserrat",
         "numeric_code": 500
     },
-    {
+    "MTQ": {
         "alpha_2_code": "MQ",
         "alpha_3_code": "MTQ",
         "english_name": "Martinique",
         "french_name": "Martinique (la)",
         "numeric_code": 474
     },
-    {
+    "MUS": {
         "alpha_2_code": "MU",
         "alpha_3_code": "MUS",
         "english_name": "Mauritius",
         "french_name": "Maurice",
         "numeric_code": 480
     },
-    {
+    "MWI": {
         "alpha_2_code": "MW",
         "alpha_3_code": "MWI",
         "english_name": "Malawi",
         "french_name": "Malawi (le)",
         "numeric_code": 454
     },
-    {
+    "MYS": {
         "alpha_2_code": "MY",
         "alpha_3_code": "MYS",
         "english_name": "Malaysia",
         "french_name": "Malaisie (la)",
         "numeric_code": 458
     },
-    {
+    "MYT": {
         "alpha_2_code": "YT",
         "alpha_3_code": "MYT",
         "english_name": "Mayotte",
         "french_name": "Mayotte",
         "numeric_code": 175
     },
-    {
+    "NAM": {
         "alpha_2_code": "NA",
         "alpha_3_code": "NAM",
         "english_name": "Namibia",
         "french_name": "Namibie (la)",
         "numeric_code": 516
     },
-    {
+    "NCL": {
         "alpha_2_code": "NC",
         "alpha_3_code": "NCL",
         "english_name": "New Caledonia",
         "french_name": "Nouvelle-Cal\u00e9donie (la)",
         "numeric_code": 540
     },
-    {
+    "NER": {
         "alpha_2_code": "NE",
         "alpha_3_code": "NER",
         "english_name": "Niger (the)",
         "french_name": "Niger (le)",
         "numeric_code": 562
     },
-    {
+    "NFK": {
         "alpha_2_code": "NF",
         "alpha_3_code": "NFK",
         "english_name": "Norfolk Island",
         "french_name": "Norfolk (l'\u00cele)",
         "numeric_code": 574
     },
-    {
+    "NGA": {
         "alpha_2_code": "NG",
         "alpha_3_code": "NGA",
         "english_name": "Nigeria",
         "french_name": "Nig\u00e9ria (le)",
         "numeric_code": 566
     },
-    {
+    "NIC": {
         "alpha_2_code": "NI",
         "alpha_3_code": "NIC",
         "english_name": "Nicaragua",
         "french_name": "Nicaragua (le)",
         "numeric_code": 558
     },
-    {
+    "NIU": {
         "alpha_2_code": "NU",
         "alpha_3_code": "NIU",
         "english_name": "Niue",
         "french_name": "Niue",
         "numeric_code": 570
     },
-    {
+    "NLD": {
         "alpha_2_code": "NL",
         "alpha_3_code": "NLD",
-        "english_name": "Netherlands (the)",
-        "french_name": "Pays-Bas (les)",
+        "english_name": "Netherlands (Kingdom of the)",
+        "french_name": "Pays-Bas (Royaume des)",
         "numeric_code": 528
     },
-    {
+    "NOR": {
         "alpha_2_code": "NO",
         "alpha_3_code": "NOR",
         "english_name": "Norway",
         "french_name": "Norv\u00e8ge (la)",
         "numeric_code": 578
     },
-    {
+    "NPL": {
         "alpha_2_code": "NP",
         "alpha_3_code": "NPL",
         "english_name": "Nepal",
         "french_name": "N\u00e9pal (le)",
         "numeric_code": 524
     },
-    {
+    "NRU": {
         "alpha_2_code": "NR",
         "alpha_3_code": "NRU",
         "english_name": "Nauru",
         "french_name": "Nauru",
         "numeric_code": 520
     },
-    {
+    "NZL": {
         "alpha_2_code": "NZ",
         "alpha_3_code": "NZL",
         "english_name": "New Zealand",
         "french_name": "Nouvelle-Z\u00e9lande (la)",
         "numeric_code": 554
     },
-    {
+    "OMN": {
         "alpha_2_code": "OM",
         "alpha_3_code": "OMN",
         "english_name": "Oman",
         "french_name": "Oman",
         "numeric_code": 512
     },
-    {
+    "PAK": {
         "alpha_2_code": "PK",
         "alpha_3_code": "PAK",
         "english_name": "Pakistan",
         "french_name": "Pakistan (le)",
         "numeric_code": 586
     },
-    {
+    "PAN": {
         "alpha_2_code": "PA",
         "alpha_3_code": "PAN",
         "english_name": "Panama",
         "french_name": "Panama (le)",
         "numeric_code": 591
     },
-    {
+    "PCN": {
         "alpha_2_code": "PN",
         "alpha_3_code": "PCN",
         "english_name": "Pitcairn",
         "french_name": "Pitcairn",
         "numeric_code": 612
     },
-    {
+    "PER": {
         "alpha_2_code": "PE",
         "alpha_3_code": "PER",
         "english_name": "Peru",
         "french_name": "P\u00e9rou (le)",
         "numeric_code": 604
     },
-    {
+    "PHL": {
         "alpha_2_code": "PH",
         "alpha_3_code": "PHL",
         "english_name": "Philippines (the)",
         "french_name": "Philippines (les)",
         "numeric_code": 608
     },
-    {
+    "PLW": {
         "alpha_2_code": "PW",
         "alpha_3_code": "PLW",
         "english_name": "Palau",
         "french_name": "Palaos (les)",
         "numeric_code": 585
     },
-    {
+    "PNG": {
         "alpha_2_code": "PG",
         "alpha_3_code": "PNG",
         "english_name": "Papua New Guinea",
         "french_name": "Papouasie-Nouvelle-Guin\u00e9e (la)",
         "numeric_code": 598
     },
-    {
+    "POL": {
         "alpha_2_code": "PL",
         "alpha_3_code": "POL",
         "english_name": "Poland",
         "french_name": "Pologne (la)",
         "numeric_code": 616
     },
-    {
+    "PRI": {
         "alpha_2_code": "PR",
         "alpha_3_code": "PRI",
         "english_name": "Puerto Rico",
         "french_name": "Porto Rico",
         "numeric_code": 630
     },
-    {
+    "PRK": {
         "alpha_2_code": "KP",
         "alpha_3_code": "PRK",
         "english_name": "Korea (the Democratic People's Republic of)",
         "french_name": "Cor\u00e9e (la R\u00e9publique populaire d\u00e9mocratique de)",
         "numeric_code": 408
     },
-    {
+    "PRT": {
         "alpha_2_code": "PT",
         "alpha_3_code": "PRT",
         "english_name": "Portugal",
         "french_name": "Portugal (le)",
         "numeric_code": 620
     },
-    {
+    "PRY": {
         "alpha_2_code": "PY",
         "alpha_3_code": "PRY",
         "english_name": "Paraguay",
         "french_name": "Paraguay (le)",
         "numeric_code": 600
     },
-    {
+    "PSE": {
         "alpha_2_code": "PS",
         "alpha_3_code": "PSE",
         "english_name": "Palestine, State of",
         "french_name": "Palestine, \u00c9tat de",
         "numeric_code": 275
     },
-    {
+    "PYF": {
         "alpha_2_code": "PF",
         "alpha_3_code": "PYF",
         "english_name": "French Polynesia",
         "french_name": "Polyn\u00e9sie fran\u00e7aise (la)",
         "numeric_code": 258
     },
-    {
+    "QAT": {
         "alpha_2_code": "QA",
         "alpha_3_code": "QAT",
         "english_name": "Qatar",
         "french_name": "Qatar (le)",
         "numeric_code": 634
     },
-    {
+    "REU": {
         "alpha_2_code": "RE",
         "alpha_3_code": "REU",
         "english_name": "R\u00e9union",
         "french_name": "R\u00e9union (La)",
         "numeric_code": 638
     },
-    {
+    "ROU": {
         "alpha_2_code": "RO",
         "alpha_3_code": "ROU",
         "english_name": "Romania",
         "french_name": "Roumanie (la)",
         "numeric_code": 642
     },
-    {
+    "RUS": {
         "alpha_2_code": "RU",
         "alpha_3_code": "RUS",
         "english_name": "Russian Federation (the)",
         "french_name": "Russie (la F\u00e9d\u00e9ration de)",
         "numeric_code": 643
     },
-    {
+    "RWA": {
         "alpha_2_code": "RW",
         "alpha_3_code": "RWA",
         "english_name": "Rwanda",
         "french_name": "Rwanda (le)",
         "numeric_code": 646
     },
-    {
+    "SAU": {
         "alpha_2_code": "SA",
         "alpha_3_code": "SAU",
         "english_name": "Saudi Arabia",
         "french_name": "Arabie saoudite (l')",
         "numeric_code": 682
     },
-    {
+    "SDN": {
         "alpha_2_code": "SD",
         "alpha_3_code": "SDN",
         "english_name": "Sudan (the)",
         "french_name": "Soudan (le)",
         "numeric_code": 729
     },
-    {
+    "SEN": {
         "alpha_2_code": "SN",
         "alpha_3_code": "SEN",
         "english_name": "Senegal",
         "french_name": "S\u00e9n\u00e9gal (le)",
         "numeric_code": 686
     },
-    {
+    "SGP": {
         "alpha_2_code": "SG",
         "alpha_3_code": "SGP",
         "english_name": "Singapore",
         "french_name": "Singapour",
         "numeric_code": 702
     },
-    {
+    "SGS": {
         "alpha_2_code": "GS",
         "alpha_3_code": "SGS",
         "english_name": "South Georgia and the South Sandwich Islands",
         "french_name": "G\u00e9orgie du Sud-et-les \u00celes Sandwich du Sud (la)",
         "numeric_code": 239
     },
-    {
+    "SHN": {
         "alpha_2_code": "SH",
         "alpha_3_code": "SHN",
         "english_name": "Saint Helena, Ascension and Tristan da Cunha",
         "french_name": "Sainte-H\u00e9l\u00e8ne, Ascension et Tristan da Cunha",
         "numeric_code": 654
     },
-    {
+    "SJM": {
         "alpha_2_code": "SJ",
         "alpha_3_code": "SJM",
         "english_name": "Svalbard and Jan Mayen",
         "french_name": "Svalbard et l'\u00cele Jan Mayen (le)",
         "numeric_code": 744
     },
-    {
+    "SLB": {
         "alpha_2_code": "SB",
         "alpha_3_code": "SLB",
         "english_name": "Solomon Islands",
         "french_name": "Salomon (les \u00celes)",
         "numeric_code": 90
     },
-    {
+    "SLE": {
         "alpha_2_code": "SL",
         "alpha_3_code": "SLE",
         "english_name": "Sierra Leone",
         "french_name": "Sierra Leone (la)",
         "numeric_code": 694
     },
-    {
+    "SLV": {
         "alpha_2_code": "SV",
         "alpha_3_code": "SLV",
         "english_name": "El Salvador",
         "french_name": "El Salvador",
         "numeric_code": 222
     },
-    {
+    "SMR": {
         "alpha_2_code": "SM",
         "alpha_3_code": "SMR",
         "english_name": "San Marino",
         "french_name": "Saint-Marin",
         "numeric_code": 674
     },
-    {
+    "SOM": {
         "alpha_2_code": "SO",
         "alpha_3_code": "SOM",
         "english_name": "Somalia",
         "french_name": "Somalie (la)",
         "numeric_code": 706
     },
-    {
+    "SPM": {
         "alpha_2_code": "PM",
         "alpha_3_code": "SPM",
         "english_name": "Saint Pierre and Miquelon",
         "french_name": "Saint-Pierre-et-Miquelon",
         "numeric_code": 666
     },
-    {
+    "SRB": {
         "alpha_2_code": "RS",
         "alpha_3_code": "SRB",
         "english_name": "Serbia",
         "french_name": "Serbie (la)",
         "numeric_code": 688
     },
-    {
+    "SSD": {
         "alpha_2_code": "SS",
         "alpha_3_code": "SSD",
         "english_name": "South Sudan",
         "french_name": "Soudan du Sud (le)",
         "numeric_code": 728
     },
-    {
+    "STP": {
         "alpha_2_code": "ST",
         "alpha_3_code": "STP",
         "english_name": "Sao Tome and Principe",
         "french_name": "Sao Tom\u00e9-et-Principe",
         "numeric_code": 678
     },
-    {
+    "SUR": {
         "alpha_2_code": "SR",
         "alpha_3_code": "SUR",
         "english_name": "Suriname",
         "french_name": "Suriname (le)",
         "numeric_code": 740
     },
-    {
+    "SVK": {
         "alpha_2_code": "SK",
         "alpha_3_code": "SVK",
         "english_name": "Slovakia",
         "french_name": "Slovaquie (la)",
         "numeric_code": 703
     },
-    {
+    "SVN": {
         "alpha_2_code": "SI",
         "alpha_3_code": "SVN",
         "english_name": "Slovenia",
         "french_name": "Slov\u00e9nie (la)",
         "numeric_code": 705
     },
-    {
+    "SWE": {
         "alpha_2_code": "SE",
         "alpha_3_code": "SWE",
         "english_name": "Sweden",
         "french_name": "Su\u00e8de (la)",
         "numeric_code": 752
     },
-    {
+    "SWZ": {
         "alpha_2_code": "SZ",
         "alpha_3_code": "SWZ",
         "english_name": "Eswatini",
         "french_name": "Eswatini (l')",
         "numeric_code": 748
     },
-    {
+    "SXM": {
         "alpha_2_code": "SX",
         "alpha_3_code": "SXM",
         "english_name": "Sint Maarten (Dutch part)",
         "french_name": "Saint-Martin (partie n\u00e9erlandaise)",
         "numeric_code": 534
     },
-    {
+    "SYC": {
         "alpha_2_code": "SC",
         "alpha_3_code": "SYC",
         "english_name": "Seychelles",
         "french_name": "Seychelles (les)",
         "numeric_code": 690
     },
-    {
+    "SYR": {
         "alpha_2_code": "SY",
         "alpha_3_code": "SYR",
         "english_name": "Syrian Arab Republic (the)",
         "french_name": "R\u00e9publique arabe syrienne (la)",
         "numeric_code": 760
     },
-    {
+    "TCA": {
         "alpha_2_code": "TC",
         "alpha_3_code": "TCA",
         "english_name": "Turks and Caicos Islands (the)",
         "french_name": "Turks-et-Ca\u00efcos (les \u00celes)",
         "numeric_code": 796
     },
-    {
+    "TCD": {
         "alpha_2_code": "TD",
         "alpha_3_code": "TCD",
         "english_name": "Chad",
         "french_name": "Tchad (le)",
         "numeric_code": 148
     },
-    {
+    "TGO": {
         "alpha_2_code": "TG",
         "alpha_3_code": "TGO",
         "english_name": "Togo",
         "french_name": "Togo (le)",
         "numeric_code": 768
     },
-    {
+    "THA": {
         "alpha_2_code": "TH",
         "alpha_3_code": "THA",
         "english_name": "Thailand",
         "french_name": "Tha\u00eflande (la)",
         "numeric_code": 764
     },
-    {
+    "TJK": {
         "alpha_2_code": "TJ",
         "alpha_3_code": "TJK",
         "english_name": "Tajikistan",
         "french_name": "Tadjikistan (le)",
         "numeric_code": 762
     },
-    {
+    "TKL": {
         "alpha_2_code": "TK",
         "alpha_3_code": "TKL",
         "english_name": "Tokelau",
         "french_name": "Tokelau (les)",
         "numeric_code": 772
     },
-    {
+    "TKM": {
         "alpha_2_code": "TM",
         "alpha_3_code": "TKM",
         "english_name": "Turkmenistan",
         "french_name": "Turkm\u00e9nistan (le)",
         "numeric_code": 795
     },
-    {
+    "TLS": {
         "alpha_2_code": "TL",
         "alpha_3_code": "TLS",
         "english_name": "Timor-Leste",
         "french_name": "Timor-Leste (le)",
         "numeric_code": 626
     },
-    {
+    "TON": {
         "alpha_2_code": "TO",
         "alpha_3_code": "TON",
         "english_name": "Tonga",
         "french_name": "Tonga (les)",
         "numeric_code": 776
     },
-    {
+    "TTO": {
         "alpha_2_code": "TT",
         "alpha_3_code": "TTO",
         "english_name": "Trinidad and Tobago",
         "french_name": "Trinit\u00e9-et-Tobago (la)",
         "numeric_code": 780
     },
-    {
+    "TUN": {
         "alpha_2_code": "TN",
         "alpha_3_code": "TUN",
         "english_name": "Tunisia",
         "french_name": "Tunisie (la)",
         "numeric_code": 788
     },
-    {
+    "TUR": {
         "alpha_2_code": "TR",
         "alpha_3_code": "TUR",
         "english_name": "T\u00fcrkiye",
         "french_name": "T\u00fcrkiye (la)",
         "numeric_code": 792
     },
-    {
+    "TUV": {
         "alpha_2_code": "TV",
         "alpha_3_code": "TUV",
         "english_name": "Tuvalu",
         "french_name": "Tuvalu (les)",
         "numeric_code": 798
     },
-    {
+    "TWN": {
         "alpha_2_code": "TW",
         "alpha_3_code": "TWN",
         "english_name": "Taiwan (Province of China)",
         "french_name": "Ta\u00efwan (Province de Chine)",
         "numeric_code": 158
     },
-    {
+    "TZA": {
         "alpha_2_code": "TZ",
         "alpha_3_code": "TZA",
         "english_name": "Tanzania, the United Republic of",
         "french_name": "Tanzanie (la R\u00e9publique-Unie de)",
         "numeric_code": 834
     },
-    {
+    "UGA": {
         "alpha_2_code": "UG",
         "alpha_3_code": "UGA",
         "english_name": "Uganda",
         "french_name": "Ouganda (l')",
         "numeric_code": 800
     },
-    {
+    "UKR": {
         "alpha_2_code": "UA",
         "alpha_3_code": "UKR",
         "english_name": "Ukraine",
         "french_name": "Ukraine (l')",
         "numeric_code": 804
     },
-    {
+    "UMI": {
         "alpha_2_code": "UM",
         "alpha_3_code": "UMI",
         "english_name": "United States Minor Outlying Islands (the)",
         "french_name": "\u00celes mineures \u00e9loign\u00e9es des \u00c9tats-Unis (les)",
         "numeric_code": 581
     },
-    {
+    "URY": {
         "alpha_2_code": "UY",
         "alpha_3_code": "URY",
         "english_name": "Uruguay",
         "french_name": "Uruguay (l')",
         "numeric_code": 858
     },
-    {
+    "USA": {
         "alpha_2_code": "US",
         "alpha_3_code": "USA",
         "english_name": "United States of America (the)",
         "french_name": "\u00c9tats-Unis d'Am\u00e9rique (les)",
         "numeric_code": 840
     },
-    {
+    "UZB": {
         "alpha_2_code": "UZ",
         "alpha_3_code": "UZB",
         "english_name": "Uzbekistan",
         "french_name": "Ouzb\u00e9kistan (l')",
         "numeric_code": 860
     },
-    {
+    "VAT": {
         "alpha_2_code": "VA",
         "alpha_3_code": "VAT",
         "english_name": "Holy See (the)",
         "french_name": "Saint-Si\u00e8ge (le)",
         "numeric_code": 336
     },
-    {
+    "VCT": {
         "alpha_2_code": "VC",
         "alpha_3_code": "VCT",
         "english_name": "Saint Vincent and the Grenadines",
         "french_name": "Saint-Vincent-et-les Grenadines",
         "numeric_code": 670
     },
-    {
+    "VEN": {
         "alpha_2_code": "VE",
         "alpha_3_code": "VEN",
         "english_name": "Venezuela (Bolivarian Republic of)",
         "french_name": "Venezuela (R\u00e9publique bolivarienne du)",
         "numeric_code": 862
     },
-    {
+    "VGB": {
         "alpha_2_code": "VG",
         "alpha_3_code": "VGB",
         "english_name": "Virgin Islands (British)",
         "french_name": "Vierges britanniques (les \u00celes)",
         "numeric_code": 92
     },
-    {
+    "VIR": {
         "alpha_2_code": "VI",
         "alpha_3_code": "VIR",
         "english_name": "Virgin Islands (U.S.)",
         "french_name": "Vierges des \u00c9tats-Unis (les \u00celes)",
         "numeric_code": 850
     },
-    {
+    "VNM": {
         "alpha_2_code": "VN",
         "alpha_3_code": "VNM",
         "english_name": "Viet Nam",
         "french_name": "Viet Nam (le)",
         "numeric_code": 704
     },
-    {
+    "VUT": {
         "alpha_2_code": "VU",
         "alpha_3_code": "VUT",
         "english_name": "Vanuatu",
         "french_name": "Vanuatu (le)",
         "numeric_code": 548
     },
-    {
+    "WLF": {
         "alpha_2_code": "WF",
         "alpha_3_code": "WLF",
         "english_name": "Wallis and Futuna",
         "french_name": "Wallis-et-Futuna",
         "numeric_code": 876
     },
-    {
+    "WSM": {
         "alpha_2_code": "WS",
         "alpha_3_code": "WSM",
         "english_name": "Samoa",
         "french_name": "Samoa (le)",
         "numeric_code": 882
     },
-    {
+    "YEM": {
         "alpha_2_code": "YE",
         "alpha_3_code": "YEM",
         "english_name": "Yemen",
         "french_name": "Y\u00e9men (le)",
         "numeric_code": 887
     },
-    {
+    "ZAF": {
         "alpha_2_code": "ZA",
         "alpha_3_code": "ZAF",
         "english_name": "South Africa",
         "french_name": "Afrique du Sud (l')",
         "numeric_code": 710
     },
-    {
+    "ZMB": {
         "alpha_2_code": "ZM",
         "alpha_3_code": "ZMB",
         "english_name": "Zambia",
         "french_name": "Zambie (la)",
         "numeric_code": 894
     },
-    {
+    "ZWE": {
         "alpha_2_code": "ZW",
         "alpha_3_code": "ZWE",
         "english_name": "Zimbabwe",
         "french_name": "Zimbabwe (le)",
         "numeric_code": 716
     }
-]
+}
```

### Comparing `teritorio-2023.2.1/src/teritorio/_data/currency.json` & `teritorio-2023.4.28/src/teritorio/_data/currency.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('AED', OrderedDict([('code', 'AED'), ('entities', ['UNITED ARAB "*

 * *            "EMIRATES (THE)']), ('minor_units', 2), ('name', 'UAE Dirham'), ('numeric_code', "*

 * *            "784)])), ('AFN', OrderedDict([('code', 'AFN'), ('entities', ['AFGHANISTAN']), "*

 * *            "('minor_units', 2), ('name', 'Afghani'), ('numeric_code', 971)])), ('ALL', "*

 * *            "OrderedDict([('code', 'ALL'), ('entities', ['ALBANIA']), ('minor_units', 2), ('name', "*

 * *            "'Lek'), ('numeric_code', 8) […]*

```diff
@@ -1,73 +1,73 @@
-[
-    {
+{
+    "AED": {
         "code": "AED",
         "entities": [
             "UNITED ARAB EMIRATES (THE)"
         ],
         "minor_units": 2,
         "name": "UAE Dirham",
         "numeric_code": 784
     },
-    {
+    "AFN": {
         "code": "AFN",
         "entities": [
             "AFGHANISTAN"
         ],
         "minor_units": 2,
         "name": "Afghani",
         "numeric_code": 971
     },
-    {
+    "ALL": {
         "code": "ALL",
         "entities": [
             "ALBANIA"
         ],
         "minor_units": 2,
         "name": "Lek",
         "numeric_code": 8
     },
-    {
+    "AMD": {
         "code": "AMD",
         "entities": [
             "ARMENIA"
         ],
         "minor_units": 2,
         "name": "Armenian Dram",
         "numeric_code": 51
     },
-    {
+    "ANG": {
         "code": "ANG",
         "entities": [
             "CURA\u00c7AO",
             "SINT MAARTEN (DUTCH PART)"
         ],
         "minor_units": 2,
         "name": "Netherlands Antillean Guilder",
         "numeric_code": 532
     },
-    {
+    "AOA": {
         "code": "AOA",
         "entities": [
             "ANGOLA"
         ],
         "minor_units": 2,
         "name": "Kwanza",
         "numeric_code": 973
     },
-    {
+    "ARS": {
         "code": "ARS",
         "entities": [
             "ARGENTINA"
         ],
         "minor_units": 2,
         "name": "Argentine Peso",
         "numeric_code": 32
     },
-    {
+    "AUD": {
         "code": "AUD",
         "entities": [
             "AUSTRALIA",
             "CHRISTMAS ISLAND",
             "COCOS (KEELING) ISLANDS (THE)",
             "HEARD ISLAND AND McDONALD ISLANDS",
             "KIRIBATI",
@@ -75,378 +75,378 @@
             "NORFOLK ISLAND",
             "TUVALU"
         ],
         "minor_units": 2,
         "name": "Australian Dollar",
         "numeric_code": 36
     },
-    {
+    "AWG": {
         "code": "AWG",
         "entities": [
             "ARUBA"
         ],
         "minor_units": 2,
         "name": "Aruban Florin",
         "numeric_code": 533
     },
-    {
+    "AZN": {
         "code": "AZN",
         "entities": [
             "AZERBAIJAN"
         ],
         "minor_units": 2,
         "name": "Azerbaijan Manat",
         "numeric_code": 944
     },
-    {
+    "BAM": {
         "code": "BAM",
         "entities": [
             "BOSNIA AND HERZEGOVINA"
         ],
         "minor_units": 2,
         "name": "Convertible Mark",
         "numeric_code": 977
     },
-    {
+    "BBD": {
         "code": "BBD",
         "entities": [
             "BARBADOS"
         ],
         "minor_units": 2,
         "name": "Barbados Dollar",
         "numeric_code": 52
     },
-    {
+    "BDT": {
         "code": "BDT",
         "entities": [
             "BANGLADESH"
         ],
         "minor_units": 2,
         "name": "Taka",
         "numeric_code": 50
     },
-    {
+    "BGN": {
         "code": "BGN",
         "entities": [
             "BULGARIA"
         ],
         "minor_units": 2,
         "name": "Bulgarian Lev",
         "numeric_code": 975
     },
-    {
+    "BHD": {
         "code": "BHD",
         "entities": [
             "BAHRAIN"
         ],
         "minor_units": 3,
         "name": "Bahraini Dinar",
         "numeric_code": 48
     },
-    {
+    "BIF": {
         "code": "BIF",
         "entities": [
             "BURUNDI"
         ],
         "minor_units": 0,
         "name": "Burundi Franc",
         "numeric_code": 108
     },
-    {
+    "BMD": {
         "code": "BMD",
         "entities": [
             "BERMUDA"
         ],
         "minor_units": 2,
         "name": "Bermudian Dollar",
         "numeric_code": 60
     },
-    {
+    "BND": {
         "code": "BND",
         "entities": [
             "BRUNEI DARUSSALAM"
         ],
         "minor_units": 2,
         "name": "Brunei Dollar",
         "numeric_code": 96
     },
-    {
+    "BOB": {
         "code": "BOB",
         "entities": [
             "BOLIVIA (PLURINATIONAL STATE OF)"
         ],
         "minor_units": 2,
         "name": "Boliviano",
         "numeric_code": 68
     },
-    {
+    "BOV": {
         "code": "BOV",
         "entities": [
             "BOLIVIA (PLURINATIONAL STATE OF)"
         ],
         "minor_units": 2,
         "name": "Mvdol",
         "numeric_code": 984
     },
-    {
+    "BRL": {
         "code": "BRL",
         "entities": [
             "BRAZIL"
         ],
         "minor_units": 2,
         "name": "Brazilian Real",
         "numeric_code": 986
     },
-    {
+    "BSD": {
         "code": "BSD",
         "entities": [
             "BAHAMAS (THE)"
         ],
         "minor_units": 2,
         "name": "Bahamian Dollar",
         "numeric_code": 44
     },
-    {
+    "BTN": {
         "code": "BTN",
         "entities": [
             "BHUTAN"
         ],
         "minor_units": 2,
         "name": "Ngultrum",
         "numeric_code": 64
     },
-    {
+    "BWP": {
         "code": "BWP",
         "entities": [
             "BOTSWANA"
         ],
         "minor_units": 2,
         "name": "Pula",
         "numeric_code": 72
     },
-    {
+    "BYN": {
         "code": "BYN",
         "entities": [
             "BELARUS"
         ],
         "minor_units": 2,
         "name": "Belarusian Ruble",
         "numeric_code": 933
     },
-    {
+    "BZD": {
         "code": "BZD",
         "entities": [
             "BELIZE"
         ],
         "minor_units": 2,
         "name": "Belize Dollar",
         "numeric_code": 84
     },
-    {
+    "CAD": {
         "code": "CAD",
         "entities": [
             "CANADA"
         ],
         "minor_units": 2,
         "name": "Canadian Dollar",
         "numeric_code": 124
     },
-    {
+    "CDF": {
         "code": "CDF",
         "entities": [
             "CONGO (THE DEMOCRATIC REPUBLIC OF THE)"
         ],
         "minor_units": 2,
         "name": "Congolese Franc",
         "numeric_code": 976
     },
-    {
+    "CHE": {
         "code": "CHE",
         "entities": [
             "SWITZERLAND"
         ],
         "minor_units": 2,
         "name": "WIR Euro",
         "numeric_code": 947
     },
-    {
+    "CHF": {
         "code": "CHF",
         "entities": [
             "LIECHTENSTEIN",
             "SWITZERLAND"
         ],
         "minor_units": 2,
         "name": "Swiss Franc",
         "numeric_code": 756
     },
-    {
+    "CHW": {
         "code": "CHW",
         "entities": [
             "SWITZERLAND"
         ],
         "minor_units": 2,
         "name": "WIR Franc",
         "numeric_code": 948
     },
-    {
+    "CLF": {
         "code": "CLF",
         "entities": [
             "CHILE"
         ],
         "minor_units": 4,
         "name": "Unidad de Fomento",
         "numeric_code": 990
     },
-    {
+    "CLP": {
         "code": "CLP",
         "entities": [
             "CHILE"
         ],
         "minor_units": 0,
         "name": "Chilean Peso",
         "numeric_code": 152
     },
-    {
+    "CNY": {
         "code": "CNY",
         "entities": [
             "CHINA"
         ],
         "minor_units": 2,
         "name": "Yuan Renminbi",
         "numeric_code": 156
     },
-    {
+    "COP": {
         "code": "COP",
         "entities": [
             "COLOMBIA"
         ],
         "minor_units": 2,
         "name": "Colombian Peso",
         "numeric_code": 170
     },
-    {
+    "COU": {
         "code": "COU",
         "entities": [
             "COLOMBIA"
         ],
         "minor_units": 2,
         "name": "Unidad de Valor Real",
         "numeric_code": 970
     },
-    {
+    "CRC": {
         "code": "CRC",
         "entities": [
             "COSTA RICA"
         ],
         "minor_units": 2,
         "name": "Costa Rican Colon",
         "numeric_code": 188
     },
-    {
+    "CUC": {
         "code": "CUC",
         "entities": [
             "CUBA"
         ],
         "minor_units": 2,
         "name": "Peso Convertible",
         "numeric_code": 931
     },
-    {
+    "CUP": {
         "code": "CUP",
         "entities": [
             "CUBA"
         ],
         "minor_units": 2,
         "name": "Cuban Peso",
         "numeric_code": 192
     },
-    {
+    "CVE": {
         "code": "CVE",
         "entities": [
             "CABO VERDE"
         ],
         "minor_units": 2,
         "name": "Cabo Verde Escudo",
         "numeric_code": 132
     },
-    {
+    "CZK": {
         "code": "CZK",
         "entities": [
             "CZECHIA"
         ],
         "minor_units": 2,
         "name": "Czech Koruna",
         "numeric_code": 203
     },
-    {
+    "DJF": {
         "code": "DJF",
         "entities": [
             "DJIBOUTI"
         ],
         "minor_units": 0,
         "name": "Djibouti Franc",
         "numeric_code": 262
     },
-    {
+    "DKK": {
         "code": "DKK",
         "entities": [
             "DENMARK",
             "FAROE ISLANDS (THE)",
             "GREENLAND"
         ],
         "minor_units": 2,
         "name": "Danish Krone",
         "numeric_code": 208
     },
-    {
+    "DOP": {
         "code": "DOP",
         "entities": [
             "DOMINICAN REPUBLIC (THE)"
         ],
         "minor_units": 2,
         "name": "Dominican Peso",
         "numeric_code": 214
     },
-    {
+    "DZD": {
         "code": "DZD",
         "entities": [
             "ALGERIA"
         ],
         "minor_units": 2,
         "name": "Algerian Dinar",
         "numeric_code": 12
     },
-    {
+    "EGP": {
         "code": "EGP",
         "entities": [
             "EGYPT"
         ],
         "minor_units": 2,
         "name": "Egyptian Pound",
         "numeric_code": 818
     },
-    {
+    "ERN": {
         "code": "ERN",
         "entities": [
             "ERITREA"
         ],
         "minor_units": 2,
         "name": "Nakfa",
         "numeric_code": 232
     },
-    {
+    "ETB": {
         "code": "ETB",
         "entities": [
             "ETHIOPIA"
         ],
         "minor_units": 2,
         "name": "Ethiopian Birr",
         "numeric_code": 230
     },
-    {
+    "EUR": {
         "code": "EUR",
         "entities": [
             "ANDORRA",
             "AUSTRIA",
             "BELGIUM",
             "CROATIA",
             "CYPRUS",
@@ -482,917 +482,917 @@
             "SPAIN",
             "\u00c5LAND ISLANDS"
         ],
         "minor_units": 2,
         "name": "Euro",
         "numeric_code": 978
     },
-    {
+    "FJD": {
         "code": "FJD",
         "entities": [
             "FIJI"
         ],
         "minor_units": 2,
         "name": "Fiji Dollar",
         "numeric_code": 242
     },
-    {
+    "FKP": {
         "code": "FKP",
         "entities": [
             "FALKLAND ISLANDS (THE) [MALVINAS]"
         ],
         "minor_units": 2,
         "name": "Falkland Islands Pound",
         "numeric_code": 238
     },
-    {
+    "GBP": {
         "code": "GBP",
         "entities": [
             "GUERNSEY",
             "ISLE OF MAN",
             "JERSEY",
             "UNITED KINGDOM OF GREAT BRITAIN AND NORTHERN IRELAND (THE)"
         ],
         "minor_units": 2,
         "name": "Pound Sterling",
         "numeric_code": 826
     },
-    {
+    "GEL": {
         "code": "GEL",
         "entities": [
             "GEORGIA"
         ],
         "minor_units": 2,
         "name": "Lari",
         "numeric_code": 981
     },
-    {
+    "GHS": {
         "code": "GHS",
         "entities": [
             "GHANA"
         ],
         "minor_units": 2,
         "name": "Ghana Cedi",
         "numeric_code": 936
     },
-    {
+    "GIP": {
         "code": "GIP",
         "entities": [
             "GIBRALTAR"
         ],
         "minor_units": 2,
         "name": "Gibraltar Pound",
         "numeric_code": 292
     },
-    {
+    "GMD": {
         "code": "GMD",
         "entities": [
             "GAMBIA (THE)"
         ],
         "minor_units": 2,
         "name": "Dalasi",
         "numeric_code": 270
     },
-    {
+    "GNF": {
         "code": "GNF",
         "entities": [
             "GUINEA"
         ],
         "minor_units": 0,
         "name": "Guinean Franc",
         "numeric_code": 324
     },
-    {
+    "GTQ": {
         "code": "GTQ",
         "entities": [
             "GUATEMALA"
         ],
         "minor_units": 2,
         "name": "Quetzal",
         "numeric_code": 320
     },
-    {
+    "GYD": {
         "code": "GYD",
         "entities": [
             "GUYANA"
         ],
         "minor_units": 2,
         "name": "Guyana Dollar",
         "numeric_code": 328
     },
-    {
+    "HKD": {
         "code": "HKD",
         "entities": [
             "HONG KONG"
         ],
         "minor_units": 2,
         "name": "Hong Kong Dollar",
         "numeric_code": 344
     },
-    {
+    "HNL": {
         "code": "HNL",
         "entities": [
             "HONDURAS"
         ],
         "minor_units": 2,
         "name": "Lempira",
         "numeric_code": 340
     },
-    {
+    "HTG": {
         "code": "HTG",
         "entities": [
             "HAITI"
         ],
         "minor_units": 2,
         "name": "Gourde",
         "numeric_code": 332
     },
-    {
+    "HUF": {
         "code": "HUF",
         "entities": [
             "HUNGARY"
         ],
         "minor_units": 2,
         "name": "Forint",
         "numeric_code": 348
     },
-    {
+    "IDR": {
         "code": "IDR",
         "entities": [
             "INDONESIA"
         ],
         "minor_units": 2,
         "name": "Rupiah",
         "numeric_code": 360
     },
-    {
+    "ILS": {
         "code": "ILS",
         "entities": [
             "ISRAEL"
         ],
         "minor_units": 2,
         "name": "New Israeli Sheqel",
         "numeric_code": 376
     },
-    {
+    "INR": {
         "code": "INR",
         "entities": [
             "BHUTAN",
             "INDIA"
         ],
         "minor_units": 2,
         "name": "Indian Rupee",
         "numeric_code": 356
     },
-    {
+    "IQD": {
         "code": "IQD",
         "entities": [
             "IRAQ"
         ],
         "minor_units": 3,
         "name": "Iraqi Dinar",
         "numeric_code": 368
     },
-    {
+    "IRR": {
         "code": "IRR",
         "entities": [
             "IRAN (ISLAMIC REPUBLIC OF)"
         ],
         "minor_units": 2,
         "name": "Iranian Rial",
         "numeric_code": 364
     },
-    {
+    "ISK": {
         "code": "ISK",
         "entities": [
             "ICELAND"
         ],
         "minor_units": 0,
         "name": "Iceland Krona",
         "numeric_code": 352
     },
-    {
+    "JMD": {
         "code": "JMD",
         "entities": [
             "JAMAICA"
         ],
         "minor_units": 2,
         "name": "Jamaican Dollar",
         "numeric_code": 388
     },
-    {
+    "JOD": {
         "code": "JOD",
         "entities": [
             "JORDAN"
         ],
         "minor_units": 3,
         "name": "Jordanian Dinar",
         "numeric_code": 400
     },
-    {
+    "JPY": {
         "code": "JPY",
         "entities": [
             "JAPAN"
         ],
         "minor_units": 0,
         "name": "Yen",
         "numeric_code": 392
     },
-    {
+    "KES": {
         "code": "KES",
         "entities": [
             "KENYA"
         ],
         "minor_units": 2,
         "name": "Kenyan Shilling",
         "numeric_code": 404
     },
-    {
+    "KGS": {
         "code": "KGS",
         "entities": [
             "KYRGYZSTAN"
         ],
         "minor_units": 2,
         "name": "Som",
         "numeric_code": 417
     },
-    {
+    "KHR": {
         "code": "KHR",
         "entities": [
             "CAMBODIA"
         ],
         "minor_units": 2,
         "name": "Riel",
         "numeric_code": 116
     },
-    {
+    "KMF": {
         "code": "KMF",
         "entities": [
             "COMOROS (THE)"
         ],
         "minor_units": 0,
         "name": "Comorian Franc",
         "numeric_code": 174
     },
-    {
+    "KPW": {
         "code": "KPW",
         "entities": [
             "KOREA (THE DEMOCRATIC PEOPLE\u2019S REPUBLIC OF)"
         ],
         "minor_units": 2,
         "name": "North Korean Won",
         "numeric_code": 408
     },
-    {
+    "KRW": {
         "code": "KRW",
         "entities": [
             "KOREA (THE REPUBLIC OF)"
         ],
         "minor_units": 0,
         "name": "Won",
         "numeric_code": 410
     },
-    {
+    "KWD": {
         "code": "KWD",
         "entities": [
             "KUWAIT"
         ],
         "minor_units": 3,
         "name": "Kuwaiti Dinar",
         "numeric_code": 414
     },
-    {
+    "KYD": {
         "code": "KYD",
         "entities": [
             "CAYMAN ISLANDS (THE)"
         ],
         "minor_units": 2,
         "name": "Cayman Islands Dollar",
         "numeric_code": 136
     },
-    {
+    "KZT": {
         "code": "KZT",
         "entities": [
             "KAZAKHSTAN"
         ],
         "minor_units": 2,
         "name": "Tenge",
         "numeric_code": 398
     },
-    {
+    "LAK": {
         "code": "LAK",
         "entities": [
             "LAO PEOPLE\u2019S DEMOCRATIC REPUBLIC (THE)"
         ],
         "minor_units": 2,
         "name": "Lao Kip",
         "numeric_code": 418
     },
-    {
+    "LBP": {
         "code": "LBP",
         "entities": [
             "LEBANON"
         ],
         "minor_units": 2,
         "name": "Lebanese Pound",
         "numeric_code": 422
     },
-    {
+    "LKR": {
         "code": "LKR",
         "entities": [
             "SRI LANKA"
         ],
         "minor_units": 2,
         "name": "Sri Lanka Rupee",
         "numeric_code": 144
     },
-    {
+    "LRD": {
         "code": "LRD",
         "entities": [
             "LIBERIA"
         ],
         "minor_units": 2,
         "name": "Liberian Dollar",
         "numeric_code": 430
     },
-    {
+    "LSL": {
         "code": "LSL",
         "entities": [
             "LESOTHO"
         ],
         "minor_units": 2,
         "name": "Loti",
         "numeric_code": 426
     },
-    {
+    "LYD": {
         "code": "LYD",
         "entities": [
             "LIBYA"
         ],
         "minor_units": 3,
         "name": "Libyan Dinar",
         "numeric_code": 434
     },
-    {
+    "MAD": {
         "code": "MAD",
         "entities": [
             "MOROCCO",
             "WESTERN SAHARA"
         ],
         "minor_units": 2,
         "name": "Moroccan Dirham",
         "numeric_code": 504
     },
-    {
+    "MDL": {
         "code": "MDL",
         "entities": [
             "MOLDOVA (THE REPUBLIC OF)"
         ],
         "minor_units": 2,
         "name": "Moldovan Leu",
         "numeric_code": 498
     },
-    {
+    "MGA": {
         "code": "MGA",
         "entities": [
             "MADAGASCAR"
         ],
         "minor_units": 2,
         "name": "Malagasy Ariary",
         "numeric_code": 969
     },
-    {
+    "MKD": {
         "code": "MKD",
         "entities": [
             "NORTH MACEDONIA"
         ],
         "minor_units": 2,
         "name": "Denar",
         "numeric_code": 807
     },
-    {
+    "MMK": {
         "code": "MMK",
         "entities": [
             "MYANMAR"
         ],
         "minor_units": 2,
         "name": "Kyat",
         "numeric_code": 104
     },
-    {
+    "MNT": {
         "code": "MNT",
         "entities": [
             "MONGOLIA"
         ],
         "minor_units": 2,
         "name": "Tugrik",
         "numeric_code": 496
     },
-    {
+    "MOP": {
         "code": "MOP",
         "entities": [
             "MACAO"
         ],
         "minor_units": 2,
         "name": "Pataca",
         "numeric_code": 446
     },
-    {
+    "MRU": {
         "code": "MRU",
         "entities": [
             "MAURITANIA"
         ],
         "minor_units": 2,
         "name": "Ouguiya",
         "numeric_code": 929
     },
-    {
+    "MUR": {
         "code": "MUR",
         "entities": [
             "MAURITIUS"
         ],
         "minor_units": 2,
         "name": "Mauritius Rupee",
         "numeric_code": 480
     },
-    {
+    "MVR": {
         "code": "MVR",
         "entities": [
             "MALDIVES"
         ],
         "minor_units": 2,
         "name": "Rufiyaa",
         "numeric_code": 462
     },
-    {
+    "MWK": {
         "code": "MWK",
         "entities": [
             "MALAWI"
         ],
         "minor_units": 2,
         "name": "Malawi Kwacha",
         "numeric_code": 454
     },
-    {
+    "MXN": {
         "code": "MXN",
         "entities": [
             "MEXICO"
         ],
         "minor_units": 2,
         "name": "Mexican Peso",
         "numeric_code": 484
     },
-    {
+    "MXV": {
         "code": "MXV",
         "entities": [
             "MEXICO"
         ],
         "minor_units": 2,
         "name": "Mexican Unidad de Inversion (UDI)",
         "numeric_code": 979
     },
-    {
+    "MYR": {
         "code": "MYR",
         "entities": [
             "MALAYSIA"
         ],
         "minor_units": 2,
         "name": "Malaysian Ringgit",
         "numeric_code": 458
     },
-    {
+    "MZN": {
         "code": "MZN",
         "entities": [
             "MOZAMBIQUE"
         ],
         "minor_units": 2,
         "name": "Mozambique Metical",
         "numeric_code": 943
     },
-    {
+    "NAD": {
         "code": "NAD",
         "entities": [
             "NAMIBIA"
         ],
         "minor_units": 2,
         "name": "Namibia Dollar",
         "numeric_code": 516
     },
-    {
+    "NGN": {
         "code": "NGN",
         "entities": [
             "NIGERIA"
         ],
         "minor_units": 2,
         "name": "Naira",
         "numeric_code": 566
     },
-    {
+    "NIO": {
         "code": "NIO",
         "entities": [
             "NICARAGUA"
         ],
         "minor_units": 2,
         "name": "Cordoba Oro",
         "numeric_code": 558
     },
-    {
+    "NOK": {
         "code": "NOK",
         "entities": [
             "BOUVET ISLAND",
             "NORWAY",
             "SVALBARD AND JAN MAYEN"
         ],
         "minor_units": 2,
         "name": "Norwegian Krone",
         "numeric_code": 578
     },
-    {
+    "NPR": {
         "code": "NPR",
         "entities": [
             "NEPAL"
         ],
         "minor_units": 2,
         "name": "Nepalese Rupee",
         "numeric_code": 524
     },
-    {
+    "NZD": {
         "code": "NZD",
         "entities": [
             "COOK ISLANDS (THE)",
             "NEW ZEALAND",
             "NIUE",
             "PITCAIRN",
             "TOKELAU"
         ],
         "minor_units": 2,
         "name": "New Zealand Dollar",
         "numeric_code": 554
     },
-    {
+    "OMR": {
         "code": "OMR",
         "entities": [
             "OMAN"
         ],
         "minor_units": 3,
         "name": "Rial Omani",
         "numeric_code": 512
     },
-    {
+    "PAB": {
         "code": "PAB",
         "entities": [
             "PANAMA"
         ],
         "minor_units": 2,
         "name": "Balboa",
         "numeric_code": 590
     },
-    {
+    "PEN": {
         "code": "PEN",
         "entities": [
             "PERU"
         ],
         "minor_units": 2,
         "name": "Sol",
         "numeric_code": 604
     },
-    {
+    "PGK": {
         "code": "PGK",
         "entities": [
             "PAPUA NEW GUINEA"
         ],
         "minor_units": 2,
         "name": "Kina",
         "numeric_code": 598
     },
-    {
+    "PHP": {
         "code": "PHP",
         "entities": [
             "PHILIPPINES (THE)"
         ],
         "minor_units": 2,
         "name": "Philippine Peso",
         "numeric_code": 608
     },
-    {
+    "PKR": {
         "code": "PKR",
         "entities": [
             "PAKISTAN"
         ],
         "minor_units": 2,
         "name": "Pakistan Rupee",
         "numeric_code": 586
     },
-    {
+    "PLN": {
         "code": "PLN",
         "entities": [
             "POLAND"
         ],
         "minor_units": 2,
         "name": "Zloty",
         "numeric_code": 985
     },
-    {
+    "PYG": {
         "code": "PYG",
         "entities": [
             "PARAGUAY"
         ],
         "minor_units": 0,
         "name": "Guarani",
         "numeric_code": 600
     },
-    {
+    "QAR": {
         "code": "QAR",
         "entities": [
             "QATAR"
         ],
         "minor_units": 2,
         "name": "Qatari Rial",
         "numeric_code": 634
     },
-    {
+    "RON": {
         "code": "RON",
         "entities": [
             "ROMANIA"
         ],
         "minor_units": 2,
         "name": "Romanian Leu",
         "numeric_code": 946
     },
-    {
+    "RSD": {
         "code": "RSD",
         "entities": [
             "SERBIA"
         ],
         "minor_units": 2,
         "name": "Serbian Dinar",
         "numeric_code": 941
     },
-    {
+    "RUB": {
         "code": "RUB",
         "entities": [
             "RUSSIAN FEDERATION (THE)"
         ],
         "minor_units": 2,
         "name": "Russian Ruble",
         "numeric_code": 643
     },
-    {
+    "RWF": {
         "code": "RWF",
         "entities": [
             "RWANDA"
         ],
         "minor_units": 0,
         "name": "Rwanda Franc",
         "numeric_code": 646
     },
-    {
+    "SAR": {
         "code": "SAR",
         "entities": [
             "SAUDI ARABIA"
         ],
         "minor_units": 2,
         "name": "Saudi Riyal",
         "numeric_code": 682
     },
-    {
+    "SBD": {
         "code": "SBD",
         "entities": [
             "SOLOMON ISLANDS"
         ],
         "minor_units": 2,
         "name": "Solomon Islands Dollar",
         "numeric_code": 90
     },
-    {
+    "SCR": {
         "code": "SCR",
         "entities": [
             "SEYCHELLES"
         ],
         "minor_units": 2,
         "name": "Seychelles Rupee",
         "numeric_code": 690
     },
-    {
+    "SDG": {
         "code": "SDG",
         "entities": [
             "SUDAN (THE)"
         ],
         "minor_units": 2,
         "name": "Sudanese Pound",
         "numeric_code": 938
     },
-    {
+    "SEK": {
         "code": "SEK",
         "entities": [
             "SWEDEN"
         ],
         "minor_units": 2,
         "name": "Swedish Krona",
         "numeric_code": 752
     },
-    {
+    "SGD": {
         "code": "SGD",
         "entities": [
             "SINGAPORE"
         ],
         "minor_units": 2,
         "name": "Singapore Dollar",
         "numeric_code": 702
     },
-    {
+    "SHP": {
         "code": "SHP",
         "entities": [
             "SAINT HELENA, ASCENSION AND TRISTAN DA CUNHA"
         ],
         "minor_units": 2,
         "name": "Saint Helena Pound",
         "numeric_code": 654
     },
-    {
+    "SLE": {
         "code": "SLE",
         "entities": [
             "SIERRA LEONE"
         ],
         "minor_units": 2,
         "name": "Leone",
         "numeric_code": 925
     },
-    {
+    "SLL": {
         "code": "SLL",
         "entities": [
             "SIERRA LEONE"
         ],
         "minor_units": 2,
         "name": "Leone",
         "numeric_code": 694
     },
-    {
+    "SOS": {
         "code": "SOS",
         "entities": [
             "SOMALIA"
         ],
         "minor_units": 2,
         "name": "Somali Shilling",
         "numeric_code": 706
     },
-    {
+    "SRD": {
         "code": "SRD",
         "entities": [
             "SURINAME"
         ],
         "minor_units": 2,
         "name": "Surinam Dollar",
         "numeric_code": 968
     },
-    {
+    "SSP": {
         "code": "SSP",
         "entities": [
             "SOUTH SUDAN"
         ],
         "minor_units": 2,
         "name": "South Sudanese Pound",
         "numeric_code": 728
     },
-    {
+    "STN": {
         "code": "STN",
         "entities": [
             "SAO TOME AND PRINCIPE"
         ],
         "minor_units": 2,
         "name": "Dobra",
         "numeric_code": 930
     },
-    {
+    "SVC": {
         "code": "SVC",
         "entities": [
             "EL SALVADOR"
         ],
         "minor_units": 2,
         "name": "El Salvador Colon",
         "numeric_code": 222
     },
-    {
+    "SYP": {
         "code": "SYP",
         "entities": [
             "SYRIAN ARAB REPUBLIC"
         ],
         "minor_units": 2,
         "name": "Syrian Pound",
         "numeric_code": 760
     },
-    {
+    "SZL": {
         "code": "SZL",
         "entities": [
             "ESWATINI"
         ],
         "minor_units": 2,
         "name": "Lilangeni",
         "numeric_code": 748
     },
-    {
+    "THB": {
         "code": "THB",
         "entities": [
             "THAILAND"
         ],
         "minor_units": 2,
         "name": "Baht",
         "numeric_code": 764
     },
-    {
+    "TJS": {
         "code": "TJS",
         "entities": [
             "TAJIKISTAN"
         ],
         "minor_units": 2,
         "name": "Somoni",
         "numeric_code": 972
     },
-    {
+    "TMT": {
         "code": "TMT",
         "entities": [
             "TURKMENISTAN"
         ],
         "minor_units": 2,
         "name": "Turkmenistan New Manat",
         "numeric_code": 934
     },
-    {
+    "TND": {
         "code": "TND",
         "entities": [
             "TUNISIA"
         ],
         "minor_units": 3,
         "name": "Tunisian Dinar",
         "numeric_code": 788
     },
-    {
+    "TOP": {
         "code": "TOP",
         "entities": [
             "TONGA"
         ],
         "minor_units": 2,
         "name": "Pa\u2019anga",
         "numeric_code": 776
     },
-    {
+    "TRY": {
         "code": "TRY",
         "entities": [
             "T\u00dcRK\u0130YE"
         ],
         "minor_units": 2,
         "name": "Turkish Lira",
         "numeric_code": 949
     },
-    {
+    "TTD": {
         "code": "TTD",
         "entities": [
             "TRINIDAD AND TOBAGO"
         ],
         "minor_units": 2,
         "name": "Trinidad and Tobago Dollar",
         "numeric_code": 780
     },
-    {
+    "TWD": {
         "code": "TWD",
         "entities": [
             "TAIWAN (PROVINCE OF CHINA)"
         ],
         "minor_units": 2,
         "name": "New Taiwan Dollar",
         "numeric_code": 901
     },
-    {
+    "TZS": {
         "code": "TZS",
         "entities": [
             "TANZANIA, UNITED REPUBLIC OF"
         ],
         "minor_units": 2,
         "name": "Tanzanian Shilling",
         "numeric_code": 834
     },
-    {
+    "UAH": {
         "code": "UAH",
         "entities": [
             "UKRAINE"
         ],
         "minor_units": 2,
         "name": "Hryvnia",
         "numeric_code": 980
     },
-    {
+    "UGX": {
         "code": "UGX",
         "entities": [
             "UGANDA"
         ],
         "minor_units": 0,
         "name": "Uganda Shilling",
         "numeric_code": 800
     },
-    {
+    "USD": {
         "code": "USD",
         "entities": [
             "AMERICAN SAMOA",
             "BONAIRE, SINT EUSTATIUS AND SABA",
             "BRITISH INDIAN OCEAN TERRITORY (THE)",
             "ECUADOR",
             "EL SALVADOR",
@@ -1411,173 +1411,173 @@
             "VIRGIN ISLANDS (BRITISH)",
             "VIRGIN ISLANDS (U.S.)"
         ],
         "minor_units": 2,
         "name": "US Dollar",
         "numeric_code": 840
     },
-    {
+    "USN": {
         "code": "USN",
         "entities": [
             "UNITED STATES OF AMERICA (THE)"
         ],
         "minor_units": 2,
         "name": "US Dollar (Next day)",
         "numeric_code": 997
     },
-    {
+    "UYI": {
         "code": "UYI",
         "entities": [
             "URUGUAY"
         ],
         "minor_units": 0,
         "name": "Uruguay Peso en Unidades Indexadas (UI)",
         "numeric_code": 940
     },
-    {
+    "UYU": {
         "code": "UYU",
         "entities": [
             "URUGUAY"
         ],
         "minor_units": 2,
         "name": "Peso Uruguayo",
         "numeric_code": 858
     },
-    {
+    "UYW": {
         "code": "UYW",
         "entities": [
             "URUGUAY"
         ],
         "minor_units": 4,
         "name": "Unidad Previsional",
         "numeric_code": 927
     },
-    {
+    "UZS": {
         "code": "UZS",
         "entities": [
             "UZBEKISTAN"
         ],
         "minor_units": 2,
         "name": "Uzbekistan Sum",
         "numeric_code": 860
     },
-    {
+    "VED": {
         "code": "VED",
         "entities": [
             "VENEZUELA (BOLIVARIAN REPUBLIC OF)"
         ],
         "minor_units": 2,
         "name": "Bol\u00edvar Soberano",
         "numeric_code": 926
     },
-    {
+    "VES": {
         "code": "VES",
         "entities": [
             "VENEZUELA (BOLIVARIAN REPUBLIC OF)"
         ],
         "minor_units": 2,
         "name": "Bol\u00edvar Soberano",
         "numeric_code": 928
     },
-    {
+    "VND": {
         "code": "VND",
         "entities": [
             "VIET NAM"
         ],
         "minor_units": 0,
         "name": "Dong",
         "numeric_code": 704
     },
-    {
+    "VUV": {
         "code": "VUV",
         "entities": [
             "VANUATU"
         ],
         "minor_units": 0,
         "name": "Vatu",
         "numeric_code": 548
     },
-    {
+    "WST": {
         "code": "WST",
         "entities": [
             "SAMOA"
         ],
         "minor_units": 2,
         "name": "Tala",
         "numeric_code": 882
     },
-    {
+    "XAF": {
         "code": "XAF",
         "entities": [
             "CAMEROON",
             "CENTRAL AFRICAN REPUBLIC (THE)",
             "CHAD",
             "CONGO (THE)",
             "EQUATORIAL GUINEA",
             "GABON"
         ],
         "minor_units": 0,
         "name": "CFA Franc BEAC",
         "numeric_code": 950
     },
-    {
+    "XAG": {
         "code": "XAG",
         "entities": [
             "ZZ11_Silver"
         ],
         "minor_units": null,
         "name": "Silver",
         "numeric_code": 961
     },
-    {
+    "XAU": {
         "code": "XAU",
         "entities": [
             "ZZ08_Gold"
         ],
         "minor_units": null,
         "name": "Gold",
         "numeric_code": 959
     },
-    {
+    "XBA": {
         "code": "XBA",
         "entities": [
             "ZZ01_Bond Markets Unit European_EURCO"
         ],
         "minor_units": null,
         "name": "Bond Markets Unit European Composite Unit (EURCO)",
         "numeric_code": 955
     },
-    {
+    "XBB": {
         "code": "XBB",
         "entities": [
             "ZZ02_Bond Markets Unit European_EMU-6"
         ],
         "minor_units": null,
         "name": "Bond Markets Unit European Monetary Unit (E.M.U.-6)",
         "numeric_code": 956
     },
-    {
+    "XBC": {
         "code": "XBC",
         "entities": [
             "ZZ03_Bond Markets Unit European_EUA-9"
         ],
         "minor_units": null,
         "name": "Bond Markets Unit European Unit of Account 9 (E.U.A.-9)",
         "numeric_code": 957
     },
-    {
+    "XBD": {
         "code": "XBD",
         "entities": [
             "ZZ04_Bond Markets Unit European_EUA-17"
         ],
         "minor_units": null,
         "name": "Bond Markets Unit European Unit of Account 17 (E.U.A.-17)",
         "numeric_code": 958
     },
-    {
+    "XCD": {
         "code": "XCD",
         "entities": [
             "ANGUILLA",
             "ANTIGUA AND BARBUDA",
             "DOMINICA",
             "GRENADA",
             "MONTSERRAT",
@@ -1585,24 +1585,24 @@
             "SAINT LUCIA",
             "SAINT VINCENT AND THE GRENADINES"
         ],
         "minor_units": 2,
         "name": "East Caribbean Dollar",
         "numeric_code": 951
     },
-    {
+    "XDR": {
         "code": "XDR",
         "entities": [
             "INTERNATIONAL MONETARY FUND (IMF)"
         ],
         "minor_units": null,
         "name": "SDR (Special Drawing Right)",
         "numeric_code": 960
     },
-    {
+    "XOF": {
         "code": "XOF",
         "entities": [
             "BENIN",
             "BURKINA FASO",
             "C\u00d4TE D'IVOIRE",
             "GUINEA-BISSAU",
             "MALI",
@@ -1610,111 +1610,111 @@
             "SENEGAL",
             "TOGO"
         ],
         "minor_units": 0,
         "name": "CFA Franc BCEAO",
         "numeric_code": 952
     },
-    {
+    "XPD": {
         "code": "XPD",
         "entities": [
             "ZZ09_Palladium"
         ],
         "minor_units": null,
         "name": "Palladium",
         "numeric_code": 964
     },
-    {
+    "XPF": {
         "code": "XPF",
         "entities": [
             "FRENCH POLYNESIA",
             "NEW CALEDONIA",
             "WALLIS AND FUTUNA"
         ],
         "minor_units": 0,
         "name": "CFP Franc",
         "numeric_code": 953
     },
-    {
+    "XPT": {
         "code": "XPT",
         "entities": [
             "ZZ10_Platinum"
         ],
         "minor_units": null,
         "name": "Platinum",
         "numeric_code": 962
     },
-    {
+    "XSU": {
         "code": "XSU",
         "entities": [
             "SISTEMA UNITARIO DE COMPENSACION REGIONAL DE PAGOS \"SUCRE\""
         ],
         "minor_units": null,
         "name": "Sucre",
         "numeric_code": 994
     },
-    {
+    "XTS": {
         "code": "XTS",
         "entities": [
             "ZZ06_Testing_Code"
         ],
         "minor_units": null,
         "name": "Codes specifically reserved for testing purposes",
         "numeric_code": 963
     },
-    {
+    "XUA": {
         "code": "XUA",
         "entities": [
             "MEMBER COUNTRIES OF THE AFRICAN DEVELOPMENT BANK GROUP"
         ],
         "minor_units": null,
         "name": "ADB Unit of Account",
         "numeric_code": 965
     },
-    {
+    "XXX": {
         "code": "XXX",
         "entities": [
             "ZZ07_No_Currency"
         ],
         "minor_units": null,
         "name": "The codes assigned for transactions where no currency is involved",
         "numeric_code": 999
     },
-    {
+    "YER": {
         "code": "YER",
         "entities": [
             "YEMEN"
         ],
         "minor_units": 2,
         "name": "Yemeni Rial",
         "numeric_code": 886
     },
-    {
+    "ZAR": {
         "code": "ZAR",
         "entities": [
             "LESOTHO",
             "NAMIBIA",
             "SOUTH AFRICA"
         ],
         "minor_units": 2,
         "name": "Rand",
         "numeric_code": 710
     },
-    {
+    "ZMW": {
         "code": "ZMW",
         "entities": [
             "ZAMBIA"
         ],
         "minor_units": 2,
         "name": "Zambian Kwacha",
         "numeric_code": 967
     },
-    {
+    "ZWL": {
         "code": "ZWL",
         "entities": [
             "ZIMBABWE"
         ],
         "minor_units": 2,
         "name": "Zimbabwe Dollar",
         "numeric_code": 932
     }
-]
+}
```

### Comparing `teritorio-2023.2.1/src/teritorio/main.py` & `teritorio-2023.4.28/src/teritorio/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,88 @@
+from __future__ import annotations
+
 import json
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, List, Optional
+from typing import Any, Generic, TypeVar, cast
+
+T = TypeVar("T")
 
 
 class Singleton(type):
-    def __init__(cls, name, bases, dict_):
+    def __init__(cls, name: str, bases: tuple[type, ...], dict_: dict[str, Any]):
         super().__init__(name, bases, dict_)
-        cls.instance = None
+        cls.instance: Singleton | None = None
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(cls) -> Singleton:
         if cls.instance is None:
-            cls.instance = super().__call__(*args, **kwargs)
+            cls.instance = cast(Singleton, super().__call__())
         return cls.instance
 
 
-class DataListIterator:
-    def __init__(self, data):
+class DataListIterator(Generic[T]):
+    def __init__(self, data: dict[str, T]) -> None:
         self.values = (data[key] for key in sorted(data))
 
-    def __iter__(self):
+    def __iter__(self) -> DataListIterator[T]:
         return self
 
-    def __next__(self):
+    def __next__(self) -> T:
         return next(self.values)
 
 
-class DataList:
+class DataList(Generic[T]):
     _data_path: Path
-    _object_class: Any
-    _key: str
+    _object_class: type[T]
 
-    def __init__(self):
-        with open(self._data_path) as file:
+    def __init__(self) -> None:
+        with self._data_path.open() as file:
             data = json.load(file)
 
-        self._data = {}
-        for obj in data:
-            key = obj[self._key]
-            obj = self._object_class(**obj)
+        self._data: dict[str, T] = {}
+        for key, raw_obj in data.items():
+            obj = self._object_class(**raw_obj)
             self._data[key] = obj
             setattr(self, key, obj)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"{self.__class__.__name__}()"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{self.__class__.__name__}()"
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._data)
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> T:
         return self._data[key]
 
-    def __iter__(self):
+    def __iter__(self) -> DataListIterator[T]:
         return DataListIterator(self._data)
 
 
 @dataclass(frozen=True, order=True)
 class Country:
     english_name: str
     french_name: str
     alpha_2_code: str
     alpha_3_code: str
     numeric_code: int
 
 
-class Countries(DataList, metaclass=Singleton):
+class Countries(DataList[Country], metaclass=Singleton):
     _data_path = Path(__file__).parent.joinpath("_data/country.json")
     _object_class = Country
-    _key = "alpha_3_code"
 
 
 @dataclass(frozen=True, order=True)
 class Currency:
     code: str
     name: str
-    entities: List[str]
+    entities: list[str]
     numeric_code: int
-    minor_units: Optional[int]
+    minor_units: int | None
 
 
-class Currencies(DataList, metaclass=Singleton):
+class Currencies(DataList[Currency], metaclass=Singleton):
     _data_path = Path(__file__).parent.joinpath("_data/currency.json")
     _object_class = Currency
-    _key = "code"
```

### Comparing `teritorio-2023.2.1/setup.py` & `teritorio-2023.4.28/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,98 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: teritorio
+Version: 2023.4.28
+Summary: A library for country and currency ISO codes
+Home-page: https://teritorio.readthedocs.io/en/stable/
+License: LGPL-3.0+
+Keywords: iso,currency,country
+Author: Stephanos Kuma
+Author-email: stephanos@kuma.ai
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Documentation, https://teritorio.readthedocs.io/en/stable/
+Project-URL: Repository, https://github.com/spapanik/teritorio
+Description-Content-Type: text/x-rst
+
+=================================================
+teritorio: ISO codes for countries and currencies
+=================================================
+
+.. image:: https://github.com/spapanik/teritorio/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/teritorio/actions/workflows/tests.yml
+.. image:: https://img.shields.io/github/license/spapanik/teritorio
+  :alt: License
+  :target: https://github.com/spapanik/teritorio/blob/main/LICENSE.txt
+.. image:: https://img.shields.io/pypi/v/teritorio
+  :alt: PyPI
+  :target: https://pypi.org/project/teritorio
+.. image:: https://pepy.tech/badge/teritorio
+  :alt: Downloads
+  :target: https://pepy.tech/project/teritorio
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+  :alt: code style: black
+  :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
+
+``teritorio`` two iterable singletons that ``Countries`` and ``Currencies``, that contain all the
+relevant ISO information about countries and currencies, respectively.
+
+In a nutshell
+-------------
+
+Installation
+^^^^^^^^^^^^
+
+The easiest way is to use `poetry`_ to manage your dependencies and add *teritorio* to them.
+It requires Python 3.7.0+ to run.
+
+.. code-block:: toml
+
+    [tool.poetry.dependencies]
+    teritorio = "*"
+
+It is advised to always use the latest release, so that you'll get the latest ISO codes
+
+Usage
+^^^^^
+
+There are two iterable singletons that can be imported from ``teritorio``: ``Countries`` and ``Currencies``.
+
+.. code:: python
+
+    from teritorio import Countries
+    from teritorio import Currencies
+
+Versioning
+----------
+
+The project project adheres to `Calendar Versioning`_.
+The reason is that the data are dominated by political decisions,
+making semantic versioning largely irrelevant.
+
+Links
+-----
+
+- `Documentation`_
+- `Changelog`_
+
+
+.. _Calendar Versioning: https://calver.org
+.. _poetry: https://python-poetry.org/
+.. _Changelog: https://github.com/spapanik/teritorio/blob/main/CHANGELOG.rst
+.. _Documentation: https://teritorio.readthedocs.io/en/latest/
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['teritorio']
-
-package_data = \
-{'': ['*'], 'teritorio': ['_data/*']}
-
-setup_kwargs = {
-    'name': 'teritorio',
-    'version': '2023.2.1',
-    'description': 'A library for country and currency ISO codes',
-    'long_description': '=================================================\nteritorio: ISO codes for countries and currencies\n=================================================\n\n.. image:: https://github.com/spapanik/teritorio/actions/workflows/build.yml/badge.svg\n  :alt: Build\n  :target: https://github.com/spapanik/teritorio/actions/workflows/build.yml\n.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/teritorio.svg\n  :alt: Total alerts\n  :target: https://lgtm.com/projects/g/spapanik/teritorio/alerts/\n.. image:: https://img.shields.io/github/license/spapanik/teritorio\n  :alt: License\n  :target: https://github.com/spapanik/teritorio/blob/main/LICENSE.txt\n.. image:: https://img.shields.io/pypi/v/teritorio\n  :alt: PyPI\n  :target: https://pypi.org/project/teritorio\n.. image:: https://pepy.tech/badge/teritorio\n  :alt: Downloads\n  :target: https://pepy.tech/project/teritorio\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n  :alt: Code style\n  :target: https://github.com/psf/black\n\n``teritorio`` two iterable singletons that ``Countries`` and ``Currencies``, that contain all the\nrelevant ISO information about countries and currencies, respectively.\n\nIn a nutshell\n-------------\n\nInstallation\n^^^^^^^^^^^^\n\nThe easiest way is to use `poetry`_ to manage your dependencies and add *teritorio* to them.\nIt requires Python 3.7.0+ to run.\n\n.. code-block:: toml\n\n    [tool.poetry.dependencies]\n    teritorio = "*"\n\nIt is advised to always use the latest release, so that you\'ll get the latest ISO codes\n\nUsage\n^^^^^\n\nThere are two iterable singletons that can be imported from ``teritorio``: ``Countries`` and ``Currencies``.\n\n.. code:: python\n\n    from teritorio import Countries\n    from teritorio import Currencies\n\nVersioning\n----------\n\nThe project project adheres to `Calendar Versioning`_.\nThe reason is that the data are dominated by political decisions,\nmaking semantic versioning largely irrelevant.\n\nLinks\n-----\n\n- `Documentation`_\n- `Changelog`_\n\n\n.. _Calendar Versioning: https://calver.org\n.. _poetry: https://python-poetry.org/\n.. _Changelog: https://github.com/spapanik/teritorio/blob/main/CHANGELOG.rst\n.. _Documentation: https://teritorio.readthedocs.io/en/latest/\n',
-    'author': 'Stephanos Kuma',
-    'author_email': 'stephanos@kuma.ai',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/spapanik/teritorio',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

