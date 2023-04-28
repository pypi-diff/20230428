# Comparing `tmp/nonebot_plugin_l4d2_server-0.4.9.tar.gz` & `tmp/nonebot_plugin_l4d2_server-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_l4d2_server-0.4.9.tar", max compression
+gzip compressed data, was "nonebot_plugin_l4d2_server-0.5.0.tar", max compression
```

## Comparing `nonebot_plugin_l4d2_server-0.4.9.tar` & `nonebot_plugin_l4d2_server-0.5.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0    35823 2023-01-11 11:22:12.357251 nonebot_plugin_l4d2_server-0.4.9/LICENSE
--rw-r--r--   0        0        0    17186 2023-04-21 12:53:33.326433 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/__init__.py
--rw-r--r--   0        0        0     8646 2023-04-19 12:28:03.179586 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/command.py
--rw-r--r--   0        0        0     8731 2023-04-21 12:49:18.045680 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/config.py
--rw-r--r--   0        0        0   158357 2023-01-08 15:05:11.765786 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
--rw-r--r--   0        0        0   631630 2023-03-24 06:27:47.516852 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
--rw-r--r--   0        0        0   405369 2022-11-27 13:06:53.317128 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
--rw-r--r--   0        0        0     1650 2023-04-09 15:09:05.585642 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
--rw-r--r--   0        0        0   242997 2023-03-03 03:43:40.240633 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
--rw-r--r--   0        0        0     2150 2023-02-23 00:58:59.231306 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
--rw-r--r--   0        0        0     6190 2023-04-09 15:09:04.151919 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
--rw-r--r--   0        0        0     6401 2023-04-09 15:09:04.937399 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
--rw-r--r--   0        0        0     1571 2023-04-09 15:08:29.280432 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
--rw-r--r--   0        0        0     7874 2023-02-11 08:42:33.584146 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
--rw-r--r--   0        0        0     9067 2023-04-08 18:51:30.036612 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
--rw-r--r--   0        0        0     1661 2023-03-25 04:40:02.232501 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
--rw-r--r--   0        0        0     3085 2023-03-05 15:25:37.373454 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
--rw-r--r--   0        0        0     1748 2023-04-13 15:08:36.760710 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py
--rw-r--r--   0        0        0      376 2023-03-06 08:23:02.068422 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
--rw-r--r--   0        0        0     3332 2023-02-26 09:03:45.382934 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
--rw-r--r--   0        0        0      485 2023-01-14 18:23:43.868353 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/config.py
--rw-r--r--   0        0        0     3308 2023-02-26 09:03:47.639393 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/players.py
--rw-r--r--   0        0        0     1316 2023-01-20 07:16:17.336574 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
--rw-r--r--   0        0        0     4197 2023-03-28 03:12:43.717423 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
--rw-r--r--   0        0        0     1962 2023-04-21 12:49:18.045680 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
--rw-r--r--   0        0        0     2947 2023-04-21 12:49:18.074588 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py
--rw-r--r--   0        0        0     4128 2023-03-18 17:22:46.673151 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
--rw-r--r--   0        0        0     4097 2023-02-11 08:44:48.430294 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/download.py
--rw-r--r--   0        0        0     1070 2023-02-06 23:05:41.006175 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
--rw-r--r--   0        0        0      968 2023-01-14 18:06:13.728698 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
--rw-r--r--   0        0        0     3882 2023-04-08 18:51:00.452792 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py
--rw-r--r--   0        0        0     1427 2023-02-04 03:31:45.112442 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
--rw-r--r--   0        0        0     3520 2023-04-08 12:57:15.592761 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
--rw-r--r--   0        0        0     1124 2023-04-09 15:06:02.337793 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py
--rw-r--r--   0        0        0      788 2023-04-13 15:01:07.140804 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
--rw-r--r--   0        0        0    10949 2023-04-13 15:16:25.729675 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
--rw-r--r--   0        0        0     1676 2023-02-19 10:27:01.909990 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
--rw-r--r--   0        0        0     1160 2023-02-17 18:42:54.854831 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
--rw-r--r--   0        0        0     1409 2023-03-02 15:06:19.826864 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
--rw-r--r--   0        0        0        6 2023-04-21 12:49:18.115451 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/config.py
--rw-r--r--   0        0        0     6644 2023-04-21 12:49:18.181231 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/web.py
--rw-r--r--   0        0        0    11923 2023-04-21 12:49:18.234054 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
--rw-r--r--   0        0        0     1678 2023-02-26 09:29:05.903725 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/message.py
--rw-r--r--   0        0        0     1025 2023-03-05 15:52:53.333459 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/seach.py
--rw-r--r--   0        0        0     2166 2023-04-08 18:49:42.643806 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/txt_to_img.py
--rw-r--r--   0        0        0     8297 2023-04-09 05:43:10.168248 nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/utils.py
--rw-r--r--   0        0        0     1522 2023-04-21 12:53:38.686262 nonebot_plugin_l4d2_server-0.4.9/pyproject.toml
--rw-r--r--   0        0        0    11652 2023-04-21 12:53:13.473228 nonebot_plugin_l4d2_server-0.4.9/README.md
--rw-r--r--   0        0        0    13485 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.9/setup.py
--rw-r--r--   0        0        0    13339 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0    35823 2023-04-04 06:17:31.531814 nonebot_plugin_l4d2_server-0.5.0/LICENSE
+-rw-r--r--   0        0        0    17425 2023-04-28 09:27:53.056386 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/__init__.py
+-rw-r--r--   0        0        0     8845 2023-04-28 09:27:46.992526 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/command.py
+-rw-r--r--   0        0        0     8963 2023-04-28 09:13:46.843089 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/config.py
+-rw-r--r--   0        0        0   158357 2023-04-04 06:17:32.432688 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png
+-rw-r--r--   0        0        0   631630 2023-04-04 06:17:32.439653 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png
+-rw-r--r--   0        0        0   405369 2023-04-04 06:17:32.446667 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg
+-rw-r--r--   0        0        0     1650 2023-04-12 08:10:14.946997 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html
+-rw-r--r--   0        0        0   242997 2023-04-04 06:17:32.518934 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png
+-rw-r--r--   0        0        0     2150 2023-04-04 06:17:32.520927 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg
+-rw-r--r--   0        0        0     6368 2023-04-24 08:33:07.861726 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html
+-rw-r--r--   0        0        0     6401 2023-04-12 08:10:14.949986 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html
+-rw-r--r--   0        0        0     1571 2023-04-12 08:10:14.951977 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html
+-rw-r--r--   0        0        0     5515 2023-04-24 06:29:14.906083 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/l.svg
+-rw-r--r--   0        0        0     2408 2023-04-24 03:38:03.986578 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/m.svg
+-rw-r--r--   0        0        0     8404 2023-04-04 06:17:32.837979 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/vue.css
+-rw-r--r--   0        0        0      486 2023-04-24 02:39:20.313753 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/w.svg
+-rw-r--r--   0        0        0     8974 2023-04-28 08:08:47.505874 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py
+-rw-r--r--   0        0        0     1661 2023-04-04 06:17:32.842931 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py
+-rw-r--r--   0        0        0     3085 2023-04-04 06:17:33.045071 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py
+-rw-r--r--   0        0        0     1748 2023-04-20 00:42:41.559778 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py
+-rw-r--r--   0        0        0      376 2023-04-04 06:17:33.049047 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/startand.py
+-rw-r--r--   0        0        0     3332 2023-04-04 06:17:34.075276 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py
+-rw-r--r--   0        0        0      485 2023-04-04 06:17:34.076270 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/config.py
+-rw-r--r--   0        0        0     3308 2023-04-04 06:17:34.078267 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/players.py
+-rw-r--r--   0        0        0     1316 2023-04-04 06:17:34.082274 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py
+-rw-r--r--   0        0        0     4197 2023-04-04 06:17:35.069174 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py
+-rw-r--r--   0        0        0     1962 2023-04-20 02:34:31.279698 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py
+-rw-r--r--   0        0        0     2947 2023-04-20 02:28:12.756210 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py
+-rw-r--r--   0        0        0     4139 2023-04-28 08:36:18.885635 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py
+-rw-r--r--   0        0        0     4097 2023-04-04 06:17:36.400628 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/download.py
+-rw-r--r--   0        0        0     1070 2023-04-04 06:17:36.401631 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py
+-rw-r--r--   0        0        0      968 2023-04-04 06:17:36.402626 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py
+-rw-r--r--   0        0        0     3882 2023-04-12 08:10:14.955477 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py
+-rw-r--r--   0        0        0     1427 2023-04-04 06:17:36.739056 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py
+-rw-r--r--   0        0        0     3905 2023-04-25 06:48:18.748229 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py
+-rw-r--r--   0        0        0     1152 2023-04-27 01:31:26.318282 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py
+-rw-r--r--   0        0        0      788 2023-04-20 00:42:41.565761 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py
+-rw-r--r--   0        0        0    11114 2023-04-28 08:28:21.116819 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py
+-rw-r--r--   0        0        0     1676 2023-04-04 06:17:36.802363 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py
+-rw-r--r--   0        0        0     1265 2023-04-28 08:24:33.893547 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/rcon.py
+-rw-r--r--   0        0        0     1409 2023-04-04 06:17:36.926711 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py
+-rw-r--r--   0        0        0     8776 2023-04-28 09:27:34.285127 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/web.py
+-rw-r--r--   0        0        0    14389 2023-04-28 09:03:53.538976 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py
+-rw-r--r--   0        0        0     1678 2023-04-04 06:17:37.086862 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/message.py
+-rw-r--r--   0        0        0     1025 2023-04-04 06:17:37.088855 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/seach.py
+-rw-r--r--   0        0        0     2197 2023-04-28 06:37:36.428815 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/txt_to_img.py
+-rw-r--r--   0        0        0     8307 2023-04-28 08:09:27.412377 nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/utils.py
+-rw-r--r--   0        0        0     1522 2023-04-28 09:29:46.218925 nonebot_plugin_l4d2_server-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11652 2023-04-23 03:26:29.286604 nonebot_plugin_l4d2_server-0.5.0/README.md
+-rw-r--r--   0        0        0    13339 1970-01-01 00:00:00.000000 nonebot_plugin_l4d2_server-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/LICENSE` & `nonebot_plugin_l4d2_server-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 * but WITHOUT ANY WARRANTY; without even the implied warranty of
 * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 * GNU General Public License for more details.
 *
 * You should have received a copy of the GNU General Public License
 * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
+from .l4d2_web import web,webUI
+
 from typing import Tuple,Union,List
 from time import sleep
 
 from nonebot.matcher import Matcher
 from nonebot.typing import T_State
 from nonebot.params import CommandArg,ArgPlainText,RegexGroup,Arg,RawCommand,CommandStart
 from nonebot import get_driver, require
@@ -35,18 +37,14 @@
 from .l4d2_queries.ohter import load_josn
 from .l4d2_queries.qqgroup import write_json
 from .l4d2_file import updown_l4d2_vpk,all_zip_to_one
 
 from .txt_to_img import mode_txt_to_img
 # from .l4d2_server import RCONClient
 scheduler = require("nonebot_plugin_apscheduler").scheduler
-if l4_web:
-    from .l4d2_web import web,webUI
-else:
-    pass
 
 driver = get_driver()
 
 
 __version__ = "0.4.9"
 __plugin_meta__ = PluginMetadata(
     name="求生之路小助手",
@@ -57,31 +55,30 @@
         "author": "Agnes4m <Z735803792@163.com>",
     },
 )
 
 
 """相当于启动就检查数据库"""
 
-
 @up.handle()
 async def _(matcher:Matcher,event: NoticeEvent):
     args = event.dict()
     if args['notice_type'] != 'offline_file':
         matcher.set_arg('txt',args)
         return
-    l4_file_path = l4_file[CHECK_FILE]
+    l4_file_path = l4_config.l4_ipall[CHECK_FILE]['location']
     map_path = Path(l4_file_path, vpk_path)
     # 检查下载路径是否存在
     if not Path(l4_file_path).exists():
         await matcher.finish("你填写的路径不存在辣")
         return
     if not Path(map_path).exists():
         await matcher.finish("这个路径并不是求生服务器的路径，请再看看罢")
         return
-    url = args['file']['url']
+    url:str = args['file']['url']
     name: str = args['file']['name']
     # 如果不符合格式则忽略
     await up.send('已收到文件，开始下载')
     sleep(1)   # 等待一秒防止因为文件名获取出现BUG
     vpk_files = await updown_l4d2_vpk(map_path,name,url)
     if vpk_files:
         mes = "解压成功，新增以下几个vpk文件"
@@ -90,14 +87,15 @@
         await matcher.finish("你可能上传了相同的文件，或者解压失败了捏")
 
 
 
 @up.got("is_sure", prompt="请选择上传位置（输入阿拉伯数字)")    
 async def _(matcher: Matcher):
     args = matcher.get_arg('txt')
+    l4_file = l4_config.l4_ipall[CHECK_FILE]['location']
     if not args:
         await matcher.finish('获取文件出错辣，再试一次吧')
 
     is_sure = str(matcher.get_arg('is_sure')).strip()
     if not is_sure.isdigit():
         await matcher.finish('已取消上传')
     file_number = len(l4_file)
@@ -134,16 +132,15 @@
 
     await matcher.finish(mes_list(mes, vpk_files))
 
     
 @find_vpk.handle()
 async def _(bot:Bot,event: MessageEvent,matcher: Matcher):
     name_vpk = []
-    map_path = Path(l4_file[CHECK_FILE],vpk_path)
-    print
+    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
     name_vpk = get_vpk(name_vpk,map_path)
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下vpk文件"
     msg = ''
     msg = mes_list(msg,name_vpk).replace(" ","")
     
     await matcher.finish(mode_txt_to_img(mes,msg))
@@ -152,22 +149,22 @@
 async def _(matcher:Matcher,args:Message = CommandArg()):
     num1 = args.extract_plain_text()
     if num1:
         matcher.set_arg("num",args)
 
 @del_vpk.got("num",prompt="你要删除第几个序号的地图(阿拉伯数字)")
 async def _(matcher: Matcher,tag:int = ArgPlainText("num")):
-    map_path = Path(l4_file[CHECK_FILE],vpk_path)
+    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
     vpk_name = del_map(tag,map_path)
     await matcher.finish('已删除地图：' + vpk_name)
     
 @rename_vpk.handle()
 async def _(matcher:Matcher,matched: Tuple[int,str, str] = RegexGroup(),):
     num,useless,rename = matched
-    map_path = Path(l4_file[CHECK_FILE],vpk_path)
+    map_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],vpk_path)
     logger.info('检查是否名字是.vpk后缀')
     if not rename.endswith('.vpk'):
         rename = rename + '.vpk'
     logger.info('尝试改名')
     try:
         map_name = rename_map(num,rename,map_path)
         if map_name:
@@ -212,17 +209,17 @@
     if msg:
         matcher.set_arg("command",args)
 
 @rcon_to_server.got("command",prompt="请输入向服务器发送的指令")
 async def _(matcher:Matcher,tag:str = ArgPlainText("command")):
     tag = tag.strip()
     msg = await command_server(tag)
-    if l4_image:
+    try:
         await matcher.finish(mode_txt_to_img('服务器返回',msg))
-    else:
+    except:
         await matcher.finish(msg,reply_message = True)
         
 
 # 连续rcon连接
 # @connect_rcon.handle()
 # async def _(State:T_State,args:Message = CommandArg()):
 #     msg = args.extract_plain_text()
@@ -243,22 +240,22 @@
         
 @check_path.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     global CHECK_FILE
     msg = args.extract_plain_text()
     if msg.startswith('切换'):
         msg_number = int(''.join(msg.replace('切换', ' ').split()))
-        if msg_number > len(l4_file) or msg_number < 0:
+        if msg_number > len(l4_config.l4_ipall) or msg_number < 0:
             await matcher.send('没有这个序号的路径呐')
         else:
             CHECK_FILE = msg_number - 1
-            now_path = l4_file[CHECK_FILE]
+            now_path = l4_config.l4_ipall[CHECK_FILE]['location']
             await matcher.send(f'已经切换路径为\n{str(CHECK_FILE+1)}、{now_path}')
     else: 
-        now_path = l4_file[CHECK_FILE]
+        now_path = l4_config.l4_ipall[CHECK_FILE]['location']
         await matcher.send(f'当前的路径为\n{str(CHECK_FILE+1)}、{now_path}')
         
         
 @queries.handle()
 async def _(matcher:Matcher,args:Message = CommandArg()):
     msg = args.extract_plain_text()
     if msg:
@@ -402,44 +399,44 @@
     file_name:str = str(usr_id) + '.vtf'
     await upload_file(bot, event, img_bytes, file_name)
 
 
 
 @smx_file.handle()
 async def _(matcher:Matcher,):
-    smx_path = Path(l4_file[CHECK_FILE],"left4dead2/addons/sourcemod/plugins")
+    smx_path = Path(l4_config.l4_ipall[CHECK_FILE]['location'],"left4dead2/addons/sourcemod/plugins")
     smx_list = []
     name_smx = get_vpk(smx_list,smx_path,file_=".smx")
     logger.info("获取文件列表成功")
     mes = "当前服务器下有以下smx文件"
     msg = ''
     msg = mes_list(msg,name_smx).replace(" ","")
     await matcher.finish(mode_txt_to_img(mes,msg))
     
 @search_api.handle()
 async def _(matcher:Matcher,state:T_State,event:GroupMessageEvent,args:Message = CommandArg()):
     msg:str = args.extract_plain_text()
     # if msg.startswith('代码'):
         # 建图代码返回三方图信息
-    data = await seach_map(msg,l4_qq,l4_key)
+    data = await seach_map(msg,l4_config.l4_master[0],l4_config.l4_key)
     # else:
     if type(data) == str:
         await matcher.finish(data)
     else:
         state['maps'] = data
         await matcher.send(await map_dict_to_str(data))
         
 @search_api.got("is_sure",prompt='如果需要上传，请发送 "yes"')    
 async def _(matcher:Matcher,bot:Bot,event:GroupMessageEvent,state:T_State):
     is_sure = str(state["is_sure"])
     if is_sure == 'yes':
         data_dict:dict = state['maps'][0]
         if type(data_dict) == dict:
             logger.info('开始上传')
-            if l4_only:
+            if l4_config.l4_only:
                 data_file,file_name = await url_to_byte_name(data_dict['url'],'htp')
             else:
                 data_file,file_name = await url_to_byte_name(data_dict['url'])
             if data_file:
                 await matcher.send('获取地址成功，尝试上传')
                 await upload_file(bot, event, data_file, file_name)
             else:
@@ -449,22 +446,22 @@
             for data_one in data_dict:
                 data_file,file_name = await url_to_byte_name(data_one['url'])
                 await all_zip_to_one
                 await upload_file(bot, event, data_file, file_name)
     else:
         await matcher.finish('已取消上传')
         
-@reload_ip.handle()
-async def _(matcher:Matcher):
-    global matchers
-    await matcher.send('正在重载ip，可能需要一点时间')
-    for _, l4_matchers in matchers.items():
-        for l4_matcher in l4_matchers:
-            l4_matcher.destroy()
-    await get_des_ip()
-    await matcher.finish('已重载ip')
+# @reload_ip.handle()
+# async def _(matcher:Matcher):
+#     global matchers
+#     await matcher.send('正在重载ip，可能需要一点时间')
+#     for _, l4_matchers in matchers.items():
+#         for l4_matcher in l4_matchers:
+#             l4_matcher.destroy()
+#     await get_des_ip()
+#     await matcher.finish('已重载ip')
     
 
 @driver.on_shutdown
 async def close_db():
     """关闭数据库"""
     sq_L4D2._close()
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/command.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
 import asyncio
 from typing import Type
+from time import sleep
 
 from nonebot import on_notice,on_command,on_regex,on_keyword,MatcherGroup
 from nonebot.params import CommandArg,RawCommand,CommandStart
 from nonebot.matcher import Matcher
 import nonebot
 from nonebot.adapters.onebot.v11 import (
     GroupUploadNoticeEvent,
@@ -25,15 +26,15 @@
 # 服务器
 # last_operation_time = nonebot.Config.parse_obj(nonebot.get_driver().config.dict()).SUPERUSERS
 
 
 
 def wenjian(
 event:NoticeEvent):
-    superuse = nonebot.get_driver().config.l4_master
+    superuse = config_manager.config.l4_master
     args = event.dict()
     try:
         name: str = args['file']['name']
         usr_id = str(args['user_id'])
     except KeyError:
         return False
     if args['notice_type'] == 'offline_file':
@@ -118,30 +119,34 @@
 
 
     
 async def get_des_ip():
     global ALL_HOST
     global ANNE_IP
     global matchers
-    if l4_tag == None:
+    if l4_config.l4_tag == None:
         pass
     else:
-        ALL_HOST.update(await seach_map(l4_tag,l4_qq,l4_key,'ip'))
-        async def count_ips(ip_dict:dict):
+        try:
+            qq = l4_config.l4_master[0]
+        except:
+            qq = list(nonebot.get_bot().config.superusers)[0]
+        ALL_HOST.update(await seach_map(msg = l4_config.l4_tag,qq = qq, key=l4_config.l4_key,mode='ip'))
+        def count_ips(ip_dict:dict):
             global ANNE_IP
             for key, value in ip_dict.items():
                 if key in ['error_','success_']:
                     ip_dict.pop(key)
                     break
                 count = len(value)
                 logger.info(f'已加载：{key} | {count}个')
                 if key == '云':
                     ANNE_IP = {key:value}
-                
-        await count_ips(ALL_HOST)
+        sleep(1)
+        count_ips(ALL_HOST)
         ip_anne_list=[] 
         try:
             ips = ALL_HOST['云']
             ip_anne_list = []
             for one_ip in ips:
                 host,port = split_maohao(one_ip['ip'])
                 ip_anne_list.append((one_ip['id'],host,port))
@@ -215,15 +220,15 @@
         msg = await get_tan_jian(ip_anne_list,3)
         await matcher.finish(msg)
         
     
     
 async def init():
     global matchers
-
+    # print('启动辣')
     await get_des_ip()
-    print('启动辣')
+    
    
     
-@driver.on_startup
+@driver.on_bot_connect
 async def _():
     await init()
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/config.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import List,Dict
+from typing import List,Dict,Union
 import ast
 import platform
 import os
 from ruamel import yaml
 from pydantic import Extra,BaseModel,Field
 try:
     import ujson as json
@@ -49,49 +49,54 @@
     map_master: List[str] = Field([], alias='分群地图管理员')
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
 
-
 class L4d2Config(BaseModel):
     total_enable: bool = Field(True, alias='是否全局启用求生功能')
     map_path: List[str] = Field([], alias='求生地图路径')
     web_username: str = Field('l4d2', alias='后台管理用户名')
     web_password: str = Field('admin', alias='后台管理密码')
-    l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
-    l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
-    l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
-    l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
-    l4_ipall: Dict[str,Dict[str,str]] = Field(
-        {'本地地图':{
-        'place':'local',
+    l4_style: str = Field("standard", alias='图片风格')
+    # l4_file: List[str] = Field(	["/home/ubuntu/l4d2/coop"], alias='本地求生服务器地址')
+    # l4_host: List[str] = Field(['127.0.0.1'], alias='求生服务器地址')
+    # l4_port: List[str] = Field(['20715'], alias='求生服务器端口')
+    # l4_rcon: List[str] = Field(['114514'], alias='求生服务器rcon密码')
+    
+    l4_ipall: List[Dict[str,Union[str,int,bool]]] = Field(
+        [{
+        'id_rank':'1',
+        'place': False,
         'location':'C:\\l4d2',
         'host':'127.0.0.1',
         'port':'20715',
-        'rcon':'114514'
-        },
-        '远程地图':{
-        'place':'remote',
+        'rcon':'114514',
+        'server_id':'本地地图',
+        },{
+        'id_rank':'2',
+        'place': True,
         'location':'/home/unbuntu/coop',
         'host':'11.4.51.4',
         'port':'20715',
-        'rcon':'9191810'
-        },
-          },
-          alias='求生服务器ip集合')
+        'rcon':'9191810',
+        'account':'root',
+        'password':'114514',
+        'server_id':'远程地图',
+        }],
+          alias='l4服务器ip集合')
     web_secret_key: str = Field('49c294d32f69b732ef6447c18379451ce1738922a75cd1d4812ef150318a2ed0',
                                 alias='后台管理token密钥')
-    l4_master: List[str] = Field([], alias='求生地图全局管理员qq')
-    l4_ip:bool = Field(False, alias='查询地图是否显示ip')
+    l4_master: List[str] = Field(['114514919'], alias='求生地图全局管理员qq')
+    # l4_ip:bool = Field(False, alias='查询地图是否显示ip')
     l4_font: str = Field('simsun.ttc', alias='字体')
     l4_only:bool = Field(False, alias='下载地图是是否阻碍其他指令')
     l4_tag: List[str] = Field(['呆呆','橘'], alias='查服的名')
-    l4_key: str = Field('1145149191810', alias='key')
+    l4_key: str = Field('q1145149191810', alias='key')
     group_config: Dict[int, L4d2GroupConfig] = Field({}, alias='分群配置')
 
     def update(self, **kwargs):
         for key, value in kwargs.items():
             if key in self.__fields__:
                 self.__setattr__(key, value)
                 
@@ -120,28 +125,28 @@
         with self.file_path.open('w', encoding='utf-8') as f:
             yaml.dump(
                 self.config.dict(by_alias=True),
                 f,
                 indent=2,
                 Dumper=yaml.RoundTripDumper,
                 allow_unicode=True)
-            
+
+# 参数设置为全局变量
+global config_manager,l4_config            
 config_manager = L4d2ConfigManager()
+l4_config = config_manager.config
 
 class UserModel(BaseModel):
     username: str
     password: str
 
     
-class Config(BaseModel,extra = Extra.ignore):
-    l4_file: List[str] = ['/home/ubuntu/l4d2']
-    
 
 # env_config = Config.parse_obj(get_driver().config.dict())
-
+"""
 try:
     l4_file: List[str] = driver.config.l4_file
 except:
     l4_file: List[str] = ['/home/ubuntu/l4d2']
 
 
 try:
@@ -213,25 +218,27 @@
 except:
     l4_tag = None
 
 try:
     l4_web:bool = driver.config.l4_web
 except:
     l4_web:bool = False
-    
+   
+
 # 强制转list
 if type(l4_tag) == str or list:
     l4_list = [l4_file, l4_steamid, l4_host, l4_port, l4_rcon, l4_master,l4_tag]
     l4_list = [ast.literal_eval(i) if isinstance(i, str) else i for i in l4_list]
     l4_file, l4_steamid, l4_host, l4_port, l4_rcon, l4_master, l4_tag= l4_list
 else:
     l4_list = [l4_file, l4_steamid, l4_host, l4_port, l4_rcon, l4_master]
     l4_list = [ast.literal_eval(i) if isinstance(i, str) else i for i in l4_list]
     l4_file, l4_steamid, l4_host, l4_port, l4_rcon, l4_master= l4_list            
-        
+
+"""        
 '''
 地图路径
 '''
 vpk_path = "left4dead2/addons"
 # map_path = Path(l4_file[CHECK_FILE],vpk_path)
 # l4_file_one = l4_file[CHECK_FILE]
 # l4_host_one = l4_host[CHECK_FILE]
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/head/head.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/logo.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/header/player1.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/anne.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/back.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/fingerprint.svg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 <html>
   <head>
     <style>
       body {
         margin: 0px;
         zoom: 150%;
+        background-color: #0D1117;
       }
       .image {
         display: flex;
         flex-direction: column;
         overflow: scroll;
         width: max-content;
         padding: 20px;
       }
       .head {
         display: flex;
         flex-direction: row;
         align-items: center;
         justify-content: space-between;
-        background-color: #f5f6f7;
+        background-color: #161B22;
         padding-left: 20px;
         padding-right: 20px;
         padding-top: 10px;
         padding-bottom: 10px;
         border: 2px solid;
         border-radius: 50px;
-        border-color: #e5e7eb;
+        border-color: #1a1a1a;
         font-size: 16px;
         margin-bottom: 20px;
       }
 
       .plugins {
         display: grid;
         grid-template-columns: auto auto auto;
@@ -37,17 +38,17 @@
 		margin-bottom: 20px;
       }
       .plugin {
         display: flex;
         padding: 5px;
         border: 1px solid;
         border-radius: 5px;
-        border-color: #e5e7eb;
+        border-color: #161B22;
         box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-        background-color: #f5f6f7;
+        background-color: #1a1a1a;
       }
       .plugin_meta {
         display: flex;
         flex-direction: column;
         padding: 5px;
         width: 250px;
         justify-content: space-between;
@@ -106,15 +107,15 @@
         bottom: 4px;
         background-color: white;
       }
       .switch input {
         display: none;
       }
       .switch input:checked + .slider {
-        background-color: rgba(86, 40, 238, 0.5);
+        background-color: rgba(46, 160, 67);
       }
       .switch input:checked + .slider:before {
         -webkit-transform: translateX(16px);
         -ms-transform: translateX(16px);
         transform: translateX(16px);
       }
       .slider.round {
@@ -182,49 +183,49 @@
         visibility: inherit;
       }
     </style>
   </head>
   <body>
     <div class="image">
       <div class="head">
-        <span><b>已加载服务器</b></span>
-        <span>发送 “<b>服务器昵称/序号</b>” 查看详情</span>
+        <span><b><font color="Silver">已加载服务器</font></b></span>
+        <span><font color="Silver">发送“<b>服务器昵称/序号</b>”查看详情</font></span>
       </div>
       <div class="plugins">
         {% for plugin in plugins %}
         <div class="plugin">
           <div class="plugin_meta">
             <div class="plugin_meta_line1">
-              <div class="plugin_name">{{ plugin.number }}:{{ plugin.name }}</div>
+              <div class="plugin_name"><font color="DeepSkyBlue">{{ plugin.number }}:{{ plugin.name }}</font></div>
               <div class="plugin_status">
                 <label class="switch">
                   <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
                   <span class="slider round {% if plugin.locked %} locked {% endif %}">
                     <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
                   </span>
                 </label>
               </div>
             </div>
             <div class="plugin_meta_line2">
-				<font color="blue">{{ plugin.map_ }}</font><br>
+				<font color="LightSkyBlue">{{ plugin.map_ }}</font><br>
                 {% for Player in plugin.Players %}
-                    <font color="green">{{ Player }}</font><br>
+                    <font color="LightGray">{{ Player }}</font><br>
                 {% endfor %}
             </div>
             <div class="plugin_meta_line3">
               <div class="package_name_label"></div>
-              <div class="package_name">{{ plugin.max_players }}</div>
+              <div class="package_name"><font color="LightGray">{{ plugin.max_players }}</font></div>
             </div>
           </div>
         </div>
         {% endfor %}
       </div>
 	  <div class="head">
-      <span><b>©爱丽数码</b></span>
-      <span>github.com/Agnes4m/nonebot_plugin_l4d2_server</span>
+      <span><b><font color="Silver">©爱丽数码</font></b></span>
+      <span><font color="Silver">github*Agnes4m</font></span>
       </div>
     </div>
-</html>
   </body>
+</html>
+  
 
-
-
+/*暗黑风格-ArcPav*/
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-å·²å è½½æå¡å¨ åé âæå¡å¨æµç§°/åºå·â æ¥çè¯¦æ
+å·²å è½½æå¡å¨ åéâæå¡å¨æµç§°/åºå·âæ¥çè¯¦æ
 {% for plugin in plugins %}
 {{ plugin.number }}:{{ plugin.name }}
 
 % if plugin.enabled %} checked {% endif %} />
 {{ plugin.map_ }}
 {% for Player in plugin.Players %} {{ Player }}
 {% endfor %}
 {{ plugin.max_players }}
 {% endfor %}
