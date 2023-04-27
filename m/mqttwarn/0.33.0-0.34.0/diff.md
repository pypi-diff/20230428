# Comparing `tmp/mqttwarn-0.33.0.tar.gz` & `tmp/mqttwarn-0.34.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqttwarn-0.33.0.tar", last modified: Tue Apr 11 21:59:27 2023, max compression
+gzip compressed data, was "mqttwarn-0.34.0.tar", last modified: Thu Apr 27 23:09:39 2023, max compression
```

## Comparing `mqttwarn-0.33.0.tar` & `mqttwarn-0.34.0.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.371558 mqttwarn-0.33.0/
--rw-r--r--   0 amo        (501) staff       (20)    13649 2023-04-11 21:57:30.000000 mqttwarn-0.33.0/CHANGES.rst
--rw-r--r--   0 amo        (501) staff       (20)     5908 2023-04-11 21:55:55.000000 mqttwarn-0.33.0/DOCKER.md
--rw-r--r--   0 amo        (501) staff       (20)   133352 2023-04-11 20:10:09.000000 mqttwarn-0.33.0/HANDBOOK.md
--rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)      154 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)    13848 2023-04-11 21:59:27.371212 mqttwarn-0.33.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)    10862 2023-03-12 11:46:29.000000 mqttwarn-0.33.0/README.rst
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.332146 mqttwarn-0.33.0/mqttwarn/
--rw-r--r--   0 amo        (501) staff       (20)      462 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)       50 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/__main__.py
--rw-r--r--   0 amo        (501) staff       (20)     5539 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/commands.py
--rw-r--r--   0 amo        (501) staff       (20)     6023 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/configuration.py
--rw-r--r--   0 amo        (501) staff       (20)     7063 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/context.py
--rw-r--r--   0 amo        (501) staff       (20)    28702 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/core.py
--rw-r--r--   0 amo        (501) staff       (20)     2306 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/cron.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.334729 mqttwarn-0.33.0/mqttwarn/examples/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/examples/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.335372 mqttwarn-0.33.0/mqttwarn/examples/basic/
--rwxr-xr-x   0 amo        (501) staff       (20)     3839 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/examples/basic/mqttwarn.ini
--rwxr-xr-x   0 amo        (501) staff       (20)     3034 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/examples/basic/samplefuncs.py
--rw-r--r--   0 amo        (501) staff       (20)     3342 2023-03-13 00:29:11.000000 mqttwarn-0.33.0/mqttwarn/model.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.369527 mqttwarn-0.33.0/mqttwarn/services/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/alexa-notify-me.py
--rw-r--r--   0 amo        (501) staff       (20)     1322 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/amqp.py
--rw-r--r--   0 amo        (501) staff       (20)     1284 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apns.py
--rw-r--r--   0 amo        (501) staff       (20)      316 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise.py
--rw-r--r--   0 amo        (501) staff       (20)     2636 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_multi.py
--rw-r--r--   0 amo        (501) staff       (20)     2445 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_single.py
--rw-r--r--   0 amo        (501) staff       (20)     1468 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/apprise_util.py
--rw-r--r--   0 amo        (501) staff       (20)     1916 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/asterisk.py
--rw-r--r--   0 amo        (501) staff       (20)     1463 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/autoremote.py
--rw-r--r--   0 amo        (501) staff       (20)     2331 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/azure_iot.py
--rw-r--r--   0 amo        (501) staff       (20)     2114 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/carbon.py
--rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/celery.py
--rw-r--r--   0 amo        (501) staff       (20)     2160 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/chromecast.py
--rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/dbus.py
--rw-r--r--   0 amo        (501) staff       (20)     1467 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/desktopnotify.py
--rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/dnsupdate.py
--rw-r--r--   0 amo        (501) staff       (20)     1345 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/emoncms.py
--rw-r--r--   0 amo        (501) staff       (20)      886 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/execute.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/fbchat.py
--rw-r--r--   0 amo        (501) staff       (20)     2124 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/file.py
--rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/freeswitch.py
--rw-r--r--   0 amo        (501) staff       (20)     1451 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/gss.py
--rw-r--r--   0 amo        (501) staff       (20)     4560 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/gss2.py
--rw-r--r--   0 amo        (501) staff       (20)     1414 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/hangbot.py
--rw-r--r--   0 amo        (501) staff       (20)     1588 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/hipchat.py
--rw-r--r--   0 amo        (501) staff       (20)     4203 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/http_urllib.py
--rw-r--r--   0 amo        (501) staff       (20)     2237 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/icinga2.py
--rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/ifttt.py
--rw-r--r--   0 amo        (501) staff       (20)     3671 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/influxdb.py
--rw-r--r--   0 amo        (501) staff       (20)     2589 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/ionic.py
--rw-r--r--   0 amo        (501) staff       (20)     1311 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/irccat.py
--rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/linuxnotify.py
--rw-r--r--   0 amo        (501) staff       (20)      881 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/log.py
--rw-r--r--   0 amo        (501) staff       (20)     2465 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/mattermost.py
--rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/mqtt.py
--rw-r--r--   0 amo        (501) staff       (20)     2337 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mqtt_filter.py
--rw-r--r--   0 amo        (501) staff       (20)     1340 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mqttpub.py
--rw-r--r--   0 amo        (501) staff       (20)     3064 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql.py
--rw-r--r--   0 amo        (501) staff       (20)     4557 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql_dynamic.py
--rw-r--r--   0 amo        (501) staff       (20)     3075 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/mysql_remap.py
--rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/mythtv.py
--rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/nntp.py
--rw-r--r--   0 amo        (501) staff       (20)     1135 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/nsca.py
--rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/osxsay.py
--rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/pastebinpub.py
--rw-r--r--   0 amo        (501) staff       (20)     1092 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/pipe.py
--rw-r--r--   0 amo        (501) staff       (20)     3360 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/postgres.py
--rw-r--r--   0 amo        (501) staff       (20)     1164 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/prowl.py
--rw-r--r--   0 amo        (501) staff       (20)     1318 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/pushalot.py
--rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/pushbullet.py
--rw-r--r--   0 amo        (501) staff       (20)     5676 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/pushover.py
--rw-r--r--   0 amo        (501) staff       (20)     8091 2023-04-11 20:10:09.000000 mqttwarn-0.33.0/mqttwarn/services/pushsafer.py
--rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/redispub.py
--rw-r--r--   0 amo        (501) staff       (20)     1189 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/rrdtool.py
--rw-r--r--   0 amo        (501) staff       (20)     2202 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/serial.py
--rw-r--r--   0 amo        (501) staff       (20)     3480 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/slack.py
--rw-r--r--   0 amo        (501) staff       (20)     1910 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/slixmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     2156 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/smtp.py
--rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite.py
--rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite_json2cols.py
--rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/sqlite_timestamp.py
--rw-r--r--   0 amo        (501) staff       (20)     2116 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/ssh.py
--rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/syslog.py
--rw-r--r--   0 amo        (501) staff       (20)     4445 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/telegram.py
--rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/thingspeak.py
--rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.33.0/mqttwarn/services/tootpaste.py
--rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/twilio.py
--rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/twitter.py
--rw-r--r--   0 amo        (501) staff       (20)     1210 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/websocket.py
--rw-r--r--   0 amo        (501) staff       (20)     2142 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/xbmc.py
--rw-r--r--   0 amo        (501) staff       (20)     1209 2021-06-19 14:00:07.000000 mqttwarn-0.33.0/mqttwarn/services/xively.py
--rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.33.0/mqttwarn/services/xmpp.py
--rw-r--r--   0 amo        (501) staff       (20)     3239 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/services/zabbix.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.370127 mqttwarn-0.33.0/mqttwarn/testing/
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/testing/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)      375 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/testing/fixtures.py
--rw-r--r--   0 amo        (501) staff       (20)     5474 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/util.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.370885 mqttwarn-0.33.0/mqttwarn/vendor/
--rw-r--r--   0 amo        (501) staff       (20)     2294 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/vendor/ZabbixSender.py
--rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/mqttwarn/vendor/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-11 21:59:27.334460 mqttwarn-0.33.0/mqttwarn.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)    13848 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     2928 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)       51 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/entry_points.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.33.0/mqttwarn.egg-info/not-zip-safe
--rw-r--r--   0 amo        (501) staff       (20)     2255 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)       24 2023-04-11 21:59:27.000000 mqttwarn-0.33.0/mqttwarn.egg-info/top_level.txt
--rw-r--r--   0 amo        (501) staff       (20)     2008 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/pyproject.toml
--rw-r--r--   0 amo        (501) staff       (20)       14 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/requirements-release.txt
--rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-11 21:59:27.371632 mqttwarn-0.33.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     6198 2023-03-12 10:52:16.000000 mqttwarn-0.33.0/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.859610 mqttwarn-0.34.0/
+-rw-r--r--   0 amo        (501) staff       (20)    14685 2023-04-27 23:02:20.000000 mqttwarn-0.34.0/CHANGES.rst
+-rw-r--r--   0 amo        (501) staff       (20)    14197 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)      154 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)    13136 2023-04-27 23:09:39.859302 mqttwarn-0.34.0/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)    10150 2023-04-27 23:07:43.000000 mqttwarn-0.34.0/README.rst
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.816368 mqttwarn-0.34.0/mqttwarn/
+-rw-r--r--   0 amo        (501) staff       (20)      462 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)       50 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/__main__.py
+-rw-r--r--   0 amo        (501) staff       (20)     5906 2023-04-27 23:01:45.000000 mqttwarn-0.34.0/mqttwarn/commands.py
+-rw-r--r--   0 amo        (501) staff       (20)     6341 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/configuration.py
+-rw-r--r--   0 amo        (501) staff       (20)     8249 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/context.py
+-rw-r--r--   0 amo        (501) staff       (20)    30225 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/core.py
+-rw-r--r--   0 amo        (501) staff       (20)     2539 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/cron.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.821459 mqttwarn-0.34.0/mqttwarn/examples/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/examples/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.822592 mqttwarn-0.34.0/mqttwarn/examples/basic/
+-rwxr-xr-x   0 amo        (501) staff       (20)     3832 2023-04-18 22:55:29.000000 mqttwarn-0.34.0/mqttwarn/examples/basic/mqttwarn.ini
+-rwxr-xr-x   0 amo        (501) staff       (20)     3060 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/examples/basic/udf.py
+-rw-r--r--   0 amo        (501) staff       (20)     3733 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/model.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.857833 mqttwarn-0.34.0/mqttwarn/services/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     1317 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/alexa-notify-me.py
+-rw-r--r--   0 amo        (501) staff       (20)     1322 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/amqp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1310 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/apns.py
+-rw-r--r--   0 amo        (501) staff       (20)      316 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/apprise.py
+-rw-r--r--   0 amo        (501) staff       (20)     2639 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_multi.py
+-rw-r--r--   0 amo        (501) staff       (20)     2448 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_single.py
+-rw-r--r--   0 amo        (501) staff       (20)     1392 2023-04-26 22:18:29.000000 mqttwarn-0.34.0/mqttwarn/services/apprise_util.py
+-rw-r--r--   0 amo        (501) staff       (20)     1916 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/asterisk.py
+-rw-r--r--   0 amo        (501) staff       (20)     1463 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/autoremote.py
+-rw-r--r--   0 amo        (501) staff       (20)     2331 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/azure_iot.py
+-rw-r--r--   0 amo        (501) staff       (20)     2114 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/carbon.py
+-rw-r--r--   0 amo        (501) staff       (20)      862 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/celery.py
+-rw-r--r--   0 amo        (501) staff       (20)     2160 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/chromecast.py
+-rw-r--r--   0 amo        (501) staff       (20)     1369 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/dbus.py
+-rw-r--r--   0 amo        (501) staff       (20)     1604 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/desktopnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)     1580 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/dnsupdate.py
+-rw-r--r--   0 amo        (501) staff       (20)     1371 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/emoncms.py
+-rw-r--r--   0 amo        (501) staff       (20)      886 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/execute.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/fbchat.py
+-rw-r--r--   0 amo        (501) staff       (20)     2242 2023-04-18 22:40:03.000000 mqttwarn-0.34.0/mqttwarn/services/file.py
+-rw-r--r--   0 amo        (501) staff       (20)     2609 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/freeswitch.py
+-rw-r--r--   0 amo        (501) staff       (20)     1477 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/gss.py
+-rw-r--r--   0 amo        (501) staff       (20)     4586 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/gss2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1414 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/hangbot.py
+-rw-r--r--   0 amo        (501) staff       (20)     1614 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/hipchat.py
+-rw-r--r--   0 amo        (501) staff       (20)     4229 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/http_urllib.py
+-rw-r--r--   0 amo        (501) staff       (20)     2263 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/icinga2.py
+-rw-r--r--   0 amo        (501) staff       (20)     1084 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/ifttt.py
+-rw-r--r--   0 amo        (501) staff       (20)     3671 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/influxdb.py
+-rw-r--r--   0 amo        (501) staff       (20)     2615 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/ionic.py
+-rw-r--r--   0 amo        (501) staff       (20)     1311 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/irccat.py
+-rw-r--r--   0 amo        (501) staff       (20)     1022 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/linuxnotify.py
+-rw-r--r--   0 amo        (501) staff       (20)      881 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/log.py
+-rw-r--r--   0 amo        (501) staff       (20)     2491 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/mattermost.py
+-rw-r--r--   0 amo        (501) staff       (20)     3468 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/mqtt.py
+-rw-r--r--   0 amo        (501) staff       (20)     2337 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mqtt_filter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1340 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mqttpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     3064 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql.py
+-rw-r--r--   0 amo        (501) staff       (20)     4557 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql_dynamic.py
+-rw-r--r--   0 amo        (501) staff       (20)     3075 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/mysql_remap.py
+-rw-r--r--   0 amo        (501) staff       (20)     1387 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/mythtv.py
+-rw-r--r--   0 amo        (501) staff       (20)     1610 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/nntp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1135 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/nsca.py
+-rw-r--r--   0 amo        (501) staff       (20)    10095 2023-04-27 20:12:45.000000 mqttwarn-0.34.0/mqttwarn/services/ntfy.py
+-rw-r--r--   0 amo        (501) staff       (20)     1040 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/osxsay.py
+-rw-r--r--   0 amo        (501) staff       (20)     1587 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/pastebinpub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1092 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/pipe.py
+-rw-r--r--   0 amo        (501) staff       (20)     3360 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/postgres.py
+-rw-r--r--   0 amo        (501) staff       (20)     1164 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/prowl.py
+-rw-r--r--   0 amo        (501) staff       (20)     1318 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/pushalot.py
+-rw-r--r--   0 amo        (501) staff       (20)     1204 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/pushbullet.py
+-rw-r--r--   0 amo        (501) staff       (20)     5676 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/pushover.py
+-rw-r--r--   0 amo        (501) staff       (20)     8091 2023-04-11 20:10:09.000000 mqttwarn-0.34.0/mqttwarn/services/pushsafer.py
+-rw-r--r--   0 amo        (501) staff       (20)      955 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/redispub.py
+-rw-r--r--   0 amo        (501) staff       (20)     1189 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/rrdtool.py
+-rw-r--r--   0 amo        (501) staff       (20)     2202 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/serial.py
+-rw-r--r--   0 amo        (501) staff       (20)     3480 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/slack.py
+-rw-r--r--   0 amo        (501) staff       (20)     1910 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/slixmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2156 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/smtp.py
+-rw-r--r--   0 amo        (501) staff       (20)     1157 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite.py
+-rw-r--r--   0 amo        (501) staff       (20)     3024 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite_json2cols.py
+-rw-r--r--   0 amo        (501) staff       (20)     1317 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/sqlite_timestamp.py
+-rw-r--r--   0 amo        (501) staff       (20)     2116 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/ssh.py
+-rw-r--r--   0 amo        (501) staff       (20)     2329 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/syslog.py
+-rw-r--r--   0 amo        (501) staff       (20)     4471 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/telegram.py
+-rw-r--r--   0 amo        (501) staff       (20)     2881 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/thingspeak.py
+-rw-r--r--   0 amo        (501) staff       (20)     1780 2021-06-07 22:34:47.000000 mqttwarn-0.34.0/mqttwarn/services/tootpaste.py
+-rw-r--r--   0 amo        (501) staff       (20)     1050 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/twilio.py
+-rw-r--r--   0 amo        (501) staff       (20)     1070 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/twitter.py
+-rw-r--r--   0 amo        (501) staff       (20)     1210 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/services/websocket.py
+-rw-r--r--   0 amo        (501) staff       (20)     2168 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/xbmc.py
+-rw-r--r--   0 amo        (501) staff       (20)     1209 2021-06-19 14:00:07.000000 mqttwarn-0.34.0/mqttwarn/services/xively.py
+-rw-r--r--   0 amo        (501) staff       (20)     2457 2021-06-02 19:14:19.000000 mqttwarn-0.34.0/mqttwarn/services/xmpp.py
+-rw-r--r--   0 amo        (501) staff       (20)     3265 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/services/zabbix.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.858347 mqttwarn-0.34.0/mqttwarn/testing/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/testing/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)      375 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/testing/fixtures.py
+-rw-r--r--   0 amo        (501) staff       (20)     6929 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/util.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.858968 mqttwarn-0.34.0/mqttwarn/vendor/
+-rw-r--r--   0 amo        (501) staff       (20)     2320 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/mqttwarn/vendor/ZabbixSender.py
+-rw-r--r--   0 amo        (501) staff       (20)        0 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/mqttwarn/vendor/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-27 23:09:39.821048 mqttwarn-0.34.0/mqttwarn.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)    13136 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     2924 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)       51 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/entry_points.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2021-06-02 19:17:07.000000 mqttwarn-0.34.0/mqttwarn.egg-info/not-zip-safe
+-rw-r--r--   0 amo        (501) staff       (20)     2300 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)       24 2023-04-27 23:09:39.000000 mqttwarn-0.34.0/mqttwarn.egg-info/top_level.txt
+-rw-r--r--   0 amo        (501) staff       (20)     2257 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/pyproject.toml
+-rw-r--r--   0 amo        (501) staff       (20)       14 2023-03-12 10:52:16.000000 mqttwarn-0.34.0/requirements-release.txt
+-rw-r--r--   0 amo        (501) staff       (20)       38 2023-04-27 23:09:39.859691 mqttwarn-0.34.0/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     6239 2023-04-27 20:56:31.000000 mqttwarn-0.34.0/setup.py
```

### Comparing `mqttwarn-0.33.0/CHANGES.rst` & `mqttwarn-0.34.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,35 @@
 ##################
 
 
 in progress
 ===========
 
 
