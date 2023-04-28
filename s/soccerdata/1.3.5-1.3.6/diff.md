# Comparing `tmp/soccerdata-1.3.5.tar.gz` & `tmp/soccerdata-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soccerdata-1.3.5.tar", max compression
+gzip compressed data, was "soccerdata-1.3.6.tar", max compression
```

## Comparing `soccerdata-1.3.5.tar` & `soccerdata-1.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1384 2023-04-22 09:17:56.031795 soccerdata-1.3.5/LICENSE.rst
--rw-r--r--   0        0        0     3130 2023-04-22 09:17:56.031795 soccerdata-1.3.5/README.rst
--rw-r--r--   0        0        0     2352 2023-04-22 09:18:08.391831 soccerdata-1.3.5/pyproject.toml
--rw-r--r--   0        0        0      457 2023-04-22 09:18:08.391831 soccerdata-1.3.5/soccerdata/__init__.py
--rw-r--r--   0        0        0    20126 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/_common.py
--rw-r--r--   0        0        0     5144 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/_config.py
--rw-r--r--   0        0        0     6218 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/clubelo.py
--rw-r--r--   0        0        0    12693 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/espn.py
--rw-r--r--   0        0        0    30578 2023-04-22 09:17:56.039795 soccerdata-1.3.5/soccerdata/fbref.py
--rw-r--r--   0        0        0     8584 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/fivethirtyeight.py
--rw-r--r--   0        0        0     4547 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/match_history.py
--rw-r--r--   0        0        0     9712 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/sofifa.py
--rw-r--r--   0        0        0    32302 2023-04-22 09:17:56.043794 soccerdata-1.3.5/soccerdata/whoscored.py
--rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.3.5/setup.py
--rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1384 2023-04-28 15:50:52.938151 soccerdata-1.3.6/LICENSE.rst
+-rw-r--r--   0        0        0     3130 2023-04-28 15:50:52.938151 soccerdata-1.3.6/README.rst
+-rw-r--r--   0        0        0     2352 2023-04-28 15:51:06.062018 soccerdata-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0      457 2023-04-28 15:51:06.062018 soccerdata-1.3.6/soccerdata/__init__.py
+-rw-r--r--   0        0        0    20428 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/_common.py
+-rw-r--r--   0        0        0     5144 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/_config.py
+-rw-r--r--   0        0        0     6218 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/clubelo.py
+-rw-r--r--   0        0        0    12693 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/espn.py
+-rw-r--r--   0        0        0    31315 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/fbref.py
+-rw-r--r--   0        0        0     8584 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/fivethirtyeight.py
+-rw-r--r--   0        0        0     4547 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/match_history.py
+-rw-r--r--   0        0        0     9831 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/sofifa.py
+-rw-r--r--   0        0        0    32302 2023-04-28 15:50:52.946151 soccerdata-1.3.6/soccerdata/whoscored.py
+-rw-r--r--   0        0        0     4186 1970-01-01 00:00:00.000000 soccerdata-1.3.6/setup.py
+-rw-r--r--   0        0        0     4471 1970-01-01 00:00:00.000000 soccerdata-1.3.6/PKG-INFO
```

### Comparing `soccerdata-1.3.5/LICENSE.rst` & `soccerdata-1.3.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/README.rst` & `soccerdata-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/pyproject.toml` & `soccerdata-1.3.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "soccerdata"
-version = "1.3.5"
+version = "1.3.6"
 description = "A collection of wrappers over soccer data from various websites / APIs."
 authors = ["Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "Apache-2.0"
 readme = 'README.rst'
 homepage = "https://github.com/probberechts/soccerdata"
 repository = "https://github.com/probberechts/soccerdata"
 keywords = ["soccer", "football", "soccer data", "web scraping", "soccer analytics"]
```

### Comparing `soccerdata-1.3.5/soccerdata/_common.py` & `soccerdata-1.3.6/soccerdata/_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,23 @@
             data_dir=data_dir,
         )
 
         self._session = self._init_session()
 
     def _init_session(self) -> requests.Session:
         session = requests.Session()
