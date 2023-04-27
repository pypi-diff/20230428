# Comparing `tmp/scrappo-1.0.0.tar.gz` & `tmp/scrappo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrappo-1.0.0.tar", last modified: Sun Apr 16 15:10:03 2023, max compression
+gzip compressed data, was "scrappo-1.1.0.tar", last modified: Thu Apr 27 23:26:57 2023, max compression
```

## Comparing `scrappo-1.0.0.tar` & `scrappo-1.1.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.691235 scrappo-1.0.0/
--rw-rw-rw-   0        0        0     1081 2023-04-15 11:00:10.000000 scrappo-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     7041 2023-04-16 15:10:03.688242 scrappo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6346 2023-04-16 14:36:31.000000 scrappo-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.611447 scrappo-1.0.0/scrappo/
--rw-rw-rw-   0        0        0        0 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/__init__.py
--rw-rw-rw-   0        0        0      466 2023-04-16 14:35:49.000000 scrappo-1.0.0/scrappo/app.py
--rw-rw-rw-   0        0        0      872 2023-04-16 12:14:51.000000 scrappo-1.0.0/scrappo/downloader.py
--rw-rw-rw-   0        0        0      983 2023-04-16 11:41:45.000000 scrappo-1.0.0/scrappo/movies.py
--rw-rw-rw-   0        0        0     1077 2023-04-16 12:10:41.000000 scrappo-1.0.0/scrappo/processor.py
--rw-rw-rw-   0        0        0      993 2023-04-16 12:12:37.000000 scrappo-1.0.0/scrappo/series.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.643363 scrappo-1.0.0/scrappo/settings/
--rw-rw-rw-   0        0        0        0 2023-04-15 10:37:58.000000 scrappo-1.0.0/scrappo/settings/__init__.py
--rw-rw-rw-   0        0        0      983 2023-04-15 11:07:19.000000 scrappo-1.0.0/scrappo/settings/manager.py
--rw-rw-rw-   0        0        0     4599 2023-04-16 14:37:10.000000 scrappo-1.0.0/scrappo/settings/settings.py
--rw-rw-rw-   0        0        0     1662 2023-04-16 12:04:08.000000 scrappo-1.0.0/scrappo/url_parser.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.676274 scrappo-1.0.0/scrappo/utils/
--rw-rw-rw-   0        0        0        0 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/__init__.py
--rw-rw-rw-   0        0        0      622 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/bytes_conversion.py
--rw-rw-rw-   0        0        0     2615 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/date.py
--rw-rw-rw-   0        0        0      937 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/directory.py
--rw-rw-rw-   0        0        0      634 2023-04-15 13:43:07.000000 scrappo-1.0.0/scrappo/utils/file.py
--rw-rw-rw-   0        0        0      355 2023-04-15 22:32:03.000000 scrappo-1.0.0/scrappo/utils/log.py
--rw-rw-rw-   0        0        0      459 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/reflection.py
--rw-rw-rw-   0        0        0     1269 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/split_string.py
--rw-rw-rw-   0        0        0      300 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/utils/yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.685250 scrappo-1.0.0/scrappo/version/
--rw-rw-rw-   0        0        0        0 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/version/__init__.py
--rw-rw-rw-   0        0        0      293 2023-04-15 11:00:10.000000 scrappo-1.0.0/scrappo/version/progsettings.py
--rw-rw-rw-   0        0        0       27 2023-04-16 15:09:33.000000 scrappo-1.0.0/scrappo/version/progsettings.yaml
--rw-rw-rw-   0        0        0     1127 2023-04-16 12:07:39.000000 scrappo-1.0.0/scrappo/video.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:10:03.634386 scrappo-1.0.0/scrappo.egg-info/
--rw-rw-rw-   0        0        0     7041 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      779 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 15:10:03.000000 scrappo-1.0.0/scrappo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:10:03.692233 scrappo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1420 2023-04-16 15:06:20.000000 scrappo-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-27 23:26:42.000000 scrappo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 23:26:57.667125 scrappo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-04-27 23:26:42.000000 scrappo-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/movies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/url_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/scrappo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/bytes_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/split_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.667125 scrappo-1.1.0/scrappo/version/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/progsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/version/progsettings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-27 23:26:42.000000 scrappo-1.1.0/scrappo/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:26:57.663125 scrappo-1.1.0/scrappo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-27 23:26:57.000000 scrappo-1.1.0/scrappo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 23:26:57.667125 scrappo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-04-27 23:26:42.000000 scrappo-1.1.0/setup.py
```

### Comparing `scrappo-1.0.0/LICENSE` & `scrappo-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 zay
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 zay
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `scrappo-1.0.0/PKG-INFO` & `scrappo-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,155 +1,156 @@
-Metadata-Version: 2.1
-Name: scrappo
-Version: 1.0.0
-Summary: Download any video from a specific URL.
-Home-page: https://github.com/zaytiri/scrappo
-Author: zaytiri
-Project-URL: GitHub, https://github.com/zaytiri/scrappo
-Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
-Keywords: video,download,tool,scrapping,scrap,cli,url python
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
-
-# Scrappo - Video Downloader Tool
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
-
-It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                           |
-|:----------------------------------------------------------------------------------|
-| can be input a .txt file containing a list of URLs                                |
-| download movies, series or related content                                        |
-| series will be separate into season folders                                       |
-| movies can also be separated in their own folder                                  |
-| videos already downloaded will be skipped                                         |
-| any errors regarding the videos will not stop program and will appear in the end. |
-
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```
-pip --no-cache-dir install scrappo
-```
-
-or,
-
-```
-pip3 --no-cache-dir install scrappo
-```
-<a name="usage"></a>
-## Usage
-
-| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
-|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
-| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
-| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
-| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
-| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
-| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
-
----
-### Important
-
-#### URLs .txt file
-The file containing a list of URLs must obey to certain requirements.
-
-```text
-nameOfVideo1:::https://someurl.withavideo.org//video1
-nameOfVideo2:::https://someurl.withavideo.org//video2
-https://someurl.withavideo.org//video3
-https://someurl.withavideo.org//video4
-nameOfVideo5:::https://someurl.withavideo.org//video5
-
-https://someurl.withavideo.org//video6
-nameOfVideo7:::https://someurl.withavideo.org//video7
-```
-
-- It could be added the name the file should have by inserting ':::' between the name and the URL.
-- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
-- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
-- If type is 'movies', any blank lines will be ignored.
-
----
-
-The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
-```
-The same naming option is also available when not using a file.
-The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
-
-The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
-```
-
-The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
-```
-
-The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
-```
-
-If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
-```
-
-<a name="support"></a>
-## Support
- If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
-Currently maintaining it.
+Metadata-Version: 2.1
+Name: scrappo
+Version: 1.1.0
+Summary: Download any video from a specific URL.
+Home-page: https://github.com/zaytiri/scrappo
+Author: zaytiri
+Project-URL: GitHub, https://github.com/zaytiri/scrappo
+Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
+Keywords: video,download,tool,scrapping,scrap,cli,url python
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
+
+# Scrappo - Video Downloader Tool
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
+
+It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                          |
+|:---------------------------------------------------------------------------------|
+| can be input a .txt file containing a list of URLs                               |
+| download movies, series or related content                                       |
+| series will be separate into season folders                                      |
+| movies can also be separated in their own folder                                 |
+| videos already downloaded will be skipped                                        |
+| any errors regarding the videos will not stop program and will appear in the end |
+| progress bar while downloading                                                   |
+
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```
+pip --no-cache-dir install scrappo
+```
+
+or,
+
+```
+pip3 --no-cache-dir install scrappo
+```
+<a name="usage"></a>
+## Usage
+
+| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
+|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
+| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
+| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
+| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
+| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
+| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
+
+---
+### Important
+
+#### URLs .txt file
+The file containing a list of URLs must obey to certain requirements.
+
+```text
+nameOfVideo1:::https://someurl.withavideo.org//video1
+nameOfVideo2:::https://someurl.withavideo.org//video2
+https://someurl.withavideo.org//video3
+https://someurl.withavideo.org//video4
+nameOfVideo5:::https://someurl.withavideo.org//video5
+
+https://someurl.withavideo.org//video6
+nameOfVideo7:::https://someurl.withavideo.org//video7
+```
+
+- It could be added the name the file should have by inserting ':::' between the name and the URL.
+- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
+- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
+- If type is 'movies', any blank lines will be ignored.
+
+---
+
+The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
+```
+The same naming option is also available when not using a file.
+The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
+
+The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
+```
+
+The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
+```
+
+The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
+```
+
+If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
+```
+
+<a name="support"></a>
+## Support
+ If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
+Currently maintaining it.
```