+2023-04-28 0.34.0
+=================
+
+- Fix: Don't crash when receiving non-UTF8 payloads. Thanks, @sevmonster.
+- Improve exception logging in ``is_filtered``, ``get_topic_data``, and
+  ``get_all_data`` context functions. Thanks, @sevmonster.
+- [core] Allow processing of binary, non-UTF8 message payloads, for example
+  images. Thanks, @sevmonster.
+- [file] Allow writing of binary content. Thanks, @sevmonster.
+- [ux] Rename subcommand ``mqttwarn make-samplefuncs`` to ``mqttwarn make-udf``,
+  and adjust naming.
+- [ntfy] Add dedicated service plugin ``ntfy``
+- [ntfy] Use RFC 2047 for encoding HTTP header values. Thanks, @binwiederhier.
+- [ntfy] Add more fields: icon, cache, firebase, unifiedpush
+- [ntfy] Also interpolate outbound ntfy option fields
+- [ntfy] [Frigate] Improve example/tutorial about Frigate event notifications
+- [ntfy] [Frigate] Synchronize JSON event and snapshot image receive order
+- [ntfy] [Frigate] Tests: Verify notification was properly received by ntfy
+- [cli] Fix ``--config-file`` command line option
+
+
 2023-04-11 0.33.0
 =================
 
 - Pushsafer: Fix to prevent submitting empty parameters to upstream API.
 - Pushsafer: Modernize configuration layout for target addresses.
 - Pushsafer: Add parameters for "Confirm", "Answer Options", and "Force Answer".
```

### Comparing `mqttwarn-0.33.0/LICENSE` & `mqttwarn-0.34.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/PKG-INFO` & `mqttwarn-0.34.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttwarn
-Version: 0.33.0
+Version: 0.34.0
 Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
 Home-page: https://github.com/jpmens/mqttwarn
 Author: Jan-Piet Mens, Ben Jones, Andreas Motl
 Author-email: jpmens@gmail.com
 License: EPL 2.0
 Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
 Classifier: Development Status :: 4 - Beta
@@ -90,25 +90,22 @@
 .. image:: https://img.shields.io/pypi/pyversions/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/v/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/l/mqttwarn.svg
-    :alt: License
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/status/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://pepy.tech/badge/mqttwarn/month
     :target: https://pepy.tech/project/mqttwarn
 
-|
-
 .. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
 
 
 ########
 mqttwarn
 ########
 
@@ -134,104 +131,79 @@
 
 A picture says a thousand words.
 
 .. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/mqttwarn.png
     :target: #
 
 
-Coverage
-========
+Notification service coverage
+=============================
 
 *mqttwarn* comes with **over 70 notification handler plugins** for a wide
 range of notification services and is very open to further contributions.
-You can enjoy the alphabetical list of plugins at `mqttwarn notification
-services`_.
+You can enjoy the alphabetical list of plugins on the `mqttwarn notifier
+catalog`_ page.
 
 On top of that, it integrates with the excellent `Apprise`_ notification
 library. `Apprise notification services`_ has a complete list of the **80+
 notification services** supported by Apprise.
 
 
-Details
-=======
-
-The program, running as a service, subscribes to any number of MQTT topics
-(including wildcards) and publishes received payloads to one or more notification
-services, including support for notifying more than one distinct service
-for the same message.
-
-Notifications are transmitted to the appropriate service via plugins.
-*mqttwarn* provides built-in plugins for a number of services and you
-can easily add your own.
-
-A more detailed blog post about what mqttwarn can be used for is available
-at `How do your servers talk to you?`_.
-
-For example, you may wish to submit an alarm published as text to the
-MQTT topic ``home/monitoring/+`` as notification via *e-mail* and *Pushover*.
-
-
 
 *************
 Documentation
 *************
 
-The `handbook`_ is the right place to read all about *mqttwarn*'s features and
-service plugins.
+The `mqttwarn documentation`_ is the right place to read all about *mqttwarn*'s
+features and integrations, and how you can leverage all its framework components
+for building custom applications. Its service plugins can be inspected on the
+`mqttwarn notifier catalog`_ page.
 
 
 ************
 Installation
 ************
 
+Using pip
+=========
+
 Synopsis::
 
     pip install --upgrade mqttwarn
 
 You can also add support for a specific service plugin::
 
     pip install --upgrade 'mqttwarn[xmpp]'
 
 You can also add support for multiple services, all at once::
 
     pip install --upgrade 'mqttwarn[apprise,asterisk,nsca,desktopnotify,tootpaste,xmpp]'
 
+See also: `Installing mqttwarn with pip`_.
 
-***************
-Container image
-***************
+OCI container image
+===================
 
 For running ``mqttwarn`` on a container infrastructure like Docker or
 Kubernetes, corresponding images are automatically published to the
 GitHub Container Registry (GHCR).
 
 - ``ghcr.io/jpmens/mqttwarn-standard:latest``
 - ``ghcr.io/jpmens/mqttwarn-full:latest``
 
-To learn more about this topic, please follow up reading the `Docker handbook`_.
+To learn more about this topic, please follow up reading the `Using the OCI image
+with Docker or Podman`_ documentation section.
 
 
 *************
 Configuration
 *************
 
-First, create configuration and custom Python starter files
-``mqttwarn.ini`` and ``samplefuncs.py`` and edit them to your taste::
-
-    # Create configuration file
-    mqttwarn make-config > mqttwarn.ini
-
-    # Create file for custom functions
-    mqttwarn make-samplefuncs > samplefuncs.py
-
-If you are using PowerShell on Windows 10, you may find the files to be written
-using the ``UTF-16`` charset encoding. However, ``mqttwarn`` works with ``UTF-8``.
-In order to switch to ``UTF-8``, please invoke this command beforehand::
-
-    $PSDefaultParameterValues['Out-File:Encoding'] = 'utf8'
+In order to learn how to configure mqttwarn, please head over to the documentation
+section about the `mqttwarn configuration`_.
 
 
 *****
 Usage
 *****
 
 Running interactively
@@ -268,142 +240,142 @@
 
     # Launch "file" service plugin
     mqttwarn --plugin=file --options='{"message": "Hello world\n", "addrs": ["/tmp/mqttwarn.err"]}'
 
     # Launch "pushover" service plugin
     mqttwarn --plugin=pushover --options='{"title": "About", "message": "Hello world", "addrs": ["userkey", "token"], "priority": 6}'
 
-    # Launch "ssh" service plugin from the command line
+    # Launch "ntfy" service plugin
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"tags": "foo,bar,äöü", "priority": "high"}'
+
+    # Launch "ntfy" service plugin, and add remote attachment
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"attach": "https://unsplash.com/photos/spdQ1dVuIHw/download?w=320", "filename": "goat.jpg"}'
+
+    # Launch "ntfy" service plugin, and add attachment from local filesystem
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive", "file": "goat.jpg"}, "title": "Example notification", "message": "Hello world"}'
+
+    # Launch "ssh" service plugin
     mqttwarn --plugin=ssh --config='{"host": "ssh.example.org", "port": 22, "user": "foo", "password": "bar"}' --options='{"addrs": ["command with substitution %s"], "payload": "{\"args\": \"192.168.0.1\"}"}'
 
-    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib", passing "--config" parameters via command line
+    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib"
     pip install mqttwarn-contrib
     mqttwarn --plugin=mqttwarn_contrib.services.cloudflare_zone --config='{"auth-email": "foo", "auth-key": "bar"}' --options='{"addrs": ["0815", "www.example.org", ""], "message": "192.168.0.1"}'
 
-    # Submit notification to "ntfy", using Apprise service plugin.
-    mqttwarn --plugin=apprise \
-        --config='{"baseuri": "ntfy://user:password@ntfy.example.org/topic1/topic2"}' \
-        --options='{"addrs": [], "title": "Example notification", "message": "Hello world"}'
-
 
 Also, the ``--config-file`` parameter can be used to optionally specify the
 path to a configuration file.
 
 
 Running as system daemon
 ========================
-- We recommend to use Supervisor_ for running *mqttwarn* as a service, see also `supervisor.ini`_.
-- Alternatively, have a look at `mqttwarn.service`_, the systemd unit configuration file for *mqttwarn*.
 
+There are different ways to run mqttwarn as a system daemon. There are examples
+for systemd, traditional init, OpenRC, and Supervisor_ in the ``etc`` directory
+of this repository, for example `supervisor.ini`_ (Supervisor) and
+`mqttwarn.service`_ (systemd).
 
 Running in a development sandbox
 ================================
-For hacking_ on mqttwarn, please install it in development mode.
 
-
-****************
-Acknowledgements
-****************
-Thanks to all the contributors of *mqttwarn* who got their hands dirty with it
-and helped to co-create and conceive it in one way or another. You know who you are.
+For hacking on mqttwarn, please install it in development mode, using a
+`mqttwarn development sandbox`_ installation.
 
 
 *******************
 Project information
 *******************
 
 About
 =====
 These links will guide you to the source code of *mqttwarn* and its documentation.
 
 - `mqttwarn on GitHub <https://github.com/jpmens/mqttwarn>`_
 - `mqttwarn on the Python Package Index (PyPI) <https://pypi.org/project/mqttwarn/>`_
-- `mqttwarn documentation <https://github.com/jpmens/mqttwarn/tree/main/doc>`_
+- `mqttwarn documentation <https://mqttwarn.readthedocs.io/>`_
 
 
 Requirements
 ============
 You will need at least the following components:
 
 * Python 3.x or PyPy 3.x.
-* An MQTT broker. We recommend Mosquitto_.
-* Some more Python modules to satisfy service dependencies defined in the ``setup.py`` file.
+* An MQTT broker. We recommend `Mosquitto`_.
+* For invoking specific service plugins, additional Python modules may be required.
+  See ``setup.py`` file.
 
 
 Contributing
 ============
+
 We are always happy to receive code contributions, ideas, suggestions
 and problem reports from the community.
 
-So, if you'd like to contribute you're most welcome.
+So, if you would like to contribute, you are most welcome.
 Spend some time taking a look around, locate a bug, design issue or
-spelling mistake and then send us a pull request or create an `issue`_.
+spelling mistake, and then send us a pull request or create an `issue`_.
 
-Thanks in advance for your efforts, we really appreciate any help or feedback.
+Thank you in advance for your efforts, we really appreciate any help or feedback.
 
-There are also some extensions to mqttwarn not included in the core package.
-Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
-`community contributions to mqttwarn`_.
 
+License
+=======
 
-Licenses
-========
-This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
+mqttwarn is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
 
 
 ***************
 Troubleshooting
 ***************
+
 If you encounter any problems during setup or operations or if you have further
 suggestions, please let us know by `opening an issue on GitHub`_. Thank you
 already.
 
 
-*************
-Miscellaneous
-*************
-
-
-Press
-=====
-* The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
-* The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
-  as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
+************
+Attributions
+************
 
+Acknowledgements
+================
+Thanks to all the contributors of *mqttwarn* who helped to conceive it in one
+way or another. You know who you are.
 
 Legal stuff
 ===========
-"MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
+"MQTT" is a trademark of the OASIS open standards consortium, which publishes
+the MQTT specifications.
 
 
 ----
 
 Have fun!
 
 
 .. _Apprise: https://github.com/caronc/apprise
 .. _Apprise notification services: https://github.com/caronc/apprise/wiki#notification-services
 .. _backlog: https://github.com/jpmens/mqttwarn/blob/main/doc/backlog.rst
-.. _community contributions to mqttwarn: https://pypi.org/project/mqttwarn-contrib/
-.. _Docker handbook: https://github.com/jpmens/mqttwarn/blob/main/DOCKER.md
 .. _EPL-2.0: https://www.eclipse.org/legal/epl-2.0/
 .. _hacking: https://github.com/jpmens/mqttwarn/blob/main/doc/hacking.rst
-.. _handbook: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md
-.. _Hiveeyes: https://hiveeyes.org/
 .. _How do your servers talk to you?: https://jpmens.net/2014/04/03/how-do-your-servers-talk-to-you/
+.. _Installing mqttwarn with pip: https://mqttwarn.readthedocs.io/en/latest/usage/pip.html
 .. _issue: https://github.com/jpmens/mqttwarn/issues/new
 .. _LICENSE: https://github.com/jpmens/mqttwarn/blob/main/LICENSE
 .. _Mosquitto: https://mosquitto.org
 .. _MQTTwarn\: Ein Rundum-Sorglos-Notifier: https://web.archive.org/web/20140611040637/http://jaxenter.de/news/MQTTwarn-Ein-Rundum-Sorglos-Notifier-171312
