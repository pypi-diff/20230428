# Comparing `tmp/twitch-archiver-3.0.0.dev5.tar.gz` & `tmp/twitch-archiver-3.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitch-archiver-3.0.0.dev5.tar", last modified: Sun Apr 16 14:14:14 2023, max compression
+gzip compressed data, was "twitch-archiver-3.0.0.dev6.tar", last modified: Fri Apr 28 03:28:59 2023, max compression
```

## Comparing `twitch-archiver-3.0.0.dev5.tar` & `twitch-archiver-3.0.0.dev6.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:14.773853 twitch-archiver-3.0.0.dev5/
--rw-rw-rw-   0        0        0    34523 2022-03-22 11:59:38.000000 twitch-archiver-3.0.0.dev5/LICENSE
--rw-rw-rw-   0        0        0    10640 2023-04-16 14:14:14.772853 twitch-archiver-3.0.0.dev5/PKG-INFO
--rw-rw-rw-   0        0        0    10010 2023-04-16 09:17:51.000000 twitch-archiver-3.0.0.dev5/README.md
--rw-rw-rw-   0        0        0      781 2023-04-16 09:18:59.000000 twitch-archiver-3.0.0.dev5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-16 14:14:14.773853 twitch-archiver-3.0.0.dev5/setup.cfg
--rw-rw-rw-   0        0        0       92 2023-01-15 12:54:49.000000 twitch-archiver-3.0.0.dev5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:14.759851 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/
--rw-rw-rw-   0        0        0    10640 2023-04-16 14:14:14.000000 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-04-16 14:14:14.000000 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 14:14:14.000000 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-04-16 14:14:14.000000 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 14:14:14.000000 twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 14:14:14.771853 twitch-archiver-3.0.0.dev5/twitcharchiver/
--rw-rw-rw-   0        0        0    11567 2023-04-16 09:19:07.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/__init__.py
--rw-rw-rw-   0        0        0     3958 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/api.py
--rw-rw-rw-   0        0        0     3911 2023-04-16 09:17:18.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/arguments.py
--rw-rw-rw-   0        0        0     5015 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/configuration.py
--rw-rw-rw-   0        0        0     7401 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/database.py
--rw-rw-rw-   0        0        0    10173 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/downloader.py
--rw-rw-rw-   0        0        0     4263 2023-03-04 09:28:05.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/exceptions.py
--rw-rw-rw-   0        0        0     1672 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/logger.py
--rw-rw-rw-   0        0        0    41120 2023-04-16 09:17:52.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/processing.py
--rw-rw-rw-   0        0        0    13327 2023-03-18 05:40:32.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/stream.py
--rw-rw-rw-   0        0        0    11413 2023-03-04 09:27:37.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/twitch.py
--rw-rw-rw-   0        0        0    26558 2023-03-18 06:42:00.000000 twitch-archiver-3.0.0.dev5/twitcharchiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.826057 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10473 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 03:28:59.000000 twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:28:59.830057 twitch-archiver-3.0.0.dev6/twitcharchiver/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9922 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39610 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/twitch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25839 2023-04-28 03:28:45.000000 twitch-archiver-3.0.0.dev6/twitcharchiver/utils.py
```

### Comparing `twitch-archiver-3.0.0.dev5/LICENSE` & `twitch-archiver-3.0.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `twitch-archiver-3.0.0.dev5/PKG-INFO` & `twitch-archiver-3.0.0.dev6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: twitch-archiver
-Version: 3.0.0.dev5
-Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
-Author-email: Brisppy <brisppy@protonmail.com>
-Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
-Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-﻿```
- _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
-|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
-|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
-`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
-  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
-  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
-  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
-```
-<p align="center"><b>
-A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
-<br>
-Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
-</p>
-
-## Table of Contents
-
-  * [Features](#features)
-  * [Requirements](#requirements)
-  * [Installation & Usage](#installation--usage)
-    * [Installation](#installation)
-    * [Usage](#usage)
-    * [Arguments](#arguments)
-  * [Disclaimer](#disclaimer)
-
-## Features
-* Archives both video and chat logs.
-* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows real-time archiving of Twitch streams.[^2]
-* Generates a readable chat log with timestamps and user badges.
-* Supports downloading streams which aren't being archived by Twitch.
-* Error notifications supported with pushbullet.
-* Supports archiving of subscriber-only VODs.
-
-[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
-[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
-
-## Requirements
-* **[Python](https://www.python.org/) >= 3.7**
-* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
-
-## Installation & Usage
-### Installation
-Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
-Make sure to read the [usage](#usage) section after installation.
-
-#### Installing with PIP
-
-1. Ensure you meet the above [requirements](#requirements).
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Download and install TA with `python -m pip install twitch-archiver`.
-
-#### Installing Manually
-
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-4. Install Python "Build" package with `python -m pip install --upgrade build`.
-5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
-
-#### Installing as a Docker Container
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Build the container with `docker build . -t twitch-archiver`.
-4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
-```bash
-docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
-```
-
-### Usage
-Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
-
-**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
-Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
-
-Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
-
-More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
-
-#### Examples
-```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
-
-Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
-
-```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
-
-Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
-
-#### Arguments
-Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
-```
-usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
-                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
-                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
-
-requires one of:
-    -c CHANNEL, --channel CHANNEL
-            Channel(s) to download, comma separated if multiple provided.
-    -v VOD_ID, --vod-id VOD_ID
-            VOD ID(s) to download, comma separated if multiple provided.
-
-credentials are grabbed from stored config, OR provided with:
-    -i CLIENT_ID, --client-id CLIENT_ID
-            Client ID retrieved from dev.twitch.tv
-    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-            Client secret retrieved from dev.twitch.tv
-
-Both the video and chat logs are grabbed if neither are specified.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CHANNEL, --channel CHANNEL
-                        A single twitch channel to download, or multiple comma-separated channels.
-  -v VOD_ID, --vod-id VOD_ID
-                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
-  -i CLIENT_ID, --client-id CLIENT_ID
-                        Client ID retrieved from dev.twitch.tv
-  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-                        Client secret retrieved from dev.twitch.tv
-  -C, --chat            Only save chat logs.
-  -V, --video           Only save video.
-  -t THREADS, --threads THREADS
-                        Number of video download threads. (default: 20)
-  -q QUALITY, --quality QUALITY
-                        Quality to download. Options are 'best', 'worst' or a custom value.
-                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
-                        (default: best)
-  -d DIRECTORY, --directory DIRECTORY
-                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
-                        (default: $CURRENT_DIRECTORY)
-  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
-  -l, --live-only       Only download streams / VODs which are currently live.
-  -a, --archive-only    Don't download streams / VODs which are currently live.
-  -R, --real-time-archiver
-                        Enable real-time stream archiver.
-                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
-  -L LOG_FILE, --log-file LOG_FILE
-                        Output logs to specified file.
-  -I CONFIG_DIR, --config-dir CONFIG_DIR
-                        Directory to store configuration, VOD database and lock files.
-                        (default: $HOME/.config/twitch-archiver)
-  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
-                        Pushbullet key for sending pushes on error. Enabled by supplying key.
-  -Q, --quiet           Disable all log output.
-  -D, --debug           Enable debug logs.
-  --version             Show version number and exit.
-  --show-config         Show saved config and exit.
-```
-
-## Disclaimer
-This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
-
-If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
+Metadata-Version: 2.1
+Name: twitch-archiver
+Version: 3.0.0.dev6
+Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
+Author-email: Brisppy <brisppy@protonmail.com>
+Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
+Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿```
+ _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
+|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
+|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
+`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
+  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
+  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
+  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
+```
+<p align="center"><b>
+A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
+<br>
+Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
+</p>
+
+## Table of Contents
+
+  * [Features](#features)
+  * [Requirements](#requirements)
+  * [Installation & Usage](#installation--usage)
+    * [Installation](#installation)
+    * [Usage](#usage)
+    * [Arguments](#arguments)
+  * [Disclaimer](#disclaimer)
+
+## Features
+* Archives both video and chat logs.
+* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
+* Allows real-time archiving of Twitch streams.[^2]
+* Generates a readable chat log with timestamps and user badges.
+* Supports downloading streams which aren't being archived by Twitch.
+* Error notifications supported with pushbullet.
+* Supports archiving of subscriber-only VODs.
+
+[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
+[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
+
+## Requirements
+* **[Python](https://www.python.org/) >= 3.7**
+* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
+
+## Installation & Usage
+### Installation
+Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
+Make sure to read the [usage](#usage) section after installation.
+
+#### Installing with PIP
+
+1. Ensure you meet the above [requirements](#requirements).
+2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+3. Download and install TA with `python -m pip install twitch-archiver`.
+
+#### Installing Manually
+
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+
+#### Installing as a Docker Container
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Build the container with `docker build . -t twitch-archiver`.
+4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
+```bash
+docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
+```
+
+### Usage
+Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
+
+**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
+Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
+
+Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
+
+More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
+
+#### Examples
+```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
+
+Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
+
+```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
+
+Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
+
+#### Arguments
+Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
+```
+usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
+                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
+                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
+
+requires one of:
+    -c CHANNEL, --channel CHANNEL
+            Channel(s) to download, comma separated if multiple provided.
+    -v VOD_ID, --vod-id VOD_ID
+            VOD ID(s) to download, comma separated if multiple provided.
+
+credentials are grabbed from stored config, OR provided with:
+    -i CLIENT_ID, --client-id CLIENT_ID
+            Client ID retrieved from dev.twitch.tv
+    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+            Client secret retrieved from dev.twitch.tv
+
+Both the video and chat logs are grabbed if neither are specified.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CHANNEL, --channel CHANNEL
+                        A single twitch channel to download, or multiple comma-separated channels.
+  -v VOD_ID, --vod-id VOD_ID
+                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
+  -i CLIENT_ID, --client-id CLIENT_ID
+                        Client ID retrieved from dev.twitch.tv
+  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+                        Client secret retrieved from dev.twitch.tv
+  -C, --chat            Only save chat logs.
+  -V, --video           Only save video.
+  -t THREADS, --threads THREADS
+                        Number of video download threads. (default: 20)
+  -q QUALITY, --quality QUALITY
+                        Quality to download. Options are 'best', 'worst' or a custom value.
+                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
+                        (default: best)
+  -d DIRECTORY, --directory DIRECTORY
+                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
+                        (default: $CURRENT_DIRECTORY)
+  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
+  -l, --live-only       Only download streams / VODs which are currently live.
+  -a, --archive-only    Don't download streams / VODs which are currently live.
+  -R, --real-time-archiver
+                        Enable real-time stream archiver.
+                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
+  -L LOG_FILE, --log-file LOG_FILE
+                        Output logs to specified file.
+  -I CONFIG_DIR, --config-dir CONFIG_DIR
+                        Directory to store configuration, VOD database and lock files.
+                        (default: $HOME/.config/twitch-archiver)
+  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
+                        Pushbullet key for sending pushes on error. Enabled by supplying key.
+  -Q, --quiet           Disable all log output.
+  -D, --debug           Enable debug logs.
+  --version             Show version number and exit.
+  --show-config         Show saved config and exit.
+```
+
+## Disclaimer
+This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
+
+If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
```

### Comparing `twitch-archiver-3.0.0.dev5/README.md` & `twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,153 +1,167 @@
-﻿```
- _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
-|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
-|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
-`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
-  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
-  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
-  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
-```
-<p align="center"><b>
-A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
-<br>
-Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
-</p>
-
-## Table of Contents
-
-  * [Features](#features)
-  * [Requirements](#requirements)
-  * [Installation & Usage](#installation--usage)
-    * [Installation](#installation)
-    * [Usage](#usage)
-    * [Arguments](#arguments)
-  * [Disclaimer](#disclaimer)
-
-## Features
-* Archives both video and chat logs.
-* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows real-time archiving of Twitch streams.[^2]
-* Generates a readable chat log with timestamps and user badges.
-* Supports downloading streams which aren't being archived by Twitch.
-* Error notifications supported with pushbullet.
-* Supports archiving of subscriber-only VODs.
-
-[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
-[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
-
-## Requirements
-* **[Python](https://www.python.org/) >= 3.7**
-* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
-
-## Installation & Usage
-### Installation
-Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
-Make sure to read the [usage](#usage) section after installation.
-
-#### Installing with PIP
-
-1. Ensure you meet the above [requirements](#requirements).
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Download and install TA with `python -m pip install twitch-archiver`.
-
-#### Installing Manually
-
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-4. Install Python "Build" package with `python -m pip install --upgrade build`.
-5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
-
-#### Installing as a Docker Container
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Build the container with `docker build . -t twitch-archiver`.
-4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
-```bash
-docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
-```
-
-### Usage
-Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
-
-**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
-Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
-
-Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
-
-More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
-
-#### Examples
-```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
-
-Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
-
-```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
-
-Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
-
-#### Arguments
-Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
-```
-usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
-                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
-                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
-
-requires one of:
-    -c CHANNEL, --channel CHANNEL
-            Channel(s) to download, comma separated if multiple provided.
-    -v VOD_ID, --vod-id VOD_ID
-            VOD ID(s) to download, comma separated if multiple provided.
-
-credentials are grabbed from stored config, OR provided with:
-    -i CLIENT_ID, --client-id CLIENT_ID
-            Client ID retrieved from dev.twitch.tv
-    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-            Client secret retrieved from dev.twitch.tv
-
-Both the video and chat logs are grabbed if neither are specified.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CHANNEL, --channel CHANNEL
-                        A single twitch channel to download, or multiple comma-separated channels.
-  -v VOD_ID, --vod-id VOD_ID
-                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
-  -i CLIENT_ID, --client-id CLIENT_ID
-                        Client ID retrieved from dev.twitch.tv
-  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-                        Client secret retrieved from dev.twitch.tv
-  -C, --chat            Only save chat logs.
-  -V, --video           Only save video.
-  -t THREADS, --threads THREADS
-                        Number of video download threads. (default: 20)
-  -q QUALITY, --quality QUALITY
-                        Quality to download. Options are 'best', 'worst' or a custom value.
-                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
-                        (default: best)
-  -d DIRECTORY, --directory DIRECTORY
-                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
-                        (default: $CURRENT_DIRECTORY)
-  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
-  -l, --live-only       Only download streams / VODs which are currently live.
-  -a, --archive-only    Don't download streams / VODs which are currently live.
-  -R, --real-time-archiver
-                        Enable real-time stream archiver.
-                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
-  -L LOG_FILE, --log-file LOG_FILE
-                        Output logs to specified file.
-  -I CONFIG_DIR, --config-dir CONFIG_DIR
-                        Directory to store configuration, VOD database and lock files.
-                        (default: $HOME/.config/twitch-archiver)
-  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
-                        Pushbullet key for sending pushes on error. Enabled by supplying key.
-  -Q, --quiet           Disable all log output.
-  -D, --debug           Enable debug logs.
-  --version             Show version number and exit.
-  --show-config         Show saved config and exit.
-```
-
-## Disclaimer
-This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
-
-If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
+Metadata-Version: 2.1
+Name: twitch-archiver
+Version: 3.0.0.dev6
+Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
+Author-email: Brisppy <brisppy@protonmail.com>
+Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
+Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+﻿```
+ _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
+|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
+|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
+`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
+  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
+  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
+  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
+```
+<p align="center"><b>
+A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
+<br>
+Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
+</p>
+
+## Table of Contents
+
+  * [Features](#features)
+  * [Requirements](#requirements)
+  * [Installation & Usage](#installation--usage)
+    * [Installation](#installation)
+    * [Usage](#usage)
+    * [Arguments](#arguments)
+  * [Disclaimer](#disclaimer)
+
+## Features
+* Archives both video and chat logs.
+* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
+* Allows real-time archiving of Twitch streams.[^2]
+* Generates a readable chat log with timestamps and user badges.
+* Supports downloading streams which aren't being archived by Twitch.
+* Error notifications supported with pushbullet.
+* Supports archiving of subscriber-only VODs.
+
+[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
+[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
+
+## Requirements
+* **[Python](https://www.python.org/) >= 3.7**
+* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
+
+## Installation & Usage
+### Installation
+Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
+Make sure to read the [usage](#usage) section after installation.
+
+#### Installing with PIP
+
+1. Ensure you meet the above [requirements](#requirements).
+2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+3. Download and install TA with `python -m pip install twitch-archiver`.
+
+#### Installing Manually
+
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+
+#### Installing as a Docker Container
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Build the container with `docker build . -t twitch-archiver`.
+4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
+```bash
+docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
+```
+
+### Usage
+Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
+
+**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
+Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
+
+Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
+
+More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
+
+#### Examples
+```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
+
+Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
+
+```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
+
+Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
+
+#### Arguments
+Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
+```
+usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
+                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
+                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
+
+requires one of:
+    -c CHANNEL, --channel CHANNEL
+            Channel(s) to download, comma separated if multiple provided.
+    -v VOD_ID, --vod-id VOD_ID
+            VOD ID(s) to download, comma separated if multiple provided.
+
+credentials are grabbed from stored config, OR provided with:
+    -i CLIENT_ID, --client-id CLIENT_ID
+            Client ID retrieved from dev.twitch.tv
+    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+            Client secret retrieved from dev.twitch.tv
+
+Both the video and chat logs are grabbed if neither are specified.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CHANNEL, --channel CHANNEL
+                        A single twitch channel to download, or multiple comma-separated channels.
+  -v VOD_ID, --vod-id VOD_ID
+                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
+  -i CLIENT_ID, --client-id CLIENT_ID
+                        Client ID retrieved from dev.twitch.tv
+  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+                        Client secret retrieved from dev.twitch.tv
+  -C, --chat            Only save chat logs.
+  -V, --video           Only save video.
+  -t THREADS, --threads THREADS
+                        Number of video download threads. (default: 20)
+  -q QUALITY, --quality QUALITY
+                        Quality to download. Options are 'best', 'worst' or a custom value.
+                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
+                        (default: best)
+  -d DIRECTORY, --directory DIRECTORY
+                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
+                        (default: $CURRENT_DIRECTORY)
+  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
+  -l, --live-only       Only download streams / VODs which are currently live.
+  -a, --archive-only    Don't download streams / VODs which are currently live.
+  -R, --real-time-archiver
+                        Enable real-time stream archiver.
+                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
+  -L LOG_FILE, --log-file LOG_FILE
+                        Output logs to specified file.
+  -I CONFIG_DIR, --config-dir CONFIG_DIR
+                        Directory to store configuration, VOD database and lock files.
+                        (default: $HOME/.config/twitch-archiver)
+  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
+                        Pushbullet key for sending pushes on error. Enabled by supplying key.
+  -Q, --quiet           Disable all log output.
+  -D, --debug           Enable debug logs.
+  --version             Show version number and exit.
+  --show-config         Show saved config and exit.
+```
+
+## Disclaimer
+This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
+
+If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
```

### Comparing `twitch-archiver-3.0.0.dev5/pyproject.toml` & `twitch-archiver-3.0.0.dev6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "twitch-archiver"
-version = "3.0.0.dev5"
-authors = [
-  { name="Brisppy", email="brisppy@protonmail.com" },
-]
-description = "A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs."
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/Brisppy/twitch-archiver"
-"Bug Tracker" = "https://github.com/Brisppy/twitch-archiver/issues"
-
-[project.scripts]
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "twitch-archiver"
+version = "3.0.0.dev6"
+authors = [
+  { name="Brisppy", email="brisppy@protonmail.com" },
+]
+description = "A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs."
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/Brisppy/twitch-archiver"
+"Bug Tracker" = "https://github.com/Brisppy/twitch-archiver/issues"
+
+[project.scripts]
 twitch-archiver = "twitcharchiver.__init__:main"
```

### Comparing `twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/PKG-INFO` & `twitch-archiver-3.0.0.dev6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,167 +1,153 @@
-Metadata-Version: 2.1
-Name: twitch-archiver
-Version: 3.0.0.dev5
-Summary: A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
-Author-email: Brisppy <brisppy@protonmail.com>
-Project-URL: Homepage, https://github.com/Brisppy/twitch-archiver
-Project-URL: Bug Tracker, https://github.com/Brisppy/twitch-archiver/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU Affero General Public License v3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-﻿```
- _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
-|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
-|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
-`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
-  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
-  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
-  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
-```
-<p align="center"><b>
-A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
-<br>
-Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
-</p>
-
-## Table of Contents
-
-  * [Features](#features)
-  * [Requirements](#requirements)
-  * [Installation & Usage](#installation--usage)
-    * [Installation](#installation)
-    * [Usage](#usage)
-    * [Arguments](#arguments)
-  * [Disclaimer](#disclaimer)
-
-## Features
-* Archives both video and chat logs.
-* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
-* Allows real-time archiving of Twitch streams.[^2]
-* Generates a readable chat log with timestamps and user badges.
-* Supports downloading streams which aren't being archived by Twitch.
-* Error notifications supported with pushbullet.
-* Supports archiving of subscriber-only VODs.
-
-[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
-[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
-
-## Requirements
-* **[Python](https://www.python.org/) >= 3.7**
-* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
-
-## Installation & Usage
-### Installation
-Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
-Make sure to read the [usage](#usage) section after installation.
-
-#### Installing with PIP
-
-1. Ensure you meet the above [requirements](#requirements).
-2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-3. Download and install TA with `python -m pip install twitch-archiver`.
-
-#### Installing Manually
-
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
-4. Install Python "Build" package with `python -m pip install --upgrade build`.
-5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
-
-#### Installing as a Docker Container
-1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
-2. Unpack the archive and enter the directory with `cd twitch-archiver`.
-3. Build the container with `docker build . -t twitch-archiver`.
-4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
-```bash
-docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
-```
-
-### Usage
-Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
-
-**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
-Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
-
-Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
-
-More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
-
-#### Examples
-```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
-
-Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
-
-```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
-
-Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
-
-#### Arguments
-Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
-```
-usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
-                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
-                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
-
-requires one of:
-    -c CHANNEL, --channel CHANNEL
-            Channel(s) to download, comma separated if multiple provided.
-    -v VOD_ID, --vod-id VOD_ID
-            VOD ID(s) to download, comma separated if multiple provided.
-
-credentials are grabbed from stored config, OR provided with:
-    -i CLIENT_ID, --client-id CLIENT_ID
-            Client ID retrieved from dev.twitch.tv
-    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-            Client secret retrieved from dev.twitch.tv
-
-Both the video and chat logs are grabbed if neither are specified.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CHANNEL, --channel CHANNEL
-                        A single twitch channel to download, or multiple comma-separated channels.
-  -v VOD_ID, --vod-id VOD_ID
-                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
-  -i CLIENT_ID, --client-id CLIENT_ID
-                        Client ID retrieved from dev.twitch.tv
-  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-                        Client secret retrieved from dev.twitch.tv
-  -C, --chat            Only save chat logs.
-  -V, --video           Only save video.
-  -t THREADS, --threads THREADS
-                        Number of video download threads. (default: 20)
-  -q QUALITY, --quality QUALITY
-                        Quality to download. Options are 'best', 'worst' or a custom value.
-                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
-                        (default: best)
-  -d DIRECTORY, --directory DIRECTORY
-                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
-                        (default: $CURRENT_DIRECTORY)
-  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
-  -l, --live-only       Only download streams / VODs which are currently live.
-  -a, --archive-only    Don't download streams / VODs which are currently live.
-  -R, --real-time-archiver
-                        Enable real-time stream archiver.
-                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
-  -L LOG_FILE, --log-file LOG_FILE
-                        Output logs to specified file.
-  -I CONFIG_DIR, --config-dir CONFIG_DIR
-                        Directory to store configuration, VOD database and lock files.
-                        (default: $HOME/.config/twitch-archiver)
-  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
-                        Pushbullet key for sending pushes on error. Enabled by supplying key.
-  -Q, --quiet           Disable all log output.
-  -D, --debug           Enable debug logs.
-  --version             Show version number and exit.
-  --show-config         Show saved config and exit.
-```
-
-## Disclaimer
-This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
-
-If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
+﻿```
+ _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______ 
+|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
+|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
+`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
+  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
+  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
+  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
+```
+<p align="center"><b>
+A simple, fast, platform-independent tool for downloading Twitch streams, videos and chat logs.</b>
+<br>
+Primarily focused on data preservation, this script can be used to archive an entire Twitch channel at once, or to quickly grab the chat log from a single VOD. Both archived, and live VODs can be downloaded with this script.
+</p>
+
+## Table of Contents
+
+  * [Features](#features)
+  * [Requirements](#requirements)
+  * [Installation & Usage](#installation--usage)
+    * [Installation](#installation)
+    * [Usage](#usage)
+    * [Arguments](#arguments)
+  * [Disclaimer](#disclaimer)
+
+## Features
+* Archives both video and chat logs.
+* VODs can be downloaded as fast as your Internet connection (and storage) can handle.[^1]
+* Allows real-time archiving of Twitch streams.[^2]
+* Generates a readable chat log with timestamps and user badges.
+* Supports downloading streams which aren't being archived by Twitch.
+* Error notifications supported with pushbullet.
+* Supports archiving of subscriber-only VODs.
+
+[^1]: If you wish to speed up (or slow down) the downloading of VOD pieces, supply the '--threads NUMBER' argument to the script. This changes how many download threads are used to grab the individual video files. With the default of 20, I can max out my gigabit Internet while downloading to an M.2 drive.
+[^2]: There is one caveat with live archiving due to how Twitch presents ads. Ads are not downloaded, BUT while an ad is displayed, the actual stream output is not sent. This can result in missing segments under very rare circumstances, but any missing segments should be filled via a parallel VOD archival function. 
+
+## Requirements
+* **[Python](https://www.python.org/) >= 3.7**
+* **[FFmpeg](https://ffmpeg.org/) >= 4.3.1** and **ffprobe** (Accessible via your PATH - see [Installation](#installation))
+
+## Installation & Usage
+### Installation
+Twitch Archiver can be installed via pip, setup as a docker container or installed manually.\
+Make sure to read the [usage](#usage) section after installation.
+
+#### Installing with PIP
+
+1. Ensure you meet the above [requirements](#requirements).
+2. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+3. Download and install TA with `python -m pip install twitch-archiver`.
+
+#### Installing Manually
+
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Install [pip](https://pip.pypa.io/en/stable/installation/) if you do not already have it.
+4. Install Python "Build" package with `python -m pip install --upgrade build`.
+5. Build the package with `python -m build`, then install with `python -m pip install ./dist/twitch-archiver-*.tar.gz`.
+
+#### Installing as a Docker Container
+1. Either download the repository via the green code button at the top of the page, or grab the latest release [here](https://github.com/Brisppy/twitch-archiver/releases/latest).
+2. Unpack the archive and enter the directory with `cd twitch-archiver`.
+3. Build the container with `docker build . -t twitch-archiver`.
+4. Run the container with the following command. *Configuration can also be provided via environment variables (see [wiki]((https://github.com/Brisppy/twitch-archiver/wiki/Wiki#environment-variables)))*.
+```bash
+docker run -it -v {output_dir}:/output -v {config_dir}:/config twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "/output" -I "/config"
+```
+
+### Usage
+Run via your terminal of choice. Use `twitch-archiver -h` to view help text.
+
+**Before you start downloading VODs or streams** you will need generate and provide your Twitch app developer credentials to Twitch Archiver. If you do not yet have these credentials, see [Retrieving Tokens](https://github.com/Brisppy/twitch-archiver/wiki/Wiki#retrieving-tokens). \
+Once you have these, run TA once with `twitch-archiver -i CLIENT_ID -s CLIENT_SECRET -v 0`, where *CLIENT_ID* and *CLIENT_SECRET* are your Twitch client ID and client secret.
+
+Alternatively you can run TA with the above command without replacing the CLIENT_ID and CLIENT_SECRET, and instead add them manually to the configuration file located in `$HOME/.config/twitch-archiver/config.ini`.
+
+More advanced usage such as watch mode and setting up as a service can be found in the [Wiki](https://github.com/Brisppy/twitch-archiver/wiki/Wiki).
+
+#### Examples
+```# twitch-archiver -c Brisppy -i {client_id} -s {client_secret} -d "Z:\\twitch-archive"```
+
+Would download **video** and **chat** of all VODs from the channel **Brisppy**, using the provided **client_id** and **client_secret**, to the directory **Z:\twitch-archive**.
+
+```# twitch-archiver -v 1276315849,1275305106 -d "/mnt/twitch-archive" -V -t 10```
+
+Would download VODs **1276315849** and **1275305106** to the directory **/mnt/twitch-archive**, only saving the **video**  using **10 download threads**.
+
+#### Arguments
+Below is the output of the `--help` or `-h` command. This displays all the available arguments and a brief description of how to use them.
+```
+usage: twitch-archiver [-h] (-c CHANNEL | -v VOD_ID) [-i CLIENT_ID] [-s CLIENT_SECRET] [-C] [-V] 
+                       [-t THREADS] [-q QUALITY] [-d DIRECTORY] [-w] [-l | -a | -R] [-L LOG_FILE] 
+                       [-I CONFIG_DIR] [-p PUSHBULLET_KEY] [-Q | -D] [--version] [--show-config]
+
+requires one of:
+    -c CHANNEL, --channel CHANNEL
+            Channel(s) to download, comma separated if multiple provided.
+    -v VOD_ID, --vod-id VOD_ID
+            VOD ID(s) to download, comma separated if multiple provided.
+
+credentials are grabbed from stored config, OR provided with:
+    -i CLIENT_ID, --client-id CLIENT_ID
+            Client ID retrieved from dev.twitch.tv
+    -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+            Client secret retrieved from dev.twitch.tv
+
+Both the video and chat logs are grabbed if neither are specified.
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -c CHANNEL, --channel CHANNEL
+                        A single twitch channel to download, or multiple comma-separated channels.
+  -v VOD_ID, --vod-id VOD_ID
+                        A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).
+  -i CLIENT_ID, --client-id CLIENT_ID
+                        Client ID retrieved from dev.twitch.tv
+  -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+                        Client secret retrieved from dev.twitch.tv
+  -C, --chat            Only save chat logs.
+  -V, --video           Only save video.
+  -t THREADS, --threads THREADS
+                        Number of video download threads. (default: 20)
+  -q QUALITY, --quality QUALITY
+                        Quality to download. Options are 'best', 'worst' or a custom value.
+                        Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).
+                        (default: best)
+  -d DIRECTORY, --directory DIRECTORY
+                        Directory to store archived VOD(s), use TWO slashes for Windows paths.
+                        (default: $CURRENT_DIRECTORY)
+  -w, --watch           Continually check every 10 seconds for new streams/VODs from a specified channel.
+  -l, --live-only       Only download streams / VODs which are currently live.
+  -a, --archive-only    Don't download streams / VODs which are currently live.
+  -R, --real-time-archiver
+                        Enable real-time stream archiver.
+                        Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.
+  -L LOG_FILE, --log-file LOG_FILE
+                        Output logs to specified file.
+  -I CONFIG_DIR, --config-dir CONFIG_DIR
+                        Directory to store configuration, VOD database and lock files.
+                        (default: $HOME/.config/twitch-archiver)
+  -p PUSHBULLET_KEY, --pushbullet-key PUSHBULLET_KEY
+                        Pushbullet key for sending pushes on error. Enabled by supplying key.
+  -Q, --quiet           Disable all log output.
+  -D, --debug           Enable debug logs.
+  --version             Show version number and exit.
+  --show-config         Show saved config and exit.
+```
+
+## Disclaimer
+This script is intended to be used with the express permission of any involved rights holders, and is not intended to be used to duplicate, download or steal copyrighted content or information. When downloading VODs ensure you have permission from ALL involved rights holders for the content which you are downloading, and if you have the intention to share such content, you should also have explicit permission to do so.
+
+If your intent is to use this script to lazily rip and upload streams to another platform for your own gain without the permission of the streamer, I implore you to stop and think about what you are doing and the possible effect of doing so, and politely request that you find another method with which to steal the work of others.
```

### Comparing `twitch-archiver-3.0.0.dev5/twitch_archiver.egg-info/SOURCES.txt` & `twitch-archiver-3.0.0.dev6/twitch_archiver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 twitch_archiver.egg-info/PKG-INFO
 twitch_archiver.egg-info/SOURCES.txt
 twitch_archiver.egg-info/dependency_links.txt
 twitch_archiver.egg-info/entry_points.txt
 twitch_archiver.egg-info/top_level.txt
 twitcharchiver/__init__.py
 twitcharchiver/api.py
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/__init__.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-r"""
- _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______
-|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
-|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
-`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
-  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
-  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
-  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
-Created by:
-    https://github.com/Brisppy
-Inspired by:
-    https://github.com/PetterKraabol/Twitch-Chat-Downloader/
-    https://github.com/ihabunek/twitch-dl
-    https://github.com/streamlink/streamlink
-Twitch Archiver - A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
-Copyright (C) 2023 https://github.com/Brisppy
-
-This program is free software: you can redistribute it and/or modify
-it under the terms of the GNU Affero General Public License as
-published by the Free Software Foundation, either version 3 of the
-License, or (at your option) any later version.
-This program is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Affero General Public License for more details.
-You should have received a copy of the GNU Affero General Public License
-along with this program.  If not, see <https://www.gnu.org/licenses/>.
-"""
-
-import argparse
-import os
-import sys
-import textwrap
-
-from pathlib import Path
-from time import sleep
-
-from twitcharchiver.arguments import Arguments
-from twitcharchiver.configuration import Configuration
-from twitcharchiver.exceptions import TwitchAPIError
-from twitcharchiver.logger import Logger
-from twitcharchiver.processing import Processing
-from twitcharchiver.twitch import Twitch
-from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
-
-__version__ = '3.0.0.dev5'
-
-
-def main():
-    """
-    Main processing for twitch-archiver.
-    """
-    parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
-    Twitch Archiver v{__version__} - https://github.com/Brisppy/twitch-archiver
-
-    A fast, platform-independent Python script for downloading past and present Twitch VODs and chat logs.
-
-    requires one of:
-        -c CHANNEL, --channel CHANNEL
-                Channel(s) to download, comma separated if multiple provided.
-        -v VOD_ID, --vod-id VOD_ID
-                VOD ID(s) to download, comma separated if multiple provided.
-
-    credentials are grabbed from stored config, OR provided with:
-        -i CLIENT_ID, --client-id CLIENT_ID
-                Client ID retrieved from dev.twitch.tv
-        -s CLIENT_SECRET, --client-secret CLIENT_SECRET
-                Client secret retrieved from dev.twitch.tv
-                
-    Both the video and chat logs are grabbed if neither are specified.
-    """), formatter_class=argparse.RawTextHelpFormatter)
-    mode = parser.add_mutually_exclusive_group(
-        required=not (('--show-config' in sys.argv) or
-                      (
-                      (getenv("TWITCH_ARCHIVER_CHANNEL")) is not None) or
-                      (getenv("TWITCH_ARCHIVER_VOD_ID") is not None)
-                      ))
-    stream = parser.add_mutually_exclusive_group(required=False)
-    loglevel = parser.add_mutually_exclusive_group(required=False)
-    mode.add_argument('-c', '--channel', type=str, action='store',
-                      help='A single twitch channel to download, or multiple comma-separated channels.',
-                      default=getenv("TWITCH_ARCHIVER_CHANNEL"))
-    mode.add_argument('-v', '--vod-id', type=str, action='store',
-                      help='A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).',
-                      default=getenv("TWITCH_ARCHIVER_VOD_ID"))
-    parser.add_argument('-i', '--client-id', action='store', help='Client ID retrieved from dev.twitch.tv',
-                        default=getenv("TWITCH_ARCHIVER_CLIENT_ID"))
-    parser.add_argument('-s', '--client-secret', action='store', help='Client secret retrieved from dev.twitch.tv',
-                        default=getenv("TWITCH_ARCHIVER_CLIENT_SECRET"))
-    parser.add_argument('-C', '--chat', action='store_true', help='Only save chat logs.',
-                        default=getenv("TWITCH_ARCHIVER_CHAT", False, True))
-    parser.add_argument('-V', '--video', action='store_true', help='Only save video.',
-                        default=getenv("TWITCH_ARCHIVER_VIDEO", False, True))
-    parser.add_argument('-t', '--threads', type=int, action='store',
-                        help='Number of video download threads. (default: %(default)s)',
-                        default=getenv("TWITCH_ARCHIVER_THREADS", 20))
-    parser.add_argument('-q', '--quality', type=str, action='store',
-                        help="Quality to download. Options are 'best', 'worst' or a custom value.\n"
-                             'Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).\n'
-                             '(default: best)', default='best')
-    parser.add_argument('-d', '--directory', action='store',
-                        help='Directory to store archived VOD(s), use TWO slashes for Windows paths.\n'
-                             '(default: %(default)s)', type=Path,
-                        default=getenv('TWITCH_ARCHIVER_DIRECTORY', Path(os.getcwd())))
-    parser.add_argument('-w', '--watch', action='store_true',
-                        help='Continually check every 10 seconds for new streams/VODs from a specified channel.',
-                        default=getenv('TWITCH_ARCHIVER_WATCH', False, True))
-    stream.add_argument('-l', '--live-only', action='store_true',
-                        default=getenv('TWITCH_ARCHIVER_LIVE_ONLY', False, True),
-                        help='Only download streams / VODs which are currently live.')
-    stream.add_argument('-a', '--archive-only', action='store_true',
-                        help="Don't download streams / VODs which are currently live.",
-                        default=getenv("TWITCH_ARCHIVER_ARCHIVE_ONLY", False, True))
-    stream.add_argument('-R', '--real-time-archiver', action='store_true',
-                        help="Enable real-time stream archiver.\n"
-                             "Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.",
-                        default=getenv('TWITCH_ARCHIVER_REAL_TIME_ARCHIVER', False, True))
-    parser.add_argument('-L', '--log-file', action='store', help='Output logs to specified file.', type=Path,
-                        default=getenv("TWITCH_ARCHIVER_LOG_FILE", False))
-    parser.add_argument('-I', '--config-dir', action='store', type=Path,
-                        help='Directory to store configuration, VOD database and lock files.\n(default: %(default)s)',
-                        default=getenv('TWITCH_ARCHIVER_CONFIG_DIR',
-                                       Path(os.path.expanduser("~"), '.config', 'twitch-archiver')))
-    parser.add_argument('-p', '--pushbullet-key', action='store',
-                        help='Pushbullet key for sending pushes on error. Enabled by supplying key.',
-                        default=getenv("TWITCH_ARCHIVER_PUSHBULLET_KEY", False))
-    loglevel.add_argument('-Q', '--quiet', action='store_const', help='Disable all log output.', const=50, default=0)
-    loglevel.add_argument('-D', '--debug', action='store_const', help='Enable debug logs.', const=10, default=0)
-    parser.add_argument('--version', action='version', version=f'Twitch Archiver v{__version__}',
-                        help='Show version number and exit.')
-    parser.add_argument('--show-config', action='store_true', help='Show saved config and exit.', default=False)
-
-    # setup arguments
-    args = Arguments()
-    args.setup_args(parser.parse_args().__dict__)
-
-    # setup logging
-    log = Logger.setup_logger(args.get('quiet') + args.get('debug'), args.get('log_file'))
-    log.debug('Debug logging enabled.')
-
-    # debug only: output sanitized version of arguments
-    args_sanitized = args.get().copy()
-    for key in ['client_id', 'client_secret', 'pushbullet_key']:
-        if args_sanitized[key]:
-            args_sanitized.update({key: 24 * '*' + args_sanitized[key][24:]})
-
-    log.debug('Arguments: %s', args_sanitized)
-
-    # compare with current git version
-    latest_version, release_notes = get_latest_version()
-    if check_update_available(__version__, latest_version):
-        log.warning('New version of Twitch-Archiver available - Version %s:\n'
-                    'https://github.com/Brisppy/twitch-archiver/releases/latest\nRelease notes:\n\n%s\n',
-                    latest_version, release_notes)
-    else:
-        log.info('Twitch Archiver v%s - https://github.com/Brisppy/twitch-archiver', __version__)
-
-    # load configuration from ini
-    config = Configuration()
-    config.load_config(Path(args.get('config_dir'), 'config.ini'))
-    log.debug('Settings prior to loading config: %s', config.get_sanitized())
-
-    # overwrite different or missing configuration variables
-    config.generate_config(args.get())
-    log.debug('Settings after loading config: %s', config.get_sanitized())
-
-    # prompt if client id or secret empty
-    if config.get('client_id') == '' or config.get('client_secret') == '':
-        log.info('No client_id or client_secret passed as argument or found in config file.')
-        config.set('client_id', input('Your client ID: '))
-        config.set('client_secret', input('Your client secret: '))
-
-    log.debug('Performing Twitch authentication.')
-    call_twitch = Twitch(config.get('client_id'), config.get('client_secret'), config.get('oauth_token'))
-    # generate oauth token if it is missing, is invalid, or expiring soon
-    if config.get('oauth_token') == '' or call_twitch.validate_oauth_token() < 604800:
-        log.debug('No OAuth token found, or token is invalid or expiring soon - generating a new one.')
-        try:
-            config.set('oauth_token', call_twitch.generate_oauth_token())
-            log.debug('New OAuth token is: %s', config.get_sanitized("oauth_token"))
-            # store returned token
-            config.save(Path(args.get('config_dir'), 'config.ini'))
-        except TwitchAPIError as err:
-            log.error('OAuth token generation failed. Error: %s', str(err))
-            send_push(config.get('pushbullet_key'), 'OAuth token generation failed.', str(err))
-            sys.exit(1)
-
-    process = Processing(config.get(), args.get())
-
-    while True:
-        if args.get('channel') is not None:
-            process.get_channel(args.get('channel'))
-
-        if args.get('watch'):
-            sleep(10)
-
-        else:
-            break
-
-    if args.get('vod_id') is not None:
-        for vod_id in args.get('vod_id'):
-            process.get_vod_connector(vod_id, args.get('video'), args.get('chat'))
-
-
-if __name__ == '__main__':
-    main()
+r"""
+ _______ ___ ___ ___ _______ _______ ___ ___  _______ _______ _______ ___ ___ ___ ___ ___ _______ _______
+|       |   Y   |   |       |   _   |   Y   ||   _   |   _   |   _   |   Y   |   |   Y   |   _   |   _   \
+|.|   | |.  |   |.  |.|   | |.  1___|.  1   ||.  1   |.  l   |.  1___|.  1   |.  |.  |   |.  1___|.  l   /
+`-|.  |-|. / \  |.  `-|.  |-|.  |___|.  _   ||.  _   |.  _   |.  |___|.  _   |.  |.  |   |.  __)_|.  _   1
+  |:  | |:      |:  | |:  | |:  1   |:  |   ||:  |   |:  |   |:  1   |:  |   |:  |:  1   |:  1   |:  |   |
+  |::.| |::.|:. |::.| |::.| |::.. . |::.|:. ||::.|:. |::.|:. |::.. . |::.|:. |::.|\:.. ./|::.. . |::.|:. |
+  `---' `--- ---`---' `---' `-------`--- ---'`--- ---`--- ---`-------`--- ---`---' `---' `-------`--- ---'
+Created by:
+    https://github.com/Brisppy
+Inspired by:
+    https://github.com/PetterKraabol/Twitch-Chat-Downloader/
+    https://github.com/ihabunek/twitch-dl
+    https://github.com/streamlink/streamlink
+Twitch Archiver - A simple, fast, platform-independent tool for downloading Twitch streams, videos, and chat logs.
+Copyright (C) 2023 https://github.com/Brisppy
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as
+published by the Free Software Foundation, either version 3 of the
+License, or (at your option) any later version.
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""
+
+import argparse
+import os
+import sys
+import textwrap
+
+from pathlib import Path
+from time import sleep
+
+from twitcharchiver.arguments import Arguments
+from twitcharchiver.configuration import Configuration
+from twitcharchiver.exceptions import TwitchAPIError
+from twitcharchiver.logger import Logger
+from twitcharchiver.processing import Processing
+from twitcharchiver.twitch import Twitch
+from twitcharchiver.utils import getenv, send_push, get_latest_version, version_tuple, check_update_available
+
+__version__ = '3.0.0.dev6'
+
+
+def main():
+    """
+    Main processing for twitch-archiver.
+    """
+    parser = argparse.ArgumentParser(argument_default=None, description=textwrap.dedent(f"""\
+    Twitch Archiver v{__version__} - https://github.com/Brisppy/twitch-archiver
+
+    A fast, platform-independent Python script for downloading past and present Twitch VODs and chat logs.
+
+    requires one of:
+        -c CHANNEL, --channel CHANNEL
+                Channel(s) to download, comma separated if multiple provided.
+        -v VOD_ID, --vod-id VOD_ID
+                VOD ID(s) to download, comma separated if multiple provided.
+
+    credentials are grabbed from stored config, OR provided with:
+        -i CLIENT_ID, --client-id CLIENT_ID
+                Client ID retrieved from dev.twitch.tv
+        -s CLIENT_SECRET, --client-secret CLIENT_SECRET
+                Client secret retrieved from dev.twitch.tv
+                
+    Both the video and chat logs are grabbed if neither are specified.
+    """), formatter_class=argparse.RawTextHelpFormatter)
+    mode = parser.add_mutually_exclusive_group(
+        required=not (('--show-config' in sys.argv) or
+                      (
+                      (getenv("TWITCH_ARCHIVER_CHANNEL")) is not None) or
+                      (getenv("TWITCH_ARCHIVER_VOD_ID") is not None)
+                      ))
+    stream = parser.add_mutually_exclusive_group(required=False)
+    loglevel = parser.add_mutually_exclusive_group(required=False)
+    mode.add_argument('-c', '--channel', type=str, action='store',
+                      help='A single twitch channel to download, or multiple comma-separated channels.',
+                      default=getenv("TWITCH_ARCHIVER_CHANNEL"))
+    mode.add_argument('-v', '--vod-id', type=str, action='store',
+                      help='A single VOD (e.g 12763849) or many comma-separated IDs (e.g 12763159,12753056).',
+                      default=getenv("TWITCH_ARCHIVER_VOD_ID"))
+    parser.add_argument('-i', '--client-id', action='store', help='Client ID retrieved from dev.twitch.tv',
+                        default=getenv("TWITCH_ARCHIVER_CLIENT_ID"))
+    parser.add_argument('-s', '--client-secret', action='store', help='Client secret retrieved from dev.twitch.tv',
+                        default=getenv("TWITCH_ARCHIVER_CLIENT_SECRET"))
+    parser.add_argument('-C', '--chat', action='store_true', help='Only save chat logs.',
+                        default=getenv("TWITCH_ARCHIVER_CHAT", False, True))
+    parser.add_argument('-V', '--video', action='store_true', help='Only save video.',
+                        default=getenv("TWITCH_ARCHIVER_VIDEO", False, True))
+    parser.add_argument('-t', '--threads', type=int, action='store',
+                        help='Number of video download threads. (default: %(default)s)',
+                        default=getenv("TWITCH_ARCHIVER_THREADS", 20))
+    parser.add_argument('-q', '--quality', type=str, action='store',
+                        help="Quality to download. Options are 'best', 'worst' or a custom value.\n"
+                             'Format for custom values is [resolution]p[framerate], (e.g 1080p60, 720p30).\n'
+                             '(default: best)', default='best')
+    parser.add_argument('-d', '--directory', action='store',
+                        help='Directory to store archived VOD(s), use TWO slashes for Windows paths.\n'
+                             '(default: %(default)s)', type=Path,
+                        default=getenv('TWITCH_ARCHIVER_DIRECTORY', Path(os.getcwd())))
+    parser.add_argument('-w', '--watch', action='store_true',
+                        help='Continually check every 10 seconds for new streams/VODs from a specified channel.',
+                        default=getenv('TWITCH_ARCHIVER_WATCH', False, True))
+    stream.add_argument('-l', '--live-only', action='store_true',
+                        default=getenv('TWITCH_ARCHIVER_LIVE_ONLY', False, True),
+                        help='Only download streams / VODs which are currently live.')
+    stream.add_argument('-a', '--archive-only', action='store_true',
+                        help="Don't download streams / VODs which are currently live.",
+                        default=getenv("TWITCH_ARCHIVER_ARCHIVE_ONLY", False, True))
+    stream.add_argument('-R', '--real-time-archiver', action='store_true',
+                        help="Enable real-time stream archiver.\n"
+                             "Read https://github.com/Brisppy/twitch-archiver/wiki/Wiki#real-time-archiver.",
+                        default=getenv('TWITCH_ARCHIVER_REAL_TIME_ARCHIVER', False, True))
+    parser.add_argument('-L', '--log-file', action='store', help='Output logs to specified file.', type=Path,
+                        default=getenv("TWITCH_ARCHIVER_LOG_FILE", False))
+    parser.add_argument('-I', '--config-dir', action='store', type=Path,
+                        help='Directory to store configuration, VOD database and lock files.\n(default: %(default)s)',
+                        default=getenv('TWITCH_ARCHIVER_CONFIG_DIR',
+                                       Path(os.path.expanduser("~"), '.config', 'twitch-archiver')))
+    parser.add_argument('-p', '--pushbullet-key', action='store',
+                        help='Pushbullet key for sending pushes on error. Enabled by supplying key.',
+                        default=getenv("TWITCH_ARCHIVER_PUSHBULLET_KEY", False))
+    loglevel.add_argument('-Q', '--quiet', action='store_const', help='Disable all log output.', const=50, default=0)
+    loglevel.add_argument('-D', '--debug', action='store_const', help='Enable debug logs.', const=10, default=0)
+    parser.add_argument('--version', action='version', version=f'Twitch Archiver v{__version__}',
+                        help='Show version number and exit.')
+    parser.add_argument('--show-config', action='store_true', help='Show saved config and exit.', default=False)
+
+    # setup arguments
+    args = Arguments()
+    args.setup_args(parser.parse_args().__dict__)
+
+    # setup logging
+    log = Logger.setup_logger(args.get('quiet') + args.get('debug'), args.get('log_file'))
+    log.debug('Debug logging enabled.')
+
+    # debug only: output sanitized version of arguments
+    args_sanitized = args.get().copy()
+    for key in ['client_id', 'client_secret', 'pushbullet_key']:
+        if args_sanitized[key]:
+            args_sanitized.update({key: 24 * '*' + args_sanitized[key][24:]})
+
+    log.debug('Arguments: %s', args_sanitized)
+
+    # compare with current git version
+    latest_version, release_notes = get_latest_version()
+    if check_update_available(__version__, latest_version):
+        log.warning('New version of Twitch-Archiver available - Version %s:\n'
+                    'https://github.com/Brisppy/twitch-archiver/releases/latest\nRelease notes:\n\n%s\n',
+                    latest_version, release_notes)
+    else:
+        log.info('Twitch Archiver v%s - https://github.com/Brisppy/twitch-archiver', __version__)
+
+    # load configuration from ini
+    config = Configuration()
+    config.load_config(Path(args.get('config_dir'), 'config.ini'))
+    log.debug('Settings prior to loading config: %s', config.get_sanitized())
+
+    # overwrite different or missing configuration variables
+    config.generate_config(args.get())
+    log.debug('Settings after loading config: %s', config.get_sanitized())
+
+    # prompt if client id or secret empty
+    if config.get('client_id') == '' or config.get('client_secret') == '':
+        log.info('No client_id or client_secret passed as argument or found in config file.')
+        config.set('client_id', input('Your client ID: '))
+        config.set('client_secret', input('Your client secret: '))
+
+    log.debug('Performing Twitch authentication.')
+    call_twitch = Twitch(config.get('client_id'), config.get('client_secret'), config.get('oauth_token'))
+    # generate oauth token if it is missing, is invalid, or expiring soon
+    if config.get('oauth_token') == '' or call_twitch.validate_oauth_token() < 604800:
+        log.debug('No OAuth token found, or token is invalid or expiring soon - generating a new one.')
+        try:
+            config.set('oauth_token', call_twitch.generate_oauth_token())
+            log.debug('New OAuth token is: %s', config.get_sanitized("oauth_token"))
+            # store returned token
+            config.save(Path(args.get('config_dir'), 'config.ini'))
+        except TwitchAPIError as err:
+            log.error('OAuth token generation failed. Error: %s', str(err))
+            send_push(config.get('pushbullet_key'), 'OAuth token generation failed.', str(err))
+            sys.exit(1)
+
+    process = Processing(config.get(), args.get())
+
+    while True:
+        if args.get('channel') is not None:
+            process.get_channel(args.get('channel'))
+
+        if args.get('watch'):
+            sleep(10)
+
+        else:
+            break
+
+    if args.get('vod_id') is not None:
+        for vod_id in args.get('vod_id'):
+            process.get_vod_connector(vod_id, args.get('video'), args.get('chat'))
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/api.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/api.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""
-Handler for API requests.
-"""
-
-import requests
-
-from twitcharchiver.exceptions import RequestError, TwitchAPIError, TwitchAPIErrorNotFound, TwitchAPIErrorForbidden, \
-    TwitchAPIErrorBadRequest
-
-
-class Api:
-    """
-    Sends requests to a specified API endpoint.
-    """
-    @staticmethod
-    def get_request(url, p=None, h=None):
-        """
-        Wrapper for get requests for catching exceptions and status code issues.\n
-
-            :param url: http/s endpoint to send request to
-            :param p: parameter(s) to pass with request
-            :param h: header(s) to pass with request
-            :return: entire requests response
-            :raises requestError: on requests module error
-            :raises twitchAPIErrorBadRequest: on http code 400
-            :raises twitchAPIErrorForbidden: on http code 403
-            :raises twitchAPIErrorNotFound: on http code 404
-            :raises twitchAPIError: on any http code other than 400, 403, 404 or 200
-        """
-        try:
-            if p is None:
-                _r = requests.get(url, headers=h, timeout=10)
-
-            else:
-                _r = requests.get(url, params=p, timeout=10)
-
-        except requests.exceptions.RequestException as err:
-            raise RequestError(url, err) from err
-
-        if _r.status_code == 400:
-            raise TwitchAPIErrorBadRequest(_r)
-
-        if _r.status_code == 403:
-            raise TwitchAPIErrorForbidden(_r)
-
-        if _r.status_code == 404:
-            raise TwitchAPIErrorNotFound(_r)
-
-        if _r.status_code != 200:
-            raise TwitchAPIError(_r)
-
-        return _r
-
-    @staticmethod
-    def get_request_with_session(url, session):
-        """Wrapper for get requests using a session for catching exceptions and status code issues.
-
-        :param url: http/s endpoint to send request to
-        :param session: a requests session for sending request
-        :return: entire requests response
-        """
-        try:
-            _r = session.get(url, timeout=10)
-
-        except requests.exceptions.RequestException as err:
-            raise RequestError(url, err) from err
-
-        if _r.status_code == 400:
-            raise TwitchAPIErrorBadRequest(_r)
-
-        if _r.status_code == 403:
-            raise TwitchAPIErrorForbidden(_r)
-
-        if _r.status_code == 404:
-            raise TwitchAPIErrorNotFound(_r)
-
-        if _r.status_code != 200:
-            raise TwitchAPIError(_r)
-
-        return _r
-
-    @staticmethod
-    def post_request(url, d=None, j=None, h=None):
-        """Wrapper for post requests for catching exceptions and status code issues.
-
-        :param url: http/s endpoint to send request to
-        :param d: data to send with request
-        :param j: data to send with request as json
-        :param h: headers to send with request
-        :return: entire requests response
-        """
-        try:
-            if j is None:
-                _r = requests.post(url, data=d, headers=h, timeout=10)
-
-            elif d is None:
-                _r = requests.post(url, json=j, headers=h, timeout=10)
-
-        except requests.exceptions.RequestException as err:
-            raise RequestError(url, err) from err
-
-        if _r.status_code != 200:
-            raise TwitchAPIError(_r)
-
-        return _r
-
-    @staticmethod
-    def post_request_with_session(url, session, j):
-        """Wrapper for post requests for catching exceptions and status code issues.
-
-        :param url: http/s endpoint to send request to
-        :param session: requests session
-        :param j: data to send with request as json
-        :return: entire requests response
-        """
-        try:
-            _r = session.post(url, json=j, timeout=10)
-
-        except requests.exceptions.RequestException as err:
-            raise RequestError(url, err) from err
-
-        return _r
+"""
+Handler for API requests.
+"""
+
+import requests
+
+from twitcharchiver.exceptions import RequestError, TwitchAPIError, TwitchAPIErrorNotFound, TwitchAPIErrorForbidden, \
+    TwitchAPIErrorBadRequest
+
+
+class Api:
+    """
+    Sends requests to a specified API endpoint.
+    """
+    @staticmethod
+    def get_request(url, p=None, h=None):
+        """
+        Wrapper for get requests for catching exceptions and status code issues.\n
+
+            :param url: http/s endpoint to send request to
+            :param p: parameter(s) to pass with request
+            :param h: header(s) to pass with request
+            :return: entire requests response
+            :raises requestError: on requests module error
+            :raises twitchAPIErrorBadRequest: on http code 400
+            :raises twitchAPIErrorForbidden: on http code 403
+            :raises twitchAPIErrorNotFound: on http code 404
+            :raises twitchAPIError: on any http code other than 400, 403, 404 or 200
+        """
+        try:
+            if p is None:
+                _r = requests.get(url, headers=h, timeout=10)
+
+            else:
+                _r = requests.get(url, params=p, timeout=10)
+
+        except requests.exceptions.RequestException as err:
+            raise RequestError(url, err) from err
+
+        if _r.status_code == 400:
+            raise TwitchAPIErrorBadRequest(_r)
+
+        if _r.status_code == 403:
+            raise TwitchAPIErrorForbidden(_r)
+
+        if _r.status_code == 404:
+            raise TwitchAPIErrorNotFound(_r)
+
+        if _r.status_code != 200:
+            raise TwitchAPIError(_r)
+
+        return _r
+
+    @staticmethod
+    def get_request_with_session(url, session):
+        """Wrapper for get requests using a session for catching exceptions and status code issues.
+
+        :param url: http/s endpoint to send request to
+        :param session: a requests session for sending request
+        :return: entire requests response
+        """
+        try:
+            _r = session.get(url, timeout=10)
+
+        except requests.exceptions.RequestException as err:
+            raise RequestError(url, err) from err
+
+        if _r.status_code == 400:
+            raise TwitchAPIErrorBadRequest(_r)
+
+        if _r.status_code == 403:
+            raise TwitchAPIErrorForbidden(_r)
+
+        if _r.status_code == 404:
+            raise TwitchAPIErrorNotFound(_r)
+
+        if _r.status_code != 200:
+            raise TwitchAPIError(_r)
+
+        return _r
+
+    @staticmethod
+    def post_request(url, d=None, j=None, h=None):
+        """Wrapper for post requests for catching exceptions and status code issues.
+
+        :param url: http/s endpoint to send request to
+        :param d: data to send with request
+        :param j: data to send with request as json
+        :param h: headers to send with request
+        :return: entire requests response
+        """
+        try:
+            if j is None:
+                _r = requests.post(url, data=d, headers=h, timeout=10)
+
+            elif d is None:
+                _r = requests.post(url, json=j, headers=h, timeout=10)
+
+        except requests.exceptions.RequestException as err:
+            raise RequestError(url, err) from err
+
+        if _r.status_code != 200:
+            raise TwitchAPIError(_r)
+
+        return _r
+
+    @staticmethod
+    def post_request_with_session(url, session, j):
+        """Wrapper for post requests for catching exceptions and status code issues.
+
+        :param url: http/s endpoint to send request to
+        :param session: requests session
+        :param j: data to send with request as json
+        :return: entire requests response
+        """
+        try:
+            _r = session.post(url, json=j, timeout=10)
+
+        except requests.exceptions.RequestException as err:
+            raise RequestError(url, err) from err
+
+        return _r
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/arguments.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/arguments.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-"""
-Handles parsing and storage of arguments passed to twitch-archiver.
-"""
-
-import re
-import sys
-
-from pathlib import Path
-
-
-class Arguments:
-    """
-    Function for parsing arguments for access later.
-    """
-    __args = {}
-
-    @staticmethod
-    def setup_args(args):
-        """Sets up and formats provided arguments.
-
-        :param args: arguments object to create parameters from
-        """
-        for argument in args:
-            Arguments.set(argument, args[argument])
-
-        if Arguments.get('show_config'):
-            try:
-                with open(Path(Arguments.get('config_dir'), 'config.ini'), 'r', encoding='utf8') as config:
-                    print(config.read())
-                    sys.exit(0)
-            except FileNotFoundError:
-                sys.exit('Config not found. Run Twitch-Archiver once with your Client ID and Secret to generate one.')
-
-        # validate mutual exclusivity of arguments passed via CLI and environment variables
-        # required as values set via environment variables bypass argparse mutex handling
-        for mutex_args in (("vod_id", "channel"), ("live_only", "archive_only")):
-            mutex_arg_0, mutex_arg_1 = Arguments.get(mutex_args[0]), Arguments.get(mutex_args[1])
-            # check if both mutex args have a value (including empty string)
-            if mutex_arg_0 is not None and mutex_arg_1 is not None:
-                raise ValueError("Cannot accept both of the following mutually exclusive arguments: '"
-                                 f"{mutex_args[0]}={mutex_arg_0}' and '{mutex_args[1]}={mutex_arg_1}'")
-
-        # get both video and chat logs if neither selected
-        if not Arguments.get('chat') and not Arguments.get('video'):
-            Arguments.set('chat', True)
-            Arguments.set('video', True)
-
-        # generate list from comma-separated vods
-        if Arguments.get('vod_id'):
-            # generate vod list
-            vod_ids = list(Arguments.get('vod_id').split(','))
-
-            # format urls to just vod ids
-            for idx, vod_id in enumerate(vod_ids):
-                # test match and replace
-                match = re.findall(r"(?<=twitch\.tv/videos/)[0-9]*", vod_id)
-                if match:
-                    vod_ids[idx] = match[0]
-
-            # insert formatted vods
-            Arguments.set('vod_id', vod_ids)
-
-        # generate list from comma-separated channels
-        elif Arguments.get('channel'):
-            # generate channel list
-            channels = list(Arguments.get('channel').split(','))
-
-            # format urls to just channel name
-            for idx, channel in enumerate(channels):
-                # test and replace
-                match = re.findall(r"(?<=twitch\.tv/)[a-zA-Z0-9]*", channel)
-                if match:
-                    channels[idx] = match[0]
-
-            # insert formatted channels
-            Arguments.set('channel', channels)
-
-        # split quality into [resolution, framerate]
-        if Arguments.get('quality') not in ['best', 'worst']:
-            Arguments.set('quality', Arguments.get('quality').split('p'))
-
-        if Arguments.get('watch'):
-            print('Launching Twitch-Archiver in watch mode.')
-
-    @staticmethod
-    def set(name, value):
-        """Set a specified class attribute.
-
-        :param name: name of attribute to change
-        :param value: value to set attribute to
-        """
-        Arguments.__args[name] = value
-
-    @staticmethod
-    def get(name=None):
-        """Retrieve a specified attribute.
-
-        :param name: name of attribute to retrieve value of or none to return all
-        :return: value of requested attribute, or all attributes if none provided
-        """
-        if name is None:
-            return Arguments.__args
-
-        return Arguments.__args[name]
+"""
+Handles parsing and storage of arguments passed to twitch-archiver.
+"""
+
+import re
+import sys
+
+from pathlib import Path
+
+
+class Arguments:
+    """
+    Function for parsing arguments for access later.
+    """
+    __args = {}
+
+    @staticmethod
+    def setup_args(args):
+        """Sets up and formats provided arguments.
+
+        :param args: arguments object to create parameters from
+        """
+        for argument in args:
+            Arguments.set(argument, args[argument])
+
+        if Arguments.get('show_config'):
+            try:
+                with open(Path(Arguments.get('config_dir'), 'config.ini'), 'r', encoding='utf8') as config:
+                    print(config.read())
+                    sys.exit(0)
+            except FileNotFoundError:
+                sys.exit('Config not found. Run Twitch-Archiver once with your Client ID and Secret to generate one.')
+
+        # validate mutual exclusivity of arguments passed via CLI and environment variables
+        # required as values set via environment variables bypass argparse mutex handling
+        for mutex_args in (("vod_id", "channel"), ("live_only", "archive_only")):
+            mutex_arg_0, mutex_arg_1 = Arguments.get(mutex_args[0]), Arguments.get(mutex_args[1])
+            # check if both mutex args have a value (including empty string)
+            if mutex_arg_0 is not None and mutex_arg_1 is not None:
+                raise ValueError("Cannot accept both of the following mutually exclusive arguments: '"
+                                 f"{mutex_args[0]}={mutex_arg_0}' and '{mutex_args[1]}={mutex_arg_1}'")
+
+        # get both video and chat logs if neither selected
+        if not Arguments.get('chat') and not Arguments.get('video'):
+            Arguments.set('chat', True)
+            Arguments.set('video', True)
+
+        # generate list from comma-separated vods
+        if Arguments.get('vod_id'):
+            # generate vod list
+            vod_ids = list(Arguments.get('vod_id').split(','))
+
+            # format urls to just vod ids
+            for idx, vod_id in enumerate(vod_ids):
+                # test match and replace
+                match = re.findall(r"(?<=twitch\.tv/videos/)[0-9]*", vod_id)
+                if match:
+                    vod_ids[idx] = match[0]
+
+            # insert formatted vods
+            Arguments.set('vod_id', vod_ids)
+
+        # generate list from comma-separated channels
+        elif Arguments.get('channel'):
+            # generate channel list
+            channels = list(Arguments.get('channel').split(','))
+
+            # format urls to just channel name
+            for idx, channel in enumerate(channels):
+                # test and replace
+                match = re.findall(r"(?<=twitch\.tv/)[a-zA-Z0-9]*", channel)
+                if match:
+                    channels[idx] = match[0]
+
+            # insert formatted channels
+            Arguments.set('channel', channels)
+
+        # split quality into [resolution, framerate]
+        if Arguments.get('quality') not in ['best', 'worst']:
+            Arguments.set('quality', Arguments.get('quality').split('p'))
+
+        if Arguments.get('watch'):
+            print('Launching Twitch-Archiver in watch mode.')
+
+    @staticmethod
+    def set(name, value):
+        """Set a specified class attribute.
+
+        :param name: name of attribute to change
+        :param value: value to set attribute to
+        """
+        Arguments.__args[name] = value
+
+    @staticmethod
+    def get(name=None):
+        """Retrieve a specified attribute.
+
+        :param name: name of attribute to retrieve value of or none to return all
+        :return: value of requested attribute, or all attributes if none provided
+        """
+        if name is None:
+            return Arguments.__args
+
+        return Arguments.__args[name]
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/configuration.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/configuration.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-"""
-Module for generating, saving and retrieving configuration values.
-"""
-
-import configparser
-import logging
-import os
-
-
-class Configuration:
-    """
-    Generation, saving and loading of twitch-archive configuration.
-    """
-    # reference:
-    #   https://stackoverflow.com/questions/6198372/most-pythonic-way-to-provide-global-configuration-variables-in-config-py/
-    __conf = {
-        'client_id': '',
-        'client_secret': '',
-        'oauth_token': '',
-        'pushbullet_key': '',
-    }
-
-    def __init__(self):
-
-        self.log = logging.getLogger()
-
-    def generate_config(self, args):
-        """Generates the required configuration from provided arguments, overwriting loaded settings.
-
-        :param args: arguments to generate config from
-        """
-        self.log.debug('Generating config from provided arguments.')
-
-        # if setting loaded from config differs from passed arg (and arg is not none), overwrite it
-        for argument in args:
-            if argument in self.get() and args.get(argument) != self.get(argument) \
-                    and args.get(argument) not in [None, False]:
-                self.set(argument, args.get(argument))
-
-    def load_config(self, conf_file):
-        """Loads the settings stored in the configuration ini file.
-
-        :param conf_file: path to configuration file
-        """
-        # create conf file if it doesn't exist
-        if not os.path.isfile(conf_file):
-            self.log.debug('Config file not found - creating one now.')
-            self.create_config_file(conf_file)
-
-        self.log.debug('Loading config from file.')
-
-        config = configparser.ConfigParser()
-        config.read(conf_file)
-
-        # load individual settings from file
-        for setting in config['settings']:
-            self.set(setting, config['settings'][setting])
-
-    def create_config_file(self, conf_file):
-        """Creates a configuration file for the storing of settings.\n
-
-        :param conf_file: path to configuration file
-        """
-        self.log.debug('Creating directories for configuration file.')
-        os.makedirs(conf_file.parent, exist_ok=True)
-
-        config = configparser.ConfigParser()
-        config.add_section('settings')
-        self.log.debug('Current config: %s', self.get())
-
-        for setting in self.__conf:
-            config.set('settings', setting, self.get(setting))
-
-        self.log.debug('Writing config to %s', conf_file)
-
-        with open(conf_file, 'w', encoding='utf8') as f:
-            config.write(f)
-
-    @staticmethod
-    def set(name, value):
-        """Set a specified attribute.
-
-        :param name:  name of attribute to change
-        :param value: value to set attribute to
-        """
-        if name in Configuration.__conf:
-            Configuration.__conf[name] = value
-
-        else:
-            raise NameError("Configuration variable not found.")
-
-    @staticmethod
-    def get(name=None):
-        """Retrieve a specified attribute.
-
-        :param name: name of attribute to retrieve value of - 'None' returns all attributes
-        :return: requested value(s)
-        """
-        if name is None:
-            return Configuration.__conf
-
-        return Configuration.__conf[name]
-
-    @staticmethod
-    def get_sanitized(name=None):
-        """Retrieves a specified attribute, sanitizing secrets.
-
-        :param name: name of attribute to retrieve value of - 'None' returns all attributes
-        :return: requested value(s)
-        """
-        configuration = Configuration.__conf.copy()
-        for key in ['client_id', 'client_secret', 'oauth_token', 'pushbullet_key']:
-            if configuration[key] != '':
-                configuration.update({key: 24 * '*' + configuration[key][24:]})
-
-        if name is None:
-            return configuration
-
-        return configuration[name]
-
-    # reference:
-    #   https://stackoverflow.com/questions/35247900/python-creating-an-ini-or-config-file-in-the-users-home-directory
-    def save(self, conf_file, name=None):
-        """
-        Saves the running configuration to the configuration ini.
-        """
-        self.log.debug('Saving config variable(s) to ini file.')
-
-        # import saved config
-        config = configparser.ConfigParser()
-        config.read(conf_file)
-
-        # overwrite all vars
-        if name is None:
-            # overwrite with running config
-            for setting in Configuration.get():
-                config.set('settings', setting, str(Configuration.get(setting)))
-
-            # save to disk
-            with open(conf_file, 'w', encoding='utf8') as f:
-                config.write(f)
-
-        # overwrite one var
-        else:
-            config.set('settings', name, str(Configuration.get(name)))
-
-            # save to disk
-            with open(conf_file, 'w', encoding='utf8') as f:
-                config.write(f)
+"""
+Module for generating, saving and retrieving configuration values.
+"""
+
+import configparser
+import logging
+import os
+
+
+class Configuration:
+    """
+    Generation, saving and loading of twitch-archive configuration.
+    """
+    # reference:
+    #   https://stackoverflow.com/questions/6198372/most-pythonic-way-to-provide-global-configuration-variables-in-config-py/
+    __conf = {
+        'client_id': '',
+        'client_secret': '',
+        'oauth_token': '',
+        'pushbullet_key': '',
+    }
+
+    def __init__(self):
+
+        self.log = logging.getLogger()
+
+    def generate_config(self, args):
+        """Generates the required configuration from provided arguments, overwriting loaded settings.
+
+        :param args: arguments to generate config from
+        """
+        self.log.debug('Generating config from provided arguments.')
+
+        # if setting loaded from config differs from passed arg (and arg is not none), overwrite it
+        for argument in args:
+            if argument in self.get() and args.get(argument) != self.get(argument) \
+                    and args.get(argument) not in [None, False]:
+                self.set(argument, args.get(argument))
+
+    def load_config(self, conf_file):
+        """Loads the settings stored in the configuration ini file.
+
+        :param conf_file: path to configuration file
+        """
+        # create conf file if it doesn't exist
+        if not os.path.isfile(conf_file):
+            self.log.debug('Config file not found - creating one now.')
+            self.create_config_file(conf_file)
+
+        self.log.debug('Loading config from file.')
+
+        config = configparser.ConfigParser()
+        config.read(conf_file)
+
+        # load individual settings from file
+        for setting in config['settings']:
+            self.set(setting, config['settings'][setting])
+
+    def create_config_file(self, conf_file):
+        """Creates a configuration file for the storing of settings.\n
+
+        :param conf_file: path to configuration file
+        """
+        self.log.debug('Creating directories for configuration file.')
+        os.makedirs(conf_file.parent, exist_ok=True)
+
+        config = configparser.ConfigParser()
+        config.add_section('settings')
+        self.log.debug('Current config: %s', self.get())
+
+        for setting in self.__conf:
+            config.set('settings', setting, self.get(setting))
+
+        self.log.debug('Writing config to %s', conf_file)
+
+        with open(conf_file, 'w', encoding='utf8') as f:
+            config.write(f)
+
+    @staticmethod
+    def set(name, value):
+        """Set a specified attribute.
+
+        :param name:  name of attribute to change
+        :param value: value to set attribute to
+        """
+        if name in Configuration.__conf:
+            Configuration.__conf[name] = value
+
+        else:
+            raise NameError("Configuration variable not found.")
+
+    @staticmethod
+    def get(name=None):
+        """Retrieve a specified attribute.
+
+        :param name: name of attribute to retrieve value of - 'None' returns all attributes
+        :return: requested value(s)
+        """
+        if name is None:
+            return Configuration.__conf
+
+        return Configuration.__conf[name]
+
+    @staticmethod
+    def get_sanitized(name=None):
+        """Retrieves a specified attribute, sanitizing secrets.
+
+        :param name: name of attribute to retrieve value of - 'None' returns all attributes
+        :return: requested value(s)
+        """
+        configuration = Configuration.__conf.copy()
+        for key in ['client_id', 'client_secret', 'oauth_token', 'pushbullet_key']:
+            if configuration[key] != '':
+                configuration.update({key: 24 * '*' + configuration[key][24:]})
+
+        if name is None:
+            return configuration
+
+        return configuration[name]
+
+    # reference:
+    #   https://stackoverflow.com/questions/35247900/python-creating-an-ini-or-config-file-in-the-users-home-directory
+    def save(self, conf_file, name=None):
+        """
+        Saves the running configuration to the configuration ini.
+        """
+        self.log.debug('Saving config variable(s) to ini file.')
+
+        # import saved config
+        config = configparser.ConfigParser()
+        config.read(conf_file)
+
+        # overwrite all vars
+        if name is None:
+            # overwrite with running config
+            for setting in Configuration.get():
+                config.set('settings', setting, str(Configuration.get(setting)))
+
+            # save to disk
+            with open(conf_file, 'w', encoding='utf8') as f:
+                config.write(f)
+
+        # overwrite one var
+        else:
+            config.set('settings', name, str(Configuration.get(name)))
+
+            # save to disk
+            with open(conf_file, 'w', encoding='utf8') as f:
+                config.write(f)
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/database.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/database.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-"""
-Module used for creating, accessing, updating and modifying database entries.
-"""
-
-import logging
-import sqlite3
-
-from sqlite3 import Error
-
-from twitcharchiver.exceptions import DatabaseError, DatabaseQueryError
-
-__db_version__ = 4
-
-
-class Database:
-    """
-    Functions for interacting with the VOD database.
-    """
-    def __init__(self, database_path):
-        """Class constructor.
-
-        :param database_path: path to database file
-        """
-        self.log = logging.getLogger()
-
-        self.database_path = str(database_path)
-
-        try:
-            self.log.debug('Database path: %s', self.database_path)
-            self.connection = sqlite3.connect(self.database_path)
-            self.cursor = self.connection.cursor()
-            self.log.debug('Connection to SQLite DB successful.')
-
-        except Error as e:
-            raise DatabaseError(f'Connection to SQLite DB failed: {e}') from e
-
-    def setup_database(self):
-        """
-        Sets up VODs table.
-        """
-        self.log.debug("Setting up vods table if it doesn't already exist.")
-
-        with Database(self.database_path) as db:
-            [db.execute_query(query) for query in create_vods_table]
-
-    def update_database(self, version):
-        """
-        Updates database to given version.
-
-        :param version: desired version to upgrade to
-        """
-        self.log.debug("Setting up vods table if it doesn't already exist.")
-
-        if version == 2:
-            with Database(self.database_path) as db:
-                [db.execute_query(query) for query in version_2_to_3_upgrade]
-
-        if version == 3:
-            with Database(self.database_path) as db:
-                [db.execute_query(query) for query in version_3_to_4_upgrade]
-
-    # reference:
-    #   https://codereview.stackexchange.com/questions/182700/python-class-to-manage-a-table-in-sqlite
-    def __enter__(self):
-        return self
-
-    def __exit__(self, ext_type, exc_value, traceback):
-
-        self.cursor.close()
-        if isinstance(exc_value, Exception):
-            self.connection.rollback()
-            self.connection.close()
-            raise DatabaseError(exc_value)
-
-        self.connection.commit()
-        self.connection.close()
-
-    def execute_query(self, command, values=None):
-        """Executes a given SQL statement.
-
-        :param command: sql query to execute
-        :param values: values to pass if inserting data - 'None' sends no other data
-        :return: response from sqlite database to statement
-        """
-        self.log.debug('Executing SQL statement: %s', command)
-
-        try:
-            if not values:
-                _r = self.cursor.execute(command).fetchall()
-            else:
-                self.log.debug('Values: %s', values)
-                _r = self.cursor.execute(command, list(values.values())).fetchall()
-
-        except Exception as e:
-            raise DatabaseQueryError(str(e)) from e
-
-        return _r
-
-
-create_vods_table = [
-    """CREATE TABLE "vods" (
-        "vod_id"            INTEGER,
-        "stream_id"         INTEGER,
-        "user_id"           INTEGER,
-        "user_login"        TEXT,
-        "user_name"         TEXT,
-        "title"             TEXT,
-        "description"       TEXT,
-        "created_at"        DATETIME,
-        "published_at"      DATETIME,
-        "url"               TEXT,
-        "thumbnail_url"     TEXT,
-        "viewable"          TEXT,
-        "view_count"        TEXT,
-        "language"          TEXT,
-        "type"              TEXT,
-        "duration"          INTEGER,
-        "muted_segments"    TEXT,
-        "store_directory"   TEXT,
-        "video_archived"    BIT,
-        "chat_archived"     BIT,
-        PRIMARY KEY("vod_id","stream_id")
-    );""",
-    f"PRAGMA user_version = {__db_version__};"]
-
-CREATE_VOD = """
-INSERT INTO
-vods (stream_id, user_id, user_login, user_name, title, description, created_at, published_at, url, thumbnail_url,
-      viewable, view_count, language, type, duration, muted_segments, vod_id, store_directory, video_archived,
-      chat_archived)
-VALUES
-(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);
-"""
-
-UPDATE_VOD = """
-UPDATE vods
-SET stream_id=?, user_id=?, user_login=?, user_name=?, title=?, description=?, created_at=?,
-    published_at=?, url=?, thumbnail_url=?, viewable=?, view_count=?, language=?, type=?,
-    duration=?, muted_segments=?, vod_id=?, store_directory=?, video_archived=?, chat_archived=?
-WHERE stream_id IS ?;
-"""
-
-# change pk from id to user_id + created_at
-# change type of created_at, published_at from TEXT to DATETIME
-version_2_to_3_upgrade = [
-    "ALTER TABLE vods RENAME TO vods_bak;",
-    """CREATE TABLE "vods" (
-        "id"                INTEGER,
-        "stream_id"         INTEGER,
-        "user_id"           INTEGER,
-        "user_login"        TEXT,
-        "user_name"         TEXT,
-        "title"             TEXT,
-        "description"       TEXT,
-        "created_at"        DATETIME,
-        "published_at"      DATETIME,
-        "url"               TEXT,
-        "thumbnail_url"     TEXT,
-        "viewable"          TEXT,
-        "view_count"        TEXT,
-        "language"          TEXT,
-        "type"              TEXT,
-        "duration"          TEXT,
-        "muted_segments"    TEXT,
-        "store_directory"   TEXT,
-        "duration_seconds"  INTEGER,
-        PRIMARY KEY("user_id","created_at")
-    );""",
-    "INSERT INTO vods SELECT * FROM vods_bak;",
-    "DROP TABLE vods_bak;",
-    "PRAGMA user_version = 3;"]
-
-# renamed id -> vod_id
-# changed pk from user_id + created_at -> vod_id + stream_id
-#   older vods do not have a stream id, so the vod_id will be copied in its place
-# changed duration column type from TEXT -> INTEGER
-#   duration_seconds will replace the current value
-# removed duration_seconds column
-# add video_archived and chat_archived columns
-#   these are both set to 1 (true) for already archived streams
-version_3_to_4_upgrade = [
-    "ALTER TABLE vods RENAME TO vods_bak;",
-    "UPDATE vods_bak SET stream_id = id WHERE stream_id IS NULL;",
-    """CREATE TABLE "vods" (
-        "vod_id"            INTEGER,
-        "stream_id"         INTEGER,
-        "user_id"           INTEGER,
-        "user_login"        TEXT,
-        "user_name"         TEXT,
-        "title"             TEXT,
-        "description"       TEXT,
-        "created_at"        DATETIME,
-        "published_at"      DATETIME,
-        "url"               TEXT,
-        "thumbnail_url"     TEXT,
-        "viewable"          TEXT,
-        "view_count"        TEXT,
-        "language"          TEXT,
-        "type"              TEXT,
-        "duration"          INTEGER,
-        "muted_segments"    TEXT,
-        "store_directory"   TEXT,
-        "video_archived"    BIT,
-        "chat_archived"     BIT,
-        PRIMARY KEY("vod_id","stream_id")
-    );""",
-    "INSERT INTO vods SELECT id, stream_id, user_id, user_login, user_name, title, description, created_at, "
-    "published_at, url, thumbnail_url, viewable, view_count, language, type, duration_seconds, muted_segments, "
-    "store_directory, 1, 1 FROM vods_bak;",
-    "DROP TABLE vods_bak;",
-    "PRAGMA user_version = 4;"]
+"""
+Module used for creating, accessing, updating and modifying database entries.
+"""
+
+import logging
+import sqlite3
+
+from sqlite3 import Error
+
+from twitcharchiver.exceptions import DatabaseError, DatabaseQueryError
+
+__db_version__ = 4
+
+
+class Database:
+    """
+    Functions for interacting with the VOD database.
+    """
+    def __init__(self, database_path):
+        """Class constructor.
+
+        :param database_path: path to database file
+        """
+        self.log = logging.getLogger()
+
+        self.database_path = str(database_path)
+
+        try:
+            self.log.debug('Database path: %s', self.database_path)
+            self.connection = sqlite3.connect(self.database_path)
+            self.cursor = self.connection.cursor()
+            self.log.debug('Connection to SQLite DB successful.')
+
+        except Error as e:
+            raise DatabaseError(f'Connection to SQLite DB failed: {e}') from e
+
+    def setup_database(self):
+        """
+        Sets up VODs table.
+        """
+        self.log.debug("Setting up vods table if it doesn't already exist.")
+
+        with Database(self.database_path) as db:
+            [db.execute_query(query) for query in create_vods_table]
+
+    def update_database(self, version):
+        """
+        Updates database to given version.
+
+        :param version: desired version to upgrade to
+        """
+        self.log.debug("Setting up vods table if it doesn't already exist.")
+
+        if version == 2:
+            with Database(self.database_path) as db:
+                [db.execute_query(query) for query in version_2_to_3_upgrade]
+
+        if version == 3:
+            with Database(self.database_path) as db:
+                [db.execute_query(query) for query in version_3_to_4_upgrade]
+
+    # reference:
+    #   https://codereview.stackexchange.com/questions/182700/python-class-to-manage-a-table-in-sqlite
+    def __enter__(self):
+        return self
+
+    def __exit__(self, ext_type, exc_value, traceback):
+
+        self.cursor.close()
+        if isinstance(exc_value, Exception):
+            self.connection.rollback()
+            self.connection.close()
+            raise DatabaseError(exc_value)
+
+        self.connection.commit()
+        self.connection.close()
+
+    def execute_query(self, command, values=None):
+        """Executes a given SQL statement.
+
+        :param command: sql query to execute
+        :param values: values to pass if inserting data - 'None' sends no other data
+        :return: response from sqlite database to statement
+        """
+        self.log.debug('Executing SQL statement: %s', command)
+
+        try:
+            if not values:
+                _r = self.cursor.execute(command).fetchall()
+            else:
+                self.log.debug('Values: %s', values)
+                _r = self.cursor.execute(command, list(values.values())).fetchall()
+
+        except Exception as e:
+            raise DatabaseQueryError(str(e)) from e
+
+        return _r
+
+
+create_vods_table = [
+    """CREATE TABLE "vods" (
+        "vod_id"            INTEGER,
+        "stream_id"         INTEGER,
+        "user_id"           INTEGER,
+        "user_login"        TEXT,
+        "user_name"         TEXT,
+        "title"             TEXT,
+        "description"       TEXT,
+        "created_at"        DATETIME,
+        "published_at"      DATETIME,
+        "url"               TEXT,
+        "thumbnail_url"     TEXT,
+        "viewable"          TEXT,
+        "view_count"        TEXT,
+        "language"          TEXT,
+        "type"              TEXT,
+        "duration"          INTEGER,
+        "muted_segments"    TEXT,
+        "store_directory"   TEXT,
+        "video_archived"    BIT,
+        "chat_archived"     BIT,
+        PRIMARY KEY("vod_id","stream_id")
+    );""",
+    f"PRAGMA user_version = {__db_version__};"]
+
+CREATE_VOD = """
+INSERT INTO
+vods (stream_id, user_id, user_login, user_name, title, description, created_at, published_at, url, thumbnail_url,
+      viewable, view_count, language, type, duration, muted_segments, vod_id, store_directory, video_archived,
+      chat_archived)
+VALUES
+(?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?);
+"""
+
+UPDATE_VOD = """
+UPDATE vods
+SET stream_id=?, user_id=?, user_login=?, user_name=?, title=?, description=?, created_at=?,
+    published_at=?, url=?, thumbnail_url=?, viewable=?, view_count=?, language=?, type=?,
+    duration=?, muted_segments=?, vod_id=?, store_directory=?, video_archived=?, chat_archived=?
+WHERE stream_id IS ?;
+"""
+
+# change pk from id to user_id + created_at
+# change type of created_at, published_at from TEXT to DATETIME
+version_2_to_3_upgrade = [
+    "ALTER TABLE vods RENAME TO vods_bak;",
+    """CREATE TABLE "vods" (
+        "id"                INTEGER,
+        "stream_id"         INTEGER,
+        "user_id"           INTEGER,
+        "user_login"        TEXT,
+        "user_name"         TEXT,
+        "title"             TEXT,
+        "description"       TEXT,
+        "created_at"        DATETIME,
+        "published_at"      DATETIME,
+        "url"               TEXT,
+        "thumbnail_url"     TEXT,
+        "viewable"          TEXT,
+        "view_count"        TEXT,
+        "language"          TEXT,
+        "type"              TEXT,
+        "duration"          TEXT,
+        "muted_segments"    TEXT,
+        "store_directory"   TEXT,
+        "duration_seconds"  INTEGER,
+        PRIMARY KEY("user_id","created_at")
+    );""",
+    "INSERT INTO vods SELECT * FROM vods_bak;",
+    "DROP TABLE vods_bak;",
+    "PRAGMA user_version = 3;"]
+
+# renamed id -> vod_id
+# changed pk from user_id + created_at -> vod_id + stream_id
+#   older vods do not have a stream id, so the vod_id will be copied in its place
+# changed duration column type from TEXT -> INTEGER
+#   duration_seconds will replace the current value
+# removed duration_seconds column
+# add video_archived and chat_archived columns
+#   these are both set to 1 (true) for already archived streams
+version_3_to_4_upgrade = [
+    "ALTER TABLE vods RENAME TO vods_bak;",
+    "UPDATE vods_bak SET stream_id = id WHERE stream_id IS NULL;",
+    """CREATE TABLE "vods" (
+        "vod_id"            INTEGER,
+        "stream_id"         INTEGER,
+        "user_id"           INTEGER,
+        "user_login"        TEXT,
+        "user_name"         TEXT,
+        "title"             TEXT,
+        "description"       TEXT,
+        "created_at"        DATETIME,
+        "published_at"      DATETIME,
+        "url"               TEXT,
+        "thumbnail_url"     TEXT,
+        "viewable"          TEXT,
+        "view_count"        TEXT,
+        "language"          TEXT,
+        "type"              TEXT,
+        "duration"          INTEGER,
+        "muted_segments"    TEXT,
+        "store_directory"   TEXT,
+        "video_archived"    BIT,
+        "chat_archived"     BIT,
+        PRIMARY KEY("vod_id","stream_id")
+    );""",
+    "INSERT INTO vods SELECT id, stream_id, user_id, user_login, user_name, title, description, created_at, "
+    "published_at, url, thumbnail_url, viewable, view_count, language, type, duration_seconds, muted_segments, "
+    "store_directory, 1, 1 FROM vods_bak;",
+    "DROP TABLE vods_bak;",
+    "PRAGMA user_version = 4;"]
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/downloader.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/downloader.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,251 +1,251 @@
-"""
-Module used for downloading archived videos and chat logs from Twitch.
-"""
-
-from glob import glob
-import json
-import logging
-import os
-import tempfile
-
-from concurrent.futures import ThreadPoolExecutor
-from pathlib import Path
-
-import requests
-
-from twitcharchiver.api import Api
-from twitcharchiver.exceptions import VodPartDownloadError, TwitchAPIErrorNotFound, ChatDownloadError, RequestError
-from twitcharchiver.utils import Progress, to_ranges, safe_move
-
-
-class Downloader:
-    """
-    Functions used for the downloading of video and chat from Twitch VODs.
-    """
-    def __init__(self, client_id, oauth_token, threads=20, quiet=False):
-        """
-
-        :param client_id: twitch client id
-        :param oauth_token: oauth token retrieved with client id and secret
-        :param threads: number of download threads
-        :param quiet: hide progress bars
-        """
-
-        self.log = logging.getLogger()
-
-        self.client_id = client_id
-        self.oauth_token = oauth_token
-
-        self.threads = threads
-        self.quiet = quiet
-
-    def get_m3u8_video(self, m3u8_playlist, m3u8_base_url, store_directory):
-        """Downloads the video for a specified m3u8 playlist.
-
-        :param m3u8_playlist: m3u8 playlist to retrieve video from
-        :param m3u8_base_url: url from which .ts files are derived from
-        :param store_directory: location to store downloaded segments
-        :raises vodPartDownloadError: error returned when downloading vod parts
-        """
-        Path(store_directory, 'parts').mkdir(parents=True, exist_ok=True)
-
-        ts_url_list = []
-        ts_path_list = []
-        muted_segments = []
-
-        # collect ids of all downloaded parts
-        downloaded_ids = [str(Path(p).name)[:4].lstrip('0') + str(Path(p).name)[4:]
-                          for p in glob(str(Path(store_directory, 'parts', '*.ts')))]
-
-        # process all ids in playlist
-        for ts_id in [s.uri for s in m3u8_playlist.segments]:
-            if '-unmuted' in ts_id:
-                # rename segments as their url remains unchanged after being unmuted
-                ts_id = ts_id.replace('-unmuted', '-muted')
-
-            # store all muted segments
-            if '-muted' in ts_id:
-                muted_segments.append(int(ts_id.replace('-muted.ts', '')))
-
-            # append ts_id to to-download list if it isn't already downloaded
-            if ts_id.replace('-muted', '') not in downloaded_ids:
-                # create a tuple with (TS_URL, TS_PATH)
-                ts_url_list.append(m3u8_base_url + ts_id)
-                ts_path_list.append(Path(store_directory, 'parts',
-                                         str(f'{int(ts_id.split(".")[0].replace("-muted", "")):05d}' + '.ts')))
-
-        # export list of muted ids if present
-        with open(Path(store_directory, 'parts', '.muted'), 'w', encoding='utf8') as mutefile:
-            json.dump(list(to_ranges(muted_segments)), mutefile)
-
-        if ts_url_list and ts_path_list:
-            # create worker pool for downloading vods
-            with ThreadPoolExecutor(max_workers=self.threads) as pool:
-                download_error = []
-                futures = []
-                ct = 0
-                # append work orders along with args to queue
-                for ts_url, ts_path in zip(ts_url_list, ts_path_list):
-                    futures.append(pool.submit(self.get_ts_segment, ts_url, ts_path))
-
-                progress = Progress()
-
-                # process queue
-                for future in futures:
-                    if future.result():
-                        # append any returned errors
-                        download_error.append(future.result())
-                        continue
-
-                    ct += 1
-                    if not self.quiet:
-                        progress.print_progress(ct, len(ts_url_list))
-
-            if download_error:
-                raise VodPartDownloadError(download_error)
-
-    def get_ts_segment(self, ts_url, ts_path):
-        """Retrieves a specific ts file.
-
-        :param ts_url: url of .ts file to download
-        :param ts_path: destination path for .ts file after downloading
-        :return: error on failure
-        """
-        self.log.debug('Downloading segment %s to %s', ts_url, ts_path)
-
-        # don't bother if piece already downloaded
-        if os.path.exists(ts_path):
-            return False
-
-        # files are downloaded to $TMP, then moved to final destination
-        # takes 3:32 to download an hour long VOD to NAS, compared to 5:00 without using $TMP as download cache
-        #   a better method would be to have 20 workers downloading, and 20 moving temp
-        #   files from storage avoiding any downtime downloading
-
-        # create temporary file for downloading to
-        with open(Path(tempfile.gettempdir(), os.urandom(24).hex()), 'wb') as tmp_ts_file:
-            for _ in range(6):
-                if _ > 4:
-                    self.log.debug('Maximum retries for segment %s reached.', Path(ts_path).stem)
-                    return {1, f'Maximum retries for segment {Path(ts_path).stem} reached.'}
-
-                try:
-                    _r = requests.get(ts_url, stream=True, timeout=10)
-
-                    # break on non 200 status code
-                    if _r.status_code != 200:
-                        self.log.error('Code other than 200 received when trying to download segment.')
-                        continue
-
-                    # write downloaded chunks to temporary file
-                    for chunk in _r.iter_content(chunk_size=262144):
-                        tmp_ts_file.write(chunk)
-
-                    self.log.debug('Segment %s download completed.', Path(ts_path).stem)
-
-                    break
-
-                except requests.exceptions.RequestException as e:
-                    self.log.debug('Segment %s download failed (Attempt %s). Error: %s)',
-                                   Path(ts_path).stem, _ + 1, str(e))
-                    continue
-
-        try:
-            # move part to destination storage
-            safe_move(tmp_ts_file.name, ts_path)
-            self.log.debug('Segment %s completed.', Path(ts_path).stem)
-
-        except FileNotFoundError as e:
-            raise VodPartDownloadError(f'MPEG-TS segment did not download correctly. Piece: {ts_url}') from e
-
-        except BaseException as e:
-            self.log.error('Exception encountered while moving downloaded MPEG-TS segment %s.', ts_url, exc_info=True)
-            return e
-
-        return False
-
-    def get_chat(self, vod_json, offset=0):
-        """Downloads the chat for a specified VOD, returning comments beginning from offset (if provided).
-
-        :param vod_json: dict of vod information
-        :param offset: offset in seconds to begin chat retrieval from - none to begin at start
-        """
-        chat_log = []
-
-        _s = requests.session()
-        _s.headers.update({'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'})
-
-        # grab initial chat segment containing cursor
-        initial_segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], offset=offset)
-        chat_log.extend(initial_segment)
-
-        progress = Progress()
-
-        while True:
-            if not cursor:
-                break
-
-            try:
-                # grab next chat segment along with cursor for next segment
-                segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], cursor=cursor)
-                chat_log.extend(segment)
-                # vod duration in seconds is used as the total for progress bar
-                # comment offset is used to track what's been done
-                # could be done properly if there was a way to get the total number of comments
-                if not self.quiet:
-                    progress.print_progress(int(segment[-1]['contentOffsetSeconds']),
-                                            vod_json['duration'], not cursor)
-
-            except TwitchAPIErrorNotFound:
-                break
-
-            finally:
-                _s.close()
-
-        self.log.info('Found %s messages.', len(chat_log))
-
-        return chat_log
-
-    def get_chat_segment(self, session, vod_id, offset=None, cursor=None):
-        """Retrieves a single chat segment.
-
-        :param session: requests session to link request to
-        :param vod_id: id of vod to retrieve segment from
-        :param offset: offset in seconds to begin retrieval from
-        :param cursor: cursor returned by a previous call of this function
-        :return: list of comments and cursor if one is returned from twitch
-        """
-        # build payload
-        if offset is not None:
-            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
-                   "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
-
-        else:
-            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
-                   "variables": {"videoID": vod_id, "cursor": cursor}}]
-
-        _p[0]['extensions'] =\
-            {'persistedQuery': {'version': 1,
-                                'sha256Hash': "b70a3591ff0f4e0313d126c6a1502d79a1c02baebb288227c582044aa76adf6a"}}
-
-        for attempt in range(6):
-            if attempt > 4:
-                self.log.error('Maximum attempts reached while downloading chat segment at cursor or offset: %s, %s.',
-                               cursor, offset)
-                raise ChatDownloadError
-
-            try:
-                _r = Api.post_request_with_session('https://gql.twitch.tv/gql', session, _p).json()
-
-            except RequestError:
-                continue
-
-            break
-
-        comments = _r[0]['data']['video']['comments']
-
-        # check if next page exists
-        if comments['pageInfo']['hasNextPage']:
-            return [c['node'] for c in comments['edges']], comments['edges'][-1]['cursor']
-
-        return [c['node'] for c in comments['edges']], None
+"""
+Module used for downloading archived videos and chat logs from Twitch.
+"""
+
+from glob import glob
+import json
+import logging
+import os
+import tempfile
+
+from concurrent.futures import ThreadPoolExecutor
+from pathlib import Path
+
+import requests
+
+from twitcharchiver.api import Api
+from twitcharchiver.exceptions import VodPartDownloadError, TwitchAPIErrorNotFound, ChatDownloadError, RequestError
+from twitcharchiver.utils import Progress, to_ranges, safe_move
+
+
+class Downloader:
+    """
+    Functions used for the downloading of video and chat from Twitch VODs.
+    """
+    def __init__(self, client_id, oauth_token, threads=20, quiet=False):
+        """
+
+        :param client_id: twitch client id
+        :param oauth_token: oauth token retrieved with client id and secret
+        :param threads: number of download threads
+        :param quiet: hide progress bars
+        """
+
+        self.log = logging.getLogger()
+
+        self.client_id = client_id
+        self.oauth_token = oauth_token
+
+        self.threads = threads
+        self.quiet = quiet
+
+    def get_m3u8_video(self, m3u8_playlist, m3u8_base_url, store_directory):
+        """Downloads the video for a specified m3u8 playlist.
+
+        :param m3u8_playlist: m3u8 playlist to retrieve video from
+        :param m3u8_base_url: url from which .ts files are derived from
+        :param store_directory: location to store downloaded segments
+        :raises vodPartDownloadError: error returned when downloading vod parts
+        """
+        Path(store_directory, 'parts').mkdir(parents=True, exist_ok=True)
+
+        ts_url_list = []
+        ts_path_list = []
+        muted_segments = []
+
+        # collect ids of all downloaded parts
+        downloaded_ids = [str(Path(p).name)[:4].lstrip('0') + str(Path(p).name)[4:]
+                          for p in glob(str(Path(store_directory, 'parts', '*.ts')))]
+
+        # process all ids in playlist
+        for ts_id in [s.uri for s in m3u8_playlist.segments]:
+            if '-unmuted' in ts_id:
+                # rename segments as their url remains unchanged after being unmuted
+                ts_id = ts_id.replace('-unmuted', '-muted')
+
+            # store all muted segments
+            if '-muted' in ts_id:
+                muted_segments.append(int(ts_id.replace('-muted.ts', '')))
+
+            # append ts_id to to-download list if it isn't already downloaded
+            if ts_id.replace('-muted', '') not in downloaded_ids:
+                # create a tuple with (TS_URL, TS_PATH)
+                ts_url_list.append(m3u8_base_url + ts_id)
+                ts_path_list.append(Path(store_directory, 'parts',
+                                         str(f'{int(ts_id.split(".")[0].replace("-muted", "")):05d}' + '.ts')))
+
+        # export list of muted ids if present
+        with open(Path(store_directory, 'parts', '.muted'), 'w', encoding='utf8') as mutefile:
+            json.dump(list(to_ranges(muted_segments)), mutefile)
+
+        if ts_url_list and ts_path_list:
+            # create worker pool for downloading vods
+            with ThreadPoolExecutor(max_workers=self.threads) as pool:
+                download_error = []
+                futures = []
+                ct = 0
+                # append work orders along with args to queue
+                for ts_url, ts_path in zip(ts_url_list, ts_path_list):
+                    futures.append(pool.submit(self.get_ts_segment, ts_url, ts_path))
+
+                progress = Progress()
+
+                # process queue
+                for future in futures:
+                    if future.result():
+                        # append any returned errors
+                        download_error.append(future.result())
+                        continue
+
+                    ct += 1
+                    if not self.quiet:
+                        progress.print_progress(ct, len(ts_url_list))
+
+            if download_error:
+                raise VodPartDownloadError(download_error)
+
+    def get_ts_segment(self, ts_url, ts_path):
+        """Retrieves a specific ts file.
+
+        :param ts_url: url of .ts file to download
+        :param ts_path: destination path for .ts file after downloading
+        :return: error on failure
+        """
+        self.log.debug('Downloading segment %s to %s', ts_url, ts_path)
+
+        # don't bother if piece already downloaded
+        if os.path.exists(ts_path):
+            return False
+
+        # files are downloaded to $TMP, then moved to final destination
+        # takes 3:32 to download an hour long VOD to NAS, compared to 5:00 without using $TMP as download cache
+        #   a better method would be to have 20 workers downloading, and 20 moving temp
+        #   files from storage avoiding any downtime downloading
+
+        # create temporary file for downloading to
+        with open(Path(tempfile.gettempdir(), os.urandom(24).hex()), 'wb') as tmp_ts_file:
+            for _ in range(6):
+                if _ > 4:
+                    self.log.debug('Maximum retries for segment %s reached.', Path(ts_path).stem)
+                    return {1, f'Maximum retries for segment {Path(ts_path).stem} reached.'}
+
+                try:
+                    _r = requests.get(ts_url, stream=True, timeout=10)
+
+                    # break on non 200 status code
+                    if _r.status_code != 200:
+                        self.log.error('Code other than 200 received when trying to download segment.')
+                        continue
+
+                    # write downloaded chunks to temporary file
+                    for chunk in _r.iter_content(chunk_size=262144):
+                        tmp_ts_file.write(chunk)
+
+                    self.log.debug('Segment %s download completed.', Path(ts_path).stem)
+
+                    break
+
+                except requests.exceptions.RequestException as e:
+                    self.log.debug('Segment %s download failed (Attempt %s). Error: %s)',
+                                   Path(ts_path).stem, _ + 1, str(e))
+                    continue
+
+        try:
+            # move part to destination storage
+            safe_move(tmp_ts_file.name, ts_path)
+            self.log.debug('Segment %s completed.', Path(ts_path).stem)
+
+        except FileNotFoundError as e:
+            raise VodPartDownloadError(f'MPEG-TS segment did not download correctly. Piece: {ts_url}') from e
+
+        except BaseException as e:
+            self.log.error('Exception encountered while moving downloaded MPEG-TS segment %s.', ts_url, exc_info=True)
+            return e
+
+        return False
+
+    def get_chat(self, vod_json, offset=0):
+        """Downloads the chat for a specified VOD, returning comments beginning from offset (if provided).
+
+        :param vod_json: dict of vod information
+        :param offset: offset in seconds to begin chat retrieval from - none to begin at start
+        """
+        chat_log = []
+
+        _s = requests.session()
+        _s.headers.update({'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'})
+
+        # grab initial chat segment containing cursor
+        initial_segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], offset=offset)
+        chat_log.extend(initial_segment)
+
+        progress = Progress()
+
+        while True:
+            if not cursor:
+                break
+
+            try:
+                # grab next chat segment along with cursor for next segment
+                segment, cursor = self.get_chat_segment(_s, vod_json['vod_id'], cursor=cursor)
+                chat_log.extend(segment)
+                # vod duration in seconds is used as the total for progress bar
+                # comment offset is used to track what's been done
+                # could be done properly if there was a way to get the total number of comments
+                if not self.quiet:
+                    progress.print_progress(int(segment[-1]['contentOffsetSeconds']),
+                                            vod_json['duration'], not cursor)
+
+            except TwitchAPIErrorNotFound:
+                break
+
+            finally:
+                _s.close()
+
+        self.log.info('Found %s messages.', len(chat_log))
+
+        return chat_log
+
+    def get_chat_segment(self, session, vod_id, offset=None, cursor=None):
+        """Retrieves a single chat segment.
+
+        :param session: requests session to link request to
+        :param vod_id: id of vod to retrieve segment from
+        :param offset: offset in seconds to begin retrieval from
+        :param cursor: cursor returned by a previous call of this function
+        :return: list of comments and cursor if one is returned from twitch
+        """
+        # build payload
+        if offset is not None:
+            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
+                   "variables": {"videoID": vod_id, "contentOffsetSeconds": offset}}]
+
+        else:
+            _p = [{"operationName": "VideoCommentsByOffsetOrCursor",
+                   "variables": {"videoID": vod_id, "cursor": cursor}}]
+
+        _p[0]['extensions'] =\
+            {'persistedQuery': {'version': 1,
+                                'sha256Hash': "b70a3591ff0f4e0313d126c6a1502d79a1c02baebb288227c582044aa76adf6a"}}
+
+        for attempt in range(6):
+            if attempt > 4:
+                self.log.error('Maximum attempts reached while downloading chat segment at cursor or offset: %s, %s.',
+                               cursor, offset)
+                raise ChatDownloadError
+
+            try:
+                _r = Api.post_request_with_session('https://gql.twitch.tv/gql', session, _p).json()
+
+            except RequestError:
+                continue
+
+            break
+
+        comments = _r[0]['data']['video']['comments']
+
+        # check if next page exists
+        if comments['pageInfo']['hasNextPage']:
+            return [c['node'] for c in comments['edges']], comments['edges'][-1]['cursor']
+
+        return [c['node'] for c in comments['edges']], None
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/processing.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,794 +1,779 @@
-"""
-Primary processing loops for calling the various download functions using the supplied user variables.
-"""
-
-import json
-import logging
-import multiprocessing
-import os
-import re
-import shutil
-import sys
-import tempfile
-
-from datetime import datetime, timezone
-from glob import glob
-from math import floor
-from pathlib import Path
-from time import sleep
-
-import m3u8
-
-from twitcharchiver.api import Api
-from twitcharchiver.database import Database, CREATE_VOD, UPDATE_VOD, __db_version__
-from twitcharchiver.downloader import Downloader
-from twitcharchiver.exceptions import VodDownloadError, ChatDownloadError, ChatExportError, VodMergeError, \
-    UnlockingError, TwitchAPIErrorNotFound, TwitchAPIErrorForbidden, RequestError, CorruptPartError
-from twitcharchiver.stream import Stream
-from twitcharchiver.twitch import Twitch
-from twitcharchiver.utils import create_lock, remove_lock, sanitize_date, sanitize_text, combine_vod_parts, \
-    convert_vod, cleanup_vod_parts, send_push, convert_to_seconds, import_json, format_vod_chapters, \
-    verify_vod_length, generate_readable_chat_log, export_readable_chat_log, time_since_date, export_json, \
-    export_verbose_chat_log, get_hash, safe_move
-
-
-class Processing:
-    """
-    Primary processing loops for downloading content.
-    """
-    def __init__(self, config, args):
-
-        self.log = logging.getLogger()
-
-        self.directory = args['directory']
-        self.vod_directory = Path(self.directory)
-        self.video = args['video']
-        self.chat = args['chat']
-        self.quality = args['quality']
-        self.live_only = args['live_only']
-        self.archive_only = args['archive_only']
-        self.config_dir = args['config_dir']
-        self.quiet = args['quiet']
-        self.debug = args['debug']
-
-        self.client_id = config['client_id']
-        self.client_secret = config['client_secret']
-        self.oauth_token = config['oauth_token']
-
-        self.pushbullet_key = config['pushbullet_key']
-
-        self.call_twitch = Twitch(self.client_id, self.client_secret, self.oauth_token)
-        self.download = Downloader(self.client_id, self.oauth_token, args['threads'], args['quiet'])
-
-    def get_channel(self, channels):
-        """
-        Download all vods from a specified channel or list of channels.
-        """
-        for channel in channels:
-            self.log.info("Now archiving channel '%s'.", channel)
-            self.log.debug('Fetching user data from Twitch.')
-
-            user_data = self.call_twitch.get_api(f'users?login={channel}')['data'][0]
-            user_id = user_data['id']
-            user_name = user_data['display_name']
-
-            channel_live = False
-            stream = Stream(self.client_id, self.client_secret, self.oauth_token)
-            tmp_buffer_dir = Path(tempfile.gettempdir(), os.urandom(24).hex())
-
-            self.vod_directory = Path(self.directory, user_name)
-
-            # setup database
-            with Database(Path(self.config_dir, 'vods.db')) as db:
-                # check db version
-                version = db.execute_query('pragma user_version')[0][0]
-
-                if version != __db_version__:
-                    # incremental database updating based on version number
-                    # create the latest db schema if none exists
-                    if version == 0:
-                        self.log.debug('No schema found, creating database.')
-                        db.setup_database()
-
-                    # update version 2 schema to version 3
-                    if version == 2:
-                        self.log.debug('Performing incremental DB update. Version 2 -> Version 3.')
-                        db.update_database(2)
-                        version = 3
-
-                    # update version 3 schema to version 4
-                    if version == 3:
-                        self.log.debug('Performing incremental DB update. Version 3 -> Version 4.')
-                        db.update_database(3)
-
-            # fetch channel info and live status
-            channel_data = self.call_twitch.get_api(f'streams?user_id={user_id}')['data']
-            if channel_data and channel_data[0]['type'] == 'live':
-                channel_live = True
-                # ensure enough time has passed for vod api to update before archiving
-                stream_length = time_since_date(datetime.strptime(
-                    channel_data[0]['started_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
-
-                # TODO: ensure that if the stream ends, we clean up and merge segments
-                # while we wait for the api to update we must build a temporary buffer of any parts advertised in the
-                # meantime in case there is no vod and thus no way to retrieve them after the fact
-                if stream_length < 90:
-                    self.log.debug('Stream began less than 90s ago, delaying archival start until VOD API updated.')
-                    # create temp dir for buffer
-                    Path(tmp_buffer_dir).mkdir(parents=True, exist_ok=True)
-
-                    stream.unsynced_setup(tmp_buffer_dir)
-                    index_uri = self.call_twitch.get_channel_hls_index(channel, self.quality)
-
-                    # download new parts every 4s
-                    for i in range(int((90 - stream_length) / 4)):
-                        # grab required values
-                        start_timestamp = int(datetime.utcnow().timestamp())
-                        incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
-
-                        # create buffer and download segments to temp dir
-                        stream.build_unsynced_buffer(incoming_segments)
-                        stream.download_buffer(tmp_buffer_dir)
-
-                        # wait if less than 5s passed since grabbing more parts
-                        processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
-                        if processing_time < 4:
-                            sleep(4 - processing_time)
-
-                    # wait any remaining time
-                    sleep((90 - stream_length) % 4)
-
-            # retrieve available vods
-            available_vods: dict[int: tuple[int]] = {}
-            cursor = ''
-            try:
-                while True:
-                    _r = self.call_twitch.get_api(f'videos?user_id={user_id}&first=100&type=archive&after={cursor}')
-                    if not _r['pagination']:
-                        break
-
-                    # dict containing stream_id: (vod_id)
-                    available_vods.update(dict([(int(vod['stream_id']), (vod['id'])) for vod in _r['data']]))
-                    cursor = _r['pagination']['cursor']
-
-            except BaseException as e:
-                self.log.error('Error retrieving VODs from Twitch. Error: %s', str(e))
-                continue
-
-            self.log.debug(f'Online VODs: {available_vods}')
-
-            # retrieve downloaded vods
-            with Database(Path(self.config_dir, 'vods.db')) as db:
-                # dict containing stream_id: (vod_id, video_downloaded, chat_downloaded)
-                downloaded_vods = dict([(i[0], (i[1], i[2], i[3])) for i in db.execute_query(
-                    'SELECT stream_id, vod_id, video_archived, chat_archived FROM vods WHERE user_id IS ?',
-                    {'user_id': user_id})])
-            self.log.debug(f'Downloaded vods: {downloaded_vods}')
-
-            # generate vod queue using downloaded and available vods
-            vod_queue = {}
-            for stream_id in available_vods.keys():
-                # add any vods not present in database
-                if stream_id not in downloaded_vods.keys():
-                    vod_queue.update({stream_id: (available_vods[stream_id], self.video, self.chat)})
-
-                # if vod in database but downloaded as stream, go over it again using backup vod downloader
-                # to ensure the vod is properly archived along with the chat which we missed
-                elif downloaded_vods[stream_id][0] is None:
-                    vod_queue.update({stream_id: (available_vods[stream_id], True, self.chat)})
-
-                # if vod in database, check downloaded formats against requested ones, adding vod with missing formats
-                # to queue
-                elif not downloaded_vods[stream_id][1] and self.video or \
-                        not downloaded_vods[stream_id][2] and self.chat:
-                    vod_queue.update({stream_id: (available_vods[stream_id],
-                                                  not downloaded_vods[stream_id][1] and self.video,
-                                                  not downloaded_vods[stream_id][2] and self.chat)})
-
-            # check if stream being archived to vod
-            live_vod_exists = (channel_data and int(channel_data[0]['id']) in available_vods.keys())
-
-            # move on if channel offline and no vods are available
-            if not self.live_only and not channel_live and not available_vods:
-                self.log.info('No VODs were found for %s.', user_name)
-                continue
-
-            # move on if channel offline and we are only looking for live vods
-            if not channel_live and self.live_only:
-                self.log.info('Running in stream-only mode and no stream available for %s.', user_name)
-                continue
-
-            # archive stream in non-segmented mode if no paired vod exists, unless we are in no_stream mode or not
-            # archiving video.
-            if not self.archive_only and channel_live and not live_vod_exists and self.video:
-                self.log.info('Channel live but not being archived to a VOD, running stream archiver.')
-                self.log.debug('Creating lock file for stream.')
-
-                if create_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
-                    self.log.info('Lock file present for stream by %s (.lock.%s-stream-only), skipping.',
-                                  user_name, channel_data[0]["id"])
-
-                else:
-                    # check if stream in database
-                    with Database(Path(self.config_dir, 'vods.db')) as db:
-                        downloaded_streams = [str(i[0]) for i in db.execute_query(
-                            'SELECT stream_id FROM vods WHERE user_id IS ?', {'user_id': user_id})]
-
-                    # Check if stream id in database
-                    if channel_data[0]['id'] in downloaded_streams:
-                        self.log.info('Ignoring steam as it has already been downloaded.')
-
-                    else:
-                        try:
-                            # move parts from temp stream buffer to output dir
-                            # gather parts from temp dir
-                            buffered_parts = [Path(p) for p in sorted(glob(str(Path(tmp_buffer_dir, '*.ts'))))]
-                            # create output dir
-                            output_dir = \
-                                str(Path(self.vod_directory,
-                                         f"{sanitize_date(channel_data[0]['started_at'])} - "
-                                         f"{sanitize_text(channel_data[0]['title'])} - STREAM_ONLY", 'parts'))
-                            Path(output_dir).mkdir(parents=True, exist_ok=True)
-
-                            # move parts individually to destination dir
-                            for part in buffered_parts:
-                                dst_part = str(Path(part).name)
-                                safe_move(part, Path(output_dir, dst_part))
-
-                            stream_json = self.get_unsynced_stream(channel_data[0], stream)
-
-                            if stream_json:
-                                # add to database
-                                self.log.debug('Adding stream info to database.')
-                                with Database(Path(self.config_dir, 'vods.db')) as db:
-                                    db.execute_query(CREATE_VOD, stream_json)
-
-                            else:
-                                self.log.debug('No stream information returned to channel function, stream downloader'
-                                               ' exited with error.')
-
-                        except BaseException as e:
-                            self.log.error('Exception encountered while archiving live-only stream by %s. Error: %s',
-                                           {user_name}, str(e))
-                            return
-
-                        finally:
-                            # remove lock
-                            self.log.debug('Removing lock file.')
-                            if remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
-                                raise UnlockingError(user_name, stream_id=channel_data[0]['id'])
-
-            # wipe stream buffer as stream has paired vod
-            if Path(tmp_buffer_dir).exists():
-                shutil.rmtree(tmp_buffer_dir)
-
-            # exit if vod queue empty
-            if not vod_queue:
-                self.log.info('No new VODs were found for %s.', user_name)
-                continue
-
-            self.log.info('%s VOD(s) in download queue.', len(vod_queue))
-            self.log.debug('VOD queue: %s', vod_queue)
-
-            # begin processing each available vod
-            for stream_id in vod_queue:
-                vod_id = vod_queue[stream_id][0]
-
-                # skip if we are only after currently live streams, and stream_id is not live
-                if channel_data and self.live_only and stream_id != int(channel_data[0]['id']):
-                    continue
-
-                # skip if we aren't after currently lives streams, and stream_id is live
-                if channel_data and self.archive_only and stream_id == int(channel_data[0]['id']):
-                    self.log.info('Skipping VOD as it is live and no-stream argument provided.')
-                    continue
-
-                self.log.debug('Processing VOD %s by %s', vod_id, user_name)
-                self.log.debug('Creating lock file for VOD.')
-
-                if create_lock(self.config_dir, stream_id):
-                    self.log.info('Lock file present for VOD %s (.lock.%s), skipping.', vod_id, stream_id)
-                    continue
-
-                # check if vod in database
-                with Database(Path(self.config_dir, 'vods.db')) as db:
-                    downloaded_vod = db.execute_query(
-                        'SELECT vod_id, video_archived, chat_archived FROM vods WHERE stream_id IS ?',
-                        {'stream_id': stream_id})
-
-                # check if vod_id exists in database in the requested format(s)
-                if downloaded_vod and vod_queue[stream_id][1] and downloaded_vod[0][1] \
-                        and vod_queue[stream_id][2] and downloaded_vod[0][2]:
-                    self.log.info('VOD has been downloaded in requested format since download queue was created.')
-                    continue
-
-                vod_json = self.get_vod_connector(vod_id, vod_queue[stream_id][1], vod_queue[stream_id][2])
-
-                if vod_json:
-                    # insert video, chat archival flags
-                    vod_json['video_archived'] = vod_queue[stream_id][1]
-                    if 'chat_archived' not in vod_json.keys():
-                        vod_json['chat_archived'] = vod_queue[stream_id][2]
-                    # null empty values
-                    for key in vod_json.keys():
-                        if isinstance(vod_json[key], str) and vod_json[key] == "":
-                            vod_json[key] = None
-
-                    try:
-                        # add to database
-                        self.log.debug('Adding VOD info to database.')
-                        with Database(Path(self.config_dir, 'vods.db')) as db:
-                            # check if stream already exists and update if so
-                            db_vod = db.execute_query(
-                                'SELECT stream_id, video_archived, chat_archived FROM vods WHERE stream_id IS ?',
-                                {'stream_id': vod_json['stream_id']})
-                            if db_vod:
-                                # update archived flags using previous and current processing flags
-                                vod_json['video_archived'] = db_vod[0][1] or vod_json['video_archived']
-                                vod_json['chat_archived'] = db_vod[0][2] or vod_json['chat_archived']
-                                vod_json['sid'] = vod_json['stream_id']
-                                db.execute_query(UPDATE_VOD, vod_json)
-
-                            else:
-                                db.execute_query(CREATE_VOD, vod_json)
-
-                    finally:
-                        # remove lock
-                        self.log.debug('Removing lock file.')
-                        if remove_lock(self.config_dir, vod_json['stream_id']):
-                            raise UnlockingError(vod_json['user_name'], vod_json['stream_id'], vod_id)
-
-                else:
-                    self.log.debug('No VOD information returned to channel function, downloader exited with error.')
-                    continue
-
-    def get_unsynced_stream(self, channel_data, stream=None):
-        """Archives a live stream without a paired VOD.
-
-        :param channel_data: json retrieved from channel endpoint
-        :param stream: optionally provided stream method if existing buffer needs to be kept
-        :return: sanitized / formatted stream json
-        """
-        if not stream:
-            stream = Stream(self.client_id, self.client_secret, self.oauth_token)
-
-        try:
-            # generate stream dict
-            stream_json_keys = \
-                ['vod_id', 'stream_id', 'user_id', 'user_login', 'user_name', 'title', 'description', 'created_at',
-                 'published_at', 'url', 'thumbnail_url', 'viewable', 'view_count', 'language', 'type', 'duration',
-                 'muted_segments', 'store_directory', 'video_archived', 'chat_archived']
-            stream_json = {k: None for k in stream_json_keys}
-
-            stream_json.update(
-                {'stream_id': channel_data['id'], 'user_id': channel_data['user_id'],
-                 'user_login': channel_data['user_login'], 'user_name': channel_data['user_name'],
-                 'title': channel_data['title'], 'created_at': channel_data['started_at'],
-                 'published_at': channel_data['started_at'], 'language': channel_data['language'],
-                 'type': channel_data['type'], 'video_archived': 1, 'chat_archived': 0})
-
-            stream_json['store_directory'] = \
-                str(Path(self.vod_directory, f'{sanitize_date(stream_json["created_at"])} - '
-                                             f'{sanitize_text(stream_json["title"])} - STREAM_ONLY'))
-
-            stream.get_stream(
-                stream_json['user_name'], Path(stream_json['store_directory'], 'parts'), self.quality, False)
-
-            # insert duration into json using stream created datetime
-            created_at = int((datetime.strptime(stream_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').timestamp()))
-            stream_json['duration'] = int(datetime.utcnow().timestamp() - created_at)
-
-            # merge stream segments and convert to mp4
-            try:
-                combine_vod_parts(stream_json, print_progress=not self.quiet)
-                convert_vod(stream_json, [(0, 99999)], print_progress=not self.quiet)
-
-            except Exception as e:
-                raise VodMergeError(e) from e
-
-            self.log.debug('Cleaning up temporary files...')
-            cleanup_vod_parts(stream_json['store_directory'])
-
-            return stream_json
-
-        except KeyboardInterrupt:
-            self.log.debug('User requested stop, halting stream downloader.')
-            if Path(self.config_dir, f'.lock.{channel_data["user_name"]}').exists():
-                remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only')
-
-            sys.exit(0)
-
-        except (RequestError, VodMergeError) as e:
-            self.log.debug('Exception downloading or merging stream.\n{e}', exc_info=True)
-            send_push(self.pushbullet_key, 'Exception encountered while downloading or merging downloaded stream '
-                                           f'by {channel_data["user_name"]}', str(e))
-
-        except BaseException as e:
-            self.log.error('Unexpected exception encountered while downloading live-only stream.\n%s', str(e),
-                           exc_info=True)
-            send_push(self.pushbullet_key, 'Unexpected exception encountered while downloading live-only stream '
-                                           f'by {channel_data["user_name"]}', str(e))
-
-        return False
-
-    def get_vod_connector(self, vod_id, get_video, get_chat):
-        """Download a single vod or list of vod IDs.
-
-        :param vod_id: vod id to download
-        :param get_video: bool whether to grab video
-        :param get_chat: bool whether to grab chat logs
-        :return: dict containing current vod information returned by get_vod
-        """
-        self.log.info('Now processing VOD: %s', vod_id)
-        vod_json = self.call_twitch.get_api(f'videos?id={vod_id}')['data'][0]
-        vod_json['vod_id'] = vod_json.pop('id')
-        vod_json['muted_segments'] = str(vod_json['muted_segments'])
-        vod_json['store_directory'] = \
-            str(Path(self.vod_directory, f'{sanitize_date(vod_json["created_at"])} - '
-                                         f'{sanitize_text(vod_json["title"])} - {vod_id}'))
-        vod_json['duration'] = convert_to_seconds(vod_json['duration'])
-
-        # get vod status
-        vod_live = self.call_twitch.get_vod_status(vod_json['user_id'], vod_json['created_at'])
-
-        self.log.info("VOD %s", 'currently or recently live. Running in LIVE mode.' if vod_live else 'offline.')
-
-        _r = None
-
-        try:
-            # begin real-time archiver if VOD still live and real-time archiver enabled
-            if self.real_time_archiver and vod_live:
-                stream = Stream(self.client_id, self.client_secret, self.oauth_token)
-                # concurrently grab live pieces and vod chunks
-
-                workers = []
-
-                # the stream module itself has no checks for what to download so this is done here
-                if get_video:
-                    workers.append(multiprocessing.Process(target=stream.get_stream, args=(
-                        vod_json['user_name'], Path(vod_json['store_directory'], 'parts'), self.quality)))
-
-                workers.append(multiprocessing.Process(target=self.get_vod, args=(
-                    vod_json, get_video, get_chat, vod_live)))
-
-                for worker in workers:
-                    worker.start()
-
-                for worker in workers:
-                    worker.join()
-
-            else:
-                self.get_vod(vod_json, get_video, get_chat, vod_live)
-
-            # return imported json rather than returning from get_vod process as there were issues with returning
-            # values via multiprocessing
-            vod_json = import_json(vod_json)
-
-            # combine vod segments
-            if get_video:
-                # combine all the 10s long .ts parts into a single file, then convert to .mp4
-                try:
-                    # retrieve vod chapters
-                    try:
-                        vod_chapters = Twitch.get_vod_chapters(vod_id)
-                        if vod_chapters:
-                            # write chapters to file
-                            with open(Path(vod_json['store_directory'], 'chapters.json'), 'w',
-                                      encoding='utf8') as chapters_file:
-                                chapters_file.write(json.dumps(vod_chapters))
-
-                        else:
-                            # get category if no separate chapters found
-                            vod_chapters = (Twitch.get_vod_category(vod_id), 0, vod_json['duration'] * 1000)
-
-                        # format and write vod chapters to parts dir
-                        with open(Path(vod_json['store_directory'], 'parts', 'chapters.txt'),
-                                  'w', encoding='utf8') as chapters_file:
-                            chapters_file.write(format_vod_chapters(vod_chapters))
-
-                    except BaseException as e:
-                        self.log.error('Failed to retrieve or insert chapters into VOD file. %s', str(e))
-
-                    try:
-                        combine_vod_parts(vod_json, print_progress=not self.quiet)
-                        # load muted segments if any exists
-                        with open(Path(vod_json['store_directory'], 'parts', '.muted'), 'r',
-                                  encoding='utf8') as mutefile:
-                            muted_segments = json.load(mutefile)
-                        convert_vod(vod_json, muted_segments, print_progress=not self.quiet)
-
-                    except CorruptPartError as c:
-                        self.log.error("Corrupt segments found while converting VOD. Attempting to retry parts:"
-                                       "\n%s", ', '.join([str(p) for p in c.parts]))
-
-                        # check vod still available
-                        if not self.call_twitch.get_vod_index(vod_json, self.quality):
-                            raise VodDownloadError("Corrupt segments were found while converting VOD and TA was "
-                                                   "unable to re-download the missing segments. Either re-download "
-                                                   "the VOD if it is still available, or manually convert 'merged.ts' "
-                                                   f"using FFmpeg. Corrupt parts:\n{', '.join(c.f_parts)}")
-
-                        # rename corrupt segments
-                        for part in c.parts:
-                            # convert part number to segment file
-                            part = str(f'{int(part):05d}' + '.ts')
-
-                            # rename part
-                            shutil.move(Path(vod_json['store_directory'], 'parts', part),
-                                        Path(vod_json['store_directory'], 'parts', part + '.corrupt'))
-
-                        # download and combine vod again
-                        try:
-                            self.get_vod(vod_json, True, False, False)
-
-                            # compare downloaded .ts to corrupt parts - corrupt parts SHOULD have different hashes
-                            # so we can work out if a segment is corrupt on twitch's end or ours
-                            for part_num in c.parts:
-                                part = str('{:05d}'.format(int(part_num)) + '.ts')
-
-                                # compare hashes
-                                if get_hash(Path(vod_json['store_directory'], 'parts', part)) == \
-                                        get_hash(Path(vod_json['store_directory'], 'parts', part + '.corrupt')):
-                                    self.log.debug(f"Re-downloaded .ts segment {part_num} matches corrupt one, "
-                                                   "assuming corruption is on Twitch's end and ignoring.")
-                                    muted_segments.append([part_num, part_num])
-
-                            combine_vod_parts(vod_json, print_progress=not self.quiet)
-                            convert_vod(vod_json, muted_segments, print_progress=not self.quiet)
-
-                        except CorruptPartError as e:
-                            raise VodDownloadError(
-                                "Corrupt part(s) still present after retrying VOD download. Ensure VOD is still "
-                                "available and either delete the listed #####.ts part(s) from 'parts' folder or entire "
-                                f"'parts' folder if issue persists.\n{', '.join(c.f_parts)}") from e
-
-                except BaseException as e:
-                    raise VodMergeError(e) from e
-
-                # verify vod length is equal to what is grabbed from twitch
-                if verify_vod_length(vod_json):
-                    raise VodMergeError('VOD length outside of acceptable range. If error persists delete '
-                                        "'vod/parts' directory if VOD still available.")
-
-            if get_chat:
-                try:
-                    with open(Path(vod_json['store_directory'], 'verbose_chat.json'), 'r',
-                              encoding='utf8') as chat_file:
-                        chat_log = json.loads(chat_file.read())
-
-                    # generate and export the readable chat log
-                    if chat_log:
-                        try:
-                            self.log.debug('Generating readable chat log and saving to disk...')
-                            r_chat_log = generate_readable_chat_log(chat_log, datetime.strptime(
-                                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc))
-                            export_readable_chat_log(r_chat_log, vod_json['store_directory'])
-
-                        except BaseException as e:
-                            raise ChatExportError(e) from e
-
-                    else:
-                        self.log.info('No chat messages found.')
-
-                # catch missing chat log and modify database insert
-                except FileNotFoundError:
-                    self.log.error('No chat log found, download likely failed or log unavailable.')
-                    vod_json['chat_archived'] = False
-
-            if get_video:
-                # grab thumbnail at 1080p resolution - any resolution can be used but this should be fine for almost
-                # every stream
-                try:
-                    self.log.debug('Downloading VOD thumbnail.')
-                    thumbnail = Api.get_request(vod_json['thumbnail_url'].replace('%{width}x%{height}', '1920x1080'))
-                    with open(Path(vod_json['store_directory'], 'thumbnail.jpg'), 'wb') as thumbnail_file:
-                        thumbnail_file.write(thumbnail.content)
-
-                except BaseException as e:
-                    self.log.error('Failed to grab thumbnail for VOD. Error: %s', str(e))
-
-                # delete temporary .ts parts and merged.ts file
-                self.log.debug('Cleaning up temporary files...')
-                cleanup_vod_parts(vod_json['store_directory'])
-
-        # catch user exiting and remove lock file
-        except KeyboardInterrupt:
-            if vod_live:
-                self.log.debug('User requested stop, terminating download workers...')
-                for worker in workers:
-                    worker.terminate()
-                    worker.join()
-
-            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
-                remove_lock(self.config_dir, vod_json['stream_id'])
-
-            sys.exit(0)
-
-        # catch halting errors, send notification and remove lock file
-        except (RequestError, VodDownloadError, ChatDownloadError, VodMergeError, ChatExportError) as e:
-            if vod_live:
-                self.log.debug('Exception encountered, terminating download workers...')
-                for worker in workers:
-                    worker.terminate()
-                    worker.join()
-
-            self.log.error('Error downloading VOD %s.', vod_id, exc_info=True)
-            send_push(self.pushbullet_key, f'Error downloading VOD {vod_id} by {vod_json["user_name"]}', str(e))
-            # remove lock file if archiving channel
-            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
-                remove_lock(self.config_dir, vod_json['stream_id'])
-
-            # set to None so that channel function knows download failed
-            vod_json = None
-
-        # catch unhandled exceptions
-        except BaseException as e:
-            if vod_live:
-                self.log.debug('Exception encountered, terminating download workers...')
-                for worker in workers:
-                    worker.terminate()
-                    worker.join()
-
-            send_push(self.pushbullet_key, f'Exception encountered while downloading VOD {vod_id} by '
-                                           f'{vod_json["user_name"]}', str(e))
-            self.log.error('Exception encountered while downloading VOD %s.', vod_id, exc_info=True)
-            return
-
-        # this is only used when archiving a channel
-        return vod_json
-
-    def get_vod(self, vod_json, get_video=True, get_chat=True, vod_live=False):
-        """Retrieves a specified VOD.
-
-        :param vod_json: dict of vod parameters retrieved from twitch
-        :param get_video: boolean whether to grab video
-        :param get_chat: boolean whether to grab chat logs
-        :param vod_live: boolean true if vod currently live, false otherwise
-        :return: dict containing current vod information
-        """
-        # create vod dir
-        Path(vod_json['store_directory']).mkdir(parents=True, exist_ok=True)
-
-        # wait if vod recently created
-        if time_since_date(datetime.strptime(
-                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp()) < 300:
-            self.log.info('Waiting 5m to download initial VOD parts as it was created very recently. Live archiving '
-                          'will still function.')
-            sleep(300)
-
-        if time_since_date(datetime.strptime(
-                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp()) \
-                < (vod_json['duration'] + 360):
-            self.log.debug('Time since VOD was created + its duration is a point in time < 10 minutes ago. '
-                           'Running in live mode in case not all parts are available yet.')
-            vod_live = True
-
-        # import chat log if it has been partially downloaded
-        try:
-            with open(Path(vod_json['store_directory'], 'verbose_chat.json'), 'r', encoding='utf8') as chat_file:
-                chat_log = json.loads(chat_file.read())
-
-            # ignore chat logs created with older incompatible schema - see v2.2.1 changes
-            if chat_log and 'contentOffsetSeconds' not in chat_log[0].keys():
-                chat_log = []
-
-        except FileNotFoundError:
-            chat_log = []
-
-        # fetch all streams for a particular vod
-        if get_video:
-            try:
-                vod_index = self.call_twitch.get_vod_index(vod_json, self.quality)
-
-                # attempt to fetch playlist for requested stream
-                Api.get_request(vod_index).text
-
-            except TwitchAPIErrorForbidden as e:
-                raise VodDownloadError('Error retrieving VOD index. VOD may have been deleted or supplied resolution '
-                                       f'was invalid. Error: {str(e)}') from e
-
-        # loop for processing live vods
-        while True:
-            try:
-                _r = self.call_twitch.get_api(f'videos?id={vod_json["vod_id"]}')
-
-                vod_json = _r['data'][0]
-                vod_json['vod_id'] = vod_json.pop('id')
-                vod_json['muted_segments'] = str(vod_json['muted_segments']) if vod_json['muted_segments'] else None
-                vod_json['store_directory'] = \
-                    str(Path(self.vod_directory, f'{sanitize_date(vod_json["created_at"])} - '
-                                                 f'{sanitize_text(vod_json["title"])} - {vod_json["vod_id"]}'))
-                vod_json['duration'] = convert_to_seconds(vod_json['duration'])
-
-                export_json(vod_json)
-
-            except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
-                self.log.warning('Error retrieving VOD json - VOD was likely deleted.')
-                with open(Path(vod_json['store_directory'], '.ignorelength'), 'w', encoding='utf8') as _:
-                    pass
-
-                vod_live = False
-
-            if get_video:
-                # download all available vod parts
-                self.log.info('Grabbing video...')
-                try:
-                    vod_playlist = Api.get_request(vod_index).text
-
-                    # update vod json with m3u8 duration - more accurate than twitch API
-                    _m = re.findall(r'(?<=#EXT-X-TWITCH-TOTAL-SECS:).*(?=\n)', vod_playlist)[0]
-                    vod_json['duration'] = floor(float(_m))
-                    export_json(vod_json)
-
-                    # replace extra chars in base_url like /chunked/index[-muted-JU07DEVBNK.m3u8]
-                    _m = re.findall(r'(?<=\/)(index.*)', vod_index)[0]
-                    vod_base_url = vod_index.replace(_m, '')
-
-                    self.download.get_m3u8_video(m3u8.loads(vod_playlist), vod_base_url, vod_json['store_directory'])
-
-                except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
-                    self.log.debug('Error 403 or 404 returned when downloading VOD parts - VOD was likely deleted.')
-                    with open(Path(vod_json['store_directory'], '.ignorelength'), 'w') as _:
-                        pass
-
-                    vod_live = False
-
-                except BaseException as e:
-                    raise VodDownloadError(e) from e
-
-            if get_chat:
-                # download all available chat segments
-                self.log.info('Grabbing chat logs...')
-                try:
-                    if not chat_log:
-                        chat_log = self.download.get_chat(vod_json)
-
-                    # only try to grab more chat logs if we aren't past vod length
-                    elif int(chat_log[-1]['contentOffsetSeconds']) < vod_json['duration']:
-                        self.log.debug(f'Grabbing chat logs from offset: {chat_log[-1]["contentOffsetSeconds"]}')
-                        chat_log.extend(
-                            [n for n in
-                             self.download.get_chat(vod_json, floor(int(chat_log[-1]['contentOffsetSeconds'])))
-                             if n['id'] not in [m['id'] for m in chat_log]])
-
-                    export_verbose_chat_log(chat_log, vod_json['store_directory'])
-
-                except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
-                    self.log.debug('Error 403 or 404 returned when downloading chat log - VOD was likely deleted.')
-                    with open(Path(vod_json['store_directory'], '.ignorelength'), 'w', encoding='utf8') as _:
-                        pass
-
-                    vod_live = False
-
-                except Exception as e:
-                    raise ChatDownloadError(e) from e
-
-            if vod_live:
-                # wait up to 10 minutes, checking every minute to verify if vod is still being updated or not
-                for _ in range(11):
-                    self.log.debug('Waiting 60s to see if VOD changes.')
-                    sleep(60)
-                    try:
-                        # restart while loop if new video segments found
-                        if len(m3u8.loads(vod_playlist).segments) \
-                                < len(m3u8.loads(Api.get_request(vod_index).text).segments):
-                            self.log.debug('New VOD parts found.')
-                            vod_live = True
-                            break
-
-                        # exit loop if 10 minutes pass without new vod segments being added
-                        if _ > 9:
-                            self.log.debug('10m has passed since VOD duration changed - assuming it is no longer live.')
-                            vod_live = False
-
-                        else:
-                            continue
-
-                    except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
-                        self.log.debug('Error 403 or 404 returned when checking for new VOD parts - VOD was likely'
-                                       ' deleted.')
-                        vod_live = False
-                        break
-
-            else:
-                break
+"""
+Primary processing loops for calling the various download functions using the supplied user variables.
+"""
+
+import json
+import logging
+import multiprocessing
+import os
+import re
+import shutil
+import sys
+import tempfile
+
+from datetime import datetime, timezone
+from glob import glob
+from math import floor
+from pathlib import Path
+from time import sleep
+
+import m3u8
+
+from twitcharchiver.api import Api
+from twitcharchiver.database import Database, CREATE_VOD, UPDATE_VOD, __db_version__
+from twitcharchiver.downloader import Downloader
+from twitcharchiver.exceptions import VodDownloadError, ChatDownloadError, ChatExportError, VodMergeError, \
+    UnlockingError, TwitchAPIErrorNotFound, TwitchAPIErrorForbidden, RequestError, CorruptPartError
+from twitcharchiver.stream import Stream
+from twitcharchiver.twitch import Twitch
+from twitcharchiver.utils import create_lock, remove_lock, sanitize_date, sanitize_text, combine_vod_parts, \
+    convert_vod, cleanup_vod_parts, send_push, convert_to_seconds, import_json, format_vod_chapters, \
+    verify_vod_length, generate_readable_chat_log, export_readable_chat_log, time_since_date, export_json, \
+    export_verbose_chat_log, get_hash, safe_move
+
+
+class Processing:
+    """
+    Primary processing loops for downloading content.
+    """
+    def __init__(self, config, args):
+
+        self.log = logging.getLogger()
+
+        self.directory = args['directory']
+        self.vod_directory = Path(self.directory)
+        self.video = args['video']
+        self.chat = args['chat']
+        self.quality = args['quality']
+        self.live_only = args['live_only']
+        self.archive_only = args['archive_only']
+        self.config_dir = args['config_dir']
+        self.quiet = args['quiet']
+        self.debug = args['debug']
+
+        self.client_id = config['client_id']
+        self.client_secret = config['client_secret']
+        self.oauth_token = config['oauth_token']
+
+        self.pushbullet_key = config['pushbullet_key']
+
+        self.call_twitch = Twitch(self.client_id, self.client_secret, self.oauth_token)
+        self.download = Downloader(self.client_id, self.oauth_token, args['threads'], args['quiet'])
+
+    def get_channel(self, channels):
+        """
+        Download all vods from a specified channel or list of channels.
+        """
+        for channel in channels:
+            self.log.info("Now archiving channel '%s'.", channel)
+            self.log.debug('Fetching user data from Twitch.')
+
+            user_data = self.call_twitch.get_api(f'users?login={channel}')['data'][0]
+            user_id = user_data['id']
+            user_name = user_data['display_name']
+
+            channel_live = False
+            stream = Stream(self.client_id, self.client_secret, self.oauth_token)
+            tmp_buffer_dir = Path(tempfile.gettempdir(), os.urandom(24).hex())
+
+            self.vod_directory = Path(self.directory, user_name)
+
+            # setup database
+            with Database(Path(self.config_dir, 'vods.db')) as db:
+                # check db version
+                version = db.execute_query('pragma user_version')[0][0]
+
+                if version != __db_version__:
+                    # incremental database updating based on version number
+                    # create the latest db schema if none exists
+                    if version == 0:
+                        self.log.debug('No schema found, creating database.')
+                        db.setup_database()
+
+                    # update version 2 schema to version 3
+                    if version == 2:
+                        self.log.debug('Performing incremental DB update. Version 2 -> Version 3.')
+                        db.update_database(2)
+                        version = 3
+
+                    # update version 3 schema to version 4
+                    if version == 3:
+                        self.log.debug('Performing incremental DB update. Version 3 -> Version 4.')
+                        db.update_database(3)
+
+            # fetch channel info and live status
+            channel_data = self.call_twitch.get_api(f'streams?user_id={user_id}')['data']
+            if channel_data and channel_data[0]['type'] == 'live':
+                channel_live = True
+                # ensure enough time has passed for vod api to update before archiving
+                stream_length = time_since_date(datetime.strptime(
+                    channel_data[0]['started_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
+
+                # while we wait for the api to update we must build a temporary buffer of any parts advertised in the
+                # meantime in case there is no vod and thus no way to retrieve them after the fact
+                if stream_length < 90:
+                    self.log.debug('Stream began less than 90s ago, delaying archival start until VOD API updated.')
+                    # create temp dir for buffer
+                    Path(tmp_buffer_dir).mkdir(parents=True, exist_ok=True)
+
+                    stream.unsynced_setup(tmp_buffer_dir)
+                    index_uri = self.call_twitch.get_channel_hls_index(channel, self.quality)
+
+                    # download new parts every 4s
+                    for i in range(int((90 - stream_length) / 4)):
+                        # grab required values
+                        start_timestamp = int(datetime.utcnow().timestamp())
+                        incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
+
+                        # create buffer and download segments to temp dir
+                        stream.build_unsynced_buffer(incoming_segments)
+                        stream.download_buffer(tmp_buffer_dir)
+
+                        # wait if less than 5s passed since grabbing more parts
+                        processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
+                        if processing_time < 4:
+                            sleep(4 - processing_time)
+
+                    # wait any remaining time
+                    sleep((90 - stream_length) % 4)
+
+            # retrieve available vods
+            available_vods = Twitch.get_channel_videos(channel)
+
+            self.log.debug(f'Online VODs: {available_vods}')
+
+            # retrieve downloaded vods
+            with Database(Path(self.config_dir, 'vods.db')) as db:
+                # dict containing stream_id: (vod_id, video_downloaded, chat_downloaded)
+                downloaded_vods = dict([(i[0], (i[1], i[2], i[3])) for i in db.execute_query(
+                    'SELECT stream_id, vod_id, video_archived, chat_archived FROM vods WHERE user_id IS ?',
+                    {'user_id': user_id})])
+            self.log.debug(f'Downloaded vods: {downloaded_vods}')
+
+            # generate vod queue using downloaded and available vods
+            vod_queue = {}
+            for stream_id in available_vods.keys():
+                # add any vods not present in database
+                if stream_id not in downloaded_vods.keys():
+                    vod_queue.update({stream_id: (available_vods[stream_id], self.video, self.chat)})
+
+                # if vod in database but downloaded as stream, go over it again using backup vod downloader
+                # to ensure the vod is properly archived along with the chat which we missed
+                elif downloaded_vods[stream_id][0] is None:
+                    vod_queue.update({stream_id: (available_vods[stream_id], True, self.chat)})
+
+                # if vod in database, check downloaded formats against requested ones, adding vod with missing formats
+                # to queue
+                elif not downloaded_vods[stream_id][1] and self.video or \
+                        not downloaded_vods[stream_id][2] and self.chat:
+                    vod_queue.update({stream_id: (available_vods[stream_id],
+                                                  not downloaded_vods[stream_id][1] and self.video,
+                                                  not downloaded_vods[stream_id][2] and self.chat)})
+
+            # check if stream being archived to vod
+            live_vod_exists = (channel_data and int(channel_data[0]['id']) in available_vods.keys())
+
+            # move on if channel offline and no vods are available
+            if not self.live_only and not channel_live and not available_vods:
+                self.log.info('No VODs were found for %s.', user_name)
+                continue
+
+            # move on if channel offline and we are only looking for live vods
+            if not channel_live and self.live_only:
+                self.log.info('Running in stream-only mode and no stream available for %s.', user_name)
+                continue
+
+            # archive stream in non-segmented mode if no paired vod exists, unless we are in no_stream mode or not
+            # archiving video.
+            if not self.archive_only and channel_live and not live_vod_exists and self.video:
+                self.log.info('Channel live but not being archived to a VOD, running stream archiver.')
+                self.log.debug('Creating lock file for stream.')
+
+                if create_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
+                    self.log.info('Lock file present for stream by %s (.lock.%s-stream-only), skipping.',
+                                  user_name, channel_data[0]["id"])
+
+                else:
+                    # check if stream in database
+                    with Database(Path(self.config_dir, 'vods.db')) as db:
+                        downloaded_streams = [str(i[0]) for i in db.execute_query(
+                            'SELECT stream_id FROM vods WHERE user_id IS ?', {'user_id': user_id})]
+
+                    # Check if stream id in database
+                    if channel_data[0]['id'] in downloaded_streams:
+                        self.log.info('Ignoring steam as it has already been downloaded.')
+
+                    else:
+                        try:
+                            # move parts from temp stream buffer to output dir
+                            # gather parts from temp dir
+                            buffered_parts = [Path(p) for p in sorted(glob(str(Path(tmp_buffer_dir, '*.ts'))))]
+                            # create output dir
+                            output_dir = \
+                                str(Path(self.vod_directory,
+                                         f"{sanitize_date(channel_data[0]['started_at'])} - "
+                                         f"{sanitize_text(channel_data[0]['title'])} - STREAM_ONLY", 'parts'))
+                            Path(output_dir).mkdir(parents=True, exist_ok=True)
+
+                            # move parts individually to destination dir
+                            for part in buffered_parts:
+                                dst_part = str(Path(part).name)
+                                safe_move(part, Path(output_dir, dst_part))
+
+                            stream_json = self.get_unsynced_stream(channel_data[0], stream)
+
+                            if stream_json:
+                                # add to database
+                                self.log.debug('Adding stream info to database.')
+                                with Database(Path(self.config_dir, 'vods.db')) as db:
+                                    db.execute_query(CREATE_VOD, stream_json)
+
+                            else:
+                                self.log.debug('No stream information returned to channel function, stream downloader'
+                                               ' exited with error.')
+
+                        except BaseException as e:
+                            self.log.error('Exception encountered while archiving live-only stream by %s. Error: %s',
+                                           {user_name}, str(e))
+                            return
+
+                        finally:
+                            # remove lock
+                            self.log.debug('Removing lock file.')
+                            if remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only'):
+                                raise UnlockingError(user_name, stream_id=channel_data[0]['id'])
+
+            # wipe stream buffer as stream has paired vod
+            if Path(tmp_buffer_dir).exists():
+                shutil.rmtree(tmp_buffer_dir)
+
+            # exit if vod queue empty
+            if not vod_queue:
+                self.log.info('No new VODs were found for %s.', user_name)
+                continue
+
+            self.log.info('%s VOD(s) in download queue.', len(vod_queue))
+            self.log.debug('VOD queue: %s', vod_queue)
+
+            # begin processing each available vod
+            for stream_id in vod_queue:
+                vod_id = vod_queue[stream_id][0]
+
+                # skip if we are only after currently live streams, and stream_id is not live
+                if channel_data and self.live_only and stream_id != int(channel_data[0]['id']):
+                    continue
+
+                # skip if we aren't after currently lives streams, and stream_id is live
+                if channel_data and self.archive_only and stream_id == int(channel_data[0]['id']):
+                    self.log.info('Skipping VOD as it is live and no-stream argument provided.')
+                    continue
+
+                self.log.debug('Processing VOD %s by %s', vod_id, user_name)
+                self.log.debug('Creating lock file for VOD.')
+
+                if create_lock(self.config_dir, stream_id):
+                    self.log.info('Lock file present for VOD %s (.lock.%s), skipping.', vod_id, stream_id)
+                    continue
+
+                # check if vod in database
+                with Database(Path(self.config_dir, 'vods.db')) as db:
+                    downloaded_vod = db.execute_query(
+                        'SELECT vod_id, video_archived, chat_archived FROM vods WHERE stream_id IS ?',
+                        {'stream_id': stream_id})
+
+                # check if vod_id exists in database in the requested format(s)
+                if downloaded_vod and vod_queue[stream_id][1] and downloaded_vod[0][1] \
+                        and vod_queue[stream_id][2] and downloaded_vod[0][2]:
+                    self.log.info('VOD has been downloaded in requested format since download queue was created.')
+                    continue
+
+                vod_json = self.get_vod_connector(vod_id, vod_queue[stream_id][1], vod_queue[stream_id][2])
+
+                if vod_json:
+                    # insert video, chat archival flags
+                    vod_json['video_archived'] = vod_queue[stream_id][1]
+                    if 'chat_archived' not in vod_json.keys():
+                        vod_json['chat_archived'] = vod_queue[stream_id][2]
+                    # null empty values
+                    for key in vod_json.keys():
+                        if isinstance(vod_json[key], str) and vod_json[key] == "":
+                            vod_json[key] = None
+
+                    try:
+                        # add to database
+                        self.log.debug('Adding VOD info to database.')
+                        with Database(Path(self.config_dir, 'vods.db')) as db:
+                            # check if stream already exists and update if so
+                            db_vod = db.execute_query(
+                                'SELECT stream_id, video_archived, chat_archived FROM vods WHERE stream_id IS ?',
+                                {'stream_id': vod_json['stream_id']})
+                            if db_vod:
+                                # update archived flags using previous and current processing flags
+                                vod_json['video_archived'] = db_vod[0][1] or vod_json['video_archived']
+                                vod_json['chat_archived'] = db_vod[0][2] or vod_json['chat_archived']
+                                vod_json['sid'] = vod_json['stream_id']
+                                db.execute_query(UPDATE_VOD, vod_json)
+
+                            else:
+                                db.execute_query(CREATE_VOD, vod_json)
+
+                    finally:
+                        # remove lock
+                        self.log.debug('Removing lock file.')
+                        if remove_lock(self.config_dir, vod_json['stream_id']):
+                            raise UnlockingError(vod_json['user_name'], vod_json['stream_id'], vod_id)
+
+                else:
+                    self.log.debug('No VOD information returned to channel function, downloader exited with error.')
+                    continue
+
+    def get_unsynced_stream(self, channel_data, stream=None):
+        """Archives a live stream without a paired VOD.
+
+        :param channel_data: json retrieved from channel endpoint
+        :param stream: optionally provided stream method if existing buffer needs to be kept
+        :return: sanitized / formatted stream json
+        """
+        if not stream:
+            stream = Stream(self.client_id, self.client_secret, self.oauth_token)
+
+        try:
+            # generate stream dict
+            stream_json_keys = \
+                ['vod_id', 'stream_id', 'user_id', 'user_login', 'user_name', 'title', 'description', 'created_at',
+                 'published_at', 'url', 'thumbnail_url', 'viewable', 'view_count', 'language', 'type', 'duration',
+                 'muted_segments', 'store_directory', 'video_archived', 'chat_archived']
+            stream_json = {k: None for k in stream_json_keys}
+
+            stream_json.update(
+                {'stream_id': channel_data['id'], 'user_id': channel_data['user_id'],
+                 'user_login': channel_data['user_login'], 'user_name': channel_data['user_name'],
+                 'title': channel_data['title'], 'created_at': channel_data['started_at'],
+                 'published_at': channel_data['started_at'], 'language': channel_data['language'],
+                 'type': channel_data['type'], 'video_archived': 1, 'chat_archived': 0})
+
+            stream_json['store_directory'] = \
+                str(Path(self.vod_directory, f'{sanitize_date(stream_json["created_at"])} - '
+                                             f'{sanitize_text(stream_json["title"])} - STREAM_ONLY'))
+
+            stream.get_stream(
+                stream_json['user_name'], Path(stream_json['store_directory'], 'parts'), self.quality, False)
+
+            # insert duration into json using stream created datetime
+            created_at = int((datetime.strptime(stream_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').timestamp()))
+            stream_json['duration'] = int(datetime.utcnow().timestamp() - created_at)
+
+            # merge stream segments and convert to mp4
+            try:
+                combine_vod_parts(stream_json, print_progress=not self.quiet)
+                convert_vod(stream_json, [(0, 99999)], print_progress=not self.quiet)
+
+            except Exception as e:
+                raise VodMergeError(e) from e
+
+            self.log.debug('Cleaning up temporary files...')
+            cleanup_vod_parts(stream_json['store_directory'])
+
+            return stream_json
+
+        except KeyboardInterrupt:
+            self.log.debug('User requested stop, halting stream downloader.')
+            if Path(self.config_dir, f'.lock.{channel_data["user_name"]}').exists():
+                remove_lock(self.config_dir, channel_data[0]['id'] + '-stream-only')
+
+            sys.exit(0)
+
+        except (RequestError, VodMergeError) as e:
+            self.log.debug('Exception downloading or merging stream.\n{e}', exc_info=True)
+            send_push(self.pushbullet_key, 'Exception encountered while downloading or merging downloaded stream '
+                                           f'by {channel_data["user_name"]}', str(e))
+
+        except BaseException as e:
+            self.log.error('Unexpected exception encountered while downloading live-only stream.\n%s', str(e),
+                           exc_info=True)
+            send_push(self.pushbullet_key, 'Unexpected exception encountered while downloading live-only stream '
+                                           f'by {channel_data["user_name"]}', str(e))
+
+        return False
+
+    def get_vod_connector(self, vod_id, get_video, get_chat):
+        """Download a single vod or list of vod IDs.
+
+        :param vod_id: vod id to download
+        :param get_video: bool whether to grab video
+        :param get_chat: bool whether to grab chat logs
+        :return: dict containing current vod information returned by get_vod
+        """
+        self.log.info('Now processing VOD: %s', vod_id)
+        vod_json = self.call_twitch.get_api(f'videos?id={vod_id}')['data'][0]
+        vod_json['vod_id'] = vod_json.pop('id')
+        vod_json['muted_segments'] = str(vod_json['muted_segments'])
+        vod_json['store_directory'] = \
+            str(Path(self.vod_directory, f'{sanitize_date(vod_json["created_at"])} - '
+                                         f'{sanitize_text(vod_json["title"])} - {vod_id}'))
+        vod_json['duration'] = convert_to_seconds(vod_json['duration'])
+
+        # get vod status
+        vod_live = self.call_twitch.get_vod_status(vod_json['user_id'], vod_json['created_at'])
+
+        self.log.info("VOD %s", 'currently or recently live. Running in LIVE mode.' if vod_live else 'offline.')
+
+        _r = None
+
+        try:
+            # begin real-time archiver if VOD still live and real-time archiver enabled
+            if self.real_time_archiver and vod_live:
+                stream = Stream(self.client_id, self.client_secret, self.oauth_token)
+                # concurrently grab live pieces and vod chunks
+
+                workers = []
+
+                # the stream module itself has no checks for what to download so this is done here
+                if get_video:
+                    workers.append(multiprocessing.Process(target=stream.get_stream, args=(
+                        vod_json['user_name'], Path(vod_json['store_directory'], 'parts'), self.quality)))
+
+                workers.append(multiprocessing.Process(target=self.get_vod, args=(
+                    vod_json, get_video, get_chat, vod_live)))
+
+                for worker in workers:
+                    worker.start()
+
+                for worker in workers:
+                    worker.join()
+
+            else:
+                self.get_vod(vod_json, get_video, get_chat, vod_live)
+
+            # return imported json rather than returning from get_vod process as there were issues with returning
+            # values via multiprocessing
+            vod_json = import_json(vod_json)
+
+            # combine vod segments
+            if get_video:
+                # combine all the 10s long .ts parts into a single file, then convert to .mp4
+                try:
+                    # retrieve vod chapters
+                    try:
+                        vod_chapters = Twitch.get_vod_chapters(vod_id)
+                        if vod_chapters:
+                            # write chapters to file
+                            with open(Path(vod_json['store_directory'], 'chapters.json'), 'w',
+                                      encoding='utf8') as chapters_file:
+                                chapters_file.write(json.dumps(vod_chapters))
+
+                        else:
+                            # get category if no separate chapters found
+                            vod_chapters = (Twitch.get_vod_category(vod_id), 0, vod_json['duration'] * 1000)
+
+                        # format and write vod chapters to parts dir
+                        with open(Path(vod_json['store_directory'], 'parts', 'chapters.txt'),
+                                  'w', encoding='utf8') as chapters_file:
+                            chapters_file.write(format_vod_chapters(vod_chapters))
+
+                    except BaseException as e:
+                        self.log.error('Failed to retrieve or insert chapters into VOD file. %s', str(e))
+
+                    try:
+                        combine_vod_parts(vod_json, print_progress=not self.quiet)
+                        # load muted segments if any exists
+                        with open(Path(vod_json['store_directory'], 'parts', '.muted'), 'r',
+                                  encoding='utf8') as mutefile:
+                            muted_segments = json.load(mutefile)
+                        convert_vod(vod_json, muted_segments, print_progress=not self.quiet)
+
+                    except CorruptPartError as c:
+                        self.log.error("Corrupt segments found while converting VOD. Attempting to retry parts:"
+                                       "\n%s", ', '.join([str(p) for p in c.parts]))
+
+                        # check vod still available
+                        if not self.call_twitch.get_vod_index(vod_json, self.quality):
+                            raise VodDownloadError("Corrupt segments were found while converting VOD and TA was "
+                                                   "unable to re-download the missing segments. Either re-download "
+                                                   "the VOD if it is still available, or manually convert 'merged.ts' "
+                                                   f"using FFmpeg. Corrupt parts:\n{', '.join(c.f_parts)}")
+
+                        # rename corrupt segments
+                        for part in c.parts:
+                            # convert part number to segment file
+                            part = str(f'{int(part):05d}' + '.ts')
+
+                            # rename part
+                            shutil.move(Path(vod_json['store_directory'], 'parts', part),
+                                        Path(vod_json['store_directory'], 'parts', part + '.corrupt'))
+
+                        # download and combine vod again
+                        try:
+                            self.get_vod(vod_json, True, False, False)
+
+                            # compare downloaded .ts to corrupt parts - corrupt parts SHOULD have different hashes
+                            # so we can work out if a segment is corrupt on twitch's end or ours
+                            for part_num in c.parts:
+                                part = str('{:05d}'.format(int(part_num)) + '.ts')
+
+                                # compare hashes
+                                if get_hash(Path(vod_json['store_directory'], 'parts', part)) == \
+                                        get_hash(Path(vod_json['store_directory'], 'parts', part + '.corrupt')):
+                                    self.log.debug(f"Re-downloaded .ts segment {part_num} matches corrupt one, "
+                                                   "assuming corruption is on Twitch's end and ignoring.")
+                                    muted_segments.append([part_num, part_num])
+
+                            combine_vod_parts(vod_json, print_progress=not self.quiet)
+                            convert_vod(vod_json, muted_segments, print_progress=not self.quiet)
+
+                        except CorruptPartError as e:
+                            raise VodDownloadError(
+                                "Corrupt part(s) still present after retrying VOD download. Ensure VOD is still "
+                                "available and either delete the listed #####.ts part(s) from 'parts' folder or entire "
+                                f"'parts' folder if issue persists.\n{', '.join(c.f_parts)}") from e
+
+                except BaseException as e:
+                    raise VodMergeError(e) from e
+
+                # verify vod length is equal to what is grabbed from twitch
+                if verify_vod_length(vod_json):
+                    raise VodMergeError('VOD length outside of acceptable range. If error persists delete '
+                                        "'vod/parts' directory if VOD still available.")
+
+            if get_chat:
+                try:
+                    with open(Path(vod_json['store_directory'], 'verbose_chat.json'), 'r',
+                              encoding='utf8') as chat_file:
+                        chat_log = json.loads(chat_file.read())
+
+                    # generate and export the readable chat log
+                    if chat_log:
+                        try:
+                            self.log.debug('Generating readable chat log and saving to disk...')
+                            r_chat_log = generate_readable_chat_log(chat_log, datetime.strptime(
+                                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc))
+                            export_readable_chat_log(r_chat_log, vod_json['store_directory'])
+
+                        except BaseException as e:
+                            raise ChatExportError(e) from e
+
+                    else:
+                        self.log.info('No chat messages found.')
+
+                # catch missing chat log and modify database insert
+                except FileNotFoundError:
+                    self.log.error('No chat log found, download likely failed or log unavailable.')
+                    vod_json['chat_archived'] = False
+
+            if get_video:
+                # grab thumbnail at 1080p resolution - any resolution can be used but this should be fine for almost
+                # every stream
+                try:
+                    self.log.debug('Downloading VOD thumbnail.')
+                    thumbnail = Api.get_request(vod_json['thumbnail_url'].replace('%{width}x%{height}', '1920x1080'))
+                    with open(Path(vod_json['store_directory'], 'thumbnail.jpg'), 'wb') as thumbnail_file:
+                        thumbnail_file.write(thumbnail.content)
+
+                except BaseException as e:
+                    self.log.error('Failed to grab thumbnail for VOD. Error: %s', str(e))
+
+                # delete temporary .ts parts and merged.ts file
+                self.log.debug('Cleaning up temporary files...')
+                cleanup_vod_parts(vod_json['store_directory'])
+
+        # catch user exiting and remove lock file
+        except KeyboardInterrupt:
+            if vod_live:
+                self.log.debug('User requested stop, terminating download workers...')
+                for worker in workers:
+                    worker.terminate()
+                    worker.join()
+
+            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
+                remove_lock(self.config_dir, vod_json['stream_id'])
+
+            sys.exit(0)
+
+        # catch halting errors, send notification and remove lock file
+        except (RequestError, VodDownloadError, ChatDownloadError, VodMergeError, ChatExportError) as e:
+            if vod_live:
+                self.log.debug('Exception encountered, terminating download workers...')
+                for worker in workers:
+                    worker.terminate()
+                    worker.join()
+
+            self.log.error('Error downloading VOD %s.', vod_id, exc_info=True)
+            send_push(self.pushbullet_key, f'Error downloading VOD {vod_id} by {vod_json["user_name"]}', str(e))
+            # remove lock file if archiving channel
+            if Path(self.config_dir, f'.lock.{vod_json["stream_id"]}').exists():
+                remove_lock(self.config_dir, vod_json['stream_id'])
+
+            # set to None so that channel function knows download failed
+            vod_json = None
+
+        # catch unhandled exceptions
+        except BaseException as e:
+            if vod_live:
+                self.log.debug('Exception encountered, terminating download workers...')
+                for worker in workers:
+                    worker.terminate()
+                    worker.join()
+
+            send_push(self.pushbullet_key, f'Exception encountered while downloading VOD {vod_id} by '
+                                           f'{vod_json["user_name"]}', str(e))
+            self.log.error('Exception encountered while downloading VOD %s.', vod_id, exc_info=True)
+            return
+
+        # this is only used when archiving a channel
+        return vod_json
+
+    def get_vod(self, vod_json, get_video=True, get_chat=True, vod_live=False):
+        """Retrieves a specified VOD.
+
+        :param vod_json: dict of vod parameters retrieved from twitch
+        :param get_video: boolean whether to grab video
+        :param get_chat: boolean whether to grab chat logs
+        :param vod_live: boolean true if vod currently live, false otherwise
+        :return: dict containing current vod information
+        """
+        # create vod dir
+        Path(vod_json['store_directory']).mkdir(parents=True, exist_ok=True)
+
+        # wait if vod recently created
+        if time_since_date(datetime.strptime(
+                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp()) < 300:
+            self.log.info('Waiting 5m to download initial VOD parts as it was created very recently. Live archiving '
+                          'will still function.')
+            sleep(300)
+
+        if time_since_date(datetime.strptime(
+                vod_json['created_at'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp()) \
+                < (vod_json['duration'] + 360):
+            self.log.debug('Time since VOD was created + its duration is a point in time < 10 minutes ago. '
+                           'Running in live mode in case not all parts are available yet.')
+            vod_live = True
+
+        # import chat log if it has been partially downloaded
+        try:
+            with open(Path(vod_json['store_directory'], 'verbose_chat.json'), 'r', encoding='utf8') as chat_file:
+                chat_log = json.loads(chat_file.read())
+
+            # ignore chat logs created with older incompatible schema - see v2.2.1 changes
+            if chat_log and 'contentOffsetSeconds' not in chat_log[0].keys():
+                chat_log = []
+
+        except FileNotFoundError:
+            chat_log = []
+
+        # fetch all streams for a particular vod
+        if get_video:
+            try:
+                vod_index = self.call_twitch.get_vod_index(vod_json, self.quality)
+
+                # attempt to fetch playlist for requested stream
+                Api.get_request(vod_index).text
+
+            except TwitchAPIErrorForbidden as e:
+                raise VodDownloadError('Error retrieving VOD index. VOD may have been deleted or supplied resolution '
+                                       f'was invalid. Error: {str(e)}') from e
+
+        # loop for processing live vods
+        while True:
+            try:
+                _r = self.call_twitch.get_api(f'videos?id={vod_json["vod_id"]}')
+
+                vod_json = _r['data'][0]
+                vod_json['vod_id'] = vod_json.pop('id')
+                vod_json['muted_segments'] = str(vod_json['muted_segments']) if vod_json['muted_segments'] else None
+                vod_json['store_directory'] = \
+                    str(Path(self.vod_directory, f'{sanitize_date(vod_json["created_at"])} - '
+                                                 f'{sanitize_text(vod_json["title"])} - {vod_json["vod_id"]}'))
+                vod_json['duration'] = convert_to_seconds(vod_json['duration'])
+
+                export_json(vod_json)
+
+            except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
+                self.log.warning('Error retrieving VOD json - VOD was likely deleted.')
+                with open(Path(vod_json['store_directory'], '.ignorelength'), 'w', encoding='utf8') as _:
+                    pass
+
+                vod_live = False
+
+            if get_video:
+                # download all available vod parts
+                self.log.info('Grabbing video...')
+                try:
+                    vod_playlist = Api.get_request(vod_index).text
+
+                    # update vod json with m3u8 duration - more accurate than twitch API
+                    _m = re.findall(r'(?<=#EXT-X-TWITCH-TOTAL-SECS:).*(?=\n)', vod_playlist)[0]
+                    vod_json['duration'] = floor(float(_m))
+                    export_json(vod_json)
+
+                    # replace extra chars in base_url like /chunked/index[-muted-JU07DEVBNK.m3u8]
+                    _m = re.findall(r'(?<=\/)(index.*)', vod_index)[0]
+                    vod_base_url = vod_index.replace(_m, '')
+
+                    self.download.get_m3u8_video(m3u8.loads(vod_playlist), vod_base_url, vod_json['store_directory'])
+
+                except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
+                    self.log.debug('Error 403 or 404 returned when downloading VOD parts - VOD was likely deleted.')
+                    with open(Path(vod_json['store_directory'], '.ignorelength'), 'w') as _:
+                        pass
+
+                    vod_live = False
+
+                except BaseException as e:
+                    raise VodDownloadError(e) from e
+
+            if get_chat:
+                # download all available chat segments
+                self.log.info('Grabbing chat logs...')
+                try:
+                    if not chat_log:
+                        chat_log = self.download.get_chat(vod_json)
+
+                    # only try to grab more chat logs if we aren't past vod length
+                    elif int(chat_log[-1]['contentOffsetSeconds']) < vod_json['duration']:
+                        self.log.debug(f'Grabbing chat logs from offset: {chat_log[-1]["contentOffsetSeconds"]}')
+                        chat_log.extend(
+                            [n for n in
+                             self.download.get_chat(vod_json, floor(int(chat_log[-1]['contentOffsetSeconds'])))
+                             if n['id'] not in [m['id'] for m in chat_log]])
+
+                    export_verbose_chat_log(chat_log, vod_json['store_directory'])
+
+                except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
+                    self.log.debug('Error 403 or 404 returned when downloading chat log - VOD was likely deleted.')
+                    with open(Path(vod_json['store_directory'], '.ignorelength'), 'w', encoding='utf8') as _:
+                        pass
+
+                    vod_live = False
+
+                except Exception as e:
+                    raise ChatDownloadError(e) from e
+
+            if vod_live:
+                # wait up to 10 minutes, checking every minute to verify if vod is still being updated or not
+                for _ in range(11):
+                    self.log.debug('Waiting 60s to see if VOD changes.')
+                    sleep(60)
+                    try:
+                        # restart while loop if new video segments found
+                        if len(m3u8.loads(vod_playlist).segments) \
+                                < len(m3u8.loads(Api.get_request(vod_index).text).segments):
+                            self.log.debug('New VOD parts found.')
+                            vod_live = True
+                            break
+
+                        # exit loop if 10 minutes pass without new vod segments being added
+                        if _ > 9:
+                            self.log.debug('10m has passed since VOD duration changed - assuming it is no longer live.')
+                            vod_live = False
+
+                        else:
+                            continue
+
+                    except (TwitchAPIErrorNotFound, TwitchAPIErrorForbidden):
+                        self.log.debug('Error 403 or 404 returned when checking for new VOD parts - VOD was likely'
+                                       ' deleted.')
+                        vod_live = False
+                        break
+
+            else:
+                break
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/stream.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/stream.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,304 +1,304 @@
-"""
-Module for downloading currently live Twitch broadcasts.
-"""
-
-import logging
-import os
-import tempfile
-
-from datetime import datetime, timezone
-from glob import glob
-from math import floor
-from pathlib import Path
-from time import sleep
-
-import m3u8
-import requests
-
-from twitcharchiver.api import Api
-from twitcharchiver.exceptions import TwitchAPIErrorNotFound, UnsupportedStreamPartDuration
-from twitcharchiver.twitch import Twitch
-from twitcharchiver.utils import time_since_date, safe_move
-
-
-class Stream:
-    """
-    Functions pertaining to grabbing and downloading stream segments.
-    """
-    def __init__(self, client_id, client_secret, oauth_token):
-
-        self.log = logging.getLogger()
-
-        self.call_twitch = Twitch(client_id, client_secret, oauth_token)
-
-        self.buffer = {}
-        self.segment_ids = {}
-        self.downloaded_segments = set()
-        # track progress for unsynced streams
-        self.processed_segments = set()
-        self.segment_id = 0
-
-    def unsynced_setup(self, output_dir):
-        # get existing parts to resume counting if archiving halted
-        existing_parts = [Path(p) for p in sorted(glob(str(Path(output_dir, '*.ts'))))]
-        if existing_parts:
-            # set to 1 above highest numbered part
-            self.segment_id = int(existing_parts[-1].name.strip('.ts')) + 1
-
-        self.buffer[self.segment_id] = []
-        self.segment_ids[self.segment_id] = os.urandom(24).hex()
-
-    def get_stream(self, channel, output_dir, quality='best', sync_vod_segments=True):
-        """Retrieves a stream for a specified channel.
-
-        :param channel: name of twitch channel to download
-        :param output_dir: location to place downloaded .ts chunks
-        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
-        :param sync_vod_segments: create segments for combining with archived VOD parts. If true we will try to recreate
-                                  the segment numbering scheme Twitch uses, otherwise we use our own numbering scheme.
-                                  Used when archiving a live stream without a VOD.
-        """
-        Path(output_dir).mkdir(parents=True, exist_ok=True)
-        latest_segment = None
-        latest_segment_timestamp = None
-
-        # vars for unsynced download - skip if running in synced mode, or setup already performed
-        if not sync_vod_segments and not self.segment_ids:
-            self.unsynced_setup(output_dir)
-
-        try:
-            self.log.debug('Fetching required stream information.')
-            index_uri = self.call_twitch.get_channel_hls_index(channel, quality)
-            stream_json = self.call_twitch.get_api(f'users?login={channel}')['data'][0]
-            user_id = stream_json['id']
-            latest_vod_created_time = self.call_twitch.get_api(f'videos?user_id={user_id}')['data'][0]['created_at']
-            latest_vod_created_time = datetime.strptime(latest_vod_created_time, '%Y-%m-%dT%H:%M:%SZ')
-
-        # raised when channel goes offline
-        except TwitchAPIErrorNotFound:
-            self.log.error('Stream offline.')
-            return
-
-        while True:
-            start_timestamp = int(datetime.utcnow().timestamp())
-
-            # attempt to grab new segments from Twitch
-            for attempt in range(6):
-                if attempt > 4:
-                    return
-
-                try:
-                    self.log.debug('Fetching incoming stream segments.')
-                    incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
-                    break
-
-                # stream has ended if exception encountered
-                except TwitchAPIErrorNotFound:
-                    self.get_final_segment(self.buffer, output_dir, self.segment_ids)
-                    return
-
-                except requests.exceptions.ConnectTimeout:
-                    self.log.debug('Timed out attempting to fetch new stream segments, retrying. (Attempt %s)',
-                                   attempt + 1)
-                    continue
-
-            # set latest segment and timestamp if new segment found
-            if incoming_segments['segments'][-1]['uri'] != latest_segment:
-                latest_segment = incoming_segments['segments'][-1]['uri']
-                latest_segment_timestamp = int(datetime.now(timezone.utc).timestamp())
-
-            # assume stream has ended once >20s has passed since the last segment was advertised
-            if self.buffer and time_since_date(latest_segment_timestamp) > 20:
-                self.get_final_segment(self.buffer, output_dir, self.segment_ids)
-                return
-
-            if not sync_vod_segments:
-                self.build_unsynced_buffer(incoming_segments)
-
-            else:
-                self.build_synced_buffer(incoming_segments, latest_vod_created_time)
-
-            # download buffer and store completed segments
-            self.download_buffer(output_dir)
-
-            # sleep if processing time < 4s before checking for new segments
-            processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
-            if processing_time < 4:
-                sleep(4 - processing_time)
-
-    def build_synced_buffer(self, incoming_segments, latest_vod_created_time):
-        """Creates a buffer of parts to download without syncing with the part timestamping used by Twitch VODs.
-
-        :param incoming_segments: dict of segments advertised by Twitch
-        :param latest_vod_created_time: timestamp of vod creation
-        """
-        # manage incoming segments and create buffer of segments to download
-        bad_segments = []
-        for segment in incoming_segments['segments']:
-            self.log.debug('Processing part: %s', segment)
-
-            # skip ad segments
-            if segment['title'] != 'live':
-                self.log.debug('Ad detected, skipping.')
-                continue
-
-            # catch streams with dynamic part length - set to 2 as often the final 2 segments are < 2s
-            if len(bad_segments) > 2:
-                raise UnsupportedStreamPartDuration
-
-            if segment['duration'] != 2.0 and segment not in bad_segments:
-                self.log.debug("Part has invalid duration (%s).", segment['duration'])
-                bad_segments.append(segment)
-                continue
-
-            # get time between vod start and segment time
-            time_since_start = \
-                segment['program_date_time'].replace(
-                    tzinfo=None).timestamp() - latest_vod_created_time.timestamp()
-
-            # get segment id based on time since vod start
-            # manual offset of 4 seconds is added - it just works
-            segment_id = floor((4 + time_since_start) / 10)
-
-            if segment_id in self.downloaded_segments:
-                continue
-
-            if segment_id not in self.segment_ids.keys():
-                self.log.debug('New live segment found: %s', segment_id)
-                # give each segment id a unique id
-                self.segment_ids[segment_id] = os.urandom(24).hex()
-                self.buffer[segment_id] = []
-
-            segment = tuple(
-                (segment['uri'], segment['program_date_time'].replace(tzinfo=None), segment['duration']))
-
-            # only continue processing if segment not yet in buffer for segment id
-            if segment in self.buffer[segment_id]:
-                continue
-
-            self.log.debug('New part added to buffer: %s <- %s', segment_id, segment)
-            self.buffer[segment_id].append(segment)
-
-    def build_unsynced_buffer(self, incoming_segments):
-        """Creates a buffer of parts to download without syncing with the part timestamping used by Twitch VODs.
-
-        :param incoming_segments: dict of segments advertised by Twitch
-        :return: updated segment id
-        """
-        # manage incoming segments and create buffer of segments to download
-        bad_segments = []
-        for segment in incoming_segments['segments']:
-            self.log.debug('Processing part: %s', segment)
-
-            # skip ad segments
-            if segment['title'] != 'live':
-                self.log.debug('Ad detected, skipping.')
-                continue
-
-            # catch streams with dynamic part length - set to 2 as often the final 2 segments are < 2s
-            if len(bad_segments) > 2:
-                raise UnsupportedStreamPartDuration
-
-            segment = tuple(
-                (segment['uri'], segment['program_date_time'].replace(tzinfo=None), segment['duration']))
-
-            # skip already processed segments
-            if segment in self.processed_segments:
-                continue
-
-            self.processed_segments.add(segment)
-
-            # check if segment already completed as id may not have been incremented if current segment is
-            # completed before the next pass causing a KeyError
-            if self.segment_id in self.downloaded_segments or len(self.buffer[self.segment_id]) == 5:
-                self.segment_id += 1
-
-            # add segment id to buffer if not present
-            if self.segment_id not in self.buffer.keys():
-                self.segment_ids[self.segment_id] = os.urandom(24).hex()
-                self.buffer[self.segment_id] = []
-
-            self.log.debug('New part added to buffer: %s <- %s', self.segment_id, segment)
-            self.buffer[self.segment_id].append(segment)
-
-    def download_buffer(self, output_dir):
-        """Downloads all completed segments (containing 5 parts) from the buffer to the desired directory.
-
-        :param output_dir: path to download buffer to
-        """
-        for segment_id in [seg_id for seg_id in self.buffer.keys() if len(self.buffer[seg_id]) == 5]:
-            for attempt in range(6):
-                if attempt > 4:
-                    self.log.error('Maximum attempts reached while downloading segment %s.', segment_id)
-                    break
-
-                if self.write_buffer_segment(segment_id, output_dir, self.segment_ids[segment_id],
-                                             self.buffer[segment_id]):
-                    continue
-
-                # clean buffer
-                self.buffer.pop(segment_id)
-                self.downloaded_segments.add(segment_id)
-                break
-
-    def write_buffer_segment(self, segment_id, output_dir, tmp_file, segment_parts):
-        """Downloads and moves a given segment from the buffer.
-
-        :param segment_id: numbered segment to download
-        :param output_dir: location to output segment to
-        :param tmp_file: name of temporary file
-        :param segment_parts: list of parts which make up the segment
-        :return: True on error
-        """
-        with open(Path(tempfile.gettempdir(), tmp_file), 'wb') as tmp_ts_file:
-            for segment in segment_parts:
-                try:
-                    _r = requests.get(segment[0], stream=True, timeout=5)
-
-                    if _r.status_code != 200:
-                        return True
-
-                    # write part to file
-                    for chunk in _r.iter_content(chunk_size=262144):
-                        tmp_ts_file.write(chunk)
-
-                except requests.exceptions.RequestException as e:
-                    self.log.debug(
-                        'Error downloading VOD stream segment %s : %s. Error: %s', segment_id, segment, str(e))
-                    return True
-
-        # move finished ts file to destination storage
-        try:
-            safe_move(Path(tempfile.gettempdir(), tmp_file), Path(output_dir, str(f'{segment_id:05d}' + '.ts')))
-            self.log.debug('Live segment: %s completed.', segment_id)
-
-        except BaseException as e:
-            self.log.debug('Exception while moving stream segment %s. Error: %s', segment_id, str(e))
-            return True
-
-        return False
-
-    def get_final_segment(self, buffer, output_dir, segment_ids):
-        """Downloads and stores the final stream segments.
-
-        :param buffer: segments which are available for download
-        :param output_dir: location to move completed segment to
-        :param segment_ids: segment id(s) to download
-        """
-        # ensure final segment present
-        if buffer.keys():
-            # export the highest segment if stream ends before final segment meets requirements
-            last_id = max(buffer.keys())
-
-            if not Path(output_dir, str(f'{last_id:05d}') + '.ts').exists():
-                self.log.debug('Final part not found in output directory, assuming last segment is complete and'
-                               ' downloading.')
-                for attempt in range(6):
-                    if attempt > 4:
-                        self.log.debug('Maximum attempts reached while downloading segment %s.', last_id)
-                        break
-
-                    if self.write_buffer_segment(last_id, output_dir, segment_ids[last_id], buffer[last_id]):
-                        continue
-
-                    break
+"""
+Module for downloading currently live Twitch broadcasts.
+"""
+
+import logging
+import os
+import tempfile
+
+from datetime import datetime, timezone
+from glob import glob
+from math import floor
+from pathlib import Path
+from time import sleep
+
+import m3u8
+import requests
+
+from twitcharchiver.api import Api
+from twitcharchiver.exceptions import TwitchAPIErrorNotFound, UnsupportedStreamPartDuration
+from twitcharchiver.twitch import Twitch
+from twitcharchiver.utils import time_since_date, safe_move
+
+
+class Stream:
+    """
+    Functions pertaining to grabbing and downloading stream segments.
+    """
+    def __init__(self, client_id, client_secret, oauth_token):
+
+        self.log = logging.getLogger()
+
+        self.call_twitch = Twitch(client_id, client_secret, oauth_token)
+
+        self.buffer = {}
+        self.segment_ids = {}
+        self.downloaded_segments = set()
+        # track progress for unsynced streams
+        self.processed_segments = set()
+        self.segment_id = 0
+
+    def unsynced_setup(self, output_dir):
+        # get existing parts to resume counting if archiving halted
+        existing_parts = [Path(p) for p in sorted(glob(str(Path(output_dir, '*.ts'))))]
+        if existing_parts:
+            # set to 1 above highest numbered part
+            self.segment_id = int(existing_parts[-1].name.strip('.ts')) + 1
+
+        self.buffer[self.segment_id] = []
+        self.segment_ids[self.segment_id] = os.urandom(24).hex()
+
+    def get_stream(self, channel, output_dir, quality='best', sync_vod_segments=True):
+        """Retrieves a stream for a specified channel.
+
+        :param channel: name of twitch channel to download
+        :param output_dir: location to place downloaded .ts chunks
+        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
+        :param sync_vod_segments: create segments for combining with archived VOD parts. If true we will try to recreate
+                                  the segment numbering scheme Twitch uses, otherwise we use our own numbering scheme.
+                                  Used when archiving a live stream without a VOD.
+        """
+        Path(output_dir).mkdir(parents=True, exist_ok=True)
+        latest_segment = None
+        latest_segment_timestamp = None
+
+        # vars for unsynced download - skip if running in synced mode, or setup already performed
+        if not sync_vod_segments and not self.segment_ids:
+            self.unsynced_setup(output_dir)
+
+        try:
+            self.log.debug('Fetching required stream information.')
+            index_uri = self.call_twitch.get_channel_hls_index(channel, quality)
+            stream_json = self.call_twitch.get_api(f'users?login={channel}')['data'][0]
+            user_id = stream_json['id']
+            latest_vod_created_time = self.call_twitch.get_api(f'videos?user_id={user_id}')['data'][0]['created_at']
+            latest_vod_created_time = datetime.strptime(latest_vod_created_time, '%Y-%m-%dT%H:%M:%SZ')
+
+        # raised when channel goes offline
+        except TwitchAPIErrorNotFound:
+            self.log.error('Stream offline.')
+            return
+
+        while True:
+            start_timestamp = int(datetime.utcnow().timestamp())
+
+            # attempt to grab new segments from Twitch
+            for attempt in range(6):
+                if attempt > 4:
+                    return
+
+                try:
+                    self.log.debug('Fetching incoming stream segments.')
+                    incoming_segments = m3u8.loads(Api.get_request(index_uri).text).data
+                    break
+
+                # stream has ended if exception encountered
+                except TwitchAPIErrorNotFound:
+                    self.get_final_segment(self.buffer, output_dir, self.segment_ids)
+                    return
+
+                except requests.exceptions.ConnectTimeout:
+                    self.log.debug('Timed out attempting to fetch new stream segments, retrying. (Attempt %s)',
+                                   attempt + 1)
+                    continue
+
+            # set latest segment and timestamp if new segment found
+            if incoming_segments['segments'][-1]['uri'] != latest_segment:
+                latest_segment = incoming_segments['segments'][-1]['uri']
+                latest_segment_timestamp = int(datetime.now(timezone.utc).timestamp())
+
+            # assume stream has ended once >20s has passed since the last segment was advertised
+            if self.buffer and time_since_date(latest_segment_timestamp) > 20:
+                self.get_final_segment(self.buffer, output_dir, self.segment_ids)
+                return
+
+            if not sync_vod_segments:
+                self.build_unsynced_buffer(incoming_segments)
+
+            else:
+                self.build_synced_buffer(incoming_segments, latest_vod_created_time)
+
+            # download buffer and store completed segments
+            self.download_buffer(output_dir)
+
+            # sleep if processing time < 4s before checking for new segments
+            processing_time = int(datetime.utcnow().timestamp() - start_timestamp)
+            if processing_time < 4:
+                sleep(4 - processing_time)
+
+    def build_synced_buffer(self, incoming_segments, latest_vod_created_time):
+        """Creates a buffer of parts to download without syncing with the part timestamping used by Twitch VODs.
+
+        :param incoming_segments: dict of segments advertised by Twitch
+        :param latest_vod_created_time: timestamp of vod creation
+        """
+        # manage incoming segments and create buffer of segments to download
+        bad_segments = []
+        for segment in incoming_segments['segments']:
+            self.log.debug('Processing part: %s', segment)
+
+            # skip ad segments
+            if segment['title'] != 'live':
+                self.log.debug('Ad detected, skipping.')
+                continue
+
+            # catch streams with dynamic part length - set to 2 as often the final 2 segments are < 2s
+            if len(bad_segments) > 2:
+                raise UnsupportedStreamPartDuration
+
+            if segment['duration'] != 2.0 and segment not in bad_segments:
+                self.log.debug("Part has invalid duration (%s).", segment['duration'])
+                bad_segments.append(segment)
+                continue
+
+            # get time between vod start and segment time
+            time_since_start = \
+                segment['program_date_time'].replace(
+                    tzinfo=None).timestamp() - latest_vod_created_time.timestamp()
+
+            # get segment id based on time since vod start
+            # manual offset of 4 seconds is added - it just works
+            segment_id = floor((4 + time_since_start) / 10)
+
+            if segment_id in self.downloaded_segments:
+                continue
+
+            if segment_id not in self.segment_ids.keys():
+                self.log.debug('New live segment found: %s', segment_id)
+                # give each segment id a unique id
+                self.segment_ids[segment_id] = os.urandom(24).hex()
+                self.buffer[segment_id] = []
+
+            segment = tuple(
+                (segment['uri'], segment['program_date_time'].replace(tzinfo=None), segment['duration']))
+
+            # only continue processing if segment not yet in buffer for segment id
+            if segment in self.buffer[segment_id]:
+                continue
+
+            self.log.debug('New part added to buffer: %s <- %s', segment_id, segment)
+            self.buffer[segment_id].append(segment)
+
+    def build_unsynced_buffer(self, incoming_segments):
+        """Creates a buffer of parts to download without syncing with the part timestamping used by Twitch VODs.
+
+        :param incoming_segments: dict of segments advertised by Twitch
+        :return: updated segment id
+        """
+        # manage incoming segments and create buffer of segments to download
+        bad_segments = []
+        for segment in incoming_segments['segments']:
+            self.log.debug('Processing part: %s', segment)
+
+            # skip ad segments
+            if segment['title'] != 'live':
+                self.log.debug('Ad detected, skipping.')
+                continue
+
+            # catch streams with dynamic part length - set to 2 as often the final 2 segments are < 2s
+            if len(bad_segments) > 2:
+                raise UnsupportedStreamPartDuration
+
+            segment = tuple(
+                (segment['uri'], segment['program_date_time'].replace(tzinfo=None), segment['duration']))
+
+            # skip already processed segments
+            if segment in self.processed_segments:
+                continue
+
+            self.processed_segments.add(segment)
+
+            # check if segment already completed as id may not have been incremented if current segment is
+            # completed before the next pass causing a KeyError
+            if self.segment_id in self.downloaded_segments or len(self.buffer[self.segment_id]) == 5:
+                self.segment_id += 1
+
+            # add segment id to buffer if not present
+            if self.segment_id not in self.buffer.keys():
+                self.segment_ids[self.segment_id] = os.urandom(24).hex()
+                self.buffer[self.segment_id] = []
+
+            self.log.debug('New part added to buffer: %s <- %s', self.segment_id, segment)
+            self.buffer[self.segment_id].append(segment)
+
+    def download_buffer(self, output_dir):
+        """Downloads all completed segments (containing 5 parts) from the buffer to the desired directory.
+
+        :param output_dir: path to download buffer to
+        """
+        for segment_id in [seg_id for seg_id in self.buffer.keys() if len(self.buffer[seg_id]) == 5]:
+            for attempt in range(6):
+                if attempt > 4:
+                    self.log.error('Maximum attempts reached while downloading segment %s.', segment_id)
+                    break
+
+                if self.write_buffer_segment(segment_id, output_dir, self.segment_ids[segment_id],
+                                             self.buffer[segment_id]):
+                    continue
+
+                # clean buffer
+                self.buffer.pop(segment_id)
+                self.downloaded_segments.add(segment_id)
+                break
+
+    def write_buffer_segment(self, segment_id, output_dir, tmp_file, segment_parts):
+        """Downloads and moves a given segment from the buffer.
+
+        :param segment_id: numbered segment to download
+        :param output_dir: location to output segment to
+        :param tmp_file: name of temporary file
+        :param segment_parts: list of parts which make up the segment
+        :return: True on error
+        """
+        with open(Path(tempfile.gettempdir(), tmp_file), 'wb') as tmp_ts_file:
+            for segment in segment_parts:
+                try:
+                    _r = requests.get(segment[0], stream=True, timeout=5)
+
+                    if _r.status_code != 200:
+                        return True
+
+                    # write part to file
+                    for chunk in _r.iter_content(chunk_size=262144):
+                        tmp_ts_file.write(chunk)
+
+                except requests.exceptions.RequestException as e:
+                    self.log.debug(
+                        'Error downloading VOD stream segment %s : %s. Error: %s', segment_id, segment, str(e))
+                    return True
+
+        # move finished ts file to destination storage
+        try:
+            safe_move(Path(tempfile.gettempdir(), tmp_file), Path(output_dir, str(f'{segment_id:05d}' + '.ts')))
+            self.log.debug('Live segment: %s completed.', segment_id)
+
+        except BaseException as e:
+            self.log.debug('Exception while moving stream segment %s. Error: %s', segment_id, str(e))
+            return True
+
+        return False
+
+    def get_final_segment(self, buffer, output_dir, segment_ids):
+        """Downloads and stores the final stream segments.
+
+        :param buffer: segments which are available for download
+        :param output_dir: location to move completed segment to
+        :param segment_ids: segment id(s) to download
+        """
+        # ensure final segment present
+        if buffer.keys():
+            # export the highest segment if stream ends before final segment meets requirements
+            last_id = max(buffer.keys())
+
+            if not Path(output_dir, str(f'{last_id:05d}') + '.ts').exists():
+                self.log.debug('Final part not found in output directory, assuming last segment is complete and'
+                               ' downloading.')
+                for attempt in range(6):
+                    if attempt > 4:
+                        self.log.debug('Maximum attempts reached while downloading segment %s.', last_id)
+                        break
+
+                    if self.write_buffer_segment(last_id, output_dir, segment_ids[last_id], buffer[last_id]):
+                        continue
+
+                    break
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/twitch.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/twitch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,305 +1,353 @@
-"""
-Handler for any requests made to the Twitch API.
-"""
-
-import logging
-
-from datetime import datetime, timezone
-from random import randrange
-from time import sleep
-
-import m3u8
-
-from twitcharchiver.api import Api
-from twitcharchiver.exceptions import TwitchAPIError, TwitchAPIErrorForbidden
-from twitcharchiver.utils import get_quality_index, time_since_date
-
-
-class Twitch:
-    """
-    Functions and processes for interacting with the Twitch API.
-    """
-    def __init__(self, client_id=None, client_secret=None, oauth_token=None):
-        """Class constructor.
-
-        :param client_id: twitch client_id
-        :param client_secret: twitch client_secret
-        :param oauth_token: twitch oauth_token
-        """
-        self.log = logging.getLogger()
-
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.oauth_token = oauth_token
-
-    def get_api(self, api_path):
-        """Retrieves information from the Twitch API.
-
-        :param api_path: twitch api endpoint to send request to
-        :return: requests response json
-        """
-        _h = {'Authorization': f'Bearer {self.oauth_token}', 'Client-Id': self.client_id}
-        _r = Api.get_request(f'https://api.twitch.tv/helix/{api_path}', h=_h)
-
-        return _r.json()
-
-    def generate_oauth_token(self):
-        """Generates an OAuth token from the provided client ID and secret.
-
-        :return: oauth token
-        """
-        _d = {'client_id': self.client_id, 'client_secret': self.client_secret,
-              'grant_type': 'client_credentials'}
-        _t = Api.post_request('https://id.twitch.tv/oauth2/token', d=_d).json()['access_token']
-
-        return _t
-
-    def validate_oauth_token(self):
-        """Validates a specified OAuth token with Twitch.
-
-        :return: token expiration date
-        """
-        self.log.debug('Verifying OAuth token.')
-        _h = {'Authorization': f'Bearer {self.oauth_token}'}
-
-        try:
-            _r = Api.get_request('https://id.twitch.tv/oauth2/validate', h=_h)
-
-            self.log.info('OAuth token verified successfully. Expiring in %s', _r.json()["expires_in"])
-            return _r.json()['expires_in']
-
-        except TwitchAPIError as e:
-            self.log.debug('OAuth token validation failed. Error: %s', str(e))
-
-        # error on expired or invalid credentials
-        return 1
-
-    @staticmethod
-    def get_playback_access_token(vod_id):
-        """Gets a playback access token for a specified vod.
-
-        :param vod_id: id of vod to retrieve token for
-        :return: playback access token
-        """
-        # only accepts the default client ID for non-authenticated clients
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
-        _q = """
-        {{
-            videoPlaybackAccessToken(
-                id: {vod_id},
-                params: {{
-                    platform: "web",
-                    playerBackend: "mediaplayer",
-                    playerType: "site"
-                }}
-            ) {{
-                signature
-                value
-            }}
-        }}
-        """.format(vod_id=vod_id)
-        _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
-
-        return _r.json()['data']['videoPlaybackAccessToken']
-
-    def get_vod_index(self, vod_json, quality='best'):
-        """Retrieves an index of m3u8 streams for a given VOD.
-
-        :param vod_json: vod information retrieved from Twitch
-        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
-        :return: url of m3u8 playlist
-        """
-        access_token = self.get_playback_access_token(vod_json['vod_id'])
-
-        _p = {
-            'player': 'twitchweb',
-            'nauth': access_token['value'],
-            'nauthsig': access_token['signature'],
-            'allow_source': 'true',
-            'playlist_include_framerate': 'true',
-            'p': randrange(1000000, 9999999)
-        }
-
-        try:
-            _r = Api.get_request(f'https://usher.ttvnw.net/vod/{vod_json["vod_id"]}.m3u8', p=_p)
-
-            _index = m3u8.loads(_r.text)
-
-            # grab 'name' of m3u8 streams - contains [resolution]p[framerate]
-            available_resolutions = [m[0].group_id.split('p') for m in [m.media for m in _index.playlists] if
-                                     m[0].group_id != 'chunked']
-            # insert 'chunked' stream separately as its named differently
-            available_resolutions.insert(0, _index.media[0].name.split('p'))
-
-        # catch for sub-only vods
-        except TwitchAPIErrorForbidden as e:
-            # retrieve cloudfront storage location from VOD thumbnail
-            cf_info = vod_json['thumbnail_url'].split('/')
-            cf_domain = cf_info[4]
-            vod_uid = cf_info[5]
-
-            # parse user-provided quality
-            if quality == 'best':
-                quality = 'chunked'
-            elif quality == 'worst':
-                quality = '160p30'
-            else:
-                quality = 'p'.join(quality)
-
-            # create index url
-            index_url = f'https://{cf_domain}.cloudfront.net/{vod_uid}/{quality}/index-dvr.m3u8'
-            return index_url
-
-        return _index.playlists[get_quality_index(quality, available_resolutions)].uri
-
-    @staticmethod
-    def get_channel_hls_index(channel, quality='best'):
-        """Retrieves an index of a live m3u8 stream.
-
-        :param channel: name of channel to retrieve index of
-        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
-        :return: url of m3u8 playlist
-        """
-        channel = channel.lower()
-
-        access_token = Twitch.get_stream_playback_access_token(channel)
-
-        _p = {
-            'player': 'twitchweb',
-            'fast_bread': 'true',
-            'token': access_token['value'],
-            'sig': access_token['signature'],
-            'allow_source': 'true',
-            'playlist_include_framerate': 'true',
-            'player_backend': 'mediaplayer',
-            'supported_codecs': 'avc1',
-            'p': randrange(1000000, 9999999)
-        }
-        _r = Api.get_request(f'https://usher.ttvnw.net/api/channel/hls/{channel}.m3u8', p=_p)
-
-        _index = m3u8.loads(_r.text)
-
-        # grab 'name' of m3u8 streams - contains [resolution]p[framerate]
-        available_resolutions = [m[0].group_id.split('p') for m in [m.media for m in _index.playlists] if
-                                 m[0].group_id != 'chunked']
-        # insert 'chunked' stream separately as its named differently and strip ' (source)' from name
-        available_resolutions.insert(0, _index.media[0].name.strip(' (source)').split('p'))
-
-        return _index.playlists[get_quality_index(quality, available_resolutions)].uri
-
-    @staticmethod
-    def get_stream_playback_access_token(channel):
-        """Gets a stream access token for a specified channel.
-
-        :param channel: channel name to retrieve token for
-        :return: playback access token
-        """
-        # only accepts the default client ID for non-authenticated clients
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
-        _q = """
-        {{
-            streamPlaybackAccessToken(
-                channelName: "{channel}",
-                params: {{
-                    platform: "web",
-                    playerBackend: "mediaplayer",
-                    playerType: "embed"
-                }}
-            ) {{
-                signature
-                value
-            }}
-        }}
-        """.format(channel=channel.lower())
-        _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
-
-        return _r.json()['data']['streamPlaybackAccessToken']
-
-    @staticmethod
-    def get_vod_category(vod_id):
-        """Retrieves category for a specified VOD.
-
-        :param vod_id: id of twitch vod to retrieve information for
-        :return: name of category / game
-        """
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
-        _q = [{
-            "extensions": {
-                "persistedQuery": {
-                    "sha256Hash": "e1edae8122517d013405f237ffcc124515dc6ded82480a88daef69c83b53ac01",
-                    "version": 1
-                }
-            },
-            "operationName": "ComscoreStreamingQuery",
-            "variables": {
-                "channel": "",
-                "clipSlug": "",
-                "isClip": False,
-                "isLive": False,
-                "isVodOrCollection": True,
-                "vodID": str(vod_id)
-            }
-        }]
-
-        _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
-
-        return _r.json()[0]['data']['video']['game']['name']
-
-    def get_vod_status(self, user_id, vod_created_time):
-        """Determines whether a live stream is paired with a given vod.
-
-        :param user_id: twitch channel name
-        :param vod_created_time: time and date a vod was created
-        :return: True if vod and stream creation dates match
-        """
-        # wait until 1m has passed since vod created time as the stream api may not have updated yet
-        time_since_created = time_since_date(
-            datetime.strptime(vod_created_time, '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
-        if time_since_created < 60:
-            sleep(60 - time_since_created)
-        try:
-            # if stream live and vod start time matches
-            stream_created_time = \
-                datetime.strptime(self.get_api(f'streams?user_id={user_id}')['data'][0]['started_at'],
-                                  '%Y-%m-%dT%H:%M:%SZ').timestamp()
-            vod_created_time = datetime.strptime(vod_created_time, '%Y-%m-%dT%H:%M:%SZ').timestamp()
-            # if vod created within 10s of stream created time
-            if 10 >= vod_created_time - stream_created_time >= -10:
-                self.log.debug('VOD creation time is within 10s of stream created time, running in live mode.')
-                return True
-
-        except IndexError:
-            pass
-
-        return False
-
-    @staticmethod
-    def get_vod_chapters(vod_id):
-        """Retrieves the chapters for a given Twitch VOD.
-
-        :param vod_id: id of twitch vod to retrieve chapters for
-        :return: list of vod chapters
-        """
-        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
-        _q = [{
-            "extensions": {
-                "persistedQuery": {
-                    "sha256Hash": "8d2793384aac3773beab5e59bd5d6f585aedb923d292800119e03d40cd0f9b41",
-                    "version": 1
-                }
-            },
-            "operationName": "VideoPlayer_ChapterSelectButtonVideo",
-            "variables": {
-                "includePrivate": False,
-                "videoID": str(vod_id)
-            }
-        }]
-
-        _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
-
-        # extract and return list of moments from returned json
-        try:
-            return [node['node'] for node in _r.json()[0]['data']['video']['moments']['edges']]
-
-        except TypeError:
-            return []
+"""
+Handler for any requests made to the Twitch API.
+"""
+
+import logging
+
+from datetime import datetime, timezone
+from random import randrange
+from time import sleep
+
+import m3u8
+
+from twitcharchiver.api import Api
+from twitcharchiver.exceptions import TwitchAPIError, TwitchAPIErrorForbidden
+from twitcharchiver.utils import get_quality_index, time_since_date
+
+
+class Twitch:
+    """
+    Functions and processes for interacting with the Twitch API.
+    """
+    def __init__(self, client_id=None, client_secret=None, oauth_token=None):
+        """Class constructor.
+
+        :param client_id: twitch client_id
+        :param client_secret: twitch client_secret
+        :param oauth_token: twitch oauth_token
+        """
+        self.log = logging.getLogger()
+
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.oauth_token = oauth_token
+
+    def get_api(self, api_path):
+        """Retrieves information from the Twitch API.
+
+        :param api_path: twitch api endpoint to send request to
+        :return: requests response json
+        """
+        _h = {'Authorization': f'Bearer {self.oauth_token}', 'Client-Id': self.client_id}
+        _r = Api.get_request(f'https://api.twitch.tv/helix/{api_path}', h=_h)
+
+        return _r.json()
+
+    def generate_oauth_token(self):
+        """Generates an OAuth token from the provided client ID and secret.
+
+        :return: oauth token
+        """
+        _d = {'client_id': self.client_id, 'client_secret': self.client_secret,
+              'grant_type': 'client_credentials'}
+        _t = Api.post_request('https://id.twitch.tv/oauth2/token', d=_d).json()['access_token']
+
+        return _t
+
+    def validate_oauth_token(self):
+        """Validates a specified OAuth token with Twitch.
+
+        :return: token expiration date
+        """
+        self.log.debug('Verifying OAuth token.')
+        _h = {'Authorization': f'Bearer {self.oauth_token}'}
+
+        try:
+            _r = Api.get_request('https://id.twitch.tv/oauth2/validate', h=_h)
+
+            self.log.info('OAuth token verified successfully. Expiring in %s', _r.json()["expires_in"])
+            return _r.json()['expires_in']
+
+        except TwitchAPIError as e:
+            self.log.debug('OAuth token validation failed. Error: %s', str(e))
+
+        # error on expired or invalid credentials
+        return 1
+
+    @staticmethod
+    def get_playback_access_token(vod_id):
+        """Gets a playback access token for a specified vod.
+
+        :param vod_id: id of vod to retrieve token for
+        :return: playback access token
+        """
+        # only accepts the default client ID for non-authenticated clients
+        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _q = """
+        {{
+            videoPlaybackAccessToken(
+                id: {vod_id},
+                params: {{
+                    platform: "web",
+                    playerBackend: "mediaplayer",
+                    playerType: "site"
+                }}
+            ) {{
+                signature
+                value
+            }}
+        }}
+        """.format(vod_id=vod_id)
+        _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
+
+        return _r.json()['data']['videoPlaybackAccessToken']
+
+    @staticmethod
+    def get_channel_videos(channel):
+        """Retrieves archived (saved VODs) of a specified channel.
+
+        :param channel: Name of Twitch channel/user
+        :return: dict containing pairs of stream_id: vod_id
+        """
+        # Uses default client header
+        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _q = [{
+            "extensions": {
+                "persistedQuery": {
+                    "sha256Hash": "a937f1d22e269e39a03b509f65a7490f9fc247d7f83d6ac1421523e3b68042cb",
+                    "version": 1
+                }
+            },
+            "operationName": "FilterableVideoTower_Videos",
+            "variables": {
+                "broadcastType": "ARCHIVE",
+                "channelOwnerLogin": f"{channel.lower()}",
+                "limit": 30,
+                "videoSort": "TIME"
+            }
+        }]
+        _cursor = True
+        _ids = {}
+
+        # fetch video pages one after another as long as cursor exists
+        while _cursor:
+            _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
+            _d = _r.json()[0]['data']['user']['videos']
+
+            # extract vod and stream ids from thumbnail url (stream id isnt provided directly with this call) and
+            # add to id dict. this will likely break at some point but requires far fewer requests if there are
+            # hundreds of vods.
+            _thumbnail_urls = [v['node']['animatedPreviewURL'].split('/') for v in _d['edges']]
+            _ids.update({int(t[3].split('_')[2]): t[5].split('-')[0] for t in _thumbnail_urls})
+
+            # set cursor if nextPage provided
+            if _d['pageInfo']['hasNextPage']:
+                _cursor = _d['edges'][-1]['cursor']
+                _q[0]['variables']['cursor'] = _cursor
+
+            else:
+                _cursor = None
+
+        return _ids
+
+    def get_vod_index(self, vod_json, quality='best'):
+        """Retrieves an index of m3u8 streams for a given VOD.
+
+        :param vod_json: vod information retrieved from Twitch
+        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
+        :return: url of m3u8 playlist
+        """
+        access_token = self.get_playback_access_token(vod_json['vod_id'])
+
+        _p = {
+            'player': 'twitchweb',
+            'nauth': access_token['value'],
+            'nauthsig': access_token['signature'],
+            'allow_source': 'true',
+            'playlist_include_framerate': 'true',
+            'p': randrange(1000000, 9999999)
+        }
+
+        try:
+            _r = Api.get_request(f'https://usher.ttvnw.net/vod/{vod_json["vod_id"]}.m3u8', p=_p)
+
+            _index = m3u8.loads(_r.text)
+
+            # grab 'name' of m3u8 streams - contains [resolution]p[framerate]
+            available_resolutions = [m[0].group_id.split('p') for m in [m.media for m in _index.playlists] if
+                                     m[0].group_id != 'chunked']
+            # insert 'chunked' stream separately as its named differently
+            available_resolutions.insert(0, _index.media[0].name.split('p'))
+
+        # catch for sub-only vods
+        except TwitchAPIErrorForbidden as e:
+            # retrieve cloudfront storage location from VOD thumbnail
+            cf_info = vod_json['thumbnail_url'].split('/')
+            cf_domain = cf_info[4]
+            vod_uid = cf_info[5]
+
+            # parse user-provided quality
+            if quality == 'best':
+                quality = 'chunked'
+            elif quality == 'worst':
+                quality = '160p30'
+            else:
+                quality = 'p'.join(quality)
+
+            # create index url
+            index_url = f'https://{cf_domain}.cloudfront.net/{vod_uid}/{quality}/index-dvr.m3u8'
+            return index_url
+
+        return _index.playlists[get_quality_index(quality, available_resolutions)].uri
+
+    @staticmethod
+    def get_channel_hls_index(channel, quality='best'):
+        """Retrieves an index of a live m3u8 stream.
+
+        :param channel: name of channel to retrieve index of
+        :param quality: desired quality in the format [resolution]p[framerate] or 'best', 'worst'
+        :return: url of m3u8 playlist
+        """
+        channel = channel.lower()
+
+        access_token = Twitch.get_stream_playback_access_token(channel)
+
+        _p = {
+            'player': 'twitchweb',
+            'fast_bread': 'true',
+            'token': access_token['value'],
+            'sig': access_token['signature'],
+            'allow_source': 'true',
+            'playlist_include_framerate': 'true',
+            'player_backend': 'mediaplayer',
+            'supported_codecs': 'avc1',
+            'p': randrange(1000000, 9999999)
+        }
+        _r = Api.get_request(f'https://usher.ttvnw.net/api/channel/hls/{channel}.m3u8', p=_p)
+
+        _index = m3u8.loads(_r.text)
+
+        # grab 'name' of m3u8 streams - contains [resolution]p[framerate]
+        available_resolutions = [m[0].group_id.split('p') for m in [m.media for m in _index.playlists] if
+                                 m[0].group_id != 'chunked']
+        # insert 'chunked' stream separately as its named differently and strip ' (source)' from name
+        available_resolutions.insert(0, _index.media[0].name.strip(' (source)').split('p'))
+
+        return _index.playlists[get_quality_index(quality, available_resolutions)].uri
+
+    @staticmethod
+    def get_stream_playback_access_token(channel):
+        """Gets a stream access token for a specified channel.
+
+        :param channel: channel name to retrieve token for
+        :return: playback access token
+        """
+        # only accepts the default client ID for non-authenticated clients
+        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _q = """
+        {{
+            streamPlaybackAccessToken(
+                channelName: "{channel}",
+                params: {{
+                    platform: "web",
+                    playerBackend: "mediaplayer",
+                    playerType: "embed"
+                }}
+            ) {{
+                signature
+                value
+            }}
+        }}
+        """.format(channel=channel.lower())
+        _r = Api.post_request('https://gql.twitch.tv/gql', j={'query': _q}, h=_h)
+
+        return _r.json()['data']['streamPlaybackAccessToken']
+
+    @staticmethod
+    def get_vod_category(vod_id):
+        """Retrieves category for a specified VOD.
+
+        :param vod_id: id of twitch vod to retrieve information for
+        :return: name of category / game
+        """
+        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _q = [{
+            "extensions": {
+                "persistedQuery": {
+                    "sha256Hash": "e1edae8122517d013405f237ffcc124515dc6ded82480a88daef69c83b53ac01",
+                    "version": 1
+                }
+            },
+            "operationName": "ComscoreStreamingQuery",
+            "variables": {
+                "channel": "",
+                "clipSlug": "",
+                "isClip": False,
+                "isLive": False,
+                "isVodOrCollection": True,
+                "vodID": str(vod_id)
+            }
+        }]
+
+        _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
+
+        return _r.json()[0]['data']['video']['game']['name']
+
+    def get_vod_status(self, user_id, vod_created_time):
+        """Determines whether a live stream is paired with a given vod.
+
+        :param user_id: twitch channel name
+        :param vod_created_time: time and date a vod was created
+        :return: True if vod and stream creation dates match
+        """
+        # wait until 1m has passed since vod created time as the stream api may not have updated yet
+        time_since_created = time_since_date(
+            datetime.strptime(vod_created_time, '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc).timestamp())
+        if time_since_created < 60:
+            sleep(60 - time_since_created)
+        try:
+            # if stream live and vod start time matches
+            stream_created_time = \
+                datetime.strptime(self.get_api(f'streams?user_id={user_id}')['data'][0]['started_at'],
+                                  '%Y-%m-%dT%H:%M:%SZ').timestamp()
+            vod_created_time = datetime.strptime(vod_created_time, '%Y-%m-%dT%H:%M:%SZ').timestamp()
+            # if vod created within 10s of stream created time
+            if 10 >= vod_created_time - stream_created_time >= -10:
+                self.log.debug('VOD creation time is within 10s of stream created time, running in live mode.')
+                return True
+
+        except IndexError:
+            pass
+
+        return False
+
+    @staticmethod
+    def get_vod_chapters(vod_id):
+        """Retrieves the chapters for a given Twitch VOD.
+
+        :param vod_id: id of twitch vod to retrieve chapters for
+        :return: list of vod chapters
+        """
+        _h = {'Client-Id': 'kimne78kx3ncx6brgo4mv6wki5h1ko'}
+        _q = [{
+            "extensions": {
+                "persistedQuery": {
+                    "sha256Hash": "8d2793384aac3773beab5e59bd5d6f585aedb923d292800119e03d40cd0f9b41",
+                    "version": 1
+                }
+            },
+            "operationName": "VideoPlayer_ChapterSelectButtonVideo",
+            "variables": {
+                "includePrivate": False,
+                "videoID": str(vod_id)
+            }
+        }]
+
+        _r = Api.post_request('https://gql.twitch.tv/gql', j=_q, h=_h)
+
+        # extract and return list of moments from returned json
+        try:
+            return [node['node'] for node in _r.json()[0]['data']['video']['moments']['edges']]
+
+        except TypeError:
+            return []
```

### Comparing `twitch-archiver-3.0.0.dev5/twitcharchiver/utils.py` & `twitch-archiver-3.0.0.dev6/twitcharchiver/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,719 +1,719 @@
-"""
-Various utility functions for modifying, retrieving and saving information.
-"""
-
-import hashlib
-import json
-import logging
-import os
-import re
-import shutil
-import subprocess
-
-from datetime import datetime, timezone
-from glob import glob
-from itertools import groupby
-from math import ceil, floor
-from pathlib import Path
-from textwrap import dedent
-
-import requests
-
-from twitcharchiver.exceptions import VodConvertError, CorruptPartError
-
-log = logging.getLogger()
-
-
-def generate_readable_chat_log(chat_log, stream_start):
-    """Converts the raw chat log into a scrollable, readable format.
-
-    :param chat_log: list of chat messages retrieved from twitch which are to be converted
-    :param stream_start: stream start utc timestamp
-    :return: formatted chat log
-    """
-    r_chat_log = []
-    for comment in chat_log:
-        # format comments with / without millisecond timestamp
-        if '.' in comment['createdAt']:
-            created_time = \
-                datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
-        else:
-            created_time = \
-                datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc)
-
-        comment_time = f'{get_time_difference(stream_start, created_time):.3f}'
-
-        # catch comments without commenter informations
-        if comment['commenter']:
-            user_name = str(comment['commenter']['displayName'])
-        else:
-            user_name = '~MISSING_COMMENTER_INFO~'
-
-        # catch comments without data
-        if comment['message']['fragments']:
-            user_message = str(comment['message']['fragments'][0]['text'])
-        else:
-            user_message = '~MISSING_MESSAGE_INFO~'
-
-        user_badges = ''
-        try:
-            for badge in comment['message']['userBadges']:
-                if 'broadcaster' in badge['setID']:
-                    user_badges += '(B)'
-
-                if 'moderator' in badge['setID']:
-                    user_badges += '(M)'
-
-                if 'subscriber' in badge['setID']:
-                    user_badges += '(S)'
-
-        except KeyError:
-            pass
-
-        # FORMAT: [TIME] (B1)(B2)NAME: MESSAGE
-        r_chat_log.append(f'[{comment_time}] {user_badges}{user_name}: {user_message}')
-
-    return r_chat_log
-
-
-def export_verbose_chat_log(chat_log, vod_directory):
-    """Exports a given chat log to disk.
-
-    :param chat_log: chat log retrieved from twitch to export
-    :param vod_directory: directory used to store chat log
-    """
-    Path(vod_directory).parent.mkdir(parents=True, exist_ok=True)
-
-    with open(Path(vod_directory, 'verbose_chat.json'), 'w+', encoding="utf-8") as chat_file:
-        chat_file.write(json.dumps(chat_log))
-
-
-def export_readable_chat_log(chat_log, vod_directory):
-    """Exports the provided readable chat log to disk.
-
-    :param chat_log: chat log retrieved from twitch to export
-    :param vod_directory: directory used to store chat log
-    """
-    if Path(vod_directory, 'readable_chat.log').is_file():
-        Path(vod_directory, 'readable_chat.log').unlink()
-
-    with open(Path(vod_directory, 'readable_chat.log'), 'a+', encoding="utf-8") as chat_file:
-        for message in chat_log:
-            chat_file.write(f'{message}\n')
-
-
-def export_json(vod_json):
-    """Exports all VOD information to a file.
-
-    :param vod_json: dict of vod parameters retrieved from twitch
-    """
-    with open(Path(vod_json['store_directory'], 'vod.json'), 'w', encoding='utf8') as json_out_file:
-        json_out_file.write(json.dumps(vod_json))
-
-
-def import_json(vod_json):
-    """Imports all VOD information from a file.
-
-    :param vod_json: dict of vod parameters retrieved from twitch
-    """
-    if Path(vod_json['store_directory'], 'vod.json').exists():
-        with open(Path(vod_json['store_directory'], 'vod.json'), 'r', encoding='utf8') as json_in_file:
-            return json.loads(json_in_file.read())
-
-    return []
-
-
-def combine_vod_parts(vod_json, print_progress=True):
-    """Combines the downloaded VOD .ts parts.
-
-    :param vod_json: dict of vod parameters retrieved from twitch
-    :param print_progress: boolean whether to print progress bar
-    """
-    log.info('Merging VOD parts. This may take a while.')
-
-    # get ordered list of vod parts
-    vod_parts = [Path(p) for p in sorted(glob(str(Path(vod_json['store_directory'], 'parts', '*.ts'))))]
-
-    progress = Progress()
-
-    # concat files if all pieces present, otherwise fall back to using ffmpeg
-    last_part = int(vod_parts[-1].name.strip('.ts'))
-    part_list = [int(i.name.strip('.ts')) for i in vod_parts]
-
-    dicontinuity = set([i for i in range(last_part + 1)]).difference(part_list)
-    if not dicontinuity:
-        # merge all .ts files by concatenating them
-        with open(str(Path(vod_json['store_directory'], 'merged.ts')), 'wb') as merged:
-            pr = 0
-            for ts_file in vod_parts:
-                pr += 1
-                # append part to merged file
-                with open(ts_file, 'rb') as mergefile:
-                    shutil.copyfileobj(mergefile, merged)
-
-                if print_progress:
-                    progress.print_progress(pr, len(vod_parts))
-
-    else:
-        # merge all .ts files with ffmpeg concat demuxer as missing segments can cause corruption with
-        # other method
-
-        log.debug('Discontinuity found, merging with ffmpeg.\n Discontinuity: %s', dicontinuity)
-
-        # create file with list of parts for ffmpeg
-        with open(Path(vod_json['store_directory'], 'parts', 'segments.txt'), 'w', encoding='utf8') as segment_file:
-            for part in vod_parts:
-                segment_file.write(f"file '{part}'\n")
-
-        with subprocess.Popen(f'ffmpeg -hide_banner -fflags +genpts -f concat -safe 0 -y -i '
-                              f'"{str(Path(vod_json["store_directory"], "parts", "segments.txt"))}"'
-                              f' -c copy "{str(Path(vod_json["store_directory"], "merged.ts"))}"',
-                              shell=True, stderr=subprocess.PIPE, universal_newlines=True) as p:
-            # get progress from ffmpeg output and print progress bar
-            for line in p.stderr:
-                if 'time=' in line:
-                    # extract current timestamp from output
-                    current_time = re.search('(?<=time=).*(?= bitrate=)', line).group(0).split(':')
-                    current_time = \
-                        int(current_time[0]) * 3600 + int(current_time[1]) * 60 + int(current_time[2][:2])
-
-                    if print_progress:
-                        progress.print_progress(int(current_time), vod_json['duration'])
-
-            if p.returncode:
-                log.error('VOD merger exited with error. Command: %s.', p.args)
-                raise VodConvertError(f'VOD merger exited with error. Command: {p.args}.')
-
-
-def convert_vod(vod_json, ignore_corruptions=None, print_progress=True):
-    """Converts the VOD from a .ts format to .mp4.
-
-    :param vod_json: dict of vod parameters retrieved from twitch
-    :param ignore_corruptions: list of tuples containing (min, max) of corrupt segments which will be ignored
-    :param print_progress: boolean whether to print progress bar
-    :raises vodConvertError: error encountered during conversion process
-    """
-    log.info('Converting VOD to mp4. This may take a while.')
-
-    progress = Progress()
-    corrupt_parts = set()
-    corrupt_part_whitelist = set()
-    if ignore_corruptions:
-        # create corrupt part whitelist form provided (min, max) ranges. The given range is expanded +-2 as the
-        # DTS timestamps can still be wonky past them
-        [corrupt_part_whitelist.update(r) for r in [range(t[0] - 2, t[1] + 3) for t in ignore_corruptions]]
-
-    # get dts offset of first part
-    with subprocess.Popen(f'ffprobe -v quiet -print_format json -show_format -show_streams '
-                          f'"{Path(vod_json["store_directory"], "parts", "00000.ts")}"', shell=True,
-                          stdout=subprocess.PIPE, universal_newlines=True) as p:
-        ts_file_data = ''
-        for line in p.stdout:
-            ts_file_data += line
-
-        dts_offset = float(json.loads(ts_file_data)['format']['start_time']) * 90000
-
-    # create ffmpeg command
-    ffmpeg_cmd = f'ffmpeg -hide_banner -y -i "{Path(vod_json["store_directory"], "merged.ts")}" '
-    # insert metadata if present
-    if Path(vod_json['store_directory'], 'parts', 'chapters.txt').exists():
-        ffmpeg_cmd += f'-i "{Path(vod_json["store_directory"], "parts", "chapters.txt")}" -map_metadata 1 '
-
-    ffmpeg_cmd += f'-c:a copy -c:v copy "{Path(vod_json["store_directory"], "vod.mp4")}"'
-
-    # convert merged .ts file to .mp4
-    with subprocess.Popen(ffmpeg_cmd, shell=True, stderr=subprocess.PIPE, universal_newlines=True) as p:
-        # get progress from ffmpeg output and catch corrupt segments
-        ffmpeg_log = ''
-        for line in p.stderr:
-            ffmpeg_log += line
-            if 'time=' in line:
-                # extract current timestamp from output
-                current_time = re.search(r'(?<=time=).*(?= bitrate=)', line).group(0).split(':')
-                current_time = int(current_time[0]) * 3600 + int(current_time[1]) * 60 + int(current_time[2][:2])
-
-                if print_progress:
-                    progress.print_progress(int(current_time), vod_json['duration'])
-
-            elif 'Packet corrupt' in line:
-                try:
-                    dts_timestamp = int(re.search(r'(?<=dts = ).*(?=\).)', line).group(0))
-
-                # Catch corrupt parts without timestamp, shows up as 'NOPTS'
-                except ValueError as e:
-                    raise VodConvertError("Corrupt packet encountered at unknown timestamp while converting VOD. "
-                                          "Delete 'parts' folder and re-download VOD.") from e
-
-                corrupt_part = floor((dts_timestamp - dts_offset) / 90000 / 10)
-
-                # ignore if corrupt packet within ignore_corruptions range
-                if corrupt_part in corrupt_part_whitelist:
-                    log.debug('Ignoring corrupt packet as part in whitelist. Part: %s', corrupt_part)
-
-                else:
-                    corrupt_parts.add(int(corrupt_part))
-                    log.error('Corrupt packet encountered. Part: %s', corrupt_part)
-
-    if p.returncode:
-        log.debug('FFmpeg exited with error code, output dumped to VOD directory.')
-        with open(Path(vod_json["store_directory"], 'parts', 'ffmpeg.log'), 'w', encoding='utf8') as ffout:
-            ffout.write(ffmpeg_log)
-
-        raise VodConvertError("VOD converter exited with error. Delete 'parts' directory and re-download VOD.")
-
-    if corrupt_parts:
-        corrupted_ranges = to_ranges(corrupt_parts)
-        formatted_ranges = []
-        for t in corrupted_ranges:
-            if t[0] == t[1]:
-                formatted_ranges.append(f'{t[0]}.ts')
-            else:
-                formatted_ranges.append(f'{t[0]}-{t[1]}.ts')
-
-        # raise error so we can try to recover
-        raise CorruptPartError(corrupt_parts, formatted_ranges)
-
-
-# https://stackoverflow.com/a/43091576
-def to_ranges(iterable):
-    """Converts a list of integers to iterable sets of (low, high) (e.g [0, 1, 2, 5, 7, 8] -> (0, 2), (5, 5), (7, 8))
-
-    :param iterable: list of integers
-    :return: iterable generator of separate integer ranges
-    """
-    iterable = sorted(set(iterable))
-    for key, group in groupby(enumerate(iterable), lambda t: t[1] - t[0]):
-        group = list(group)
-        yield group[0][1], group[-1][1]
-
-
-def verify_vod_length(vod_json):
-    """Verifies the length of a given VOD.
-
-    :param vod_json: dict of vod parameters retrieved from twitch
-    :return: true if verification fails, otherwise false
-    """
-    log.debug('Verifying length of VOD file.')
-
-    # skip verification if .ignorelength present
-    if Path(vod_json['store_directory'], '.ignorelength').is_file():
-        log.debug('.ignorelength file present - skipping verification.')
-        return False
-
-    # retrieve vod file duration
-    p = subprocess.run(f'ffprobe -v quiet -i "{Path(vod_json["store_directory"], "vod.mp4")}" '
-                       f'-show_entries format=duration -of default=noprint_wrappers=1:nokey=1',
-                       shell=True, capture_output=True)
-
-    if p.returncode:
-        log.error('VOD length verification exited with error. Command: %s.', p.args)
-        raise VodConvertError(f'VOD length verification exited with error. Command: {p.args}.')
-
-    try:
-        downloaded_length = int(float(p.stdout.decode('ascii').rstrip()))
-
-    except Exception as e:
-        log.error('Failed to fetch downloaded VOD length. VOD may not have downloaded correctly. %s', str(e))
-        raise VodConvertError(str(e)) from e
-
-    log.debug('Downloaded VOD length is %s. Expected length is %s.', downloaded_length, vod_json["duration"])
-
-    # pass verification if downloaded file is within 2s of expected length
-    if 2 >= downloaded_length - vod_json['duration'] >= -2:
-        log.debug('VOD passed length verification.')
-        return False
-
-    return True
-
-
-def cleanup_vod_parts(vod_directory):
-    """Deletes temporary and transitional files used for archiving VOD videos.
-
-    :param vod_directory: directory of downloaded vod which needs to be cleaned up
-    """
-    Path(vod_directory, 'merged.ts').unlink()
-    shutil.rmtree(Path(vod_directory, 'parts'))
-
-
-def sanitize_text(string):
-    """Sanitize a given string removing unwanted characters which aren't allowed in directories, file names.
-
-    :param string: string of characters to sanitize
-    :return: sanitized string
-    """
-    return re.sub('[^A-Za-z0-9.,_\-\(\) ]', '_', string)
-
-
-def sanitize_date(date):
-    """Removes unwanted characters from a timedate structure.
-
-    :param date: date retrieved from twitch to sanitize
-    :return: sanitized date
-    """
-    for r in (('T', '_'), (':', '-'), ('Z', '')):
-        date = date.replace(*r)
-
-    return date
-
-
-def convert_to_seconds(duration):
-    """Converts a given time in the format HHhMMmSSs to seconds.
-
-    :param duration: time in HHhMMmSSs format to be converted
-    :return: time in seconds
-    """
-    duration = duration.replace('h', ':').replace('m', ':').replace('s', '').split(':')
-
-    if len(duration) == 1:
-        return int(duration[0])
-
-    if len(duration) == 2:
-        return (int(duration[0]) * 60) + int(duration[1])
-
-    if len(duration) == 3:
-        return (int(duration[0]) * 3600) + (int(duration[1]) * 60) + int(duration[2])
-
-
-def convert_to_hms(seconds):
-    """Converts a given time in seconds to the format HHhMMmSSs.
-
-    :param seconds: time in seconds
-    :return: time in HHhMMmSSs format
-    """
-    minutes = seconds // 60
-    hours = minutes // 60
-
-    return f"{hours:02d}h{minutes % 60:02d}m{seconds % 60:02d}s"
-
-
-def create_lock(ini_path, vod_id):
-    """Creates a lock file for a given VOD.
-
-    :param ini_path: path to config directory
-    :param vod_id: id of vod which lock file is created for
-    :return: true if lock file creation fails
-    """
-    try:
-        with open(Path(ini_path, f'.lock.{vod_id}'), 'x', encoding='utf8') as _:
-            pass
-        return
-
-    except FileExistsError:
-        return True
-
-
-def remove_lock(config_dir, vod_id):
-    """Removes a given lock file.
-
-    :param config_dir: path to config directory
-    :param vod_id: id of vod which lock file is created for
-    :return: error if lock file removal fails
-    """
-    try:
-        Path(config_dir, f'.lock.{vod_id}').unlink()
-        return
-
-    except Exception as e:
-        return e
-
-
-def time_since_date(timestamp):
-    """Returns the time in seconds between a given datetime and now.
-
-    :param timestamp: utc timestamp to compare current datetime to
-    :return: the time in seconds since the given date
-    """
-    created_at = int(timestamp)
-    current_time = int(datetime.now(timezone.utc).timestamp())
-
-    return current_time - created_at
-
-
-def get_time_difference(start_time, end_time):
-    """Returns the time in seconds between a given datetime and now.
-
-    :param start_time: start utc timestamp
-    :param end_time: end utc timestamp
-    :return: the time in seconds:milliseconds between the two datetimes
-    """
-
-    return (end_time - start_time).total_seconds()
-
-
-def get_latest_version():
-    """Fetches the latest release information from GitHub.
-
-    :return: latest version number
-    :return: latest release notes
-    """
-    try:
-        _r = requests.get('https://api.github.com/repos/Brisppy/twitch-vod-archiver/releases/latest', timeout=10)
-        # catch error codes such as 403 in case of rate limiting
-        if _r.status_code != 200:
-            return '0.0.0', ''
-        latest_version = _r.json()['tag_name'].replace('v', '')
-        release_notes = _r.json()['body']
-
-    # return a dummy value if request fails
-    except Exception:
-        return '0.0.0', ''
-
-    return latest_version, release_notes
-
-
-# reference:
-#   https://stackoverflow.com/a/11887825
-def version_tuple(v):
-    """Convert
-
-    :param v:
-    :return:
-    """
-    return tuple(map(int, (v.split("."))))
-
-
-def check_update_available(local_version, remote_version):
-    """Compares two software versions.
-
-    :param local_version: local version in use
-    :param remote_version: remote version to compare against
-    :return: True if remote version has a higher version number, otherwise False
-    """
-    # check if local version is 'special', as in a development build or release candidate
-    local_version_parts = local_version.split('.')
-    if len(local_version_parts) > 3:
-        log.warning(
-            'Currently using a development or release candidate build. These may be unfinished or contain serious '
-            'bugs. Report any issues you encounter to https://github.com/Brisppy/twitch-archiver/issues.')
-        # update is available if we are using a dev or release candidate build equal to or prior to
-        # the latest stable release
-        if version_tuple('.'.join(local_version_parts[:-1])) <= version_tuple(remote_version):
-            return True
-
-    elif version_tuple(local_version) < version_tuple(remote_version):
-        return True
-
-    return False
-
-
-def get_quality_index(desired_quality, available_qualities):
-    """Finds the index of a user defined quality from a list of available stream qualities.
-
-    :param desired_quality: desired quality to search for - best, worst or [resolution, framerate]
-    :param available_qualities: list of available qualities as [[resolution, framerate], ...]
-    :return: list index of desired quality if found
-    """
-    if desired_quality not in ['best', 'worst']:
-        # look for user defined quality in available streams
-        try:
-            return available_qualities.index(desired_quality)
-
-        except ValueError:
-            log.info('User requested quality not found in available streams.')
-            # grab first resolution match
-            try:
-                return [quality[0] for quality in available_qualities].index(desired_quality[0])
-
-            except ValueError:
-                log.info('No match found for user requested resolution. Defaulting to best.')
-                return 0
-
-    elif desired_quality == 'worst':
-        return -1
-
-    else:
-        return 0
-
-
-def send_push(pushbullet_key, title, body=''):
-    """Sends a push to an account based on a given pushbullet key.
-
-    :param pushbullet_key: key for destination pushbullet account. 'False' to not send.
-    :param title: title to send with push
-    :param body: body to send with push
-    """
-    if pushbullet_key:
-        h = {'content-type': 'application/json', 'Authorization': f'Bearer {pushbullet_key}'}
-        d = {'type': 'note', 'title': f'[twitch-archiver] {title}', 'body': body}
-
-        try:
-            _r = requests.post(url="https://api.pushbullet.com/v2/pushes", headers=h, data=json.dumps(d),
-                               timeout=10)
-
-            if _r.status_code != 200:
-                if _r.json()['error']['code'] == 'pushbullet_pro_required':
-                    log.error('Error sending push. Likely rate limited (500/month). '
-                              'Error %s: %s', _r.status_code, _r.text)
-
-                else:
-                    log.error('Error sending push. Error %s: %s', _r.status_code, _r.text)
-
-        except Exception as e:
-            log.error('Error sending push. Error: %s', e)
-
-
-# reference:
-#   https://www.geeksforgeeks.org/compare-two-files-using-hashing-in-python/
-def get_hash(file):
-    """Retrieves the hash for a given file.
-
-    :param file: path to file to hash
-    :return: hash of provided file
-    """
-    f_hash = hashlib.md5()
-
-    with open(Path(file), 'rb') as f:
-        while True:
-            # read in next chunk
-            _d = f.read(65536)
-
-            if not _d:
-                break
-
-            f_hash.update(_d)
-
-        return f_hash.hexdigest()
-
-
-# reference:
-#   https://alexwlchan.net/2019/03/atomic-cross-filesystem-moves-in-python/
-def safe_move(src_file, dst_file):
-    """Atomically moves src_file to dst_file
-
-    :param src_file: source file to copy
-    :param dst_file: path to copy file to
-    :raises FileNotFoundError: if src_file does not exist
-    """
-    log.debug('Moving "%s" to "%s".', src_file, dst_file)
-
-    if Path(src_file).exists():
-        # remove source file if it matches destination file
-        if os.path.exists(dst_file) and os.path.samefile(src_file, dst_file):
-            log.debug('%s already exists and matches %s.', dst_file, src_file)
-            os.remove(src_file)
-        else:
-            # generate temp file path and copy source file to it
-            tmp_file = Path(Path(dst_file.parent), os.urandom(6).hex())
-            shutil.copyfile(src_file, tmp_file)
-
-            # rename temp file
-            os.rename(tmp_file, dst_file)
-
-            # delete source file
-            os.remove(src_file)
-
-    else:
-        raise FileNotFoundError
-
-
-def getenv(name, default_val=None, is_bool=False):
-    """
-    Wrapper around os.getenv to convert empty strings to None type
-
-    :param name: environment variable name
-    :param default_val: default value to return if environment variable does not exist
-    :param is_bool: handle environment variable as a case-insensitive boolean string ('true' or 'false')
-    :return: environment variable value
-    """
-    val = os.getenv(name, default_val)
-
-    if is_bool and isinstance(val, str):
-        if val.upper() == "TRUE":
-            return True
-
-        if val.upper() == "FALSE":
-            return False
-
-        raise ValueError(f"Invalid boolean value (true or false) received for environment variable: {name}={val}")
-
-    # return empty strings '' as None type
-    return val if val else None
-
-
-def format_vod_chapters(chapters):
-    """Formats vod chapters retrieved from Twitch into an FFmpeg insertable format
-
-    :param chapters: either a list of vod chapters or tuple containing (chapter_name, start, end)
-    :return: chapters formatted as a string readable by ffmpeg
-    """
-    formatted_chapters = ";FFMETADATA1\n"
-    chapter_base = dedent("""\
-    [CHAPTER]
-    TIMEBASE=1/1000
-    START={start}
-    END={end}
-    title={title}
-    
-    """)
-
-    if isinstance(chapters, tuple):
-        formatted_chapters += chapter_base.format(
-            start=chapters[1],
-            end=chapters[2],
-            title=chapters[0])
-
-    else:
-        # some chapters have no game attached and so the 'description' is used instead
-        for chapter in chapters:
-            formatted_chapters += chapter_base.format(
-                start=chapter['positionMilliseconds'],
-                end=chapter['positionMilliseconds'] + chapter['durationMilliseconds'],
-                title=chapter['description'])
-
-    return formatted_chapters
-
-
-class Progress:
-    """
-    Functions for displaying progress.
-    """
-    start_time = 0
-
-    def __init__(self):
-        """
-        Sets the start time used for computing the time remaining.
-        """
-        if self.start_time == 0:
-            self.start_time = int(datetime.utcnow().timestamp())
-
-    # reference:
-    #   https://stackoverflow.com/questions/63865536/how-to-convert-seconds-to-hhmmss-format-without-failing-if-hour-more-than-24
-    @staticmethod
-    def to_hms(s):
-        """Converts a given time in seconds to HHhMMmSSs.
-
-        :param s: time in seconds
-        :return: time formatted as HHhMMmSSs
-        """
-        m, s = divmod(s, 60)
-        h, m = divmod(m, 60)
-        return f'{h:0>2}:{m:0>2}:{s:0>2}'
-
-    def print_progress(self, cur, total, last_frame=False):
-        """Prints and updates a nice progress bar.
-
-        :param cur: current progress out of total
-        :param total: highest value of progress bar
-        :param last_frame: boolean if last frame of progress bar
-        """
-        percent = floor(100 * (cur / total))
-        progress = floor((0.25 * percent)) * '#' + ceil(25 - (0.25 * percent)) * ' '
-        if cur == 0 or self.start_time == 0:
-            remaining_time = '?'
-
-        else:
-            remaining_time = self.to_hms(
-                ceil(((int(datetime.utcnow().timestamp()) - self.start_time) / cur) * (total - cur)))
-
-        if len(str(percent)) < 3:
-            percent = ' ' * (3 - len(str(percent))) + str(percent)
-
-        if len(str(cur)) < len(str(total)):
-            cur = ' ' * (len(str(total)) - len(str(cur))) + str(cur)
-
-        # end with newline rather than return
-        if last_frame:
-            print(f'  100%  -  [#########################]  -  {cur} / {total}  -  ETA: 00:00:00', end='\n')
-
-        else:
-            print(f'  {percent}%  -  [{progress}]  -  {cur} / {total}  -  ETA: {remaining_time}', end='\r')
+"""
+Various utility functions for modifying, retrieving and saving information.
+"""
+
+import hashlib
+import json
+import logging
+import os
+import re
+import shutil
+import subprocess
+
+from datetime import datetime, timezone
+from glob import glob
+from itertools import groupby
+from math import ceil, floor
+from pathlib import Path
+from textwrap import dedent
+
+import requests
+
+from twitcharchiver.exceptions import VodConvertError, CorruptPartError
+
+log = logging.getLogger()
+
+
+def generate_readable_chat_log(chat_log, stream_start):
+    """Converts the raw chat log into a scrollable, readable format.
+
+    :param chat_log: list of chat messages retrieved from twitch which are to be converted
+    :param stream_start: stream start utc timestamp
+    :return: formatted chat log
+    """
+    r_chat_log = []
+    for comment in chat_log:
+        # format comments with / without millisecond timestamp
+        if '.' in comment['createdAt']:
+            created_time = \
+                datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%S.%fZ').replace(tzinfo=timezone.utc)
+        else:
+            created_time = \
+                datetime.strptime(comment['createdAt'], '%Y-%m-%dT%H:%M:%SZ').replace(tzinfo=timezone.utc)
+
+        comment_time = f'{get_time_difference(stream_start, created_time):.3f}'
+
+        # catch comments without commenter informations
+        if comment['commenter']:
+            user_name = str(comment['commenter']['displayName'])
+        else:
+            user_name = '~MISSING_COMMENTER_INFO~'
+
+        # catch comments without data
+        if comment['message']['fragments']:
+            user_message = str(comment['message']['fragments'][0]['text'])
+        else:
+            user_message = '~MISSING_MESSAGE_INFO~'
+
+        user_badges = ''
+        try:
+            for badge in comment['message']['userBadges']:
+                if 'broadcaster' in badge['setID']:
+                    user_badges += '(B)'
+
+                if 'moderator' in badge['setID']:
+                    user_badges += '(M)'
+
+                if 'subscriber' in badge['setID']:
+                    user_badges += '(S)'
+
+        except KeyError:
+            pass
+
+        # FORMAT: [TIME] (B1)(B2)NAME: MESSAGE
+        r_chat_log.append(f'[{comment_time}] {user_badges}{user_name}: {user_message}')
+
+    return r_chat_log
+
+
+def export_verbose_chat_log(chat_log, vod_directory):
+    """Exports a given chat log to disk.
+
+    :param chat_log: chat log retrieved from twitch to export
+    :param vod_directory: directory used to store chat log
+    """
+    Path(vod_directory).parent.mkdir(parents=True, exist_ok=True)
+
+    with open(Path(vod_directory, 'verbose_chat.json'), 'w+', encoding="utf-8") as chat_file:
+        chat_file.write(json.dumps(chat_log))
+
+
+def export_readable_chat_log(chat_log, vod_directory):
+    """Exports the provided readable chat log to disk.
+
+    :param chat_log: chat log retrieved from twitch to export
+    :param vod_directory: directory used to store chat log
+    """
+    if Path(vod_directory, 'readable_chat.log').is_file():
+        Path(vod_directory, 'readable_chat.log').unlink()
+
+    with open(Path(vod_directory, 'readable_chat.log'), 'a+', encoding="utf-8") as chat_file:
+        for message in chat_log:
+            chat_file.write(f'{message}\n')
+
+
+def export_json(vod_json):
+    """Exports all VOD information to a file.
+
+    :param vod_json: dict of vod parameters retrieved from twitch
+    """
+    with open(Path(vod_json['store_directory'], 'vod.json'), 'w', encoding='utf8') as json_out_file:
+        json_out_file.write(json.dumps(vod_json))
+
+
+def import_json(vod_json):
+    """Imports all VOD information from a file.
+
+    :param vod_json: dict of vod parameters retrieved from twitch
+    """
+    if Path(vod_json['store_directory'], 'vod.json').exists():
+        with open(Path(vod_json['store_directory'], 'vod.json'), 'r', encoding='utf8') as json_in_file:
+            return json.loads(json_in_file.read())
+
+    return []
+
+
+def combine_vod_parts(vod_json, print_progress=True):
+    """Combines the downloaded VOD .ts parts.
+
+    :param vod_json: dict of vod parameters retrieved from twitch
+    :param print_progress: boolean whether to print progress bar
+    """
+    log.info('Merging VOD parts. This may take a while.')
+
+    # get ordered list of vod parts
+    vod_parts = [Path(p) for p in sorted(glob(str(Path(vod_json['store_directory'], 'parts', '*.ts'))))]
+
+    progress = Progress()
+
+    # concat files if all pieces present, otherwise fall back to using ffmpeg
+    last_part = int(vod_parts[-1].name.strip('.ts'))
+    part_list = [int(i.name.strip('.ts')) for i in vod_parts]
+
+    dicontinuity = set([i for i in range(last_part + 1)]).difference(part_list)
+    if not dicontinuity:
+        # merge all .ts files by concatenating them
+        with open(str(Path(vod_json['store_directory'], 'merged.ts')), 'wb') as merged:
+            pr = 0
+            for ts_file in vod_parts:
+                pr += 1
+                # append part to merged file
+                with open(ts_file, 'rb') as mergefile:
+                    shutil.copyfileobj(mergefile, merged)
+
+                if print_progress:
+                    progress.print_progress(pr, len(vod_parts))
+
+    else:
+        # merge all .ts files with ffmpeg concat demuxer as missing segments can cause corruption with
+        # other method
+
+        log.debug('Discontinuity found, merging with ffmpeg.\n Discontinuity: %s', dicontinuity)
+
+        # create file with list of parts for ffmpeg
+        with open(Path(vod_json['store_directory'], 'parts', 'segments.txt'), 'w', encoding='utf8') as segment_file:
+            for part in vod_parts:
+                segment_file.write(f"file '{part}'\n")
+
+        with subprocess.Popen(f'ffmpeg -hide_banner -fflags +genpts -f concat -safe 0 -y -i '
+                              f'"{str(Path(vod_json["store_directory"], "parts", "segments.txt"))}"'
+                              f' -c copy "{str(Path(vod_json["store_directory"], "merged.ts"))}"',
+                              shell=True, stderr=subprocess.PIPE, universal_newlines=True) as p:
+            # get progress from ffmpeg output and print progress bar
+            for line in p.stderr:
+                if 'time=' in line:
+                    # extract current timestamp from output
+                    current_time = re.search('(?<=time=).*(?= bitrate=)', line).group(0).split(':')
+                    current_time = \
+                        int(current_time[0]) * 3600 + int(current_time[1]) * 60 + int(current_time[2][:2])
+
+                    if print_progress:
+                        progress.print_progress(int(current_time), vod_json['duration'])
+
+            if p.returncode:
+                log.error('VOD merger exited with error. Command: %s.', p.args)
+                raise VodConvertError(f'VOD merger exited with error. Command: {p.args}.')
+
+
+def convert_vod(vod_json, ignore_corruptions=None, print_progress=True):
+    """Converts the VOD from a .ts format to .mp4.
+
+    :param vod_json: dict of vod parameters retrieved from twitch
+    :param ignore_corruptions: list of tuples containing (min, max) of corrupt segments which will be ignored
+    :param print_progress: boolean whether to print progress bar
+    :raises vodConvertError: error encountered during conversion process
+    """
+    log.info('Converting VOD to mp4. This may take a while.')
+
+    progress = Progress()
+    corrupt_parts = set()
+    corrupt_part_whitelist = set()
+    if ignore_corruptions:
+        # create corrupt part whitelist form provided (min, max) ranges. The given range is expanded +-2 as the
+        # DTS timestamps can still be wonky past them
+        [corrupt_part_whitelist.update(r) for r in [range(t[0] - 2, t[1] + 3) for t in ignore_corruptions]]
+
+    # get dts offset of first part
+    with subprocess.Popen(f'ffprobe -v quiet -print_format json -show_format -show_streams '
+                          f'"{Path(vod_json["store_directory"], "parts", "00000.ts")}"', shell=True,
+                          stdout=subprocess.PIPE, universal_newlines=True) as p:
+        ts_file_data = ''
+        for line in p.stdout:
+            ts_file_data += line
+
+        dts_offset = float(json.loads(ts_file_data)['format']['start_time']) * 90000
+
+    # create ffmpeg command
+    ffmpeg_cmd = f'ffmpeg -hide_banner -y -i "{Path(vod_json["store_directory"], "merged.ts")}" '
+    # insert metadata if present
+    if Path(vod_json['store_directory'], 'parts', 'chapters.txt').exists():
+        ffmpeg_cmd += f'-i "{Path(vod_json["store_directory"], "parts", "chapters.txt")}" -map_metadata 1 '
+
+    ffmpeg_cmd += f'-c:a copy -c:v copy "{Path(vod_json["store_directory"], "vod.mp4")}"'
+
+    # convert merged .ts file to .mp4
+    with subprocess.Popen(ffmpeg_cmd, shell=True, stderr=subprocess.PIPE, universal_newlines=True) as p:
+        # get progress from ffmpeg output and catch corrupt segments
+        ffmpeg_log = ''
+        for line in p.stderr:
+            ffmpeg_log += line
+            if 'time=' in line:
+                # extract current timestamp from output
+                current_time = re.search(r'(?<=time=).*(?= bitrate=)', line).group(0).split(':')
+                current_time = int(current_time[0]) * 3600 + int(current_time[1]) * 60 + int(current_time[2][:2])
+
+                if print_progress:
+                    progress.print_progress(int(current_time), vod_json['duration'])
+
+            elif 'Packet corrupt' in line:
+                try:
+                    dts_timestamp = int(re.search(r'(?<=dts = ).*(?=\).)', line).group(0))
+
+                # Catch corrupt parts without timestamp, shows up as 'NOPTS'
+                except ValueError as e:
+                    raise VodConvertError("Corrupt packet encountered at unknown timestamp while converting VOD. "
+                                          "Delete 'parts' folder and re-download VOD.") from e
+
+                corrupt_part = floor((dts_timestamp - dts_offset) / 90000 / 10)
+
+                # ignore if corrupt packet within ignore_corruptions range
+                if corrupt_part in corrupt_part_whitelist:
+                    log.debug('Ignoring corrupt packet as part in whitelist. Part: %s', corrupt_part)
+
+                else:
+                    corrupt_parts.add(int(corrupt_part))
+                    log.error('Corrupt packet encountered. Part: %s', corrupt_part)
+
+    if p.returncode:
+        log.debug('FFmpeg exited with error code, output dumped to VOD directory.')
+        with open(Path(vod_json["store_directory"], 'parts', 'ffmpeg.log'), 'w', encoding='utf8') as ffout:
+            ffout.write(ffmpeg_log)
+
+        raise VodConvertError("VOD converter exited with error. Delete 'parts' directory and re-download VOD.")
+
+    if corrupt_parts:
+        corrupted_ranges = to_ranges(corrupt_parts)
+        formatted_ranges = []
+        for t in corrupted_ranges:
+            if t[0] == t[1]:
+                formatted_ranges.append(f'{t[0]}.ts')
+            else:
+                formatted_ranges.append(f'{t[0]}-{t[1]}.ts')
+
+        # raise error so we can try to recover
+        raise CorruptPartError(corrupt_parts, formatted_ranges)
+
+
+# https://stackoverflow.com/a/43091576
+def to_ranges(iterable):
+    """Converts a list of integers to iterable sets of (low, high) (e.g [0, 1, 2, 5, 7, 8] -> (0, 2), (5, 5), (7, 8))
+
+    :param iterable: list of integers
+    :return: iterable generator of separate integer ranges
+    """
+    iterable = sorted(set(iterable))
+    for key, group in groupby(enumerate(iterable), lambda t: t[1] - t[0]):
+        group = list(group)
+        yield group[0][1], group[-1][1]
+
+
+def verify_vod_length(vod_json):
+    """Verifies the length of a given VOD.
+
+    :param vod_json: dict of vod parameters retrieved from twitch
+    :return: true if verification fails, otherwise false
+    """
+    log.debug('Verifying length of VOD file.')
+
+    # skip verification if .ignorelength present
+    if Path(vod_json['store_directory'], '.ignorelength').is_file():
+        log.debug('.ignorelength file present - skipping verification.')
+        return False
+
+    # retrieve vod file duration
+    p = subprocess.run(f'ffprobe -v quiet -i "{Path(vod_json["store_directory"], "vod.mp4")}" '
+                       f'-show_entries format=duration -of default=noprint_wrappers=1:nokey=1',
+                       shell=True, capture_output=True)
+
+    if p.returncode:
+        log.error('VOD length verification exited with error. Command: %s.', p.args)
+        raise VodConvertError(f'VOD length verification exited with error. Command: {p.args}.')
+
+    try:
+        downloaded_length = int(float(p.stdout.decode('ascii').rstrip()))
+
+    except Exception as e:
+        log.error('Failed to fetch downloaded VOD length. VOD may not have downloaded correctly. %s', str(e))
+        raise VodConvertError(str(e)) from e
+
+    log.debug('Downloaded VOD length is %s. Expected length is %s.', downloaded_length, vod_json["duration"])
+
+    # pass verification if downloaded file is within 2s of expected length
+    if 2 >= downloaded_length - vod_json['duration'] >= -2:
+        log.debug('VOD passed length verification.')
+        return False
+
+    return True
+
+
+def cleanup_vod_parts(vod_directory):
+    """Deletes temporary and transitional files used for archiving VOD videos.
+
+    :param vod_directory: directory of downloaded vod which needs to be cleaned up
+    """
+    Path(vod_directory, 'merged.ts').unlink()
+    shutil.rmtree(Path(vod_directory, 'parts'))
+
+
+def sanitize_text(string):
+    """Sanitize a given string removing unwanted characters which aren't allowed in directories, file names.
+
+    :param string: string of characters to sanitize
+    :return: sanitized string
+    """
+    return re.sub('[^A-Za-z0-9.,_\-\(\) ]', '_', string)
+
+
+def sanitize_date(date):
+    """Removes unwanted characters from a timedate structure.
+
+    :param date: date retrieved from twitch to sanitize
+    :return: sanitized date
+    """
+    for r in (('T', '_'), (':', '-'), ('Z', '')):
+        date = date.replace(*r)
+
+    return date
+
+
+def convert_to_seconds(duration):
+    """Converts a given time in the format HHhMMmSSs to seconds.
+
+    :param duration: time in HHhMMmSSs format to be converted
+    :return: time in seconds
+    """
+    duration = duration.replace('h', ':').replace('m', ':').replace('s', '').split(':')
+
+    if len(duration) == 1:
+        return int(duration[0])
+
+    if len(duration) == 2:
+        return (int(duration[0]) * 60) + int(duration[1])
+
+    if len(duration) == 3:
+        return (int(duration[0]) * 3600) + (int(duration[1]) * 60) + int(duration[2])
+
+
+def convert_to_hms(seconds):
+    """Converts a given time in seconds to the format HHhMMmSSs.
+
+    :param seconds: time in seconds
+    :return: time in HHhMMmSSs format
+    """
+    minutes = seconds // 60
+    hours = minutes // 60
+
+    return f"{hours:02d}h{minutes % 60:02d}m{seconds % 60:02d}s"
+
+
+def create_lock(ini_path, vod_id):
+    """Creates a lock file for a given VOD.
+
+    :param ini_path: path to config directory
+    :param vod_id: id of vod which lock file is created for
+    :return: true if lock file creation fails
+    """
+    try:
+        with open(Path(ini_path, f'.lock.{vod_id}'), 'x', encoding='utf8') as _:
+            pass
+        return
+
+    except FileExistsError:
+        return True
+
+
+def remove_lock(config_dir, vod_id):
+    """Removes a given lock file.
+
+    :param config_dir: path to config directory
+    :param vod_id: id of vod which lock file is created for
+    :return: error if lock file removal fails
+    """
+    try:
+        Path(config_dir, f'.lock.{vod_id}').unlink()
+        return
+
+    except Exception as e:
+        return e
+
+
+def time_since_date(timestamp):
+    """Returns the time in seconds between a given datetime and now.
+
+    :param timestamp: utc timestamp to compare current datetime to
+    :return: the time in seconds since the given date
+    """
+    created_at = int(timestamp)
+    current_time = int(datetime.now(timezone.utc).timestamp())
+
+    return current_time - created_at
+
+
+def get_time_difference(start_time, end_time):
+    """Returns the time in seconds between a given datetime and now.
+
+    :param start_time: start utc timestamp
+    :param end_time: end utc timestamp
+    :return: the time in seconds:milliseconds between the two datetimes
+    """
+
+    return (end_time - start_time).total_seconds()
+
+
+def get_latest_version():
+    """Fetches the latest release information from GitHub.
+
+    :return: latest version number
+    :return: latest release notes
+    """
+    try:
+        _r = requests.get('https://api.github.com/repos/Brisppy/twitch-vod-archiver/releases/latest', timeout=10)
+        # catch error codes such as 403 in case of rate limiting
+        if _r.status_code != 200:
+            return '0.0.0', ''
+        latest_version = _r.json()['tag_name'].replace('v', '')
+        release_notes = _r.json()['body']
+
+    # return a dummy value if request fails
+    except Exception:
+        return '0.0.0', ''
+
+    return latest_version, release_notes
+
+
+# reference:
+#   https://stackoverflow.com/a/11887825
+def version_tuple(v):
+    """Convert
+
+    :param v:
+    :return:
+    """
+    return tuple(map(int, (v.split("."))))
+
+
+def check_update_available(local_version, remote_version):
+    """Compares two software versions.
+
+    :param local_version: local version in use
+    :param remote_version: remote version to compare against
+    :return: True if remote version has a higher version number, otherwise False
+    """
+    # check if local version is 'special', as in a development build or release candidate
+    local_version_parts = local_version.split('.')
+    if len(local_version_parts) > 3:
+        log.warning(
+            'Currently using a development or release candidate build. These may be unfinished or contain serious '
+            'bugs. Report any issues you encounter to https://github.com/Brisppy/twitch-archiver/issues.')
+        # update is available if we are using a dev or release candidate build equal to or prior to
+        # the latest stable release
+        if version_tuple('.'.join(local_version_parts[:-1])) <= version_tuple(remote_version):
+            return True
+
+    elif version_tuple(local_version) < version_tuple(remote_version):
+        return True
+
+    return False
+
+
+def get_quality_index(desired_quality, available_qualities):
+    """Finds the index of a user defined quality from a list of available stream qualities.
+
+    :param desired_quality: desired quality to search for - best, worst or [resolution, framerate]
+    :param available_qualities: list of available qualities as [[resolution, framerate], ...]
+    :return: list index of desired quality if found
+    """
+    if desired_quality not in ['best', 'worst']:
+        # look for user defined quality in available streams
+        try:
+            return available_qualities.index(desired_quality)
+
+        except ValueError:
+            log.info('User requested quality not found in available streams.')
+            # grab first resolution match
+            try:
+                return [quality[0] for quality in available_qualities].index(desired_quality[0])
+
+            except ValueError:
+                log.info('No match found for user requested resolution. Defaulting to best.')
+                return 0
+
+    elif desired_quality == 'worst':
+        return -1
+
+    else:
+        return 0
+
+
+def send_push(pushbullet_key, title, body=''):
+    """Sends a push to an account based on a given pushbullet key.
+
+    :param pushbullet_key: key for destination pushbullet account. 'False' to not send.
+    :param title: title to send with push
+    :param body: body to send with push
+    """
+    if pushbullet_key:
+        h = {'content-type': 'application/json', 'Authorization': f'Bearer {pushbullet_key}'}
+        d = {'type': 'note', 'title': f'[twitch-archiver] {title}', 'body': body}
+
+        try:
+            _r = requests.post(url="https://api.pushbullet.com/v2/pushes", headers=h, data=json.dumps(d),
+                               timeout=10)
+
+            if _r.status_code != 200:
+                if _r.json()['error']['code'] == 'pushbullet_pro_required':
+                    log.error('Error sending push. Likely rate limited (500/month). '
+                              'Error %s: %s', _r.status_code, _r.text)
+
+                else:
+                    log.error('Error sending push. Error %s: %s', _r.status_code, _r.text)
+
+        except Exception as e:
+            log.error('Error sending push. Error: %s', e)
+
+
+# reference:
+#   https://www.geeksforgeeks.org/compare-two-files-using-hashing-in-python/
+def get_hash(file):
+    """Retrieves the hash for a given file.
+
+    :param file: path to file to hash
+    :return: hash of provided file
+    """
+    f_hash = hashlib.md5()
+
+    with open(Path(file), 'rb') as f:
+        while True:
+            # read in next chunk
+            _d = f.read(65536)
+
+            if not _d:
+                break
+
+            f_hash.update(_d)
+
+        return f_hash.hexdigest()
+
+
+# reference:
+#   https://alexwlchan.net/2019/03/atomic-cross-filesystem-moves-in-python/
+def safe_move(src_file, dst_file):
+    """Atomically moves src_file to dst_file
+
+    :param src_file: source file to copy
+    :param dst_file: path to copy file to
+    :raises FileNotFoundError: if src_file does not exist
+    """
+    log.debug('Moving "%s" to "%s".', src_file, dst_file)
+
+    if Path(src_file).exists():
+        # remove source file if it matches destination file
+        if os.path.exists(dst_file) and os.path.samefile(src_file, dst_file):
+            log.debug('%s already exists and matches %s.', dst_file, src_file)
+            os.remove(src_file)
+        else:
+            # generate temp file path and copy source file to it
+            tmp_file = Path(Path(dst_file.parent), os.urandom(6).hex())
+            shutil.copyfile(src_file, tmp_file)
+
+            # rename temp file
+            os.rename(tmp_file, dst_file)
+
+            # delete source file
+            os.remove(src_file)
+
+    else:
+        raise FileNotFoundError
+
+
+def getenv(name, default_val=None, is_bool=False):
+    """
+    Wrapper around os.getenv to convert empty strings to None type
+
+    :param name: environment variable name
+    :param default_val: default value to return if environment variable does not exist
+    :param is_bool: handle environment variable as a case-insensitive boolean string ('true' or 'false')
+    :return: environment variable value
+    """
+    val = os.getenv(name, default_val)
+
+    if is_bool and isinstance(val, str):
+        if val.upper() == "TRUE":
+            return True
+
+        if val.upper() == "FALSE":
+            return False
+
+        raise ValueError(f"Invalid boolean value (true or false) received for environment variable: {name}={val}")
+
+    # return empty strings '' as None type
+    return val if val else None
+
+
+def format_vod_chapters(chapters):
+    """Formats vod chapters retrieved from Twitch into an FFmpeg insertable format
+
+    :param chapters: either a list of vod chapters or tuple containing (chapter_name, start, end)
+    :return: chapters formatted as a string readable by ffmpeg
+    """
+    formatted_chapters = ";FFMETADATA1\n"
+    chapter_base = dedent("""\
+    [CHAPTER]
+    TIMEBASE=1/1000
+    START={start}
+    END={end}
+    title={title}
+    
+    """)
+
+    if isinstance(chapters, tuple):
+        formatted_chapters += chapter_base.format(
+            start=chapters[1],
+            end=chapters[2],
+            title=chapters[0])
+
+    else:
+        # some chapters have no game attached and so the 'description' is used instead
+        for chapter in chapters:
+            formatted_chapters += chapter_base.format(
+                start=chapter['positionMilliseconds'],
+                end=chapter['positionMilliseconds'] + chapter['durationMilliseconds'],
+                title=chapter['description'])
+
+    return formatted_chapters
+
+
+class Progress:
+    """
+    Functions for displaying progress.
+    """
+    start_time = 0
+
+    def __init__(self):
+        """
+        Sets the start time used for computing the time remaining.
+        """
+        if self.start_time == 0:
+            self.start_time = int(datetime.utcnow().timestamp())
+
+    # reference:
+    #   https://stackoverflow.com/questions/63865536/how-to-convert-seconds-to-hhmmss-format-without-failing-if-hour-more-than-24
+    @staticmethod
+    def to_hms(s):
+        """Converts a given time in seconds to HHhMMmSSs.
+
+        :param s: time in seconds
+        :return: time formatted as HHhMMmSSs
+        """
+        m, s = divmod(s, 60)
+        h, m = divmod(m, 60)
+        return f'{h:0>2}:{m:0>2}:{s:0>2}'
+
+    def print_progress(self, cur, total, last_frame=False):
+        """Prints and updates a nice progress bar.
+
+        :param cur: current progress out of total
+        :param total: highest value of progress bar
+        :param last_frame: boolean if last frame of progress bar
+        """
+        percent = floor(100 * (cur / total))
+        progress = floor((0.25 * percent)) * '#' + ceil(25 - (0.25 * percent)) * ' '
+        if cur == 0 or self.start_time == 0:
+            remaining_time = '?'
+
+        else:
+            remaining_time = self.to_hms(
+                ceil(((int(datetime.utcnow().timestamp()) - self.start_time) / cur) * (total - cur)))
+
+        if len(str(percent)) < 3:
+            percent = ' ' * (3 - len(str(percent))) + str(percent)
+
+        if len(str(cur)) < len(str(total)):
+            cur = ' ' * (len(str(total)) - len(str(cur))) + str(cur)
+
+        # end with newline rather than return
+        if last_frame:
+            print(f'  100%  -  [#########################]  -  {cur} / {total}  -  ETA: 00:00:00', end='\n')
+
+        else:
+            print(f'  {percent}%  -  [{progress}]  -  {cur} / {total}  -  ETA: {remaining_time}', end='\r')
```