-Â©ç±ä¸½æ°ç  github.com/Agnes4m/nonebot_plugin_l4d2_server
+Â©ç±ä¸½æ°ç  github*Agnes4m
+/*æé»é£æ ¼-ArcPav*/
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/help_dack.html` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/help.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 <html>
   <head>
     <style>
       body {
         margin: 0px;
         zoom: 150%;
-        background-color: #0D1117;
       }
       .image {
         display: flex;
         flex-direction: column;
         overflow: scroll;
         width: max-content;
         padding: 20px;
       }
       .head {
         display: flex;
         flex-direction: row;
         align-items: center;
         justify-content: space-between;
-        background-color: #161B22;
+        background-color: #f5f6f7;
         padding-left: 20px;
         padding-right: 20px;
         padding-top: 10px;
         padding-bottom: 10px;
         border: 2px solid;
         border-radius: 50px;
-        border-color: #1a1a1a;
+        border-color: #e5e7eb;
         font-size: 16px;
         margin-bottom: 20px;
       }
 
       .plugins {
         display: grid;
         grid-template-columns: auto auto auto;
@@ -38,17 +37,17 @@
 		margin-bottom: 20px;
       }
       .plugin {
         display: flex;
         padding: 5px;
         border: 1px solid;
         border-radius: 5px;
-        border-color: #161B22;
+        border-color: #e5e7eb;
         box-shadow: 0px 2px 6px 1px rgba(0, 0, 0, 0.2);
-        background-color: #1a1a1a;
+        background-color: #f5f6f7;
       }
       .plugin_meta {
         display: flex;
         flex-direction: column;
         padding: 5px;
         width: 250px;
         justify-content: space-between;
@@ -69,15 +68,15 @@
         justify-content: space-between;
       }
       .plugin_meta_line3 {
         display: flex;
         flex-direction: row;
         align-items: center;
       }
-      .package_name_label {
+      .package_name_label{
         background-image: url(./fingerprint.svg);
         width: 13px;
         height: 13px;
         margin-right: 8px;
       }
       .package_name {
         font-size: 13px;
@@ -107,15 +106,15 @@
         bottom: 4px;
         background-color: white;
       }
       .switch input {
         display: none;
       }
       .switch input:checked + .slider {
-        background-color: rgba(46, 160, 67);
+        background-color: rgba(86, 40, 238, 0.5);
       }
       .switch input:checked + .slider:before {
         -webkit-transform: translateX(16px);
         -ms-transform: translateX(16px);
         transform: translateX(16px);
       }
       .slider.round {
@@ -183,49 +182,52 @@
         visibility: inherit;
       }
     </style>
   </head>
   <body>
     <div class="image">
       <div class="head">
-        <span><b><font color="Silver">已加载服务器</font></b></span>
-        <span><font color="Silver">发送“<b>服务器昵称/序号</b>”查看详情</font></span>
+        <span><b>已加载服务器</b></span>
+        <span>发送 “<b>服务器昵称/序号</b>” 查看详情</span>
       </div>
       <div class="plugins">
         {% for plugin in plugins %}
         <div class="plugin">
           <div class="plugin_meta">
             <div class="plugin_meta_line1">
-              <div class="plugin_name"><font color="DeepSkyBlue">{{ plugin.number }}:{{ plugin.name }}</font></div>
+              <div class="plugin_name">{{ plugin.number }}:{{ plugin.name }}</div>
               <div class="plugin_status">
                 <label class="switch">
                   <input class="checkbox" type="checkbox" {% if plugin.enabled %} checked {% endif %} />
                   <span class="slider round {% if plugin.locked %} locked {% endif %}">
                     <span class="lock {% if plugin.locked %} locked {% endif %}"></span>
                   </span>
                 </label>
               </div>
             </div>
             <div class="plugin_meta_line2">
-				<font color="LightSkyBlue">{{ plugin.map_ }}</font><br>
+				<font color="blue">{{ plugin.map_ }}</font><br>
                 {% for Player in plugin.Players %}
-                    <font color="LightGray">{{ Player }}</font><br>
+                    <font color="green">{{ Player }}</font><br>
                 {% endfor %}
             </div>
             <div class="plugin_meta_line3">
-              <div class="package_name_label"></div>
-              <div class="package_name"><font color="LightGray">{{ plugin.max_players }}</font></div>
+              <svg width="13px" height="13px">
+                <image xlink:href="{{ plugin.system }}" width="13px" height="13px"/>
+              </svg>
+              <div class="package_name">&nbsp{{ plugin.max_players }} </div>
+              <div class="package_name">&nbsp{{ plugin.tick }} </div>
             </div>
           </div>
         </div>
         {% endfor %}
       </div>
 	  <div class="head">
-      <span><b><font color="Silver">©爱丽数码</font></b></span>
-      <span><font color="Silver">github*Agnes4m</font></span>
+      <span><b>©爱丽数码</b></span>
+      <span>github.com/Agnes4m/nonebot_plugin_l4d2_server</span>
       </div>
     </div>
-  </body>
 </html>
-  
+  </body>
+
+
 
-/*暗黑风格-ArcPav*/
```

#### html2text {}