-.. _mqttwarn notification services: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md#supported-notification-services
+.. _mqttwarn configuration: https://mqttwarn.readthedocs.io/en/latest/configure/
+.. _mqttwarn development sandbox: https://mqttwarn.readthedocs.io/en/latest/workbench/sandbox.html
+.. _mqttwarn documentation: https://mqttwarn.readthedocs.io/
+.. _mqttwarn notifier catalog: https://mqttwarn.readthedocs.io/en/latest/notifier-catalog.html
 .. _mqttwarn.service: https://github.com/jpmens/mqttwarn/blob/main/etc/mqttwarn.service
 .. _opening an issue on GitHub: https://github.com/jpmens/mqttwarn/issues/new
 .. _Schwarmalarm using mqttwarn: https://hiveeyes.org/docs/system/schwarmalarm-mqttwarn.html
 .. _Supervisor: https://jpmens.net/2014/02/13/in-my-toolbox-supervisord/
 .. _supervisor.ini: https://github.com/jpmens/mqttwarn/blob/main/etc/supervisor.ini
+.. _Using the OCI image with Docker or Podman: https://mqttwarn.readthedocs.io/en/latest/usage/oci.html
```

### Comparing `mqttwarn-0.33.0/README.rst` & `mqttwarn-0.34.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,22 @@
 .. image:: https://img.shields.io/pypi/pyversions/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/v/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/l/mqttwarn.svg
-    :alt: License
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/status/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://pepy.tech/badge/mqttwarn/month
     :target: https://pepy.tech/project/mqttwarn
 
-|
-
 .. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
 
 
 ########
 mqttwarn
 ########
 
@@ -51,104 +48,79 @@
 
 A picture says a thousand words.
 
 .. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/mqttwarn.png
     :target: #
 
 
-Coverage
-========
+Notification service coverage
+=============================
 
 *mqttwarn* comes with **over 70 notification handler plugins** for a wide
 range of notification services and is very open to further contributions.
-You can enjoy the alphabetical list of plugins at `mqttwarn notification
-services`_.
+You can enjoy the alphabetical list of plugins on the `mqttwarn notifier
+catalog`_ page.
 
 On top of that, it integrates with the excellent `Apprise`_ notification
 library. `Apprise notification services`_ has a complete list of the **80+
 notification services** supported by Apprise.
 
 
-Details
-=======
-
-The program, running as a service, subscribes to any number of MQTT topics
-(including wildcards) and publishes received payloads to one or more notification
-services, including support for notifying more than one distinct service
-for the same message.
-
-Notifications are transmitted to the appropriate service via plugins.
-*mqttwarn* provides built-in plugins for a number of services and you
-can easily add your own.
-
-A more detailed blog post about what mqttwarn can be used for is available
-at `How do your servers talk to you?`_.
-
-For example, you may wish to submit an alarm published as text to the
-MQTT topic ``home/monitoring/+`` as notification via *e-mail* and *Pushover*.
-
-
 
 *************
 Documentation
 *************
 
-The `handbook`_ is the right place to read all about *mqttwarn*'s features and
-service plugins.
+The `mqttwarn documentation`_ is the right place to read all about *mqttwarn*'s
+features and integrations, and how you can leverage all its framework components
+for building custom applications. Its service plugins can be inspected on the
+`mqttwarn notifier catalog`_ page.
 
 
 ************
 Installation
 ************
 
+Using pip
+=========
+
 Synopsis::
 
     pip install --upgrade mqttwarn
 
 You can also add support for a specific service plugin::
 
     pip install --upgrade 'mqttwarn[xmpp]'
 
 You can also add support for multiple services, all at once::
 
     pip install --upgrade 'mqttwarn[apprise,asterisk,nsca,desktopnotify,tootpaste,xmpp]'
 
+See also: `Installing mqttwarn with pip`_.
 
-***************
-Container image
-***************
+OCI container image
+===================
 
 For running ``mqttwarn`` on a container infrastructure like Docker or
 Kubernetes, corresponding images are automatically published to the
 GitHub Container Registry (GHCR).
 
 - ``ghcr.io/jpmens/mqttwarn-standard:latest``
 - ``ghcr.io/jpmens/mqttwarn-full:latest``
 
-To learn more about this topic, please follow up reading the `Docker handbook`_.
+To learn more about this topic, please follow up reading the `Using the OCI image
+with Docker or Podman`_ documentation section.
 
 
 *************
 Configuration
 *************
 
-First, create configuration and custom Python starter files
-``mqttwarn.ini`` and ``samplefuncs.py`` and edit them to your taste::
-
-    # Create configuration file
-    mqttwarn make-config > mqttwarn.ini
-
-    # Create file for custom functions
-    mqttwarn make-samplefuncs > samplefuncs.py
-
-If you are using PowerShell on Windows 10, you may find the files to be written
-using the ``UTF-16`` charset encoding. However, ``mqttwarn`` works with ``UTF-8``.
-In order to switch to ``UTF-8``, please invoke this command beforehand::
-
-    $PSDefaultParameterValues['Out-File:Encoding'] = 'utf8'
+In order to learn how to configure mqttwarn, please head over to the documentation
+section about the `mqttwarn configuration`_.
 
 
 *****
 Usage
 *****
 
 Running interactively
@@ -185,142 +157,142 @@
 
     # Launch "file" service plugin
     mqttwarn --plugin=file --options='{"message": "Hello world\n", "addrs": ["/tmp/mqttwarn.err"]}'
 
     # Launch "pushover" service plugin
     mqttwarn --plugin=pushover --options='{"title": "About", "message": "Hello world", "addrs": ["userkey", "token"], "priority": 6}'
 
-    # Launch "ssh" service plugin from the command line
+    # Launch "ntfy" service plugin
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"tags": "foo,bar,äöü", "priority": "high"}'
+
+    # Launch "ntfy" service plugin, and add remote attachment
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"attach": "https://unsplash.com/photos/spdQ1dVuIHw/download?w=320", "filename": "goat.jpg"}'
+
+    # Launch "ntfy" service plugin, and add attachment from local filesystem
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive", "file": "goat.jpg"}, "title": "Example notification", "message": "Hello world"}'
+
+    # Launch "ssh" service plugin
     mqttwarn --plugin=ssh --config='{"host": "ssh.example.org", "port": 22, "user": "foo", "password": "bar"}' --options='{"addrs": ["command with substitution %s"], "payload": "{\"args\": \"192.168.0.1\"}"}'
 
-    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib", passing "--config" parameters via command line
+    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib"
     pip install mqttwarn-contrib
     mqttwarn --plugin=mqttwarn_contrib.services.cloudflare_zone --config='{"auth-email": "foo", "auth-key": "bar"}' --options='{"addrs": ["0815", "www.example.org", ""], "message": "192.168.0.1"}'
 
-    # Submit notification to "ntfy", using Apprise service plugin.
-    mqttwarn --plugin=apprise \
-        --config='{"baseuri": "ntfy://user:password@ntfy.example.org/topic1/topic2"}' \
-        --options='{"addrs": [], "title": "Example notification", "message": "Hello world"}'
-
 
 Also, the ``--config-file`` parameter can be used to optionally specify the
 path to a configuration file.
 
 
 Running as system daemon
 ========================
-- We recommend to use Supervisor_ for running *mqttwarn* as a service, see also `supervisor.ini`_.
-- Alternatively, have a look at `mqttwarn.service`_, the systemd unit configuration file for *mqttwarn*.
 
+There are different ways to run mqttwarn as a system daemon. There are examples
+for systemd, traditional init, OpenRC, and Supervisor_ in the ``etc`` directory
+of this repository, for example `supervisor.ini`_ (Supervisor) and
+`mqttwarn.service`_ (systemd).
 
 Running in a development sandbox
 ================================
-For hacking_ on mqttwarn, please install it in development mode.
 
-
-****************
-Acknowledgements
-****************
-Thanks to all the contributors of *mqttwarn* who got their hands dirty with it
-and helped to co-create and conceive it in one way or another. You know who you are.
+For hacking on mqttwarn, please install it in development mode, using a
+`mqttwarn development sandbox`_ installation.
 
 
 *******************
 Project information
 *******************
 
 About
 =====
 These links will guide you to the source code of *mqttwarn* and its documentation.
 
 - `mqttwarn on GitHub <https://github.com/jpmens/mqttwarn>`_
 - `mqttwarn on the Python Package Index (PyPI) <https://pypi.org/project/mqttwarn/>`_
-- `mqttwarn documentation <https://github.com/jpmens/mqttwarn/tree/main/doc>`_
+- `mqttwarn documentation <https://mqttwarn.readthedocs.io/>`_
 
 
 Requirements
 ============
 You will need at least the following components:
 
 * Python 3.x or PyPy 3.x.
-* An MQTT broker. We recommend Mosquitto_.
-* Some more Python modules to satisfy service dependencies defined in the ``setup.py`` file.
+* An MQTT broker. We recommend `Mosquitto`_.
+* For invoking specific service plugins, additional Python modules may be required.
+  See ``setup.py`` file.
 
 
 Contributing
 ============
+
 We are always happy to receive code contributions, ideas, suggestions
 and problem reports from the community.
 
-So, if you'd like to contribute you're most welcome.
+So, if you would like to contribute, you are most welcome.
 Spend some time taking a look around, locate a bug, design issue or
-spelling mistake and then send us a pull request or create an `issue`_.
+spelling mistake, and then send us a pull request or create an `issue`_.
 
-Thanks in advance for your efforts, we really appreciate any help or feedback.
+Thank you in advance for your efforts, we really appreciate any help or feedback.
 
-There are also some extensions to mqttwarn not included in the core package.
-Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
-`community contributions to mqttwarn`_.
 
+License
+=======
 
-Licenses
-========
-This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
+mqttwarn is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
 
 
 ***************
 Troubleshooting
 ***************
+
 If you encounter any problems during setup or operations or if you have further
 suggestions, please let us know by `opening an issue on GitHub`_. Thank you
 already.
 
 
-*************
-Miscellaneous
-*************
-
-
-Press
-=====
-* The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
-* The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
-  as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
+************
+Attributions
+************
 
+Acknowledgements
+================
+Thanks to all the contributors of *mqttwarn* who helped to conceive it in one
+way or another. You know who you are.
 
 Legal stuff
 ===========
-"MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
+"MQTT" is a trademark of the OASIS open standards consortium, which publishes
+the MQTT specifications.
 
 
 ----
 
 Have fun!
 
 
 .. _Apprise: https://github.com/caronc/apprise
 .. _Apprise notification services: https://github.com/caronc/apprise/wiki#notification-services
 .. _backlog: https://github.com/jpmens/mqttwarn/blob/main/doc/backlog.rst
-.. _community contributions to mqttwarn: https://pypi.org/project/mqttwarn-contrib/
-.. _Docker handbook: https://github.com/jpmens/mqttwarn/blob/main/DOCKER.md
 .. _EPL-2.0: https://www.eclipse.org/legal/epl-2.0/
 .. _hacking: https://github.com/jpmens/mqttwarn/blob/main/doc/hacking.rst
-.. _handbook: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md
-.. _Hiveeyes: https://hiveeyes.org/
 .. _How do your servers talk to you?: https://jpmens.net/2014/04/03/how-do-your-servers-talk-to-you/
+.. _Installing mqttwarn with pip: https://mqttwarn.readthedocs.io/en/latest/usage/pip.html
 .. _issue: https://github.com/jpmens/mqttwarn/issues/new
 .. _LICENSE: https://github.com/jpmens/mqttwarn/blob/main/LICENSE
 .. _Mosquitto: https://mosquitto.org
 .. _MQTTwarn\: Ein Rundum-Sorglos-Notifier: https://web.archive.org/web/20140611040637/http://jaxenter.de/news/MQTTwarn-Ein-Rundum-Sorglos-Notifier-171312
-.. _mqttwarn notification services: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md#supported-notification-services
+.. _mqttwarn configuration: https://mqttwarn.readthedocs.io/en/latest/configure/
+.. _mqttwarn development sandbox: https://mqttwarn.readthedocs.io/en/latest/workbench/sandbox.html
+.. _mqttwarn documentation: https://mqttwarn.readthedocs.io/
+.. _mqttwarn notifier catalog: https://mqttwarn.readthedocs.io/en/latest/notifier-catalog.html
 .. _mqttwarn.service: https://github.com/jpmens/mqttwarn/blob/main/etc/mqttwarn.service
 .. _opening an issue on GitHub: https://github.com/jpmens/mqttwarn/issues/new
 .. _Schwarmalarm using mqttwarn: https://hiveeyes.org/docs/system/schwarmalarm-mqttwarn.html
 .. _Supervisor: https://jpmens.net/2014/02/13/in-my-toolbox-supervisord/
 .. _supervisor.ini: https://github.com/jpmens/mqttwarn/blob/main/etc/supervisor.ini
+.. _Using the OCI image with Docker or Podman: https://mqttwarn.readthedocs.io/en/latest/usage/oci.html
```

### Comparing `mqttwarn-0.33.0/mqttwarn/commands.py` & `mqttwarn-0.34.0/mqttwarn/commands.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # -*- coding: utf-8 -*-
-# (c) 2014-2019 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
 from __future__ import print_function
 
 import codecs
 import json
 import logging
 import os
 import signal
 import sys
+import typing as t
 
 from docopt import docopt
 
 from mqttwarn import __version__
 from mqttwarn.configuration import Config, load_configuration
 from mqttwarn.core import bootstrap, cleanup, run_plugin, subscribe_forever
 from mqttwarn.util import get_resource_content
@@ -21,36 +22,36 @@
 APP_NAME = "mqttwarn"
 
 
 def run():
     """
     Usage:
       {program} [make-config]
-      {program} [make-samplefuncs]
-      {program} [--config=] [--config-file=] [--plugin=] [--options=]
+      {program} [make-udf]
+      {program} [--config=] [--config-file=] [--plugin=] [--options=] [--data=]
       {program} --version
       {program} (-h | --help)
 
     No options:
       mqttwarn will start as a service.
 
     Interactive options:
       [--config=]               Use configuration settings from JSON string
       [--config-file=]          Use configuration settings from JSON file
       [--plugin=]               The plugin name to load. This can either be a
                                 full qualified Python package/module name or a
                                 path to a Python file.
-      [--options=]              Configuration options to propagate to the plugin
-                                entrypoint.
+      [--options=]              Configuration options to propagate to the plugin entrypoint.
+      [--data=]                 Data to propagate to the plugin entrypoint.
 
     Bootstrapping options:
       make-config               Dump configuration file blueprint to STDOUT,
                                 suitable for redirecting into a configuration file.
-      make-samplefuncs          Dump blueprint for custom functions file to STDOUT,
-                                suitable for redirecting into a `samplefuncs.py` file.
+      make-udf                  Dump blueprint for user-defined functions file to STDOUT,
+                                suitable for redirecting into a `udf.py` file.
 
     Miscellaneous options:
       --version                 Show version information
       -h --help                 Show this screen
 
     """
 
@@ -64,38 +65,45 @@
     utf8_writer = codecs.getwriter("utf-8")
     sys.stdout = utf8_writer(sys.stdout.buffer)
 
     if options["make-config"]:
         payload = get_resource_content("mqttwarn.examples", "basic/mqttwarn.ini")
         print(payload)
 
