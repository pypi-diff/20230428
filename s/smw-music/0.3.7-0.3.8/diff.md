# Comparing `tmp/smw_music-0.3.7.tar.gz` & `tmp/smw_music-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smw_music-0.3.7.tar", max compression
+gzip compressed data, was "smw_music-0.3.8.tar", max compression
```

## Comparing `smw_music-0.3.7.tar` & `smw_music-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0        0        0        0 2023-04-06 07:47:06.518671 smw_music-0.3.7/LICENSES/
--rw-r--r--   0        0        0     5252 2023-04-06 07:47:06.518671 smw_music-0.3.7/README.rst
--rw-r--r--   0        0        0     2496 2023-04-06 07:47:06.518671 smw_music-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      710 2023-04-06 07:47:06.518671 smw_music-0.3.7/smw_music/__init__.py
--rw-r--r--   0        0        0   131530 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/ashtley.gif
--rw-r--r--   0        0        0       66 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/codenames.csv
--rw-r--r--   0        0        0      252 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/convert.bat
--rw-r--r--   0        0        0      270 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/convert.sh
--rw-r--r--   0        0        0   107468 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/dashboard.ui
--rw-r--r--   0        0        0     9009 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/maestro.svg
--rw-r--r--   0        0        0     5330 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/mml.txt
--rw-r--r--   0        0        0     4321 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/data/preferences.ui
--rw-r--r--   0        0        0     2684 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/log.py
--rw-r--r--   0        0        0      500 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/__init__.py
--rw-r--r--   0        0        0     6716 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/channel.py
--rw-r--r--   0        0        0     5685 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/echo.py
--rw-r--r--   0        0        0    14070 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/instrument.py
--rw-r--r--   0        0        0    12411 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/mml.py
--rw-r--r--   0        0        0    16816 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/reduction.py
--rw-r--r--   0        0        0     1041 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/shared.py
--rw-r--r--   0        0        0    25691 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/song.py
--rw-r--r--   0        0        0    18411 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/music_xml/tokens.py
--rw-r--r--   0        0        0        0 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/py.typed
--rw-r--r--   0        0        0      204 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/scripts/__init__.py
--rw-r--r--   0        0        0     2559 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/scripts/convert.py
--rw-r--r--   0        0        0     1645 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/scripts/dashboard.py
--rw-r--r--   0        0        0     7933 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/scripts/filttool.py
--rw-r--r--   0        0        0      205 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/__init__.py
--rw-r--r--   0        0        0    53476 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/dashboard.py
--rw-r--r--   0        0        0     8837 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/dashboard_view.py
--rw-r--r--   0        0        0     8356 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/envelope_preview.py
--rw-r--r--   0        0        0     8522 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/keyboard.py
--rw-r--r--   0        0        0    57346 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/model.py
--rw-r--r--   0        0        0      205 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/old_save/__init__.py
--rw-r--r--   0        0        0     6739 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/old_save/v0.py
--rw-r--r--   0        0        0     4568 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/preferences.py
--rw-r--r--   0        0        0      852 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/preferences_view.py
--rw-r--r--   0        0        0    22284 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/quotes.py
--rw-r--r--   0        0        0     5823 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/sample.py
--rw-r--r--   0        0        0    11460 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/save.py
--rw-r--r--   0        0        0     4017 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/state.py
--rw-r--r--   0        0        0     8040 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/utilization.py
--rw-r--r--   0        0        0     1261 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/ui/utils.py
--rw-r--r--   0        0        0     1811 2023-04-06 07:47:06.522671 smw_music-0.3.7/smw_music/utils.py
--rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 smw_music-0.3.7/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-28 00:41:15.166135 smw_music-0.3.8/LICENSES/
+-rw-r--r--   0        0        0     5252 2023-04-28 00:41:15.166135 smw_music-0.3.8/README.rst
+-rw-r--r--   0        0        0     2496 2023-04-28 00:41:15.166135 smw_music-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      710 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/__init__.py
+-rw-r--r--   0        0        0     9772 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/brr.py
+-rw-r--r--   0        0        0    77544 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/ankha.gif
+-rw-r--r--   0        0        0   131530 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/ashtley.gif
+-rw-r--r--   0        0        0       84 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/codenames.csv
+-rw-r--r--   0        0        0      252 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/convert.bat
+-rw-r--r--   0        0        0      270 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/convert.sh
+-rw-r--r--   0        0        0   126564 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/dashboard.ui
+-rw-r--r--   0        0        0     9009 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/maestro.svg
+-rw-r--r--   0        0        0     5330 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/mml.txt
+-rw-r--r--   0        0        0     4321 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/data/preferences.ui
+-rw-r--r--   0        0        0     2684 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/log.py
+-rw-r--r--   0        0        0      500 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/__init__.py
+-rw-r--r--   0        0        0     6716 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/channel.py
+-rw-r--r--   0        0        0     5685 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/echo.py
+-rw-r--r--   0        0        0    14750 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/instrument.py
+-rw-r--r--   0        0        0    12411 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/mml.py
+-rw-r--r--   0        0        0    16816 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/reduction.py
+-rw-r--r--   0        0        0     1041 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/shared.py
+-rw-r--r--   0        0        0    25691 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/song.py
+-rw-r--r--   0        0        0    18411 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/music_xml/tokens.py
+-rw-r--r--   0        0        0     1759 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/nspc.py
+-rw-r--r--   0        0        0        0 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/py.typed
+-rw-r--r--   0        0        0      204 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/__init__.py
+-rw-r--r--   0        0        0     2559 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/convert.py
+-rw-r--r--   0        0        0     1645 2023-04-28 00:41:15.170135 smw_music-0.3.8/smw_music/scripts/dashboard.py
+-rw-r--r--   0        0        0     7933 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/scripts/filttool.py
+-rw-r--r--   0        0        0      205 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/__init__.py
+-rw-r--r--   0        0        0    57971 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/dashboard.py
+-rw-r--r--   0        0        0     9824 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/dashboard_view.py
+-rw-r--r--   0        0        0     8356 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/envelope_preview.py
+-rw-r--r--   0        0        0     8522 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/keyboard.py
+-rw-r--r--   0        0        0    62892 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/model.py
+-rw-r--r--   0        0        0      205 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/old_save/__init__.py
+-rw-r--r--   0        0        0     6739 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/old_save/v0.py
+-rw-r--r--   0        0        0     4568 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/preferences.py
+-rw-r--r--   0        0        0      852 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/preferences_view.py
+-rw-r--r--   0        0        0    22284 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/quotes.py
+-rw-r--r--   0        0        0     6062 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/sample.py
+-rw-r--r--   0        0        0    12081 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/save.py
+-rw-r--r--   0        0        0     4084 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/state.py
+-rw-r--r--   0        0        0     8040 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/utilization.py
+-rw-r--r--   0        0        0     1261 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/ui/utils.py
+-rw-r--r--   0        0        0     1811 2023-04-28 00:41:15.174135 smw_music-0.3.8/smw_music/utils.py
+-rw-r--r--   0        0        0     6698 1970-01-01 00:00:00.000000 smw_music-0.3.8/PKG-INFO
```

### Comparing `smw_music-0.3.7/README.rst` & `smw_music-0.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/pyproject.toml` & `smw_music-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 filter_files = true
 known_first_party = ["smw_music"]
 known_third_party = ["music21"]
 skip_glob = ["smw_music/doc/"]
 
 [tool.poetry]
 name = "smw_music"