```diff
@@ -1,12 +1,13 @@
-å·²å è½½æå¡å¨ åéâæå¡å¨æµç§°/åºå·âæ¥çè¯¦æ
+å·²å è½½æå¡å¨ åé âæå¡å¨æµç§°/åºå·â æ¥çè¯¦æ
 {% for plugin in plugins %}
 {{ plugin.number }}:{{ plugin.name }}
 
 % if plugin.enabled %} checked {% endif %} />
 {{ plugin.map_ }}
 {% for Player in plugin.Players %} {{ Player }}
 {% endfor %}
-{{ plugin.max_players }}
+
+ {{ plugin.max_players }}
+ {{ plugin.tick }}
 {% endfor %}
-Â©ç±ä¸½æ°ç  github*Agnes4m
-/*æé»é£æ ¼-ArcPav*/
+Â©ç±ä¸½æ°ç  github.com/Agnes4m/nonebot_plugin_l4d2_server
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/data/L4D2/image/template/ip.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,566 +2,560 @@
 00000010: 6f67 2069 6d70 6f72 7420 6c6f 6767 6572  og import logger
 00000020: 0d0a 0d0a 696d 706f 7274 2070 616e 6461  ....import panda
 00000030: 7320 6173 2070 640d 0a66 726f 6d20 7479  s as pd..from ty
 00000040: 7069 6e67 2069 6d70 6f72 7420 4c69 7374  ping import List
 00000050: 0d0a 0d0a 6672 6f6d 202e 616e 616c 7973  ....from .analys
 00000060: 6973 2069 6d70 6f72 7420 6466 5f74 6f5f  is import df_to_
 00000070: 6775 6f67 7561 6e6c 760d 0a66 726f 6d20  guoguanlv..from 
-00000080: 2e2e 636f 6e66 6967 2069 6d70 6f72 7420  ..config import 
-00000090: 6c34 5f73 7465 616d 6964 0d0a 6672 6f6d  l4_steamid..from
-000000a0: 202e 2e73 6561 6368 2069 6d70 6f72 7420   ..seach import 
-000000b0: 2a0d 0a66 726f 6d20 2e2e 6c34 6432 5f64  *..from ..l4d2_d
-000000c0: 6174 612e 706c 6179 6572 7320 696d 706f  ata.players impo
-000000d0: 7274 204c 3444 3250 6c61 7965 720d 0a66  rt L4D2Player..f
-000000e0: 726f 6d20 2e2e 6c34 6432 5f69 6d61 6765  rom ..l4d2_image
-000000f0: 2069 6d70 6f72 7420 6f75 745f 706e 670d   import out_png.
-00000100: 0a23 2066 726f 6d20 2e61 6e6e 655f 7465  .# from .anne_te
-00000110: 6c65 636f 6d20 696d 706f 7274 2041 4e4e  lecom import ANN
-00000120: 455f 4150 490d 0a0d 0a0d 0a73 203d 204c  E_API......s = L
-00000130: 3444 3250 6c61 7965 7228 290d 0a0d 0a20  4D2Player().... 
-00000140: 2020 200d 0a61 7379 6e63 2064 6566 2061     ..async def a
-00000150: 6e6e 655f 6874 6d6c 286e 616d 653a 7374  nne_html(name:st
-00000160: 7229 3a0d 0a20 2020 2022 2222 e690 9ce7  r):..    """....
-00000170: b4a2 e987 8ce6 8f90 e58f 96e7 8ea9 e5ae  ................
-00000180: b6e4 bfa1 e681 afef bc8c e8bf 94e5 9b9e  ................
-00000190: e588 97e8 a1a8 e5ad 97e5 85b8 2222 2220  ............""" 
-000001a0: 0d0a 2020 2020 6461 7461 5f74 6974 6c65  ..    data_title
-000001b0: 203d 2061 6e6e 655f 7365 6172 6368 286e   = anne_search(n
-000001c0: 616d 6529 0d0a 2020 2020 6461 7461 203d  ame)..    data =
-000001d0: 2064 6174 615f 7469 746c 655b 305d 0d0a   data_title[0]..
-000001e0: 2020 2020 7469 746c 6520 3d20 6461 7461      title = data
-000001f0: 5f74 6974 6c65 5b31 5d0d 0a20 2020 2069  _title[1]..    i
-00000200: 6620 6c65 6e28 6461 7461 2920 3d3d 3020  f len(data) ==0 
-00000210: 6f72 2064 6174 615b 305d 203d 3d20 224e  or data[0] == "N
-00000220: 6f20 506c 6179 6572 2066 6f75 6e64 2e22  o Player found."
-00000230: 3a0d 0a20 2020 2020 2020 2072 6574 7572  :..        retur
-00000240: 6e20 7b7d 0d0a 2020 2020 6461 7461 5f6c  n {}..    data_l
-00000250: 6973 743a 6c69 7374 203d 205b 5d0d 0a20  ist:list = [].. 
-00000260: 2020 206c 6f67 6765 722e 696e 666f 2864     logger.info(d
-00000270: 6174 6129 0d0a 2020 2020 666f 7220 6920  ata)..    for i 
-00000280: 696e 2064 6174 613a 0d0a 2020 2020 2020  in data:..      
-00000290: 2020 693a 4265 6175 7469 6675 6c53 6f75    i:BeautifulSou
-000002a0: 700d 0a20 2020 2020 2020 2074 7279 3a0d  p..        try:.
-000002b0: 0a20 2020 2020 2020 2020 2020 2052 616e  .            Ran
-000002c0: 6b20 3d20 692e 6669 6e64 2827 7464 272c  k = i.find('td',
-000002d0: 207b 2764 6174 612d 7469 746c 6527 3a20   {'data-title': 
-000002e0: 2752 616e 6b3a 277d 292e 7465 7874 2e73  'Rank:'}).text.s
-000002f0: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
-00000300: 2020 2020 706c 6179 6572 203d 2069 2e66      player = i.f
-00000310: 696e 6428 2774 6427 2c20 7b27 6461 7461  ind('td', {'data
-00000320: 2d74 6974 6c65 273a 2027 506c 6179 6572  -title': 'Player
-00000330: 3a27 7d29 2e74 6578 742e 7374 7269 7028  :'}).text.strip(
-00000340: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
-00000350: 6f69 6e74 7320 3d20 692e 6669 6e64 2827  oints = i.find('
-00000360: 7464 272c 207b 2764 6174 612d 7469 746c  td', {'data-titl
-00000370: 6527 3a20 2750 6f69 6e74 733a 277d 292e  e': 'Points:'}).
-00000380: 7465 7874 2e73 7472 6970 2829 0d0a 2020  text.strip()..  
-00000390: 2020 2020 2020 2020 2020 2320 636f 756e            # coun
-000003a0: 7472 7920 3d20 692e 6669 6e64 2827 696d  try = i.find('im
-000003b0: 6727 295b 2761 6c74 275d 0d0a 2020 2020  g')['alt']..    
-000003c0: 2020 2020 2020 2020 706c 6179 7469 6d65          playtime
-000003d0: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
-000003e0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
-000003f0: 506c 6179 7469 6d65 3a27 7d29 2e74 6578  Playtime:'}).tex
-00000400: 742e 7374 7269 7028 290d 0a20 2020 2020  t.strip()..     
-00000410: 2020 2020 2020 206c 6173 745f 6f6e 6c69         last_onli
-00000420: 6e65 203d 2069 2e66 696e 6428 2774 6427  ne = i.find('td'
-00000430: 2c20 7b27 6461 7461 2d74 6974 6c65 273a  , {'data-title':
-00000440: 2027 4c61 7374 204f 6e6c 696e 653a 277d   'Last Online:'}
-00000450: 292e 7465 7874 2e73 7472 6970 2829 0d0a  ).text.strip()..
-00000460: 2020 2020 2020 2020 6578 6365 7074 2041          except A
-00000470: 7474 7269 6275 7465 4572 726f 723a 0d0a  ttributeError:..
-00000480: 2020 2020 2020 2020 2020 2020 5261 6e6b              Rank
-00000490: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
-000004a0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
-000004b0: e68e 92e5 908d 3a27 7d29 2e74 6578 742e  ......:'}).text.
-000004c0: 7374 7269 7028 290d 0a20 2020 2020 2020  strip()..       
-000004d0: 2020 2020 2070 6c61 7965 7220 3d20 692e       player = i.
-000004e0: 6669 6e64 2827 7464 272c 207b 2764 6174  find('td', {'dat
-000004f0: 612d 7469 746c 6527 3a20 27e7 8ea9 e5ae  a-title': '.....
-00000500: b63a 277d 292e 7465 7874 2e73 7472 6970  .:'}).text.strip
-00000510: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-00000520: 706f 696e 7473 203d 2069 2e66 696e 6428  points = i.find(
-00000530: 2774 6427 2c20 7b27 6461 7461 2d74 6974  'td', {'data-tit
-00000540: 6c65 273a 2027 e588 86e6 95b0 3a27 7d29  le': '......:'})
-00000550: 2e74 6578 742e 7374 7269 7028 290d 0a20  .text.strip().. 
-00000560: 2020 2020 2020 2020 2020 2070 6c61 7974             playt
-00000570: 696d 6520 3d20 692e 6669 6e64 2827 7464  ime = i.find('td
-00000580: 272c 207b 2764 6174 612d 7469 746c 6527  ', {'data-title'
-00000590: 3a20 27e6 b8b8 e78e a9e6 97b6 e997 b43a  : '............:
-000005a0: 277d 292e 7465 7874 2e73 7472 6970 2829  '}).text.strip()
-000005b0: 0d0a 2020 2020 2020 2020 2020 2020 6c61  ..            la
-000005c0: 7374 5f6f 6e6c 696e 6520 3d20 692e 6669  st_online = i.fi
-000005d0: 6e64 2827 7464 272c 207b 2764 6174 612d  nd('td', {'data-
-000005e0: 7469 746c 6527 3a20 27e6 9c80 e590 8ee4  title': '.......
-000005f0: b88a e7ba bfe6 97b6 e997 b43a 277d 292e  ...........:'}).
-00000600: 7465 7874 2e73 7472 6970 2829 0d0a 2020  text.strip()..  
-00000610: 2020 2020 2020 6f6e 636c 6963 6b20 3d20        onclick = 
-00000620: 695b 276f 6e63 6c69 636b 275d 0d0a 2020  i['onclick']..  
-00000630: 2020 2020 2020 7374 6561 6d69 6420 3d20        steamid = 
-00000640: 6f6e 636c 6963 6b2e 7370 6c69 7428 273d  onclick.split('=
-00000650: 2729 5b32 5d2e 7374 7269 7028 2227 2229  ')[2].strip("'")
-00000660: 0d0a 2020 2020 2020 2020 706c 6179 5f6a  ..        play_j
-00000670: 736f 6e20 3d7b 0d0a 2020 2020 2020 2020  son ={..        
-00000680: 2020 2020 7469 746c 655b 305d 3a52 616e      title[0]:Ran
-00000690: 6b2c 0d0a 2020 2020 2020 2020 2020 2020  k,..            
-000006a0: 7469 746c 655b 315d 3a70 6c61 7965 722c  title[1]:player,
-000006b0: 0d0a 2020 2020 2020 2020 2020 2020 7469  ..            ti
-000006c0: 746c 655b 325d 3a70 6f69 6e74 732c 0d0a  tle[2]:points,..
-000006d0: 2020 2020 2020 2020 2020 2020 2320 7469              # ti
-000006e0: 746c 655b 335d 3a63 6f75 6e74 7279 2c0d  tle[3]:country,.
-000006f0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-00000700: 6c65 5b33 5d3a 706c 6179 7469 6d65 2c0d  le[3]:playtime,.
-00000710: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-00000720: 6c65 5b34 5d3a 6c61 7374 5f6f 6e6c 696e  le[4]:last_onlin
-00000730: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-00000740: 7469 746c 655b 355d 3a73 7465 616d 6964  title[5]:steamid
-00000750: 0d0a 2020 2020 2020 2020 7d0d 0a20 2020  ..        }..   
-00000760: 2020 2020 2064 6174 615f 6c69 7374 2e61       data_list.a
-00000770: 7070 656e 6428 706c 6179 5f6a 736f 6e29  ppend(play_json)
-00000780: 0d0a 2020 2020 6c6f 6767 6572 2e69 6e66  ..    logger.inf
-00000790: 6f28 22e6 909c e5af bbe6 95b0 e68d ae22  o("............"
-000007a0: 290d 0a20 2020 2072 6574 7572 6e20 6461  )..    return da
-000007b0: 7461 5f6c 6973 740d 0a0d 0a64 6566 2061  ta_list....def a
-000007c0: 6e6e 655f 6874 6d6c 5f6d 7367 2864 6174  nne_html_msg(dat
-000007d0: 615f 6c69 7374 3a6c 6973 7429 3a0d 0a20  a_list:list):.. 
-000007e0: 2020 2022 2222 e4bb 8ee6 909c e7b4 a2e7     """..........
-000007f0: bb93 e69e 9ce7 9a84 e5ad 97e5 85b8 e588  ................
-00000800: 97e8 a1a8 e4b8 adef bc8c e8bf 94e5 9b9e  ................
-00000810: e58f 91e9 8081 e4bf a1e6 81af 2222 220d  ............""".
-00000820: 0a20 2020 206d 6573 203d 2027 e690 9ce7  .    mes = '....
-00000830: b4a2 e588 b0e4 bba5 e4b8 8be7 8ea9 e5ae  ................
-00000840: b6e4 bfa1 e681 af27 0d0a 2020 2020 6e73  .......'..    ns
-00000850: 203d 2030 0d0a 2020 2020 0d0a 2020 2020   = 0..    ..    
-00000860: 666f 7220 6f6e 6520 696e 2064 6174 615f  for one in data_
-00000870: 6c69 7374 3a0d 0a20 2020 2020 2020 206f  list:..        o
-00000880: 6e65 3a64 6963 740d 0a20 2020 2020 2020  ne:dict..       
-00000890: 206e 7320 2b3d 2031 0d0a 2020 2020 2020   ns += 1..      
-000008a0: 2020 6966 206c 345f 7374 6561 6d69 643a    if l4_steamid:
-000008b0: 0d0a 2020 2020 2020 2020 2020 2020 7820  ..            x 
-000008c0: 3d20 360d 0a20 2020 2020 2020 2065 6c73  = 6..        els
-000008d0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000008e0: 7820 3d20 350d 0a20 2020 2020 2020 2074  x = 5..        t
-000008f0: 6974 6c65 7320 3d20 6c69 7374 286f 6e65  itles = list(one
-00000900: 2e6b 6579 7328 2929 0d0a 2020 2020 2020  .keys())..      
-00000910: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00000920: 2878 293a 0d0a 2020 2020 2020 2020 2020  (x):..          
-00000930: 2020 6d65 7320 2b3d 2027 5c6e 2720 2b20    mes += '\n' + 
-00000940: 7469 746c 6573 5b69 5d20 2b20 273a 2720  titles[i] + ':' 
-00000950: 2b20 7374 7228 6f6e 655b 7469 746c 6573  + str(one[titles
-00000960: 5b69 5d5d 290d 0a20 2020 2020 2020 206d  [i]])..        m
-00000970: 6573 202b 3d20 275c 6e2d 2d2d 2d2d 2d2d  es += '\n-------
-00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d27 0d0a  -------------'..
-00000990: 2020 2020 2020 2020 6966 206e 733e 343a          if ns>4:
-000009a0: 0d0a 2020 2020 2020 2020 2020 2020 6272  ..            br
-000009b0: 6561 6b0d 0a20 2020 2072 6574 7572 6e20  eak..    return 
-000009c0: 6d65 730d 0a0d 0a0d 0a20 200d 0a20 2020  mes......  ..   
-000009d0: 0d0a 6173 796e 6320 6465 6620 7772 6974  ..async def writ
-000009e0: 655f 706c 6179 6572 2869 642c 6d73 673a  e_player(id,msg:
-000009f0: 7374 722c 6e69 636b 6e61 6d65 3a73 7472  str,nickname:str
-00000a00: 293a 0d0a 2020 2020 2222 22e7 bb91 e5ae  ):..    """.....
-00000a10: 9ae7 94a8 e688 b722 2222 0d0a 2020 2020  ......."""..    
-00000a20: 2320 e588 a4e6 96ad e698 af73 7465 616d  # .........steam
-00000a30: 0d0a 2020 2020 7072 696e 7428 6d73 6729  ..    print(msg)
-00000a40: 0d0a 2020 2020 6966 206d 7367 2e73 7461  ..    if msg.sta
-00000a50: 7274 7377 6974 6828 2753 5445 414d 2729  rtswith('STEAM')
-00000a60: 3a0d 0a20 2020 2020 2020 2023 2074 7279  :..        # try
-00000a70: 3a0d 0a20 2020 2020 2020 2064 6174 615f  :..        data_
-00000a80: 7475 706c 6520 3d20 732e 5f71 7565 7279  tuple = s._query
-00000a90: 5f70 6c61 7965 725f 7171 2869 6429 0d0a  _player_qq(id)..
-00000aa0: 2020 2020 2020 2020 6966 2064 6174 615f          if data_
-00000ab0: 7475 706c 6520 213d 204e 6f6e 653a 0d0a  tuple != None:..
-00000ac0: 2020 2020 2020 2020 2020 2020 7171 202c              qq ,
-00000ad0: 206e 6963 6b6e 616d 202c 2073 7465 616d   nicknam , steam
-00000ae0: 6964 203d 2064 6174 615f 7475 706c 650d  id = data_tuple.
-00000af0: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00000b00: 2020 2020 2020 2020 2020 2020 6e69 636b              nick
-00000b10: 6e61 6d20 3d20 4e6f 6e65 0d0a 2020 2020  nam = None..    
-00000b20: 2020 2020 6177 6169 7420 732e 5f61 6464      await s._add
-00000b30: 5f70 6c61 7965 725f 616c 6c28 6964 202c  _player_all(id ,
-00000b40: 206e 6963 6b6e 616d 202c 206d 7367 290d   nicknam , msg).
-00000b50: 0a20 2020 2020 2020 2023 2065 7863 6570  .        # excep
-00000b60: 7420 5479 7065 4572 726f 723a 0d0a 2020  t TypeError:..  
-00000b70: 2020 2020 2020 2020 2020 2320 6177 6169            # awai
-00000b80: 7420 732e 5f61 6464 5f70 6c61 7965 725f  t s._add_player_
-00000b90: 7374 6561 6d69 6428 6964 202c 206d 7367  steamid(id , msg
-00000ba0: 290d 0a20 2020 2020 2020 206d 6573 203d  )..        mes =
-00000bb0: 2027 e7bb 91e5 ae9a e688 90e5 8a9f e596   '..............
-00000bc0: b57e 5c6e 5151 3a27 202b 206e 6963 6b6e  .~\nQQ:' + nickn
-00000bd0: 616d 6520 2b27 5c6e 2720 2b20 2773 7465  ame +'\n' + 'ste
-00000be0: 616d 6964 3a27 2b6d 7367 0d0a 2020 2020  amid:'+msg..    
-00000bf0: 2020 2020 7265 7475 726e 206d 6573 0d0a      return mes..
-00000c00: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-00000c10: 2020 2023 2074 7279 3a0d 0a20 2020 2020     # try:..     
-00000c20: 2020 2064 6174 615f 7475 706c 6520 3d20     data_tuple = 
-00000c30: 732e 5f71 7565 7279 5f70 6c61 7965 725f  s._query_player_
-00000c40: 7171 2869 6429 0d0a 2020 2020 2020 2020  qq(id)..        
-00000c50: 6966 2064 6174 615f 7475 706c 6520 213d  if data_tuple !=
-00000c60: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00000c70: 2020 2020 6964 202c 206e 6963 6b6e 616d      id , nicknam
-00000c80: 202c 2073 7465 616d 6964 203d 2064 6174   , steamid = dat
-00000c90: 615f 7475 706c 650d 0a20 2020 2020 2020  a_tuple..       
-00000ca0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-00000cb0: 2020 2020 7374 6561 6d69 6420 3d20 4e6f      steamid = No
-00000cc0: 6e65 0d0a 2020 2020 2020 2020 6177 6169  ne..        awai
-00000cd0: 7420 732e 5f61 6464 5f70 6c61 7965 725f  t s._add_player_
-00000ce0: 616c 6c28 6964 202c 206d 7367 202c 2073  all(id , msg , s
-00000cf0: 7465 616d 6964 290d 0a20 2020 2020 2020  teamid)..       
-00000d00: 2023 2065 7863 6570 7420 5479 7065 4572   # except TypeEr
-00000d10: 726f 723a 0d0a 2020 2020 2020 2020 2320  ror:..        # 
-00000d20: 2020 2020 6177 6169 7420 732e 5f61 6464      await s._add
-00000d30: 5f70 6c61 7965 725f 6e69 636b 6e61 6d65  _player_nickname
-00000d40: 2869 6420 2c20 6d73 6720 2920 0d0a 2020  (id , msg ) ..  
-00000d50: 2020 2020 2020 6d65 7320 3d20 27e7 bb91        mes = '...
-00000d60: e5ae 9ae6 8890 e58a 9fe5 96b5 7e5c 6e51  ............~\nQ
-00000d70: 513a 2720 2b20 6e69 636b 6e61 6d65 202b  Q:' + nickname +
-00000d80: 275c 6e27 202b 2027 7374 6561 6de6 98b5  '\n' + 'steam...
-00000d90: e7a7 b03a 272b 6d73 670d 0a20 2020 2020  ...:'+msg..     
-00000da0: 2020 2072 6574 7572 6e20 6d65 730d 0a0d     return mes...
-00000db0: 0a20 2020 2020 2020 200d 0a0d 0a20 2020  .        ....   
-00000dc0: 2020 2020 200d 0a64 6566 2064 656c 5f70       ..def del_p
-00000dd0: 6c61 7965 7228 6964 3a73 7472 293a 0d0a  layer(id:str):..
-00000de0: 2020 2020 2222 22e5 88a0 e999 a4e7 bb91      """.........
-00000df0: e5ae 9ae4 bfa1 e681 af2c e8bf 94e5 9b9e  .........,......
-00000e00: e6b6 88e6 81af 2222 220d 0a20 2020 2069  ......"""..    i
-00000e10: 6620 6e6f 7420 732e 5f71 7565 7279 5f70  f not s._query_p
-00000e20: 6c61 7965 725f 7171 2869 6429 3a0d 0a20  layer_qq(id):.. 
-00000e30: 2020 2020 2020 2072 6574 7572 6e20 27e4         return '.
-00000e40: bda0 e8bf 98e6 b2a1 e69c 89e7 bb91 e5ae  ................
-00000e50: 9ae8 bf87 efbc 8ce8 afb7 e4bd bfe7 94a8  ................
-00000e60: 5be6 b182 e794 9fe7 bb91 e5ae 9a2b e698  [............+..
-00000e70: b5e7 a7b0 2f73 7465 616d 6964 5d27 0d0a  ..../steamid]'..
-00000e80: 2020 2020 6966 2073 2e5f 6465 6c65 7465      if s._delete
-00000e90: 5f70 6c61 7965 723a 0d0a 2020 2020 2020  _player:..      
-00000ea0: 2020 7265 7475 726e 2027 e588 a0e9 99a4    return '......
-00000eb0: e688 90e5 8a9f e596 b57e 270d 0a20 2020  .........~'..   
-00000ec0: 2020 2020 200d 0a0d 0a20 2020 200d 0a61       ....    ..a
-00000ed0: 7379 6e63 2064 6566 2069 645f 746f 5f6d  sync def id_to_m
-00000ee0: 6573 286e 616d 653a 7374 7229 3a0d 0a20  es(name:str):.. 
-00000ef0: 2020 2022 2222 e6a0 b9e6 8dae 6e61 6d65     """......name
-00000f00: e4bb 8ee6 95b0 e68d aee5 ba93 2ce8 bf94  ............,...
-00000f10: e59b 9e73 7465 616d 6964 e380 81e6 8896  ...steamid......
-00000f20: e880 85e7 a9ba e799 bd22 2222 0d0a 2020  ........."""..  
-00000f30: 2020 6461 7461 5f74 7570 6c65 203d 2061    data_tuple = a
-00000f40: 7761 6974 2073 2e73 6561 7263 685f 6461  wait s.search_da
-00000f50: 7461 284e 6f6e 652c 6e61 6d65 2c4e 6f6e  ta(None,name,Non
-00000f60: 6529 0d0a 2020 2020 7072 696e 7428 6461  e)..    print(da
-00000f70: 7461 5f74 7570 6c65 290d 0a20 2020 2069  ta_tuple)..    i
-00000f80: 6620 6461 7461 5f74 7570 6c65 3a0d 0a20  f data_tuple:.. 
-00000f90: 2020 2020 2020 2073 7465 616d 6964 203d         steamid =
-00000fa0: 2064 6174 615f 7475 706c 655b 325d 0d0a   data_tuple[2]..
-00000fb0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00000fc0: 7465 616d 6964 0d0a 2020 2020 7265 7475  teamid..    retu
-00000fd0: 726e 204e 6f6e 650d 0a20 2020 200d 0a0d  rn None..    ...
-00000fe0: 0a64 6566 2061 6e6e 655f 7261 6e6b 5f64  .def anne_rank_d
-00000ff0: 6963 7428 6e61 6d65 3a73 7472 293a 0d0a  ict(name:str):..
-00001000: 2020 2020 2222 22e7 94a8 7374 6561 6d69      """...steami
-00001010: 642c e69f a5e8 afa6 e683 852c e8be 93e5  d,.........,....
-00001020: 87ba e5ad 97e5 85b8 2222 220d 0a20 2020  ........"""..   
-00001030: 2064 6174 615f 6469 6374 203d 207b 7d0d   data_dict = {}.
-00001040: 0a20 2020 2075 726c 203d 6627 6874 7470  .    url =f'http
-00001050: 733a 2f2f 7362 2e74 7279 6765 6b2e 636f  s://sb.trygek.co
-00001060: 6d2f 6c34 645f 7374 6174 732f 7261 6e6b  m/l4d_stats/rank
-00001070: 696e 672f 706c 6179 6572 2e70 6870 3f73  ing/player.php?s
-00001080: 7465 616d 6964 3d7b 6e61 6d65 7d27 0d0a  teamid={name}'..
-00001090: 2020 2020 6865 6164 6572 7320 3d20 7b0d      headers = {.
-000010a0: 0a20 2020 2020 2020 2027 5573 6572 2d41  .        'User-A
-000010b0: 6765 6e74 273a 274d 6f7a 696c 6c61 2f35  gent':'Mozilla/5
-000010c0: 2e30 2028 5769 6e64 6f77 7320 4e54 2031  .0 (Windows NT 1
-000010d0: 302e 303b 2057 696e 3634 3b20 7836 343b  0.0; Win64; x64;
-000010e0: 2072 763a 3130 372e 3029 2047 6563 6b6f   rv:107.0) Gecko
-000010f0: 2f32 3031 3030 3130 3120 4669 7265 666f  /20100101 Firefo
-00001100: 782f 3130 372e 3027 0d0a 2020 2020 7d0d  x/107.0'..    }.
-00001110: 0a20 2020 2064 6174 6120 3d20 6874 7470  .    data = http
-00001120: 782e 6765 7428 7572 6c3d 7572 6c2c 6865  x.get(url=url,he
-00001130: 6164 6572 733d 6865 6164 6572 732c 7469  aders=headers,ti
-00001140: 6d65 6f75 743d 3529 0d0a 2020 2020 6966  meout=5)..    if
-00001150: 2064 6174 612e 7374 6174 7573 5f63 6f64   data.status_cod
-00001160: 6520 213d 2032 3030 3a0d 0a20 2020 2020  e != 200:..     
-00001170: 2020 2072 6574 7572 6e20 5b66 22e6 9fa5     return [f"...
-00001180: e8af a2e9 9499 e8af afef bc8c e78a b6e6  ................
-00001190: 8081 e7a0 817b 6461 7461 2e73 7461 7475  .....{data.statu
-000011a0: 735f 636f 6465 7d22 5d0d 0a20 2020 2064  s_code}"]..    d
-000011b0: 6174 6120 3d20 6461 7461 2e63 6f6e 7465  ata = data.conte
-000011c0: 6e74 2e64 6563 6f64 6528 2775 7466 2d38  nt.decode('utf-8
-000011d0: 2729 0d0a 2020 2020 6461 7461 203d 2042  ')..    data = B
-000011e0: 6561 7574 6966 756c 536f 7570 2864 6174  eautifulSoup(dat
-000011f0: 612c 2027 6874 6d6c 2e70 6172 7365 7227  a, 'html.parser'
-00001200: 290d 0a20 2020 2064 6574 6169 6c20 3d20  )..    detail = 
-00001210: 6461 7461 2e66 696e 645f 616c 6c28 2774  data.find_all('t
-00001220: 6162 6c65 2729 0d0a 2020 2020 6e20 3d20  able')..    n = 
-00001230: 300d 0a20 2020 2077 6869 6c65 206e 203c  0..    while n <
-00001240: 2032 3a0d 0a20 2020 2020 2020 2064 6174   2:..        dat
-00001250: 615f 6c69 7374 3a4c 6973 745b 6469 6374  a_list:List[dict
-00001260: 5d20 3d20 5b5d 0d0a 2020 2020 2020 2020  ] = []..        
-00001270: 6465 7461 696c 3220 3d20 6465 7461 696c  detail2 = detail
-00001280: 5b6e 5d0d 0a20 2020 2020 2020 2074 7220  [n]..        tr 
-00001290: 3d20 6465 7461 696c 322e 6669 6e64 5f61  = detail2.find_a
-000012a0: 6c6c 2827 7472 2729 0d0a 2020 2020 2020  ll('tr')..      
-000012b0: 2020 666f 7220 6920 696e 2074 723a 0d0a    for i in tr:..
-000012c0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
-000012d0: 6520 3d20 692e 6669 6e64 2827 7464 272c  e = i.find('td',
-000012e0: 207b 2763 6c61 7373 273a 2027 772d 3530   {'class': 'w-50
-000012f0: 277d 290d 0a20 2020 2020 2020 2020 2020  '})..           
-00001300: 2076 616c 7565 203d 2074 6974 6c65 2e66   value = title.f
-00001310: 696e 645f 6e65 7874 5f73 6962 6c69 6e67  ind_next_sibling
-00001320: 2827 7464 2729 0d0a 2020 2020 2020 2020  ('td')..        
-00001330: 2020 2020 6e65 775f 6469 6374 203d 207b      new_dict = {
-00001340: 7469 746c 652e 7465 7874 3a76 616c 7565  title.text:value
-00001350: 2e74 6578 747d 0d0a 2020 2020 2020 2020  .text}..        
-00001360: 2020 2020 6461 7461 5f64 6963 742e 7570      data_dict.up
-00001370: 6461 7465 286e 6577 5f64 6963 7429 0d0a  date(new_dict)..
-00001380: 2020 2020 2020 2020 6461 7461 5f6c 6973          data_lis
-00001390: 742e 6170 7065 6e64 2864 6174 615f 6469  t.append(data_di
-000013a0: 6374 290d 0a20 2020 2020 2020 206e 202b  ct)..        n +
-000013b0: 3d20 310d 0a20 2020 2023 20e8 8eb7 e58f  = 1..    # .....
-000013c0: 96e5 a4b4 e583 8f0d 0a20 2020 2065 6c65  .........    ele
-000013d0: 6d65 6e74 3a73 7472 203d 2064 6174 612e  ment:str = data.
-000013e0: 6669 6e64 5f61 6c6c 2861 7474 7273 3d7b  find_all(attrs={
-000013f0: 2273 7479 6c65 223a 2022 6375 7273 6f72  "style": "cursor
-00001400: 3a70 6f69 6e74 6572 227d 295b 305d 2e67  :pointer"})[0].g
-00001410: 6574 2822 6f6e 636c 6963 6b22 290d 0a20  et("onclick").. 
-00001420: 2020 2070 6c61 7965 725f 7572 6c20 3d20     player_url = 
-00001430: 656c 656d 656e 742e 7370 6c69 7428 2227  element.split("'
-00001440: 2229 5b31 5d0d 0a20 2020 2064 6174 615f  ")[1]..    data_
-00001450: 6c69 7374 5b30 5d2e 7570 6461 7465 287b  list[0].update({
-00001460: 22e4 b8aa e4ba bae8 b584 e696 9922 3a70  "............":p
-00001470: 6c61 7965 725f 7572 6c7d 290d 0a20 2020  layer_url})..   
-00001480: 2023 20e8 8eb7 e58f 96e4 b880 e8a8 800d   # .............
-00001490: 0a20 2020 206d 6573 7361 6765 203d 2064  .    message = d
-000014a0: 6174 612e 7365 6c65 6374 2822 6874 6d6c  ata.select("html
-000014b0: 2062 6f64 7920 6469 762e 636f 6e74 656e   body div.conten
-000014c0: 742e 7465 7874 2d63 656e 7465 722e 7465  t.text-center.te
-000014d0: 7874 2d6d 642d 6c65 6674 2064 6976 2e63  xt-md-left div.c
-000014e0: 6f6e 7461 696e 6572 2e74 6578 742d 6c65  ontainer.text-le
-000014f0: 6674 2064 6976 2e63 6f6c 2d6d 642d 3132  ft div.col-md-12
-00001500: 2e68 2d31 3030 2064 6976 2e63 6172 642d  .h-100 div.card-
-00001510: 626f 6479 2e77 6f72 6c64 6d61 702e 642d  body.worldmap.d-
-00001520: 666c 6578 2e66 6c65 782d 636f 6c75 6d6e  flex.flex-column
-00001530: 2e6a 7573 7469 6679 2d63 6f6e 7465 6e74  .justify-content
-00001540: 2d63 656e 7465 722e 7465 7874 2d63 656e  -center.text-cen
-00001550: 7465 7220 7370 616e 2229 0d0a 2020 2020  ter span")..    
-00001560: 6d73 675f 6c69 7374 203d 205b 5d0d 0a20  msg_list = [].. 
-00001570: 2020 2066 6f72 2069 2069 6e20 6d65 7373     for i in mess
-00001580: 6167 653a 0d0a 2020 2020 2020 2020 6d73  age:..        ms
-00001590: 675f 6c69 7374 2e61 7070 656e 6428 692e  g_list.append(i.
-000015a0: 7465 7874 290d 0a20 2020 2064 6174 615f  text)..    data_
-000015b0: 6c69 7374 5b30 5d2e 7570 6461 7465 287b  list[0].update({
-000015c0: 22e4 b880 e8a8 8022 3a6d 7367 5f6c 6973  "......":msg_lis
-000015d0: 747d 290d 0a20 2020 2072 6574 7572 6e20  t})..    return 
-000015e0: 6461 7461 5f6c 6973 740d 0a0d 0a64 6566  data_list....def
-000015f0: 2061 6e6e 655f 7261 6e6b 5f64 6963 745f   anne_rank_dict_
-00001600: 6d73 6728 6461 7461 5f6c 6973 7429 3a0d  msg(data_list):.
-00001610: 0a20 2020 2022 2222 e5ad 97e5 85b8 e8bd  .    """........
-00001620: ac6d 7367 2222 220d 0a20 2020 206d 7367  .msg"""..    msg
-00001630: 203d 2027 270d 0a20 2020 2066 6f72 2064   = ''..    for d
-00001640: 6174 615f 6469 6374 2069 6e20 6461 7461  ata_dict in data
-00001650: 5f6c 6973 743a 0d0a 2020 2020 2020 2020  _list:..        
-00001660: 6d65 7320 3d20 2727 0d0a 2020 2020 2020  mes = ''..      
-00001670: 2020 666f 7220 6920 696e 2064 6174 615f    for i in data_
-00001680: 6469 6374 3a0d 0a20 2020 2020 2020 2020  dict:..         
-00001690: 2020 206d 6573 202b 3d27 5c6e 272b 2069     mes +='\n'+ i
-000016a0: 202b 2064 6174 615f 6469 6374 5b69 5d0d   + data_dict[i].
-000016b0: 0a20 2020 2020 2020 206d 6573 202b 3d20  .        mes += 
-000016c0: 275c 6e2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  '\n-------------
-000016d0: 2d2d 2d2d 2d2d 2d27 0d0a 2020 2020 2020  -------'..      
-000016e0: 2020 6d73 6720 2b3d 206d 6573 0d0a 2020    msg += mes..  
-000016f0: 2020 7265 7475 726e 206d 7367 0d0a 0d0a    return msg....
-00001700: 0d0a 6173 796e 6320 6465 6620 616e 6e65  ..async def anne
-00001710: 5f6d 6573 7367 6165 286e 616d 653a 7374  _messgae(name:st
-00001720: 722c 7573 725f 6964 3a73 7472 293a 0d0a  r,usr_id:str):..
-00001730: 2020 2020 2222 22e8 8eb7 e58f 9661 6e6e      """......ann
-00001740: 65e4 bfa1 e681 afe5 8faf e8be 93e5 87ba  e...............
-00001750: e4bf a1e6 81af 2222 220d 0a20 2020 2069  ......"""..    i
-00001760: 6620 6e61 6d65 3a0d 0a20 2020 2020 2020  f name:..       
-00001770: 206c 6f67 6765 722e 696e 666f 2822 e585   logger.info("..
-00001780: b3e9 94ae e8af 8de6 9fa5 e8af a222 202b  ............." +
-00001790: 206e 616d 6529 0d0a 2020 2020 2020 2020   name)..        
-000017a0: 6966 206e 6f74 206e 616d 652e 7374 6172  if not name.star
-000017b0: 7473 7769 7468 2827 5354 4541 4d27 293a  tswith('STEAM'):
-000017c0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-000017d0: 6561 6d69 6420 3d20 6177 6169 7420 6964  eamid = await id
-000017e0: 5f74 6f5f 6d65 7328 6e61 6d65 290d 0a20  _to_mes(name).. 
-000017f0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00001800: 7420 7374 6561 6d69 643a 0d0a 2020 2020  t steamid:..    
-00001810: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00001820: 6572 2e69 6e66 6f28 22e6 b2a1 e69c 89e6  er.info(".......
-00001830: 89be e588 b071 71ef bc8c e4bd bfe7 94a8  .....qq.........
-00001840: e9bb 98e8 aea4 e5a4 b4e5 838f 2229 0d0a  ............")..
-00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001860: 6d65 7373 6167 6520 3d20 6177 6169 7420  message = await 
-00001870: 616e 6e65 5f68 746d 6c28 6e61 6d65 290d  anne_html(name).
-00001880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001890: 2075 7372 5f69 6420 3d20 2231 3134 3531   usr_id = "11451
-000018a0: 3439 3139 3138 3130 220d 0a20 2020 2020  49191810"..     
-000018b0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
-000018c0: 6e28 6d65 7373 6167 6529 203d 3d20 303a  n(message) == 0:
-000018d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000018e0: 2020 2020 2020 7265 7475 726e 2027 e6b2        return '..
-000018f0: a1e6 9c89 e58f abe8 bf99 e4b8 aae5 908d  ................
-00001900: e5ad 97e7 9a84 2e2e 2e5c 6e27 0d0a 2020  .........\n'..  
-00001910: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001920: 206c 656e 286d 6573 7361 6765 2920 3e20   len(message) > 
-00001930: 313a 0d0a 2020 2020 2020 2020 2020 2020  1:..            
-00001940: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-00001950: 6e6e 655f 6874 6d6c 5f6d 7367 286d 6573  nne_html_msg(mes
-00001960: 7361 6765 290d 0a20 2020 2020 2020 2020  sage)..         
-00001970: 2020 2020 2020 206e 616d 6520 3d20 6d65         name = me
-00001980: 7373 6167 655b 305d 5b27 7374 6561 6d69  ssage[0]['steami
-00001990: 6427 5d0d 0a20 2020 2020 2020 2020 2020  d']..           
-000019a0: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-000019b0: 2020 2020 2020 2020 6e61 6d65 203d 2073          name = s
-000019c0: 7465 616d 6964 0d0a 2020 2020 2020 2020  teamid..        
-000019d0: 2320 7374 6561 6d69 640d 0a20 2020 2020  # steamid..     
-000019e0: 2020 206d 7367 203d 2061 6e6e 655f 7261     msg = anne_ra
-000019f0: 6e6b 5f64 6963 7428 6e61 6d65 295b 305d  nk_dict(name)[0]
-00001a00: 0d0a 2020 2020 2020 2020 6966 2074 7970  ..        if typ
-00001a10: 6528 6d73 6729 203d 3d20 6469 6374 3a0d  e(msg) == dict:.
-00001a20: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
-00001a30: 2e75 7064 6174 6528 6177 6169 7420 6466  .update(await df
-00001a40: 5f74 6f5f 6775 6f67 7561 6e6c 7628 6177  _to_guoguanlv(aw
-00001a50: 6169 7420 616e 6e65 5f6d 6170 5f6d 7367  ait anne_map_msg
-00001a60: 286e 616d 6529 2929 0d0a 2020 2020 2020  (name)))..      
-00001a70: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-00001a80: 6f28 27e4 bdbf e794 a8e5 9bbe e789 8727  o('............'
-00001a90: 290d 0a20 2020 2020 2020 2020 2020 206d  )..            m
-00001aa0: 7367 203d 2061 7761 6974 206f 7574 5f70  sg = await out_p
-00001ab0: 6e67 2875 7372 5f69 642c 6d73 6729 0d0a  ng(usr_id,msg)..
-00001ac0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
-00001ad0: 7367 0d0a 2020 2020 656c 7365 3a0d 0a20  sg..    else:.. 
-00001ae0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00001af0: 2020 2020 31e3 8081 7171 3ee6 95b0 e68d      1...qq>.....
-00001b00: ae3e e6b2 a1e6 9c89 e695 b0e6 8dae efbc  .>..............
-00001b10: 8ce8 bf94 e59b 9e0d 0a20 2020 2020 2020  .........       
-00001b20: 2032 e380 8171 713e e695 b0e6 8dae 3e73   2...qq>......>s
-00001b30: 7465 616d 6964 3ee6 9fa5 e8af a20d 0a20  teamid>........ 
-00001b40: 2020 2020 2020 2033 e380 8171 713e e695         3...qq>..
-00001b50: b0e6 8dae 3ee6 98b5 e7a7 b03e e69f a5e8  ....>......>....
-00001b60: afa2 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
-00001b70: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00001b80: 696e 666f 2822 7171 e4bf a1e6 81af e69f  info("qq........
-00001b90: a5e8 afa2 2229 0d0a 2020 2020 2020 2020  ....")..        
-00001ba0: 6461 7461 5f74 7570 6c65 203d 2073 2e5f  data_tuple = s._
-00001bb0: 7175 6572 795f 706c 6179 6572 5f71 7128  query_player_qq(
-00001bc0: 7573 725f 6964 290d 0a20 2020 2020 2020  usr_id)..       
-00001bd0: 206c 6f67 6765 722e 696e 666f 2864 6174   logger.info(dat
-00001be0: 615f 7475 706c 6529 0d0a 2020 2020 2020  a_tuple)..      
-00001bf0: 2020 6966 2064 6174 615f 7475 706c 653d    if data_tuple=
-00001c00: 3d20 4e6f 6e65 3a0d 0a20 2020 2020 2020  = None:..       
-00001c10: 2020 2020 2072 6574 7572 6e20 6622 e6b2       return f"..
-00001c20: a1e6 9c89 e7bb 91e5 ae9a e4bf a1e6 81af  ................
-00001c30: 2e2e 2ee8 afb7 e4bd bfe7 94a8 e380 90e6  ................
-00001c40: b182 e794 9fe7 bb91 e5ae 9a20 7878 78e3  ........... xxx.
-00001c50: 8091 5c6e 220d 0a20 2020 2020 2020 2023  ..\n"..        #
-00001c60: 20e5 8faa e69c 89e5 908d e5ad 97ef bc8c   ...............
-00001c70: e585 88e6 9fa5 e8af a2e6 95b0 e68d aee5  ................
-00001c80: 9ca8 e588 a4e6 96ad 0d0a 2020 2020 2020  ..........      
-00001c90: 2020 656c 6966 2064 6174 615f 7475 706c    elif data_tupl
-00001ca0: 655b 325d 3a0d 0a20 2020 2020 2020 2020  e[2]:..         
-00001cb0: 2020 206e 616d 6520 3d20 6461 7461 5f74     name = data_t
-00001cc0: 7570 6c65 5b32 5d0d 0a20 2020 2020 2020  uple[2]..       
-00001cd0: 2065 6c69 6620 6461 7461 5f74 7570 6c65   elif data_tuple
-00001ce0: 5b31 5d3a 0d0a 2020 2020 2020 2020 2020  [1]:..          
-00001cf0: 2020 6e61 6d65 203d 2061 7761 6974 2069    name = await i
-00001d00: 645f 746f 5f6d 6573 2864 6174 615f 7475  d_to_mes(data_tu
-00001d10: 706c 655b 315d 290d 0a20 2020 2020 2020  ple[1])..       
-00001d20: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00001d30: 286e 616d 6529 0d0a 2020 2020 2020 2020  (name)..        
-00001d40: 2020 2020 6966 206e 6f74 206e 616d 653a      if not name:
-00001d50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001d60: 2020 6d65 7373 6167 6520 3d20 6177 6169    message = awai
-00001d70: 7420 616e 6e65 5f68 746d 6c28 6461 7461  t anne_html(data
-00001d80: 5f74 7570 6c65 5b31 5d29 0d0a 2020 2020  _tuple[1])..    
-00001d90: 2020 2020 2020 2020 2020 2020 7573 725f              usr_
-00001da0: 6964 203d 2022 3131 3435 3134 3931 3931  id = "1145149191
-00001db0: 3831 3022 0d0a 2020 2020 2020 2020 2020  810"..          
-00001dc0: 2020 2020 2020 6966 206c 656e 286d 6573        if len(mes
-00001dd0: 7361 6765 2920 3d3d 2030 3a0d 0a20 2020  sage) == 0:..   
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2072 6574 7572 6e20 27e6 b2a1 e69c 89e5   return '.......
-00001e00: 8fab e8bf 99e4 b8aa e590 8de5 ad97 e79a  ................
-00001e10: 842e 2e2e 5c6e 270d 0a20 2020 2020 2020  ....\n'..       
-00001e20: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
-00001e30: 6d65 7373 6167 6529 203e 2031 3a0d 0a20  message) > 1:.. 
-00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 2020 2072 6574 7572 6e20 616e 6e65 5f68     return anne_h
-00001e60: 746d 6c5f 6d73 6728 6d65 7373 6167 6529  tml_msg(message)
-00001e70: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001e80: 2020 6e61 6d65 203d 206d 6573 7361 6765    name = message
-00001e90: 5b30 5d5b 2773 7465 616d 6964 275d 0d0a  [0]['steamid']..
-00001ea0: 2020 2020 2020 2020 2320 6e61 6d65 e698          # name..
-00001eb0: af73 7465 616d 6964 0d0a 2020 2020 2020  .steamid..      
-00001ec0: 2020 6d73 6720 3d20 616e 6e65 5f72 616e    msg = anne_ran
-00001ed0: 6b5f 6469 6374 286e 616d 6529 5b30 5d0d  k_dict(name)[0].
-00001ee0: 0a20 2020 2020 2020 2069 6620 7479 7065  .        if type
-00001ef0: 286d 7367 2920 3d3d 2064 6963 743a 0d0a  (msg) == dict:..
-00001f00: 2020 2020 2020 2020 2020 2020 6d73 672e              msg.
-00001f10: 7570 6461 7465 2861 7761 6974 2064 665f  update(await df_
-00001f20: 746f 5f67 756f 6775 616e 6c76 2861 7761  to_guoguanlv(awa
-00001f30: 6974 2061 6e6e 655f 6d61 705f 6d73 6728  it anne_map_msg(
-00001f40: 6e61 6d65 2929 290d 0a20 2020 2020 2020  name)))..       
-00001f50: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-00001f60: 2827 e4bd bfe7 94a8 e59b bee7 8987 2729  ('............')
-00001f70: 0d0a 2020 2020 2020 2020 2020 2020 6d73  ..            ms
-00001f80: 6720 3d20 6177 6169 7420 6f75 745f 706e  g = await out_pn
-00001f90: 6728 7573 725f 6964 2c6d 7367 290d 0a20  g(usr_id,msg).. 
-00001fa0: 2020 2020 2020 2072 6574 7572 6e20 6d73         return ms
-00001fb0: 670d 0a20 2020 200d 0a61 7379 6e63 2064  g..    ..async d
-00001fc0: 6566 2061 6e6e 655f 6d61 705f 6d73 6728  ef anne_map_msg(
-00001fd0: 7374 6561 6d69 643a 7374 7229 3a0d 0a20  steamid:str):.. 
-00001fe0: 2020 2022 2222 7374 6561 6d69 642d 3ee5     """steamid->.
-00001ff0: 9cb0 e59b bee4 bfa1 e681 af22 2222 0d0a  ..........."""..
-00002000: 2020 2020 7572 6c20 3d20 6622 6874 7470      url = f"http
-00002010: 733a 2f2f 7362 2e74 7279 6765 6b2e 636f  s://sb.trygek.co
-00002020: 6d2f 6c34 645f 7374 6174 732f 7261 6e6b  m/l4d_stats/rank
-00002030: 696e 672f 7469 6d65 646d 6170 732e 7068  ing/timedmaps.ph
-00002040: 703f 7374 6561 6d69 643d 7b73 7465 616d  p?steamid={steam
-00002050: 6964 7d22 0d0a 2020 2020 6865 6164 6572  id}"..    header
-00002060: 7320 3d20 7b0d 0a20 2020 2020 2020 2027  s = {..        '
-00002070: 5573 6572 2d41 6765 6e74 273a 274d 6f7a  User-Agent':'Moz
-00002080: 696c 6c61 2f35 2e30 2028 5769 6e64 6f77  illa/5.0 (Window
-00002090: 7320 4e54 2031 302e 303b 2057 696e 3634  s NT 10.0; Win64
-000020a0: 3b20 7836 343b 2072 763a 3130 372e 3029  ; x64; rv:107.0)
-000020b0: 2047 6563 6b6f 2f32 3031 3030 3130 3120   Gecko/20100101 
-000020c0: 4669 7265 666f 782f 3130 372e 3027 0d0a  Firefox/107.0'..
-000020d0: 2020 2020 7d0d 0a20 2020 2064 6174 6120      }..    data 
-000020e0: 3d20 6874 7470 782e 6765 7428 7572 6c2c  = httpx.get(url,
-000020f0: 6865 6164 6572 733d 6865 6164 6572 732c  headers=headers,
-00002100: 7469 6d65 6f75 743d 3529 2e63 6f6e 7465  timeout=5).conte
-00002110: 6e74 2e64 6563 6f64 6528 2775 7466 2d38  nt.decode('utf-8
-00002120: 2729 0d0a 2020 2020 736f 7570 203d 2042  ')..    soup = B
-00002130: 6561 7574 6966 756c 536f 7570 2864 6174  eautifulSoup(dat
-00002140: 612c 2027 6874 6d6c 2e70 6172 7365 7227  a, 'html.parser'
-00002150: 290d 0a20 2020 2064 6174 615f 6c69 7374  )..    data_list
-00002160: 203d 205b 5d0d 0a20 2020 2063 6172 6473   = []..    cards
-00002170: 203d 2073 6f75 702e 7365 6c65 6374 2827   = soup.select('
-00002180: 6469 762e 6361 7264 2e72 6f75 6e64 6564  div.card.rounded
-00002190: 2d30 2729 0d0a 2020 2020 666f 7220 6361  -0')..    for ca
-000021a0: 7264 2069 6e20 6361 7264 733a 0d0a 2020  rd in cards:..  
-000021b0: 2020 2020 2020 7462 6f64 6965 7320 3d20        tbodies = 
-000021c0: 6361 7264 2e73 656c 6563 7428 2774 626f  card.select('tbo
-000021d0: 6479 2729 0d0a 2020 2020 2020 2020 666f  dy')..        fo
-000021e0: 7220 7462 6f64 7920 696e 2074 626f 6469  r tbody in tbodi
-000021f0: 6573 3a0d 0a20 2020 2020 2020 2020 2020  es:..           
-00002200: 2072 6f77 7320 3d20 5b74 642e 7465 7874   rows = [td.text
-00002210: 2e73 7472 6970 2829 2066 6f72 2074 6420  .strip() for td 
-00002220: 696e 2074 626f 6479 2e66 696e 645f 616c  in tbody.find_al
-00002230: 6c28 2774 6427 295d 0d0a 2020 2020 2020  l('td')]..      
-00002240: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00002250: 616e 6765 2830 2c20 6c65 6e28 726f 7773  ange(0, len(rows
-00002260: 292c 2039 293a 0d0a 2020 2020 2020 2020  ), 9):..        
-00002270: 2020 2020 2020 2020 726f 7720 3d20 726f          row = ro
-00002280: 7773 5b69 3a69 2b39 5d0d 0a20 2020 2020  ws[i:i+9]..     
-00002290: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-000022a0: 6c69 7374 2e61 7070 656e 6428 726f 7729  list.append(row)
-000022b0: 0d0a 2020 2020 6466 203d 2070 642e 4461  ..    df = pd.Da
-000022c0: 7461 4672 616d 6528 6461 7461 5f6c 6973  taFrame(data_lis
-000022d0: 742c 2063 6f6c 756d 6e73 3d5b 27e6 b8b8  t, columns=['...
-000022e0: e688 8fe6 a8a1 e5bc 8f27 2c20 27e5 9cb0  .........', '...
-000022f0: e59b be27 2c20 27e9 9abe e5ba a627 2c20  ...', '......', 
-00002300: 27e5 ae8c e688 90e6 97b6 e997 b427 2c20  '............', 
-00002310: 27e7 89b9 e684 9fe6 95b0 e987 8f27 2c20  '............', 
-00002320: 27e5 88b7 e696 b0e9 97b4 e99a 9427 2c20  '............', 
-00002330: 2742 e695 b0e4 bdbf e794 a827 2c20 27e5  'B.........', '.
-00002340: 88b7 e789 b9e6 a8a1 e5bc 8f27 2c20 2741  ...........', 'A
-00002350: 6e6e 65e7 8988 e69c ac27 5d29 0d0a 2020  nne......'])..  
-00002360: 2020 7265 7475 726e 2064 66                return df
+00000080: 2e2e 7365 6163 6820 696d 706f 7274 202a  ..seach import *
+00000090: 0d0a 6672 6f6d 202e 2e6c 3464 325f 6461  ..from ..l4d2_da
+000000a0: 7461 2e70 6c61 7965 7273 2069 6d70 6f72  ta.players impor
+000000b0: 7420 4c34 4432 506c 6179 6572 0d0a 6672  t L4D2Player..fr
+000000c0: 6f6d 202e 2e6c 3464 325f 696d 6167 6520  om ..l4d2_image 
+000000d0: 696d 706f 7274 206f 7574 5f70 6e67 0d0a  import out_png..
+000000e0: 2320 6672 6f6d 202e 616e 6e65 5f74 656c  # from .anne_tel
+000000f0: 6563 6f6d 2069 6d70 6f72 7420 414e 4e45  ecom import ANNE
+00000100: 5f41 5049 0d0a 0d0a 0d0a 7320 3d20 4c34  _API......s = L4
+00000110: 4432 506c 6179 6572 2829 0d0a 0d0a 2020  D2Player()....  
+00000120: 2020 0d0a 6173 796e 6320 6465 6620 616e    ..async def an
+00000130: 6e65 5f68 746d 6c28 6e61 6d65 3a73 7472  ne_html(name:str
+00000140: 293a 0d0a 2020 2020 2222 22e6 909c e7b4  ):..    """.....
+00000150: a2e9 878c e68f 90e5 8f96 e78e a9e5 aeb6  ................
+00000160: e4bf a1e6 81af efbc 8ce8 bf94 e59b 9ee5  ................
+00000170: 8897 e8a1 a8e5 ad97 e585 b822 2222 200d  ...........""" .
+00000180: 0a20 2020 2064 6174 615f 7469 746c 6520  .    data_title 
+00000190: 3d20 616e 6e65 5f73 6561 7263 6828 6e61  = anne_search(na
+000001a0: 6d65 290d 0a20 2020 2064 6174 6120 3d20  me)..    data = 
+000001b0: 6461 7461 5f74 6974 6c65 5b30 5d0d 0a20  data_title[0].. 
+000001c0: 2020 2074 6974 6c65 203d 2064 6174 615f     title = data_
+000001d0: 7469 746c 655b 315d 0d0a 2020 2020 6966  title[1]..    if
+000001e0: 206c 656e 2864 6174 6129 203d 3d30 206f   len(data) ==0 o
+000001f0: 7220 6461 7461 5b30 5d20 3d3d 2022 4e6f  r data[0] == "No
+00000200: 2050 6c61 7965 7220 666f 756e 642e 223a   Player found.":
+00000210: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000220: 207b 7d0d 0a20 2020 2064 6174 615f 6c69   {}..    data_li
+00000230: 7374 3a6c 6973 7420 3d20 5b5d 0d0a 2020  st:list = []..  
+00000240: 2020 6c6f 6767 6572 2e69 6e66 6f28 6461    logger.info(da
+00000250: 7461 290d 0a20 2020 2066 6f72 2069 2069  ta)..    for i i
+00000260: 6e20 6461 7461 3a0d 0a20 2020 2020 2020  n data:..       
+00000270: 2069 3a42 6561 7574 6966 756c 536f 7570   i:BeautifulSoup
+00000280: 0d0a 2020 2020 2020 2020 7472 793a 0d0a  ..        try:..
+00000290: 2020 2020 2020 2020 2020 2020 5261 6e6b              Rank
+000002a0: 203d 2069 2e66 696e 6428 2774 6427 2c20   = i.find('td', 
+000002b0: 7b27 6461 7461 2d74 6974 6c65 273a 2027  {'data-title': '
+000002c0: 5261 6e6b 3a27 7d29 2e74 6578 742e 7374  Rank:'}).text.st
+000002d0: 7269 7028 290d 0a20 2020 2020 2020 2020  rip()..         
+000002e0: 2020 2070 6c61 7965 7220 3d20 692e 6669     player = i.fi
+000002f0: 6e64 2827 7464 272c 207b 2764 6174 612d  nd('td', {'data-
+00000300: 7469 746c 6527 3a20 2750 6c61 7965 723a  title': 'Player:
+00000310: 277d 292e 7465 7874 2e73 7472 6970 2829  '}).text.strip()
+00000320: 0d0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+00000330: 696e 7473 203d 2069 2e66 696e 6428 2774  ints = i.find('t
+00000340: 6427 2c20 7b27 6461 7461 2d74 6974 6c65  d', {'data-title
+00000350: 273a 2027 506f 696e 7473 3a27 7d29 2e74  ': 'Points:'}).t
+00000360: 6578 742e 7374 7269 7028 290d 0a20 2020  ext.strip()..   
+00000370: 2020 2020 2020 2020 2023 2063 6f75 6e74           # count
+00000380: 7279 203d 2069 2e66 696e 6428 2769 6d67  ry = i.find('img
+00000390: 2729 5b27 616c 7427 5d0d 0a20 2020 2020  ')['alt']..     
+000003a0: 2020 2020 2020 2070 6c61 7974 696d 6520         playtime 
+000003b0: 3d20 692e 6669 6e64 2827 7464 272c 207b  = i.find('td', {
+000003c0: 2764 6174 612d 7469 746c 6527 3a20 2750  'data-title': 'P
+000003d0: 6c61 7974 696d 653a 277d 292e 7465 7874  laytime:'}).text
+000003e0: 2e73 7472 6970 2829 0d0a 2020 2020 2020  .strip()..      
+000003f0: 2020 2020 2020 6c61 7374 5f6f 6e6c 696e        last_onlin
+00000400: 6520 3d20 692e 6669 6e64 2827 7464 272c  e = i.find('td',
+00000410: 207b 2764 6174 612d 7469 746c 6527 3a20   {'data-title': 
+00000420: 274c 6173 7420 4f6e 6c69 6e65 3a27 7d29  'Last Online:'})
+00000430: 2e74 6578 742e 7374 7269 7028 290d 0a20  .text.strip().. 
+00000440: 2020 2020 2020 2065 7863 6570 7420 4174         except At
+00000450: 7472 6962 7574 6545 7272 6f72 3a0d 0a20  tributeError:.. 
+00000460: 2020 2020 2020 2020 2020 2052 616e 6b20             Rank 
+00000470: 3d20 692e 6669 6e64 2827 7464 272c 207b  = i.find('td', {
+00000480: 2764 6174 612d 7469 746c 6527 3a20 27e6  'data-title': '.
+00000490: 8e92 e590 8d3a 277d 292e 7465 7874 2e73  .....:'}).text.s
+000004a0: 7472 6970 2829 0d0a 2020 2020 2020 2020  trip()..        
+000004b0: 2020 2020 706c 6179 6572 203d 2069 2e66      player = i.f
+000004c0: 696e 6428 2774 6427 2c20 7b27 6461 7461  ind('td', {'data
+000004d0: 2d74 6974 6c65 273a 2027 e78e a9e5 aeb6  -title': '......
+000004e0: 3a27 7d29 2e74 6578 742e 7374 7269 7028  :'}).text.strip(
+000004f0: 290d 0a20 2020 2020 2020 2020 2020 2070  )..            p
+00000500: 6f69 6e74 7320 3d20 692e 6669 6e64 2827  oints = i.find('
+00000510: 7464 272c 207b 2764 6174 612d 7469 746c  td', {'data-titl
+00000520: 6527 3a20 27e5 8886 e695 b03a 277d 292e  e': '......:'}).
+00000530: 7465 7874 2e73 7472 6970 2829 0d0a 2020  text.strip()..  
+00000540: 2020 2020 2020 2020 2020 706c 6179 7469            playti
+00000550: 6d65 203d 2069 2e66 696e 6428 2774 6427  me = i.find('td'
+00000560: 2c20 7b27 6461 7461 2d74 6974 6c65 273a  , {'data-title':
+00000570: 2027 e6b8 b8e7 8ea9 e697 b6e9 97b4 3a27   '............:'
+00000580: 7d29 2e74 6578 742e 7374 7269 7028 290d  }).text.strip().
+00000590: 0a20 2020 2020 2020 2020 2020 206c 6173  .            las
+000005a0: 745f 6f6e 6c69 6e65 203d 2069 2e66 696e  t_online = i.fin
+000005b0: 6428 2774 6427 2c20 7b27 6461 7461 2d74  d('td', {'data-t
+000005c0: 6974 6c65 273a 2027 e69c 80e5 908e e4b8  itle': '........
+000005d0: 8ae7 babf e697 b6e9 97b4 3a27 7d29 2e74  ..........:'}).t
+000005e0: 6578 742e 7374 7269 7028 290d 0a20 2020  ext.strip()..   
+000005f0: 2020 2020 206f 6e63 6c69 636b 203d 2069       onclick = i
+00000600: 5b27 6f6e 636c 6963 6b27 5d0d 0a20 2020  ['onclick']..   
+00000610: 2020 2020 2073 7465 616d 6964 203d 206f       steamid = o
+00000620: 6e63 6c69 636b 2e73 706c 6974 2827 3d27  nclick.split('='
+00000630: 295b 325d 2e73 7472 6970 2822 2722 290d  )[2].strip("'").
+00000640: 0a20 2020 2020 2020 2070 6c61 795f 6a73  .        play_js
+00000650: 6f6e 203d 7b0d 0a20 2020 2020 2020 2020  on ={..         
+00000660: 2020 2074 6974 6c65 5b30 5d3a 5261 6e6b     title[0]:Rank
+00000670: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00000680: 6974 6c65 5b31 5d3a 706c 6179 6572 2c0d  itle[1]:player,.
+00000690: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
+000006a0: 6c65 5b32 5d3a 706f 696e 7473 2c0d 0a20  le[2]:points,.. 
+000006b0: 2020 2020 2020 2020 2020 2023 2074 6974             # tit
+000006c0: 6c65 5b33 5d3a 636f 756e 7472 792c 0d0a  le[3]:country,..
+000006d0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+000006e0: 655b 335d 3a70 6c61 7974 696d 652c 0d0a  e[3]:playtime,..
+000006f0: 2020 2020 2020 2020 2020 2020 7469 746c              titl
+00000700: 655b 345d 3a6c 6173 745f 6f6e 6c69 6e65  e[4]:last_online
+00000710: 2c0d 0a20 2020 2020 2020 2020 2020 2074  ,..            t
+00000720: 6974 6c65 5b35 5d3a 7374 6561 6d69 640d  itle[5]:steamid.
+00000730: 0a20 2020 2020 2020 207d 0d0a 2020 2020  .        }..    
+00000740: 2020 2020 6461 7461 5f6c 6973 742e 6170      data_list.ap
+00000750: 7065 6e64 2870 6c61 795f 6a73 6f6e 290d  pend(play_json).
+00000760: 0a20 2020 206c 6f67 6765 722e 696e 666f  .    logger.info
+00000770: 2822 e690 9ce5 afbb e695 b0e6 8dae 2229  ("............")
+00000780: 0d0a 2020 2020 7265 7475 726e 2064 6174  ..    return dat
+00000790: 615f 6c69 7374 0d0a 0d0a 6465 6620 616e  a_list....def an
+000007a0: 6e65 5f68 746d 6c5f 6d73 6728 6461 7461  ne_html_msg(data
+000007b0: 5f6c 6973 743a 6c69 7374 293a 0d0a 2020  _list:list):..  
+000007c0: 2020 2222 22e4 bb8e e690 9ce7 b4a2 e7bb    """...........
+000007d0: 93e6 9e9c e79a 84e5 ad97 e585 b8e5 8897  ................
+000007e0: e8a1 a8e4 b8ad efbc 8ce8 bf94 e59b 9ee5  ................
+000007f0: 8f91 e980 81e4 bfa1 e681 af22 2222 0d0a  ..........."""..
+00000800: 2020 2020 6d65 7320 3d20 27e6 909c e7b4      mes = '.....
+00000810: a2e5 88b0 e4bb a5e4 b88b e78e a9e5 aeb6  ................
+00000820: e4bf a1e6 81af 270d 0a20 2020 206e 7320  ......'..    ns 
+00000830: 3d20 300d 0a20 2020 200d 0a20 2020 2066  = 0..    ..    f
+00000840: 6f72 206f 6e65 2069 6e20 6461 7461 5f6c  or one in data_l
+00000850: 6973 743a 0d0a 2020 2020 2020 2020 6f6e  ist:..        on
+00000860: 653a 6469 6374 0d0a 2020 2020 2020 2020  e:dict..        
+00000870: 6e73 202b 3d20 310d 0a20 2020 2020 2020  ns += 1..       
+00000880: 2078 203d 2036 0d0a 0d0a 2020 2020 2020   x = 6....      
+00000890: 2020 7469 746c 6573 203d 206c 6973 7428    titles = list(
+000008a0: 6f6e 652e 6b65 7973 2829 290d 0a20 2020  one.keys())..   
+000008b0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000008c0: 6e67 6528 7829 3a0d 0a20 2020 2020 2020  nge(x):..       
+000008d0: 2020 2020 206d 6573 202b 3d20 275c 6e27       mes += '\n'
+000008e0: 202b 2074 6974 6c65 735b 695d 202b 2027   + titles[i] + '
+000008f0: 3a27 202b 2073 7472 286f 6e65 5b74 6974  :' + str(one[tit
+00000900: 6c65 735b 695d 5d29 0d0a 2020 2020 2020  les[i]])..      
+00000910: 2020 6d65 7320 2b3d 2027 5c6e 2d2d 2d2d    mes += '\n----
+00000920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000930: 270d 0a20 2020 2020 2020 2069 6620 6e73  '..        if ns
+00000940: 3e34 3a0d 0a20 2020 2020 2020 2020 2020  >4:..           
+00000950: 2062 7265 616b 0d0a 2020 2020 7265 7475   break..    retu
+00000960: 726e 206d 6573 0d0a 0d0a 0d0a 2020 0d0a  rn mes......  ..
+00000970: 2020 200d 0a61 7379 6e63 2064 6566 2077     ..async def w
+00000980: 7269 7465 5f70 6c61 7965 7228 6964 2c6d  rite_player(id,m
+00000990: 7367 3a73 7472 2c6e 6963 6b6e 616d 653a  sg:str,nickname:
+000009a0: 7374 7229 3a0d 0a20 2020 2022 2222 e7bb  str):..    """..
+000009b0: 91e5 ae9a e794 a8e6 88b7 2222 220d 0a20  ..........""".. 
+000009c0: 2020 2023 20e5 88a4 e696 ade6 98af 7374     # .........st
+000009d0: 6561 6d0d 0a20 2020 2070 7269 6e74 286d  eam..    print(m
+000009e0: 7367 290d 0a20 2020 2069 6620 6d73 672e  sg)..    if msg.
+000009f0: 7374 6172 7473 7769 7468 2827 5354 4541  startswith('STEA
+00000a00: 4d27 293a 0d0a 2020 2020 2020 2020 2320  M'):..        # 
+00000a10: 7472 793a 0d0a 2020 2020 2020 2020 6461  try:..        da
+00000a20: 7461 5f74 7570 6c65 203d 2073 2e5f 7175  ta_tuple = s._qu
+00000a30: 6572 795f 706c 6179 6572 5f71 7128 6964  ery_player_qq(id
+00000a40: 290d 0a20 2020 2020 2020 2069 6620 6461  )..        if da
+00000a50: 7461 5f74 7570 6c65 2021 3d20 4e6f 6e65  ta_tuple != None
+00000a60: 3a0d 0a20 2020 2020 2020 2020 2020 2071  :..            q
+00000a70: 7120 2c20 6e69 636b 6e61 6d20 2c20 7374  q , nicknam , st
+00000a80: 6561 6d69 6420 3d20 6461 7461 5f74 7570  eamid = data_tup
+00000a90: 6c65 0d0a 2020 2020 2020 2020 656c 7365  le..        else
+00000aa0: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
+00000ab0: 6963 6b6e 616d 203d 204e 6f6e 650d 0a20  icknam = None.. 
+00000ac0: 2020 2020 2020 2061 7761 6974 2073 2e5f         await s._
+00000ad0: 6164 645f 706c 6179 6572 5f61 6c6c 2869  add_player_all(i
+00000ae0: 6420 2c20 6e69 636b 6e61 6d20 2c20 6d73  d , nicknam , ms
+00000af0: 6729 0d0a 2020 2020 2020 2020 2320 6578  g)..        # ex
+00000b00: 6365 7074 2054 7970 6545 7272 6f72 3a0d  cept TypeError:.
+00000b10: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
+00000b20: 7761 6974 2073 2e5f 6164 645f 706c 6179  wait s._add_play
+00000b30: 6572 5f73 7465 616d 6964 2869 6420 2c20  er_steamid(id , 
+00000b40: 6d73 6729 0d0a 2020 2020 2020 2020 6d65  msg)..        me
+00000b50: 7320 3d20 27e7 bb91 e5ae 9ae6 8890 e58a  s = '...........
+00000b60: 9fe5 96b5 7e5c 6e51 513a 2720 2b20 6e69  ....~\nQQ:' + ni
+00000b70: 636b 6e61 6d65 202b 275c 6e27 202b 2027  ckname +'\n' + '
+00000b80: 7374 6561 6d69 643a 272b 6d73 670d 0a20  steamid:'+msg.. 
+00000b90: 2020 2020 2020 2072 6574 7572 6e20 6d65         return me
+00000ba0: 730d 0a20 2020 2065 6c73 653a 0d0a 2020  s..    else:..  
+00000bb0: 2020 2020 2020 2320 7472 793a 0d0a 2020        # try:..  
+00000bc0: 2020 2020 2020 6461 7461 5f74 7570 6c65        data_tuple
+00000bd0: 203d 2073 2e5f 7175 6572 795f 706c 6179   = s._query_play
+00000be0: 6572 5f71 7128 6964 290d 0a20 2020 2020  er_qq(id)..     
+00000bf0: 2020 2069 6620 6461 7461 5f74 7570 6c65     if data_tuple
+00000c00: 2021 3d20 4e6f 6e65 3a0d 0a20 2020 2020   != None:..     
+00000c10: 2020 2020 2020 2069 6420 2c20 6e69 636b         id , nick
+00000c20: 6e61 6d20 2c20 7374 6561 6d69 6420 3d20  nam , steamid = 
+00000c30: 6461 7461 5f74 7570 6c65 0d0a 2020 2020  data_tuple..    
+00000c40: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00000c50: 2020 2020 2020 2073 7465 616d 6964 203d         steamid =
+00000c60: 204e 6f6e 650d 0a20 2020 2020 2020 2061   None..        a
+00000c70: 7761 6974 2073 2e5f 6164 645f 706c 6179  wait s._add_play
+00000c80: 6572 5f61 6c6c 2869 6420 2c20 6d73 6720  er_all(id , msg 
+00000c90: 2c20 7374 6561 6d69 6429 0d0a 2020 2020  , steamid)..    
+00000ca0: 2020 2020 2320 6578 6365 7074 2054 7970      # except Typ
+00000cb0: 6545 7272 6f72 3a0d 0a20 2020 2020 2020  eError:..       
+00000cc0: 2023 2020 2020 2061 7761 6974 2073 2e5f   #     await s._
+00000cd0: 6164 645f 706c 6179 6572 5f6e 6963 6b6e  add_player_nickn
+00000ce0: 616d 6528 6964 202c 206d 7367 2029 200d  ame(id , msg ) .
+00000cf0: 0a20 2020 2020 2020 206d 6573 203d 2027  .        mes = '
+00000d00: e7bb 91e5 ae9a e688 90e5 8a9f e596 b57e  ...............~
+00000d10: 5c6e 5151 3a27 202b 206e 6963 6b6e 616d  \nQQ:' + nicknam
+00000d20: 6520 2b27 5c6e 2720 2b20 2773 7465 616d  e +'\n' + 'steam
+00000d30: e698 b5e7 a7b0 3a27 2b6d 7367 0d0a 2020  ......:'+msg..  
+00000d40: 2020 2020 2020 7265 7475 726e 206d 6573        return mes
+00000d50: 0d0a 0d0a 2020 2020 2020 2020 0d0a 0d0a  ....        ....
+00000d60: 2020 2020 2020 2020 0d0a 6465 6620 6465          ..def de
+00000d70: 6c5f 706c 6179 6572 2869 643a 7374 7229  l_player(id:str)
+00000d80: 3a0d 0a20 2020 2022 2222 e588 a0e9 99a4  :..    """......
+00000d90: e7bb 91e5 ae9a e4bf a1e6 81af 2ce8 bf94  ............,...
+00000da0: e59b 9ee6 b688 e681 af22 2222 0d0a 2020  ........."""..  
+00000db0: 2020 6966 206e 6f74 2073 2e5f 7175 6572    if not s._quer
+00000dc0: 795f 706c 6179 6572 5f71 7128 6964 293a  y_player_qq(id):
+00000dd0: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000de0: 2027 e4bd a0e8 bf98 e6b2 a1e6 9c89 e7bb   '..............
+00000df0: 91e5 ae9a e8bf 87ef bc8c e8af b7e4 bdbf  ................
+00000e00: e794 a85b e6b1 82e7 949f e7bb 91e5 ae9a  ...[............
+00000e10: 2be6 98b5 e7a7 b02f 7374 6561 6d69 645d  +....../steamid]
+00000e20: 270d 0a20 2020 2069 6620 732e 5f64 656c  '..    if s._del
+00000e30: 6574 655f 706c 6179 6572 3a0d 0a20 2020  ete_player:..   
+00000e40: 2020 2020 2072 6574 7572 6e20 27e5 88a0       return '...
+00000e50: e999 a4e6 8890 e58a 9fe5 96b5 7e27 0d0a  ............~'..
+00000e60: 2020 2020 2020 2020 0d0a 0d0a 2020 2020          ....    
+00000e70: 0d0a 6173 796e 6320 6465 6620 6964 5f74  ..async def id_t
+00000e80: 6f5f 6d65 7328 6e61 6d65 3a73 7472 293a  o_mes(name:str):
+00000e90: 0d0a 2020 2020 2222 22e6 a0b9 e68d ae6e  ..    """......n
+00000ea0: 616d 65e4 bb8e e695 b0e6 8dae e5ba 932c  ame............,
+00000eb0: e8bf 94e5 9b9e 7374 6561 6d69 64e3 8081  ......steamid...
+00000ec0: e688 96e8 8085 e7a9 bae7 99bd 2222 220d  ............""".
+00000ed0: 0a20 2020 2064 6174 615f 7475 706c 6520  .    data_tuple 
+00000ee0: 3d20 6177 6169 7420 732e 7365 6172 6368  = await s.search
+00000ef0: 5f64 6174 6128 4e6f 6e65 2c6e 616d 652c  _data(None,name,
+00000f00: 4e6f 6e65 290d 0a20 2020 2070 7269 6e74  None)..    print
+00000f10: 2864 6174 615f 7475 706c 6529 0d0a 2020  (data_tuple)..  
+00000f20: 2020 6966 2064 6174 615f 7475 706c 653a    if data_tuple:
+00000f30: 0d0a 2020 2020 2020 2020 7374 6561 6d69  ..        steami
+00000f40: 6420 3d20 6461 7461 5f74 7570 6c65 5b32  d = data_tuple[2
+00000f50: 5d0d 0a20 2020 2020 2020 2072 6574 7572  ]..        retur
+00000f60: 6e20 7374 6561 6d69 640d 0a20 2020 2072  n steamid..    r
+00000f70: 6574 7572 6e20 4e6f 6e65 0d0a 2020 2020  eturn None..    
+00000f80: 0d0a 0d0a 6465 6620 616e 6e65 5f72 616e  ....def anne_ran
+00000f90: 6b5f 6469 6374 286e 616d 653a 7374 7229  k_dict(name:str)
+00000fa0: 3a0d 0a20 2020 2022 2222 e794 a873 7465  :..    """...ste
+00000fb0: 616d 6964 2ce6 9fa5 e8af a6e6 8385 2ce8  amid,.........,.
+00000fc0: be93 e587 bae5 ad97 e585 b822 2222 0d0a  ..........."""..
+00000fd0: 2020 2020 6461 7461 5f64 6963 7420 3d20      data_dict = 
+00000fe0: 7b7d 0d0a 2020 2020 7572 6c20 3d66 2768  {}..    url =f'h
+00000ff0: 7474 7073 3a2f 2f73 622e 7472 7967 656b  ttps://sb.trygek
+00001000: 2e63 6f6d 2f6c 3464 5f73 7461 7473 2f72  .com/l4d_stats/r
+00001010: 616e 6b69 6e67 2f70 6c61 7965 722e 7068  anking/player.ph
+00001020: 703f 7374 6561 6d69 643d 7b6e 616d 657d  p?steamid={name}
+00001030: 270d 0a20 2020 2068 6561 6465 7273 203d  '..    headers =
+00001040: 207b 0d0a 2020 2020 2020 2020 2755 7365   {..        'Use
+00001050: 722d 4167 656e 7427 3a27 4d6f 7a69 6c6c  r-Agent':'Mozill
+00001060: 612f 352e 3020 2857 696e 646f 7773 204e  a/5.0 (Windows N
+00001070: 5420 3130 2e30 3b20 5769 6e36 343b 2078  T 10.0; Win64; x
+00001080: 3634 3b20 7276 3a31 3037 2e30 2920 4765  64; rv:107.0) Ge
+00001090: 636b 6f2f 3230 3130 3031 3031 2046 6972  cko/20100101 Fir
+000010a0: 6566 6f78 2f31 3037 2e30 270d 0a20 2020  efox/107.0'..   
+000010b0: 207d 0d0a 2020 2020 6461 7461 203d 2068   }..    data = h
+000010c0: 7474 7078 2e67 6574 2875 726c 3d75 726c  ttpx.get(url=url
+000010d0: 2c68 6561 6465 7273 3d68 6561 6465 7273  ,headers=headers
+000010e0: 2c74 696d 656f 7574 3d35 290d 0a20 2020  ,timeout=5)..   
+000010f0: 2069 6620 6461 7461 2e73 7461 7475 735f   if data.status_
+00001100: 636f 6465 2021 3d20 3230 303a 0d0a 2020  code != 200:..  
+00001110: 2020 2020 2020 7265 7475 726e 205b 6622        return [f"
+00001120: e69f a5e8 afa2 e994 99e8 afaf efbc 8ce7  ................
+00001130: 8ab6 e680 81e7 a081 7b64 6174 612e 7374  ........{data.st
+00001140: 6174 7573 5f63 6f64 657d 225d 0d0a 2020  atus_code}"]..  
+00001150: 2020 6461 7461 203d 2064 6174 612e 636f    data = data.co
+00001160: 6e74 656e 742e 6465 636f 6465 2827 7574  ntent.decode('ut
+00001170: 662d 3827 290d 0a20 2020 2064 6174 6120  f-8')..    data 
+00001180: 3d20 4265 6175 7469 6675 6c53 6f75 7028  = BeautifulSoup(
+00001190: 6461 7461 2c20 2768 746d 6c2e 7061 7273  data, 'html.pars
+000011a0: 6572 2729 0d0a 2020 2020 6465 7461 696c  er')..    detail
+000011b0: 203d 2064 6174 612e 6669 6e64 5f61 6c6c   = data.find_all
+000011c0: 2827 7461 626c 6527 290d 0a20 2020 206e  ('table')..    n
+000011d0: 203d 2030 0d0a 2020 2020 7768 696c 6520   = 0..    while 
+000011e0: 6e20 3c20 323a 0d0a 2020 2020 2020 2020  n < 2:..        
+000011f0: 6461 7461 5f6c 6973 743a 4c69 7374 5b64  data_list:List[d
+00001200: 6963 745d 203d 205b 5d0d 0a20 2020 2020  ict] = []..     
+00001210: 2020 2064 6574 6169 6c32 203d 2064 6574     detail2 = det
+00001220: 6169 6c5b 6e5d 0d0a 2020 2020 2020 2020  ail[n]..        
+00001230: 7472 203d 2064 6574 6169 6c32 2e66 696e  tr = detail2.fin
+00001240: 645f 616c 6c28 2774 7227 290d 0a20 2020  d_all('tr')..   
+00001250: 2020 2020 2066 6f72 2069 2069 6e20 7472       for i in tr
+00001260: 3a0d 0a20 2020 2020 2020 2020 2020 2074  :..            t
+00001270: 6974 6c65 203d 2069 2e66 696e 6428 2774  itle = i.find('t
+00001280: 6427 2c20 7b27 636c 6173 7327 3a20 2777  d', {'class': 'w
+00001290: 2d35 3027 7d29 0d0a 2020 2020 2020 2020  -50'})..        
+000012a0: 2020 2020 7661 6c75 6520 3d20 7469 746c      value = titl
+000012b0: 652e 6669 6e64 5f6e 6578 745f 7369 626c  e.find_next_sibl
+000012c0: 696e 6728 2774 6427 290d 0a20 2020 2020  ing('td')..     
+000012d0: 2020 2020 2020 206e 6577 5f64 6963 7420         new_dict 
+000012e0: 3d20 7b74 6974 6c65 2e74 6578 743a 7661  = {title.text:va
+000012f0: 6c75 652e 7465 7874 7d0d 0a20 2020 2020  lue.text}..     
+00001300: 2020 2020 2020 2064 6174 615f 6469 6374         data_dict
+00001310: 2e75 7064 6174 6528 6e65 775f 6469 6374  .update(new_dict
+00001320: 290d 0a20 2020 2020 2020 2064 6174 615f  )..        data_
+00001330: 6c69 7374 2e61 7070 656e 6428 6461 7461  list.append(data
+00001340: 5f64 6963 7429 0d0a 2020 2020 2020 2020  _dict)..        
+00001350: 6e20 2b3d 2031 0d0a 2020 2020 2320 e88e  n += 1..    # ..
+00001360: b7e5 8f96 e5a4 b4e5 838f 0d0a 2020 2020  ............    
+00001370: 656c 656d 656e 743a 7374 7220 3d20 6461  element:str = da
+00001380: 7461 2e66 696e 645f 616c 6c28 6174 7472  ta.find_all(attr
+00001390: 733d 7b22 7374 796c 6522 3a20 2263 7572  s={"style": "cur
+000013a0: 736f 723a 706f 696e 7465 7222 7d29 5b30  sor:pointer"})[0
+000013b0: 5d2e 6765 7428 226f 6e63 6c69 636b 2229  ].get("onclick")
+000013c0: 0d0a 2020 2020 706c 6179 6572 5f75 726c  ..    player_url
+000013d0: 203d 2065 6c65 6d65 6e74 2e73 706c 6974   = element.split
+000013e0: 2822 2722 295b 315d 0d0a 2020 2020 6461  ("'")[1]..    da
+000013f0: 7461 5f6c 6973 745b 305d 2e75 7064 6174  ta_list[0].updat
+00001400: 6528 7b22 e4b8 aae4 baba e8b5 84e6 9699  e({"............
+00001410: 223a 706c 6179 6572 5f75 726c 7d29 0d0a  ":player_url})..
+00001420: 2020 2020 2320 e88e b7e5 8f96 e4b8 80e8      # ..........
+00001430: a880 0d0a 2020 2020 6d65 7373 6167 6520  ....    message 
+00001440: 3d20 6461 7461 2e73 656c 6563 7428 2268  = data.select("h
+00001450: 746d 6c20 626f 6479 2064 6976 2e63 6f6e  tml body div.con
+00001460: 7465 6e74 2e74 6578 742d 6365 6e74 6572  tent.text-center
+00001470: 2e74 6578 742d 6d64 2d6c 6566 7420 6469  .text-md-left di
+00001480: 762e 636f 6e74 6169 6e65 722e 7465 7874  v.container.text
+00001490: 2d6c 6566 7420 6469 762e 636f 6c2d 6d64  -left div.col-md
+000014a0: 2d31 322e 682d 3130 3020 6469 762e 6361  -12.h-100 div.ca
+000014b0: 7264 2d62 6f64 792e 776f 726c 646d 6170  rd-body.worldmap
+000014c0: 2e64 2d66 6c65 782e 666c 6578 2d63 6f6c  .d-flex.flex-col
+000014d0: 756d 6e2e 6a75 7374 6966 792d 636f 6e74  umn.justify-cont
+000014e0: 656e 742d 6365 6e74 6572 2e74 6578 742d  ent-center.text-
+000014f0: 6365 6e74 6572 2073 7061 6e22 290d 0a20  center span").. 
+00001500: 2020 206d 7367 5f6c 6973 7420 3d20 5b5d     msg_list = []
+00001510: 0d0a 2020 2020 666f 7220 6920 696e 206d  ..    for i in m
+00001520: 6573 7361 6765 3a0d 0a20 2020 2020 2020  essage:..       
+00001530: 206d 7367 5f6c 6973 742e 6170 7065 6e64   msg_list.append
+00001540: 2869 2e74 6578 7429 0d0a 2020 2020 6461  (i.text)..    da
+00001550: 7461 5f6c 6973 745b 305d 2e75 7064 6174  ta_list[0].updat
+00001560: 6528 7b22 e4b8 80e8 a880 223a 6d73 675f  e({"......":msg_
+00001570: 6c69 7374 7d29 0d0a 2020 2020 7265 7475  list})..    retu
+00001580: 726e 2064 6174 615f 6c69 7374 0d0a 0d0a  rn data_list....
+00001590: 6465 6620 616e 6e65 5f72 616e 6b5f 6469  def anne_rank_di
+000015a0: 6374 5f6d 7367 2864 6174 615f 6c69 7374  ct_msg(data_list
+000015b0: 293a 0d0a 2020 2020 2222 22e5 ad97 e585  ):..    """.....
+000015c0: b8e8 bdac 6d73 6722 2222 0d0a 2020 2020  ....msg"""..    
+000015d0: 6d73 6720 3d20 2727 0d0a 2020 2020 666f  msg = ''..    fo
+000015e0: 7220 6461 7461 5f64 6963 7420 696e 2064  r data_dict in d
+000015f0: 6174 615f 6c69 7374 3a0d 0a20 2020 2020  ata_list:..     
+00001600: 2020 206d 6573 203d 2027 270d 0a20 2020     mes = ''..   
+00001610: 2020 2020 2066 6f72 2069 2069 6e20 6461       for i in da
+00001620: 7461 5f64 6963 743a 0d0a 2020 2020 2020  ta_dict:..      
+00001630: 2020 2020 2020 6d65 7320 2b3d 275c 6e27        mes +='\n'
+00001640: 2b20 6920 2b20 6461 7461 5f64 6963 745b  + i + data_dict[
+00001650: 695d 0d0a 2020 2020 2020 2020 6d65 7320  i]..        mes 
+00001660: 2b3d 2027 5c6e 2d2d 2d2d 2d2d 2d2d 2d2d  += '\n----------
+00001670: 2d2d 2d2d 2d2d 2d2d 2d2d 270d 0a20 2020  ----------'..   
+00001680: 2020 2020 206d 7367 202b 3d20 6d65 730d       msg += mes.
+00001690: 0a20 2020 2072 6574 7572 6e20 6d73 670d  .    return msg.
+000016a0: 0a0d 0a0d 0a61 7379 6e63 2064 6566 2061  .....async def a
+000016b0: 6e6e 655f 6d65 7373 6761 6528 6e61 6d65  nne_messgae(name
+000016c0: 3a73 7472 2c75 7372 5f69 643a 7374 7229  :str,usr_id:str)
+000016d0: 3a0d 0a20 2020 2022 2222 e88e b7e5 8f96  :..    """......
+000016e0: 616e 6e65 e4bf a1e6 81af e58f afe8 be93  anne............
+000016f0: e587 bae4 bfa1 e681 af22 2222 0d0a 2020  ........."""..  
+00001700: 2020 6966 206e 616d 653a 0d0a 2020 2020    if name:..    
+00001710: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00001720: 22e5 85b3 e994 aee8 af8d e69f a5e8 afa2  "...............
+00001730: 2220 2b20 6e61 6d65 290d 0a20 2020 2020  " + name)..     
+00001740: 2020 2069 6620 6e6f 7420 6e61 6d65 2e73     if not name.s
+00001750: 7461 7274 7377 6974 6828 2753 5445 414d  tartswith('STEAM
+00001760: 2729 3a0d 0a20 2020 2020 2020 2020 2020  '):..           
+00001770: 2073 7465 616d 6964 203d 2061 7761 6974   steamid = await
+00001780: 2069 645f 746f 5f6d 6573 286e 616d 6529   id_to_mes(name)
+00001790: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000017a0: 206e 6f74 2073 7465 616d 6964 3a0d 0a20   not steamid:.. 
+000017b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000017c0: 6f67 6765 722e 696e 666f 2822 e6b2 a1e6  ogger.info("....
+000017d0: 9c89 e689 bee5 88b0 7171 efbc 8ce4 bdbf  ........qq......
+000017e0: e794 a8e9 bb98 e8ae a4e5 a4b4 e583 8f22  ..............."
+000017f0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+00001800: 2020 206d 6573 7361 6765 203d 2061 7761     message = awa
+00001810: 6974 2061 6e6e 655f 6874 6d6c 286e 616d  it anne_html(nam
+00001820: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00001830: 2020 2020 7573 725f 6964 203d 2022 3131      usr_id = "11
+00001840: 3435 3134 3931 3931 3831 3022 0d0a 2020  45149191810"..  
+00001850: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001860: 206c 656e 286d 6573 7361 6765 2920 3d3d   len(message) ==
+00001870: 2030 3a0d 0a20 2020 2020 2020 2020 2020   0:..           
+00001880: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00001890: 27e6 b2a1 e69c 89e5 8fab e8bf 99e4 b8aa  '...............
+000018a0: e590 8de5 ad97 e79a 842e 2e2e 5c6e 270d  ............\n'.
+000018b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000018c0: 2069 6620 6c65 6e28 6d65 7373 6167 6529   if len(message)
+000018d0: 203e 2031 3a0d 0a20 2020 2020 2020 2020   > 1:..         
+000018e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000018f0: 6e20 616e 6e65 5f68 746d 6c5f 6d73 6728  n anne_html_msg(
+00001900: 6d65 7373 6167 6529 0d0a 2020 2020 2020  message)..      
+00001910: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+00001920: 206d 6573 7361 6765 5b30 5d5b 2773 7465   message[0]['ste
+00001930: 616d 6964 275d 0d0a 2020 2020 2020 2020  amid']..        
+00001940: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+00001950: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+00001960: 3d20 7374 6561 6d69 640d 0a20 2020 2020  = steamid..     
+00001970: 2020 2023 2073 7465 616d 6964 0d0a 2020     # steamid..  
+00001980: 2020 2020 2020 6d73 6720 3d20 616e 6e65        msg = anne
+00001990: 5f72 616e 6b5f 6469 6374 286e 616d 6529  _rank_dict(name)
+000019a0: 5b30 5d0d 0a20 2020 2020 2020 2069 6620  [0]..        if 
+000019b0: 7479 7065 286d 7367 2920 3d3d 2064 6963  type(msg) == dic
+000019c0: 743a 0d0a 2020 2020 2020 2020 2020 2020  t:..            
+000019d0: 6d73 672e 7570 6461 7465 2861 7761 6974  msg.update(await
+000019e0: 2064 665f 746f 5f67 756f 6775 616e 6c76   df_to_guoguanlv
+000019f0: 2861 7761 6974 2061 6e6e 655f 6d61 705f  (await anne_map_
+00001a00: 6d73 6728 6e61 6d65 2929 290d 0a20 2020  msg(name)))..   
+00001a10: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00001a20: 696e 666f 2827 e4bd bfe7 94a8 e59b bee7  info('..........
+00001a30: 8987 2729 0d0a 2020 2020 2020 2020 2020  ..')..          
+00001a40: 2020 6d73 6720 3d20 6177 6169 7420 6f75    msg = await ou
+00001a50: 745f 706e 6728 7573 725f 6964 2c6d 7367  t_png(usr_id,msg
+00001a60: 290d 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00001a70: 6e20 6d73 670d 0a20 2020 2065 6c73 653a  n msg..    else:
+00001a80: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001a90: 2020 2020 2020 2031 e380 8171 713e e695         1...qq>..
+00001aa0: b0e6 8dae 3ee6 b2a1 e69c 89e6 95b0 e68d  ....>...........
+00001ab0: aeef bc8c e8bf 94e5 9b9e 0d0a 2020 2020  ............    
+00001ac0: 2020 2020 32e3 8081 7171 3ee6 95b0 e68d      2...qq>.....
+00001ad0: ae3e 7374 6561 6d69 643e e69f a5e8 afa2  .>steamid>......
+00001ae0: 0d0a 2020 2020 2020 2020 33e3 8081 7171  ..        3...qq
+00001af0: 3ee6 95b0 e68d ae3e e698 b5e7 a7b0 3ee6  >......>......>.
+00001b00: 9fa5 e8af a20d 0a20 2020 2020 2020 2022  .......        "
+00001b10: 2222 0d0a 2020 2020 2020 2020 6c6f 6767  ""..        logg
+00001b20: 6572 2e69 6e66 6f28 2271 71e4 bfa1 e681  er.info("qq.....
+00001b30: afe6 9fa5 e8af a222 290d 0a20 2020 2020  .......")..     
+00001b40: 2020 2064 6174 615f 7475 706c 6520 3d20     data_tuple = 
+00001b50: 732e 5f71 7565 7279 5f70 6c61 7965 725f  s._query_player_
+00001b60: 7171 2875 7372 5f69 6429 0d0a 2020 2020  qq(usr_id)..    
+00001b70: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+00001b80: 6461 7461 5f74 7570 6c65 290d 0a20 2020  data_tuple)..   
+00001b90: 2020 2020 2069 6620 6461 7461 5f74 7570       if data_tup
+00001ba0: 6c65 3d3d 204e 6f6e 653a 0d0a 2020 2020  le== None:..    
+00001bb0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
+00001bc0: 22e6 b2a1 e69c 89e7 bb91 e5ae 9ae4 bfa1  "...............
+00001bd0: e681 af2e 2e2e e8af b7e4 bdbf e794 a8e3  ................
+00001be0: 8090 e6b1 82e7 949f e7bb 91e5 ae9a 2078  .............. x
+00001bf0: 7878 e380 915c 6e22 0d0a 2020 2020 2020  xx...\n"..      
+00001c00: 2020 2320 e58f aae6 9c89 e590 8de5 ad97    # ............
+00001c10: efbc 8ce5 8588 e69f a5e8 afa2 e695 b0e6  ................
+00001c20: 8dae e59c a8e5 88a4 e696 ad0d 0a20 2020  .............   
+00001c30: 2020 2020 2065 6c69 6620 6461 7461 5f74       elif data_t
+00001c40: 7570 6c65 5b32 5d3a 0d0a 2020 2020 2020  uple[2]:..      
+00001c50: 2020 2020 2020 6e61 6d65 203d 2064 6174        name = dat
+00001c60: 615f 7475 706c 655b 325d 0d0a 2020 2020  a_tuple[2]..    
+00001c70: 2020 2020 656c 6966 2064 6174 615f 7475      elif data_tu
+00001c80: 706c 655b 315d 3a0d 0a20 2020 2020 2020  ple[1]:..       
+00001c90: 2020 2020 206e 616d 6520 3d20 6177 6169       name = awai
+00001ca0: 7420 6964 5f74 6f5f 6d65 7328 6461 7461  t id_to_mes(data
+00001cb0: 5f74 7570 6c65 5b31 5d29 0d0a 2020 2020  _tuple[1])..    
+00001cc0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00001cd0: 6e66 6f28 6e61 6d65 290d 0a20 2020 2020  nfo(name)..     
+00001ce0: 2020 2020 2020 2069 6620 6e6f 7420 6e61         if not na
+00001cf0: 6d65 3a0d 0a20 2020 2020 2020 2020 2020  me:..           
+00001d00: 2020 2020 206d 6573 7361 6765 203d 2061       message = a
+00001d10: 7761 6974 2061 6e6e 655f 6874 6d6c 2864  wait anne_html(d
+00001d20: 6174 615f 7475 706c 655b 315d 290d 0a20  ata_tuple[1]).. 
+00001d30: 2020 2020 2020 2020 2020 2020 2020 2075                 u
+00001d40: 7372 5f69 6420 3d20 2231 3134 3531 3439  sr_id = "1145149
+00001d50: 3139 3138 3130 220d 0a20 2020 2020 2020  191810"..       
+00001d60: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00001d70: 6d65 7373 6167 6529 203d 3d20 303a 0d0a  message) == 0:..
+00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d90: 2020 2020 7265 7475 726e 2027 e6b2 a1e6      return '....
+00001da0: 9c89 e58f abe8 bf99 e4b8 aae5 908d e5ad  ................
+00001db0: 97e7 9a84 2e2e 2e5c 6e27 0d0a 2020 2020  .......\n'..    
+00001dc0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
+00001dd0: 656e 286d 6573 7361 6765 2920 3e20 313a  en(message) > 1:
+00001de0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00001df0: 2020 2020 2020 7265 7475 726e 2061 6e6e        return ann
+00001e00: 655f 6874 6d6c 5f6d 7367 286d 6573 7361  e_html_msg(messa
+00001e10: 6765 290d 0a20 2020 2020 2020 2020 2020  ge)..           
+00001e20: 2020 2020 206e 616d 6520 3d20 6d65 7373       name = mess
+00001e30: 6167 655b 305d 5b27 7374 6561 6d69 6427  age[0]['steamid'
+00001e40: 5d0d 0a20 2020 2020 2020 2023 206e 616d  ]..        # nam
+00001e50: 65e6 98af 7374 6561 6d69 640d 0a20 2020  e...steamid..   
+00001e60: 2020 2020 206d 7367 203d 2061 6e6e 655f       msg = anne_
+00001e70: 7261 6e6b 5f64 6963 7428 6e61 6d65 295b  rank_dict(name)[
+00001e80: 305d 0d0a 2020 2020 2020 2020 6966 2074  0]..        if t
+00001e90: 7970 6528 6d73 6729 203d 3d20 6469 6374  ype(msg) == dict
+00001ea0: 3a0d 0a20 2020 2020 2020 2020 2020 206d  :..            m
+00001eb0: 7367 2e75 7064 6174 6528 6177 6169 7420  sg.update(await 
+00001ec0: 6466 5f74 6f5f 6775 6f67 7561 6e6c 7628  df_to_guoguanlv(
+00001ed0: 6177 6169 7420 616e 6e65 5f6d 6170 5f6d  await anne_map_m
+00001ee0: 7367 286e 616d 6529 2929 0d0a 2020 2020  sg(name)))..    
+00001ef0: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00001f00: 6e66 6f28 27e4 bdbf e794 a8e5 9bbe e789  nfo('...........
+00001f10: 8727 290d 0a20 2020 2020 2020 2020 2020  .')..           
+00001f20: 206d 7367 203d 2061 7761 6974 206f 7574   msg = await out
+00001f30: 5f70 6e67 2875 7372 5f69 642c 6d73 6729  _png(usr_id,msg)
+00001f40: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00001f50: 206d 7367 0d0a 2020 2020 0d0a 6173 796e   msg..    ..asyn
+00001f60: 6320 6465 6620 616e 6e65 5f6d 6170 5f6d  c def anne_map_m
+00001f70: 7367 2873 7465 616d 6964 3a73 7472 293a  sg(steamid:str):
+00001f80: 0d0a 2020 2020 2222 2273 7465 616d 6964  ..    """steamid
+00001f90: 2d3e e59c b0e5 9bbe e4bf a1e6 81af 2222  ->............""
+00001fa0: 220d 0a20 2020 2075 726c 203d 2066 2268  "..    url = f"h
+00001fb0: 7474 7073 3a2f 2f73 622e 7472 7967 656b  ttps://sb.trygek
+00001fc0: 2e63 6f6d 2f6c 3464 5f73 7461 7473 2f72  .com/l4d_stats/r
+00001fd0: 616e 6b69 6e67 2f74 696d 6564 6d61 7073  anking/timedmaps
+00001fe0: 2e70 6870 3f73 7465 616d 6964 3d7b 7374  .php?steamid={st
+00001ff0: 6561 6d69 647d 220d 0a20 2020 2068 6561  eamid}"..    hea
+00002000: 6465 7273 203d 207b 0d0a 2020 2020 2020  ders = {..      
+00002010: 2020 2755 7365 722d 4167 656e 7427 3a27    'User-Agent':'
+00002020: 4d6f 7a69 6c6c 612f 352e 3020 2857 696e  Mozilla/5.0 (Win
+00002030: 646f 7773 204e 5420 3130 2e30 3b20 5769  dows NT 10.0; Wi
+00002040: 6e36 343b 2078 3634 3b20 7276 3a31 3037  n64; x64; rv:107
+00002050: 2e30 2920 4765 636b 6f2f 3230 3130 3031  .0) Gecko/201001
+00002060: 3031 2046 6972 6566 6f78 2f31 3037 2e30  01 Firefox/107.0
+00002070: 270d 0a20 2020 207d 0d0a 2020 2020 6461  '..    }..    da
+00002080: 7461 203d 2068 7474 7078 2e67 6574 2875  ta = httpx.get(u
+00002090: 726c 2c68 6561 6465 7273 3d68 6561 6465  rl,headers=heade
+000020a0: 7273 2c74 696d 656f 7574 3d35 292e 636f  rs,timeout=5).co
+000020b0: 6e74 656e 742e 6465 636f 6465 2827 7574  ntent.decode('ut
+000020c0: 662d 3827 290d 0a20 2020 2073 6f75 7020  f-8')..    soup 
+000020d0: 3d20 4265 6175 7469 6675 6c53 6f75 7028  = BeautifulSoup(
+000020e0: 6461 7461 2c20 2768 746d 6c2e 7061 7273  data, 'html.pars
+000020f0: 6572 2729 0d0a 2020 2020 6461 7461 5f6c  er')..    data_l
+00002100: 6973 7420 3d20 5b5d 0d0a 2020 2020 6361  ist = []..    ca
+00002110: 7264 7320 3d20 736f 7570 2e73 656c 6563  rds = soup.selec
+00002120: 7428 2764 6976 2e63 6172 642e 726f 756e  t('div.card.roun
+00002130: 6465 642d 3027 290d 0a20 2020 2066 6f72  ded-0')..    for
+00002140: 2063 6172 6420 696e 2063 6172 6473 3a0d   card in cards:.
+00002150: 0a20 2020 2020 2020 2074 626f 6469 6573  .        tbodies
+00002160: 203d 2063 6172 642e 7365 6c65 6374 2827   = card.select('
+00002170: 7462 6f64 7927 290d 0a20 2020 2020 2020  tbody')..       
+00002180: 2066 6f72 2074 626f 6479 2069 6e20 7462   for tbody in tb
+00002190: 6f64 6965 733a 0d0a 2020 2020 2020 2020  odies:..        
+000021a0: 2020 2020 726f 7773 203d 205b 7464 2e74      rows = [td.t
+000021b0: 6578 742e 7374 7269 7028 2920 666f 7220  ext.strip() for 
+000021c0: 7464 2069 6e20 7462 6f64 792e 6669 6e64  td in tbody.find
+000021d0: 5f61 6c6c 2827 7464 2729 5d0d 0a20 2020  _all('td')]..   
+000021e0: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+000021f0: 6e20 7261 6e67 6528 302c 206c 656e 2872  n range(0, len(r
+00002200: 6f77 7329 2c20 3929 3a0d 0a20 2020 2020  ows), 9):..     
+00002210: 2020 2020 2020 2020 2020 2072 6f77 203d             row =
+00002220: 2072 6f77 735b 693a 692b 395d 0d0a 2020   rows[i:i+9]..  
+00002230: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00002240: 7461 5f6c 6973 742e 6170 7065 6e64 2872  ta_list.append(r
+00002250: 6f77 290d 0a20 2020 2064 6620 3d20 7064  ow)..    df = pd
+00002260: 2e44 6174 6146 7261 6d65 2864 6174 615f  .DataFrame(data_
+00002270: 6c69 7374 2c20 636f 6c75 6d6e 733d 5b27  list, columns=['
+00002280: e6b8 b8e6 888f e6a8 a1e5 bc8f 272c 2027  ............', '
+00002290: e59c b0e5 9bbe 272c 2027 e99a bee5 baa6  ......', '......
+000022a0: 272c 2027 e5ae 8ce6 8890 e697 b6e9 97b4  ', '............
+000022b0: 272c 2027 e789 b9e6 849f e695 b0e9 878f  ', '............
+000022c0: 272c 2027 e588 b7e6 96b0 e997 b4e9 9a94  ', '............
+000022d0: 272c 2027 42e6 95b0 e4bd bfe7 94a8 272c  ', 'B.........',
+000022e0: 2027 e588 b7e7 89b9 e6a8 a1e5 bc8f 272c   '............',
+000022f0: 2027 416e 6e65 e789 88e6 9cac 275d 290d   'Anne......']).
+00002300: 0a20 2020 2072 6574 7572 6e20 6466       .    return df
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/analysis.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/anne_telecom.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_anne/server.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_anne/server.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/players.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/players.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_data/serverip.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_data/serverip.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/ayromote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_file/remote.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_file/remote.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import List,Optional
 # from .htmlimg import dict_to_dict_img
 # from ..l4d2_anne.anne_telecom import ANNE_API
 from ..config import TEXT_PATH
 from .download import get_head_by_user_id_and_save
 from .send_image_tool import convert_img
 import jinja2
-from ..config import l4_style
+from ..config import l4_config
 template_path = TEXT_PATH/"template"
 
 env = jinja2.Environment(
     loader=jinja2.FileSystemLoader(template_path), enable_async=True
 )
 
 async def out_png(usr_id,data_dict:dict):
@@ -83,15 +83,15 @@
     pic = await get_help_img(msg_list)
 
     return pic
 
 
 async def get_help_img(plugins: List[dict]) -> Optional[bytes]:
     try:
-        if l4_style == 'black':
+        if l4_config.l4_style == 'black':
             template = env.get_template("help_dack.html")
         else:
             template = env.get_template("help.html")
         content = await template.render_async(plugins=plugins)
         return await html_to_pic(
             content,
             wait=0,
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/download.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/download.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/htmlimg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/send_image_tool.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/steam.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/steam.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_image/vtfs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     msg_dict['name'] =  msg.server_name
     msg_dict['map_'] =  msg.map_name
     msg_dict['players'] =  msg.player_count
     msg_dict['max_players'] =  msg.max_players
     msg_dict['rank_players'] =  f'{msg.player_count}/{msg.max_players}'
     msg_dict['ip'] = str(ip) + ':' +str(port)
     msg_dict['ping'] = f"{msg.ping*1000:.0f}ms"
+    msg_dict['system'] =  f"{msg.platform}.svg"
     if msg_dict['players'] < msg_dict['max_players']:
         msg_dict['enabled'] = True
     else:
         msg_dict['enabled'] = False
     return msg_dict
     
 async def player_queries_anne_dict(ip:str,port:int): 
@@ -95,8 +96,19 @@
     if hours > 0:
         time_str += f"{int(hours)}h "
     if minutes > 0 or hours > 0:
         time_str += f"{int(minutes)}m "
     time_str += f"{int(seconds)}s"
     return time_str.strip()
 
+async def server_rule_dict(ip:str,port:int): 
+    port = int(port)
+    ip = str(ip)
+    msg_dict = {}
+    # message_dict = await l4d(ip,port)
+    try:
+        msg:dict = await a2s.arules((ip,port))
+        msg_dict['tick'] = msg['l4d2_tickrate_enabler'] + "tick"
+    except:
+        msg_dict['tick'] = ''
+    return msg_dict
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/api.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             return file.json()
     elif mode == 'ip':
         rep:dict = file.json()
         try:
             logger.error(rep['error_'])
         except:
             pass
+        print(file.json())
         return file.json()
     elif mode == 'first':
         ip_tag:list = file.json()
         return ip_tag
         
 
 async def map_dict_to_str(data:List[dict]):
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/ohter.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_queries/qqgroup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ..l4d2_data.serverip import L4D2Server
 from ..l4d2_image import server_ip_pic
-from . import queries,player_queries,queries_dict,player_queries_anne_dict,msg_ip_to_list
+from . import queries,player_queries,queries_dict,player_queries_anne_dict,msg_ip_to_list,server_rule_dict
 from nonebot.log import logger
 import random
 import asyncio
 import re
 from ..message import PRISON,QUEREN,KAILAO
 from .ohter import ALL_HOST
 from typing import List,Dict
@@ -48,15 +48,15 @@
         number,qqgroup,host,port = i
         msg2 = await player_queries(host,port)
         msg1 = await queries(host,port)
         messsage += '序号、'+ str(number) + '\n' + msg1 + msg2 + '--------------------\n'
     return messsage
             
             
-async def qq_ip_querie(msg: list,igr:bool):
+async def qq_ip_querie(msg: list,igr:bool = True):
     msg_list = []
     tasks = []  # 用来保存异步任务
     if msg != []:
         for i in msg:
             try:
                 number, host, port = i
                 qqgroup = ''
@@ -65,14 +65,17 @@
             finally:
                 # 将异步任务添加到任务列表中
                 tasks.append(asyncio.create_task(process_message(number, host, port, msg_list,qqgroup,igr)))
         # 等待所有异步任务完成
         await asyncio.gather(*tasks)
         # 对msg_list按照number顺序排序
         msg_list.sort(key=lambda x: x['number'])
+        for i in msg_list:
+            print(i)
+            break
         result = {'msg_list': msg_list}
 
     else:
         result = {}
     return result
 
 
@@ -87,15 +90,17 @@
 
 
 
 async def process_message(number, host, port, msg_list:list,igr:bool,qqgroup = ''):
     try:
         msg2 = await player_queries_anne_dict(host, port)
         msg1 = await queries_dict(host, port)
+        msg3 = await server_rule_dict(host, port)
         msg1.update({'Players':msg2,'number':number,})
+        msg1.update(msg3)
         if qqgroup:
             msg1.update({'tag':qqgroup})
         msg_list.append(msg1)
     except errors:
         if igr:
             pass
         else:
@@ -212,15 +217,15 @@
         return str(host) + ':' + str(port)
     except TypeError:
         return None
 
 def split_maohao(msg:str) -> list:
     """分割大小写冒号"""
     msg:list = re.split(":|：",msg.strip())
-    mse = [msg[0],msg[-1]] if msg[0] != msg[-1] else [msg[0],20715]
+    mse = [msg[0],msg[-1]] if len(msg)==2 else [msg[0],20715]
     return mse
 
 async def write_json(data_str: str):
     """
     添加数据或者删除数据
      - 【求生更新 添加 腐竹 ip 模式 序号】
      - 【求生更新 添加 腐竹 ip 模式】
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/__init__.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_server/workshop.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_server/workshop.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/web.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/web.py`

 * *Files 21% similar despite different names*