-    elif options["make-samplefuncs"]:
-        payload = get_resource_content("mqttwarn.examples", "basic/samplefuncs.py")
+    elif options["make-udf"]:
+        payload = get_resource_content("mqttwarn.examples", "basic/udf.py")
         print(payload)
 
     elif options["--plugin"] and options["--options"]:
 
         # Decode arguments
         arg_plugin = options["--plugin"]
-        arg_options = json.loads(options["--options"])
+        arg_options = options["--options"] and json.loads(options["--options"]) or {}
+        arg_data = options["--data"] and json.loads(options["--data"]) or {}
         arg_config = None
         if "--config" in options and options["--config"] is not None:
             arg_config = json.loads(options["--config"])
 
         # Launch service plugin in standalone mode
         launch_plugin_standalone(
-            arg_plugin, arg_options, configfile=options.get("--config-file"), config_more=arg_config
+            arg_plugin, arg_options, arg_data, configfile=options.get("--config-file"), config_more=arg_config
         )
 
     # Run mqttwarn in service mode when no command line arguments are given
     else:
-        run_mqttwarn()
+        run_mqttwarn(configfile=options["--config-file"])
 
 
-def launch_plugin_standalone(plugin, options, configfile=None, config_more=None):
+def launch_plugin_standalone(
+    plugin: str,
+    options: t.Dict,
+    data: t.Dict,
+    configfile: t.Optional[str] = None,
+    config_more: t.Optional[t.Dict] = None,
+):
 
     # Optionally load configuration file
     does_not_exist = False
     scriptname = os.path.splitext(os.path.basename(sys.argv[0]))[0]
     try:
         config = load_configuration(configfile=configfile, name=scriptname)
     except FileNotFoundError:
@@ -116,24 +124,24 @@
     setup_logging(config)
     if does_not_exist:
         logger.info('Configuration file "{}" does not exist, using default settings'.format(configfile))
 
     logger.info('Running service plugin "{}" with options "{}"'.format(plugin, options))
 
     # Launch service plugin
-    run_plugin(config=config, name=plugin, options=options)
+    run_plugin(config=config, name=plugin, options=options, data=data)
 
 
-def run_mqttwarn():
+def run_mqttwarn(configfile: t.Optional[str] = None):
 
     # Script name (without extension) used as last resort fallback for config/logfile names
     scriptname = os.path.splitext(os.path.basename(sys.argv[0]))[0]
 
     # Load configuration file
-    config = load_configuration(name=scriptname)
+    config = load_configuration(configfile=configfile, name=scriptname)
 
     # Setup logging
     setup_logging(config)
     logger.info("Starting {}".format(scriptname))
     logger.info("Log level is %s" % logging.getLevelName(logger.getEffectiveLevel()))
 
     # Handle signals
@@ -143,15 +151,15 @@
     # Bootstrap mqttwarn.core
     bootstrap(config=config, scriptname=scriptname)
 
     # Connect to broker and start listening
     subscribe_forever()
 
 
-def setup_logging(config):
+def setup_logging(config: Config):
     LOGLEVEL = config.loglevelnumber
     LOGFILE = config.logfile
     LOGFORMAT = config.logformat
 
     # Send log messages to sys.stderr by configuring "logfile = stream://sys.stderr"
     if not LOGFILE:
         pass
```

### Comparing `mqttwarn-0.33.0/mqttwarn/configuration.py` & `mqttwarn-0.34.0/mqttwarn/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
-# (c) 2014-2022 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
 import ast
 import codecs
 import logging
 import os
 import sys
+import typing as t
 from configparser import NoOptionError, RawConfigParser
 
 from mqttwarn.util import load_functions
 
 HAVE_TLS = True
 try:
     import ssl
@@ -17,21 +18,21 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class Config(RawConfigParser):
 
