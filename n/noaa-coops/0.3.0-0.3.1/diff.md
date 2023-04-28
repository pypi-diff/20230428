# Comparing `tmp/noaa_coops-0.3.0.tar.gz` & `tmp/noaa_coops-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noaa_coops-0.3.0.tar", max compression
+gzip compressed data, was "noaa_coops-0.3.1.tar", max compression
```

## Comparing `noaa_coops-0.3.0.tar` & `noaa_coops-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11345 2023-04-19 16:48:21.778836 noaa_coops-0.3.0/LICENSE
--rw-r--r--   0        0        0     5654 2023-04-19 16:48:21.780187 noaa_coops-0.3.0/README.md
--rw-r--r--   0        0        0      101 2023-04-19 16:48:21.781179 noaa_coops-0.3.0/noaa_coops/__init__.py
--rw-r--r--   0        0        0    30171 2023-04-19 16:48:21.782340 noaa_coops-0.3.0/noaa_coops/station.py
--rw-r--r--   0        0        0     1567 2023-04-19 16:48:21.783609 noaa_coops-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6650 1970-01-01 00:00:00.000000 noaa_coops-0.3.0/setup.py
--rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 noaa_coops-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-04-19 16:48:21.778836 noaa_coops-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5746 2023-04-19 17:05:24.060617 noaa_coops-0.3.1/README.md
+-rw-r--r--   0        0        0      101 2023-04-28 07:40:26.252516 noaa_coops-0.3.1/noaa_coops/__init__.py
+-rw-r--r--   0        0        0    31293 2023-04-28 07:40:26.253391 noaa_coops-0.3.1/noaa_coops/station.py
+-rw-r--r--   0        0        0     1567 2023-04-28 07:40:26.254125 noaa_coops-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     6751 1970-01-01 00:00:00.000000 noaa_coops-0.3.1/setup.py
+-rw-r--r--   0        0        0     6649 1970-01-01 00:00:00.000000 noaa_coops-0.3.1/PKG-INFO
```

### Comparing `noaa_coops-0.3.0/LICENSE` & `noaa_coops-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noaa_coops-0.3.0/README.md` & `noaa_coops-0.3.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # noaa_coops
 