```diff
@@ -99,56 +99,63 @@
             }
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
             }
 
-    @app.post('/l4d2/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def post_chat_global_config(data: dict):
+    @app.post('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def post_l4d2_global_config(data: dict):
         config_manager.config.update(**data)
         config_manager.save()
         return {
             'status': 0,
             'msg':    '保存成功'
         }
 
-    @app.get('/l4d2/api/chat_global_config', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_global_config():
+    @app.get('/l4d2/api/l4d2_global_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_global_config():
         try:
             bot = get_bot()
             groups = await bot.get_group_list()
             member_list = []
             for group in groups:
                 members = await bot.get_group_member_list(group_id=group['group_id'])
                 member_list.extend(
                     [{'label': f'{member["nickname"] or member["card"]}({member["user_id"]})',
                       'value': member['user_id']}
                      for
                      member in members])
             config = config_manager.config.dict(exclude={'group_config'})
             config['member_list'] = member_list
+            config['l4_styles'] = ['standard','black']
+
             return config
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '获取群和好友列表失败，请确认已连接GOCQ'
             }
             
-    @app.get('/l4d2/api/get_chat_contexts', response_class=JSONResponse, dependencies=[authentication()])
-    async def get_chat_context():
+    @app.get('/l4d2/api/get_query_contexts', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_query_context():
         try:
             from ..command import ALL_HOST
             this_ips = ALL_HOST
             ip_lists = []
             for ip_list, v in this_ips.items():
                 for d in v:
                     host, port = split_maohao(d['ip'])
                     ip_lists.append((d['id'], ip_list, host, port))
             data_dict = await qq_ip_querie(ip_lists)
+            if not data_dict:
+                return{
+                'status': -100,
+                'msg':    '返回失败，请确保有可用的服务器ip' 
+                }
             data_list = data_dict['msg_list']
             return {
                 'status': 0,
                 'msg': 'ok',
                 'data': {
                     'items': data_list,
                     'total': len(data_list),
@@ -156,24 +163,72 @@
             }
         except ValueError:
             return {
                 'status': -100,
                 'msg':    '返回失败，请确保网络连接正常'
             }
 
+    @app.get('/l4d2/api/get_l4d2_messages', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_messages():
+        try:
+            l4_ipall = config_manager.config.l4_ipall
+            config = [{'label': item['server_id'] , 'value': item['id_rank']}
+                for item in l4_ipall]
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': {'server_list':config}
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
+    @app.get('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def get_l4d2_server_config(id_rank :str):
+        try:
+            l4_ipall = config_manager.config.l4_ipall
+            config = {}
+            for item in l4_ipall:
+                if item['id_rank'] == id_rank :
+                    item['place'] = item['place'] == 'True' or item['place'] == True
+                    config = item
+                    break
+            return {
+                'status': 0,
+                'msg': 'ok',
+                'data': config
+            }
+        except ValueError:
+            return {
+                'status': -100,
+                'msg':    '返回失败，请确保网络连接正常'
+            }
+        
+    @app.post('/l4d2/api/l4d2_server_config', response_class=JSONResponse, dependencies=[authentication()])
+    async def post_l4d2_server_config(id_rank :str,data: dict):
+        for one in config_manager.config.l4_ipall:
+            if one['id_rank']==id_rank:
+                one.update(**data)
+        config_manager.save()
+        return {
+            'status': 0,
+            'msg':    '保存成功'
+        }        
 
+        
     @app.get('/l4d2', response_class=RedirectResponse)
     async def redirect_page():
         return RedirectResponse('/l4d2/login')
 
     @app.get('/l4d2/login', response_class=HTMLResponse)
     async def login_page_app():
         return login_page.render(site_title='登录 | l4d2 后台管理',
                                  theme='ang')
 
     @app.get('/l4d2/admin', response_class=HTMLResponse)
     async def admin_page_app():
-        return admin_app.render(site_title='l4d2-Chat 后台管理',
+        return admin_app.render(site_title='l4d2-l4d2 后台管理',
                                 theme='ang',
                                 requestAdaptor=requestAdaptor,
                                 responseAdaptor=responseAdaptor)
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/l4d2_web/webUI.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/l4d2_web/webUI.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..config import NICKNAME
 
 logo = Html(html='''
 <p align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server">
         <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png"
-         width="256" height="256" alt="Learning-Chat">
+         width="256" height="256" alt="l4d2-server">
     </a>
 </p>
 <h1 align="center">Nonebot-Plugin-L4d2-Server 控制台</h1>
 <div align="center">
     <a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/" target="_blank">
     Github仓库</a>
 </div>
@@ -40,71 +40,85 @@
 ], mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9, offset=5), redirect='/l4d2/admin')
 body = Wrapper(className='w-2/5 mx-auto my-0 m:w-full', body=login_form)
 login_page = Page(title='', body=[logo, body])
 
 global_config_form = Form(
     title='全局配置',
     name='global_config',
-    initApi='/l4d2/api/chat_global_config',
-    api='post:/l4d2/api/chat_global_config',
+    initApi='/l4d2/api/l4d2_global_config',
+    api='post:/l4d2/api/l4d2_global_config',
     body=[
-        Switch(label='求生功能总开关', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
+        Switch(label='控制总开关（摆设）', name='total_enable', value='${total_enable}', onText='开启', offText='关闭',
                labelRemark=Remark(shape='circle',
-                                  content='关闭后，全局都将禁用求生功能。')),
+                                  content='关闭后，禁用网页控制台，请参考文档启动方法')),
         InputText(label='后台管理用户名', name='web_username', value='${web_username}',
                   labelRemark=Remark(shape='circle',
                                      content='登录本后台管理所需要的用户名。')),
         InputPassword(label='后台管理密码', name='web_password', value='${web_password}',
                       labelRemark=Remark(shape='circle',
                                          content='登录本后台管理所需要的密码。')),
         InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
                   labelRemark=Remark(shape='circle',
                                      content='用于本后台管理加密验证token的密钥。')),
         InputText(label='查询key', name='l4_key', value='${l4_key}',
                   labelRemark=Remark(shape='circle',
-                                     content='用于获取拓展功能的key。')),
+                                     content='用于获取拓展功能的key,加q群399365126领取。')),
+        InputText(label='字体', name='l4_font', value='${l4_font}',
+                  labelRemark=Remark(shape='circle',
+                                     content='机器人返回图片中文字的字体。')),
+        Select(label='图片风格', name='l4_style', value='${l4_style}',source='${l4_styles}',
+                  labelRemark=Remark(shape='circle',
+                                     content='仅仅是批量查询的风格')),
+        InputTag(label='查询的远程服务器tag', name='l4_tag', value='${l4_tag}',
+                 enableBatchAdd=True,
+                 placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
+                 labelRemark=Remark(shape='circle',
+                                    content='在这里加入的用户，才能上传地图')),
         InputTag(label='求生上传地图用户', name='l4_master', value='${l4_master}',
                  enableBatchAdd=True,
                  placeholder='添加qq号', visibleOn='${total_enable}', joinValues=False, extractValue=True,
                  labelRemark=Remark(shape='circle',
                                     content='在这里加入的用户，才能上传地图')),
+
     ],
     actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
              Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
 upload_map_form = Form(
     title='全局配置',
     name='global_config',
-    api='post:/l4d2/api/chat_map_config',
+    api='post:/l4d2/api/l4d2_map_config',
     body=[
         InputText(label='服务器host', name='web_username', value='${web_username}',
                   labelRemark=Remark(shape='circle',
                                      content='127.0.0.1')),
         InputPassword(label='服务器', name='web_password', value='${web_password}',
                       labelRemark=Remark(shape='circle',
                                          content='登录本后台管理所需要的密码。')),
         InputText(label='后台管理token密钥', name='web_secret_key', value='${web_secret_key}',
                   labelRemark=Remark(shape='circle',
                                      content='用于本后台管理加密验证token的密钥。')),
         InputText(label='查询key', name='l4_key', value='${l4_key}',
                   labelRemark=Remark(shape='circle',
                                      content='用于获取拓展功能的key。')),
+
     ],
     actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
              Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
-group_select = Select(label='分群配置', name='group_id', source='${group_list}',
+
+group_select = Select(label='分群配置（暂未完成）', name='group_id', source='${group_list}',
                       placeholder='选择群')
 group_config_form = Form(
     title='分群配置（暂未完成）',
     visibleOn='group_id != null',
-    initApi='/l4d2/api/chat_group_config?group_id=${group_id}',
-    api='post:/l4d2/api/chat_group_config?group_id=${group_id}',
+    initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}',
+    api='post:/l4d2/api/l4d2_group_config?group_id=${group_id}',
     body=[
         Switch(label='分群开关', name='enable', value='${enable}', onText='开启', offText='关闭',
                labelRemark=Remark(shape='circle', content='针对该群的群聊学习开关，关闭后，仅该群不会学习和回复。')),
         InputNumber(label='占位符', name='answer_threshold', value='${answer_threshold}', visibleOn='${enable}',
                     min=2,
                     labelRemark=Remark(shape='circle', content='单文本')),
         InputTag(label='占位符', name='ban_words', value='${ban_words}', enableBatchAdd=True,
@@ -113,87 +127,110 @@
 
     ],
     actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
              ActionType.Ajax(
                  label='保存至所有群',
                  level=LevelEnum.primary,
                  confirmText='确认将当前配置保存至所有群？',
-                 api='post:/l4d2/api/chat_group_config?group_id=all'
+                 api='post:/l4d2/api/l4d2_group_config?group_id=all'
              ),
              Action(label='重置', level=LevelEnum.warning, type='reset')]
 )
 
-message_table = TableCRUD(
-    mode='table',
+server_control = Select(label='服务器设置', name='id_rank', source='${server_list}',
+                      placeholder='选择服务器')
+
+server_ditail= Form(
     title='',
-    syncLocation=False,
-    api='/l4d2/api/get_chat_messages',
-    interval=12000,
-    footable=True,
-    columns=[TableColumn(label='序号', name='message_id'),
-            TableColumn(label='服务器ip', name='group_id', searchable=True),
-            TableColumn(label='服务器端口', name='user_id', searchable=True),
-            TableColumn(type='tpl', tpl='${raw_message|truncate:20}', label='rcon密码',
-                        name='message',
-                        searchable=True, popOver={'mode':      'dialog', 'title': '消息全文',
-                                                    'className': 'break-all',
-                                                    'body':      {'type': 'tpl',
-                                                                'tpl':  '${raw_message}'}}),
-            TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}', label='时间',
-                        name='time', sortable=True)
-            ])
+    api='post:/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
+    initApi='/l4d2/api/l4d2_server_config?id_rank=${id_rank}',
+    visibleOn='id_rank != null',
+    body=[
+        Switch(label='是否是远程服务器', name='place', value='${place}', onText='是的', offText='不是',
+               labelRemark=Remark(shape='circle',
+                                  content='开启则确认为远程服务器')),
+        InputText(label='服务器名称', name='server_id', value='${server_id}',
+                  labelRemark=Remark(shape='circle',
+                                     content='服务器名字')),
+        InputText(label='服务器ip地址', name='host', value='${host}',
+                  labelRemark=Remark(shape='circle',
+                                     content='服务端所在ip地址,也可以是域名')),
+        InputText(label='所在端口', name='port', value='${port}',
+                      labelRemark=Remark(shape='circle',
+                                         content='服务端所在端口')),
+        InputPassword(label='rcon控制台密码', name='rcon', value='${rcon}',
+                      labelRemark=Remark(shape='circle',
+                                         content='服务端rcon密码')),
+        InputText(label='服务器本地文件位置', name='location', value='${location}',
+                      labelRemark=Remark(shape='circle',
+                                         content='求生服务器所在路径,该路径下有文件srcds_run')),        
+        InputText(label='远程账户', name='account', value='${account}',
+                  visibleOn='${place}',
+                  labelRemark=Remark(shape='circle',
+                                     content='远程服务器的登录账户名')),
+        InputPassword(label='远程密码', name='password', value='${password}',
+                      visibleOn='${place}',
+                  labelRemark=Remark(shape='circle',
+                                     content='远程服务器的登录密码')),
+    ],
+    actions=[Action(label='保存', level=LevelEnum.success, type='submit'),
+             Action(label='重置', level=LevelEnum.warning, type='reset')]
+)
 
-context_table = TableCRUD(mode='table',
+query_table = TableCRUD(mode='table',
                           title='',
                           syncLocation=False,
-                          api='/l4d2/api/get_chat_contexts',
+                          api='/l4d2/api/get_query_contexts',
                           interval=60000,
                           footable=True,
                           itemActions=[ActionType.Url(
                                 tooltip='加入游戏',
                                 icon='fa fa-gamepad',
                                 confirmText = "加入steam://connect/"+'${ip}',
                                 url= "steam://connect/"+'${ip}',
                                 # url= "http://"+'${ip}',
                                 blank= True
                                  ),
                             ],
                           columns = [
-                                    TableColumn(label='服主', name='tag', searchable=True),
+                                    TableColumn(label='服主', name='master', searchable=True),
                                     TableColumn(label='名称', name='name', searchable=True),
                                     TableColumn(label='地图', name='map_', searchable=True),
                                     TableColumn(label='玩家', name='rank_players', searchable=True),
                                     TableColumn(label='延迟', name='ping', searchable=True),
                                     TableColumn(label='IP 地址', name='ip', searchable=True),
                                     ])
 
-message_page = PageSchema(url='/messages', icon='fa fa-comments', label='本地服务器管理',
-                          schema=Page(title='本地服务器管理', body=[
+server_page = PageSchema(url='/messages', icon='fa fa-comment', label='本地服务器管理',
+                          schema=Page(title='本地服务器管理',
+                                      interval=120000,
+                                      initApi='/l4d2/api/get_l4d2_messages',
+                                        body=[
                               Alert(level=LevelEnum.info,
                                     className='white-space-pre-wrap',
                                     body=(f'此数据库记录了{NICKNAME}所在服务器下的求生服务器。\n'
 
                                           f'· 功能暂未完善')),
-                              message_table]))
-context_page = PageSchema(url='/contexts', icon='fa fa-comment', label='远程服务器查询',
+                              server_control,server_ditail]))
+query_page = PageSchema(url='/contexts', icon='fa fa-comments', label='远程服务器查询',
                           schema=Page(title='远程服务器查询',
                                       body=[Alert(level=LevelEnum.info,
                                                   className='white-space-pre-wrap',
                                                   body=(f'此数据库记录了{NICKNAME}所记录可查询的服务器ip。\n'
                                                         # '· 点击"回复列表"可以查看该条内容已学习到的可能的回复。\n'
                                                         # '· 点击"禁用"可以将该学习进行禁用，以后不会再学。\n'
                                                         f'· 功能暂未完善')),
-                                            context_table]))
+                                            query_table]))
 
 database_page = PageSchema(label='数据库', icon='fa fa-database',
-                           children=[message_page, context_page])
+                           children=[server_page, query_page])
 config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-wrench', label='配置',
                          schema=Page(title='配置', initApi='/l4d2/api/get_group_list',
-                                     body=[global_config_form, group_select, group_config_form]))
-chat_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
+                                     body=[global_config_form,group_select, group_config_form]))
+l4d2_page = PageSchema(label='求生之路', icon='fa fa-wechat (alias)', children=[config_page, database_page])
 
 github_logo = Tpl(className='w-full',
                   tpl='<div class="flex justify-between"><div></div><div><a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server" target="_blank" title="Copyright"><i class="fa fa-github fa-2x"></i></a></div></div>')
 header = Flex(className='w-full', justify='flex-end', alignItems='flex-end', items=[github_logo])
 
 admin_app = App(brandName='L4d2-Server',
                 logo='https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png',
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 from amis import ActionType, TableCRUD, TableColumn from amis import
 PageSchema, Switch, InputNumber, InputTag, Action, App from amis import Form,
 InputText, InputPassword, DisplayModeEnum, Horizontal, Remark, Html, Page,
 AmisAPI, Wrapper from amis import LevelEnum, Select, Alert, Tpl, Flex from
 ..config import NICKNAME logo = Html(html='''
-                                [Learning-Chat]
+                                 [l4d2-server]
               ****** Nonebot-Plugin-L4d2-Server æ§å¶å° ******
                                  Githubä»åº
 
 
 ''') login_api = AmisAPI( url='/l4d2/api/login', method='post', adaptor=''' if
 (payload.status == 0) { localStorage.setItem("token", payload.data.token); }
 return payload; ''' ) login_form = Form(api=login_api, title='', body=
@@ -15,108 +15,135 @@
 (shape='circle', content='åå°ç®¡çç¨æ·åï¼é»è®¤ä¸ºl4d2')),
 InputPassword(name='password', label='å¯ç ', labelRemark=Remark
 (shape='circle', content='åå°ç®¡çå¯ç ï¼é»è®¤ä¸ºadmin')), ],
 mode=DisplayModeEnum.horizontal, horizontal=Horizontal(left=3, right=9,
 offset=5), redirect='/l4d2/admin') body = Wrapper(className='w-2/5 mx-auto my-
 0 m:w-full', body=login_form) login_page = Page(title='', body=[logo, body])
 global_config_form = Form( title='å¨å±éç½®', name='global_config',
-initApi='/l4d2/api/chat_global_config', api='post:/l4d2/api/
-chat_global_config', body=[ Switch(label='æ±çåè½æ»å¼å³',
+initApi='/l4d2/api/l4d2_global_config', api='post:/l4d2/api/
+l4d2_global_config', body=[ Switch(label='æ§å¶æ»å¼å³ï¼æè®¾ï¼',
 name='total_enable', value='${total_enable}', onText='å¼å¯',
 offText='å³é­', labelRemark=Remark(shape='circle',
-content='å³é­åï¼å¨å±é½å°ç¦ç¨æ±çåè½ã')), InputText
-(label='åå°ç®¡çç¨æ·å', name='web_username', value='${web_username}',
-labelRemark=Remark(shape='circle',
+content='å³é­åï¼ç¦ç¨ç½é¡µæ§å¶å°ï¼è¯·åèææ¡£å¯å¨æ¹æ³')),
+InputText(label='åå°ç®¡çç¨æ·å', name='web_username', value='$
+{web_username}', labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çç¨æ·åã')), InputPassword
 (label='åå°ç®¡çå¯ç ', name='web_password', value='${web_password}',
 labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
 (label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
 {web_secret_key}', labelRemark=Remark(shape='circle',
 content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
 (label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
-(shape='circle', content='ç¨äºè·åæå±åè½çkeyã')), InputTag
+(shape='circle',
+content='ç¨äºè·åæå±åè½çkey,å qç¾¤399365126é¢åã')), InputText
+(label='å­ä½', name='l4_font', value='${l4_font}', labelRemark=Remark
+(shape='circle', content='æºå¨äººè¿åå¾çä¸­æå­çå­ä½ã')), Select
+(label='å¾çé£æ ¼', name='l4_style', value='${l4_style}',source='$
+{l4_styles}', labelRemark=Remark(shape='circle',
+content='ä»ä»æ¯æ¹éæ¥è¯¢çé£æ ¼')), InputTag
+(label='æ¥è¯¢çè¿ç¨æå¡å¨tag', name='l4_tag', value='${l4_tag}',
+enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
+joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
+content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), InputTag
 (label='æ±çä¸ä¼ å°å¾ç¨æ·', name='l4_master', value='${l4_master}',
 enableBatchAdd=True, placeholder='æ·»å qqå·', visibleOn='${total_enable}',
 joinValues=False, extractValue=True, labelRemark=Remark(shape='circle',
 content='å¨è¿éå å¥çç¨æ·ï¼æè½ä¸ä¼ å°å¾')), ], actions=[Action
 (label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) upload_map_form =
 Form( title='å¨å±éç½®', name='global_config', api='post:/l4d2/api/
-chat_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
+l4d2_map_config', body=[ InputText(label='æå¡å¨host', name='web_username',
 value='${web_username}', labelRemark=Remark(shape='circle',
 content='127.0.0.1')), InputPassword(label='æå¡å¨', name='web_password',
 value='${web_password}', labelRemark=Remark(shape='circle',
 content='ç»å½æ¬åå°ç®¡çæéè¦çå¯ç ã')), InputText
 (label='åå°ç®¡çtokenå¯é¥', name='web_secret_key', value='$
 {web_secret_key}', labelRemark=Remark(shape='circle',
 content='ç¨äºæ¬åå°ç®¡çå å¯éªè¯tokençå¯é¥ã')), InputText
 (label='æ¥è¯¢key', name='l4_key', value='${l4_key}', labelRemark=Remark
 (shape='circle', content='ç¨äºè·åæå±åè½çkeyã')), ], actions=
 [Action(label='ä¿å­', level=LevelEnum.success, type='submit'), Action
 (label='éç½®', level=LevelEnum.warning, type='reset')] ) group_select =
-Select(label='åç¾¤éç½®', name='group_id', source='${group_list}',
-placeholder='éæ©ç¾¤') group_config_form = Form
+Select(label='åç¾¤éç½®ï¼ææªå®æï¼', name='group_id', source='$
+{group_list}', placeholder='éæ©ç¾¤') group_config_form = Form
 ( title='åç¾¤éç½®ï¼ææªå®æï¼', visibleOn='group_id != null',
-initApi='/l4d2/api/chat_group_config?group_id=${group_id}', api='post:/l4d2/
-api/chat_group_config?group_id=${group_id}', body=[ Switch
+initApi='/l4d2/api/l4d2_group_config?group_id=${group_id}', api='post:/l4d2/
+api/l4d2_group_config?group_id=${group_id}', body=[ Switch
 (label='åç¾¤å¼å³', name='enable', value='${enable}', onText='å¼å¯',
 offText='å³é­', labelRemark=Remark(shape='circle',
 content='éå¯¹è¯¥ç¾¤çç¾¤èå­¦ä¹ å¼å³ï¼å³é­åï¼ä»è¯¥ç¾¤ä¸ä¼å­¦ä¹ ååå¤ã')),
 InputNumber(label='å ä½ç¬¦', name='answer_threshold', value='$
 {answer_threshold}', visibleOn='${enable}', min=2, labelRemark=Remark
 (shape='circle', content='åææ¬')), InputTag(label='å ä½ç¬¦',
 name='ban_words', value='${ban_words}', enableBatchAdd=True,
 placeholder='å ä½ç¬¦ï¼è¯æ¡', visibleOn='${enable}', joinValues=False,
 extractValue=True, labelRemark=Remark(shape='circle',
 content='å ä½ç¬¦è¯æ¡')), ], actions=[Action(label='ä¿å­',
 level=LevelEnum.success, type='submit'), ActionType.Ajax
 ( label='ä¿å­è³ææç¾¤', level=LevelEnum.primary,
 confirmText='ç¡®è®¤å°å½åéç½®ä¿å­è³ææç¾¤ï¼', api='post:/l4d2/api/
-chat_group_config?group_id=all' ), Action(label='éç½®',
-level=LevelEnum.warning, type='reset')] ) message_table = TableCRUD
-( mode='table', title='', syncLocation=False, api='/l4d2/api/
-get_chat_messages', interval=12000, footable=True, columns=[TableColumn
-(label='åºå·', name='message_id'), TableColumn(label='æå¡å¨ip',
-name='group_id', searchable=True), TableColumn(label='æå¡å¨ç«¯å£',
-name='user_id', searchable=True), TableColumn(type='tpl', tpl='$
-{raw_message|truncate:20}', label='rconå¯ç ', name='message',
-searchable=True, popOver={'mode': 'dialog', 'title': 'æ¶æ¯å¨æ',
-'className': 'break-all', 'body': {'type': 'tpl', 'tpl': '${raw_message}'}}),
-TableColumn(type='tpl', tpl='${time|date:YYYY-MM-DD HH\\:mm\\:ss}',
-label='æ¶é´', name='time', sortable=True) ]) context_table = TableCRUD
-(mode='table', title='', syncLocation=False, api='/l4d2/api/get_chat_contexts',
+l4d2_group_config?group_id=all' ), Action(label='éç½®',
+level=LevelEnum.warning, type='reset')] ) server_control = Select
+(label='æå¡å¨è®¾ç½®', name='id_rank', source='${server_list}',
+placeholder='éæ©æå¡å¨') server_ditail= Form( title='', api='post:/l4d2/
+api/l4d2_server_config?id_rank=${id_rank}', initApi='/l4d2/api/
+l4d2_server_config?id_rank=${id_rank}', visibleOn='id_rank != null', body=
+[ Switch(label='æ¯å¦æ¯è¿ç¨æå¡å¨', name='place', value='${place}',
+onText='æ¯ç', offText='ä¸æ¯', labelRemark=Remark(shape='circle',
+content='å¼å¯åç¡®è®¤ä¸ºè¿ç¨æå¡å¨')), InputText
+(label='æå¡å¨åç§°', name='server_id', value='${server_id}',
+labelRemark=Remark(shape='circle', content='æå¡å¨åå­')), InputText
+(label='æå¡å¨ipå°å', name='host', value='${host}', labelRemark=Remark
+(shape='circle', content='æå¡ç«¯æå¨ipå°å,ä¹å¯ä»¥æ¯åå')),
+InputText(label='æå¨ç«¯å£', name='port', value='${port}',
+labelRemark=Remark(shape='circle', content='æå¡ç«¯æå¨ç«¯å£')),
+InputPassword(label='rconæ§å¶å°å¯ç ', name='rcon', value='${rcon}',
+labelRemark=Remark(shape='circle', content='æå¡ç«¯rconå¯ç ')), InputText
+(label='æå¡å¨æ¬å°æä»¶ä½ç½®', name='location', value='${location}',
+labelRemark=Remark(shape='circle',
+content='æ±çæå¡å¨æå¨è·¯å¾,è¯¥è·¯å¾ä¸ææä»¶srcds_run')),
+InputText(label='è¿ç¨è´¦æ·', name='account', value='${account}',
+visibleOn='${place}', labelRemark=Remark(shape='circle',
+content='è¿ç¨æå¡å¨çç»å½è´¦æ·å')), InputPassword
+(label='è¿ç¨å¯ç ', name='password', value='${password}', visibleOn='$
+{place}', labelRemark=Remark(shape='circle',
+content='è¿ç¨æå¡å¨çç»å½å¯ç ')), ], actions=[Action(label='ä¿å­',
+level=LevelEnum.success, type='submit'), Action(label='éç½®',
+level=LevelEnum.warning, type='reset')] ) query_table = TableCRUD(mode='table',
+title='', syncLocation=False, api='/l4d2/api/get_query_contexts',
 interval=60000, footable=True, itemActions=[ActionType.Url
 ( tooltip='å å¥æ¸¸æ', icon='fa fa-gamepad', confirmText = "å å¥steam://
 connect/"+'${ip}', url= "steam://connect/"+'${ip}', # url= "http://"+'${ip}',
-blank= True ), ], columns = [ TableColumn(label='æä¸»', name='tag',
+blank= True ), ], columns = [ TableColumn(label='æä¸»', name='master',
 searchable=True), TableColumn(label='åç§°', name='name', searchable=True),
 TableColumn(label='å°å¾', name='map_', searchable=True), TableColumn
 (label='ç©å®¶', name='rank_players', searchable=True), TableColumn
 (label='å»¶è¿', name='ping', searchable=True), TableColumn(label='IP å°å',
-name='ip', searchable=True), ]) message_page = PageSchema(url='/messages',
-icon='fa fa-comments', label='æ¬å°æå¡å¨ç®¡ç', schema=Page
-(title='æ¬å°æå¡å¨ç®¡ç', body=[ Alert(level=LevelEnum.info,
-className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
+name='ip', searchable=True), ]) server_page = PageSchema(url='/messages',
+icon='fa fa-comment', label='æ¬å°æå¡å¨ç®¡ç', schema=Page
+(title='æ¬å°æå¡å¨ç®¡ç', interval=120000, initApi='/l4d2/api/
+get_l4d2_messages', body=[ Alert(level=LevelEnum.info, className='white-space-
+pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
 {NICKNAME}æå¨æå¡å¨ä¸çæ±çæå¡å¨ã\n' f'Â·
-åè½ææªå®å')), message_table])) context_page = PageSchema(url='/
-contexts', icon='fa fa-comment', label='è¿ç¨æå¡å¨æ¥è¯¢', schema=Page
-(title='è¿ç¨æå¡å¨æ¥è¯¢', body=[Alert(level=LevelEnum.info,
+åè½ææªå®å')), server_control,server_ditail])) query_page = PageSchema
+(url='/contexts', icon='fa fa-comments', label='è¿ç¨æå¡å¨æ¥è¯¢',
+schema=Page(title='è¿ç¨æå¡å¨æ¥è¯¢', body=[Alert(level=LevelEnum.info,
 className='white-space-pre-wrap', body=(f'æ­¤æ°æ®åºè®°å½äº
 {NICKNAME}æè®°å½å¯æ¥è¯¢çæå¡å¨ipã\n' # 'Â·
 ç¹å»"åå¤åè¡¨"å¯ä»¥æ¥çè¯¥æ¡åå®¹å·²å­¦ä¹ å°çå¯è½çåå¤ã\n'
 # 'Â· ç¹å»"ç¦ç¨"å¯ä»¥å°è¯¥å­¦ä¹ è¿è¡ç¦ç¨ï¼ä»¥åä¸ä¼åå­¦ã\n'
-f'Â· åè½ææªå®å')), context_table])) database_page = PageSchema
-(label='æ°æ®åº', icon='fa fa-database', children=[message_page,
-context_page]) config_page = PageSchema(url='/configs', isDefaultPage=True,
-icon='fa fa-wrench', label='éç½®', schema=Page(title='éç½®', initApi='/
-l4d2/api/get_group_list', body=[global_config_form, group_select,
-group_config_form])) chat_page = PageSchema(label='æ±çä¹è·¯', icon='fa fa-
-wechat (alias)', children=[config_page, database_page]) github_logo = Tpl
-(className='w-full', tpl='
+f'Â· åè½ææªå®å')), query_table])) database_page = PageSchema
+(label='æ°æ®åº', icon='fa fa-database', children=[server_page, query_page])
+config_page = PageSchema(url='/configs', isDefaultPage=True, icon='fa fa-
+wrench', label='éç½®', schema=Page(title='éç½®', initApi='/l4d2/api/
+get_group_list', body=[global_config_form,group_select, group_config_form]))
+l4d2_page = PageSchema(label='æ±çä¹è·¯', icon='fa fa-wechat (alias)',
+children=[config_page, database_page]) github_logo = Tpl(className='w-full',
+tpl='
 ') header = Flex(className='w-full', justify='flex-end', alignItems='flex-end',
 items=[github_logo]) admin_app = App(brandName='L4d2-Server', logo='https://
 raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/
 logo.png', header=header, pages=[{ 'children': [config_page, database_page] }],
 footer='
 Copyright Â© 2022 - 2023 AGNES_DIGIAL Xamis_v2.2.0
 ')
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/message.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/seach.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/seach.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/txt_to_img.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/txt_to_img.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from io import BytesIO
 from PIL import Image, ImageDraw, ImageFont
 from nonebot.adapters.onebot.v11 import MessageSegment
 from nonebot_plugin_txt2img import Txt2Img
-from .config import l4_font
+from .config import l4_config
 
+l4_font = l4_config.l4_font
 """直接超的智障回复"""
 def txt_to_img(text: str, font_size=30, font_path=l4_font) -> bytes:
     text = line_break(text)
     d_font = ImageFont.truetype(font_path, font_size)
     lines = text.count('\n')  # 计算行数
     image = Image.new("L", (LINE_CHAR_COUNT*font_size //
                       2 + 50, font_size*lines+50), "white")
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/nonebot_plugin_l4d2_server/utils.py` & `nonebot_plugin_l4d2_server-0.5.0/nonebot_plugin_l4d2_server/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 async def get_file(url: str, down_file: Path):
     '''
     下载指定Url到指定位置
     '''
     try:
-        if l4_only:
+        if l4_config.l4_only:
             maps = await url_to_byte(url)
         else:
             maps = httpx.get(url).content
         logger.info('已获取文件，尝试新建文件并写入')
         with open(down_file, 'wb') as mfile:
             mfile.write(maps)
         logger.info('下载成功')
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/pyproject.toml` & `nonebot_plugin_l4d2_server-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-l4d2-server"
-version = "0.4.9"
+version = "0.5.0"
 description = "L4D2 server related operations plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 repository = "https://github.com/Agnes4m/nonebot_plugin_l4d2_server"
 keywords = ["steam", "game", "l4d2", "nonebot2", "plugin"]
```