-    specials = {
+    specials: t.Dict[str, t.Union[bool, None]] = {
         "TRUE": True,
         "FALSE": False,
         "NONE": None,
     }
 
-    def __init__(self, configuration_file=None, defaults=None):
+    def __init__(self, configuration_file: t.Optional[str] = None, defaults: t.Optional[t.Dict] = None):
 
         defaults = defaults or {}
 
         self.configuration_path = None
 
         RawConfigParser.__init__(self)
         if configuration_file is not None:
@@ -44,14 +45,15 @@
         """ set defaults """
         self.hostname = "localhost"
         self.port = 1883
         self.username = None
         self.password = None
         self.clientid = None
         self.lwt = None
+        self.lwt_alive = None
         self.skipretained = False
         self.cleansession = False
         self.protocol = 3
 
         self.logformat = "%(asctime)-15s %(levelname)-8s [%(name)-26s] %(message)s"
         self.logfile = "stream://sys.stderr"
         self.loglevel = "DEBUG"
@@ -106,66 +108,67 @@
 
             # Load function file relative to path of configuration file if path is relative.
             else:
                 functions_file = os.path.join(self.configuration_path, self.functions)
 
             self.functions = load_functions(functions_file)
 
-    def level2number(self, level):
+    def level2number(self, level: str) -> int:
 
         levels = {
             "CRITICAL": 50,
             "DEBUG": 10,
             "ERROR": 40,
             "FATAL": 50,
             "INFO": 20,
             "NOTSET": 0,
             "WARN": 30,
             "WARNING": 30,
         }
 
         return levels.get(level.upper(), levels["DEBUG"])
 
-    def g(self, section, key, default=None):
+    def g(self, section: str, key: str, default=None) -> t.Any:
+        val = None
         try:
             val = self.get(section, key)
             if isinstance(val, str) and val.upper() in self.specials:
                 return self.specials[val.upper()]
             return ast.literal_eval(val)
         except NoOptionError:
             return default
         except ValueError:  # e.g. %(xxx)s in string
             return val
         except SyntaxError:  # If not python value, e.g. list of targets coma separated
             return val
         except:
             raise
-            return val
 
-    def getlist(self, section, key):
+    def getlist(self, section: str, key: str) -> t.Union[t.List, None]:
         """Return a list, fail if it isn't a list"""
 
         val = None
         try:
-            val = self.get(section, key)
-            val = [s.strip() for s in val.split(",")]
+            val_str = self.get(section, key)
+            val = [s.strip() for s in val_str.split(",")]
         except Exception as e:
             logger.warning("Expecting a list in section `%s', key `%s' (%s)" % (section, key, e))
 
         return val
 
-    def getdict(self, section, key):
+    # TODO: Add return type annotation.
+    def getdict(self, section: str, key: str):
         val = self.g(section, key)
 
         try:
             return dict(val)
         except:
             return None
 
-    def config(self, section):
+    def config(self, section: str) -> t.Dict:
         """Convert a whole section's options (except the options specified
         explicitly below) into a dict, turning
 
             [config:mqtt]
             host = 'localhost'
             username = None
             list = [1, 'aaa', 'bbb', 4]
@@ -179,25 +182,25 @@
 
         d = {}
         if self.has_section(section):
             d = dict((key, self.g(section, key)) for (key) in self.options(section) if key not in ["targets", "module"])
         return d
 
 
-def load_configuration(configfile=None, name="mqttwarn"):
+def load_configuration(configfile: t.Optional[str] = None, name: str = "mqttwarn") -> Config:
 
     if configfile is None:
-        configfile = os.getenv(name.upper() + "INI", name + ".ini")
+        configfile = str(os.getenv(name.upper() + "INI", name + ".ini"))
 
     if not os.path.exists(configfile):
         raise FileNotFoundError('Configuration file "{}" does not exist'.format(configfile))
 
     # TODO: There should be a factory method which creates a `Config` instance,
     #       including defaults, but without loading a configuration file.
-    defaults = {
+    defaults: t.Dict[str, str] = {
         "clientid": name,
         "lwt": "clients/{}".format(name),
         "lwt_alive": "1",
         "lwt_dead": "0",
     }
 
     return Config(configfile, defaults=defaults)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/context.py` & `mqttwarn-0.34.0/mqttwarn/context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # -*- coding: utf-8 -*-
-# (c) 2014-2022 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
 import logging
 import typing as t
 
 import attr
 
 from mqttwarn.configuration import Config
+from mqttwarn.model import Service, TdataType, TopicTargetType
 from mqttwarn.util import load_function, sanitize_function_name
 
 logger = logging.getLogger(__name__)
 
 
 @attr.s
 class RuntimeContext:
     """
     This carries runtime information and provides the core
     with essential methods for accessing the configuration
     and for invoking parts of the transformation machinery.
     """
 
     config: Config = attr.ib()
-    invoker: t.Optional["FunctionInvoker"] = attr.ib()
+    invoker: "FunctionInvoker" = attr.ib()
 
-    def get_sections(self):
+    def get_sections(self) -> t.List[str]:
         sections = []
         for section in self.config.sections():
             if section == "defaults":
                 continue
             if section == "cron":
                 continue
             if section == "failover":
@@ -35,121 +36,133 @@
                 continue
             if self.config.has_option(section, "targets"):
                 sections.append(section)
             else:
                 logger.warning("Section `%s' has no targets defined" % section)
         return sections
 
-    def get_topic(self, section):
+    def get_topic(self, section: str) -> str:
         if self.config.has_option(section, "topic"):
             return self.config.get(section, "topic")
         return section
 
-    def get_qos(self, section):
+    def get_qos(self, section: str) -> int:
         qos = 0
         if self.config.has_option(section, "qos"):
             qos = int(self.config.get(section, "qos"))
         return qos
 
-    def get_config(self, section, name):
+    def get_config(self, section: str, name: str) -> t.Any:
         value = None
         if self.config.has_option(section, name):
             value = self.config.get(section, name)
         return value
 
-    def is_filtered(self, section, topic, payload):
+    def is_filtered(self, section: str, topic: str, payload: t.AnyStr) -> bool:
         if self.config.has_option(section, "filter"):
-            filterfunc = sanitize_function_name(self.config.get(section, "filter"))
             try:
-                return self.invoker.filter(filterfunc, topic, payload, section)
+                name = sanitize_function_name(self.config.get(section, "filter"))
+                return self.invoker.filter(name, topic, payload, section)
             except Exception as e:
-                logger.warning("Cannot invoke filter function '%s' defined in '%s': %s" % (filterfunc, section, e))
+                logger.exception("Cannot invoke filter function '%s' defined in '%s': %s" % (name, section, e))
         return False
 
-    def get_topic_data(self, section, topic):
+    def get_topic_data(self, section: str, data: TdataType) -> t.Optional[TdataType]:
         if self.config.has_option(section, "datamap"):
-            name = sanitize_function_name(self.config.get(section, "datamap"))
             try:
-                return self.invoker.datamap(name, topic)
+                name = sanitize_function_name(self.config.get(section, "datamap"))
+                return self.invoker.datamap(name, data)
             except Exception as e:
-                logger.warning("Cannot invoke datamap function '%s' defined in '%s': %s" % (name, section, e))
+                logger.exception("Cannot invoke datamap function '%s' defined in '%s': %s" % (name, section, e))
         return None
 
-    def get_all_data(self, section, topic, data):
+    def get_all_data(self, section: str, topic: str, data: TdataType) -> t.Optional[TdataType]:
         if self.config.has_option(section, "alldata"):
-            name = sanitize_function_name(self.config.get(section, "alldata"))
             try:
+                name = sanitize_function_name(self.config.get(section, "alldata"))
                 return self.invoker.alldata(name, topic, data)
             except Exception as e:
-                logger.warning("Cannot invoke alldata function '%s' defined in '%s': %s" % (name, section, e))
+                logger.exception("Cannot invoke alldata function '%s' defined in '%s': %s" % (name, section, e))
         return None
 
-    def get_topic_targets(self, section, topic, data):
+    def get_topic_targets(self, section: str, topic: str, data: TdataType) -> TopicTargetType:
         """
         Topic targets function invoker.
         """
         if self.config.has_option(section, "targets"):
-            name = sanitize_function_name(self.config.get(section, "targets"))
             try:
+                name = sanitize_function_name(self.config.get(section, "targets"))
                 return self.invoker.topic_target_list(name, topic, data)
             except Exception as ex:
                 error = repr(ex)
                 logger.warning(
                     'Error invoking topic targets function "{name}" '
                     'defined in section "{section}": {error}'.format(**locals())
                 )
         return None
 
-    def get_service_config(self, service):
+    def get_service_config(self, service: str) -> t.Dict[str, t.Any]:
         config = self.config.config("config:" + service)
         if config is None:
             return {}
         return dict(config)
 
-    def get_service_targets(self, service):
-        # Be more graceful with jobs w/o any target address information (2021-10-18 [amo]).
+    def get_service_targets(self, service: str) -> t.List[TopicTargetType]:
+        """
+        Resolve target address descriptor.
+
+        2021-10-18 [amo]: Be more graceful with jobs w/o any target address information.
+        """
+        targets: t.List[TopicTargetType] = []
         try:
-            targets = self.config.getdict("config:" + service, "targets") or [None]
-            return targets
+            targets = self.config.getdict("config:" + service, "targets")
         except:
             logger.exception("Unable to access targets for service `%s'" % service)
 
+        # TODO: The target address descriptor may be of any type these days,
+        #       and not necessarily a list.
+        # TODO: Currently, this makes sure to always return one element.
+        #       Verify if this is really needed.
+        targets = targets or [None]
+        return targets
+
 
 @attr.s
 class FunctionInvoker:
     """
     This helps the ``RuntimeContext`` to dynamically invoke
     functions from a configured Python source code file.
     """
 
-    config = attr.ib()
-    srv = attr.ib()
+    config: Config = attr.ib()
+    srv: Service = attr.ib()
 
-    def datamap(self, name, topic):
+    def datamap(self, name: str, data: TdataType) -> TdataType:
         """
         Invoke function "name" loaded from the "functions" Python module.
 
         :param name:    Function name to invoke
-        :param topic:   Topic to pass to the invoked function
+        :param data:    Data to pass to the invoked function
         :return:        Return value of function invocation
         """
 
         val = None
+
         try:
             func = load_function(name=name, py_mod=self.config.functions)
             try:
-                val = func(topic, self.srv)  # new version
+                val = func(data, self.srv)  # new version
             except TypeError:
-                val = func(topic)  # legacy
+                val = func(data)  # legacy
         except:
             raise
 
         return val
 
-    def alldata(self, name, topic, data):
+    def alldata(self, name: str, topic: str, data: TdataType) -> TdataType:
         """
         Invoke function "name" loaded from the "functions" Python module.
 
         :param name:    Function name to invoke
         :param topic:   Topic to pass to the invoked function
         :param data:    Data to pass to the invoked function
         :return:        Return value of function invocation
@@ -160,15 +173,15 @@
             func = load_function(name=name, py_mod=self.config.functions)
             val = func(topic, data, self.srv)
         except:
             raise
 
         return val
 
-    def topic_target_list(self, name, topic, data):
+    def topic_target_list(self, name: str, topic: str, data: TdataType) -> TopicTargetType:
         """
         Invoke function "name" loaded from the "functions" Python module.
         Computes dynamic topic subscription targets.
         Obtains MQTT topic and transformation data.
 
         :param name:    Function name to invoke
         :param topic:   Topic to pass to the invoked function
@@ -181,29 +194,36 @@
             func = load_function(name=name, py_mod=self.config.functions)
             val = func(topic=topic, data=data, srv=self.srv)
         except:
             raise
 
         return val
 
-    def filter(self, name, topic, payload, section=None):  # noqa:A003
+    def filter(self, name: str, topic: str, payload: t.AnyStr, section: t.Optional[str] = None) -> bool:  # noqa:A003
         """
         Invoke function "name" loaded from the "functions" Python module.
         Return that function's True/False.
 
         :param name:    Function name to invoke
         :param topic:   Topic to pass to the invoked function
         :param payload: Payload to pass to the invoked function
         :return:        Return value of function invocation
         """
 
+        # Filtering currently only works on text.
+        # TODO: To let filtering also work on binary data, this line would need to go elsewhere. But where?
+        if isinstance(payload, bytes):
+            payload_decoded = payload.decode("utf-8")
+        else:
+            payload_decoded = payload
+
         rc = False
         try:
             func = load_function(name=name, py_mod=self.config.functions)
             try:
-                rc = func(topic, payload, section, self.srv)  # new version
+                rc = func(topic, payload_decoded, section, self.srv)  # new version
             except TypeError:
-                rc = func(topic, payload)  # legacy signature
+                rc = func(topic, payload_decoded)  # legacy signature
         except:
             raise
 
         return rc
```

### Comparing `mqttwarn-0.33.0/mqttwarn/core.py` & `mqttwarn-0.34.0/mqttwarn/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 # -*- coding: utf-8 -*-
-# (c) 2014-2022 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
 import logging
 import os
 import socket
 import sys
 import threading
 import time
 import typing as t
 from builtins import chr, str
 from datetime import datetime
 from queue import Queue
 
 import paho.mqtt.client as paho
+from paho.mqtt.client import Client as MqttClient
+from paho.mqtt.client import MQTTMessage
 from pkg_resources import resource_filename
 
 import mqttwarn.configuration
 from mqttwarn.context import FunctionInvoker, RuntimeContext
 from mqttwarn.cron import PeriodicThread
-from mqttwarn.model import Job, Service, StatusInformation, Struct
+from mqttwarn.model import Job, Service, StatusInformation, Struct, TdataType
 from mqttwarn.util import (
     Formatter,
     asbool,
     load_function,
     load_module_by_name,
     load_module_from_file,
     parse_cron_options,
     sanitize_function_name,
     timeout,
+    truncate,
 )
 
 try:
     import json
 except ImportError:  # pragma: nocover
     import simplejson as json  # type: ignore
 
@@ -47,35 +50,35 @@
 
 logger = logging.getLogger(__name__)
 
 # Name of calling program
 SCRIPTNAME = "mqttwarn"
 
 # Global runtime context object
-context: t.Optional[RuntimeContext] = None
+context: RuntimeContext
 
 # Global configuration object
-cf: t.Optional[mqttwarn.configuration.Config] = None
+cf: mqttwarn.configuration.Config
 
 # Global handle to MQTT client
-mqttc: t.Optional[paho.Client] = None
-
+mqttc: paho.Client
+mqttc = None
 
 # Initialize processor queue
 q_in: Queue = Queue(maxsize=0)
 exit_flag = False
 
 # Instances of PeriodicThread objects
-ptlist = {}
+ptlist: t.Dict[str, PeriodicThread] = {}
 
 # Instances of loaded service plugins
 service_plugins: t.Dict[str, t.Dict[str, t.Any]] = dict()
 
 
-def make_service(mqttc=None, name=None):
+def make_service(mqttc: paho.Client = None, name: t.Optional[str] = None) -> Service:
     """
     Service object factory.
     Prepare service object for plugin.
     Inject appropriate MQTT client and logger objects.
 
     :param mqttc: Instance of PAHO MQTT client object.
     :param name:  Name used for obtaining a logger instance.
@@ -83,25 +86,25 @@
     """
     name = name or "unknown"
     logger = logging.getLogger(name)
     service = Service(mqttc=mqttc, logger=logger, mwcore=globals(), program=SCRIPTNAME)
     return service
 
 
-def render_template(filename, data):
+def render_template(filename: str, data: TdataType) -> t.Optional[str]:
     text = None
     if HAVE_JINJA is True:
         template = jenv.get_template(filename)
         text = template.render(data)
 
     return text
 
 
 # MQTT broker callbacks
-def on_connect(mosq, userdata, flags, result_code):
+def on_connect(mosq: MqttClient, userdata: t.Dict[str, str], flags: t.Dict[str, str], result_code: int):
     """
     Handle connections (or failures) to the broker.
     This is called after the client has received a CONNACK message
     from the broker in response to calling connect().
 
     The result_code is one of;
     0: Success
@@ -143,34 +146,44 @@
         logger.error("Connection refused - bad user name or password")
     elif result_code == 5:
         logger.error("Connection refused - not authorised")
     else:
         logger.error("Connection failed - result code %d" % (result_code))
 
 
-def on_disconnect(mosq, userdata, result_code):
+def on_disconnect(mosq: MqttClient, userdata: t.Dict[str, str], result_code: int):
     """
     Handle disconnections from the broker
     """
     if result_code == 0:
         logger.info("Clean disconnection from broker")
     else:
-        send_failover("brokerdisconnected", "Broker connection lost. Will attempt to reconnect in 5s")
+        send_failover("brokerdisconnected", b"Broker connection lost. Will attempt to reconnect in 5s")
         # TODO: Review this.
         time.sleep(5)
 
 
-def on_message(mosq, userdata, msg):
+def on_message(mosq: MqttClient, userdata: t.Dict[str, str], msg: MQTTMessage):
+    """
+    Dispatch message received from the MQTT broker to mqttwarn's handler machinery.
+    """
+    try:
+        return on_message_handler(mosq, userdata, msg)
+    except:
+        logger.exception("Receiving and decoding MQTT message failed")
+
+
+def on_message_handler(mosq: MqttClient, userdata: t.Dict[str, str], msg: MQTTMessage):
     """
     Message received from the broker
     """
 
     topic = msg.topic
-    payload = msg.payload.decode("utf-8")
-    logger.debug("Message received on %s: %s" % (topic, payload))
+    payload = msg.payload
+    logger.debug(f"Message received on {topic}: {truncate(payload)}")
 
     if msg.retain == 1:
         if cf.skipretained:
             logger.debug("Skipping retained message on %s" % topic)
             return
 
     # Try to find matching settings for this topic
@@ -189,37 +202,44 @@
             # Send the message to any targets specified
             send_to_targets(section, topic, payload)
 
 
 # End of MQTT broker callbacks
 
 
-def send_failover(reason, message):
+def send_failover(reason: str, message: t.AnyStr):
     # Make sure we dump this event to the log
     logger.warning(message)
     # Attempt to send the message to our failover targets
     send_to_targets("failover", reason, message)
 
 
-def send_to_targets(section, topic, payload):
+def send_to_targets(section: str, topic: str, payload: t.AnyStr):
     if cf.has_section(section) is False:
         logger.warning(
             "Section [%s] does not exist in your INI file, skipping message on topic '%s'" % (section, topic)
         )
         return
 
     # decode raw payload into transformation data
     data = decode_payload(section, topic, payload)
 
+    # Probe if it's a function name.
+    function_name = None
+    try:
+        function_name = sanitize_function_name(context.get_config(section, "targets"))
+    except:
+        pass
     dispatcher_dict = cf.getdict(section, "targets")
-    function_name = sanitize_function_name(context.get_config(section, "targets"))
 
     # `targets` is a function symbol.
     if function_name is not None:
         targetlist = context.get_topic_targets(section, topic, data)
+        # TODO: Verify if this is still the case. @amotl thinks that the
+        #       target address descriptor may be of any type these days.
         if not isinstance(targetlist, list):
             targetlist_type = type(targetlist)
             logger.error(
                 'Topic target definition by function "{function_name}" '
                 'in section "{section}" is empty or incorrect. Should be a list. '
                 "targetlist={targetlist}, type={targetlist_type}".format(**locals())
             )
@@ -273,15 +293,15 @@
         try:
             target = target.format(**data)
             targetlist_resolved.append(target)
         except Exception as ex:
             error = repr(ex)
             logger.error(
                 f"Cannot interpolate transformation data into topic target '{target}': {error}. "
-                f"section={section}, topic={topic}, payload={payload}, data={data}"
+                f"section={section}, topic={topic}, payload={truncate(payload)}, data={data}"
             )
     targetlist = targetlist_resolved
 
     for item in targetlist:
         logger.debug("Message on %s going to %s" % (topic, item))
         # Each target is either "service" or "service:target"
         # If no target specified then notify ALL targets
@@ -297,108 +317,121 @@
                 continue
 
         # skip targets with invalid services
         if service not in service_plugins:
             logger.error("Invalid configuration: Topic '%s' points to non-existing service '%s'" % (topic, service))
             continue
 
+        service_config = context.get_service_config(service)
+        payload_out: t.Union[str, bytes]
+        if asbool(service_config.get("decode_utf8", True)) and isinstance(payload, bytes):
+            payload_out = payload.decode("utf-8")
+        else:
+            payload_out = payload
+
         sendtos = None
         if target is None:
             sendtos = context.get_service_targets(service)
         else:
             sendtos = [target]
 
         for sendto in sendtos:
             logger.debug("New `%s:%s' job: %s" % (service, sendto, topic))
-            job = Job(1, service, section, topic, payload, data, sendto)
+            job = Job(1, service, section, topic, payload_out, data, sendto)
             q_in.put(job)
 
 
-def builtin_transform_data(topic, payload):
+def builtin_transform_data(topic: str, payload: t.AnyStr) -> TdataType:
     """Return a dict with initial transformation data which is made
     available to all plugins"""
 
-    tdata = {}
+    tdata: TdataType = {}
     dt = datetime.now()
 
     tdata["topic"] = topic
     tdata["payload"] = payload
     tdata["_dtepoch"] = int(time.time())  # 1392628581
     tdata["_dtiso"] = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%fZ")  # 2014-02-17T10:38:43.910691Z
     tdata["_ltiso"] = datetime.now().isoformat()  # local time in iso format
     tdata["_dthhmm"] = dt.strftime("%H:%M")  # 10:16
     tdata["_dthhmmss"] = dt.strftime("%H:%M:%S")  # hhmmss=10:16:21
 
     return tdata
 
 
-def xform(function, orig_value, transform_data):
+def xform(function: str, orig_value: t.Any, transform_data: TdataType) -> t.Union[TdataType, str, None]:
     """
     Attempt transformation on orig_value.
 
     - 1st. function()
     - 2nd. inline {xxxx}
     """
 
     if orig_value is None:
         return None
 
     res = orig_value
 
     if function is not None:
-        function_name = sanitize_function_name(function)
-        if function_name is not None:
+        try:
+            function_name = sanitize_function_name(function)
             try:
                 res = context.invoker.datamap(function_name, transform_data)
                 return res
             except Exception:
-                logger.exception(f"Invoking function '{function_name}' failed")
+                logger.exception(f"Invoking function '{function}' failed")
+        except:
+            pass
 
         try:
             res = Formatter().format(function, **transform_data)
         except Exception:
             logger.exception(f"Formatting message with function '{function}' failed")
 
     if isinstance(res, str):
         res = res.replace("\\n", "\n")
 
     return res
 
 
-def decode_payload(section, topic, payload):
+def decode_payload(section: str, topic: str, payload: t.AnyStr) -> TdataType:
     """
     Decode message payload through transformation machinery.
     """
 
     transform_data = builtin_transform_data(topic, payload)
 
-    topic_data = context.get_topic_data(section, topic)
+    topic_data = context.get_topic_data(section, transform_data)
     if topic_data is not None and isinstance(topic_data, dict):
         transform_data.update(topic_data)
 
     # The dict returned is completely merged into transformation data
     # The difference between this and `get_topic_data()' is that this
     # function obtains the topic string as well as the payload and any
     # existing transformation data, and it can do 'things' with all.
     # This is the way it should originally have been, but I can no
     # longer fix the original (legacy).
 
     all_data = context.get_all_data(section, topic, transform_data)
     if all_data is not None and isinstance(all_data, dict):
         transform_data.update(all_data)
 
-    # Attempt to decode the payload from JSON. If it's possible, add
-    # the JSON keys into item to pass to the plugin, and create the
-    # outgoing (i.e. transformed) message.
+    # Gracefully attempt to decode the payload from JSON. If it's possible, add
+    # the JSON keys into item to pass to the plugin, and create the outgoing
+    # (i.e. transformed) message.
     try:
-        payload = payload.rstrip("\0")
-        payload_data = json.loads(payload)
+        if isinstance(payload, bytes):
+            outdata = payload.decode("utf-8")
+        else:
+            outdata = payload
+        outdata = outdata.rstrip("\0")
+        payload_data = json.loads(outdata)
         transform_data.update(payload_data)
     except Exception as ex:
-        logger.debug(f"Cannot decode JSON object, payload={payload}: {ex}")
+        logger.debug(f"Decoding JSON failed: {ex}. payload={truncate(payload)}")
 
     return transform_data
 
 
 def processor(worker_id=None):
     """
     Queue runner. Pull a job from the queue, find the module in charge
@@ -763,15 +796,15 @@
     invoker = FunctionInvoker(config=config, srv=make_service(mqttc=None, name="mqttwarn.context"))
     context = RuntimeContext(config=config, invoker=invoker)
     cf = config
     if scriptname is not None:
         SCRIPTNAME = scriptname
 
 
-def run_plugin(config=None, name=None, options=None):
+def run_plugin(config=None, name=None, options=None, data=None):
     """
     Run service plugins directly without the
     dispatching and transformation machinery.
 
     On the one hand, this might look like a bit of a hack.
     On the other hand, it shows very clearly how some of
     the innards of mqttwarn interact so it might also please
@@ -796,15 +829,15 @@
 
     # Build a mimikry item instance for feeding to the service plugin
     item = Struct(**options)
     # TODO: Read configuration optionally from data.
     item.config = config.config("config:" + name)
     item.service = srv
     item.target = "mqttwarn"
-    item.data = {}  # FIXME
+    item.data = data or {}
 
     # Launch plugin
     module = service_plugins[name]["module"]
     response = module.plugin(srv, item)
     logger.info("Plugin response: {}".format(response))
     if response is False:
         sys.exit(1)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/cron.py` & `mqttwarn-0.34.0/mqttwarn/cron.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 # -*- coding: utf-8 -*-
-# (c) 2014-2022 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
 import logging
 import threading
+import typing as t
+
+from mqttwarn.model import Service
 
 logger = logging.getLogger(__name__)
 
 
 # This class, shamelessly stolen from https://gist.github.com/cypreess/5481681
 # The `srv` bits are added for mqttwarn
 class PeriodicThread:
     """
     Python periodic Thread using Timer with instant cancellation
     """
 
-    def __init__(self, callback=None, period=1, name=None, srv=None, now=False, *args, **kwargs):
+    def __init__(
+        self,
+        callback: t.Optional[t.Callable] = None,
+        period: t.Optional[int] = 1,
+        name: t.Optional[str] = None,
+        srv: t.Optional[Service] = None,
+        now: t.Optional[bool] = False,
+        *args,
+        **kwargs,
+    ):
         self.name = name
         self.srv = srv
         self.now = now
         self.args = args
         self.kwargs = kwargs
         self.callback = callback
         self.period = period
```

### Comparing `mqttwarn-0.33.0/mqttwarn/examples/basic/mqttwarn.ini` & `mqttwarn-0.34.0/mqttwarn/examples/basic/mqttwarn.ini`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,16 @@
 ;logformat = '%(asctime)-15s %(levelname)-8s [%(name)-25s] %(message)s'
 
 
 ; --------
 ; Services
 ; --------
 
-; path to file containing self-defined functions for formatmap and datamap
-functions = 'samplefuncs.py'
+; path to file containing self-defined functions like `format` or `alldata`
+functions = 'udf.py'
 
 ; name the service providers you will be using.
 launch    = file, log
 
 ; Publish mqttwarn status information (retained)
 status_publish = True
 ; status_topic = mqttwarn/$SYS
```

### Comparing `mqttwarn-0.33.0/mqttwarn/examples/basic/samplefuncs.py` & `mqttwarn-0.34.0/mqttwarn/examples/basic/udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # mqttwarn example function extensions
 import time
 import copy
 
 try:
     import json
 except ImportError:
-    import simplejson as json
+    import simplejson as json  # type: ignore[no-redef]
 
 def OwnTracksTopic2Data(topic):
     try:
         # owntracks/username/device
         parts = topic.split('/')
         username = parts[1]
         deviceid = parts[2]
```

### Comparing `mqttwarn-0.33.0/mqttwarn/model.py` & `mqttwarn-0.34.0/mqttwarn/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 # -*- coding: utf-8 -*-
-# (c) 2021-2022 The mqttwarn developers
+# (c) 2021-2023 The mqttwarn developers
 import dataclasses
 import platform
 import sys
+import typing as t
 from dataclasses import dataclass, field
 from functools import total_ordering
-from typing import Dict, List, Optional, Union
+from logging import Logger
+from typing import Dict, Optional, Union
 
 from mqttwarn import __version__
 
+# Type definitions.
+
+# The venerable transformation data dictionary.
+TdataType = t.Dict[str, t.Union[t.AnyStr, int]]
+
+# Covering old- and new-style configuration layouts. `addrs` has
+# originally been a list of strings, has been expanded to be a
+# list of dictionaries (Apprise), to be a dictionary (Pushsafer),
+# and finally to be a scalar string only (ntfy).
+TopicTargetType = t.Union[t.List, t.Dict[str, t.Any], str, None]
+
 
 class Struct:
     """
     Data container for feeding information into service plugins - V1.
     """
 
     # Convert Python dict to object?
@@ -33,39 +46,37 @@
     def enum(self):
         item = {}
         for (k, v) in list(self.__dict__.items()):
             item[k] = v
         return item
 
 
-# Covering old- and new-style configuration layouts. `addrs` has
-# originally been a list of strings, has been expanded to be a
-# list of dictionaries (Apprise), and to be a dictionary (Pushsafer).
-addrs_type = Union[List[Union[str, Dict[str, str]]], Dict[str, str]]
-
-
 @dataclass
 class ProcessorItem:
     """
     Data container for feeding information into service plugins - V2.
     """
 
     service: Optional[str] = None
     target: Optional[str] = None
     config: Dict = field(default_factory=dict)
-    addrs: addrs_type = field(default_factory=list)  # type: ignore[assignment]
+    # TODO: `addrs` can also be a string or dictionary now.
+    addrs: TopicTargetType = field(default_factory=list)  # type: ignore[assignment]
     priority: Optional[int] = None
     topic: Optional[str] = None
     title: Optional[str] = None
     message: Optional[Union[str, bytes]] = None
     data: Optional[Dict] = None
 
     def asdict(self):
         return dataclasses.asdict(self)
 
+    def get(self, key, default=None):
+        return getattr(self, key, default)
+
 
 @dataclasses.dataclass
 class StatusInformation:
     """
     Different bits of information published to `mqttwarn/$SYS` when the `status_publish` feature is enabled.
     """
 
@@ -84,15 +95,15 @@
         # Reference to MQTT client object.
         self.mqttc = mqttc
 
         # Reference to all mqttwarn globals, for using its machinery from plugins.
         self.mwcore = mwcore
 
         # Reference to logging object.
-        self.logging = logger
+        self.logging: Logger = logger  # type: ignore[annotation-unchecked]
 
         # Name of self ("mqttwarn", mostly).
         self.SCRIPTNAME = program
 
 
 @total_ordering
 class Job:
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/alexa-notify-me.py` & `mqttwarn-0.34.0/mqttwarn/services/alexa-notify-me.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/amqp.py` & `mqttwarn-0.34.0/mqttwarn/services/amqp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/apns.py` & `mqttwarn-0.34.0/mqttwarn/services/apns.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 # -*- coding: utf-8 -*-
 
 __author__ = 'Jan-Piet Mens <jpmens()gmail.com>'
 __copyright__ = 'Copyright 2014 Jan-Piet Mens'
 __license__ = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
 import json
-from apns import APNs, Payload
+try:
+    from apns import APNs, Payload
+except:
+    pass
 
 
 def plugin(srv, item):
     addrs = item.addrs
     data = item.data
     text = item.message
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/apprise_multi.py` & `mqttwarn-0.34.0/mqttwarn/services/apprise_multi.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
         for address in addresses:
             baseuri = address["baseuri"]
 
             # Collect URL parameters.
             params = OrderedDict()
 
-            # Obtain and apply all possible Ntfy parameters from data dictionary.
+            # Obtain and apply all possible Apprise parameters from data dictionary.
             params.update(obtain_apprise_arguments(item, APPRISE_ALL_ARGUMENT_NAMES))
 
             # Apply addressee information.
             if "recipients" in address:
                 to = ','.join(address["recipients"])
                 if to:
                     params["to"] = to
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/apprise_single.py` & `mqttwarn-0.34.0/mqttwarn/services/apprise_single.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
         # Create an Apprise instance.
         apobj = apprise.Apprise(asset=apprise.AppriseAsset(async_mode=False))
 
         # Collect URL parameters.
         params = OrderedDict()
 
-        # Obtain and apply all possible Ntfy parameters from data dictionary.
+        # Obtain and apply all possible Apprise parameters from data dictionary.
         params.update(obtain_apprise_arguments(item, APPRISE_ALL_ARGUMENT_NAMES))
 
         # Apply addressee information.
         if sender:
             params["from"] = sender
         if to:
             params["to"] = to
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/apprise_util.py` & `mqttwarn-0.34.0/mqttwarn/services/apprise_util.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,14 @@
 
     return sorted(set(all_arg_names))
 
 
 def obtain_apprise_arguments(item: ProcessorItem, arg_names: list) -> dict:
     """
     Obtain eventual Apprise parameters from data dictionary.
-
-    https://github.com/caronc/apprise/wiki/Notify_ntfy#parameter-breakdown
     """
     params = dict()
     for arg_name in arg_names:
         if isinstance(item.data, dict) and arg_name in item.data:
             params[arg_name] = item.data[arg_name]
     return params
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/asterisk.py` & `mqttwarn-0.34.0/mqttwarn/services/asterisk.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/autoremote.py` & `mqttwarn-0.34.0/mqttwarn/services/autoremote.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/azure_iot.py` & `mqttwarn-0.34.0/mqttwarn/services/azure_iot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/carbon.py` & `mqttwarn-0.34.0/mqttwarn/services/carbon.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/celery.py` & `mqttwarn-0.34.0/mqttwarn/services/celery.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/chromecast.py` & `mqttwarn-0.34.0/mqttwarn/services/chromecast.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/dbus.py` & `mqttwarn-0.34.0/mqttwarn/services/dbus.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/desktopnotify.py` & `mqttwarn-0.34.0/mqttwarn/services/desktopnotify.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,44 +3,48 @@
 
 __author__    = 'Alexander Gräf <portalzine.projects()gmail.com>'
 __copyright__ = 'Copyright 2022 Alexander Gräf'
 __version__   = '1.0.0'
 __license__   = 'Eclipse Public License - v 2.0 - https://www.eclipse.org/legal/epl-2.0/'
 
 import json
+import typing as t
+
 from desktop_notifier import DesktopNotifier, Urgency, Button, ReplyField
 
+from mqttwarn.model import Service, ProcessorItem, Struct
+
 notify = DesktopNotifier()
 
-def is_json(msg):
+def is_json(msg: t.Union[str, bytes]) -> bool:
    try:
      json.loads(msg)
    except ValueError as e:
      return False
    return True
 
-def plugin(srv, item):
+def plugin(srv: Service, item: ProcessorItem):
     # Log
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
 
     # Load Config
     config = item.config
 
     # Play Sound ?
     playSound = True
     if isinstance(config, dict):
        playSound = config.get('sound', True)
 
     # Get Message
     message = item.message
-    if is_json(message) == True:
+    if message and is_json(message):
        data = json.loads(message)
     else:
        data = {
-         "title"  : item.get('title',item.topic),
+         "title"  : item.get('title', item.topic),
          "message": message
        }
 
     srv.logging.debug("Sending desktop notification")
     try:
         # Synchronous Notification (allows no callbacks in OSX)
         # Asynchronous would require asyncio and require some changes to the plugin handler
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/dnsupdate.py` & `mqttwarn-0.34.0/mqttwarn/services/dnsupdate.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/emoncms.py` & `mqttwarn-0.34.0/mqttwarn/services/emoncms.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from builtins import str
 
 import urllib.request, urllib.parse, urllib.error
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     """ addrs: (node, name) """
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/execute.py` & `mqttwarn-0.34.0/mqttwarn/services/execute.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/fbchat.py` & `mqttwarn-0.34.0/mqttwarn/services/fbchat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/file.py` & `mqttwarn-0.34.0/mqttwarn/services/file.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,17 +50,23 @@
     text = item.message
 
     if newline:
         text += "\n"
     if overwrite:
         mode = "w"
 
+    if isinstance(text, bytes):
+        mode += "b"
+        encoding = None
+    else:
+        encoding = "utf-8"
+
     try:
-        f = io.open(filename, mode, encoding='utf-8')
+        f = io.open(filename, mode=mode, encoding=encoding)
         f.write(text)
         f.close()
 
     except Exception as e:
-        srv.logging.warning("Cannot write to file `%s': %s" % (filename, e))
+        srv.logging.error("Cannot write to file `%s': %s" % (filename, e))
         return False
 
     return True
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/freeswitch.py` & `mqttwarn-0.34.0/mqttwarn/services/freeswitch.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/gss.py` & `mqttwarn-0.34.0/mqttwarn/services/gss.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 __copyright__ = 'Copyright 2014 Jan Badenhorst'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
 from builtins import str
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 import gdata.spreadsheet.service
 
 
 def plugin(srv, item):
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/gss2.py` & `mqttwarn-0.34.0/mqttwarn/services/gss2.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
 import os
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 import gspread
 import oauth2client.client
 import oauth2client.file
 from oauth2client import clientsecrets
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/hangbot.py` & `mqttwarn-0.34.0/mqttwarn/services/hangbot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/hipchat.py` & `mqttwarn-0.34.0/mqttwarn/services/hipchat.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 standard_library.install_aliases()
 from builtins import str
 
 import urllib.request, urllib.parse, urllib.error
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     """ addrs: (token, roomid, color, notify) """
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/http_urllib.py` & `mqttwarn-0.34.0/mqttwarn/services/http_urllib.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import urllib.request, urllib.parse, urllib.error
 import base64
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     """ addrs: (method, url, dict(params), list(username, password), json) """
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/icinga2.py` & `mqttwarn-0.34.0/mqttwarn/services/icinga2.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
 
     host = item.config['host']
     port = item.config['port']
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/ifttt.py` & `mqttwarn-0.34.0/mqttwarn/services/ifttt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/influxdb.py` & `mqttwarn-0.34.0/mqttwarn/services/influxdb.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/ionic.py` & `mqttwarn-0.34.0/mqttwarn/services/ionic.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import urllib.request, urllib.error, urllib.parse
 import base64
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     # item.addrs is an array with three or more elements:
     # 0 is the Ionic appid
     # 1 is the Ionic appsecret (private key)
     # 2..N are the push tokens returned by Ionic push service
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/irccat.py` & `mqttwarn-0.34.0/mqttwarn/services/irccat.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/linuxnotify.py` & `mqttwarn-0.34.0/mqttwarn/services/linuxnotify.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/log.py` & `mqttwarn-0.34.0/mqttwarn/services/log.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mattermost.py` & `mqttwarn-0.34.0/mqttwarn/services/mattermost.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from six import string_types
 
 import requests
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
 
     hook_url = item.addrs[0]
     channel = item.addrs[1]
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mqtt.py` & `mqttwarn-0.34.0/mqttwarn/services/mqtt.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mqtt_filter.py` & `mqttwarn-0.34.0/mqttwarn/services/mqtt_filter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mqttpub.py` & `mqttwarn-0.34.0/mqttwarn/services/mqttpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mysql.py` & `mqttwarn-0.34.0/mqttwarn/services/mysql.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mysql_dynamic.py` & `mqttwarn-0.34.0/mqttwarn/services/mysql_dynamic.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mysql_remap.py` & `mqttwarn-0.34.0/mqttwarn/services/mysql_remap.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/mythtv.py` & `mqttwarn-0.34.0/mqttwarn/services/mythtv.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/nntp.py` & `mqttwarn-0.34.0/mqttwarn/services/nntp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/nsca.py` & `mqttwarn-0.34.0/mqttwarn/services/nsca.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/osxsay.py` & `mqttwarn-0.34.0/mqttwarn/services/osxsay.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pastebinpub.py` & `mqttwarn-0.34.0/mqttwarn/services/pastebinpub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pipe.py` & `mqttwarn-0.34.0/mqttwarn/services/pipe.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/postgres.py` & `mqttwarn-0.34.0/mqttwarn/services/postgres.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/prowl.py` & `mqttwarn-0.34.0/mqttwarn/services/prowl.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pushalot.py` & `mqttwarn-0.34.0/mqttwarn/services/pushalot.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pushbullet.py` & `mqttwarn-0.34.0/mqttwarn/services/pushbullet.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pushover.py` & `mqttwarn-0.34.0/mqttwarn/services/pushover.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/pushsafer.py` & `mqttwarn-0.34.0/mqttwarn/services/pushsafer.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/redispub.py` & `mqttwarn-0.34.0/mqttwarn/services/redispub.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/rrdtool.py` & `mqttwarn-0.34.0/mqttwarn/services/rrdtool.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/serial.py` & `mqttwarn-0.34.0/mqttwarn/services/serial.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/slack.py` & `mqttwarn-0.34.0/mqttwarn/services/slack.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/slixmpp.py` & `mqttwarn-0.34.0/mqttwarn/services/slixmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/smtp.py` & `mqttwarn-0.34.0/mqttwarn/services/smtp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/sqlite.py` & `mqttwarn-0.34.0/mqttwarn/services/sqlite.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/sqlite_json2cols.py` & `mqttwarn-0.34.0/mqttwarn/services/sqlite_json2cols.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/sqlite_timestamp.py` & `mqttwarn-0.34.0/mqttwarn/services/sqlite_timestamp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/ssh.py` & `mqttwarn-0.34.0/mqttwarn/services/ssh.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/syslog.py` & `mqttwarn-0.34.0/mqttwarn/services/syslog.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/telegram.py` & `mqttwarn-0.34.0/mqttwarn/services/telegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from builtins import str
 from builtins import object
 import requests
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
     """
     addrs: (tg_contact, token, text)
     """
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/thingspeak.py` & `mqttwarn-0.34.0/mqttwarn/services/thingspeak.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/tootpaste.py` & `mqttwarn-0.34.0/mqttwarn/services/tootpaste.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/twilio.py` & `mqttwarn-0.34.0/mqttwarn/services/twilio.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/twitter.py` & `mqttwarn-0.34.0/mqttwarn/services/twitter.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/websocket.py` & `mqttwarn-0.34.0/mqttwarn/services/websocket.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/xbmc.py` & `mqttwarn-0.34.0/mqttwarn/services/xbmc.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 standard_library.install_aliases()
 
 import urllib.request, urllib.parse, urllib.error
 import base64
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 
 
 def plugin(srv, item):
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
 
     xbmchost = item.addrs[0]
```

### Comparing `mqttwarn-0.33.0/mqttwarn/services/xively.py` & `mqttwarn-0.34.0/mqttwarn/services/xively.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/xmpp.py` & `mqttwarn-0.34.0/mqttwarn/services/xmpp.py`

 * *Files identical despite different names*

### Comparing `mqttwarn-0.33.0/mqttwarn/services/zabbix.py` & `mqttwarn-0.34.0/mqttwarn/services/zabbix.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __author__    = 'Jan-Piet Mens <jpmens()gmail.com>'
 __copyright__ = 'Copyright 2014 Jan-Piet Mens'
 __license__   = 'Eclipse Public License - v 1.0 (http://www.eclipse.org/legal/epl-v10.html)'
 
 try:
     import simplejson as json
 except ImportError:
-    import json
+    import json  # type: ignore[no-redef]
 from mqttwarn.vendor import ZabbixSender
 import time
 
 
 def plugin(srv, item):
 
     srv.logging.debug("*** MODULE=%s: service=%s, target=%s", __file__, item.service, item.target)
```

### Comparing `mqttwarn-0.33.0/mqttwarn/util.py` & `mqttwarn-0.34.0/mqttwarn/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,34 @@
-# -*- coding: utf-8 -*-
-# (c) 2014-2022 The mqttwarn developers
+# (c) 2014-2023 The mqttwarn developers
+import functools
 import hashlib
 import imp
 import json
+import logging
 import os
 import re
 import string
+import types
+import typing as t
 
+import funcy
 import pkg_resources
 from six import string_types
 
+logger = logging.getLogger(__name__)
+
 
 class Formatter(string.Formatter):
     """
     A custom string formatter. See also:
     - https://docs.python.org/2/library/string.html#format-string-syntax
     - https://docs.python.org/2/library/string.html#custom-string-formatting
     """
 
-    def convert_field(self, value, conversion):
+    def convert_field(self, value: str, conversion: str) -> str:
         """
         The conversion field causes a type coercion before formatting.
         By default, two conversion flags are supported: '!s' which calls
         str() on the value, and '!r' which calls repr().
 
         This also adds the '!j' conversion flag, which serializes the
         value to JSON format.
@@ -30,15 +36,15 @@
         See also https://github.com/jpmens/mqttwarn/issues/146.
         """
         if conversion == "j":
             value = json.dumps(value)
         return value
 
 
-def asbool(obj):
+def asbool(obj: t.Any) -> bool:
     """
     Shamelessly stolen from beaker.converters
     # (c) 2005 Ian Bicking and contributors; written for Paste (http://pythonpaste.org)
     # Licensed under the MIT license: http://www.opensource.org/licenses/mit-license.php
     """
     if isinstance(obj, string_types):
         obj = obj.strip().lower()
@@ -47,38 +53,38 @@
         elif obj in ["false", "no", "off", "n", "f", "0"]:
             return False
         else:
             raise ValueError("String is not true/false: %r" % obj)
     return bool(obj)
 
 
-def parse_cron_options(argstring):
+def parse_cron_options(argstring: str) -> t.Dict[str, t.Union[str, float]]:
     """
     Parse periodic task options.
     Obtains configuration value, returns dictionary.
 
     Example::
 
         my_periodic_task = 60; now=true
 
     Respective "argstring"::
 
         60; now=true
 
     """
     parts = argstring.split(";")
-    options = {"interval": float(parts[0].strip())}
+    options: t.Dict[str, t.Union[str, float]] = {"interval": float(parts[0].strip())}
     for part in parts[1:]:
         name, value = part.split("=")
         options[name.strip()] = value.strip()
     return options
 
 
 # http://code.activestate.com/recipes/473878-timeout-function-using-threading/
-def timeout(func, args=(), kwargs={}, timeout_secs=10, default=False):
+def timeout(func: t.Callable, args=(), kwargs={}, timeout_secs: int = 10, default: bool = False) -> t.Any:
     import threading
 
     class InterruptableThread(threading.Thread):
         def __init__(self):
             threading.Thread.__init__(self)
             self.result = None
             self.exception = None
@@ -101,83 +107,83 @@
 
     if it.is_alive():
         return default
     else:
         return it.result
 
 
-def sanitize_function_name(s):
-    func = None
+def sanitize_function_name(name: str) -> str:
+    if name is None:
+        raise ValueError(f"Empty function name: {name}")
 
-    if s is not None:
-        try:
-            valid = re.match(r"^[\w]+\(\)", s)
-            if valid is not None:
-                func = re.sub("[()]", "", s)
-        except:
-            pass
-    return func
+    try:
+        valid = re.match(r"^[\w]+\(\)", name)
+        if valid is not None:
+            return re.sub("[()]", "", name)
+    except:
+        pass
+    raise ValueError(f"Invalid function name: {name}")
 
 
-def load_module_from_file(path):
+def load_module_from_file(path: str) -> types.ModuleType:
     """
     http://code.davidjanes.com/blog/2008/11/27/how-to-dynamically-load-python-code/
 
     :param path:
     :return:
     """
     try:
         fp = open(path, "rb")
         digest = hashlib.md5(path.encode("utf-8")).hexdigest()
-        return imp.load_source(digest, path, fp)
+        return imp.load_source(digest, path, fp)  # type: ignore[arg-type]
     finally:
         try:
             fp.close()
         except:
             pass
 
 
-def load_module_by_name(name):
+def load_module_by_name(name: str) -> types.ModuleType:
     """
     https://pymotw.com/2/imp/#loading-modules
 
     :param name:
     :return:
     """
     module = import_module(name)
     return module
 
 
-def import_module(name, path=None):
+def import_module(name: str, path: t.Optional[t.List[str]] = None) -> types.ModuleType:
     """
     Derived from `import_from_dotted_path`:
     https://chase-seibert.github.io/blog/2014/04/23/python-imp-examples.html
 
     import_from_dotted_path('foo.bar') -> from foo import bar; return bar
     """
 
     try:
         next_module, remaining_names = name.split(".", 1)
     except ValueError:
         next_module = name
         remaining_names = None
 
     fp, pathname, description = imp.find_module(next_module, path)
-    module = imp.load_module(next_module, fp, pathname, description)
+    module = imp.load_module(next_module, fp, pathname, description)  # type: ignore[arg-type]
 
     if remaining_names is None:
         return module
 
     if hasattr(module, remaining_names):
         return getattr(module, remaining_names)
     else:
-        return import_module(remaining_names, path=module.__path__)
+        return import_module(remaining_names, path=list(module.__path__))
 
 
-def load_functions(filepath=None):
+def load_functions(filepath: t.Optional[str] = None) -> t.Optional[types.ModuleType]:
 
     if not filepath:
         return None
 
     if not os.path.isfile(filepath):
         raise IOError("'{}' not found".format(filepath))
 
@@ -191,22 +197,53 @@
 
     else:
         raise ValueError("'{}' does not have the .py or .pyc extension".format(filepath))
 
     return py_mod
 
 
-def load_function(name=None, py_mod=None):
+def load_function(name: str, py_mod: t.Optional[types.ModuleType]) -> t.Callable:
     assert name, "Function name must be given"
     assert py_mod, "Python module must be given"
 
     func = getattr(py_mod, name, None)
 
     if func is None:
         raise AttributeError("Function '{}' does not exist in '{}'".format(name, py_mod.__file__))
 
     return func
 
 
-def get_resource_content(package, filename):
+def get_resource_content(package: str, filename: str) -> str:
     with pkg_resources.resource_stream(package, filename) as stream:
         return stream.read().decode("utf-8")
+
+
+def truncate(s: t.Union[str, bytes], limit: int = 200, ellipsis="...") -> str:
+    try:
+        if isinstance(s, bytes):
+            s = s.decode("utf-8")
+    except UnicodeDecodeError:
+        pass
+    s = str(s)
+    s = s.strip()
+    if len(s) > limit:
+        return s[:limit].strip() + ellipsis
+    return s
+
+
+def load_file(path: str, retry_tries=None, retry_interval=0.075, unlink=False) -> t.IO[bytes]:
+    """
+    Load file content from filesystem gracefully, with optional retrying.
+    """
+    call = functools.partial(open, path, "rb")
+    if retry_tries:
+        logger.info(f"Retry loading file {path} for {retry_tries} times")
+        payload = funcy.retry(tries=int(retry_tries), timeout=float(retry_interval))(call)()
+    else:
+        payload = call()
+    if unlink:
+        try:
+            os.unlink(path)
+        except:
+            pass
+    return payload
```

### Comparing `mqttwarn-0.33.0/mqttwarn/vendor/ZabbixSender.py` & `mqttwarn-0.34.0/mqttwarn/vendor/ZabbixSender.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Copyright (C) 2010 Takanori Suzuki
 
 # JPM: s/simplejson/json/g
 
 try:
     import json
 except ImportError:
-    import simplejson as json
+    import simplejson as json  # type: ignore[no-redef]
 
 
 class ZabbixSender:
     
     zbx_header = b'ZBXD'
     zbx_version = 1
     zbx_sender_data = {u'request': u'sender data', u'data': []}
```

### Comparing `mqttwarn-0.33.0/mqttwarn.egg-info/PKG-INFO` & `mqttwarn-0.34.0/mqttwarn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqttwarn
-Version: 0.33.0
+Version: 0.34.0
 Summary: mqttwarn - subscribe to MQTT topics and notify pluggable services
 Home-page: https://github.com/jpmens/mqttwarn
 Author: Jan-Piet Mens, Ben Jones, Andreas Motl
 Author-email: jpmens@gmail.com
 License: EPL 2.0
 Keywords: mqtt notification plugins data acquisition push transformation engine mosquitto
 Classifier: Development Status :: 4 - Beta
@@ -90,25 +90,22 @@
 .. image:: https://img.shields.io/pypi/pyversions/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/v/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/l/mqttwarn.svg
-    :alt: License
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://img.shields.io/pypi/status/mqttwarn.svg
     :target: https://pypi.org/project/mqttwarn/
 
 .. image:: https://pepy.tech/badge/mqttwarn/month
     :target: https://pepy.tech/project/mqttwarn
 
-|
-
 .. image:: https://cloud.githubusercontent.com/assets/2345521/6320105/4dd7a826-bade-11e4-9a61-72aa163a40a9.png
 
 
 ########
 mqttwarn
 ########
 
@@ -134,104 +131,79 @@
 
 A picture says a thousand words.
 
 .. image:: https://raw.githubusercontent.com/jpmens/mqttwarn/main/assets/mqttwarn.png
     :target: #
 
 
-Coverage
-========
+Notification service coverage
+=============================
 
 *mqttwarn* comes with **over 70 notification handler plugins** for a wide
 range of notification services and is very open to further contributions.
-You can enjoy the alphabetical list of plugins at `mqttwarn notification
-services`_.
+You can enjoy the alphabetical list of plugins on the `mqttwarn notifier
+catalog`_ page.
 
 On top of that, it integrates with the excellent `Apprise`_ notification
 library. `Apprise notification services`_ has a complete list of the **80+
 notification services** supported by Apprise.
 
 
-Details
-=======
-
-The program, running as a service, subscribes to any number of MQTT topics
-(including wildcards) and publishes received payloads to one or more notification
-services, including support for notifying more than one distinct service
-for the same message.
-
-Notifications are transmitted to the appropriate service via plugins.
-*mqttwarn* provides built-in plugins for a number of services and you
-can easily add your own.
-
-A more detailed blog post about what mqttwarn can be used for is available
-at `How do your servers talk to you?`_.
-
-For example, you may wish to submit an alarm published as text to the
-MQTT topic ``home/monitoring/+`` as notification via *e-mail* and *Pushover*.
-
-
 
 *************
 Documentation
 *************
 
-The `handbook`_ is the right place to read all about *mqttwarn*'s features and
-service plugins.
+The `mqttwarn documentation`_ is the right place to read all about *mqttwarn*'s
+features and integrations, and how you can leverage all its framework components
+for building custom applications. Its service plugins can be inspected on the
+`mqttwarn notifier catalog`_ page.
 
 
 ************
 Installation
 ************
 
+Using pip
+=========
+
 Synopsis::
 
     pip install --upgrade mqttwarn
 
 You can also add support for a specific service plugin::
 
     pip install --upgrade 'mqttwarn[xmpp]'
 
 You can also add support for multiple services, all at once::
 
     pip install --upgrade 'mqttwarn[apprise,asterisk,nsca,desktopnotify,tootpaste,xmpp]'
 
+See also: `Installing mqttwarn with pip`_.
 
-***************
-Container image
-***************
+OCI container image
+===================
 
 For running ``mqttwarn`` on a container infrastructure like Docker or
 Kubernetes, corresponding images are automatically published to the
 GitHub Container Registry (GHCR).
 
 - ``ghcr.io/jpmens/mqttwarn-standard:latest``
 - ``ghcr.io/jpmens/mqttwarn-full:latest``
 
-To learn more about this topic, please follow up reading the `Docker handbook`_.
+To learn more about this topic, please follow up reading the `Using the OCI image
+with Docker or Podman`_ documentation section.
 
 
 *************
 Configuration
 *************
 
-First, create configuration and custom Python starter files
-``mqttwarn.ini`` and ``samplefuncs.py`` and edit them to your taste::
-
-    # Create configuration file
-    mqttwarn make-config > mqttwarn.ini
-
-    # Create file for custom functions
-    mqttwarn make-samplefuncs > samplefuncs.py
-
-If you are using PowerShell on Windows 10, you may find the files to be written
-using the ``UTF-16`` charset encoding. However, ``mqttwarn`` works with ``UTF-8``.
-In order to switch to ``UTF-8``, please invoke this command beforehand::
-
-    $PSDefaultParameterValues['Out-File:Encoding'] = 'utf8'
+In order to learn how to configure mqttwarn, please head over to the documentation
+section about the `mqttwarn configuration`_.
 
 
 *****
 Usage
 *****
 
 Running interactively
@@ -268,142 +240,142 @@
 
     # Launch "file" service plugin
     mqttwarn --plugin=file --options='{"message": "Hello world\n", "addrs": ["/tmp/mqttwarn.err"]}'
 
     # Launch "pushover" service plugin
     mqttwarn --plugin=pushover --options='{"title": "About", "message": "Hello world", "addrs": ["userkey", "token"], "priority": 6}'
 
-    # Launch "ssh" service plugin from the command line
+    # Launch "ntfy" service plugin
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"tags": "foo,bar,äöü", "priority": "high"}'
+
+    # Launch "ntfy" service plugin, and add remote attachment
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive"}, "title": "Example notification", "message": "Hello world"}' --data='{"attach": "https://unsplash.com/photos/spdQ1dVuIHw/download?w=320", "filename": "goat.jpg"}'
+
+    # Launch "ntfy" service plugin, and add attachment from local filesystem
+    mqttwarn --plugin=ntfy --options='{"addrs": {"url": "http://localhost:5555/testdrive", "file": "goat.jpg"}, "title": "Example notification", "message": "Hello world"}'
+
+    # Launch "ssh" service plugin
     mqttwarn --plugin=ssh --config='{"host": "ssh.example.org", "port": 22, "user": "foo", "password": "bar"}' --options='{"addrs": ["command with substitution %s"], "payload": "{\"args\": \"192.168.0.1\"}"}'
 