-[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)
 [![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)
 
 A Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)
 and [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.
 
 ## Installation
-This package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.
+This package is distributed via [PyPi](https://pypi.org/project/noaa-coops/) and can be installed using , `pip`, `poetry`, etc.
+```bash
+# Install with pip
+❯ pip install noaa_coops
+
+# Install with poetry
+❯ poetry add noaa_coops
+```
 
 ## Getting Started
 
 ### Stations
 Data is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:
 
 ```python
@@ -75,15 +81,15 @@
 ```
 
 ### Data Retrieval
 Available data products can be found in NOAA CO-OPS Data API docs.
 
 Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.
 
-The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
+The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The corresponding [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> df_water_levels = seattle.get_data(
 ...     begin_date="20150101",
 ...     end_date="20150131",
@@ -98,14 +104,17 @@
 2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v
 2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v
 2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v
 2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v
 
 ```
 
+![image](https://user-images.githubusercontent.com/28986302/233147224-765fbe05-372c-40f3-8bbe-4102536e7ff3.png)
+
+
 ## Development
 
 ### Requirements
 This package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):
 
 ```bash
 poetry install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noaa_coops-0.3.0/noaa_coops/station.py` & `noaa_coops-0.3.1/noaa_coops/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -737,70 +737,111 @@
         df.index = pd.to_datetime(df["t"])
         df = df.drop(columns=["t"])
 
         # Try to convert strings to numeric values where possible
         for col in df.columns:
             df[col] = pd.to_numeric(df[col], errors="ignore")
 
-        df.drop_duplicates(inplace=True)  # Drop any duplicate rows
+        df = df[~df.index.duplicated(keep="first")]
         self.data = df
 
         return df
 
 
 if __name__ == "__main__":
     # DEBUGGING
     from pprint import pprint
 
     import noaa_coops as nc
 
-    station = nc.Station(id="9447130")  # Seattle, WA
+    station = nc.Station(id="8775241")
+
+    df = station.get_data(
+        begin_date="20230320 00:00",
+        end_date="20230421 00:00",
+        product="predictions",
+        datum="MSL",
+        interval="h",
+        units="english",
+        time_zone="gmt",
+    )
+
+    pprint(df.head())
+    print("\n" * 2)
+
+    pprint(df.tail())
+    print("\n" * 2)
+
+    print(df.info())
+
+    df.to_csv("debug.csv")
+
+    # station = nc.Station(id="9447130")  # Seattle, WA
+
+    # Test replicating the data seen on the station page:
+    # https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20220101&edate=20220430&timezone=GMT&datum=MLLW&interval=h&action=
+    # 2022-01-01 00:00:00, 2022-04-30 23:00:00, 1-hr, MLLW, GMT, metric
 
     # print("Test that metadata is working:")
     # pprint(station.metadata)
     # print("\n" * 2)
 
     # print("Test that attributes are populated from metadata:")
     # pprint(station.sensors)
     # print("\n" * 2)
 
     # print("Test that data_inventory is working:")
     # pprint(station.data_inventory, indent=4, compact=True, width=100)
     # print("\n" * 2)
 
-    print("6-min water level station request:")
-    data = station.get_data(
-        begin_date="20150101",
-        end_date="20150331",
-        product="water_level",
-        datum="MLLW",
-        units="metric",
-        time_zone="gmt",
-    )
-    pprint(data.head())
-    print("\n" * 2)
+    # print("6-min water level station request:")
+    # data = station.get_data(
+    #     begin_date="20220101 00:00",
+    #     end_date="20220430 23:00",
+    #     product="hourly_height",
+    #     datum="MLLW",
+    #     units="metric",
+    #     time_zone="gmt",
+    # )
+    # pprint(data.head())
+    # print("\n" * 2)
 
-    print("1-hr water level station request (SHOULD NOT WORK):")
-    data = station.get_data(
-        begin_date="20150101",
-        end_date="20150331",
-        product="water_level",
-        interval="h",
-        datum="MLLW",
-        units="metric",
-        time_zone="gmt",
-    )
-    pprint(data.head())
-    print("\n" * 2)
+    # pprint(data.tail())
+    # print("\n" * 2)
 
-    print("high-low request:")
-    data = station.get_data(
-        begin_date="20150101",
-        end_date="20150331",
-        product="high_low",
-        datum="MLLW",
-        units="metric",
-        time_zone="gmt",
-    )
-    pprint(data.head())
-    print("\n" * 2)
-    pprint(data.loc["2015"])
+    # print("6-min water level station request:")
+    # data = station.get_data(
+    #     begin_date="20150101",
+    #     end_date="20150331",
+    #     product="water_level",
+    #     datum="MLLW",
+    #     units="metric",
+    #     time_zone="gmt",
+    # )
+    # pprint(data.head())
+    # print("\n" * 2)
+
+    # print("1-hr water level station request (SHOULD NOT WORK):")
+    # data = station.get_data(
+    #     begin_date="20150101",
+    #     end_date="20150331",
+    #     product="water_level",
+    #     interval="h",
+    #     datum="MLLW",
+    #     units="metric",
+    #     time_zone="gmt",
+    # )
+    # pprint(data.head())
+    # print("\n" * 2)
+
+    # print("high-low request:")
+    # data = station.get_data(
+    #     begin_date="20150101",
+    #     end_date="20150331",
+    #     product="high_low",
+    #     datum="MLLW",
+    #     units="metric",
+    #     time_zone="gmt",
+    # )
+    # pprint(data.head())
+    # print("\n" * 2)
+    # pprint(data.loc["2015"])
```

### Comparing `noaa_coops-0.3.0/pyproject.toml` & `noaa_coops-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "noaa-coops"
-version = "0.3.0"
+version = "0.3.1"
 description = "Python wrapper for NOAA Tides & Currents Data and Metadata."
 authors = ["Greg Clunies <greg.clunies@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/GClunies/noaa_coops"
 keywords = ["noaa", "coops", "tides", "currents", "weather", "api"]
 packages = [{include = "noaa_coops"}]
```

### Comparing `noaa_coops-0.3.0/setup.py` & `noaa_coops-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['numpy>=1.24.1,<2.0.0',
  'pandas>=1.5.3,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'zeep>=4.2.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'noaa-coops',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Python wrapper for NOAA Tides & Currents Data and Metadata.',
-    'long_description': '# noaa_coops\n\n[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n### Data Retrieval\nAvailable data products can be found in NOAA CO-OPS Data API docs.\n\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.\n\nThe example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150131",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                         v      s        f  q\nt\n2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v\n\n```\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
+    'long_description': '# noaa_coops\n\n[![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)\n\nA Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)\nand [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.\n\n## Installation\nThis package is distributed via [PyPi](https://pypi.org/project/noaa-coops/) and can be installed using , `pip`, `poetry`, etc.\n```bash\n# Install with pip\n❯ pip install noaa_coops\n\n# Install with poetry\n❯ poetry add noaa_coops\n```\n\n## Getting Started\n\n### Stations\nData is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")  # Create Station object for Seattle (ID = 9447130)\n```\n\nStations and their IDs can be found using the Tides & Currents [mapping interface](https://tidesandcurrents.noaa.gov/). Alternatively, you can search for stations in a bounding box using the `get_stations_from_bbox` function, which will return a list of stations found in the box (if any).\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station, get_stations_from_bbox\n>>> stations = get_stations_from_bbox(lat_coords=[40.389, 40.9397], lon_coords=[-74.4751, -73.7432])\n>>> pprint(stations)\n[\'8516945\', \'8518750\', \'8519483\', \'8531680\']\n>>> station_one = Station(id="8516945")\n>>> pprint(station_one.name)\n\'Kings Point\'\n```\n\n### Metadata\nStation metadata is stored in the `.metadata` attribute of a `Station` object. Additionally, the keys of the metadata attribute dictionary are also assigned as attributes of the station object itself.\n\n```python\n>>> from pprint import pprint\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> pprint(list(seattle.metadata.items())[:5])                   # Print first 3 items in metadata\n[(\'tidal\', True), (\'greatlakes\', False), (\'shefcode\', \'EBSW1\')]  # Metadata dictionary can be very long\n>>> pprint(seattle.lat_lon[\'lat\'])                               # Print latitude\n47.601944\n>>> pprint(seattle.lat_lon[\'lon\'])                               # Print longitude\n-122.339167\n```\n\n### Data Inventory\nA description of a Station\'s data products and available dates can be accessed via the `.data_inventory` attribute of a `Station` object.\n\n```python\n>>> from noaa_coops import Station\n>>> from pprint import pprint\n>>> seattle = Station(id="9447130")\n>>> pprint(seattle.data_inventory)\n{\'Air Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                     \'start_date\': \'1991-11-09 01:00\'},\n \'Barometric Pressure\': {\'end_date\': \'2019-01-02 18:36\',\n                         \'start_date\': \'1991-11-09 00:00\'},\n \'Preliminary 6-Minute Water Level\': {\'end_date\': \'2023-02-05 19:54\',\n                                      \'start_date\': \'2001-01-01 00:00\'},\n \'Verified 6-Minute Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1995-06-01 00:00\'},\n \'Verified High/Low Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                   \'start_date\': \'1977-10-18 02:18\'},\n \'Verified Hourly Height Water Level\': {\'end_date\': \'2022-12-31 23:00\',\n                                        \'start_date\': \'1899-01-01 00:00\'},\n \'Verified Monthly Mean Water Level\': {\'end_date\': \'2022-12-31 23:54\',\n                                       \'start_date\': \'1898-12-01 00:00\'},\n \'Water Temperature\': {\'end_date\': \'2019-01-02 18:36\',\n                       \'start_date\': \'1991-11-09 00:00\'},\n \'Wind\': {\'end_date\': \'2019-01-02 18:36\', \'start_date\': \'1991-11-09 00:00\'}}\n```\n\n### Data Retrieval\nAvailable data products can be found in NOAA CO-OPS Data API docs.\n\nStation data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.\n\nThe example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The corresponding [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.\n\n```python\n>>> from noaa_coops import Station\n>>> seattle = Station(id="9447130")\n>>> df_water_levels = seattle.get_data(\n...     begin_date="20150101",\n...     end_date="20150131",\n...     product="water_level",\n...     datum="MLLW",\n...     units="metric",\n...     time_zone="gmt")\n>>> df_water_levels.head()\n                         v      s        f  q\nt\n2015-01-01 00:00:00  1.799  0.023  0,0,0,0  v\n2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v\n2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v\n2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v\n2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v\n\n```\n\n![image](https://user-images.githubusercontent.com/28986302/233147224-765fbe05-372c-40f3-8bbe-4102536e7ff3.png)\n\n\n## Development\n\n### Requirements\nThis package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):\n\n```bash\npoetry install\n```\n\n### TODO\nClick [here](https://github.com/GClunies/noaa_coops/issues) for a list of existing issues and to submit a new one.\n\n### Contribution\nContributions are welcome, feel free to submit a pull request.\n',
     'author': 'Greg Clunies',
     'author_email': 'greg.clunies@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GClunies/noaa_coops',
     'packages': packages,
     'package_data': package_data,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `noaa_coops-0.3.0/PKG-INFO` & `noaa_coops-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noaa-coops
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python wrapper for NOAA Tides & Currents Data and Metadata.
 Home-page: https://github.com/GClunies/noaa_coops
 License: Apache-2.0
 Keywords: noaa,coops,tides,currents,weather,api
 Author: Greg Clunies
 Author-email: greg.clunies@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,23 +19,29 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: zeep (>=4.2.1,<5.0.0)
 Project-URL: Repository, https://github.com/GClunies/noaa_coops
 Description-Content-Type: text/markdown
 
 # noaa_coops
 
-[![Build Status](https://travis-ci.org/GClunies/noaa_coops.svg?branch=master)](https://travis-ci.org/GClunies/noaa_coops)
 [![PyPI](https://img.shields.io/pypi/v/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/noaa_coops.svg)](https://pypi.python.org/pypi/noaa-coops)
 
 A Python wrapper for the NOAA CO-OPS Tides &amp; Currents [Data](https://tidesandcurrents.noaa.gov/api/)
 and [Metadata](https://tidesandcurrents.noaa.gov/mdapi/latest/) APIs.
 
 ## Installation
-This package is distributed through [pip](https://pypi.org/project/noaa-coops/) and can be installed to an environment via `pip install noaa-coops`.
+This package is distributed via [PyPi](https://pypi.org/project/noaa-coops/) and can be installed using , `pip`, `poetry`, etc.
+```bash
+# Install with pip
+❯ pip install noaa_coops
+
+# Install with poetry
+❯ poetry add noaa_coops
+```
 
 ## Getting Started
 
 ### Stations
 Data is accessed via `Station` class objects. Each station is uniquely identified by an `id`. To initialize a `Station` object, run:
 
 ```python
@@ -98,15 +104,15 @@
 ```
 
 ### Data Retrieval
 Available data products can be found in NOAA CO-OPS Data API docs.
 
 Station data can be fetched using the `.get_data` method on a `Station` object. Data is returned as a Pandas [DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html) for ease of use and analysis. DataFrame columns are named according to the NOAA CO-OPS API [docs](https://api.tidesandcurrents.noaa.gov/api/prod/responseHelp.html), with the `t` column (timestamp) set as the DataFrame index.
 
-The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
+The example below fetches water level data from the Seattle station (id=9447130) for a 1 month period. The corresponding [web output](https://tidesandcurrents.noaa.gov/waterlevels.html?id=9447130&units=metric&bdate=20150101&edate=20150131&timezone=GMT&datum=MLLW) is shown below the code as a reference.
 
 ```python
 >>> from noaa_coops import Station
 >>> seattle = Station(id="9447130")
 >>> df_water_levels = seattle.get_data(
 ...     begin_date="20150101",
 ...     end_date="20150131",
@@ -121,14 +127,17 @@
 2015-01-01 00:06:00  1.718  0.018  0,0,0,0  v
 2015-01-01 00:12:00  1.639  0.013  0,0,0,0  v
 2015-01-01 00:18:00  1.557  0.012  0,0,0,0  v
 2015-01-01 00:24:00  1.473  0.014  0,0,0,0  v
 
 ```
 
+![image](https://user-images.githubusercontent.com/28986302/233147224-765fbe05-372c-40f3-8bbe-4102536e7ff3.png)
+
+
 ## Development
 
 ### Requirements
 This package and its dependencies are managed using [poetry](https://python-poetry.org/). To install the development environment for `noaa_coops`, first install poetry, then run (inside the repo):
 
 ```bash
 poetry install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