### Comparing `nonebot_plugin_l4d2_server-0.4.9/README.md` & `nonebot_plugin_l4d2_server-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_l4d2_server-0.4.9/setup.py` & `nonebot_plugin_l4d2_server-0.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,398 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-l4d2-server
+Version: 0.5.0
+Summary: L4D2 server related operations plugin for NoneBot2
+Home-page: https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+License: GPLv3
+Keywords: steam,game,l4d2,nonebot2,plugin
+Author: Agnes_Digital
+Author-email: Z735803792@163.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: amis-python (>=1.0.6,<2.0.0)
+Requires-Dist: asyncio (>=3.4.3)
+Requires-Dist: beautifulsoup4 (>=4.8.0)
+Requires-Dist: h11 (>=0.14.0,<0.15.0)
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: jieba (>=0.42.1,<0.43.0)
+Requires-Dist: jinja2 (>=3.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.5)
+Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0)
+Requires-Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0)
+Requires-Dist: nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0)
+Requires-Dist: nonebot_plugin_txt2img (>=0.3.0)
+Requires-Dist: pandas (>=1.5.2)
+Requires-Dist: patool (>=1.12,<2.0)
+Requires-Dist: pillow (>=9.3.0,<10.0.0)
+Requires-Dist: python-a2s (>=1.3.0,<2.0.0)
+Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0)
+Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0)
+Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
+Requires-Dist: srctools (>=2.3.9,<3.0.0)
+Project-URL: Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_l4d2_server',
- 'nonebot_plugin_l4d2_server.l4d2_anne',
- 'nonebot_plugin_l4d2_server.l4d2_data',
- 'nonebot_plugin_l4d2_server.l4d2_file',
- 'nonebot_plugin_l4d2_server.l4d2_image',
- 'nonebot_plugin_l4d2_server.l4d2_queries',
- 'nonebot_plugin_l4d2_server.l4d2_server',
- 'nonebot_plugin_l4d2_server.l4d2_web']
-
-package_data = \
-{'': ['*'],
- 'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*',
-                                'data/L4D2/image/header/*',
-                                'data/L4D2/image/template/*']}
-
-install_requires = \
-['aiohttp>=3.8.3,<4.0.0',
- 'amis-python>=1.0.6,<2.0.0',
- 'asyncio>=3.4.3',
- 'beautifulsoup4>=4.8.0',
- 'h11>=0.14.0,<0.15.0',
- 'httpx>=0.23.3,<0.24.0',
- 'jieba>=0.42.1,<0.43.0',
- 'jinja2>=3.0.0',
- 'nonebot-adapter-onebot>=2.1.5',
- 'nonebot2>=2.0.0rc4,<3.0.0',
- 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
- 'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0',
- 'nonebot_plugin_txt2img>=0.3.0',
- 'pandas>=1.5.2',
- 'patool>=1.12,<2.0',
- 'pillow>=9.3.0,<10.0.0',
- 'python-a2s>=1.3.0,<2.0.0',
- 'python-jose>=3.3.0,<4.0.0',
- 'pyunpack>=0.3.0,<0.4.0',
- 'rarfile>=4.0,<5.0',
- 'rcon>=2.1.0,<3.0.0',
- 'ruamel.yaml>=0.17.21,<0.18.0',
- 'srctools>=2.3.9,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-l4d2-server',
-    'version': '0.4.9',
-    'description': 'L4D2 server related operations plugin for NoneBot2',
-    'long_description': '<div align="center">\n  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">\n  <br>\n  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_l4d2_server\n\n_✨Nonebot & Left 4 Dead 2 server操作✨_\n<div align = "center">\n        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;\n        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>\n</div><br>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">\n        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">\n</a>\n<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">\n        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">\n</a>\n<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">\n        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">\n    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">\n</a>\n    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">\n    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">\n\n</div>\n\n## 快速使用（env示例）\n\n    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置\n    # 所有的多选，用逗号隔开\n    l4_master = [\'1145149191\']            # 允许上传地图的qq号\n    l4_file = [\'/home/ubuntu/l4d2/coop\']  # 本地服务器路径\n    l4_host = [\'127.0.0.1\']               # 服务器ip（建议内网，公网也可以）\n    l4_port = [\'20715\']                   # 服务器端口\n    l4_rcon = [\'1145149191810\']           # 服务器rcon密码，如果没有可以列空str对象元素\n    l4_font = \'simsun.ttc\'                # 服务器字体\n    l4_web = True                         # 网页控制台，默认是关闭\n\n## 主要功能\n\n- 求生服务器-本地多路径操作（传地图）\n- 批量查询指定ip服务器状态和玩家\n- 创意工坊下载和喷漆制作\n- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)\n\n## 如何获取key\n\n为了使得ip不被滥用，我采取这种方式管理。\n\n这并不影响正常使用，如果不需要可以忽略\n\n[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”\n如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：\n\n        l4_tag = [\'呆呆\',\'橘\']      # 这里是内置可以查询的服的list对象\n        l4_key = \'qwertyuiopasdfg\'  # 这里是获取的key，是13个字符组成的字符串\n\n## 提交自己的服务器？\n\n__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__\n\n__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__\n\n新增一个json文件，格式如下,文件名与需要响应的指令一致\n\n        {\n        "呆呆": [\n                {\n                "id": 1,\n                "version": "战役",\n                "ip": "43.248.188.17:27031"\n                },\n                {\n                "id": 2,\n                "version": "战役",\n                "ip": "43.248.188.17:27032"\n                }\n        ]\n        }\n\n## 🌐 默认服务器\n\n目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主\n\n| 指令 | 服务器 | op | 数量 |\n|:-----:|:----:|:----:|:----:|\n| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4\n| 云 | anne电信服云服 | 东 | 27\n| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15\n| 橘 | 橘希实香的小窝 | 橘希实香 | 21\n| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21\n| 音理 | 星空列车与白的旅行 | 音理 | 3\n| 尤 | 尤尤 | 晓音 | 3\n| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3\n| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1\n| Air | Air | Air | 15\n| 3ks | 为人民服务 | DK | 14\n\n## 🔖 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.4.9--2022.4\n\n- 修复h11版本错误的bug\n- 重写了config，下个版本正式使用yaml替代env设置\n- 新增远程连接测试代码\n\n### 0.4.8--2022.4.16\n\n- 新增重载ip\n- 修复了一些windows启动下奇奇怪怪的bug\n\n### 0.4.7--2022.4.13\n\n- 新增模式查询\n- 列表推导替换套娃循环\n\n### 0.4.6--2022.4.9\n\n- 显示无效服\n- 优化服务器排序算法（list.sort()天下第一）\n- 默认关闭web端\n\n### 0.4.5--2022.4.9\n\n- 修bug（恼）\n\n### 0.4.2--2022.4.9\n\n- 修复响应开头匹配出现的重大bug\n- 启用web端\n- web使用yaml管理，未来可能删除env配置\n\n### 0.4.1--2022.3\n\n- 修复rar压缩包命名错误\n- 更新了tag的参数读取方式\n- 确定了传文件私聊比群聊快速\n- 修复了电信服计算错误\n\n### 0.4.0--2022.3.27\n\n- 新增web控制台\n- 修复传图超时参数错误\n- 重写求生ip获取方法 ~ 数据库苦手 ~\n- 重写文档\n- 不再内置ip（毕竟ipv4都暴露太危险了）\n\n### 0.3.7--2022.3\n\n- 新增三方下载网盘\n- 修复windows上传临时文件错误\n- 优化查服流程\n- 优化anne服随机功能\n\n### 0.3.6--2022.3.10\n\n- 暂时关闭web端，后续修改\n- 优化图片显示\n- 修复了海量bug\n- 新增三方图查询\n\n### 0.3.5--2022.3.6\n\n- 新增ping查询（在ip里包括）\n- 新增api查询（未完成）\n- 修复了电信服查询绑定名字无法查询的错误\n- 新增了救援率的显示\n- 新增web端（未完成）\n\n### 0.3.4--2022.3.1\n\n- 新增本地插件smx查询\n- 增加了三个内置群服\n- 修改了图片的UI,变好看了\n- 删减了部分图片和字体，使得轻量化\n- 修复了海量bug\n- 修复了python3.8中typing错误\n\n### 0.3.3--2022.2.26\n\n- 重写协议，使用a2s库，同时解决win端不同报错无法输出\n- 重~抄~写服务器查询UI,解决了不好看的问题\n- 从win测试，解决了一些win特有的bug\n- 重写服务器查询~还得是json~\n- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问\n- 新增批量查询服务器，不带参数则返回图片\n\n### 0.3.1--2022.2.22\n\n- 修复了路径识别为str对象的错误\n- 修复了初始化找不到文件的错误\n- 修复了路径拼接错误\n- 在win端成功测试，修复压缩包bug\n- 新增开关协程异步env设置\n- 测试rcon建立通讯\n- 实现切换路径查看地图和使用rcon指令\n\n### 0.3.0--2022.2.18\n\n- 修改了新的env配置，使得支持本地多服务器操作\n- 彻底解决了压缩包解压linux端的问题\n- 解决了win端默认gbk解码的错误\n- 解决rcon指令字体报错\n\n### 0.2.5--2022.2.10\n\n- 修复了依赖不足的bug\n- 更新了电信服战绩个人图片UI\n- 更新了批量服务器查看的UI\n- 修改了传文件为协程异步\n- 优化了部分rcon指令\n- ~tnd7z怎么不去死啊~使用pyunpack库解压7z\n\n### 0.2.4--2022.2.8\n\n- 使用poetry修复了pip安装文件缺失的bug\n\n### 0.2.3--2022.2.7\n\n- 新增坐牢和开牢\n- 修改了获取资源为异步协程却阻碍其他指令的bug\n- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）\n- 喷剂制作开摆了，推测需要c/c++环境\n- 修改抽取文案\n- 新增查询服务器状态时返回connect ip\n- 修复了服务器查询无响应的时候，因为报错无回复信息的bug\n- 个人信息重置测试代码，下个版本更新\n- 新增求生更新添加和删除\n\n### 0.2.2--2022.2.1\n\n- 新增探监\n- 新增喷漆制作\n- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）\n- 修改了部分对话响应\n\n### 0.2.1--2022.1.25\n\n- 新增电信服获取（东哥的肯定）\n- 优化图片UI\n- 新增云服快捷查询\n- 修复了因为没用玩家，导致的服务器状态查询错误\n- 新增电信服ip爬取（仅仅作为单次更新ip列表）\n\n### 0.2.0--2022.1.21\n\n- 新增创意工坊查询\n- 优化查询图片UI\n- 新增创意工坊文件下载\n- 修复了因为电信服官网前端修改导致查询失败的BUG\n\n### 0.1.7--2022.1.19\n\n- 新增群ip订阅，批量查询\n- 新增图片显示ip状态\n- 修复了因为玩家名字特殊字符导致的utf-8解码错误\n- 更新自己的第三方库VSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n- 新增ip查询服务器提供玩家数量和名字\n- 增加协程函数修复因为加载顺序导致的错误\n- 更新自己的第三方库VSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n- 新增服务器控制台指令，新增依赖rcon\n- 重新了数据库，不再使用json而是使用sql3\n- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示\n\n### 0.1.4--2022.1.9\n\n- 新增求生anne详情（看排名）\n- 所有的请求改为httpx\n- 更新了anne信息图片\n- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)\n\n### 0.1.3--2022.1.7\n\n- 新增绑定昵称和steamid\n- 新增可以艾特人查询anne成绩\n- 新增解绑信息\n\n### 0.1.2--2022.1.6\n\n- 新增支持图片输出\n- 新增查询anne服数据\n\n### 0.1.1--2022.1.5\n\n- 新增删除地图\n- 新增地图改名\n- 新增支持图片输出\n\n### 0.1.0--2022.1.4\n\n- 集中修复了Bug\n\n### 0.0.9--2022.1.4\n\n- 新增上传地图后，检测对比回复新地图名字\n- 修复中文名乱码问题\n\n### 0.0.8--2022.1.4\n\n- 支持vpk格式地图\n- 支持查看所有vpk格式文件\n\n### 0.0.6--2022.1.3\n\n- 修复了7z压缩包的方式，优化代码\n\n### 0.0.1--2022.1.3\n\n- 插件初次发布，可私聊添加地图\n\n</details>\n\n## 🙈 其他\n\n- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr\n- 如果本插件对你有帮助，不要忘了点个Star~\n- 本项目仅供学习使用，请勿用于商业用途\n- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)\n\n## 🌐 感谢\n\n- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架\n- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考\n- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)\n- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法\n  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考\n- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考\n- [日向麻麻](https://github.com/Special-Week)- 代码优化参考\n- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考\n- 呆呆- 提供三方地图的详细数据\n',
-    'author': 'Agnes_Digital',
-    'author_email': 'Z735803792@163.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+<div align="center">
+  <img src="https://raw.githubusercontent.com/Agnes4m/nonebot_plugin_l4d2_server/main/image/logo.png" width="180" height="180"  alt="AgnesDigitalLogo">
+  <br>
+  <p><img src="https://s2.loli.net/2022/06/16/xsVUGRrkbn1ljTD.png" width="240" alt="NoneBotPluginText"></p>
+</div>
 
+<div align="center">
+
+# nonebot_plugin_l4d2_server
+
+_✨Nonebot & Left 4 Dead 2 server操作✨_
+<div align = "center">
+        <a href="https://agnes4m.github.io/l4d2/" target="_blank">文档</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/reader/#%E5%8A%9F%E8%83%BD-%E6%8C%87%E4%BB%A4-%F0%9F%A4%94" target="_blank">指令列表</a> &nbsp; · &nbsp;
+        <a href="https://agnes4m.github.io/l4d2/bug/">常见问题</a>
+</div><br>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/stargazers">
+        <img alt="GitHub stars" src="https://img.shields.io/github/stars/Agnes4m/nonebot_plugin_l4d2_server" alt="stars">
+</a>
+<a href="https://github.com/Agnes4m/nonebot_plugin_l4d2_server/issues">
+        <img alt="GitHub issues" src="https://img.shields.io/github/issues/Agnes4m/nonebot_plugin_l4d2_server" alt="issues">
+</a>
+<a href="https://jq.qq.com/?_wv=1027&k=HdjoCcAe">
+        <img src="https://img.shields.io/badge/QQ%E7%BE%A4-399365126-orange?style=flat-square" alt="QQ Chat Group">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+        <img src="https://img.shields.io/pypi/v/nonebot_plugin_l4d2_server.svg" alt="pypi">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_l4d2_server">
+    <img src="https://img.shields.io/pypi/dm/nonebot_plugin_l4d2_server" alt="pypi download">
+</a>
+    <img src="https://img.shields.io/badge/python-3.9+-blue.svg" alt="python">
+    <img src="https://img.shields.io/badge/nonebot-2.0.0rc3-red.svg" alt="NoneBot">
+
+</div>
+
+## 快速使用（env示例）
+
+    # 复制到env文件里，没有默认就是下列值，如需修改安装下面env设置
+    # 所有的多选，用逗号隔开
+    l4_master = ['1145149191']            # 允许上传地图的qq号
+    l4_file = ['/home/ubuntu/l4d2/coop']  # 本地服务器路径
+    l4_host = ['127.0.0.1']               # 服务器ip（建议内网，公网也可以）
+    l4_port = ['20715']                   # 服务器端口
+    l4_rcon = ['1145149191810']           # 服务器rcon密码，如果没有可以列空str对象元素
+    l4_font = 'simsun.ttc'                # 服务器字体
+    l4_web = True                         # 网页控制台，默认是关闭
+
+## 主要功能
+
+- 求生服务器-本地多路径操作（传地图）
+- 批量查询指定ip服务器状态和玩家
+- 创意工坊下载和喷漆制作
+- [求生电信服anne](https://github.com/fantasylidong/CompetitiveWithAnne)[查询~](https://sb.trygek.com/l4d_stats/ranking/index.php)
+
+## 如何获取key
+
+为了使得ip不被滥用，我采取这种方式管理。
+
+这并不影响正常使用，如果不需要可以忽略
+
+[点击这里加群](https://jq.qq.com/?_wv=1027&k=HdjoCcAe)并在群内发送“申请求生key”
+如果你只查询自己的服务器ip则可以忽略如下，并且更改env设置：
+
+        l4_tag = ['呆呆','橘']      # 这里是内置可以查询的服的list对象
+        l4_key = 'qwertyuiopasdfg'  # 这里是获取的key，是13个字符组成的字符串
+
+## 提交自己的服务器？
+
+__本项目原旨在方便自己查询管理服务器，如果你希望提供了ip__
+
+__那么我只能尽可能保证您的ip不会泄漏，如果无法承担风险则请勿提供ip__
+
+新增一个json文件，格式如下,文件名与需要响应的指令一致
+
+        {
+        "呆呆": [
+                {
+                "id": 1,
+                "version": "战役",
+                "ip": "43.248.188.17:27031"
+                },
+                {
+                "id": 2,
+                "version": "战役",
+                "ip": "43.248.188.17:27032"
+                }
+        ]
+        }
+
+## 🌐 默认服务器
+
+目前 __已授权__ 的服务器查询，如果需要加入自己的ip可以进qq群私聊群主
+
+| 指令 | 服务器 | op | 数量 |
+|:-----:|:----:|:----:|:----:|
+| 数码 | 爱丽数码想要涩涩 | 爱丽数码 | 4
+| 云 | anne电信服云服 | 东 | 27
+| 呆呆 | 呆呆的小窝 | 提莫大魔王 | 15
+| 橘 | 橘希实香的小窝 | 橘希实香 | 21
+| 竹 | 竹烨 | 竹烨oО柠檬茶 | 21
+| 音理 | 星空列车与白的旅行 | 音理 | 3
+| 尤 | 尤尤 | 晓音 | 3
+| 鱼 | 飞鱼の小窝 | 飞鱼桑 | 3
+| 恋恋 | 恋氏集团雪糕制作研究中心 | 古明地恋 | 1
+| Air | Air | Air | 15
+| 3ks | 为人民服务 | DK | 14
+
+## 🔖 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
+### 0.4.9--2022.4
+
+- 修复h11版本错误的bug
+- 重写了config，下个版本正式使用yaml替代env设置
+- 新增远程连接测试代码
+
+### 0.4.8--2022.4.16
+
+- 新增重载ip
+- 修复了一些windows启动下奇奇怪怪的bug
+
+### 0.4.7--2022.4.13
+
+- 新增模式查询
+- 列表推导替换套娃循环
+
+### 0.4.6--2022.4.9
+
+- 显示无效服
+- 优化服务器排序算法（list.sort()天下第一）
+- 默认关闭web端
+
+### 0.4.5--2022.4.9
+
+- 修bug（恼）
+
+### 0.4.2--2022.4.9
+
+- 修复响应开头匹配出现的重大bug
+- 启用web端
+- web使用yaml管理，未来可能删除env配置
+
+### 0.4.1--2022.3
+
+- 修复rar压缩包命名错误
+- 更新了tag的参数读取方式
+- 确定了传文件私聊比群聊快速
+- 修复了电信服计算错误
+
+### 0.4.0--2022.3.27
+
+- 新增web控制台
+- 修复传图超时参数错误
+- 重写求生ip获取方法 ~ 数据库苦手 ~
+- 重写文档
+- 不再内置ip（毕竟ipv4都暴露太危险了）
+
+### 0.3.7--2022.3
+
+- 新增三方下载网盘
+- 修复windows上传临时文件错误
+- 优化查服流程
+- 优化anne服随机功能
+
+### 0.3.6--2022.3.10
+
+- 暂时关闭web端，后续修改
+- 优化图片显示
+- 修复了海量bug
+- 新增三方图查询
+
+### 0.3.5--2022.3.6
+
+- 新增ping查询（在ip里包括）
+- 新增api查询（未完成）
+- 修复了电信服查询绑定名字无法查询的错误
+- 新增了救援率的显示
+- 新增web端（未完成）
+
+### 0.3.4--2022.3.1
+
+- 新增本地插件smx查询
+- 增加了三个内置群服
+- 修改了图片的UI,变好看了
+- 删减了部分图片和字体，使得轻量化
+- 修复了海量bug
+- 修复了python3.8中typing错误
+
+### 0.3.3--2022.2.26
+
+- 重写协议，使用a2s库，同时解决win端不同报错无法输出
+- 重~抄~写服务器查询UI,解决了不好看的问题
+- 从win测试，解决了一些win特有的bug
+- 重写服务器查询~还得是json~
+- 内置服务器查询系统，可以通过[服务器简称]+[number]/[模式]来访问
+- 新增批量查询服务器，不带参数则返回图片
+
+### 0.3.1--2022.2.22
+
+- 修复了路径识别为str对象的错误
+- 修复了初始化找不到文件的错误
+- 修复了路径拼接错误
+- 在win端成功测试，修复压缩包bug
+- 新增开关协程异步env设置
+- 测试rcon建立通讯
+- 实现切换路径查看地图和使用rcon指令
+
+### 0.3.0--2022.2.18
+
+- 修改了新的env配置，使得支持本地多服务器操作
+- 彻底解决了压缩包解压linux端的问题
+- 解决了win端默认gbk解码的错误
+- 解决rcon指令字体报错
+
+### 0.2.5--2022.2.10
+
+- 修复了依赖不足的bug
+- 更新了电信服战绩个人图片UI
+- 更新了批量服务器查看的UI
+- 修改了传文件为协程异步
+- 优化了部分rcon指令
+- ~tnd7z怎么不去死啊~使用pyunpack库解压7z
+
+### 0.2.4--2022.2.8
+
+- 使用poetry修复了pip安装文件缺失的bug
+
+### 0.2.3--2022.2.7
+
+- 新增坐牢和开牢
+- 修改了获取资源为异步协程却阻碍其他指令的bug
+- 新增json统计部分已知服务器（未来应该独立成库持续更新，如果把您的非公开服记录请联系我删除）
+- 喷剂制作开摆了，推测需要c/c++环境
+- 修改抽取文案
+- 新增查询服务器状态时返回connect ip
+- 修复了服务器查询无响应的时候，因为报错无回复信息的bug
+- 个人信息重置测试代码，下个版本更新
+- 新增求生更新添加和删除
+
+### 0.2.2--2022.2.1
+
+- 新增探监
+- 新增喷漆制作
+- 修复了魔改服务器导致解包错误的bug（就是直接忽略了）
+- 修改了部分对话响应
+
+### 0.2.1--2022.1.25
+
+- 新增电信服获取（东哥的肯定）
+- 优化图片UI
+- 新增云服快捷查询
+- 修复了因为没用玩家，导致的服务器状态查询错误
+- 新增电信服ip爬取（仅仅作为单次更新ip列表）
+
+### 0.2.0--2022.1.21
+
+- 新增创意工坊查询
+- 优化查询图片UI
+- 新增创意工坊文件下载
+- 修复了因为电信服官网前端修改导致查询失败的BUG
+
+### 0.1.7--2022.1.19
+
+- 新增群ip订阅，批量查询
+- 新增图片显示ip状态
+- 修复了因为玩家名字特殊字符导致的utf-8解码错误
+- 更新自己的第三方库VSQ==0.0.6
+
+### 0.1.6--2022.1.15
+
+- 新增ip查询服务器提供玩家数量和名字
+- 增加协程函数修复因为加载顺序导致的错误
+- 更新自己的第三方库VSQ==0.0.4
+
+### 0.1.5--2022.1.15
+
+- 新增服务器控制台指令，新增依赖rcon
+- 重新了数据库，不再使用json而是使用sql3
+- 改写了求生anne信息显示方式：如果单个数据以图片显示，如果多个数据以文字显示
+
+### 0.1.4--2022.1.9
+
+- 新增求生anne详情（看排名）
+- 所有的请求改为httpx
+- 更新了anne信息图片
+- 可选使用模拟谷歌浏览器来获取anne更多数据（~有点屎了，希望大佬救救~)
+
+### 0.1.3--2022.1.7
+
+- 新增绑定昵称和steamid
+- 新增可以艾特人查询anne成绩
+- 新增解绑信息
+
+### 0.1.2--2022.1.6
+
+- 新增支持图片输出
+- 新增查询anne服数据
+
+### 0.1.1--2022.1.5
+
+- 新增删除地图
+- 新增地图改名
+- 新增支持图片输出
+
+### 0.1.0--2022.1.4
+
+- 集中修复了Bug
+
+### 0.0.9--2022.1.4
+
+- 新增上传地图后，检测对比回复新地图名字
+- 修复中文名乱码问题
+
+### 0.0.8--2022.1.4
+
+- 支持vpk格式地图
+- 支持查看所有vpk格式文件
+
+### 0.0.6--2022.1.3
+
+- 修复了7z压缩包的方式，优化代码
+
+### 0.0.1--2022.1.3
+
+- 插件初次发布，可私聊添加地图
+
+</details>
+
+## 🙈 其他
+
+- 本人技术很差，如果您有发现BUG或者更好的建议，欢迎提Issue & Pr
+- 如果本插件对你有帮助，不要忘了点个Star~
+- 本项目仅供学习使用，请勿用于商业用途
+- [GPL-3.0 License](https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) ©[@Agnes4m](https://github.com/Agnes4m)
+
+## 🌐 感谢
+
+- [nonebot2](https://github.com/nonebot/nonebot2)- 聊天机器人的基础框架
+- [修仙](https://github.com/s52047qwas/nonebot_plugin_xiuxian)- 数据库参考
+- ~~[自己写的求生之路查询库](https://github.com/Agnes4m/VSQ)~~ (已弃用)
+- [@MeetWq](https://github.com/MeetWq)- 非常热心解答nonebot2相关的写法
+  - [可爱小Q](https://github.com/MeetWq/mybot)- 服务器图片参考
+- [群聊学习](https://github.com/CMHopeSunshine/nonebot-plugin-learning-chat)- web控制台参考
+- [日向麻麻](https://github.com/Special-Week)- 代码优化参考
+- [gsuid](https://github.com/KimigaiiWuyi/GenshinUID)- readme和wiki的格式参考
+- 呆呆- 提供三方地图的详细数据
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,175 +1,172 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_l4d2_server', 'nonebot_plugin_l4d2_server.l4d2_anne',
-'nonebot_plugin_l4d2_server.l4d2_data', 'nonebot_plugin_l4d2_server.l4d2_file',
-'nonebot_plugin_l4d2_server.l4d2_image',
-'nonebot_plugin_l4d2_server.l4d2_queries',
-'nonebot_plugin_l4d2_server.l4d2_server',
-'nonebot_plugin_l4d2_server.l4d2_web'] package_data = \ {'': ['*'],
-'nonebot_plugin_l4d2_server': ['data/L4D2/image/head/*', 'data/L4D2/image/
-header/*', 'data/L4D2/image/template/*']} install_requires = \
-['aiohttp>=3.8.3,<4.0.0', 'amis-python>=1.0.6,<2.0.0', 'asyncio>=3.4.3',
-'beautifulsoup4>=4.8.0', 'h11>=0.14.0,<0.15.0', 'httpx>=0.23.3,<0.24.0',
-'jieba>=0.42.1,<0.43.0', 'jinja2>=3.0.0', 'nonebot-adapter-onebot>=2.1.5',
-'nonebot2>=2.0.0rc4,<3.0.0', 'nonebot_plugin_apscheduler>=0.2.0,<0.3.0',
-'nonebot_plugin_htmlrender>=0.2.0.1,<0.3.0.0', 'nonebot_plugin_txt2img>=0.3.0',
-'pandas>=1.5.2', 'patool>=1.12,<2.0', 'pillow>=9.3.0,<10.0.0', 'python-
-a2s>=1.3.0,<2.0.0', 'python-jose>=3.3.0,<4.0.0', 'pyunpack>=0.3.0,<0.4.0',
-'rarfile>=4.0,<5.0', 'rcon>=2.1.0,<3.0.0', 'ruamel.yaml>=0.17.21,<0.18.0',
-'srctools>=2.3.9,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-l4d2-
-server', 'version': '0.4.9', 'description': 'L4D2 server related operations
-plugin for NoneBot2', 'long_description': '
-                           \n [AgnesDigitalLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-l4d2-server Version: 0.5.0 Summary:
+L4D2 server related operations plugin for NoneBot2 Home-page: https://
+github.com/Agnes4m/nonebot_plugin_l4d2_server License: GPLv3 Keywords:
+steam,game,l4d2,nonebot2,plugin Author: Agnes_Digital Author-email:
+Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
+Approved :: GNU General Public License v3 (GPLv3) Classifier: License :: Other/
+Proprietary License Classifier: Operating System :: OS Independent Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Requires-Dist: aiohttp
+(>=3.8.3,<4.0.0) Requires-Dist: amis-python (>=1.0.6,<2.0.0) Requires-Dist:
+asyncio (>=3.4.3) Requires-Dist: beautifulsoup4 (>=4.8.0) Requires-Dist: h11
+(>=0.14.0,<0.15.0) Requires-Dist: httpx (>=0.23.3,<0.24.0) Requires-Dist: jieba
+(>=0.42.1,<0.43.0) Requires-Dist: jinja2 (>=3.0.0) Requires-Dist: nonebot-
+adapter-onebot (>=2.1.5) Requires-Dist: nonebot2 (>=2.0.0rc4,<3.0.0) Requires-
+Dist: nonebot_plugin_apscheduler (>=0.2.0,<0.3.0) Requires-Dist:
+nonebot_plugin_htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist:
+nonebot_plugin_txt2img (>=0.3.0) Requires-Dist: pandas (>=1.5.2) Requires-Dist:
+patool (>=1.12,<2.0) Requires-Dist: pillow (>=9.3.0,<10.0.0) Requires-Dist:
+python-a2s (>=1.3.0,<2.0.0) Requires-Dist: python-jose (>=3.3.0,<4.0.0)
+Requires-Dist: pyunpack (>=0.3.0,<0.4.0) Requires-Dist: rarfile (>=4.0,<5.0)
+Requires-Dist: rcon (>=2.1.0,<3.0.0) Requires-Dist: ruamel.yaml
+(>=0.17.21,<0.18.0) Requires-Dist: srctools (>=2.3.9,<3.0.0) Project-URL:
+Repository, https://github.com/Agnes4m/nonebot_plugin_l4d2_server Description-
+Content-Type: text/markdown
+                              [AgnesDigitalLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-        \n\n# nonebot_plugin_l4d2_server\n\n_â¨Nonebot & Left 4 Dead 2
-                              serveræä½â¨_\n
-            \n ææ¡£   Â·  \n æä»¤åè¡¨   Â·  \n å¸¸è§é®é¢\n
+   # nonebot_plugin_l4d2_server _â¨Nonebot & Left 4 Dead 2 serveræä½â¨_
+                ææ¡£   Â·   æä»¤åè¡¨   Â·   å¸¸è§é®é¢
 
-    \n\n_[GitHub_stars]\n\n\n_[GitHub_issues]\n\n\n_[QQ_Chat_Group]\n\n\n_
-           [pypi]\n\n\n_[pypi_download]\n\n [python]\n [NoneBot]\n\n
-\n\n## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼\n\n #
-å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®\n
-# ææçå¤éï¼ç¨éå·éå¼\n l4_master = [\'1145149191\'] #
-åè®¸ä¸ä¼ å°å¾çqqå·\n l4_file = [\'/home/ubuntu/l4d2/coop\'] #
-æ¬å°æå¡å¨è·¯å¾\n l4_host = [\'127.0.0.1\'] #
-æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼\n l4_port = [\'20715\'] #
-æå¡å¨ç«¯å£\n l4_rcon = [\'1145149191810\'] #
-æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´ \n l4_font =
-\'simsun.ttc\' # æå¡å¨å­ä½\n l4_web = True #
-ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­\n\n## ä¸»è¦åè½\n\n- æ±çæå¡å¨-
-æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼\n-
-æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶\n-
-åæå·¥åä¸è½½åå·æ¼å¶ä½\n- [æ±ççµä¿¡æanne](https://github.com/
+[GitHub_stars] [GitHub_issues] [QQ_Chat_Group] [pypi] [pypi_download] [python]
+                                   [NoneBot]
+## å¿«éä½¿ç¨ï¼envç¤ºä¾ï¼ #
+å¤å¶å°envæä»¶éï¼æ²¡æé»è®¤å°±æ¯ä¸åå¼ï¼å¦éä¿®æ¹å®è£ä¸é¢envè®¾ç½®
+# ææçå¤éï¼ç¨éå·éå¼ l4_master = ['1145149191'] #
+åè®¸ä¸ä¼ å°å¾çqqå· l4_file = ['/home/ubuntu/l4d2/coop'] #
+æ¬å°æå¡å¨è·¯å¾ l4_host = ['127.0.0.1'] #
+æå¡å¨ipï¼å»ºè®®åç½ï¼å¬ç½ä¹å¯ä»¥ï¼ l4_port = ['20715'] #
+æå¡å¨ç«¯å£ l4_rcon = ['1145149191810'] #
+æå¡å¨rconå¯ç ï¼å¦ææ²¡æå¯ä»¥åç©ºstrå¯¹è±¡åç´  l4_font =
+'simsun.ttc' # æå¡å¨å­ä½ l4_web = True #
+ç½é¡µæ§å¶å°ï¼é»è®¤æ¯å³é­ ## ä¸»è¦åè½ - æ±çæå¡å¨-
+æ¬å°å¤è·¯å¾æä½ï¼ä¼ å°å¾ï¼ -
+æ¹éæ¥è¯¢æå®ipæå¡å¨ç¶æåç©å®¶ -
+åæå·¥åä¸è½½åå·æ¼å¶ä½ - [æ±ççµä¿¡æanne](https://github.com/
 fantasylidong/CompetitiveWithAnne)[æ¥è¯¢~](https://sb.trygek.com/l4d_stats/
-ranking/index.php)\n\n##
-å¦ä½è·åkey\n\nä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã\n\nè¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥\n\n
-[ç¹å»è¿éå ç¾¤](https://jq.qq.com/
-?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ\nå¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼\n\n
-l4_tag = [\'åå\',\'æ©\'] #
-è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡\n l4_key = \'qwertyuiopasdfg\' #
-è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸²\n\n##
-æäº¤èªå·±çæå¡å¨ï¼\n\n__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__\n\n__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__\n\næ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´\n\n
-{\n "åå": [\n {\n "id": 1,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27031"\n },\n {\n "id": 2,\n "version": "æå½¹",\n "ip": "43.248.188.17:
-27032"\n }\n ]\n }\n\n## ð é»è®¤æå¡å¨\n\nç®å __å·²ææ__
-çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸»\n\n|
-æä»¤ | æå¡å¨ | op | æ°é |\n|:-----:|:----:|:----:|:----:|\n| æ°ç  |
-ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4\n| äº | anneçµä¿¡æäºæ | ä¸
-| 27\n| åå | ååçå°çª | æè«å¤§é­ç | 15\n| æ© |
-æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21\n| ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶
-| 21\n| é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3\n| å°¤ | å°¤å°¤ |
-æé³ | 3\n| é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3\n| ææ |
-ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1\n| Air | Air | Air |
-15\n| 3ks | ä¸ºäººæ°æå¡ | DK | 14\n\n## ð æ´æ°æ¥å¿\n\n\nå±å¼/
-æ¶èµ·\n\n### 0.4.9--2022.4\n\n- ä¿®å¤h11çæ¬éè¯¯çbug\n-
-éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½®\n-
-æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç \n\n### 0.4.8--2022.4.16\n\n- æ°å¢éè½½ip\n-
-ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug\n\n### 0.4.7--2022.4.13\n\n-
-æ°å¢æ¨¡å¼æ¥è¯¢\n- åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯\n\n### 0.4.6--
-2022.4.9\n\n- æ¾ç¤ºæ ææ\n- ä¼åæå¡å¨æåºç®æ³ï¼list.sort
-()å¤©ä¸ç¬¬ä¸ï¼\n- é»è®¤å³é­webç«¯\n\n### 0.4.5--2022.4.9\n\n-
-ä¿®bugï¼æ¼ï¼\n\n### 0.4.2--2022.4.9\n\n-
-ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug\n- å¯ç¨webç«¯\n-
-webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½®\n\n### 0.4.1--2022.3\n\n-
-ä¿®å¤raråç¼©åå½åéè¯¯\n- æ´æ°äºtagçåæ°è¯»åæ¹å¼\n-
-ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é\n-
-ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯\n\n### 0.4.0--2022.3.27\n\n-
-æ°å¢webæ§å¶å°\n- ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯\n-
-éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~\n- éåææ¡£\n-
-ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼\n\n### 0.3.7--2022.3\n\n-
-æ°å¢ä¸æ¹ä¸è½½ç½ç\n- ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯\n-
-ä¼åæ¥ææµç¨\n- ä¼åanneæéæºåè½\n\n### 0.3.6--2022.3.10\n\n-
-ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹\n- ä¼åå¾çæ¾ç¤º\n-
-ä¿®å¤äºæµ·ébug\n- æ°å¢ä¸æ¹å¾æ¥è¯¢\n\n### 0.3.5--2022.3.6\n\n-
-æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼\n- æ°å¢apiæ¥è¯¢ï¼æªå®æï¼\n-
-ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯\n-
-æ°å¢äºææ´ççæ¾ç¤º\n- æ°å¢webç«¯ï¼æªå®æï¼\n\n### 0.3.4--
-2022.3.1\n\n- æ°å¢æ¬å°æä»¶smxæ¥è¯¢\n- å¢å äºä¸ä¸ªåç½®ç¾¤æ\n-
-ä¿®æ¹äºå¾ççUI,åå¥½çäº\n-
-å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå\n- ä¿®å¤äºæµ·ébug\n-
-ä¿®å¤äºpython3.8ä¸­typingéè¯¯\n\n### 0.3.3--2022.2.26\n\n-
-éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº\n-
-é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢\n-
-ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug\n-
-éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~\n-
+ranking/index.php) ## å¦ä½è·åkey
+ä¸ºäºä½¿å¾ipä¸è¢«æ»¥ç¨ï¼æéåè¿ç§æ¹å¼ç®¡çã
+è¿å¹¶ä¸å½±åæ­£å¸¸ä½¿ç¨ï¼å¦æä¸éè¦å¯ä»¥å¿½ç¥ [ç¹å»è¿éå ç¾¤]
+(https://jq.qq.com/?_wv=1027&k=HdjoCcAe)å¹¶å¨ç¾¤ååéâç³è¯·æ±çkeyâ
+å¦æä½ åªæ¥è¯¢èªå·±çæå¡å¨ipåå¯ä»¥å¿½ç¥å¦ä¸ï¼å¹¶ä¸æ´æ¹envè®¾ç½®ï¼
+l4_tag = ['åå','æ©'] # è¿éæ¯åç½®å¯ä»¥æ¥è¯¢çæçlistå¯¹è±¡
+l4_key = 'qwertyuiopasdfg' #
+è¿éæ¯è·åçkeyï¼æ¯13ä¸ªå­ç¬¦ç»æçå­ç¬¦ä¸² ##
+æäº¤èªå·±çæå¡å¨ï¼
+__æ¬é¡¹ç®åæ¨å¨æ¹ä¾¿èªå·±æ¥è¯¢ç®¡çæå¡å¨ï¼å¦æä½ å¸ææä¾äºip__
+__é£ä¹æåªè½å°½å¯è½ä¿è¯æ¨çipä¸ä¼æ³æ¼ï¼å¦ææ æ³æ¿æé£é©åè¯·å¿æä¾ip__
+æ°å¢ä¸ä¸ªjsonæä»¶ï¼æ ¼å¼å¦ä¸,æä»¶åä¸éè¦ååºçæä»¤ä¸è´
+{ "åå": [ { "id": 1, "version": "æå½¹", "ip": "43.248.188.17:27031" },
+{ "id": 2, "version": "æå½¹", "ip": "43.248.188.17:27032" } ] } ## ð
+é»è®¤æå¡å¨ ç®å __å·²ææ__
+çæå¡å¨æ¥è¯¢ï¼å¦æéè¦å å¥èªå·±çipå¯ä»¥è¿qqç¾¤ç§èç¾¤ä¸» |
+æä»¤ | æå¡å¨ | op | æ°é | |:-----:|:----:|:----:|:----:| | æ°ç  |
+ç±ä¸½æ°ç æ³è¦æ¶©æ¶© | ç±ä¸½æ°ç  | 4 | äº | anneçµä¿¡æäºæ | ä¸ |
+27 | åå | ååçå°çª | æè«å¤§é­ç | 15 | æ© |
+æ©å¸å®é¦çå°çª | æ©å¸å®é¦ | 21 | ç«¹ | ç«¹ç¨ | ç«¹ç¨oÐæ æª¬è¶ |
+21 | é³ç | æç©ºåè½¦ä¸ç½çæè¡ | é³ç | 3 | å°¤ | å°¤å°¤ | æé³
+| 3 | é±¼ | é£é±¼ã®å°çª | é£é±¼æ¡ | 3 | ææ |
+ææ°éå¢éªç³å¶ä½ç ç©¶ä¸­å¿ | å¤æå°æ | 1 | Air | Air | Air | 15
+| 3ks | ä¸ºäººæ°æå¡ | DK | 14 ## ð æ´æ°æ¥å¿  å±å¼/æ¶èµ· ###
+0.4.9--2022.4 - ä¿®å¤h11çæ¬éè¯¯çbug -
+éåäºconfigï¼ä¸ä¸ªçæ¬æ­£å¼ä½¿ç¨yamlæ¿ä»£envè®¾ç½® -
+æ°å¢è¿ç¨è¿æ¥æµè¯ä»£ç  ### 0.4.8--2022.4.16 - æ°å¢éè½½ip -
+ä¿®å¤äºä¸äºwindowså¯å¨ä¸å¥å¥æªæªçbug ### 0.4.7--2022.4.13 -
+æ°å¢æ¨¡å¼æ¥è¯¢ - åè¡¨æ¨å¯¼æ¿æ¢å¥å¨å¾ªç¯ ### 0.4.6--2022.4.9 -
+æ¾ç¤ºæ ææ - ä¼åæå¡å¨æåºç®æ³ï¼list.sort()å¤©ä¸ç¬¬ä¸ï¼ -
+é»è®¤å³é­webç«¯ ### 0.4.5--2022.4.9 - ä¿®bugï¼æ¼ï¼ ### 0.4.2--2022.4.9 -
+ä¿®å¤ååºå¼å¤´å¹éåºç°çéå¤§bug - å¯ç¨webç«¯ -
+webä½¿ç¨yamlç®¡çï¼æªæ¥å¯è½å é¤envéç½® ### 0.4.1--2022.3 -
+ä¿®å¤raråç¼©åå½åéè¯¯ - æ´æ°äºtagçåæ°è¯»åæ¹å¼ -
+ç¡®å®äºä¼ æä»¶ç§èæ¯ç¾¤èå¿«é - ä¿®å¤äºçµä¿¡æè®¡ç®éè¯¯ ###
+0.4.0--2022.3.27 - æ°å¢webæ§å¶å° - ä¿®å¤ä¼ å¾è¶æ¶åæ°éè¯¯ -
+éåæ±çipè·åæ¹æ³ ~ æ°æ®åºè¦æ ~ - éåææ¡£ -
+ä¸ååç½®ipï¼æ¯ç«ipv4é½æ´é²å¤ªå±é©äºï¼ ### 0.3.7--2022.3 -
+æ°å¢ä¸æ¹ä¸è½½ç½ç - ä¿®å¤windowsä¸ä¼ ä¸´æ¶æä»¶éè¯¯ -
+ä¼åæ¥ææµç¨ - ä¼åanneæéæºåè½ ### 0.3.6--2022.3.10 -
+ææ¶å³é­webç«¯ï¼åç»­ä¿®æ¹ - ä¼åå¾çæ¾ç¤º - ä¿®å¤äºæµ·ébug -
+æ°å¢ä¸æ¹å¾æ¥è¯¢ ### 0.3.5--2022.3.6 -
+æ°å¢pingæ¥è¯¢ï¼å¨ipéåæ¬ï¼ - æ°å¢apiæ¥è¯¢ï¼æªå®æï¼ -
+ä¿®å¤äºçµä¿¡ææ¥è¯¢ç»å®åå­æ æ³æ¥è¯¢çéè¯¯ -
+æ°å¢äºææ´ççæ¾ç¤º - æ°å¢webç«¯ï¼æªå®æï¼ ### 0.3.4--2022.3.1 -
+æ°å¢æ¬å°æä»¶smxæ¥è¯¢ - å¢å äºä¸ä¸ªåç½®ç¾¤æ -
+ä¿®æ¹äºå¾ççUI,åå¥½çäº -
+å åäºé¨åå¾çåå­ä½ï¼ä½¿å¾è½»éå - ä¿®å¤äºæµ·ébug -
+ä¿®å¤äºpython3.8ä¸­typingéè¯¯ ### 0.3.3--2022.2.26 -
+éååè®®ï¼ä½¿ç¨a2såºï¼åæ¶è§£å³winç«¯ä¸åæ¥éæ æ³è¾åº -
+é~æ~åæå¡å¨æ¥è¯¢UI,è§£å³äºä¸å¥½ççé®é¢ -
+ä»winæµè¯ï¼è§£å³äºä¸äºwinç¹æçbug -
+éåæå¡å¨æ¥è¯¢~è¿å¾æ¯json~ -
 åç½®æå¡å¨æ¥è¯¢ç³»ç»ï¼å¯ä»¥éè¿[æå¡å¨ç®ç§°]+[number]/
-[æ¨¡å¼]æ¥è®¿é®\n-
-æ°å¢æ¹éæ¥è¯¢æå¡å¨ï¼ä¸å¸¦åæ°åè¿åå¾ç\n\n### 0.3.1--
-2022.2.22\n\n- ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯\n-
-ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯\n- ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯\n-
-å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug\n-
-æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®\n- æµè¯rconå»ºç«éè®¯\n-
-å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤\n\n### 0.3.0--2022.2.18\n\n-
-ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½\n-
-å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢\n-
-è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯\n- è§£å³rconæä»¤å­ä½æ¥é\n\n###
-0.2.5--2022.2.10\n\n- ä¿®å¤äºä¾èµä¸è¶³çbug\n-
-æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI\n-
-æ´æ°äºæ¹éæå¡å¨æ¥ççUI\n- ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥\n-
-ä¼åäºé¨årconæä»¤\n-
-~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z\n\n### 0.2.4--2022.2.8\n\n-
-ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug\n\n### 0.2.3--2022.2.7\n\n-
-æ°å¢åç¢åå¼ç¢\n-
-ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug\n-
-æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼\n-
-å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢\n- ä¿®æ¹æ½åææ¡\n-
-æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip\n-
-ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug\n-
-ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ°\n-
-æ°å¢æ±çæ´æ°æ·»å åå é¤\n\n### 0.2.2--2022.2.1\n\n- æ°å¢æ¢ç\n-
-æ°å¢å·æ¼å¶ä½\n-
-ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼\n-
-ä¿®æ¹äºé¨åå¯¹è¯ååº\n\n### 0.2.1--2022.1.25\n\n-
-æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼\n- ä¼åå¾çUI\n-
-æ°å¢äºæå¿«æ·æ¥è¯¢\n-
-ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯\n-
-æ°å¢çµä¿¡æipç¬åï¼ä»ä»ä½ä¸ºåæ¬¡æ´æ°ipåè¡¨ï¼\n\n### 0.2.0--
-2022.1.21\n\n- æ°å¢åæå·¥åæ¥è¯¢\n- ä¼åæ¥è¯¢å¾çUI\n-
-æ°å¢åæå·¥åæä»¶ä¸è½½\n-
-ä¿®å¤äºå ä¸ºçµä¿¡æå®ç½åç«¯ä¿®æ¹å¯¼è´æ¥è¯¢å¤±è´¥çBUG\n\n###
-0.1.7--2022.1.19\n\n- æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢\n-
-æ°å¢å¾çæ¾ç¤ºipç¶æ\n-
-ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯\n-
-æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6\n\n### 0.1.6--2022.1.15\n\n-
-æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­\n-
-å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯\n-
-æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.4\n\n### 0.1.5--2022.1.15\n\n-
-æ°å¢æå¡å¨æ§å¶å°æä»¤ï¼æ°å¢ä¾èµrcon\n-
-éæ°äºæ°æ®åºï¼ä¸åä½¿ç¨jsonèæ¯ä½¿ç¨sql3\n-
-æ¹åäºæ±çanneä¿¡æ¯æ¾ç¤ºæ¹å¼ï¼å¦æåä¸ªæ°æ®ä»¥å¾çæ¾ç¤ºï¼å¦æå¤ä¸ªæ°æ®ä»¥æå­æ¾ç¤º\n\n###
-0.1.4--2022.1.9\n\n- æ°å¢æ±çanneè¯¦æï¼çæåï¼\n-
-ææçè¯·æ±æ¹ä¸ºhttpx\n- æ´æ°äºanneä¿¡æ¯å¾ç\n-
-å¯éä½¿ç¨æ¨¡æè°·æ­æµè§å¨æ¥è·åanneæ´å¤æ°æ®ï¼~æç¹å±äºï¼å¸æå¤§ä½¬ææ~)\n\n###
-0.1.3--2022.1.7\n\n- æ°å¢ç»å®æµç§°åsteamid\n-
-æ°å¢å¯ä»¥è¾ç¹äººæ¥è¯¢anneæç»©\n- æ°å¢è§£ç»ä¿¡æ¯\n\n### 0.1.2--
-2022.1.6\n\n- æ°å¢æ¯æå¾çè¾åº\n- æ°å¢æ¥è¯¢anneææ°æ®\n\n###
-0.1.1--2022.1.5\n\n- æ°å¢å é¤å°å¾\n- æ°å¢å°å¾æ¹å\n-
-æ°å¢æ¯æå¾çè¾åº\n\n### 0.1.0--2022.1.4\n\n- éä¸­ä¿®å¤äºBug\n\n###
-0.0.9--2022.1.4\n\n-
-æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­\n-
-ä¿®å¤ä¸­æåä¹±ç é®é¢\n\n### 0.0.8--2022.1.4\n\n-
-æ¯ævpkæ ¼å¼å°å¾\n- æ¯ææ¥çæævpkæ ¼å¼æä»¶\n\n### 0.0.6--
-2022.1.3\n\n- ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç \n\n### 0.0.1--
-2022.1.3\n\n- æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾\n\n\n\n## ð
-å¶ä»\n\n-
+[æ¨¡å¼]æ¥è®¿é® - æ°å¢æ¹éæ¥è¯¢æå¡å¨ï¼ä¸å¸¦åæ°åè¿åå¾ç
+### 0.3.1--2022.2.22 - ä¿®å¤äºè·¯å¾è¯å«ä¸ºstrå¯¹è±¡çéè¯¯ -
+ä¿®å¤äºåå§åæ¾ä¸å°æä»¶çéè¯¯ - ä¿®å¤äºè·¯å¾æ¼æ¥éè¯¯ -
+å¨winç«¯æåæµè¯ï¼ä¿®å¤åç¼©åbug - æ°å¢å¼å³åç¨å¼æ­¥envè®¾ç½®
+- æµè¯rconå»ºç«éè®¯ - å®ç°åæ¢è·¯å¾æ¥çå°å¾åä½¿ç¨rconæä»¤
+### 0.3.0--2022.2.18 -
+ä¿®æ¹äºæ°çenvéç½®ï¼ä½¿å¾æ¯ææ¬å°å¤æå¡å¨æä½ -
+å½»åºè§£å³äºåç¼©åè§£ålinuxç«¯çé®é¢ -
+è§£å³äºwinç«¯é»è®¤gbkè§£ç çéè¯¯ - è§£å³rconæä»¤å­ä½æ¥é ###
+0.2.5--2022.2.10 - ä¿®å¤äºä¾èµä¸è¶³çbug -
+æ´æ°äºçµä¿¡ææç»©ä¸ªäººå¾çUI - æ´æ°äºæ¹éæå¡å¨æ¥ççUI -
+ä¿®æ¹äºä¼ æä»¶ä¸ºåç¨å¼æ­¥ - ä¼åäºé¨årconæä»¤ -
+~tnd7zæä¹ä¸å»æ­»å~ä½¿ç¨pyunpackåºè§£å7z ### 0.2.4--2022.2.8 -
+ä½¿ç¨poetryä¿®å¤äºpipå®è£æä»¶ç¼ºå¤±çbug ### 0.2.3--2022.2.7 -
+æ°å¢åç¢åå¼ç¢ -
+ä¿®æ¹äºè·åèµæºä¸ºå¼æ­¥åç¨å´é»ç¢å¶ä»æä»¤çbug -
+æ°å¢jsonç»è®¡é¨åå·²ç¥æå¡å¨ï¼æªæ¥åºè¯¥ç¬ç«æåºæç»­æ´æ°ï¼å¦æææ¨çéå¬å¼æè®°å½è¯·èç³»æå é¤ï¼
+- å·åå¶ä½å¼æäºï¼æ¨æµéè¦c/c++ç¯å¢ - ä¿®æ¹æ½åææ¡ -
+æ°å¢æ¥è¯¢æå¡å¨ç¶ææ¶è¿åconnect ip -
+ä¿®å¤äºæå¡å¨æ¥è¯¢æ ååºçæ¶åï¼å ä¸ºæ¥éæ åå¤ä¿¡æ¯çbug
+- ä¸ªäººä¿¡æ¯éç½®æµè¯ä»£ç ï¼ä¸ä¸ªçæ¬æ´æ° -
+æ°å¢æ±çæ´æ°æ·»å åå é¤ ### 0.2.2--2022.2.1 - æ°å¢æ¢ç -
+æ°å¢å·æ¼å¶ä½ -
+ä¿®å¤äºé­æ¹æå¡å¨å¯¼è´è§£åéè¯¯çbugï¼å°±æ¯ç´æ¥å¿½ç¥äºï¼ -
+ä¿®æ¹äºé¨åå¯¹è¯ååº ### 0.2.1--2022.1.25 -
+æ°å¢çµä¿¡æè·åï¼ä¸å¥çè¯å®ï¼ - ä¼åå¾çUI -
+æ°å¢äºæå¿«æ·æ¥è¯¢ -
+ä¿®å¤äºå ä¸ºæ²¡ç¨ç©å®¶ï¼å¯¼è´çæå¡å¨ç¶ææ¥è¯¢éè¯¯ -
+æ°å¢çµä¿¡æipç¬åï¼ä»ä»ä½ä¸ºåæ¬¡æ´æ°ipåè¡¨ï¼ ### 0.2.0--
+2022.1.21 - æ°å¢åæå·¥åæ¥è¯¢ - ä¼åæ¥è¯¢å¾çUI -
+æ°å¢åæå·¥åæä»¶ä¸è½½ -
+ä¿®å¤äºå ä¸ºçµä¿¡æå®ç½åç«¯ä¿®æ¹å¯¼è´æ¥è¯¢å¤±è´¥çBUG ### 0.1.7--
+2022.1.19 - æ°å¢ç¾¤ipè®¢éï¼æ¹éæ¥è¯¢ - æ°å¢å¾çæ¾ç¤ºipç¶æ -
+ä¿®å¤äºå ä¸ºç©å®¶åå­ç¹æ®å­ç¬¦å¯¼è´çutf-8è§£ç éè¯¯ -
+æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.6 ### 0.1.6--2022.1.15 -
+æ°å¢ipæ¥è¯¢æå¡å¨æä¾ç©å®¶æ°éååå­ -
+å¢å åç¨å½æ°ä¿®å¤å ä¸ºå è½½é¡ºåºå¯¼è´çéè¯¯ -
+æ´æ°èªå·±çç¬¬ä¸æ¹åºVSQ==0.0.4 ### 0.1.5--2022.1.15 -
+æ°å¢æå¡å¨æ§å¶å°æä»¤ï¼æ°å¢ä¾èµrcon -
+éæ°äºæ°æ®åºï¼ä¸åä½¿ç¨jsonèæ¯ä½¿ç¨sql3 -
+æ¹åäºæ±çanneä¿¡æ¯æ¾ç¤ºæ¹å¼ï¼å¦æåä¸ªæ°æ®ä»¥å¾çæ¾ç¤ºï¼å¦æå¤ä¸ªæ°æ®ä»¥æå­æ¾ç¤º
+### 0.1.4--2022.1.9 - æ°å¢æ±çanneè¯¦æï¼çæåï¼ -
+ææçè¯·æ±æ¹ä¸ºhttpx - æ´æ°äºanneä¿¡æ¯å¾ç -
+å¯éä½¿ç¨æ¨¡æè°·æ­æµè§å¨æ¥è·åanneæ´å¤æ°æ®ï¼~æç¹å±äºï¼å¸æå¤§ä½¬ææ~)
+### 0.1.3--2022.1.7 - æ°å¢ç»å®æµç§°åsteamid -
+æ°å¢å¯ä»¥è¾ç¹äººæ¥è¯¢anneæç»© - æ°å¢è§£ç»ä¿¡æ¯ ### 0.1.2--2022.1.6
+- æ°å¢æ¯æå¾çè¾åº - æ°å¢æ¥è¯¢anneææ°æ® ### 0.1.1--2022.1.5 -
+æ°å¢å é¤å°å¾ - æ°å¢å°å¾æ¹å - æ°å¢æ¯æå¾çè¾åº ### 0.1.0--
+2022.1.4 - éä¸­ä¿®å¤äºBug ### 0.0.9--2022.1.4 -
+æ°å¢ä¸ä¼ å°å¾åï¼æ£æµå¯¹æ¯åå¤æ°å°å¾åå­ -
+ä¿®å¤ä¸­æåä¹±ç é®é¢ ### 0.0.8--2022.1.4 - æ¯ævpkæ ¼å¼å°å¾ -
+æ¯ææ¥çæævpkæ ¼å¼æä»¶ ### 0.0.6--2022.1.3 -
+ä¿®å¤äº7zåç¼©åçæ¹å¼ï¼ä¼åä»£ç  ### 0.0.1--2022.1.3 -
+æä»¶åæ¬¡åå¸ï¼å¯ç§èæ·»å å°å¾  ## ð å¶ä» -
 æ¬äººææ¯å¾å·®ï¼å¦ææ¨æåç°BUGæèæ´å¥½çå»ºè®®ï¼æ¬¢è¿æIssue
-& Pr\n- å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~\n-
-æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é\n- [GPL-3.0 License]
+& Pr - å¦ææ¬æä»¶å¯¹ä½ æå¸®å©ï¼ä¸è¦å¿äºç¹ä¸ªStar~ -
+æ¬é¡¹ç®ä»ä¾å­¦ä¹ ä½¿ç¨ï¼è¯·å¿ç¨äºåä¸ç¨é - [GPL-3.0 License]
 (https://github.com/Agnes4m/nonebot_plugin_l4d2_server/blob/main/LICENSE) Â©
-[@Agnes4m](https://github.com/Agnes4m)\n\n## ð æè°¢\n\n- [nonebot2](https:
-//github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶\n- [ä¿®ä»]
-(https://github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè\n- ~~
+[@Agnes4m](https://github.com/Agnes4m) ## ð æè°¢ - [nonebot2](https://
+github.com/nonebot/nonebot2)- èå¤©æºå¨äººçåºç¡æ¡æ¶ - [ä¿®ä»](https:/
+/github.com/s52047qwas/nonebot_plugin_xiuxian)- æ°æ®åºåè - ~~
 [èªå·±åçæ±çä¹è·¯æ¥è¯¢åº](https://github.com/Agnes4m/VSQ)~~
-(å·²å¼ç¨)\n- [@MeetWq](https://github.com/MeetWq)-
-éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³\n - [å¯ç±å°Q](https://github.com/
-MeetWq/mybot)- æå¡å¨å¾çåè\n- [ç¾¤èå­¦ä¹ ](https://github.com/
-CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè\n-
-[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè\n- [gsuid]
-(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè\n-
-åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®\n', 'author': 'Agnes_Digital',
-'author_email': 'Z735803792@163.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/Agnes4m/nonebot_plugin_l4d2_server',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.9,<4.0', } setup(**setup_kwargs)
+(å·²å¼ç¨) - [@MeetWq](https://github.com/MeetWq)-
+éå¸¸ç­å¿è§£ç­nonebot2ç¸å³çåæ³ - [å¯ç±å°Q](https://github.com/
+MeetWq/mybot)- æå¡å¨å¾çåè - [ç¾¤èå­¦ä¹ ](https://github.com/
+CMHopeSunshine/nonebot-plugin-learning-chat)- webæ§å¶å°åè -
+[æ¥åéº»éº»](https://github.com/Special-Week)- ä»£ç ä¼ååè - [gsuid]
+(https://github.com/KimigaiiWuyi/GenshinUID)- readmeåwikiçæ ¼å¼åè -
+åå- æä¾ä¸æ¹å°å¾çè¯¦ç»æ°æ®
```