-    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib", passing "--config" parameters via command line
+    # Launch "cloudflare_zone" service plugin from "mqttwarn-contrib"
     pip install mqttwarn-contrib
     mqttwarn --plugin=mqttwarn_contrib.services.cloudflare_zone --config='{"auth-email": "foo", "auth-key": "bar"}' --options='{"addrs": ["0815", "www.example.org", ""], "message": "192.168.0.1"}'
 
-    # Submit notification to "ntfy", using Apprise service plugin.
-    mqttwarn --plugin=apprise \
-        --config='{"baseuri": "ntfy://user:password@ntfy.example.org/topic1/topic2"}' \
-        --options='{"addrs": [], "title": "Example notification", "message": "Hello world"}'
-
 
 Also, the ``--config-file`` parameter can be used to optionally specify the
 path to a configuration file.
 
 
 Running as system daemon
 ========================
-- We recommend to use Supervisor_ for running *mqttwarn* as a service, see also `supervisor.ini`_.
-- Alternatively, have a look at `mqttwarn.service`_, the systemd unit configuration file for *mqttwarn*.
 
+There are different ways to run mqttwarn as a system daemon. There are examples
+for systemd, traditional init, OpenRC, and Supervisor_ in the ``etc`` directory
+of this repository, for example `supervisor.ini`_ (Supervisor) and
+`mqttwarn.service`_ (systemd).
 
 Running in a development sandbox
 ================================