-version = "0.3.7"
+version = "0.3.8"
 description = "Tools for working with SMW Music"
 authors = ["Thomas A. Werne <werneta@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.rst"
 repository = "http://github.com/com-posers-pit/smw_music"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `smw_music-0.3.7/smw_music/__init__.py` & `smw_music-0.3.8/smw_music/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """Top level SMW Music Module."""
 
 ###############################################################################
 # API variable definitions
 ###############################################################################
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 
 ###############################################################################
 # API class definitions
 ###############################################################################
 
 
 class SmwMusicException(Exception):
```

### Comparing `smw_music-0.3.7/smw_music/data/ashtley.gif` & `smw_music-0.3.8/smw_music/data/ashtley.gif`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/data/dashboard.ui` & `smw_music-0.3.8/smw_music/data/dashboard.ui`

 * *Files 2% similar despite different names*

#### Comparing `smw_music-0.3.7/smw_music/data/dashboard.ui` & `smw_music-0.3.8/smw_music/data/dashboard.ui`

```diff
@@ -30,142 +30,142 @@
                     <enum>Qt::Horizontal</enum>
                   </property>
                   <widget class="QGroupBox" name="control_groupBox">
                     <property name="title">
                       <string>Control Panel</string>
                     </property>
                     <layout class="QGridLayout" name="gridLayout">
-                      <item row="0" column="0">
-                        <widget class="QPushButton" name="select_musicxml_fname">
+                      <item row="3" column="0">
+                        <widget class="QLabel" name="game_name_label">
                           <property name="text">
-                            <string>MusicXML</string>
+                            <string>Game:</string>
                           </property>
-                        </widget>
-                      </item>
-                      <item row="10" column="0" colspan="2">
-                        <widget class="QPushButton" name="open_history">
-                          <property name="text">
-                            <string>History</string>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
                           </property>
                         </widget>
                       </item>
                       <item row="1" column="0">
                         <widget class="QPushButton" name="select_mml_fname">
                           <property name="text">
                             <string>MML</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="0" column="1">
-                        <widget class="QLineEdit" name="musicxml_fname"/>
+                      <item row="2" column="0">
+                        <widget class="QLabel" name="porter_name_label">
+                          <property name="text">
+                            <string>Porter:</string>
+                          </property>
+                          <property name="alignment">
+                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                          </property>
+                        </widget>
                       </item>
-                      <item row="11" column="0">
-                        <spacer name="verticalSpacer_2">
-                          <property name="orientation">
-                            <enum>Qt::Vertical</enum>
+                      <item row="9" column="0" colspan="2">
+                        <widget class="QPushButton" name="open_quicklook">
+                          <property name="text">
+                            <string>Open Quicklook</string>
                           </property>
-                          <property name="sizeHint" stdset="0">
-                            <size>
-                              <width>20</width>
-                              <height>40</height>
-                            </size>
+                        </widget>
+                      </item>
+                      <item row="10" column="0" colspan="2">
+                        <widget class="QPushButton" name="open_history">
+                          <property name="text">
+                            <string>History</string>
                           </property>
-                        </spacer>
+                        </widget>
                       </item>
-                      <item row="1" column="1">
-                        <widget class="QLineEdit" name="mml_fname"/>
+                      <item row="5" column="0" colspan="3">
+                        <widget class="QCheckBox" name="superloop_analysis">
+                          <property name="enabled">
+                            <bool>false</bool>
+                          </property>
+                          <property name="text">
+                            <string>Superloop Analysis</string>
+                          </property>
+                        </widget>
                       </item>
                       <item row="7" column="0">
                         <spacer name="control_frame_spacer">
                           <property name="orientation">
                             <enum>Qt::Vertical</enum>
                           </property>
                           <property name="sizeHint" stdset="0">
                             <size>
                               <width>20</width>
                               <height>40</height>
                             </size>
                           </property>
                         </spacer>
                       </item>
-                      <item row="2" column="0">
-                        <widget class="QLabel" name="porter_name_label">
-                          <property name="text">
-                            <string>Porter:</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
-                          </property>
-                        </widget>
-                      </item>
-                      <item row="3" column="1">
-                        <widget class="QLineEdit" name="game_name"/>
+                      <item row="1" column="1">
+                        <widget class="QLineEdit" name="mml_fname"/>
                       </item>
-                      <item row="12" column="0" colspan="2">
-                        <widget class="QPushButton" name="generate_mml">
+                      <item row="6" column="0" colspan="3">
+                        <widget class="QCheckBox" name="measure_numbers">
                           <property name="text">
-                            <string>Generate MML</string>
+                            <string>Measure Numbers</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="2" column="1">
-                        <widget class="QLineEdit" name="porter_name"/>
-                      </item>
-                      <item row="13" column="0" colspan="2">
-                        <widget class="QPushButton" name="generate_spc">
+                      <item row="14" column="0" colspan="2">
+                        <widget class="QPushButton" name="play_spc">
                           <property name="text">
-                            <string>MML → SPC</string>
+                            <string>Play SPC</string>
                           </property>
                         </widget>
                       </item>
                       <item row="4" column="0" colspan="3">
                         <widget class="QCheckBox" name="loop_analysis">
                           <property name="text">
                             <string>Loop Analysis</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="14" column="0" colspan="2">
-                        <widget class="QPushButton" name="play_spc">
-                          <property name="text">
-                            <string>Play SPC</string>
-                          </property>
-                        </widget>
-                      </item>
-                      <item row="5" column="0" colspan="3">
-                        <widget class="QCheckBox" name="superloop_analysis">
-                          <property name="enabled">
-                            <bool>false</bool>
+                      <item row="11" column="0">
+                        <spacer name="verticalSpacer_2">
+                          <property name="orientation">
+                            <enum>Qt::Vertical</enum>
                           </property>
-                          <property name="text">
-                            <string>Superloop Analysis</string>
+                          <property name="sizeHint" stdset="0">
+                            <size>
+                              <width>20</width>
+                              <height>40</height>
+                            </size>
                           </property>
-                        </widget>
+                        </spacer>
                       </item>
-                      <item row="9" column="0" colspan="2">
-                        <widget class="QPushButton" name="open_quicklook">
+                      <item row="13" column="0" colspan="2">
+                        <widget class="QPushButton" name="generate_spc">
                           <property name="text">
-                            <string>Open Quicklook</string>
+                            <string>MML → SPC</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="3" column="0">
-                        <widget class="QLabel" name="game_name_label">
+                      <item row="3" column="1">
+                        <widget class="QLineEdit" name="game_name"/>
+                      </item>
+                      <item row="2" column="1">
+                        <widget class="QLineEdit" name="porter_name"/>
+                      </item>
+                      <item row="0" column="0">
+                        <widget class="QPushButton" name="select_musicxml_fname">
                           <property name="text">
-                            <string>Game:</string>
-                          </property>
-                          <property name="alignment">
-                            <set>Qt::AlignRight|Qt::AlignTrailing|Qt::AlignVCenter</set>
+                            <string>MusicXML</string>
                           </property>
                         </widget>
                       </item>
-                      <item row="6" column="0" colspan="3">
-                        <widget class="QCheckBox" name="measure_numbers">
+                      <item row="0" column="1">
+                        <widget class="QLineEdit" name="musicxml_fname"/>
+                      </item>
+                      <item row="12" column="0" colspan="2">
+                        <widget class="QPushButton" name="generate_mml">
                           <property name="text">
-                            <string>Measure Numbers</string>
+                            <string>Generate MML</string>
                           </property>
                         </widget>
                       </item>
                     </layout>
                   </widget>
                   <widget class="QTabWidget" name="settings_tab_widget">
                     <property name="currentIndex">
@@ -578,15 +578,15 @@
                                                               <property name="maximum">
                                                                 <number>7</number>
                                                               </property>
                                                               <property name="orientation">
                                                                 <enum>Qt::Vertical</enum>
                                                               </property>
                                                               <property name="invertedAppearance">
-                                                                <bool>true</bool>
+                                                                <bool>false</bool>
                                                               </property>
                                                               <property name="invertedControls">
                                                                 <bool>true</bool>
                                                               </property>
                                                             </widget>
                                                           </item>
                                                           <item row="3" column="0">
@@ -597,15 +597,15 @@
                                                               <property name="maximum">
                                                                 <number>31</number>
                                                               </property>
                                                               <property name="orientation">
                                                                 <enum>Qt::Vertical</enum>
                                                               </property>
                                                               <property name="invertedAppearance">
-                                                                <bool>true</bool>
+                                                                <bool>false</bool>
                                                               </property>
                                                               <property name="invertedControls">
                                                                 <bool>true</bool>
                                                               </property>
                                                             </widget>
                                                           </item>
                                                           <item row="3" column="2">
@@ -629,15 +629,15 @@
                                                               <property name="maximum">
                                                                 <number>15</number>
                                                               </property>
                                                               <property name="orientation">
                                                                 <enum>Qt::Vertical</enum>
                                                               </property>
                                                               <property name="invertedAppearance">
-                                                                <bool>true</bool>
+                                                                <bool>false</bool>
                                                               </property>
                                                               <property name="invertedControls">
                                                                 <bool>true</bool>
                                                               </property>
                                                             </widget>
                                                           </item>
                                                           <item row="1" column="0">
@@ -847,72 +847,435 @@
                                                 </layout>
                                               </widget>
                                               <widget class="QWidget" name="tuning_tab">
                                                 <attribute name="title">
                                                   <string>Tuning</string>
                                                 </attribute>
                                                 <layout class="QGridLayout" name="gridLayout_10">
-                                                  <item row="2" column="1">
-                                                    <widget class="QLineEdit" name="subtune_setting"/>
-                                                  </item>
                                                   <item row="1" column="1">
-                                                    <widget class="QSlider" name="subtune_slider">
-                                                      <property name="maximum">
-                                                        <number>255</number>
-                                                      </property>
-                                                      <property name="tracking">
-                                                        <bool>false</bool>
-                                                      </property>
-                                                      <property name="orientation">
-                                                        <enum>Qt::Vertical</enum>
-                                                      </property>
+                                                    <widget class="QWidget" name="tune_control_box" native="true">
+                                                      <layout class="QGridLayout" name="gridLayout_19">
+                                                        <item row="0" column="1">
+                                                          <widget class="QLabel" name="subtune_label">
+                                                            <property name="text">
+                                                              <string>Subtune</string>
+                                                            </property>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="1" column="1">
+                                                          <widget class="QSlider" name="subtune_slider">
+                                                            <property name="maximum">
+                                                              <number>255</number>
+                                                            </property>
+                                                            <property name="tracking">
+                                                              <bool>false</bool>
+                                                            </property>
+                                                            <property name="orientation">
+                                                              <enum>Qt::Vertical</enum>
+                                                            </property>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="0" column="0">
+                                                          <widget class="QLabel" name="tune_label">
+                                                            <property name="text">
+                                                              <string>Tune</string>
+                                                            </property>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="1" column="0">
+                                                          <widget class="QSlider" name="tune_slider">
+                                                            <property name="maximum">
+                                                              <number>255</number>
+                                                            </property>
+                                                            <property name="tracking">
+                                                              <bool>false</bool>
+                                                            </property>
+                                                            <property name="orientation">
+                                                              <enum>Qt::Vertical</enum>
+                                                            </property>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="2" column="1">
+                                                          <widget class="QLineEdit" name="subtune_setting"/>
+                                                        </item>
+                                                        <item row="2" column="0">
+                                                          <widget class="QLineEdit" name="tune_setting"/>
+                                                        </item>
+                                                      </layout>
                                                     </widget>
                                                   </item>
-                                                  <item row="0" column="0">
-                                                    <widget class="QLabel" name="tune_label">
-                                                      <property name="text">
-                                                        <string>Tune</string>
-                                                      </property>
-                                                    </widget>
-                                                  </item>
-                                                  <item row="3" column="0">
-                                                    <widget class="QLabel" name="tune_setting_label">
+                                                  <item row="3" column="3">
+                                                    <widget class="QLabel" name="subtune_setting_label">
                                                       <property name="text">
                                                         <string/>
                                                       </property>
                                                     </widget>
                                                   </item>
-                                                  <item row="2" column="0">
-                                                    <widget class="QLineEdit" name="tune_setting"/>
-                                                  </item>
-                                                  <item row="0" column="1">
-                                                    <widget class="QLabel" name="subtune_label">
-                                                      <property name="text">
-                                                        <string>Subtune</string>
-                                                      </property>
-                                                    </widget>
-                                                  </item>
-                                                  <item row="3" column="1">
-                                                    <widget class="QLabel" name="subtune_setting_label">
+                                                  <item row="3" column="2">
+                                                    <widget class="QLabel" name="tune_setting_label">
                                                       <property name="text">
                                                         <string/>
                                                       </property>
                                                     </widget>
                                                   </item>
                                                   <item row="1" column="0">
-                                                    <widget class="QSlider" name="tune_slider">
-                                                      <property name="maximum">
-                                                        <number>255</number>
-                                                      </property>
-                                                      <property name="tracking">
-                                                        <bool>false</bool>
-                                                      </property>
-                                                      <property name="orientation">
-                                                        <enum>Qt::Vertical</enum>
+                                                    <widget class="QGroupBox" name="tuning_box">
+                                                      <property name="title">
+                                                        <string>Experimental Autotune</string>
                                                       </property>
+                                                      <layout class="QGridLayout" name="gridLayout_20">
+                                                        <item row="0" column="0" colspan="3">
+                                                          <widget class="QGroupBox" name="tuning_input_box">
+                                                            <property name="title">
+                                                              <string>Fundamental</string>
+                                                            </property>
+                                                            <layout class="QGridLayout" name="gridLayout_21">
+                                                              <item row="2" column="2">
+                                                                <widget class="QComboBox" name="tuning_manual_note">
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>C</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>C#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>D</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>D#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>E</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>F</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>F#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>G</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>G#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>A</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>A#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>B</string>
+                                                                    </property>
+                                                                  </item>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="3" column="0">
+                                                                <widget class="QRadioButton" name="tuning_use_manual_freq">
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                  <property name="checkable">
+                                                                    <bool>true</bool>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="2" column="1">
+                                                                <widget class="QLabel" name="tuning_manual_note_label">
+                                                                  <property name="text">
+                                                                    <string>Note</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="2" column="0">
+                                                                <widget class="QRadioButton" name="tuning_use_manual_note">
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="3" column="1">
+                                                                <widget class="QLabel" name="tuning_manual_freq_label">
+                                                                  <property name="text">
+                                                                    <string>Frequency</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="2" column="3">
+                                                                <widget class="QSpinBox" name="tuning_manual_octave">
+                                                                  <property name="value">
+                                                                    <number>4</number>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="0" column="0">
+                                                                <widget class="QRadioButton" name="tuning_use_auto_freq">
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                  <property name="checked">
+                                                                    <bool>true</bool>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="4" column="2" colspan="2">
+                                                                <widget class="QLineEdit" name="tuning_sample_freq">
+                                                                  <property name="text">
+                                                                    <string>32000</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="3" column="2" colspan="2">
+                                                                <widget class="QLineEdit" name="tuning_manual_freq"/>
+                                                              </item>
+                                                              <item row="0" column="1">
+                                                                <widget class="QLabel" name="tuning_auto_label">
+                                                                  <property name="text">
+                                                                    <string>Auto</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="0" column="2" colspan="2">
+                                                                <widget class="QLabel" name="tuning_auto_freq">
+                                                                  <property name="sizePolicy">
+                                                                    <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
+                                                                      <horstretch>0</horstretch>
+                                                                      <verstretch>0</verstretch>
+                                                                    </sizepolicy>
+                                                                  </property>
+                                                                  <property name="minimumSize">
+                                                                    <size>
+                                                                      <width>70</width>
+                                                                      <height>0</height>
+                                                                    </size>
+                                                                  </property>
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="4" column="1">
+                                                                <widget class="QLabel" name="tuning_sample_freq_label">
+                                                                  <property name="text">
+                                                                    <string>Sample Freq.</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="1" column="2" colspan="2">
+                                                                <widget class="QSpinBox" name="tuning_semitone_shift">
+                                                                  <property name="minimum">
+                                                                    <number>-99</number>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="1" column="1">
+                                                                <widget class="QLabel" name="tuning_semitone_shift_label">
+                                                                  <property name="text">
+                                                                    <string>Semitone Shift</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                            </layout>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="7" column="0">
+                                                          <widget class="QPushButton" name="apply_suggested_tune">
+                                                            <property name="text">
+                                                              <string>Apply</string>
+                                                            </property>
+                                                          </widget>
+                                                        </item>
+                                                        <item row="6" column="0">
+                                                          <spacer name="verticalSpacer_7">
+                                                            <property name="orientation">
+                                                              <enum>Qt::Vertical</enum>
+                                                            </property>
+                                                            <property name="sizeHint" stdset="0">
+                                                              <size>
+                                                                <width>20</width>
+                                                                <height>40</height>
+                                                              </size>
+                                                            </property>
+                                                          </spacer>
+                                                        </item>
+                                                        <item row="1" column="0" colspan="3">
+                                                          <widget class="QGroupBox" name="tuning_output_box">
+                                                            <property name="title">
+                                                              <string>Output</string>
+                                                            </property>
+                                                            <layout class="QGridLayout" name="gridLayout_22">
+                                                              <item row="1" column="0">
+                                                                <widget class="QLabel" name="tuning_goal_freq_label">
+                                                                  <property name="text">
+                                                                    <string>Goal</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="2" column="0">
+                                                                <widget class="QLabel" name="tuning_recommended_pitch_label">
+                                                                  <property name="text">
+                                                                    <string>Actual</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="0" column="0">
+                                                                <widget class="QLabel" name="tuning_output_note_label">
+                                                                  <property name="toolTip">
+                                                                    <string>Note that plays when an MML C4 is played</string>
+                                                                  </property>
+                                                                  <property name="text">
+                                                                    <string>Note</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="2" column="1" colspan="2">
+                                                                <widget class="QLabel" name="tuning_recommended_pitch">
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="3" column="1" colspan="2">
+                                                                <widget class="QLabel" name="tuning_recommendation">
+                                                                  <property name="sizePolicy">
+                                                                    <sizepolicy hsizetype="Minimum" vsizetype="Preferred">
+                                                                      <horstretch>0</horstretch>
+                                                                      <verstretch>0</verstretch>
+                                                                    </sizepolicy>
+                                                                  </property>
+                                                                  <property name="minimumSize">
+                                                                    <size>
+                                                                      <width>70</width>
+                                                                      <height>0</height>
+                                                                    </size>
+                                                                  </property>
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="3" column="0">
+                                                                <widget class="QLabel" name="tuning_recommendation_label">
+                                                                  <property name="text">
+                                                                    <string>Tune</string>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="1" column="1" colspan="2">
+                                                                <widget class="QLabel" name="tuning_goal_freq">
+                                                                  <property name="text">
+                                                                    <string/>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="0" column="2">
+                                                                <widget class="QSpinBox" name="tuning_output_octave">
+                                                                  <property name="minimum">
+                                                                    <number>0</number>
+                                                                  </property>
+                                                                  <property name="maximum">
+                                                                    <number>99</number>
+                                                                  </property>
+                                                                  <property name="value">
+                                                                    <number>4</number>
+                                                                  </property>
+                                                                </widget>
+                                                              </item>
+                                                              <item row="0" column="1">
+                                                                <widget class="QComboBox" name="tuning_output_note">
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>C</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>C#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>D</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>D#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>E</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>F</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>F#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>G</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>G#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>A</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>A#</string>
+                                                                    </property>
+                                                                  </item>
+                                                                  <item>
+                                                                    <property name="text">
+                                                                      <string>B</string>
+                                                                    </property>
+                                                                  </item>
+                                                                </widget>
+                                                              </item>
+                                                            </layout>
+                                                          </widget>
+                                                        </item>
+                                                      </layout>
                                                     </widget>
                                                   </item>
                                                 </layout>
                                               </widget>
                                             </widget>
                                           </item>
                                           <item>
@@ -2555,17 +2918,27 @@
     <tabstop>artic_stacc_length_setting</tabstop>
     <tabstop>artic_stacc_volume_slider</tabstop>
     <tabstop>artic_stacc_volume_setting</tabstop>
     <tabstop>artic_accstacc_length_slider</tabstop>
     <tabstop>artic_accstacc_length_setting</tabstop>
     <tabstop>artic_accstacc_volume_slider</tabstop>
     <tabstop>artic_accstacc_volume_setting</tabstop>
+    <tabstop>pan_enable</tabstop>
+    <tabstop>pan_setting</tabstop>
+    <tabstop>pan_l_invert</tabstop>
+    <tabstop>pan_r_invert</tabstop>
+    <tabstop>multisample_unmapped_list</tabstop>
+    <tabstop>multisample_sample_name</tabstop>
+    <tabstop>multisample_sample_notes</tabstop>
+    <tabstop>multisample_sample_notehead</tabstop>
+    <tabstop>multisample_sample_output</tabstop>
+    <tabstop>multisample_sample_add</tabstop>
+    <tabstop>multisample_sample_remove</tabstop>
     <tabstop>global_volume_slider</tabstop>
     <tabstop>global_volume_setting</tabstop>
-    <tabstop>global_legato</tabstop>
     <tabstop>echo_enable</tabstop>
     <tabstop>echo_ch0</tabstop>
     <tabstop>echo_ch1</tabstop>
     <tabstop>echo_ch2</tabstop>
     <tabstop>echo_ch3</tabstop>
     <tabstop>echo_ch4</tabstop>
     <tabstop>echo_ch5</tabstop>
@@ -2580,25 +2953,15 @@
     <tabstop>echo_right_setting</tabstop>
     <tabstop>echo_right_surround</tabstop>
     <tabstop>echo_feedback_slider</tabstop>
     <tabstop>echo_feedback_setting</tabstop>
     <tabstop>echo_feedback_surround</tabstop>
     <tabstop>echo_delay_slider</tabstop>
     <tabstop>echo_delay_setting</tabstop>
-    <tabstop>pan_l_invert</tabstop>
-    <tabstop>pan_r_invert</tabstop>
-    <tabstop>pan_setting</tabstop>
-    <tabstop>pan_enable</tabstop>
-    <tabstop>multisample_sample_remove</tabstop>
-    <tabstop>multisample_unmapped_list</tabstop>
-    <tabstop>multisample_sample_name</tabstop>
-    <tabstop>multisample_sample_notes</tabstop>
-    <tabstop>multisample_sample_notehead</tabstop>
-    <tabstop>multisample_sample_output</tabstop>
-    <tabstop>multisample_sample_add</tabstop>
+    <tabstop>global_legato</tabstop>
     <tabstop>start_measure</tabstop>
     <tabstop>reload_musicxml</tabstop>
     <tabstop>generate_and_play</tabstop>
     <tabstop>render_zip</tabstop>
   </tabstops>
   <resources/>
   <connections/>
```

### Comparing `smw_music-0.3.7/smw_music/data/maestro.svg` & `smw_music-0.3.8/smw_music/data/maestro.svg`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/data/mml.txt` & `smw_music-0.3.8/smw_music/data/mml.txt`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/data/preferences.ui` & `smw_music-0.3.8/smw_music/data/preferences.ui`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/log.py` & `smw_music-0.3.8/smw_music/log.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/channel.py` & `smw_music-0.3.8/smw_music/music_xml/channel.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/echo.py` & `smw_music-0.3.8/smw_music/music_xml/echo.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/instrument.py` & `smw_music-0.3.8/smw_music/music_xml/instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from functools import cache
 from pathlib import Path
 
 # Library imports
 from music21.pitch import Pitch
 
 # Package imports
+from smw_music.brr import SAMPLE_FREQ
 from smw_music.music_xml.tokens import Note
 from smw_music.utils import hexb
 
 ###############################################################################
 # Private variable definitions
 ###############################################################################
 
@@ -149,14 +150,36 @@
     BRR = auto()
     OVERRIDE = auto()
 
 
 ###############################################################################
 
 
+class TuneSource(IntEnum):
+    AUTO = auto()
+    MANUAL_NOTE = auto()
+    MANUAL_FREQ = auto()
+
+
+###############################################################################
+
+
+@dataclass
+class Tuning:
+    source: TuneSource = TuneSource.AUTO
+    semitone_shift: int = 0
+    pitch: Pitch = field(default_factory=lambda: Pitch("C", octave=4))
+    frequency: float = Pitch("C", octave=4).frequency
+    sample_freq: float = SAMPLE_FREQ
+    output: Pitch = field(default_factory=lambda: Pitch("C", octave=4))
+
+
+###############################################################################
+
+
 @dataclass
 class InstrumentSample:
     default_octave: int = 3
     octave_shift: int = -1
     dynamics: dict[Dynamics, int] = field(
         default_factory=lambda: {
             Dynamics.PPPP: 26,
@@ -199,14 +222,15 @@
     subtune_setting: int = 0
     mute: bool = False
     solo: bool = False
     llim: Pitch = field(default_factory=lambda: Pitch("A", octave=0))
     ulim: Pitch = field(default_factory=lambda: Pitch("C", octave=7))
     notehead: NoteHead = NoteHead.NORMAL
     start: Pitch = field(default_factory=lambda: Pitch("A", octave=0))
+    tuning: Tuning = field(default_factory=Tuning)
 
     _instrument_idx: int = field(default=0, init=False)
 
     ###########################################################################
     # API method definitions
     ###########################################################################
```

### Comparing `smw_music-0.3.7/smw_music/music_xml/mml.py` & `smw_music-0.3.8/smw_music/music_xml/mml.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/reduction.py` & `smw_music-0.3.8/smw_music/music_xml/reduction.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/shared.py` & `smw_music-0.3.8/smw_music/music_xml/shared.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/song.py` & `smw_music-0.3.8/smw_music/music_xml/song.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/music_xml/tokens.py` & `smw_music-0.3.8/smw_music/music_xml/tokens.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/scripts/convert.py` & `smw_music-0.3.8/smw_music/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/scripts/dashboard.py` & `smw_music-0.3.8/smw_music/scripts/dashboard.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/scripts/filttool.py` & `smw_music-0.3.8/smw_music/scripts/filttool.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/dashboard.py` & `smw_music-0.3.8/smw_music/ui/dashboard.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,15 @@
 from typing import Callable, NamedTuple, cast
 
 # Library imports
 import qdarkstyle  # type: ignore
 from music21.pitch import Pitch
 from PyQt6 import uic
 from PyQt6.QtCore import QEvent, QModelIndex, QObject, QSignalBlocker, Qt
-from PyQt6.QtGui import (
-    QAction,
-    QColor,
-    QFont,
-    QIcon,
-    QKeyEvent,
-    QMovie,
-    QPainter,
-    QPixmap,
-)
+from PyQt6.QtGui import QAction, QFont, QIcon, QKeyEvent, QMovie, QPixmap
 from PyQt6.QtWidgets import (
     QAbstractSlider,
     QApplication,
     QCheckBox,
     QComboBox,
     QFileDialog,
     QLabel,
@@ -57,15 +48,15 @@
 )
 
 # Package imports
 from smw_music import __version__
 from smw_music.music_xml.echo import EchoCh
 from smw_music.music_xml.instrument import Artic
 from smw_music.music_xml.instrument import Dynamics as Dyn
-from smw_music.music_xml.instrument import GainMode, SampleSource
+from smw_music.music_xml.instrument import GainMode, SampleSource, TuneSource
 from smw_music.ui.dashboard_view import DashboardView
 from smw_music.ui.envelope_preview import EnvelopePreview
 from smw_music.ui.model import Model
 from smw_music.ui.preferences import Preferences
 from smw_music.ui.quotes import labeouf
 from smw_music.ui.sample import SamplePack
 from smw_music.ui.state import NoSample, State
@@ -132,14 +123,18 @@
         Qt.Key.Key_Right,
         Qt.Key.Key_B,
         Qt.Key.Key_A,
     ]
 )
 
 ###############################################################################
+
+_REV_KONAMI = deque(reversed(_KONAMI))
+
+###############################################################################
 # Private class definitions
 ###############################################################################
 
 
 class _ArticWidgets(NamedTuple):
     length_slider: QSlider
     length_setting: QLineEdit
@@ -189,14 +184,15 @@
 ###############################################################################
 
 
 class Dashboard(QWidget):
     _history: QMainWindow
     _quicklook: QMainWindow
     _checkitout: QMainWindow
+    _camelitout: QMainWindow
     _envelope_preview: EnvelopePreview
     _extension = "prj"
     _model: Model
     _preferences: Preferences
     _view: DashboardView
     _dyn_widgets: dict[Dyn, _DynamicsWidgets]
     _artic_widgets: dict[Artic, _ArticWidgets]
@@ -253,14 +249,23 @@
         label = QLabel(self)
         movie = QMovie(parent=self)
         movie.setFileName(str(data_lib / "ashtley.gif"))
         label.setMovie(movie)
         movie.start()
         self._checkitout.setCentralWidget(label)
 
+        self._camelitout = QMainWindow(parent=self)
+        self._camelitout.setWindowTitle("Camel by camel")
+        label = QLabel(self)
+        movie = QMovie(parent=self)
+        movie.setFileName(str(data_lib / "ankha.gif"))
+        label.setMovie(movie)
+        movie.start()
+        self._camelitout.setCentralWidget(label)
+
         self._history = QMainWindow(parent=self)
         self._history.setWindowTitle("Action history")
         self._history.setMinimumSize(800, 600)
         self._history.setCentralWidget(QListWidget())
 
         self._envelope_preview = EnvelopePreview(self)
         self._history.setWindowTitle("History")
@@ -325,14 +330,16 @@
                     else:
                         event.accept()
                 return True
             case QEvent.Type.KeyRelease:
                 self._keyhist.append(cast(QKeyEvent, event).key())
                 if self._keyhist == _KONAMI:
                     self._checkitout.show()
+                elif self._keyhist == _REV_KONAMI:
+                    self._camelitout.show()
 
         return super().eventFilter(obj, event)
 
     ###########################################################################
     # API slot definitions
     ###########################################################################
 
@@ -428,14 +435,28 @@
         self._setup_utilization(dark_mode)
 
         # advance_enabled handling
         v.generate_mml.setVisible(advanced_enabled)
         v.generate_spc.setVisible(advanced_enabled)
         v.play_spc.setVisible(advanced_enabled)
         v.other_settings_box.setVisible(advanced_enabled)
+        v.tuning_use_auto_freq.setVisible(advanced_enabled)
+        v.tuning_use_manual_note.setVisible(advanced_enabled)
+        v.tuning_manual_note_label.setVisible(advanced_enabled)
+        v.tuning_manual_note.setVisible(advanced_enabled)
+        v.tuning_manual_octave.setVisible(advanced_enabled)
+        v.tuning_use_manual_freq.setVisible(advanced_enabled)
+        v.tuning_manual_freq_label.setVisible(advanced_enabled)
+        v.tuning_manual_freq.setVisible(advanced_enabled)
+        v.tuning_sample_freq_label.setVisible(advanced_enabled)
+        v.tuning_sample_freq.setVisible(advanced_enabled)
+        v.tuning_output_note.setVisible(advanced_enabled)
+        v.tuning_output_note_label.setText(
+            "Note" if advanced_enabled else "Octave"
+        )
 
         # amk_valid handling
         for action in [
             v.new_project,
             v.open_project,
             v.save_project,
             v.menuRecent_Projects,
@@ -574,14 +595,37 @@
 
             self._update_solomute(state)
             self._update_multisample(state)
 
             with suppress(NoSample):
                 if state.sample.sample_source == SampleSource.BUILTIN:
                     v.sample_pack_list.clearSelection()
+                tuning = state.sample.tuning
+                v.tuning_use_auto_freq.setChecked(
+                    tuning.source == TuneSource.AUTO
+                )
+                v.tuning_use_manual_freq.setChecked(
+                    tuning.source == TuneSource.MANUAL_FREQ
+                )
+                v.tuning_use_manual_note.setChecked(
+                    tuning.source == TuneSource.MANUAL_NOTE
+                )
+                v.tuning_semitone_shift.setValue(tuning.semitone_shift)
+                v.tuning_manual_note.setCurrentIndex(tuning.pitch.pitchClass)
+                v.tuning_manual_octave.setValue(tuning.pitch.octave)
+                v.tuning_manual_freq.setText(f"{tuning.frequency:.2f}")
+                v.tuning_sample_freq.setText(f"{tuning.sample_freq:.2f}")
+
+                freq, (setting, actual) = state.calculated_tune
+                v.tuning_auto_freq.setText(f"{freq:.2f}Hz")
+                freq = tuning.output.frequency
+                v.tuning_goal_freq.setText(f"{freq:.2f}Hz")
+                tune, subtune = divmod(setting, 256)
+                v.tuning_recommended_pitch.setText(f"{actual:.2f}Hz")
+                v.tuning_recommendation.setText(f"${tune:02x} ${subtune:02x}")
 
             # Global settings
             v.global_volume_slider.setValue(state.global_volume)
             v.global_volume_setting.setText(pct(state.global_volume))
             v.global_volume_setting_label.setText(hexb(state.global_volume))
             v.global_legato.setChecked(state.global_legato)
 
@@ -738,14 +782,25 @@
             (v.attack_setting, m.on_attack_changed),
             (v.decay_slider, m.on_decay_changed),
             (v.decay_setting, m.on_decay_changed),
             (v.sus_level_slider, m.on_sus_level_changed),
             (v.sus_level_setting, m.on_sus_level_changed),
             (v.sus_rate_slider, m.on_sus_rate_changed),
             (v.sus_rate_setting, m.on_sus_rate_changed),
+            (v.tuning_use_auto_freq, m.on_tuning_use_auto_freq_selected),
+            (v.tuning_use_manual_freq, m.on_tuning_use_manual_freq_selected),
+            (v.tuning_use_manual_note, m.on_tuning_use_manual_note_selected),
+            (v.tuning_semitone_shift, m.on_tuning_semitone_shift_changed),
+            (v.tuning_manual_freq, m.on_tuning_manual_freq_changed),
+            (v.tuning_manual_note, self._on_tuning_manual_note_changed),
+            (v.tuning_manual_octave, self._on_tuning_manual_octave_changed),
+            (v.tuning_sample_freq, m.on_tuning_sample_freq_changed),
+            (v.tuning_output_note, self._on_tuning_output_note_changed),
+            (v.tuning_output_octave, self._on_tuning_output_octave_changed),
+            (v.apply_suggested_tune, m.on_apply_suggested_tune_clicked),
             (v.tune_slider, m.on_tune_changed),
             (v.tune_setting, m.on_tune_changed),
             (v.subtune_slider, m.on_subtune_changed),
             (v.subtune_setting, m.on_subtune_changed),
             (v.brr_setting, m.on_brr_setting_changed),
             (v.preview_envelope, self.on_preview_envelope_clicked),
             # Global settings
@@ -1016,14 +1071,38 @@
         sample = item.data(_TblCol.NAME, Qt.ItemDataRole.UserRole)
 
         solo = col == _TblCol.SOLO
         self._model.on_solomute_changed(sample, solo, checked)
 
     ###########################################################################
 
+    def _on_tuning_manual_note_changed(self, pitch_class: int) -> None:
+        octave = self._view.tuning_manual_octave.value()
+        self._model.on_tuning_manual_note_changed(pitch_class, octave)
+
+    ###########################################################################
+
+    def _on_tuning_manual_octave_changed(self, octave: int) -> None:
+        pitch_class = self._view.tuning_manual_note.currentIndex()
+        self._model.on_tuning_manual_note_changed(pitch_class, octave)
+
+    ###########################################################################
+
+    def _on_tuning_output_note_changed(self, pitch_class: int) -> None:
+        octave = self._view.tuning_output_octave.value()
+        self._model.on_tuning_output_note_changed(pitch_class, octave)
+
+    ###########################################################################
+
+    def _on_tuning_output_octave_changed(self, octave: int) -> None:
+        pitch_class = self._view.tuning_output_note.currentIndex()
+        self._model.on_tuning_output_note_changed(pitch_class, octave)
+
+    ###########################################################################
+
     def _open_project(self) -> None:
         fname, _ = QFileDialog.getOpenFileName(
             self._view, "Project File", filter=f"*.{self._extension}"
         )
         if fname:
             self._model.on_load(Path(fname))
```

### Comparing `smw_music-0.3.7/smw_music/ui/dashboard_view.py` & `smw_music-0.3.8/smw_music/ui/dashboard_view.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     QWidget,
 )
 
 
 class DashboardView(QMainWindow):
     actionClearRecentProjects: QAction
     adsr_box: QFrame
+    apply_suggested_tune: QPushButton
     artic_acc_group: QGroupBox
     artic_acc_length_label: QLabel
     artic_acc_length_setting: QLineEdit
     artic_acc_length_slider: QSlider
     artic_acc_setting_label: QLabel
     artic_acc_volume_label: QLabel
     artic_acc_volume_setting: QLineEdit
@@ -279,19 +280,46 @@
     sus_level_label: QLabel
     sus_level_setting: QLineEdit
     sus_level_slider: QSlider
     sus_rate_eu_label: QLabel
     sus_rate_label: QLabel
     sus_rate_setting: QLineEdit
     sus_rate_slider: QSlider
+    tune_control_box: QWidget
     tune_label: QLabel
     tune_setting: QLineEdit
     tune_setting_label: QLabel
     tune_slider: QSlider
+    tuning_auto_freq: QLabel
+    tuning_auto_label: QLabel
+    tuning_box: QGroupBox
+    tuning_goal_freq: QLabel
+    tuning_goal_freq_label: QLabel
+    tuning_input_box: QGroupBox
+    tuning_manual_freq: QLineEdit
+    tuning_manual_freq_label: QLabel
+    tuning_manual_note: QComboBox
+    tuning_manual_note_label: QLabel
+    tuning_manual_octave: QSpinBox
+    tuning_output_box: QGroupBox
+    tuning_output_note: QComboBox
+    tuning_output_note_label: QLabel
+    tuning_output_octave: QSpinBox
+    tuning_recommendation: QLabel
+    tuning_recommendation_label: QLabel
+    tuning_recommended_pitch: QLabel
+    tuning_recommended_pitch_label: QLabel
+    tuning_sample_freq: QLineEdit
+    tuning_sample_freq_label: QLabel
+    tuning_semitone_shift: QSpinBox
+    tuning_semitone_shift_label: QLabel
     tuning_tab: QWidget
+    tuning_use_auto_freq: QRadioButton
+    tuning_use_manual_freq: QRadioButton
+    tuning_use_manual_note: QRadioButton
     undo: QAction
     utilization: QLabel
     utilization_echo: QLabel
     utilization_engine: QLabel
     utilization_frame: QFrame
     utilization_pct_free: QLabel
     utilization_samples: QLabel
```

### Comparing `smw_music-0.3.7/smw_music/ui/envelope_preview.py` & `smw_music-0.3.8/smw_music/ui/envelope_preview.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/keyboard.py` & `smw_music-0.3.8/smw_music/ui/keyboard.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/model.py` & `smw_music-0.3.8/smw_music/ui/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,26 +30,29 @@
 import yaml
 from mako.template import Template  # type: ignore
 from music21.pitch import Pitch, PitchException
 from PyQt6.QtCore import QObject, pyqtSignal
 from watchdog import events, observers
 
 # Package imports
-from smw_music import SmwMusicException, __version__
+from smw_music import SmwMusicException, __version__, nspc
+from smw_music.brr import SAMPLE_FREQ, Brr
 from smw_music.music_xml import MusicXmlException
 from smw_music.music_xml.echo import EchoCh, EchoConfig
 from smw_music.music_xml.instrument import (
     Artic,
     ArticSetting,
     Dynamics,
     GainMode,
     InstrumentConfig,
     InstrumentSample,
     NoteHead,
     SampleSource,
+    TuneSource,
+    Tuning,
 )
 from smw_music.music_xml.song import Song
 from smw_music.ui.quotes import ashtley, quotes
 from smw_music.ui.sample import SamplePack
 from smw_music.ui.save import load, save
 from smw_music.ui.state import NoSample, PreferencesState, State
 from smw_music.ui.utilization import (
@@ -329,14 +332,22 @@
     def update_status(self, msg: str) -> None:
         self.status_updated.emit(msg)
 
     ###########################################################################
     # API slot definitions
     ###########################################################################
 
+    def on_apply_suggested_tune_clicked(self) -> None:
+        setting = self.state.calculated_tune[1][0]
+        tune, subtune = divmod(setting, 256)
+        self._update_sample_state(tune_setting=tune, subtune_setting=subtune)
+        self.update_status(f"Tune setting set to {tune}.{subtune}")
+
+    ###########################################################################
+
     def on_artic_length_changed(self, artic: Artic, val: int | str) -> None:
         max_len = 7
         with suppress(NoSample):
             artics = deepcopy(self.state.sample.artics)
             artics[artic].length = _parse_setting(val, max_len)
             self._update_sample_state(artics=artics)
             self.update_status(f"{artic} length set to {val}")
@@ -945,14 +956,95 @@
     def on_tune_changed(self, val: int | str) -> None:
         setting = _parse_setting(val)
         self._update_sample_state(tune_setting=setting)
         self.update_status(f"Tune set to {setting}")
 
     ###########################################################################
 
+    def on_tuning_sample_freq_changed(self, setting: str) -> None:
+        with suppress(ValueError, NoSample):
+            freq = float(setting)
+            tuning = replace(self.state.sample.tuning, sample_freq=freq)
+            self._update_sample_state(tuning=tuning)
+            self.update_status(f"Using sampling frequency {freq}Hz")
+
+    ###########################################################################
+
+    def on_tuning_manual_freq_changed(self, setting: str) -> None:
+        with suppress(ValueError, NoSample):
+            freq = float(setting)
+            tuning = replace(self.state.sample.tuning, frequency=freq)
+            self._update_sample_state(tuning=tuning)
+            self.update_status(f"Using manual tuning frequency {freq}Hz")
+
+    ###########################################################################
+
+    def on_tuning_manual_note_changed(
+        self, pitch_class: int, octave: int
+    ) -> None:
+        with suppress(NoSample):
+            pitch = Pitch(octave=octave, pitchClass=pitch_class)
+            tuning = replace(self.state.sample.tuning, pitch=pitch)
+            self._update_sample_state(tuning=tuning)
+            self.update_status(f"Target pitch set to {pitch.nameWithOctave}")
+
+    ###########################################################################
+
+    def on_tuning_output_note_changed(
+        self, pitch_class: int, octave: int
+    ) -> None:
+        with suppress(NoSample):
+            pitch = Pitch(octave=octave, pitchClass=pitch_class)
+            tuning = replace(self.state.sample.tuning, output=pitch)
+            self._update_sample_state(tuning=tuning)
+            self.update_status(f"Target output set to {pitch.nameWithOctave}")
+
+    ###########################################################################
+
+    def on_tuning_semitone_shift_changed(self, shift: int) -> None:
+        with suppress(NoSample):
+            tuning = replace(self.state.sample.tuning, semitone_shift=shift)
+            self._update_sample_state(tuning=tuning)
+            self.update_status(f"Set semitone shift to {shift}")
+
+    ###########################################################################
+
+    def on_tuning_use_auto_freq_selected(self, state: bool) -> None:
+        with suppress(NoSample):
+            if state:
+                tuning = replace(
+                    self.state.sample.tuning, source=TuneSource.AUTO
+                )
+                self._update_sample_state(tuning=tuning)
+                self.update_status("Using auto frequency tuning")
+
+    ###########################################################################
+
+    def on_tuning_use_manual_freq_selected(self, state: bool) -> None:
+        with suppress(NoSample):
+            if state:
+                tuning = replace(
+                    self.state.sample.tuning, source=TuneSource.MANUAL_FREQ
+                )
+                self._update_sample_state(tuning=tuning)
+                self.update_status("Using manual frequency tuning")
+
+    ###########################################################################
+
+    def on_tuning_use_manual_note_selected(self, state: bool) -> None:
+        with suppress(NoSample):
+            if state:
+                tuning = replace(
+                    self.state.sample.tuning, source=TuneSource.MANUAL_NOTE
+                )
+                self._update_sample_state(tuning=tuning)
+                self.update_status("Using manual note tuning")
+
+    ###########################################################################
+
     def on_undo_clicked(self) -> None:
         if self._undo_level < len(self._history) - 1:
             self._undo_level += 1
             self._signal_state_change(update_aram_util=False)
             self.update_status("Undo")
 
     ###########################################################################
@@ -1101,18 +1193,16 @@
         state = self.state
 
         # All the inputs need to be present to continue
         if not all([name, notes, notehead, output]):
             return
 
         # Make sure we've got an instrument selected
-        try:
+        with suppress(NoSample):
             sample = state.sample
-        except NoSample:
-            return
 
         # Exit if we're trying to change a sample that doesn't exist (this can
         # happen when tabbing through and entering values before adding it
         if not new and name not in state.instrument.multisamples:
             return
 
         # Parse the input parameters and bail if something went wrong
@@ -1319,14 +1409,55 @@
         state = self.state
 
         state.unsaved = state_change
         self.state.unmapped = set()
 
         self._update_aram_util()
 
+        brr: Brr | None = None
+        with suppress(NoSample):
+            sample = self.state.sample
+            if sample.sample_source == SampleSource.SAMPLEPACK:
+                pack, path = sample.pack_sample
+                brr = self._sample_packs[pack][path].brr
+
+            else:
+
+                with suppress(FileNotFoundError):
+                    brr = Brr.from_file(sample.brr_fname)
+
+        if brr is not None:
+            tuning = self.state.sample.tuning
+            scale = SAMPLE_FREQ / tuning.sample_freq
+            source = tuning.source
+
+            # When not in advanced mode, always use auto tuning
+            if not self.preferences.advanced_mode:
+                source = TuneSource.AUTO
+
+            match source:
+                case TuneSource.AUTO:
+                    fundamental = brr.fundamental
+                    fundamental /= 2 ** (tuning.semitone_shift / 12)
+                case TuneSource.MANUAL_NOTE:
+                    fundamental = tuning.pitch.frequency * scale
+                case TuneSource.MANUAL_FREQ:
+                    fundamental = tuning.frequency * scale
+
+            self.state.calculated_tune = (
+                brr.fundamental,
+                brr.tune(
+                    nspc.midi_to_nspc(Pitch("C", octave=4).midi),
+                    tuning.output.frequency,
+                    fundamental,
+                ),
+            )
+        else:
+            self.state.calculated_tune = (0, (0, 0))
+
         with suppress(NoSample):
             if self.song:
                 name = state.sample_idx[0]
 
                 unmapped = self.song.unmapped_notes(
                     name, state.instruments[name]
                 )
@@ -1377,15 +1508,16 @@
         | dict[Artic, ArticSetting]
         | set[Dynamics]
         | bool
         | SampleSource
         | tuple[str, Path]
         | tuple[bool, bool]
         | Path
-        | GainMode,
+        | GainMode
+        | Tuning,
     ) -> None:
         with suppress(NoSample):
             old_sample = self.state.sample
             new_sample = replace(old_sample)
             for key, val in kwargs.items():
                 setattr(new_sample, key, val)
 
@@ -1561,7 +1693,9 @@
         return total_size
 
     ###########################################################################
 
     @property
     def state(self) -> State:
         return self._history[-1 - self._undo_level]
+
+    ###########################################################################
```

### Comparing `smw_music-0.3.7/smw_music/ui/old_save/v0.py` & `smw_music-0.3.8/smw_music/ui/old_save/v0.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/preferences.py` & `smw_music-0.3.8/smw_music/ui/preferences.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/preferences_view.py` & `smw_music-0.3.8/smw_music/ui/preferences_view.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/quotes.py` & `smw_music-0.3.8/smw_music/ui/quotes.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/sample.py` & `smw_music-0.3.8/smw_music/ui/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,34 +7,42 @@
 
 ###############################################################################
 # Imports
 ###############################################################################
 
 # Standard library imports
 from dataclasses import dataclass
+from functools import cached_property
 from glob import glob
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import TextIO
 from zipfile import ZipFile
 
 # Package imports
+from smw_music.brr import Brr
 from smw_music.music_xml.instrument import GainMode
 
 ###############################################################################
 # API Class Definitions
 ###############################################################################
 
 
 @dataclass
 class Sample:
     path: Path
     params: "SampleParams"
     data: bytes
 
+    ###########################################################################
+
+    @cached_property
+    def brr(self) -> Brr:
+        return Brr.from_binary(self.data)
+
 
 ###############################################################################
 
 
 @dataclass
 class SamplePack:
     path: Path
```

### Comparing `smw_music-0.3.7/smw_music/ui/save.py` & `smw_music-0.3.8/smw_music/ui/save.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,14 +278,32 @@
     assert save_version == 0
     state = v0.load(fname)
 
     return state, backup
 
 
 ###############################################################################
+
+
+def _update_convert_scripts(dirname: Path) -> None:
+    for fname in ["convert.bat", "convert.sh"]:
+        fpath = dirname / fname
+
+        with open(fpath, "r", encoding="utf8") as fobj:
+            lines = fobj.readlines()
+
+        if "-visualize" not in lines[-1]:
+            split = lines[-1].split('"')
+            split[0] += "-visualize "
+            lines[-1] = '"'.join(split)
+            with open(fpath, "w", encoding="utf8") as fobj:
+                fobj.write("".join(lines))
+
+
+###############################################################################
 # API function definitions
 ###############################################################################
 
 
 def load(fname: Path) -> tuple[State, Path | None]:
     rv: tuple[State, Path | None]
 
@@ -299,14 +317,15 @@
             + f"supports up to {_CURRENT_SAVE_VERSION}"
         )
 
     # Visualization support added in the middle of support for v1 version
     # files, so we should try to add it
     if save_version <= 1:
         make_vis_dir(fname.parent)