+        session.headers.update(
+            {
+                "User-Agent": (
+                    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) "
+                    "AppleWebKit/537.36 (KHTML, like Gecko) "
+                    "Chrome/59.0.3071.86 Safari/537.36"
+                )
+            }
+        )
         session.proxies.update(self.proxy())
         return session
 
     def _download_and_save(
         self,
         url: str,
         filepath: Optional[Path] = None,
```

### Comparing `soccerdata-1.3.5/soccerdata/_config.py` & `soccerdata-1.3.6/soccerdata/_config.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/soccerdata/clubelo.py` & `soccerdata-1.3.6/soccerdata/clubelo.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/soccerdata/espn.py` & `soccerdata-1.3.6/soccerdata/espn.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/soccerdata/fbref.py` & `soccerdata-1.3.6/soccerdata/fbref.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         url = f"{FBREF_API}/en/comps/"
         filepath = self.data_dir / "leagues.html"
         reader = self.get(url, filepath)
 
         # extract league links
         leagues = []
         tree = html.parse(reader)
-        for table in tree.xpath("//table[contains(@id, 'comps')]"):
-            df_table = pd.read_html(etree.tostring(table, method="html"))[0]
-            df_table["url"] = table.xpath(".//th[@data-stat='league_name']/a/@href")
+        for html_table in tree.xpath("//table[contains(@id, 'comps')]"):
+            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table["url"] = html_table.xpath(".//th[@data-stat='league_name']/a/@href")
             leagues.append(df_table)
         df = (
             pd.concat(leagues)
             .pipe(standardize_colnames)
             .rename(columns={"competition_name": "league"})
             .pipe(self._translate_league)
             .drop_duplicates(subset="league")
@@ -168,17 +168,18 @@
         for lkey, league in df_leagues.iterrows():
             url = FBREF_API + league.url
             filepath = self.data_dir / filemask.format(lkey)
             reader = self.get(url, filepath)
 
             # extract season links
             tree = html.parse(reader)
-            df_table = pd.read_html(etree.tostring(tree), attrs={"id": "seasons"})[0]
-            df_table["url"] = tree.xpath(
-                "//table[@id='seasons']//th[@data-stat='year_id' or @data-stat='year']/a/@href"
+            (html_table,) = tree.xpath("//table[@id='seasons']")
+            (df_table,) = pd.read_html(html.tostring(html_table))
+            df_table["url"] = html_table.xpath(
+                "//th[@data-stat='year_id' or @data-stat='year']/a/@href"
             )
             # Override the competition name or add if missing
             df_table["Competition Name"] = lkey
             # Some tournaments have a "year" column instead of "season"
             if "Year" in df_table.columns:
                 df_table.rename(columns={"Year": "Season"}, inplace=True)
             # Get the competition format
@@ -287,25 +288,26 @@
                 + "/".join(season.url.split("/")[:-1])
                 + (f"/{page}/squads/" if big_five else f"/{page}/" if tournament else "/")
                 + season.url.split("/")[-1]
             )
             reader = self.get(url, filepath)
 
             # parse HTML and select table
-            tree = html.parse(reader).xpath(
+            tree = html.parse(reader)
+            (html_table,) = tree.xpath(
                 f"//table[@id='stats_teams_{stat_type}' or @id='stats_squads_{stat_type}']"
-            )[0]
+            )
             # remove icons
-            for elem in tree.xpath("//span"):
+            for elem in html_table.xpath("//span"):
                 elem.getparent().remove(elem)
             # parse table
-            df_table = pd.read_html(etree.tostring(tree))[0]
+            (df_table,) = pd.read_html(html.tostring(html_table))
             df_table["league"] = lkey
             df_table["season"] = skey
-            df_table["url"] = tree.xpath(".//*[@data-stat='team']/a/@href")
+            df_table["url"] = html_table.xpath(".//*[@data-stat='team']/a/@href")
             if big_five:
                 df_table["league"] = (
                     df_table.xs("Comp", axis=1, level=1).squeeze().map(BIG_FIVE_DICT)
                 )
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
                 df_table.drop("Rk", axis=1, level=1, inplace=True)
             teams.append(df_table)
@@ -400,23 +402,23 @@
             )
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             # remove icons
             for elem in tree.xpath("//td[@data-stat='comp_level']//span"):
                 elem.getparent().remove(elem)
             if big_five:
-                df_table = pd.read_html(etree.tostring(tree))[0]
+                (df_table,) = pd.read_html(html.tostring(tree))
                 df_table[("Unnamed: league", "league")] = (
                     df_table.xs("Comp", axis=1, level=1).squeeze().map(BIG_FIVE_DICT)
                 )
                 df_table[("Unnamed: season", "season")] = skey
                 df_table.drop("Comp", axis=1, level=1, inplace=True)
             else:
-                el = tree.xpath(f"//comment()[contains(.,'div_stats_{stat_type}')]")[0]
-                df_table = pd.read_html(el.text, attrs={"id": f"stats_{stat_type}"})[0]
+                (el,) = tree.xpath(f"//comment()[contains(.,'div_stats_{stat_type}')]")
+                (df_table,) = pd.read_html(el.text, attrs={"id": f"stats_{stat_type}"})
                 df_table[("Unnamed: league", "league")] = lkey
                 df_table[("Unnamed: season", "season")] = skey
 
             if not ("Unnamed: 2_level_0", "Nation") in df_table.columns:
                 df_table.loc[:, (slice(None), "Squad")] = (
                     df_table.xs("Squad", axis=1, level=1)
                     .squeeze()
@@ -482,21 +484,21 @@
             url_fixtures = FBREF_API + tree.xpath("//a[text()='Scores & Fixtures']")[0].get("href")
             filepath_fixtures = self.data_dir / f"schedule_{lkey}_{skey}.html"
             current_season = not self._is_complete(lkey, skey)
             reader = self.get(
                 url_fixtures, filepath_fixtures, no_cache=current_season and not force_cache
             )
             tree = html.parse(reader)
-            table = tree.xpath("//table[contains(@id, 'sched')]")[0]
-            df_table = pd.read_html(etree.tostring(table))[0]
+            html_table = tree.xpath("//table[contains(@id, 'sched')]")[0]
+            (df_table,) = pd.read_html(html.tostring(html_table))
             df_table["Match Report"] = [
                 mlink.xpath("./a/@href")[0]
                 if mlink.xpath("./a") and mlink.xpath("./a")[0].text == "Match Report"
                 else None
-                for mlink in table.xpath(".//td[@data-stat='match_report']")
+                for mlink in html_table.xpath(".//td[@data-stat='match_report']")
             ]
             df_table["league"] = lkey
             df_table["season"] = skey
             df_table = df_table.dropna(how="all")
             schedule.append(df_table)
         df = (
             pd.concat(schedule)
@@ -579,27 +581,27 @@
             ]
             if len(iterator) == 0:
                 raise ValueError("No games found with the given IDs in the selected seasons.")
         else:
             iterator = df_schedule
 
         lineups = []
-        for i, game in iterator.iterrows():
+        for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             teams = self._parse_teams(tree)
-            tables = tree.xpath("//div[@class='lineup']")
-            for i, table in enumerate(tables):
-                df_table = pd.read_html(etree.tostring(table))[0]
+            html_tables = tree.xpath("//div[@class='lineup']")
+            for i, html_table in enumerate(html_tables):
+                (df_table,) = pd.read_html(html.tostring(html_table))
                 df_table.columns = ["jersey_number", "player"]
                 df_table["team"] = teams[i]["name"]
                 if "Bench" in df_table.jersey_number.values:
                     bench_idx = df_table.index[df_table.jersey_number == "Bench"][0]
                     df_table.loc[:bench_idx, "is_starter"] = True
                     df_table.loc[bench_idx:, "is_starter"] = False
                     df_table["game"] = game["game"]
@@ -677,44 +679,50 @@
             ]
             if len(iterator) == 0:
                 raise ValueError("No games found with the given IDs in the selected seasons.")
         else:
             iterator = df_schedule
 
         stats = []
-        for i, game in iterator.iterrows():
+        for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
             (home_team, away_team) = self._parse_teams(tree)
             if stat_type == "keepers":
                 id_format = "keeper_stats_{}"
             else:
                 id_format = "stats_{}_" + stat_type
-            table = tree.xpath("//table[@id='" + id_format.format(home_team["id"]) + "']")[0]
-            df_table = pd.read_html(etree.tostring(table))[0]
-            df_table["team"] = home_team["name"]
-            df_table["game"] = game["game"]
-            df_table["league"] = game["league"]
-            df_table["season"] = game["season"]
-            df_table["game_id"] = game["game_id"]
-            stats.append(df_table)
-            table = tree.xpath("//table[@id='" + id_format.format(away_team["id"]) + "']")[0]
-            df_table = pd.read_html(etree.tostring(table))[0]
-            df_table["team"] = away_team["name"]
-            df_table["game"] = game["game"]
-            df_table["league"] = game["league"]
-            df_table["season"] = game["season"]
-            df_table["game_id"] = game["game_id"]
-            stats.append(df_table)
+            html_table = tree.find("//table[@id='" + id_format.format(home_team["id"]) + "']")
+            if html_table is not None:
+                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table["team"] = home_team["name"]
+                df_table["game"] = game["game"]
+                df_table["league"] = game["league"]
+                df_table["season"] = game["season"]
+                df_table["game_id"] = game["game_id"]
+                stats.append(df_table)
+            else:
+                logger.warning("No stats found for home team for game with id=%s", game["game_id"])
+            html_table = tree.find("//table[@id='" + id_format.format(away_team["id"]) + "']")
+            if html_table is not None:
+                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table["team"] = away_team["name"]
+                df_table["game"] = game["game"]
+                df_table["league"] = game["league"]
+                df_table["season"] = game["season"]
+                df_table["game_id"] = game["game_id"]
+                stats.append(df_table)
+            else:
+                logger.warning("No stats found for away team for game with id=%s", game["game_id"])
 
         df = _concat(stats)
         df = df[~df.Player.str.contains(r"^\d+\sPlayers$")]
         df = (
             df.rename(columns={"Player": "player"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .set_index(["league", "season", "game", "team", "player"])
@@ -762,28 +770,32 @@
             ]
             if len(iterator) == 0:
                 raise ValueError("No games found with the given IDs in the selected seasons.")
         else:
             iterator = df_schedule
 
         shots = []
-        for i, game in iterator.iterrows():
+        for i, game in iterator.reset_index().iterrows():
             url = urlmask.format(game["game_id"])
             # get league and season
             logger.info(
                 "[%s/%s] Retrieving game with id=%s", i + 1, len(iterator), game["game_id"]
             )
             filepath = self.data_dir / filemask.format(game["game_id"])
             reader = self.get(url, filepath)
             tree = html.parse(reader)
-            df_table = pd.read_html(etree.tostring(tree), attrs={"id": "shots_all"})[0]
-            df_table["league"] = game["league"]
-            df_table["season"] = game["season"]
-            df_table["game"] = game["game"]
-            shots.append(df_table)
+            html_table = tree.find("//table[@id='shots_all']")
+            if html_table is not None:
+                (df_table,) = pd.read_html(html.tostring(html_table))
+                df_table["league"] = game["league"]
+                df_table["season"] = game["season"]
+                df_table["game"] = game["game"]
+                shots.append(df_table)
+            else:
+                logger.warning("No shot data found for game with id=%s", game["game_id"])
 
         df = (
             _concat(shots)
             .rename(columns={"Squad": "team"})
             .replace({"team": TEAMNAME_REPLACEMENTS})
             .pipe(
                 standardize_colnames,
```

### Comparing `soccerdata-1.3.5/soccerdata/fivethirtyeight.py` & `soccerdata-1.3.6/soccerdata/fivethirtyeight.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/soccerdata/match_history.py` & `soccerdata-1.3.6/soccerdata/match_history.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/soccerdata/sofifa.py` & `soccerdata-1.3.6/soccerdata/sofifa.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Union
 
 import pandas as pd
 from lxml import html
 
 from ._common import BaseRequestsReader, standardize_colnames
-from ._config import DATA_DIR, NOCACHE, NOSTORE, TEAMNAME_REPLACEMENTS
+from ._config import DATA_DIR, NOCACHE, NOSTORE, TEAMNAME_REPLACEMENTS, logger
 
 SO_FIFA_DATADIR = DATA_DIR / "SoFIFA"
 SO_FIFA_API = "https://sofifa.com"
 
 
 class SoFIFA(BaseRequestsReader):
     """Provides pd.DataFrames from data at http://sofifa.com.
@@ -162,14 +162,15 @@
         teams = self.read_teams().reset_index()
 
         # collect players
         players = []
         for _, team in teams.iterrows():
             season_id = team.season[:2]
             team_name = team.team
+
             # read html page (team overview)
             filepath = self.data_dir / filemask.format(team_name, season_id)
             url = urlmask.format(team["team_id"], season_id)
             reader = self.get(url, filepath)
 
             # extract player links
             tree = html.parse(reader)
@@ -246,17 +247,19 @@
             "GK Diving",
             "GK Handling",
             "GK Kicking",
             "GK Positioning",
             "GK Reflexes",
         ]
 
-        for _, player in players.iterrows():
-            # read html page (player overview)
+        for i, player in players.reset_index().iterrows():
             player_name = player.player
+            logger.info("[%s/%s] Retrieving ratings for %s", i + 1, len(players), player_name)
+
+            # read html page (player overview)
             filepath = self.data_dir / filemask.format(player_name, player.season)
             url = urlmask.format(player["player_id"], player.season[:2])
             reader = self.get(url, filepath)
 
             # extract scores one-by-one
             tree = html.parse(reader)
             scores = {
```

### Comparing `soccerdata-1.3.5/soccerdata/whoscored.py` & `soccerdata-1.3.6/soccerdata/whoscored.py`

 * *Files identical despite different names*

### Comparing `soccerdata-1.3.5/setup.py` & `soccerdata-1.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'rich>=13.0.0,<14.0.0',
  'selenium>=4.0.0,<5.0.0',
  'undetected-chromedriver>=3.1.3,<4.0.0',
  'unicode>=2.7,<3.0']
 
 setup_kwargs = {
     'name': 'soccerdata',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'A collection of wrappers over soccer data from various websites / APIs.',
     'long_description': ".. image:: https://raw.githubusercontent.com/probberechts/soccerdata/master/docs/_static/logo2.png\n   :align: center\n   :alt: SoccerData\n   :width: 600px\n\n.. badges-begin\n\n|PyPI| |Python Version| |License| |Read the Docs| |Tests| |Codecov| |pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/soccerdata.svg\n   :target: https://pypi.org/project/soccerdata/\n   :alt: PyPI\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/soccerdata\n   :target: https://pypi.org/project/soccerdata\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/soccerdata.svg\n   :target: https://opensource.org/licenses/Apache-2.0\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/soccerdata/latest.svg?label=Read%20the%20Docs\n   :target: https://soccerdata.readthedocs.io/\n   :alt: Read the documentation at https://soccerdata.readthedocs.io/\n.. |Tests| image:: https://github.com/probberechts/soccerdata/workflows/CI/badge.svg\n   :target: https://github.com/probberechts/soccerdata/actions?workflow=CI\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/probberechts/soccerdata/branch/master/graph/badge.svg\n   :target: https://app.codecov.io/gh/probberechts/soccerdata\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n.. badges-end\n\nSoccerData is a collection of wrappers over soccer data from `Club Elo`_,\n`ESPN`_, `FBref`_, `FiveThirtyEight`_, `Football-Data.co.uk`_, `SoFIFA`_ and\n`WhoScored`_. You get Pandas DataFrames with sensible, matching column names\nand identifiers across datasets. Data is downloaded when needed and cached\nlocally.\n\n.. code:: python\n\n   import soccerdata as sd\n\n   # Create scraper class instance for the Premier League\n   five38 = sd.FiveThirtyEight('ENG-Premier League', '1819')\n\n   # Fetch dataframes\n   games = five38.read_games()\n\nTo learn how to install, configure and use SoccerData, see the\n`Quickstart guide <https://soccerdata.readthedocs.io/en/latest/usage.html>`__. For documentation on each of the\nsupported data sources, see the `example notebooks <https://soccerdata.readthedocs.io/en/latest/datasources/>`__ and `API reference <https://soccerdata.readthedocs.io/en/latest/reference/>`__.\n\n.. _Club Elo: https://www.clubelo.com/\n.. _ESPN: https://www.espn.com/soccer/\n.. _FBref: https://www.fbref.com/en/\n.. _FiveThirtyEight: https://fivethirtyeight.com/soccer-predictions/\n.. _Football-Data.co.uk: https://www.football-data.co.uk/\n.. _SoFIFA: https://sofifa.com/\n.. _WhoScored: https://www.whoscored.com/\n\n**Disclaimer:** As soccerdata relies on web scraping, any changes to the\nscraped websites will break the package. Hence, do not expect that all code\nwill work all the time. If you spot any bugs, then please `fork it and start\na pull request <https://github.com/probberechts/soccerdata/blob/master/CONTRIBUTING.rst>`__.\n",
     'author': 'Pieter Robberechts',
     'author_email': 'pieter.robberechts@kuleuven.be',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/probberechts/soccerdata',
```

### Comparing `soccerdata-1.3.5/PKG-INFO` & `soccerdata-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soccerdata
-Version: 1.3.5
+Version: 1.3.6
 Summary: A collection of wrappers over soccer data from various websites / APIs.
 Home-page: https://github.com/probberechts/soccerdata
 License: Apache-2.0
 Keywords: soccer,football,soccer data,web scraping,soccer analytics
 Author: Pieter Robberechts
 Author-email: pieter.robberechts@kuleuven.be
 Requires-Python: >=3.8.1,<4.0.0
```