-For hacking_ on mqttwarn, please install it in development mode.
 
-
-****************
-Acknowledgements
-****************
-Thanks to all the contributors of *mqttwarn* who got their hands dirty with it
-and helped to co-create and conceive it in one way or another. You know who you are.
+For hacking on mqttwarn, please install it in development mode, using a
+`mqttwarn development sandbox`_ installation.
 
 
 *******************
 Project information
 *******************
 
 About
 =====
 These links will guide you to the source code of *mqttwarn* and its documentation.
 
 - `mqttwarn on GitHub <https://github.com/jpmens/mqttwarn>`_
 - `mqttwarn on the Python Package Index (PyPI) <https://pypi.org/project/mqttwarn/>`_
-- `mqttwarn documentation <https://github.com/jpmens/mqttwarn/tree/main/doc>`_
+- `mqttwarn documentation <https://mqttwarn.readthedocs.io/>`_
 
 
 Requirements
 ============
 You will need at least the following components:
 
 * Python 3.x or PyPy 3.x.
-* An MQTT broker. We recommend Mosquitto_.
-* Some more Python modules to satisfy service dependencies defined in the ``setup.py`` file.
+* An MQTT broker. We recommend `Mosquitto`_.
+* For invoking specific service plugins, additional Python modules may be required.
+  See ``setup.py`` file.
 
 
 Contributing
 ============