+        _update_convert_scripts(fname.parent)
 
     if save_version < _CURRENT_SAVE_VERSION:
         rv = _upgrade_save(fname)
     else:
         project = contents["song"]
         sdict = contents["state"]
         musicxml = sdict["musicxml_fname"]
```

### Comparing `smw_music-0.3.7/smw_music/ui/state.py` & `smw_music-0.3.8/smw_music/ui/state.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     start_measure: int = 1
 
     _sample_idx: tuple[str, str] | None = None
 
     unmapped: set[tuple[Pitch, str]] = field(default_factory=set)
     aram_util: Utilization = field(default_factory=default_utilization)
     aram_custom_sample_b: int = 0
+    calculated_tune: tuple[float, tuple[int, float]] = (0, (0, 0))
 
     ###########################################################################
     # Property definitions
     ###########################################################################
 
     @property
     def instrument(self) -> InstrumentConfig:
```

### Comparing `smw_music-0.3.7/smw_music/ui/utilization.py` & `smw_music-0.3.8/smw_music/ui/utilization.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/ui/utils.py` & `smw_music-0.3.8/smw_music/ui/utils.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/smw_music/utils.py` & `smw_music-0.3.8/smw_music/utils.py`

 * *Files identical despite different names*

### Comparing `smw_music-0.3.7/PKG-INFO` & `smw_music-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smw-music
-Version: 0.3.7
+Version: 0.3.8
 Summary: Tools for working with SMW Music
 Home-page: http://github.com/com-posers-pit/smw_music
 License: AGPL-3.0-only
 Author: Thomas A. Werne
 Author-email: werneta@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
```