### Comparing `scrappo-1.0.0/README.md` & `scrappo-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,137 +1,138 @@
-[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
-
-# Scrappo - Video Downloader Tool
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
-
-It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                           |
-|:----------------------------------------------------------------------------------|
-| can be input a .txt file containing a list of URLs                                |
-| download movies, series or related content                                        |
-| series will be separate into season folders                                       |
-| movies can also be separated in their own folder                                  |
-| videos already downloaded will be skipped                                         |
-| any errors regarding the videos will not stop program and will appear in the end. |
-
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```
-pip --no-cache-dir install scrappo
-```
-
-or,
-
-```
-pip3 --no-cache-dir install scrappo
-```
-<a name="usage"></a>
-## Usage
-
-| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
-|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
-| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
-| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
-| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
-| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
-| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
-
----
-### Important
-
-#### URLs .txt file
-The file containing a list of URLs must obey to certain requirements.
-
-```text
-nameOfVideo1:::https://someurl.withavideo.org//video1
-nameOfVideo2:::https://someurl.withavideo.org//video2
-https://someurl.withavideo.org//video3
-https://someurl.withavideo.org//video4
-nameOfVideo5:::https://someurl.withavideo.org//video5
-
-https://someurl.withavideo.org//video6
-nameOfVideo7:::https://someurl.withavideo.org//video7
-```
-
-- It could be added the name the file should have by inserting ':::' between the name and the URL.
-- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
-- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
-- If type is 'movies', any blank lines will be ignored.
-
----
-
-The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
-```
-The same naming option is also available when not using a file.
-The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
-
-The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
-```
-
-The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
-```
-
-The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
-```
-
-If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
-```
-
-<a name="support"></a>
-## Support
- If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
+[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
+
+# Scrappo - Video Downloader Tool
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
+
+It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                          |
+|:---------------------------------------------------------------------------------|
+| can be input a .txt file containing a list of URLs                               |
+| download movies, series or related content                                       |
+| series will be separate into season folders                                      |
+| movies can also be separated in their own folder                                 |
+| videos already downloaded will be skipped                                        |
+| any errors regarding the videos will not stop program and will appear in the end |
+| progress bar while downloading                                                   |
+
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```
+pip --no-cache-dir install scrappo
+```
+
+or,
+
+```
+pip3 --no-cache-dir install scrappo
+```
+<a name="usage"></a>
+## Usage
+
+| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
+|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
+| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
+| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
+| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
+| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
+| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
+
+---
+### Important
+
+#### URLs .txt file
+The file containing a list of URLs must obey to certain requirements.
+
+```text
+nameOfVideo1:::https://someurl.withavideo.org//video1
+nameOfVideo2:::https://someurl.withavideo.org//video2
+https://someurl.withavideo.org//video3
+https://someurl.withavideo.org//video4
+nameOfVideo5:::https://someurl.withavideo.org//video5
+
+https://someurl.withavideo.org//video6
+nameOfVideo7:::https://someurl.withavideo.org//video7
+```
+
+- It could be added the name the file should have by inserting ':::' between the name and the URL.
+- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
+- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
+- If type is 'movies', any blank lines will be ignored.
+
+---
+
+The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
+```
+The same naming option is also available when not using a file.
+The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
+
+The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
+```
+
+The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
+```
+
+The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
+```
+
+If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
+```
+
+<a name="support"></a>
+## Support
+ If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
 Currently maintaining it.
```

### Comparing `scrappo-1.0.0/scrappo/movies.py` & `scrappo-1.1.0/scrappo/movies.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-import os
-
-from scrappo.downloader import Downloader
-from scrappo.utils.log import show
-from scrappo.video import Video
-
-
-class Movies(Video):
-    def __init__(self, urls, output, separate):
-        super().__init__(urls, output)
-        self.separate = separate
-
-    def process_urls(self):
-        # returns a flat list
-        urls = [item for sublist in self.urls for item in sublist]
-
-        show('Downloading movies...')
-        for index, movie in enumerate(urls):
-            url = movie['url']
-            name = self.resolve_video_name(movie['name'], 'movie' + str(index + 1))
-
-            parent_path = self.output
-            if self.separate:
-                parent_path = self.add_folder(name)
-
-            path = os.path.join(parent_path, name + '.mp4')
-            if self.file_exists(path):
-                continue
-
-            successful = Downloader(url, path).download_video()
-
-            self.add_errors(successful, path, url)
+import os
+
+from scrappo.downloader import Downloader
+from scrappo.utils.log import show
+from scrappo.video import Video
+
+
+class Movies(Video):
+    def __init__(self, urls, output, separate):
+        super().__init__(urls, output)
+        self.separate = separate
+
+    def process_urls(self):
+        # returns a flat list
+        urls = [item for sublist in self.urls for item in sublist]
+
+        for index, movie in enumerate(urls):
+            url = movie['url']
+            name = self.resolve_video_name(movie['name'], 'movie' + str(index + 1))
+            show('Downloading ' + name + '...')
+
+            parent_path = self.output
+            if self.separate:
+                parent_path = self.add_folder(name)
+
+            path = os.path.join(parent_path, name + '.mp4')
+            if self.file_exists(path):
+                continue
+
+            successful = Downloader(url, path).download_video()
+
+            self.add_errors(successful, path, url)
```

### Comparing `scrappo-1.0.0/scrappo/processor.py` & `scrappo-1.1.0/scrappo/processor.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import os
-
-from scrappo.movies import Movies
-from scrappo.series import Series
-from scrappo.url_parser import UrlParser
-from scrappo.utils.log import show
-
-
-class Processor:
-
-    def __init__(self, arguments):
-        self.urls = arguments.urls.value
-        self.output = arguments.output.value
-        self.type = arguments.type.value
-        self.separate = arguments.separate.value
-
-    def process(self):
-        parser = UrlParser(self.urls)
-        urls = parser.parse()
-
-        path_main = self.output
-        if not os.path.isdir(path_main):
-            os.mkdir(path_main)
-
-        videos = None
-        if self.type == 'series':
-            videos = Series(urls, path_main, parser.file_name)
-        elif self.type == 'movies':
-            videos = Movies(urls, path_main, self.separate)
-
-        errors = videos.download()
-
-        if len(errors) != 0:
-            show('Following videos were not downloaded:')
-            for error in errors:
-                show('\t- ' + error['path'] + ': ' + error['url'], with_date=False)
+import os
+
+from scrappo.movies import Movies
+from scrappo.series import Series
+from scrappo.url_parser import UrlParser
+from scrappo.utils.log import show
+
+
+class Processor:
+
+    def __init__(self, arguments):
+        self.urls = arguments.urls.value
+        self.output = arguments.output.value
+        self.type = arguments.type.value
+        self.separate = arguments.separate.value
+
+    def process(self):
+        parser = UrlParser(self.urls)
+        urls = parser.parse()
+
+        path_main = self.output
+        if not os.path.isdir(path_main):
+            os.mkdir(path_main)
+
+        videos = None
+        if self.type == 'series':
+            videos = Series(urls, path_main, parser.file_name)
+        elif self.type == 'movies':
+            videos = Movies(urls, path_main, self.separate)
+
+        errors = videos.download()
+
+        if len(errors) != 0:
+            show('Following videos were not downloaded:')
+            for error in errors:
+                show('\t- ' + error['path'] + ': ' + error['url'], with_date=False)
```

### Comparing `scrappo-1.0.0/scrappo/series.py` & `scrappo-1.1.0/scrappo/series.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-import os
-
-from scrappo.downloader import Downloader
-from scrappo.utils.log import show
-from scrappo.video import Video
-
-
-class Series(Video):
-    def __init__(self, urls, output, file_name):
-        super().__init__(urls, output)
-        self.file_name = file_name
-
-    def process_urls(self):
-        show('Downloading series...')
-
-        parent_folder = self.add_folder(self.file_name)
-
-        for i, season in enumerate(self.urls):
-            season_folder = self.add_folder('season' + str(i+1), root=parent_folder)
-
-            for j, episode in enumerate(season):
-                url = episode['url']
-                name = self.resolve_video_name(episode['name'], 'episode' + str(j + 1))
-
-                path = os.path.join(season_folder, name + '.mp4')
-                if self.file_exists(path):
-                    continue
-
-                successful = Downloader(url, path).download_video()
-
-                self.add_errors(successful, path, url)
+import os
+
+from scrappo.downloader import Downloader
+from scrappo.utils.log import show
+from scrappo.video import Video
+
+
+class Series(Video):
+    def __init__(self, urls, output, file_name):
+        super().__init__(urls, output)
+        self.file_name = file_name
+
+    def process_urls(self):
+        parent_folder = self.add_folder(self.file_name)
+
+        for i, season in enumerate(self.urls):
+            show('Downloading season ' + str(i+1) + '...')
+            season_folder = self.add_folder('season' + str(i+1), root=parent_folder)
+
+            for j, episode in enumerate(season):
+                url = episode['url']
+                name = self.resolve_video_name(episode['name'], 'episode' + str(j + 1))
+                show('Downloading ' + name + '...')
+
+                path = os.path.join(season_folder, name + '.mp4')
+                if self.file_exists(path):
+                    continue
+
+                successful = Downloader(url, path).download_video()
+
+                self.add_errors(successful, path, url)
```

### Comparing `scrappo-1.0.0/scrappo/settings/manager.py` & `scrappo-1.1.0/scrappo/settings/manager.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os
-
-import argparse
-
-from margument.non_repeatable_settings import NonRepeatableSettings
-from margument.options import Options
-from margument.settings_processor import SettingsProcessor
-from scrappo.settings.settings import Settings
-from scrappo.version.progsettings import get_version
-
-
-class Manager:
-    def __init__(self):
-        self.args = argparse.ArgumentParser()
-        self.args.add_argument('--version', action='version', version='%(prog)s ' + str(get_version()))
-
-    def configure_arguments(self):
-        # manage generic configurations
-        settings = NonRepeatableSettings(path=os.path.join(os.path.dirname(os.path.realpath(__file__)), 'configs.yaml'),
-                                         program_arguments=Settings(),
-                                         options=Options(show_saved=True, save_different=True))
-
-        settings_processor = SettingsProcessor([settings], self.args)
-
+import os
+
+import argparse
+
+from margument.non_repeatable_settings import NonRepeatableSettings
+from margument.options import Options
+from margument.settings_processor import SettingsProcessor
+from scrappo.settings.settings import Settings
+from scrappo.version.progsettings import get_version
+
+
+class Manager:
+    def __init__(self):
+        self.args = argparse.ArgumentParser()
+        self.args.add_argument('--version', action='version', version='%(prog)s ' + str(get_version()))
+
+    def configure_arguments(self):
+        # manage generic configurations
+        settings = NonRepeatableSettings(path=os.path.join(os.path.dirname(os.path.realpath(__file__)), 'configs.yaml'),
+                                         program_arguments=Settings(),
+                                         options=Options(show_saved=True, save_different=True))
+
+        settings_processor = SettingsProcessor([settings], self.args)
+
         return settings_processor.run()
```

### Comparing `scrappo-1.0.0/scrappo/settings/settings.py` & `scrappo-1.1.0/scrappo/settings/settings.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import argparse
-
-from margument.argument import Argument
-from margument.arguments import Arguments
-
-from scrappo.utils.directory import Directory
-from scrappo.utils.log import throw
-
-
-class Settings(Arguments):
-    def __init__(self):
-        self.urls = Argument(name='urls',
-                             abbreviation_name='-u',
-                             full_name='--urls',
-                             help_message='A list of URLs of the videos to download or the path of a .txt file containing a list of URLs. More '
-                                          'details on creating the file in the README.md',
-                             metavar="",
-                             default=[])
-
-        self.output = Argument(name='output',
-                               abbreviation_name='-o',
-                               full_name='--output',
-                               help_message='The output folder path in which the videos will be downloaded.',
-                               metavar="",
-                               default='')
-
-        self.type = Argument(name='type',
-                             abbreviation_name='-t',
-                             full_name='--type',
-                             help_message='The type of the videos to download. Choices are "movies" or "series". The difference between the two '
-                                          'is that a series expects to have seasons and these will be separated in different folders. Default is '
-                                          '"movies".',
-                             metavar="",
-                             choices=['movies', 'series'],
-                             default='movies')
-
-        self.separate = Argument(name='separate',
-                                 abbreviation_name='',
-                                 full_name='--separate',
-                                 help_message='If enabled, it will separate every movie into his own folder. Default is disabled. True: --separate | '
-                                              'False: --no-separate',
-                                 metavar="",
-                                 default=False)
-
-        self.shutdown = Argument(name='shutdown',
-                                 abbreviation_name='',
-                                 full_name='--shutdown',
-                                 help_message='Enable/disable if computer will shutdown when the program has ended. Default is disabled.'
-                                              'True: --shutdown | False: --no-shutdown',
-                                 metavar="",
-                                 default=False)
-
-    def add_arguments(self, args_parser):
-        args_parser.add_argument(self.urls.abbreviation_name, self.urls.full_name,
-                                 nargs='*',
-                                 required=True,
-                                 help=self.urls.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.output.abbreviation_name, self.output.full_name,
-                                 type=str,
-                                 required=True,
-                                 help=self.output.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.type.abbreviation_name, self.type.full_name,
-                                 type=str,
-                                 required=True,
-                                 choices=self.type.choices,
-                                 help=self.type.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.separate.full_name,
-                                 action=argparse.BooleanOptionalAction,
-                                 help=self.separate.help_message,
-                                 default=argparse.SUPPRESS)
-
-        args_parser.add_argument(self.shutdown.full_name,
-                                 action=argparse.BooleanOptionalAction,
-                                 help=self.shutdown.help_message,
-                                 default=argparse.SUPPRESS)
-
-    def process_arguments(self, settings):
-        self.validate_path(settings[0].user_arguments)
-
-    def validate_path(self, user_args):
-        if self.output.name in user_args:
-            argument_path = Directory(user_args.output)
-            if not argument_path.exists():
-                throw(user_args.output + ' path does not exist.')
+import argparse
+
+from margument.argument import Argument
+from margument.arguments import Arguments
+
+from scrappo.utils.directory import Directory
+from scrappo.utils.log import throw
+
+
+class Settings(Arguments):
+    def __init__(self):
+        self.urls = Argument(name='urls',
+                             abbreviation_name='-u',
+                             full_name='--urls',
+                             help_message='A list of URLs of the videos to download or the path of a .txt file containing a list of URLs. More '
+                                          'details on creating the file in the README.md',
+                             metavar="",
+                             default=[])
+
+        self.output = Argument(name='output',
+                               abbreviation_name='-o',
+                               full_name='--output',
+                               help_message='The output folder path in which the videos will be downloaded.',
+                               metavar="",
+                               default='')
+
+        self.type = Argument(name='type',
+                             abbreviation_name='-t',
+                             full_name='--type',
+                             help_message='The type of the videos to download. Choices are "movies" or "series". The difference between the two '
+                                          'is that a series expects to have seasons and these will be separated in different folders. Default is '
+                                          '"movies".',
+                             metavar="",
+                             choices=['movies', 'series'],
+                             default='movies')
+
+        self.separate = Argument(name='separate',
+                                 abbreviation_name='',
+                                 full_name='--separate',
+                                 help_message='If enabled, it will separate every movie into his own folder. Default is disabled. True: --separate | '
+                                              'False: --no-separate',
+                                 metavar="",
+                                 default=False)
+
+        self.shutdown = Argument(name='shutdown',
+                                 abbreviation_name='',
+                                 full_name='--shutdown',
+                                 help_message='Enable/disable if computer will shutdown when the program has ended. Default is disabled.'
+                                              'True: --shutdown | False: --no-shutdown',
+                                 metavar="",
+                                 default=False)
+
+    def add_arguments(self, args_parser):
+        args_parser.add_argument(self.urls.abbreviation_name, self.urls.full_name,
+                                 nargs='*',
+                                 required=True,
+                                 help=self.urls.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.output.abbreviation_name, self.output.full_name,
+                                 type=str,
+                                 required=True,
+                                 help=self.output.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.type.abbreviation_name, self.type.full_name,
+                                 type=str,
+                                 required=True,
+                                 choices=self.type.choices,
+                                 help=self.type.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.separate.full_name,
+                                 action=argparse.BooleanOptionalAction,
+                                 help=self.separate.help_message,
+                                 default=argparse.SUPPRESS)
+
+        args_parser.add_argument(self.shutdown.full_name,
+                                 action=argparse.BooleanOptionalAction,
+                                 help=self.shutdown.help_message,
+                                 default=argparse.SUPPRESS)
+
+    def process_arguments(self, settings):
+        self.validate_path(settings[0].user_arguments)
+
+    def validate_path(self, user_args):
+        if self.output.name in user_args:
+            argument_path = Directory(user_args.output)
+            if not argument_path.exists():
+                throw(user_args.output + ' path does not exist.')
```

### Comparing `scrappo-1.0.0/scrappo/url_parser.py` & `scrappo-1.1.0/scrappo/url_parser.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import os
-
-from scrappo.utils.file import File
-from scrappo.utils.log import throw
-
-
-class UrlParser:
-    def __init__(self, urls):
-        self.urls = urls
-        self.file_name = ''
-
-    def parse(self):
-        if os.path.isdir(os.path.dirname(self.urls[0])):
-            try:
-                urls_file = File(self.urls[0])
-
-                # resolve file name without extension
-                name = os.path.basename(self.urls[0]).split('.')
-                name.pop()
-                self.file_name = '.'.join(name)
-
-                return self.parse_urls(urls_file.get_lines())
-
-            except FileNotFoundError:
-                throw(self.urls[0] + ' was not found.')
-
-        return self.parse_urls(self.urls)
-
-    @staticmethod
-    def split_url(url):
-        info = url.split(':::')
-        if len(info) > 1:
-            url = {'name': info[0], 'url': info[1]}
-        else:
-            url = {'name': '', 'url': info[0]}
-        return url
-
-    def parse_urls(self, urls_list):
-        urls = []
-        urls_found = []
-
-        for url in urls_list:
-            # remove '\n' from the string
-            url = url.rstrip()
-
-            # if it's a blank line it will append a new list
-            if not url:
-                urls.append(urls_found)
-                urls_found = []
-                continue
-
-            urls_found.append(self.split_url(url))
-
-        if len(urls_found) != 0:
-            urls.append(urls_found)
-
-        # just returns lists that are not empty
-        urls = [list_not_empty for list_not_empty in urls if len(list_not_empty) > 0]
-
-        return urls
+import os
+
+from scrappo.utils.file import File
+from scrappo.utils.log import throw
+
+
+class UrlParser:
+    def __init__(self, urls):
+        self.urls = urls
+        self.file_name = ''
+
+    def parse(self):
+        if os.path.isdir(os.path.dirname(self.urls[0])):
+            try:
+                urls_file = File(self.urls[0])
+
+                # resolve file name without extension
+                name = os.path.basename(self.urls[0]).split('.')
+                name.pop()
+                self.file_name = '.'.join(name)
+
+                return self.parse_urls(urls_file.get_lines())
+
+            except FileNotFoundError:
+                throw(self.urls[0] + ' was not found.')
+
+        return self.parse_urls(self.urls)
+
+    @staticmethod
+    def split_url(url):
+        info = url.split(':::')
+        if len(info) > 1:
+            url = {'name': info[0], 'url': info[1]}
+        else:
+            url = {'name': '', 'url': info[0]}
+        return url
+
+    def parse_urls(self, urls_list):
+        urls = []
+        urls_found = []
+
+        for url in urls_list:
+            # remove '\n' from the string
+            url = url.rstrip()
+
+            # if it's a blank line it will append a new list
+            if not url:
+                urls.append(urls_found)
+                urls_found = []
+                continue
+
+            urls_found.append(self.split_url(url))
+
+        if len(urls_found) != 0:
+            urls.append(urls_found)
+
+        # just returns lists that are not empty
+        urls = [list_not_empty for list_not_empty in urls if len(list_not_empty) > 0]
+
+        return urls
```

### Comparing `scrappo-1.0.0/scrappo/utils/date.py` & `scrappo-1.1.0/scrappo/utils/date.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from datetime import datetime, timedelta
-
-
-class Date:
-
-    def __init__(self, date='', time='', date_separator='', time_separator=''):
-        self.date_str = date
-        self.time_str = time
-        self.date_separator = date_separator
-        self.time_separator = time_separator
-        self.now = datetime.now()
-        self.converted_date = self.convert_date()
-        self.converted_time = self.convert_time()
-
-    def convert_date(self):
-        try:
-            splitted_date = self.date_str.split(self.date_separator)
-            self.converted_date = datetime(
-                day=int(splitted_date[0]),
-                month=int(splitted_date[1]),
-                year=int(splitted_date[2]),
-            )
-            return self.converted_date
-        except ValueError:
-            pass
-
-    def convert_time(self):
-        try:
-            splitted_time = self.time_str.split(self.time_separator)
-            self.converted_time = datetime(
-                day=datetime.min.day,
-                month=datetime.min.month,
-                year=datetime.min.year,
-
-                hour=int(splitted_time[0]),
-                minute=int(splitted_time[1])
-            )
-            if len(splitted_time) == 3:
-                self.converted_time += timedelta(seconds=int(splitted_time[2]))
-
-            return self.converted_time
-        except ValueError:
-            pass
-
-    def greater_than_today(self):
-        if self.converted_date is None:
-            return False
-
-        if self.converted_date > datetime.combine(datetime.today().date(), self.converted_date.time()):
-            return True
-        return False
-
-    def lesser_than_today(self):
-        if self.converted_date is None:
-            return False
-
-        if self.converted_date < datetime.combine(datetime.today().date(), self.converted_date.time()):
-            return True
-        return False
-
-    def equals_to_today(self):
-        if self.converted_date is None:
-            return False
-
-        if self.converted_date == datetime.combine(datetime.today().date(), self.converted_date.time()):
-            return True
-        return False
-
-    def time_greater_than_today(self):
-        if self.converted_time is None:
-            return False
-
-        self.now = datetime.now()
-        if self.now.hour >= int(self.converted_time.hour) and self.now.minute >= int(self.converted_time.minute):
-            return True
-        return False
-
-    @staticmethod
-    def get_current_day_name():
-        return datetime.now().strftime("%A").lower()
+from datetime import datetime, timedelta
+
+
+class Date:
+
+    def __init__(self, date='', time='', date_separator='', time_separator=''):
+        self.date_str = date
+        self.time_str = time
+        self.date_separator = date_separator
+        self.time_separator = time_separator
+        self.now = datetime.now()
+        self.converted_date = self.convert_date()
+        self.converted_time = self.convert_time()
+
+    def convert_date(self):
+        try:
+            splitted_date = self.date_str.split(self.date_separator)
+            self.converted_date = datetime(
+                day=int(splitted_date[0]),
+                month=int(splitted_date[1]),
+                year=int(splitted_date[2]),
+            )
+            return self.converted_date
+        except ValueError:
+            pass
+
+    def convert_time(self):
+        try:
+            splitted_time = self.time_str.split(self.time_separator)
+            self.converted_time = datetime(
+                day=datetime.min.day,
+                month=datetime.min.month,
+                year=datetime.min.year,
+
+                hour=int(splitted_time[0]),
+                minute=int(splitted_time[1])
+            )
+            if len(splitted_time) == 3:
+                self.converted_time += timedelta(seconds=int(splitted_time[2]))
+
+            return self.converted_time
+        except ValueError:
+            pass
+
+    def greater_than_today(self):
+        if self.converted_date is None:
+            return False
+
+        if self.converted_date > datetime.combine(datetime.today().date(), self.converted_date.time()):
+            return True
+        return False
+
+    def lesser_than_today(self):
+        if self.converted_date is None:
+            return False
+
+        if self.converted_date < datetime.combine(datetime.today().date(), self.converted_date.time()):
+            return True
+        return False
+
+    def equals_to_today(self):
+        if self.converted_date is None:
+            return False
+
+        if self.converted_date == datetime.combine(datetime.today().date(), self.converted_date.time()):
+            return True
+        return False
+
+    def time_greater_than_today(self):
+        if self.converted_time is None:
+            return False
+
+        self.now = datetime.now()
+        if self.now.hour >= int(self.converted_time.hour) and self.now.minute >= int(self.converted_time.minute):
+            return True
+        return False
+
+    @staticmethod
+    def get_current_day_name():
+        return datetime.now().strftime("%A").lower()
```

### Comparing `scrappo-1.0.0/scrappo/utils/directory.py` & `scrappo-1.1.0/scrappo/utils/directory.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import os.path
-from os.path import exists
-
-
-class Directory:
-    current_folder = ''
-    last_folder_path = ''
-
-    def __init__(self, root):
-        self.root = root
-        self.get_current_folder()
-        self.get_last_directory()
-
-    def get_last_directory(self):
-        self.last_folder_path = os.path.dirname(self.root)
-
-    def get_current_folder(self):
-        self.current_folder = os.path.basename(os.path.normpath(self.root))
-
-    def create(self, new_folder):
-        return os.path.join(self.root, new_folder)
-
-    def create_folder(self, new_folder):
-        new_directory = self.create(new_folder)
-        if not os.path.isdir(new_directory):
-            os.mkdir(new_directory)
-
-        return new_directory
-
-    def search_through(self):
-        return os.walk(self.root)
-
-    def remove(self):
-        os.remove(self.root)
-
-    def exists(self):
-        return exists(self.root)
+import os.path
+from os.path import exists
+
+
+class Directory:
+    current_folder = ''
+    last_folder_path = ''
+
+    def __init__(self, root):
+        self.root = root
+        self.get_current_folder()
+        self.get_last_directory()
+
+    def get_last_directory(self):
+        self.last_folder_path = os.path.dirname(self.root)
+
+    def get_current_folder(self):
+        self.current_folder = os.path.basename(os.path.normpath(self.root))
+
+    def create(self, new_folder):
+        return os.path.join(self.root, new_folder)
+
+    def create_folder(self, new_folder):
+        new_directory = self.create(new_folder)
+        if not os.path.isdir(new_directory):
+            os.mkdir(new_directory)
+
+        return new_directory
+
+    def search_through(self):
+        return os.walk(self.root)
+
+    def remove(self):
+        os.remove(self.root)
+
+    def exists(self):
+        return exists(self.root)
```

### Comparing `scrappo-1.0.0/scrappo/utils/split_string.py` & `scrappo-1.1.0/scrappo/utils/split_string.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-def split_string(string, separator, stop_character, include_separator=False):
-    """
-    Splits a given string into a list using a separator except when a sub-string is between a specific stop character.
-    :param include_separator: boolean to specify if the separator character must be included in the list or not
-    :param string: string to be split
-    :param separator: separator to split the string
-    :param stop_character: split does not happen between two of these characters
-    :return: a list containing the string but separated between specified separator
-    """
-    list_of_params = []
-    param = ''
-
-    is_between = False
-    for character in string:
-        if is_between:
-            if character == stop_character:
-                is_between = False
-                if not include_separator:
-                    continue
-        else:
-            if character == stop_character:
-                is_between = True
-                if not include_separator:
-                    continue
-
-            if character == separator:
-                list_of_params.append(param)
-                param = ''
-                continue
-
-        param += character
-
-    list_of_params.append(param)
-
-    return list_of_params
+def split_string(string, separator, stop_character, include_separator=False):
+    """
+    Splits a given string into a list using a separator except when a sub-string is between a specific stop character.
+    :param include_separator: boolean to specify if the separator character must be included in the list or not
+    :param string: string to be split
+    :param separator: separator to split the string
+    :param stop_character: split does not happen between two of these characters
+    :return: a list containing the string but separated between specified separator
+    """
+    list_of_params = []
+    param = ''
+
+    is_between = False
+    for character in string:
+        if is_between:
+            if character == stop_character:
+                is_between = False
+                if not include_separator:
+                    continue
+        else:
+            if character == stop_character:
+                is_between = True
+                if not include_separator:
+                    continue
+
+            if character == separator:
+                list_of_params.append(param)
+                param = ''
+                continue
+
+        param += character
+
+    list_of_params.append(param)
+
+    return list_of_params
```

### Comparing `scrappo-1.0.0/scrappo/video.py` & `scrappo-1.1.0/scrappo/video.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import os
-
-from scrappo.utils.log import show
-
-
-class Video:
-    def __init__(self, urls, output):
-        self.urls = urls
-        self.output = output
-        self.errors = []
-
-    def download(self):
-        self.errors = []
-
-        self.process_urls()
-
-        return self.errors
-
-    def process_urls(self):
-        raise NotImplementedError('To be implemented')
-
-    def add_folder(self, name, root=''):
-        if not root:
-            root = self.output
-
-        parent_path = os.path.join(root, name)
-        if not os.path.isdir(parent_path):
-            os.mkdir(parent_path)
-        return parent_path
-
-    @staticmethod
-    def file_exists(path):
-        if os.path.isfile(path):
-            show('Skipping existing video...')
-            return True
-        return False
-
-    def add_errors(self, successful, path, url):
-        if not successful:
-            error = {'path': path, 'url': url}
-            self.errors.append(error)
-
-    @staticmethod
-    def resolve_video_name(name, alt_name):
-        if not name:
-            name = alt_name
-        return name
+import os
+
+from scrappo.utils.log import show
+
+
+class Video:
+    def __init__(self, urls, output):
+        self.urls = urls
+        self.output = output
+        self.errors = []
+
+    def download(self):
+        self.errors = []
+
+        self.process_urls()
+
+        return self.errors
+
+    def process_urls(self):
+        raise NotImplementedError('To be implemented')
+
+    def add_folder(self, name, root=''):
+        if not root:
+            root = self.output
+
+        parent_path = os.path.join(root, name)
+        if not os.path.isdir(parent_path):
+            os.mkdir(parent_path)
+        return parent_path
+
+    @staticmethod
+    def file_exists(path):
+        if os.path.isfile(path):
+            show('Skipping existing video...')
+            return True
+        return False
+
+    def add_errors(self, successful, path, url):
+        if not successful:
+            error = {'path': path, 'url': url}
+            self.errors.append(error)
+
+    @staticmethod
+    def resolve_video_name(name, alt_name):
+        if not name:
+            name = alt_name
+        return name
```

### Comparing `scrappo-1.0.0/scrappo.egg-info/PKG-INFO` & `scrappo-1.1.0/scrappo.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,155 +1,156 @@
-Metadata-Version: 2.1
-Name: scrappo
-Version: 1.0.0
-Summary: Download any video from a specific URL.
-Home-page: https://github.com/zaytiri/scrappo
-Author: zaytiri
-Project-URL: GitHub, https://github.com/zaytiri/scrappo
-Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
-Keywords: video,download,tool,scrapping,scrap,cli,url python
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
-
-# Scrappo - Video Downloader Tool
-## Table of Contents
-
-- [Description](#description)
-- [Features](#features)
-- [Prerequisites](#prerequisites)
-- [Installation](#installation)
-- [Usage](#usage)
-- [Support](#support)
-- [License](#license)
-- [Status](#status)
-
-<a name="description"></a>
-
-## Description
-
-Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
-
-It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
-
-<a name="features"></a>
-
-## Features
-
-| Feature                                                                           |
-|:----------------------------------------------------------------------------------|
-| can be input a .txt file containing a list of URLs                                |
-| download movies, series or related content                                        |
-| series will be separate into season folders                                       |
-| movies can also be separated in their own folder                                  |
-| videos already downloaded will be skipped                                         |
-| any errors regarding the videos will not stop program and will appear in the end. |
-
-
-Any new features are **_very_** welcomed.
-
-### Future features
-
-Nothing at the moment.
-
-<a name="prerequisites"></a>
-
-## Prerequisites
-
-[Python 3](https://www.python.org/downloads/) must be installed.
-
-<a name="installation"></a>
-
-## Installation
-
-```
-pip --no-cache-dir install scrappo
-```
-
-or,
-
-```
-pip3 --no-cache-dir install scrappo
-```
-<a name="usage"></a>
-## Usage
-
-| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
-|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
-| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
-| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
-| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
-| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
-| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
-
----
-### Important
-
-#### URLs .txt file
-The file containing a list of URLs must obey to certain requirements.
-
-```text
-nameOfVideo1:::https://someurl.withavideo.org//video1
-nameOfVideo2:::https://someurl.withavideo.org//video2
-https://someurl.withavideo.org//video3
-https://someurl.withavideo.org//video4
-nameOfVideo5:::https://someurl.withavideo.org//video5
-
-https://someurl.withavideo.org//video6
-nameOfVideo7:::https://someurl.withavideo.org//video7
-```
-
-- It could be added the name the file should have by inserting ':::' between the name and the URL.
-- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
-- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
-- If type is 'movies', any blank lines will be ignored.
-
----
-
-The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
-```
-The same naming option is also available when not using a file.
-The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
-
-The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
-```
-
-The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
-```bash
-scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
-```
-
-The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
-```
-
-If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
-```bash
-scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
-```
-
-<a name="support"></a>
-## Support
- If any problems occurs, feel free to open an issue.
-
-<a name="license"></a>
-## License
-
-[MIT](https://choosealicense.com/licenses/mit/)
-
-<a name="status"></a>
-
-## Status
-
-Currently maintaining it.
+Metadata-Version: 2.1
+Name: scrappo
+Version: 1.1.0
+Summary: Download any video from a specific URL.
+Home-page: https://github.com/zaytiri/scrappo
+Author: zaytiri
+Project-URL: GitHub, https://github.com/zaytiri/scrappo
+Project-URL: Changelog, https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md
+Keywords: video,download,tool,scrapping,scrap,cli,url python
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.10.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Downloads](https://pepy.tech/badge/scrappo)](https://pepy.tech/project/scrappo)
+
+# Scrappo - Video Downloader Tool
+## Table of Contents
+
+- [Description](#description)
+- [Features](#features)
+- [Prerequisites](#prerequisites)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Support](#support)
+- [License](#license)
+- [Status](#status)
+
+<a name="description"></a>
+
+## Description
+
+Scrappo downloads any video from a given URL or a file containing a list of URLs. These URLs must be the actual video.
+
+It's possible to also distinguish between a series or movies. The difference between these two options is that a series expects to have at least 1 season, therefore each season will be  separate into its own folder containing each related episode.
+
+<a name="features"></a>
+
+## Features
+
+| Feature                                                                          |
+|:---------------------------------------------------------------------------------|
+| can be input a .txt file containing a list of URLs                               |
+| download movies, series or related content                                       |
+| series will be separate into season folders                                      |
+| movies can also be separated in their own folder                                 |
+| videos already downloaded will be skipped                                        |
+| any errors regarding the videos will not stop program and will appear in the end |
+| progress bar while downloading                                                   |
+
+
+Any new features are **_very_** welcomed.
+
+### Future features
+
+Nothing at the moment.
+
+<a name="prerequisites"></a>
+
+## Prerequisites
+
+[Python 3](https://www.python.org/downloads/) must be installed.
+
+<a name="installation"></a>
+
+## Installation
+
+```
+pip --no-cache-dir install scrappo
+```
+
+or,
+
+```
+pip3 --no-cache-dir install scrappo
+```
+<a name="usage"></a>
+## Usage
+
+| Command (shortcut)        | Command (full) | Required       | Description                                                                       |
+|:--------------------------|----------------|----------------|:----------------------------------------------------------------------------------|
+| -u                        | --urls         | **REQUIRED**   | a list of URLs or a path to a .txt file containing a list of URLs.                |
+| -o                        | --output       | **REQUIRED**   | the path to the folder in which the videos will be downloaded.                    |
+| -t                        | --type         | **REQUIRED**   | the type of the videos to download. Choices are "movies" or "series".             |
+| --separate/--no-separate  | ---            | **OPTIONAL**   | if enabled, it will separate every movie into his own folder.                     |
+| --shutdown/--no-shutdown  | ---            | **OPTIONAL**   | enable or disable shutting down computer when program is done                     |
+
+---
+### Important
+
+#### URLs .txt file
+The file containing a list of URLs must obey to certain requirements.
+
+```text
+nameOfVideo1:::https://someurl.withavideo.org//video1
+nameOfVideo2:::https://someurl.withavideo.org//video2
+https://someurl.withavideo.org//video3
+https://someurl.withavideo.org//video4
+nameOfVideo5:::https://someurl.withavideo.org//video5
+
+https://someurl.withavideo.org//video6
+nameOfVideo7:::https://someurl.withavideo.org//video7
+```
+
+- It could be added the name the file should have by inserting ':::' between the name and the URL.
+- If a URL does not have ':::', its assumed the name of the file will be 'movie#' or 'episode#' (# being the number according to the position (line) the URL has in the file), depending on if the type is 'movies' or 'series', respectively.
+- If type is 'series', the seasons should be separated by blank lines. This means, for instance in the example above, the season 1 has 5 episodes and the season 2 has 2 episodes. These episodes will be separated by folders with the name of corresponding season.
+- If type is 'movies', any blank lines will be ignored.
+
+---
+
+The following command will download all given URLs with the type 'movies'. These videos will be downloaded in the 'C:\Users\<username>\Desktop\movies' folder:
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2"
+```
+The same naming option is also available when not using a file.
+The command above will download 2 videos from two different sources which the names of those video files will be 'nameOfVideo1' and 'nameOfVideo2', respectively.
+
+The command below will do the same thing but separating each movie into its own folder. The folder name will be the same name as the video file name.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "nameOfVideo1:::https://someurl.withavideo.org//video1" "nameOfVideo2:::https://someurl.withavideo.org//video2" --separate
+```
+
+The following command will download all URLs contained in the 'C:\Users\<username>\Desktop\moviesToDownload.txt' file. Can also be used the '--separate' argument.
+```bash
+scrappo --type movies --output "C:\Users\<username>\Desktop\movies" --urls "C:\Users\<username>\Desktop\moviesToDownload.txt"
+```
+
+The command below will download all URLs contained in the 'C:\Users\<username>\Desktop\seriesToDownload.txt'. Inside 'C:\Users\<username>\Desktop\series' folder there will be at least a folder named 'season1' containing all related episodes. Keep in mind that the file needs to contain a blank line to indicate separation of seasons.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt"
+```
+
+If '--shutdown' argument is used, when all videos are downloaded, the device will be shut down.
+```bash
+scrappo --type series --output "C:\Users\<username>\Desktop\series" --urls "C:\Users\<username>\Desktop\seriesToDownload.txt" --shutdown
+```
+
+<a name="support"></a>
+## Support
+ If any problems occurs, feel free to open an issue.
+
+<a name="license"></a>
+## License
+
+[MIT](https://choosealicense.com/licenses/mit/)
+
+<a name="status"></a>
+
+## Status
+
+Currently maintaining it.
```

### Comparing `scrappo-1.0.0/scrappo.egg-info/SOURCES.txt` & `scrappo-1.1.0/scrappo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrappo-1.0.0/setup.py` & `scrappo-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-from setuptools import setup
-import pathlib
-
-from scrappo.version.progsettings import get_version
-
-here = pathlib.Path(__file__).parent.resolve()
-long_description = (here / "README.md").read_text(encoding="utf-8")
-
-version = get_version()
-
-setup(
-    name="scrappo",
-    version=version,
-    description="Download any video from a specific URL.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/zaytiri/scrappo",
-    project_urls={
-        'GitHub': 'https://github.com/zaytiri/scrappo',
-        'Changelog': 'https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md',
-    },
-    author="zaytiri",
-    classifiers=[
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-    ],
-    keywords="video, download, tool, scrapping, scrap, cli, url python",
-    package_data={'scrappo': ['version/progsettings.yaml']},
-    packages=["scrappo", "scrappo.utils", "scrappo.version", "scrappo.settings"],
-    python_requires=">=3.10.6",
-    install_requires=[
-        "PyYAML~=6.0",
-        "margument>=1.1.1",
-        "requests~=2.28.2",
-    ],
-    entry_points={
-        "console_scripts": [
-            "scrappo=scrappo:app.main",
-        ],
-    }
+from setuptools import setup
+import pathlib
+
+from scrappo.version.progsettings import get_version
+
+here = pathlib.Path(__file__).parent.resolve()
+long_description = (here / "README.md").read_text(encoding="utf-8")
+
+version = get_version()
+
+setup(
+    name="scrappo",
+    version=version,
+    description="Download any video from a specific URL.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/zaytiri/scrappo",
+    project_urls={
+        'GitHub': 'https://github.com/zaytiri/scrappo',
+        'Changelog': 'https://github.com/zaytiri/scrappo/blob/main/CHANGELOG.md',
+    },
+    author="zaytiri",
+    classifiers=[
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python :: 3",
+    ],
+    keywords="video, download, tool, scrapping, scrap, cli, url python",
+    package_data={'scrappo': ['version/progsettings.yaml']},
+    packages=["scrappo", "scrappo.utils", "scrappo.version", "scrappo.settings"],
+    python_requires=">=3.10.6",
+    install_requires=[
+        "PyYAML~=6.0",
+        "margument>=1.1.1",
+        "requests~=2.28.2",
+        "progress~=1.6",
+    ],
+    entry_points={
+        "console_scripts": [
+            "scrappo=scrappo:app.main",
+        ],
+    }
 )
```