+
 We are always happy to receive code contributions, ideas, suggestions
 and problem reports from the community.
 
-So, if you'd like to contribute you're most welcome.
+So, if you would like to contribute, you are most welcome.
 Spend some time taking a look around, locate a bug, design issue or
-spelling mistake and then send us a pull request or create an `issue`_.
+spelling mistake, and then send us a pull request or create an `issue`_.
 
-Thanks in advance for your efforts, we really appreciate any help or feedback.
+Thank you in advance for your efforts, we really appreciate any help or feedback.
 
-There are also some extensions to mqttwarn not included in the core package.
-Yet, they are bundled into another package, ``mqttwarn-contrib``, see also
-`community contributions to mqttwarn`_.
 
+License
+=======
 
-Licenses
-========
-This software is copyright © 2014-2023 Jan-Piet Mens and contributors. All
+mqttwarn is copyright © 2014-2023 Jan-Piet Mens and contributors. All
 rights reserved.
 
 It is and will always be **free and open source software**.
 
 Use of the source code included here is governed by the `Eclipse Public License
 2.0 <EPL-2.0_>`_, see LICENSE_ file for details. Please also recognize the
 licenses of third-party components.
 
 
 ***************
 Troubleshooting
 ***************
+
 If you encounter any problems during setup or operations or if you have further
 suggestions, please let us know by `opening an issue on GitHub`_. Thank you
 already.
 
 
-*************
-Miscellaneous
-*************
-
-
-Press
-=====
-* The article `MQTTwarn: Ein Rundum-Sorglos-Notifier`_ in German at JAXenter.
-* The folks of the Berlin-based beekeeper collective Hiveeyes_ are monitoring their beehives and use *mqttwarn*
-  as a building block for their alert notification system, enjoy reading `Schwarmalarm using mqttwarn`_.
+************
+Attributions
+************
 
+Acknowledgements
+================
+Thanks to all the contributors of *mqttwarn* who helped to conceive it in one
+way or another. You know who you are.
 
 Legal stuff
 ===========
-"MQTT" is a trademark of the OASIS open standards consortium, which publishes the MQTT specifications.
+"MQTT" is a trademark of the OASIS open standards consortium, which publishes
+the MQTT specifications.
 
 
 ----
 
 Have fun!
 
 
 .. _Apprise: https://github.com/caronc/apprise
 .. _Apprise notification services: https://github.com/caronc/apprise/wiki#notification-services
 .. _backlog: https://github.com/jpmens/mqttwarn/blob/main/doc/backlog.rst
-.. _community contributions to mqttwarn: https://pypi.org/project/mqttwarn-contrib/
-.. _Docker handbook: https://github.com/jpmens/mqttwarn/blob/main/DOCKER.md
 .. _EPL-2.0: https://www.eclipse.org/legal/epl-2.0/
 .. _hacking: https://github.com/jpmens/mqttwarn/blob/main/doc/hacking.rst
-.. _handbook: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md
-.. _Hiveeyes: https://hiveeyes.org/
 .. _How do your servers talk to you?: https://jpmens.net/2014/04/03/how-do-your-servers-talk-to-you/
+.. _Installing mqttwarn with pip: https://mqttwarn.readthedocs.io/en/latest/usage/pip.html
 .. _issue: https://github.com/jpmens/mqttwarn/issues/new
 .. _LICENSE: https://github.com/jpmens/mqttwarn/blob/main/LICENSE
 .. _Mosquitto: https://mosquitto.org
 .. _MQTTwarn\: Ein Rundum-Sorglos-Notifier: https://web.archive.org/web/20140611040637/http://jaxenter.de/news/MQTTwarn-Ein-Rundum-Sorglos-Notifier-171312
-.. _mqttwarn notification services: https://github.com/jpmens/mqttwarn/blob/main/HANDBOOK.md#supported-notification-services
+.. _mqttwarn configuration: https://mqttwarn.readthedocs.io/en/latest/configure/
+.. _mqttwarn development sandbox: https://mqttwarn.readthedocs.io/en/latest/workbench/sandbox.html
+.. _mqttwarn documentation: https://mqttwarn.readthedocs.io/
+.. _mqttwarn notifier catalog: https://mqttwarn.readthedocs.io/en/latest/notifier-catalog.html
 .. _mqttwarn.service: https://github.com/jpmens/mqttwarn/blob/main/etc/mqttwarn.service
 .. _opening an issue on GitHub: https://github.com/jpmens/mqttwarn/issues/new
 .. _Schwarmalarm using mqttwarn: https://hiveeyes.org/docs/system/schwarmalarm-mqttwarn.html
 .. _Supervisor: https://jpmens.net/2014/02/13/in-my-toolbox-supervisord/
 .. _supervisor.ini: https://github.com/jpmens/mqttwarn/blob/main/etc/supervisor.ini
+.. _Using the OCI image with Docker or Podman: https://mqttwarn.readthedocs.io/en/latest/usage/oci.html
```

### Comparing `mqttwarn-0.33.0/mqttwarn.egg-info/SOURCES.txt` & `mqttwarn-0.34.0/mqttwarn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 CHANGES.rst
-DOCKER.md
-HANDBOOK.md
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements-release.txt
 setup.py
 mqttwarn/__init__.py
@@ -21,15 +19,15 @@
 mqttwarn.egg-info/dependency_links.txt
 mqttwarn.egg-info/entry_points.txt
 mqttwarn.egg-info/not-zip-safe
 mqttwarn.egg-info/requires.txt
 mqttwarn.egg-info/top_level.txt
 mqttwarn/examples/__init__.py
 mqttwarn/examples/basic/mqttwarn.ini
-mqttwarn/examples/basic/samplefuncs.py
+mqttwarn/examples/basic/udf.py
 mqttwarn/services/__init__.py
 mqttwarn/services/alexa-notify-me.py
 mqttwarn/services/amqp.py
 mqttwarn/services/apns.py
 mqttwarn/services/apprise.py
 mqttwarn/services/apprise_multi.py
 mqttwarn/services/apprise_single.py
@@ -66,14 +64,15 @@
 mqttwarn/services/mqttpub.py
 mqttwarn/services/mysql.py
 mqttwarn/services/mysql_dynamic.py
 mqttwarn/services/mysql_remap.py
 mqttwarn/services/mythtv.py
 mqttwarn/services/nntp.py
 mqttwarn/services/nsca.py
+mqttwarn/services/ntfy.py
 mqttwarn/services/osxsay.py
 mqttwarn/services/pastebinpub.py
 mqttwarn/services/pipe.py
 mqttwarn/services/postgres.py
 mqttwarn/services/prowl.py
 mqttwarn/services/pushalot.py
 mqttwarn/services/pushbullet.py
```

### Comparing `mqttwarn-0.33.0/mqttwarn.egg-info/requires.txt` & `mqttwarn-0.34.0/mqttwarn.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-six<2
-paho-mqtt<2
-jinja2<4
 attrs<23
 docopt<1
-requests<3
+funcy<3
 future<1,>=0.18.0
+jinja2<4
+paho-mqtt<2
+requests<3
+six<2
 
 [:python_version < "3.8"]
 importlib-metadata
 
 [all]
 puka>=0.0.7
 apns>=2.0.1
-apprise<2
+apprise<2,>=1.3
 pyst2>=0.5.0
 celery
 pychromecast>=7.5.0
 dnspython>=1.15.0
 fbchat>=1.3.6
 gdata>=2.0.18
 gspread>=2.1.1
@@ -45,15 +46,15 @@
 [amqp]
 puka>=0.0.7
 
 [apns]
 apns>=2.0.1
 
 [apprise]
-apprise<2
+apprise<2,>=1.3
 
 [asterisk]
 pyst2>=0.5.0
 
 [celery]
 celery
 
@@ -66,16 +67,17 @@
 [desktopnotify]
 desktop-notifier<4
 
 [develop]
 isort<6
 black<23
 build<1
-mypy<1
+mypy<1.3
 poethepoet<1
+sphinx-autobuild
 
 [develop:python_version >= "3.7"]
 ruff==0.0.254
 
 [dnsupdate]
 dnspython>=1.15.0
 
@@ -135,15 +137,15 @@
 pytest-mqtt<1
 tox<4
 requests-toolbelt<1,>=0.9.1
 responses<1,>=0.13.3
 pyfakefs<5,>=4.5
 puka>=0.0.7
 apns>=2.0.1
-apprise<2
+apprise<2,>=1.3
 pyst2>=0.5.0
 celery
 pychromecast>=7.5.0
 dnspython>=1.15.0
 fbchat>=1.3.6
 gdata>=2.0.18
 gspread>=2.1.1
```

### Comparing `mqttwarn-0.33.0/pyproject.toml` & `mqttwarn-0.34.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -63,26 +63,36 @@
   "mqttwarn/examples",
   "mqttwarn/services",
   "mqttwarn/vendor",
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
+exclude = [
+  "tests/etc/functions_bad.py",
+]
+files = [
+  "examples/**/*.py",
+  "mqttwarn/**/*.py",
+  "tests/acme/**/*.py",
+  "tests/fixtures/**/*.py",
+  "tests/services/**/*.py",
+]
 
 
 # ==================
 # Test configuration
 # ==================
 
 [tool.pytest.ini_options]
 minversion = "2.0"
-addopts = "-rsfEX -p pytester --strict-markers --verbosity=3 --cov --cov-report=term-missing --cov-report=xml"
+addopts = "-rsfEX -p pytester --strict-markers --verbosity=3 --cov --cov-report=term-missing --cov-report=xml --cov-report html:.pytest_results/htmlcov"
 log_level = "DEBUG"
 log_cli_level = "DEBUG"
-testpaths = ["tests"]
+testpaths = ["examples", "mqttwarn", "tests"]
 xfail_strict = true
 markers = [
   "e2e",  # Full end-to-end system tests, needing an MQTT broker.
 ]
 
 [tool.coverage.run]
 branch = false
@@ -102,17 +112,18 @@
 # ===================
 
 [tool.poe.tasks]
 format = [
   {cmd="black ."},
   {cmd="isort ."},
 ]
-check-style = [
+lint = [
   {cmd="ruff ."},
   {cmd="black --check ."},
   {cmd="isort --check ."},
-  {cmd="mypy --install-types --non-interactive mqttwarn/core.py"},
+  {cmd="mypy --install-types --non-interactive"},
 ]
 test = [
   {cmd="pytest"},
 ]
 build = {cmd="python -m build"}
+check = ["lint", "test"]
```

### Comparing `mqttwarn-0.33.0/setup.py` & `mqttwarn-0.34.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 from setuptools import find_packages, setup
 from versioningit import get_cmdclasses
 
 here = os.path.abspath(os.path.dirname(__file__))
 README = open(os.path.join(here, "README.rst")).read()
 
 requires = [
-    "six<2",
-    "paho-mqtt<2",
-    "jinja2<4",
     "attrs<23",
     "docopt<1",
-    "requests<3",
+    "funcy<3",
     "future>=0.18.0,<1",
     "importlib-metadata; python_version<'3.8'",
+    "jinja2<4",
+    "paho-mqtt<2",
+    "requests<3",
+    "six<2",
 ]
 
 extras = {
     "amqp": [
         "puka>=0.0.7",
     ],
     "apns": [
         "apns>=2.0.1",
     ],
     "apprise": [
-        "apprise<2",
+        "apprise>=1.3,<2",
     ],
     "asterisk": [
         "pyst2>=0.5.0",
     ],
     "celery": [
         "celery",
     ],
@@ -161,17 +162,18 @@
 ] + extras["all"]
 
 # Packages needed for development and running CI.
 extras["develop"] = [
     "isort<6",
     "black<23",
     "build<1",
-    "mypy<1",
+    "mypy<1.3",
     "poethepoet<1",
     'ruff==0.0.254; python_version>="3.7"',
+    "sphinx-autobuild",
 ]
 
 
 setup(
     cmdclass=get_cmdclasses(),
     name="mqttwarn",
     description="mqttwarn - subscribe to MQTT topics and notify pluggable services",
@@ -216,15 +218,15 @@
         "Topic :: System :: Systems Administration",
         "Topic :: Text Processing",
         "Topic :: Utilities",
     ],
     author="Jan-Piet Mens, Ben Jones, Andreas Motl",
     author_email="jpmens@gmail.com",
     url="https://github.com/jpmens/mqttwarn",
-    keywords="mqtt notification plugins data acquisition push transformation engine " + "mosquitto ",
+    keywords="mqtt notification plugins data acquisition push transformation engine mosquitto",
     packages=find_packages(),
     include_package_data=True,
     package_data={
         "mqttwarn": [
             "*.ini",
         ],
     },
```

