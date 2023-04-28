# Comparing `tmp/basana-1.2.2.tar.gz` & `tmp/basana-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basana-1.2.2.tar", max compression
+gzip compressed data, was "basana-1.3.0.tar", max compression
```

## Comparing `basana-1.2.2.tar` & `basana-1.3.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.2.2/LICENSE
--rw-r--r--   0        0        0     1202 2023-04-02 03:08:50.507049 basana-1.2.2/basana/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.2.2/basana/backtesting/__init__.py
--rw-r--r--   0        0        0     3922 2023-03-29 02:43:04.760023 basana-1.2.2/basana/backtesting/account_balances.py
--rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.2.2/basana/backtesting/errors.py
--rw-r--r--   0        0        0    22387 2023-04-03 17:28:32.835215 basana-1.2.2/basana/backtesting/exchange.py
--rw-r--r--   0        0        0     2567 2023-04-03 17:28:32.836099 basana-1.2.2/basana/backtesting/fees.py
--rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.2.2/basana/backtesting/helpers.py
--rw-r--r--   0        0        0     6250 2023-04-03 17:28:32.836830 basana-1.2.2/basana/backtesting/liquidity.py
--rw-r--r--   0        0        0    15649 2023-04-03 17:28:32.837655 basana-1.2.2/basana/backtesting/orders.py
--rw-r--r--   0        0        0     7953 2023-04-03 02:30:48.915325 basana-1.2.2/basana/backtesting/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.2.2/basana/core/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.2.2/basana/core/bar.py
--rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.2.2/basana/core/config.py
--rw-r--r--   0        0        0     8810 2023-04-04 18:15:17.433460 basana-1.2.2/basana/core/dispatcher.py
--rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.2.2/basana/core/dt.py
--rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.2.2/basana/core/enums.py
--rw-r--r--   0        0        0     3457 2023-04-03 17:28:32.839240 basana-1.2.2/basana/core/event.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.2.2/basana/core/event_sources/__init__.py
--rw-r--r--   0        0        0     3045 2023-03-29 02:43:04.764987 basana-1.2.2/basana/core/event_sources/csv.py
--rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.2.2/basana/core/event_sources/trading_signal.py
--rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.2.2/basana/core/helpers.py
--rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.2.2/basana/core/logs.py
--rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.2.2/basana/core/pair.py
--rw-r--r--   0        0        0     1994 2023-04-04 18:04:16.050858 basana-1.2.2/basana/core/token_bucket.py
--rw-r--r--   0        0        0     6070 2023-03-29 02:43:04.766646 basana-1.2.2/basana/core/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.2.2/basana/external/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.2.2/basana/external/binance/__init__.py
--rw-r--r--   0        0        0    20281 2023-03-29 02:43:04.767507 basana-1.2.2/basana/external/binance/client.py
--rw-r--r--   0        0        0     9695 2023-03-29 02:43:04.767804 basana-1.2.2/basana/external/binance/common.py
--rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.2.2/basana/external/binance/config.py
--rw-r--r--   0        0        0     1453 2023-03-29 02:43:04.768497 basana-1.2.2/basana/external/binance/cross_margin.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.2.2/basana/external/binance/csv/__init__.py
--rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.2.2/basana/external/binance/csv/bars.py
--rw-r--r--   0        0        0     6992 2023-03-29 02:43:04.769607 basana-1.2.2/basana/external/binance/exchange.py
--rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.2.2/basana/external/binance/helpers.py
--rw-r--r--   0        0        0     2304 2023-03-29 02:43:04.770322 basana-1.2.2/basana/external/binance/isolated_margin.py
--rw-r--r--   0        0        0     7375 2023-03-29 02:43:04.770603 basana-1.2.2/basana/external/binance/margin.py
--rw-r--r--   0        0        0     6185 2023-03-29 02:43:04.770874 basana-1.2.2/basana/external/binance/margin_requests.py
--rw-r--r--   0        0        0     3496 2023-03-29 02:43:04.771163 basana-1.2.2/basana/external/binance/order_book.py
--rw-r--r--   0        0        0     7506 2023-03-29 02:43:04.771566 basana-1.2.2/basana/external/binance/spot.py
--rw-r--r--   0        0        0     5575 2023-03-29 02:43:04.771851 basana-1.2.2/basana/external/binance/spot_requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.2.2/basana/external/binance/tools/__init__.py
--rw-r--r--   0        0        0     4373 2023-03-29 02:43:04.772398 basana-1.2.2/basana/external/binance/tools/download_bars.py
--rw-r--r--   0        0        0     2208 2023-03-29 02:43:04.772661 basana-1.2.2/basana/external/binance/trades.py
--rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.2.2/basana/external/binance/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.2.2/basana/external/bitstamp/__init__.py
--rw-r--r--   0        0        0     8684 2023-03-29 02:43:04.773512 basana-1.2.2/basana/external/bitstamp/client.py
--rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.2.2/basana/external/bitstamp/config.py
--rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.2.2/basana/external/bitstamp/csv/__init__.py
--rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.2.2/basana/external/bitstamp/csv/bars.py
--rw-r--r--   0        0        0    16497 2023-03-29 02:43:04.774878 basana-1.2.2/basana/external/bitstamp/exchange.py
--rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.2.2/basana/external/bitstamp/helpers.py
--rw-r--r--   0        0        0     3692 2023-03-29 02:43:04.775434 basana-1.2.2/basana/external/bitstamp/order_book.py
--rw-r--r--   0        0        0     2337 2023-03-29 02:43:04.775718 basana-1.2.2/basana/external/bitstamp/orders.py
--rw-r--r--   0        0        0     4303 2023-03-29 02:43:04.775981 basana-1.2.2/basana/external/bitstamp/requests.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.2.2/basana/external/bitstamp/tools/__init__.py
--rw-r--r--   0        0        0     4069 2023-03-29 02:43:04.777227 basana-1.2.2/basana/external/bitstamp/tools/download_bars.py
--rw-r--r--   0        0        0     2471 2023-03-29 02:43:04.777524 basana-1.2.2/basana/external/bitstamp/trades.py
--rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.2.2/basana/external/bitstamp/websockets.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.2.2/basana/external/common/__init__.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.2.2/basana/external/common/csv/__init__.py
--rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.2.2/basana/external/common/csv/bars.py
--rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.2.2/basana/external/yahoo/__init__.py
--rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.2.2/basana/external/yahoo/bars.py
--rw-r--r--   0        0        0      906 2023-04-04 18:16:48.436528 basana-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1145 1970-01-01 00:00:00.000000 basana-1.2.2/setup.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 basana-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      583 2023-02-25 02:54:08.614680 basana-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1263 2023-04-13 16:56:31.180127 basana-1.3.0/basana/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.759693 basana-1.3.0/basana/backtesting/__init__.py
+-rw-r--r--   0        0        0     3922 2023-04-25 19:59:42.240369 basana-1.3.0/basana/backtesting/account_balances.py
+-rw-r--r--   0        0        0    13416 2023-04-28 03:07:23.322333 basana-1.3.0/basana/backtesting/charts.py
+-rw-r--r--   0        0        0      679 2023-04-03 17:28:32.834201 basana-1.3.0/basana/backtesting/errors.py
+-rw-r--r--   0        0        0    22695 2023-04-28 03:07:23.323961 basana-1.3.0/basana/backtesting/exchange.py
+-rw-r--r--   0        0        0     2547 2023-04-28 03:07:23.324848 basana-1.3.0/basana/backtesting/fees.py
+-rw-r--r--   0        0        0     1683 2023-03-29 02:43:04.761285 basana-1.3.0/basana/backtesting/helpers.py
+-rw-r--r--   0        0        0     6150 2023-04-28 03:07:23.325407 basana-1.3.0/basana/backtesting/liquidity.py
+-rw-r--r--   0        0        0    16012 2023-04-28 03:07:23.326054 basana-1.3.0/basana/backtesting/orders.py
+-rw-r--r--   0        0        0     7913 2023-04-28 03:07:23.326667 basana-1.3.0/basana/backtesting/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.762632 basana-1.3.0/basana/core/__init__.py
+-rw-r--r--   0        0        0     6035 2023-04-03 17:28:32.838372 basana-1.3.0/basana/core/bar.py
+-rw-r--r--   0        0        0     1394 2023-03-29 02:43:04.763204 basana-1.3.0/basana/core/config.py
+-rw-r--r--   0        0        0     9620 2023-04-28 03:07:23.327710 basana-1.3.0/basana/core/dispatcher.py
+-rw-r--r--   0        0        0     1493 2023-03-29 02:43:04.763794 basana-1.3.0/basana/core/dt.py
+-rw-r--r--   0        0        0      968 2023-03-29 02:43:04.764040 basana-1.3.0/basana/core/enums.py
+-rw-r--r--   0        0        0     3456 2023-04-28 03:07:23.328623 basana-1.3.0/basana/core/event.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.764708 basana-1.3.0/basana/core/event_sources/__init__.py
+-rw-r--r--   0        0        0     3025 2023-04-28 03:07:23.329229 basana-1.3.0/basana/core/event_sources/csv.py
+-rw-r--r--   0        0        0     2277 2023-04-03 17:28:32.840140 basana-1.3.0/basana/core/event_sources/trading_signal.py
+-rw-r--r--   0        0        0     2978 2023-03-29 02:43:04.765532 basana-1.3.0/basana/core/helpers.py
+-rw-r--r--   0        0        0     1539 2023-03-29 02:43:04.765805 basana-1.3.0/basana/core/logs.py
+-rw-r--r--   0        0        0     1459 2023-04-03 17:28:32.841069 basana-1.3.0/basana/core/pair.py
+-rw-r--r--   0        0        0     2280 2023-04-13 16:56:31.182428 basana-1.3.0/basana/core/token_bucket.py
+-rw-r--r--   0        0        0     6010 2023-04-28 03:07:23.329823 basana-1.3.0/basana/core/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.766920 basana-1.3.0/basana/external/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.767178 basana-1.3.0/basana/external/binance/__init__.py
+-rw-r--r--   0        0        0    20702 2023-04-28 03:07:23.330411 basana-1.3.0/basana/external/binance/client.py
+-rw-r--r--   0        0        0    10335 2023-04-13 16:56:31.184239 basana-1.3.0/basana/external/binance/common.py
+-rw-r--r--   0        0        0      867 2023-03-29 02:43:04.768133 basana-1.3.0/basana/external/binance/config.py
+-rw-r--r--   0        0        0     2111 2023-04-13 16:56:31.184643 basana-1.3.0/basana/external/binance/cross_margin.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.768810 basana-1.3.0/basana/external/binance/csv/__init__.py
+-rw-r--r--   0        0        0     1648 2023-03-29 02:43:04.769173 basana-1.3.0/basana/external/binance/csv/bars.py
+-rw-r--r--   0        0        0    10385 2023-04-16 21:31:22.354698 basana-1.3.0/basana/external/binance/exchange.py
+-rw-r--r--   0        0        0     3052 2023-03-29 02:43:04.769989 basana-1.3.0/basana/external/binance/helpers.py
+-rw-r--r--   0        0        0     3187 2023-04-13 16:56:31.186035 basana-1.3.0/basana/external/binance/isolated_margin.py
+-rw-r--r--   0        0        0     1913 2023-04-13 16:56:31.186636 basana-1.3.0/basana/external/binance/klines.py
+-rw-r--r--   0        0        0    12082 2023-04-28 03:07:23.331079 basana-1.3.0/basana/external/binance/margin.py
+-rw-r--r--   0        0        0     6165 2023-04-28 03:07:23.331858 basana-1.3.0/basana/external/binance/margin_requests.py
+-rw-r--r--   0        0        0     4143 2023-04-16 21:31:22.355396 basana-1.3.0/basana/external/binance/order_book.py
+-rw-r--r--   0        0        0    12177 2023-04-13 16:56:31.188619 basana-1.3.0/basana/external/binance/spot.py
+-rw-r--r--   0        0        0     5555 2023-04-28 03:07:23.332666 basana-1.3.0/basana/external/binance/spot_requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.772127 basana-1.3.0/basana/external/binance/tools/__init__.py
+-rw-r--r--   0        0        0     4373 2023-03-29 02:43:04.772398 basana-1.3.0/basana/external/binance/tools/download_bars.py
+-rw-r--r--   0        0        0     2710 2023-04-13 16:56:31.189265 basana-1.3.0/basana/external/binance/trades.py
+-rw-r--r--   0        0        0     2647 2023-03-29 02:43:04.772931 basana-1.3.0/basana/external/binance/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.773220 basana-1.3.0/basana/external/bitstamp/__init__.py
+-rw-r--r--   0        0        0     8684 2023-03-29 02:43:04.773512 basana-1.3.0/basana/external/bitstamp/client.py
+-rw-r--r--   0        0        0      865 2023-03-29 02:43:04.773899 basana-1.3.0/basana/external/bitstamp/config.py
+-rw-r--r--   0        0        0      662 2023-03-29 02:43:04.774215 basana-1.3.0/basana/external/bitstamp/csv/__init__.py
+-rw-r--r--   0        0        0     2047 2023-03-29 02:43:04.774543 basana-1.3.0/basana/external/bitstamp/csv/bars.py
+-rw-r--r--   0        0        0    23031 2023-04-16 21:31:22.356361 basana-1.3.0/basana/external/bitstamp/exchange.py
+-rw-r--r--   0        0        0     2374 2023-03-29 02:43:04.775164 basana-1.3.0/basana/external/bitstamp/helpers.py
+-rw-r--r--   0        0        0     4150 2023-04-16 21:31:22.357186 basana-1.3.0/basana/external/bitstamp/order_book.py
+-rw-r--r--   0        0        0     3067 2023-04-16 21:31:22.357564 basana-1.3.0/basana/external/bitstamp/orders.py
+-rw-r--r--   0        0        0     4283 2023-04-28 03:07:23.333551 basana-1.3.0/basana/external/bitstamp/requests.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.776276 basana-1.3.0/basana/external/bitstamp/tools/__init__.py
+-rw-r--r--   0        0        0     4069 2023-03-29 02:43:04.777227 basana-1.3.0/basana/external/bitstamp/tools/download_bars.py
+-rw-r--r--   0        0        0     2968 2023-04-16 21:31:22.357932 basana-1.3.0/basana/external/bitstamp/trades.py
+-rw-r--r--   0        0        0     4620 2023-03-29 02:43:04.777839 basana-1.3.0/basana/external/bitstamp/websockets.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778237 basana-1.3.0/basana/external/common/__init__.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.778648 basana-1.3.0/basana/external/common/csv/__init__.py
+-rw-r--r--   0        0        0     1763 2023-03-29 02:43:04.779031 basana-1.3.0/basana/external/common/csv/bars.py
+-rw-r--r--   0        0        0      608 2023-03-29 02:43:04.779403 basana-1.3.0/basana/external/yahoo/__init__.py
+-rw-r--r--   0        0        0     3384 2023-03-29 02:43:04.779788 basana-1.3.0/basana/external/yahoo/bars.py
+-rw-r--r--   0        0        0     1161 2023-04-28 03:12:38.894557 basana-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 basana-1.3.0/setup.py
+-rw-r--r--   0        0        0      951 1970-01-01 00:00:00.000000 basana-1.3.0/PKG-INFO
```

### Comparing `basana-1.2.2/LICENSE` & `basana-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/__init__.py` & `basana-1.3.0/basana/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,12 @@
     truncate_decimal,
 )
 
 from .core.pair import (
     Pair,
     PairInfo,
 )
+
+from .core.token_bucket import (
+    TokenBucketLimiter,
+)
+
```

### Comparing `basana-1.2.2/basana/backtesting/__init__.py` & `basana-1.3.0/basana/backtesting/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/backtesting/account_balances.py` & `basana-1.3.0/basana/backtesting/account_balances.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/backtesting/errors.py` & `basana-1.3.0/basana/backtesting/errors.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/backtesting/exchange.py` & `basana-1.3.0/basana/backtesting/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import decimal
 from decimal import Decimal
-from typing import cast, Any, Awaitable, Callable, Dict, Generator, List, Optional, Tuple
+from typing import cast, Any, Awaitable, Callable, Dict, Generator, List, Optional, Sequence, Tuple
 import copy
 import dataclasses
 import logging
 import uuid
 
 from basana.backtesting import account_balances, errors, fees, liquidity, orders, requests
 from basana.backtesting import helpers as bt_helpers
@@ -73,14 +73,17 @@
                 yield order
                 if new_open_orders is not None and order.is_open:
                     new_open_orders.append(order)
 
         if new_open_orders is not None:
             self._open_orders = new_open_orders
 
+    def get_all_orders(self) -> Sequence[orders.Order]:
+        return self._orders.values()
+
 
 @dataclasses.dataclass
 class Balance:
     #: The available balance.
     available: Decimal
     #: The total balance (available + reserved).
     total: Decimal
@@ -332,15 +335,15 @@
         """
         self._dispatcher.subscribe(bar_source, self._on_bar_event)
 
     def subscribe_to_bar_events(self, pair: Pair, event_handler: BarEventHandler):
         """Registers an async callable that will be called when a new bar is available.
 
         :param pair: The trading pair.
-        :param event_handler: An async callable that receives a :class:`basana.BarEvent`.
+        :param event_handler: An async callable that receives a basana.BarEvent.
         """
         # Get/create the event source for the given pair.
         event_source = self._bar_event_source.get(pair)
         if event_source is None:
             event_source = event.FifoQueueEventSource()
             self._bar_event_source[pair] = event_source
         self._dispatcher.subscribe(event_source, cast(dispatcher.EventHandler, event_handler))
@@ -452,15 +455,15 @@
                 break
 
         # Update, or fail.
         if not balances_short:
             # Update the liquidity strategy.
             liquidity_strategy.take_liquidity(abs(balance_updates[bar_event.bar.pair.base_symbol]))
             # Update the order.
-            order.add_fill(balance_updates, fees)
+            order.add_fill(bar_event.when, balance_updates, fees)
             # Update balances.
             self._balances.order_updated(order, final_updates)
             logger.debug(logs.StructuredMessage(
                 "Order updated", order_id=order.id, final_updates=final_updates, order_state=order.state
             ))
         else:
             order_not_filled()
@@ -515,7 +518,13 @@
             order = order_request.create_order("temporary")
             fees = self._fee_strategy.calculate_fees(order, estimated_balance_updates)
             fees = self._round_fees(order_request.pair, fees)
         estimated_balance_updates = bt_helpers.add_amounts(estimated_balance_updates, fees)
 
         # Return only negative balance updates as required balances.
         return {symbol: -amount for symbol, amount in estimated_balance_updates.items() if amount < Decimal(0)}
+
+    def _get_all_orders(self) -> Sequence[orders.Order]:
+        return self._orders.get_all_orders()
+
+    def _get_dispatcher(self) -> dispatcher.EventDispatcher:
+        return self._dispatcher
```

### Comparing `basana-1.2.2/basana/backtesting/fees.py` & `basana-1.3.0/basana/backtesting/fees.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     .. note::
 
         * This is a base class and should not be used directly.
     """
 
     def calculate_fees(
             self, order: orders.Order, balance_updates: Dict[str, Decimal]
-    ) -> Dict[str, Decimal]:  # pragma: no cover
+    ) -> Dict[str, Decimal]:
         """TODO."""
         raise NotImplementedError()
 
 
 class NoFee(FeeStrategy):
     """This strategy applies no fees to the trades."""
```

### Comparing `basana-1.2.2/basana/backtesting/helpers.py` & `basana-1.3.0/basana/backtesting/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/backtesting/liquidity.py` & `basana-1.3.0/basana/backtesting/liquidity.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,40 +30,40 @@
 
         * This is a base class and should not be used directly.
         * Concrete strategies will be created by the :class:`basana.backtesting.exchange.Exchange` for each traded
           pair.
     """
 
     @abc.abstractmethod
-    def on_bar(self, bar: bar.Bar):  # pragma: no cover
+    def on_bar(self, bar: bar.Bar):
         """Called when a new bar is available."""
         raise NotImplementedError()
 
     @property
     @abc.abstractmethod
-    def available_liquidity(self) -> Decimal:  # pragma: no cover
+    def available_liquidity(self) -> Decimal:
         """Returns the available liquidity."""
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def take_liquidity(self, amount: Decimal) -> Decimal:  # pragma: no cover
+    def take_liquidity(self, amount: Decimal) -> Decimal:
         """Takes/consumes available liquidity.
 
         :param amount: The amount of liquidity to take. It must be <= available liquidity.
         :returns: The percentage of the price impact.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def calculate_price_impact(self, amount: Decimal) -> Decimal:  # pragma: no cover
+    def calculate_price_impact(self, amount: Decimal) -> Decimal:
         """A read-only version of :meth:`take_liquidity`."""
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def calculate_amount(self, price_impact: Decimal) -> Decimal:  # pragma: no cover
+    def calculate_amount(self, price_impact: Decimal) -> Decimal:
         """Returns the amount of liquidity that can be taken with an impact <= price_impact."""
         raise NotImplementedError()
 
 
 class InfiniteLiquidity(LiquidityStrategy):
     """This class models infinite liquidity with no price impact."""
```

### Comparing `basana-1.2.2/basana/backtesting/orders.py` & `basana-1.3.0/basana/backtesting/orders.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 import abc
 import dataclasses
+import datetime
 import enum
 import logging
 
 from basana.backtesting import helpers, liquidity
 from basana.core import bar, logs
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
@@ -57,26 +58,34 @@
         """The fill price."""
         fill_price = None
         if self.amount_filled:
             fill_price = self.quote_amount_filled / self.amount_filled
         return fill_price
 
 
+@dataclasses.dataclass
+class Fill:
+    when: datetime.datetime
+    balance_updates: Dict[str, Decimal]
+    fees: Dict[str, Decimal]
+
+
 # This is an internal abstraction to be used by the exchange.
 class Order:
     def __init__(self, id: str, operation: OrderOperation, pair: Pair, amount: Decimal, state: OrderState):
         assert amount > Decimal(0), f"Invalid amount {amount}"
 
         self._id = id
         self._operation = operation
         self._pair = pair
         self._amount = amount
         self._state = state
         self._balance_updates: Dict[str, Decimal] = {}
         self._fees: Dict[str, Decimal] = {}
+        self._fills: List[Fill] = []
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
     def pair(self) -> Pair:
@@ -114,35 +123,40 @@
     def amount_pending(self) -> Decimal:
         return self._amount - self.amount_filled
 
     @property
     def quote_amount_filled(self) -> Decimal:
         return abs(self._balance_updates.get(self.pair.quote_symbol, Decimal(0)))
 
+    @property
+    def fills(self) -> List[Fill]:
+        return self._fills
+
     def cancel(self):
         assert self._state == OrderState.OPEN
         self._state = OrderState.CANCELED
 
-    def add_fill(self, balance_updates: Dict[str, Decimal], fees: Dict[str, Decimal]):
+    def add_fill(self, when: datetime.datetime, balance_updates: Dict[str, Decimal], fees: Dict[str, Decimal]):
         self._balance_updates = helpers.add_amounts(self._balance_updates, balance_updates)
         self._fees = helpers.add_amounts(self._fees, fees)
         if self.amount_filled >= self.amount:
             self._state = OrderState.COMPLETED
+        self._fills.append(Fill(when=when, balance_updates=balance_updates, fees=fees))
 
     def get_order_info(self) -> OrderInfo:
         return OrderInfo(
             id=self.id, is_open=self._state == OrderState.OPEN, amount_filled=self.amount_filled,
             amount_remaining=self.amount_pending, quote_amount_filled=self.quote_amount_filled,
             fees={symbol: -amount for symbol, amount in self._fees.items() if amount}
         )
 
     @abc.abstractmethod
     def get_balance_updates(
             self, bar: bar.Bar, liquidity_strategy: liquidity.LiquidityStrategy
-    ) -> Dict[str, Decimal]:  # pragma: no cover
+    ) -> Dict[str, Decimal]:
         """Returns the balance updates required to fill the order.
 
         :param bar: The bar that summarizes the trading activity.
         :param liquidity_strategy: The strategy used to model available liquidity.
         :returns: A dictionary that maps the symbol to the amount.
 
         .. note::
```

### Comparing `basana-1.2.2/basana/backtesting/requests.py` & `basana-1.3.0/basana/backtesting/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,23 +47,23 @@
             raise errors.Error("Amount must be > 0")
         if self.amount != helpers.truncate_decimal(self.amount, pair_info.base_precision):
             raise errors.Error(
                 "{} exceeds maximum precision of {} decimal digits".format(self.amount, pair_info.base_precision)
             )
 
     @abc.abstractmethod
-    def get_estimated_fill_price(self) -> Optional[Decimal]:  # pragma: no cover
+    def get_estimated_fill_price(self) -> Optional[Decimal]:
         """ Returns the estimated fill price for the order.
 
         This will be used to estimate the cost of executing this order.
         """
         raise NotImplementedError()
 
     @abc.abstractmethod
-    def create_order(self, id: str) -> orders.Order:  # pragma: no cover
+    def create_order(self, id: str) -> orders.Order:
         raise NotImplementedError()
 
 
 class MarketOrder(ExchangeOrder):
     """Market order request.
 
     A market order is an order to buy or sell a stock at the best available price.
```

### Comparing `basana-1.2.2/basana/core/__init__.py` & `basana-1.3.0/basana/core/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/bar.py` & `basana-1.3.0/basana/core/bar.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/config.py` & `basana-1.3.0/basana/core/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/dispatcher.py` & `basana-1.3.0/basana/core/dispatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,18 +41,19 @@
         trading:
 
         * :func:`basana.backtesting_dispatcher`
         * :func:`basana.realtime_dispatcher`
     """
 
     def __init__(self, strict_order: bool = True, stop_when_idle: bool = True):
-        self._event_handlers: Dict[event.EventSource, Set[EventHandler]] = {}
+        self._event_handlers: Dict[event.EventSource, List[EventHandler]] = {}
         self._prefetched_events: Dict[event.EventSource, Optional[event.Event]] = {}
         self._prev_events: Dict[event.EventSource, datetime.datetime] = {}
-        self._idle_handlers: Set[IdleHandler] = set()
+        self._idle_handlers: List[IdleHandler] = []
+        self._sniffers: List[EventHandler] = []
         self._producers: Set[event.Producer] = set()
         self._open_task_group: Optional[helpers.TaskGroup] = None
         self._strict_order = strict_order
         self._stop_when_idle = stop_when_idle
         self._running = False
         self._stopped = False
         self._current_event_dt = None
@@ -70,29 +71,41 @@
 
     def subscribe_idle(self, idle_handler: IdleHandler):
         """Registers an async callable that will be called when there are no events to dispatch.
 
         :param idle_handler: An async callable that receives no arguments.
         """
 
-        # Called when there are no events to dispatch.
-        self._idle_handlers.add(idle_handler)
+        if idle_handler not in self._idle_handlers:
+            self._idle_handlers.append(idle_handler)
 
     def subscribe(self, source: event.EventSource, event_handler: EventHandler):
         """Registers an async callable that will be called when an event source has new events.
 
         :param source: An event source.
         :param event_handler: An async callable that receives an event.
         """
 
         assert not self._running
-        self._event_handlers.setdefault(source, set()).add(event_handler)
+        handlers = self._event_handlers.setdefault(source, [])
+        if event_handler not in handlers:
+            handlers.append(event_handler)
         if source.producer:
             self._producers.add(source.producer)
 
+    def subscribe_all(self, event_handler: EventHandler):
+        """Registers an async callable that will be called for all events.
+
+        :param event_handler: An async callable that receives an event.
+        """
+
+        assert not self._running
+        if event_handler not in self._sniffers:
+            self._sniffers.append(event_handler)
+
     async def run(self, stop_signals: List[int] = [signal.SIGINT, signal.SIGTERM]):
         """Executes the event dispatch loop.
 
         :param stop_signals: The signals that will be handled to request :func:`run()` to :func:`stop()`.
 
         This method will execute the following steps in order:
 
@@ -100,14 +113,15 @@
         #. Call :meth:`basana.Producer.main` on all producers and execute event dispatch loop until stopped.
         #. Call :meth:`basana.Producer.finalize` on all producers.
         """
 
         assert not self._running, "Running or already ran"
         assert self._open_task_group is None
 
+        # This block has coverage on all platforms except on Windows.
         if platform.system() != "Windows":  # pragma: no cover
             for stop_signal in stop_signals:
                 asyncio.get_event_loop().add_signal_handler(stop_signal, self.stop)
 
         self._running = True
         try:
             # Initialize producers.
@@ -164,22 +178,26 @@
         # Calculate the datetime for the next event using the prefetched events.
         next_dt = self._get_next_dt_from_prefetched()
         assert ge_or_assert is None or next_dt is None or next_dt >= ge_or_assert, \
             f"{next_dt} can't be dispatched after {ge_or_assert}"
 
         # Dispatch events matching the desired datetime.
         event_handlers = []
+        sniffer_event_handlers = []
         for source, e in self._prefetched_events.items():
             if e is not None and e.when == next_dt:
                 # Collect event handlers for the event source.
                 event_handlers += [event_handler(e) for event_handler in self._event_handlers.get(source, [])]
+                # Sniffers handle all events, no matter what their source is.
+                sniffer_event_handlers += [event_handler(e) for event_handler in self._sniffers]
                 # Consume the event.
                 self._prefetched_events[source] = None
 
         self._current_event_dt = next_dt
+        event_handlers.extend(sniffer_event_handlers)
         await asyncio.gather(*event_handlers)
         self._current_event_dt = None
 
         return next_dt
 
     async def _dispatch_loop(self):
         last_dt = None
```

### Comparing `basana-1.2.2/basana/core/dt.py` & `basana-1.3.0/basana/core/dt.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/enums.py` & `basana-1.3.0/basana/core/enums.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/event.py` & `basana-1.3.0/basana/core/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         This is a base class and should not be used directly.
     """
 
     def __init__(self, when: datetime.datetime):
         assert not dt.is_naive(when), f"{when} should have timezone information set"
 
         #: The datetime when the event occurred.
-        self.when = when
+        self.when: datetime.datetime = when
 
 
 class EventSource(metaclass=abc.ABCMeta):
     """Base class for event sources.
 
     This class declares the interface that is required by the :class:`basana.EventDispatcher` to gather events for
     processing.
@@ -79,15 +79,15 @@
     :param producer: An optional producer associated with this event source.
     """
 
     def __init__(self, producer: Optional[Producer] = None):
         self.producer = producer
 
     @abc.abstractmethod
-    def pop(self) -> Optional[Event]:  # pragma: no cover
+    def pop(self) -> Optional[Event]:
         """Override to return the next event, or None if there are no events available.
 
         This method is used by the :class:`basana.EventDispatcher` during the event dispatch loop so **it should return
         as soon as possible**.
         """
         raise NotImplementedError()
```

### Comparing `basana-1.2.2/basana/core/event_sources/__init__.py` & `basana-1.3.0/basana/core/event_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/event_sources/csv.py` & `basana-1.3.0/basana/core/event_sources/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # * aiofiles delegates operations to a separate thread pool
 # * this module will be used mostly for backtesting where there is no other IO taking place
 # I decided not to support async io initially.
 
 
 class RowParser(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def parse_row(self, row_dict: dict) -> Sequence[event.Event]:  # pragma: no cover
+    def parse_row(self, row_dict: dict) -> Sequence[event.Event]:
         raise NotImplementedError()
 
 
 def load_sort_and_yield(csv_path: str, row_parser: RowParser, dict_reader_kwargs: dict = {}):
     events = []
 
     # Load events.
```

### Comparing `basana-1.2.2/basana/core/event_sources/trading_signal.py` & `basana-1.3.0/basana/core/event_sources/trading_signal.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/helpers.py` & `basana-1.3.0/basana/core/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/logs.py` & `basana-1.3.0/basana/core/logs.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/pair.py` & `basana-1.3.0/basana/core/pair.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/core/token_bucket.py` & `basana-1.3.0/basana/core/token_bucket.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,21 @@
 # limitations under the License.
 
 import asyncio
 import time
 
 
 class TokenBucketLimiter:
+    """This class implements a token bucket algorithm, useful for throttling requests.
+
+    :param tokens_per_period: The maximum amount of tokens per perdiod.
+    :param period_duration: The period duration in seconds.
+    :param initial_tokens: The initial amount of tokens.
+    """
+
     def __init__(self, tokens_per_period: float, period_duration: int, initial_tokens=0):
         assert tokens_per_period > 0
         assert period_duration > 0
         assert initial_tokens >= 0
 
         self._tokens_per_period = tokens_per_period
         self._period_duration = period_duration
```

### Comparing `basana-1.2.2/basana/core/websockets.py` & `basana-1.3.0/basana/core/websockets.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 # Base class for event sources that generate events from websocket messages.
 class ChannelEventSource(event.FifoQueueEventSource):
     def __init__(self, producer: event.Producer):
         super().__init__(producer=producer)
 
     @abc.abstractmethod
-    async def push_from_message(self, message: dict):  # pragma: no cover
+    async def push_from_message(self, message: dict):
         raise NotImplementedError()
 
 
 class WebSocketClient(event.Producer, metaclass=abc.ABCMeta):
     """"Base class for channel based web socket clients."""
     def __init__(
             self, url: str, session: Optional[aiohttp.ClientSession] = None, config_overrides: dict = {},
@@ -106,19 +106,19 @@
                     tg.create_task(self._reconnect(ws_cli))
             except Exception as e:
                 await self.on_error(e)
 
     @abc.abstractmethod
     async def subscribe_to_channels(
             self, channels: List[str], ws_cli: aiohttp.ClientWebSocketResponse
-    ):  # pragma: no cover
+    ):
         raise NotImplementedError()
 
     @abc.abstractmethod
-    async def handle_message(self, message: dict) -> bool:  # pragma: no cover
+    async def handle_message(self, message: dict) -> bool:
         raise NotImplementedError()
 
     async def _msg_loop(self, ws_cli: aiohttp.ClientWebSocketResponse):
         logger.debug(logs.StructuredMessage("Running message loop", src=self))
 
         # The iterator exits normally when the connection is closed with close code 1000 (OK) or 1001 (going away).
         # It raises a ConnectionClosedError when the connection is closed with any other code.
```

### Comparing `basana-1.2.2/basana/external/__init__.py` & `basana-1.3.0/basana/external/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/__init__.py` & `basana-1.3.0/basana/external/binance/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/client.py` & `basana-1.3.0/basana/external/binance/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,20 +27,33 @@
 
 from . import config, helpers
 from basana.core import token_bucket, helpers as core_helpers
 from basana.core.config import get_config_value
 
 
 class Error(Exception):
-    def __init__(self, msg: str, code: Optional[int], resp: aiohttp.ClientResponse, json_response):
+    """
+    An error returned by the exchange.
+
+    :param msg: The error message, if available.
+    :param code: The error code, if available.
+    :param resp: The response.
+    :param json_response: The response body, if it was a JSON.
+    """
+    def __init__(self, msg: str, code: Optional[int], resp: aiohttp.ClientResponse, json_response: Optional[Any]):
         super().__init__(msg)
+        #: The error message.
         self.msg = msg
+        #: The error code, if available.
         self.code = code
+        #: The HTTP status code.
         self.http_status = resp.status
+        #: The HTTP reason.
         self.http_reason = resp.reason
+        #: The response body, if it was a JSON.
         self.json_response = json_response
 
 
 def raise_for_error(resp: aiohttp.ClientResponse, json_response):
     msg = None
     code = None
     if isinstance(json_response, dict):
@@ -285,15 +298,15 @@
 
 class MarginAccount(metaclass=abc.ABCMeta):
     def __init__(self, client: APIClient):
         self._client = client
 
     @property
     @abc.abstractmethod
-    def is_isolated(self) -> bool:  # pragma: no cover
+    def is_isolated(self) -> bool:
         raise NotImplementedError()
 
     async def create_order(
             self, symbol: str, side: str, type: str, time_in_force: Optional[str] = None,
             quantity: Optional[Decimal] = None, quote_order_qty: Optional[Decimal] = None,
             price: Optional[Decimal] = None, stop_price: Optional[Decimal] = None,
             new_client_order_id: Optional[str] = None, side_effect_type: Optional[str] = None, **kwargs: Dict[str, Any]
```

### Comparing `basana-1.2.2/basana/external/binance/common.py` & `basana-1.3.0/basana/external/binance/common.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,35 +25,40 @@
 
 class Balance:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def available(self) -> Decimal:
+        """The available balance."""
         return Decimal(self.json["free"])
 
     @property
     def total(self) -> Decimal:
+        """The total balance (available + locked)."""
         return self.available + self.locked
 
     @property
     def locked(self) -> Decimal:
+        """The locked balance."""
         return Decimal(self.json["locked"])
 
 
 class Trade:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def id(self) -> str:
+        """The trade id."""
         return str(self.json["id"])
 
     @property
     def order_id(self) -> str:
+        """The order id."""
         return str(self.json["orderId"])
 
     @property
     def datetime(self) -> datetime.datetime:
         return helpers.timestamp_to_datetime(self.json["time"])
 
     @property
@@ -85,283 +90,295 @@
         return Decimal(self.json["commission"])
 
     @property
     def commission_asset(self) -> str:
         return self.json["commissionAsset"]
 
 
-class OrderInfo:
-    def __init__(self, json: dict, trades: Sequence[Trade]):
+class OrderWrapper:
+    def __init__(self, json: dict):
         self.json = json
-        self.trades = trades
-        self._fees: Dict[str, Decimal] = collections.defaultdict(Decimal)
-        for trade in trades:
-            if trade.commission:
-                self._fees[trade.commission_asset] += trade.commission
 
     @property
     def id(self) -> str:
+        """The order id."""
         return str(self.json["orderId"])
 
     @property
-    def is_open(self) -> bool:
-        return helpers.order_status_is_open(self.json["status"])
+    def client_order_id(self) -> str:
+        """The client order id."""
+        return self.json["clientOrderId"]
 
     @property
-    def amount_filled(self) -> Decimal:
-        return Decimal(self.json["executedQty"])
+    def order_list_id(self) -> Optional[str]:
+        """The order list id."""
+        ret = self.json.get("orderListId")
+        ret = None if ret in [None, -1] else str(ret)
+        return ret
 
     @property
-    def amount_remaining(self) -> Decimal:
-        return self.amount - self.amount_filled
+    def status(self) -> str:
+        """The status.
+
+        Check **Order status** in https://binance-docs.github.io/apidocs/spot/en/#public-api-definitions.
+        """
+        return self.json["status"]
 
     @property
-    def quote_amount_filled(self) -> Decimal:
-        return Decimal(self.json["cummulativeQuoteQty"])
+    def is_open(self) -> bool:
+        """True if the order is open, False otherwise."""
+        return helpers.order_status_is_open(self.status)
 
     @property
-    def fill_price(self) -> Optional[Decimal]:
-        ret = None
-        if self.amount_filled:
-            ret = self.quote_amount_filled / self.amount_filled
-        return ret
+    def amount(self) -> Decimal:
+        """The amount."""
+        return Decimal(self.json["origQty"])
 
     @property
-    def fees(self) -> Dict[str, Decimal]:
-        return self._fees
+    def amount_filled(self) -> Decimal:
+        """The amount filled."""
+        return Decimal(self.json["executedQty"])
 
     @property
-    def amount(self) -> Decimal:
-        return Decimal(self.json["origQty"])
+    def quote_amount_filled(self) -> Decimal:
+        """The amount filled in quote units."""
+        return Decimal(self.json["cummulativeQuoteQty"])
 
     @property
     def limit_price(self) -> Optional[Decimal]:
+        """The limit price."""
         return helpers.get_optional_decimal(self.json, "price", True)
 
     @property
     def stop_price(self) -> Optional[Decimal]:
+        """The stop price."""
         return helpers.get_optional_decimal(self.json, "stopPrice", True)
 
+    @property
+    def time_in_force(self) -> Optional[str]:
+        """The time in force.
+
+        Check **Time in force** in https://binance-docs.github.io/apidocs/spot/en/#public-api-definitions.
+        """
+        return self.json.get("timeInForce")
+
+
+class OrderInfo(OrderWrapper):
+    def __init__(self, json: dict, trades: Sequence[Trade]):
+        super().__init__(json)
+        self.trades = trades
+        self._fees: Dict[str, Decimal] = collections.defaultdict(Decimal)
+        for trade in trades:
+            if trade.commission:
+                self._fees[trade.commission_asset] += trade.commission
+
+    @property
+    def amount_remaining(self) -> Decimal:
+        """The amount remaining to be filled."""
+        return self.amount - self.amount_filled
+
+    @property
+    def fill_price(self) -> Optional[Decimal]:
+        """The fill price."""
+        ret = None
+        if self.amount_filled:
+            ret = self.quote_amount_filled / self.amount_filled
+        return ret
+
+    @property
+    def fees(self) -> Dict[str, Decimal]:
+        """The fees."""
+        return self._fees
+
 
 class Fill:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def price(self) -> Decimal:
+        """The price."""
         return Decimal(self.json["price"])
 
     @property
     def amount(self) -> Decimal:
+        """The amount."""
         return Decimal(self.json["qty"])
 
     @property
     def commission(self) -> Decimal:
+        """The commission."""
         return Decimal(self.json["commission"])
 
     @property
     def commission_asset(self) -> str:
+        """The commission asset."""
         return self.json["commissionAsset"]
 
 
 class CreatedOrder:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def id(self) -> str:
+        """The order id."""
         return str(self.json["orderId"])
 
     @property
     def datetime(self) -> datetime.datetime:
+        """The creation datetime."""
         return helpers.timestamp_to_datetime(self.json["transactTime"])
 
     @property
     def client_order_id(self) -> str:
+        """The client order id."""
         return self.json["clientOrderId"]
 
     @property
     def limit_price(self) -> Optional[Decimal]:
-        # Only available for RESULT / FULL responses.
+        """The limit price.
+
+        Only available for RESULT / FULL responses.
+        """
         return helpers.get_optional_decimal(self.json, "price", True)
 
     @property
     def amount(self) -> Optional[Decimal]:
-        # Only available for RESULT / FULL responses.
+        """The amount.
+
+        Only available for RESULT / FULL responses.
+        """
         return helpers.get_optional_decimal(self.json, "origQty", False)
 
     @property
     def amount_filled(self) -> Optional[Decimal]:
-        # Only available for RESULT / FULL responses.
+        """The amount filled.
+
+        Only available for RESULT / FULL responses.
+        """
         return helpers.get_optional_decimal(self.json, "executedQty", False)
 
     @property
     def quote_amount_filled(self) -> Optional[Decimal]:
-        # Only available for RESULT / FULL responses.
+        """The amount filled in quote units.
+
+        Only available for RESULT / FULL responses.
+        """
         return helpers.get_optional_decimal(self.json, "cummulativeQuoteQty", False)
 
     @property
     def status(self) -> Optional[str]:
-        # Only available for RESULT / FULL responses.
+        """The status.
+
+        Only available for RESULT / FULL responses.
+        """
         return self.json.get("status")
 
     @property
     def time_in_force(self) -> Optional[str]:
-        # Only available for RESULT / FULL responses.
+        """The time in force.
+
+        Only available for RESULT / FULL responses.
+        """
         return self.json.get("timeInForce")
 
     @property
     def is_open(self) -> bool:
-        # Only available for RESULT / FULL responses.
+        """True if the order is open, False otherwise.
+
+        Only available for RESULT / FULL responses.
+        """
         assert self.status is not None, "status not set"
         return helpers.order_status_is_open(self.status)
 
 
-class CanceledOrder:
-    def __init__(self, json: dict):
-        self.json = json
-
-    @property
-    def id(self) -> str:
-        return str(self.json["orderId"])
-
-    @property
-    def is_open(self) -> bool:
-        return helpers.order_status_is_open(self.json["status"])
-
-    @property
-    def order_list_id(self) -> Optional[str]:
-        ret = self.json.get("orderListId")
-        ret = None if ret in [None, -1] else str(ret)
-        return ret
-
-    @property
-    def limit_price(self) -> Optional[Decimal]:
-        return helpers.get_optional_decimal(self.json, "price", True)
-
-    @property
-    def amount(self) -> Decimal:
-        return Decimal(self.json["origQty"])
-
-    @property
-    def amount_filled(self) -> Decimal:
-        return Decimal(self.json["executedQty"])
-
-    @property
-    def quote_amount_filled(self) -> Decimal:
-        return Decimal(self.json["cummulativeQuoteQty"])
-
-    @property
-    def status(self) -> str:
-        return self.json["status"]
-
-    @property
-    def time_in_force(self) -> Optional[str]:
-        return self.json.get("timeInForce")
-
+class CanceledOrder(OrderWrapper):
     @property
     def operation(self) -> OrderOperation:
+        """The operation."""
         return helpers.side_to_order_operation(self.json["side"])
 
     @property
     def type(self) -> str:
+        """The type of order.
+
+        Check **Order types** in https://binance-docs.github.io/apidocs/spot/en/#public-api-definitions.
+        """
         return self.json["type"]
 
 
-class OpenOrder:
-    def __init__(self, json: dict):
-        self.json = json
-
-    @property
-    def id(self) -> str:
-        return str(self.json["orderId"])
-
+class OpenOrder(OrderWrapper):
     @property
     def datetime(self) -> datetime.datetime:
+        """The creation datetime."""
         return helpers.timestamp_to_datetime(self.json["time"])
 
     @property
-    def client_order_id(self) -> str:
-        return self.json["clientOrderId"]
-
-    @property
-    def limit_price(self) -> Optional[Decimal]:
-        return helpers.get_optional_decimal(self.json, "price", True)
-
-    @property
-    def stop_price(self) -> Optional[Decimal]:
-        return helpers.get_optional_decimal(self.json, "stopPrice", True)
-
-    @property
-    def amount(self) -> Decimal:
-        return Decimal(self.json["origQty"])
-
-    @property
-    def amount_filled(self) -> Decimal:
-        return Decimal(self.json["executedQty"])
-
-    @property
-    def quote_amount_filled(self) -> Decimal:
-        return Decimal(self.json["cummulativeQuoteQty"])
-
-    @property
     def operation(self) -> OrderOperation:
+        """The operation."""
         return helpers.side_to_order_operation(self.json["side"])
 
     @property
-    def status(self) -> str:
-        return self.json["status"]
-
-    @property
-    def time_in_force(self) -> Optional[str]:
-        return self.json.get("timeInForce")
-
-    @property
     def type(self) -> str:
+        """The type of order.
+
+        Check **Order types** in https://binance-docs.github.io/apidocs/spot/en/#public-api-definitions.
+        """
         return self.json["type"]
 
 
-class CreatedOCOOrder:
+class OCOOrderWrapper:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def order_list_id(self) -> str:
+        """The order list id."""
         return str(self.json["orderListId"])
 
     @property
     def client_order_list_id(self) -> str:
+        """A client id for the order list."""
         return str(self.json["listClientOrderId"])
 
     @property
     def datetime(self) -> datetime.datetime:
+        """The creation datetime."""
         return helpers.timestamp_to_datetime(self.json["transactionTime"])
 
     @property
     def is_open(self) -> bool:
+        """True if the order is open, False otherwise."""
         return helpers.oco_order_status_is_open(self.json["listOrderStatus"])
 
     @property
     def limit_order_id(self) -> str:
+        """The id for the limit order."""
         order_ids = [
             str(order["orderId"])
             for order in self.json.get("orderReports", [])
             if order["type"] in ("LIMIT", "LIMIT_MAKER")
         ]
         return order_ids[0]
 
     @property
     def stop_loss_order_id(self) -> str:
+        """The id for the stop loss order."""
         order_ids = [
             str(order["orderId"])
             for order in self.json.get("orderReports", [])
             if order["type"] in ("STOP_LOSS", "STOP_LOSS_LIMIT")
         ]
         return order_ids[0]
 
 
-class OCOOrderInfo(CreatedOCOOrder):
+class CreatedOCOOrder(OCOOrderWrapper):
+    pass
+
+
+class OCOOrderInfo(OCOOrderWrapper):
     pass
 
 
-class CanceledOCOOrder(CreatedOCOOrder):
+class CanceledOCOOrder(OCOOrderWrapper):
     pass
```

### Comparing `basana-1.2.2/basana/external/binance/config.py` & `basana-1.3.0/basana/external/binance/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/cross_margin.py` & `basana-1.3.0/basana/external/binance/cross_margin.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,23 +17,39 @@
 from decimal import Decimal
 from typing import Dict
 
 from . import client, margin
 
 
 class Account(margin.Account):
+    """Cross margin account."""
     def __init__(self, cli: client.CrossMarginAccount):
         self._cli = cli
 
     @property
     def client(self) -> client.CrossMarginAccount:
         return self._cli
 
     async def get_balances(self) -> Dict[str, margin.Balance]:
+        """Returns all balances."""
         account_info = await self.client.get_account_information()
         return {balance["asset"].upper(): margin.Balance(balance) for balance in account_info["userAssets"]}
 
     async def transfer_from_spot_account(self, asset: str, amount: Decimal) -> dict:
+        """Transfer balances from the spot account to the cross margin account.
+
+        If the transfer can't be completed a :class:`basana.external.binance.exchange.Error` will be raised.
+
+        :param asset: The asset to transfer.
+        :param amount: The amount to transfer.
+        """
         return await self.client.transfer_from_spot_account(asset, amount)
 
     async def transfer_to_spot_account(self, asset: str, amount: Decimal) -> dict:
+        """Transfer balances from the cross margin account to the spot account.
+
+        If the transfer can't be completed a :class:`basana.external.binance.exchange.Error` will be raised.
+
+        :param asset: The asset to transfer.
+        :param amount: The amount to transfer.
+        """
         return await self.client.transfer_to_spot_account(asset, amount)
```

### Comparing `basana-1.2.2/basana/external/binance/csv/__init__.py` & `basana-1.3.0/basana/external/binance/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/csv/bars.py` & `basana-1.3.0/basana/external/binance/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/helpers.py` & `basana-1.3.0/basana/external/binance/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/isolated_margin.py` & `basana-1.3.0/basana/external/binance/isolated_margin.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,44 +23,66 @@
 
 class IsolatedBalance:
     def __init__(self, json: dict):
         self.json = json
 
     @property
     def base_asset(self) -> str:
+        """The base asset."""
         return self.json["baseAsset"]["asset"]
 
     @property
     def base_asset_balance(self) -> margin.Balance:
+        """The base asset balance."""
         return margin.Balance(self.json["baseAsset"])
 
     @property
     def quote_asset(self) -> str:
+        """The quote asset."""
         return self.json["quoteAsset"]["asset"]
 
     @property
     def quote_asset_balance(self) -> margin.Balance:
+        """The quote asset balance."""
         return margin.Balance(self.json["quoteAsset"])
 
 
 class Account(margin.Account):
+    """Isolated margin account."""
     def __init__(self, cli: client.IsolatedMarginAccount):
         self._cli = cli
 
     @property
     def client(self) -> client.IsolatedMarginAccount:
         return self._cli
 
     async def get_balances(self) -> Dict[Pair, IsolatedBalance]:
+        """Returns all balances."""
         account_info = await self.client.get_account_information()
         ret = {}
         for isolated_balance in account_info["assets"]:
             isolated_balance = IsolatedBalance(isolated_balance)
             pair = Pair(isolated_balance.base_asset, isolated_balance.quote_asset)
             ret[pair] = isolated_balance
         return ret
 
     async def transfer_from_spot_account(self, asset: str, pair: Pair, amount: Decimal) -> dict:
+        """Transfer balances from the spot account to the isolated margin account.
+
+        If the transfer can't be completed a :class:`basana.external.binance.exchange.Error` will be raised.
+
+        :param asset: The asset to transfer.
+        :param pair: The trading pair.
+        :param amount: The amount to transfer.
+        """
         return await self.client.transfer_from_spot_account(asset, helpers.pair_to_order_book_symbol(pair), amount)
 
     async def transfer_to_spot_account(self, asset: str, pair: Pair, amount: Decimal) -> dict:
+        """Transfer balances from the isolated margin account to the spot account.
+
+        If the transfer can't be completed a :class:`basana.external.binance.exchange.Error` will be raised.
+
+        :param asset: The asset to transfer.
+        :param pair: The trading pair.
+        :param amount: The amount to transfer.
+        """
         return await self.client.transfer_to_spot_account(asset, helpers.pair_to_order_book_symbol(pair), amount)
```

### Comparing `basana-1.2.2/basana/external/binance/margin.py` & `basana-1.3.0/basana/external/binance/margin_requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,162 +11,119 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from decimal import Decimal
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 import abc
 
-from . import client, common, helpers, margin_requests
+from . import helpers
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
 
 
-CanceledOCOOrder = common.CanceledOCOOrder
-CanceledOrder = common.CanceledOrder
-OpenOrder = common.OpenOrder
-CreatedOCOOrder = common.CreatedOCOOrder
-Fill = common.Fill
-OCOOrderInfo = common.OCOOrderInfo
-OrderInfo = common.OrderInfo
-
-
-class Balance(common.Balance):
-    @property
-    def borrowed(self) -> Decimal:
-        return Decimal(self.json["borrowed"])
-
-
-class Trade(common.Trade):
-    @property
-    def is_isolated(self) -> bool:
-        return self.json["isIsolated"]
-
-
-class CreatedOrder(common.CreatedOrder):
-    @property
-    def fills(self) -> List[Fill]:
-        # Only available for FULL responses.
-        return [Fill(fill) for fill in self.json.get("fills", [])]
-
+class ExchangeOrder(metaclass=abc.ABCMeta):
+    def __init__(
+            self, operation: OrderOperation, pair: Pair, amount: Optional[Decimal],
+            client_order_id: Optional[str] = None, **kwargs: Dict[str, Any]
+    ):
+        self._operation = operation
+        self._pair = pair
+        self._amount = amount
+        self._client_order_id = client_order_id
+        self._kwargs = kwargs
 
-class Account(metaclass=abc.ABCMeta):
-    @property
     @abc.abstractmethod
-    def client(self) -> client.MarginAccount:  # pragma: no cover
+    async def create_order(self, margin_account_cli) -> dict:
         raise NotImplementedError()
 
-    async def create_order(self, order_request: margin_requests.ExchangeOrder) -> CreatedOrder:
-        created_order = await order_request.create_order(self.client)
-        return CreatedOrder(created_order)
 
-    async def create_market_order(
+class MarketOrder(ExchangeOrder):
+    def __init__(
             self, operation: OrderOperation, pair: Pair, amount: Optional[Decimal] = None,
             quote_amount: Optional[Decimal] = None, client_order_id: Optional[str] = None,
             side_effect_type: str = "NO_SIDE_EFFECT", **kwargs: Dict[str, Any]
-    ) -> CreatedOrder:
-        return await self.create_order(margin_requests.MarketOrder(
-            operation, pair, amount=amount, quote_amount=quote_amount, client_order_id=client_order_id,
-            side_effect_type=side_effect_type, **kwargs
-        ))
+    ):
+        assert (amount is not None) ^ (quote_amount is not None), "Either amount or quote_amount should be set"
+        super().__init__(operation, pair, amount, client_order_id=client_order_id, **kwargs)
+        self._quote_amount = quote_amount
+        self._side_effect_type = side_effect_type
+
+    async def create_order(self, margin_account_cli) -> dict:
+        return await margin_account_cli.create_order(
+            helpers.pair_to_order_book_symbol(self._pair), helpers.order_operation_to_side(self._operation), "MARKET",
+            quantity=self._amount, quote_order_qty=self._quote_amount, new_client_order_id=self._client_order_id,
+            side_effect_type=self._side_effect_type, **self._kwargs
+        )
 
-    async def create_limit_order(
+
+class LimitOrder(ExchangeOrder):
+    def __init__(
             self, operation: OrderOperation, pair: Pair, amount: Decimal, limit_price: Decimal,
             side_effect_type: str = "NO_SIDE_EFFECT", time_in_force: str = "GTC", client_order_id: Optional[str] = None,
             **kwargs: Dict[str, Any]
-    ) -> CreatedOrder:
-        return await self.create_order(margin_requests.LimitOrder(
-            operation, pair, amount, limit_price, side_effect_type=side_effect_type, time_in_force=time_in_force,
-            client_order_id=client_order_id, **kwargs
-        ))
+    ):
+        super().__init__(operation, pair, amount, client_order_id=client_order_id, **kwargs)
+        self._limit_price = limit_price
+        self._time_in_force = time_in_force
+        self._side_effect_type = side_effect_type
+
+    async def create_order(self, margin_account_cli) -> dict:
+        return await margin_account_cli.create_order(
+            helpers.pair_to_order_book_symbol(self._pair), helpers.order_operation_to_side(self._operation), "LIMIT",
+            quantity=self._amount, price=self._limit_price, time_in_force=self._time_in_force,
+            new_client_order_id=self._client_order_id, side_effect_type=self._side_effect_type, **self._kwargs
+        )
+
 
-    async def create_stop_limit_order(
+class StopLimitOrder(ExchangeOrder):
+    def __init__(
             self, operation: OrderOperation, pair: Pair, amount: Decimal, stop_price: Decimal, limit_price: Decimal,
             side_effect_type: str = "NO_SIDE_EFFECT", time_in_force: str = "GTC",
             client_order_id: Optional[str] = None, **kwargs: Dict[str, Any]
-    ) -> CreatedOrder:
-        return await self.create_order(margin_requests.StopLimitOrder(
-            operation, pair, amount, stop_price, limit_price, side_effect_type=side_effect_type,
-            time_in_force=time_in_force, client_order_id=client_order_id, **kwargs
-        ))
-
-    async def get_order_info(
-            self, pair: Pair, order_id: Optional[str] = None, client_order_id: Optional[str] = None,
-            include_trades: bool = True
-    ) -> OrderInfo:
-        """Request order information.
-
-        @param pair: That trading pair.
-        @param order_id: The order id.
-        @param client_order_id: The client order id.
-        @return: Order information.
-
-        .. note::
-            * This requires making 2 requests to Binance.
-            * Either order_id or client_order_id have to be set.
-        """
-        order_book_symbol = helpers.pair_to_order_book_symbol(pair)
-        order_info = await self.client.query_order(
-            order_book_symbol, order_id=None if order_id is None else int(order_id),
-            orig_client_order_id=client_order_id
+    ):
+        super().__init__(operation, pair, amount, client_order_id=client_order_id, **kwargs)
+        self._stop_price = stop_price
+        self._limit_price = limit_price
+        self._time_in_force = time_in_force
+        self._side_effect_type = side_effect_type
+
+    async def create_order(self, margin_account_cli) -> dict:
+        return await margin_account_cli.create_order(
+            helpers.pair_to_order_book_symbol(self._pair), helpers.order_operation_to_side(self._operation),
+            "STOP_LOSS_LIMIT", quantity=self._amount, stop_price=self._stop_price, price=self._limit_price,
+            time_in_force=self._time_in_force, new_client_order_id=self._client_order_id,
+            side_effect_type=self._side_effect_type, **self._kwargs
         )
-        trades = []
-        if include_trades:
-            trades = [
-                Trade(trade) for trade in
-                await self.client.get_trades(order_book_symbol, order_id=order_info["orderId"])
-            ]
-        return OrderInfo(order_info, trades)
-
-    async def get_open_orders(self, pair: Optional[Pair] = None) -> List[OpenOrder]:
-        order_book_symbol = None
-        if pair:
-            order_book_symbol = helpers.pair_to_order_book_symbol(pair)
-        return [
-            OpenOrder(open_order) for open_order in await self.client.get_open_orders(order_book_symbol)
-        ]
-
-    async def cancel_order(
-            self, pair: Pair, order_id: Optional[str] = None, client_order_id: Optional[str] = None,
-    ) -> CanceledOrder:
-        canceled_order = await self.client.cancel_order(
-            helpers.pair_to_order_book_symbol(pair), order_id=None if order_id is None else int(order_id),
-            orig_client_order_id=client_order_id
-        )
-        return CanceledOrder(canceled_order)
 
-    async def create_oco_order(
+
+class OCOOrder:
+    def __init__(
             self, operation: OrderOperation, pair: Pair, amount: Decimal, limit_price: Decimal, stop_price: Decimal,
             stop_limit_price: Optional[Decimal] = None, side_effect_type: str = "NO_SIDE_EFFECT",
             stop_limit_time_in_force: str = "GTC", list_client_order_id: Optional[str] = None,
             limit_client_order_id: Optional[str] = None, stop_client_order_id: Optional[str] = None,
             **kwargs: Dict[str, Any]
-    ) -> CreatedOCOOrder:
-        order_req = margin_requests.OCOOrder(
-            operation, pair, amount, limit_price, stop_price, stop_limit_price=stop_limit_price,
-            side_effect_type=side_effect_type, stop_limit_time_in_force=stop_limit_time_in_force,
-            list_client_order_id=list_client_order_id, limit_client_order_id=limit_client_order_id,
-            stop_client_order_id=stop_client_order_id, **kwargs
-        )
-        created_order = await order_req.create_order(self.client)
-        return CreatedOCOOrder(created_order)
-
-    async def get_oco_order_info(
-            self, order_list_id: Optional[str] = None, client_order_list_id: Optional[str] = None,
-    ) -> OCOOrderInfo:
-        order_info = await self.client.query_oco_order(
-            order_list_id=None if order_list_id is None else int(order_list_id),
-            client_order_list_id=client_order_list_id
-        )
-        return OCOOrderInfo(order_info)
-
-    async def cancel_oco_order(
-            self, pair: Pair, order_list_id: Optional[str] = None, client_order_list_id: Optional[str] = None,
-    ) -> CanceledOCOOrder:
-        canceled_order = await self.client.cancel_oco_order(
-            helpers.pair_to_order_book_symbol(pair),
-            order_list_id=None if order_list_id is None else int(order_list_id),
-            client_order_list_id=client_order_list_id
+    ):
+        self._operation = operation
+        self._pair = pair
+        self._amount = amount
+        self._limit_price = limit_price
+        self._stop_price = stop_price
+        self._stop_limit_price = stop_limit_price
+        self._stop_limit_time_in_force = None if stop_limit_price is None else stop_limit_time_in_force
+        self._list_client_order_id = list_client_order_id
+        self._side_effect_type = side_effect_type
+        self._limit_client_order_id = limit_client_order_id
+        self._stop_client_order_id = stop_client_order_id
+        self._kwargs = kwargs
+
+    async def create_order(self, margin_account_cli) -> dict:
+        return await margin_account_cli.create_oco(
+            helpers.pair_to_order_book_symbol(self._pair), helpers.order_operation_to_side(self._operation),
+            self._amount, self._limit_price, self._stop_price, stop_limit_price=self._stop_limit_price,
+            stop_limit_time_in_force=self._stop_limit_time_in_force, list_client_order_id=self._list_client_order_id,
+            side_effect_type=self._side_effect_type, limit_client_order_id=self._limit_client_order_id,
+            stop_client_order_id=self._stop_client_order_id, **self._kwargs
         )
-        return CanceledOCOOrder(canceled_order)
```

### Comparing `basana-1.2.2/basana/external/binance/order_book.py` & `basana-1.3.0/basana/external/binance/order_book.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,54 +14,69 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from decimal import Decimal
 from typing import Any, List, Optional
 import asyncio
+import datetime
 import logging
 
 import aiohttp
 
 from . import client, helpers
 from basana.core import dt, event, logs, token_bucket, websockets as core_ws
 from basana.core.pair import Pair
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Entry:
+    #: The price.
     price: Decimal
+
+    #: The volume.
     volume: Decimal
 
 
 class OrderBook:
+    """An order book."""
     def __init__(self, pair: Pair, json: dict):
-        self.pair = pair
-        self.json = json
+        #: The trading pair.
+        self.pair: Pair = pair
+        #: The JSON representation.
+        self.json: dict = json
 
     @property
     def bids(self) -> List[Entry]:
+        """Returns the top bid entries."""
         return [
             Entry(price=Decimal(entry[0]), volume=Decimal(entry[1])) for entry in self.json["bids"]
         ]
 
     @property
     def asks(self) -> List[Entry]:
+        """Returns the top ask entries."""
         return [
             Entry(price=Decimal(entry[0]), volume=Decimal(entry[1])) for entry in self.json["asks"]
         ]
 
 
 class OrderBookEvent(event.Event):
-    def __init__(self, order_book: OrderBook):
-        super().__init__(dt.utc_now())
-        self.order_book = order_book
+    """An event for order book updates.
+
+    :param when: The datetime when the event occurred. It must have timezone information set.
+    :param order_book: The updated order book.
+    """
+    def __init__(self, when: datetime.datetime, order_book: OrderBook):
+        super().__init__(when)
+        #: The order book.
+        self.order_book: OrderBook = order_book
 
 
 class PollOrderBook(event.FifoQueueEventSource, event.Producer):
     def __init__(
             self, pair: Pair, interval: float, limit: Optional[int] = None,
             session: Optional[aiohttp.ClientSession] = None, tb: Optional[token_bucket.TokenBucketLimiter] = None,
             config_overrides: dict = {}
@@ -72,15 +87,18 @@
         self.pair = pair
         self._interval = interval
         self._limit = limit
         self._client = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
 
     async def _fetch_and_push(self, order_book_symbol: str):
         order_book_json = await self._client.get_order_book(order_book_symbol, limit=self._limit)
-        self.push(OrderBookEvent(OrderBook(self.pair, order_book_json)))
+        self.push(OrderBookEvent(
+            dt.utc_now(),
+            OrderBook(self.pair, order_book_json)
+        ))
 
     async def on_error(self, error: Any):
         logger.error(logs.StructuredMessage("Error polling order book", channel=self.pair, error=error))
 
     async def main(self):
         order_book_symbol = helpers.pair_to_order_book_symbol(self.pair)
         while True:
@@ -94,13 +112,17 @@
 # Generate OrderBookEvent events from websocket messages.
 class WebSocketEventSource(core_ws.ChannelEventSource):
     def __init__(self, pair: Pair, producer: event.Producer):
         super().__init__(producer=producer)
         self._pair = pair
 
     async def push_from_message(self, message: dict):
-        self.push(OrderBookEvent(OrderBook(self._pair, message["data"])))
+        event = message["data"]
+        self.push(OrderBookEvent(
+            dt.utc_now(),  # The event doesn't include a timestamp.
+            OrderBook(self._pair, event)
+        ))
 
 
 def get_channel(pair: Pair, depth: int) -> str:
     assert depth in [5, 10, 20], "Invalid depth"
     return "{}@depth{}".format(helpers.pair_to_order_book_symbol(pair).lower(), depth)
```

### Comparing `basana-1.2.2/basana/external/binance/spot_requests.py` & `basana-1.3.0/basana/external/binance/spot_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self._operation = operation
         self._pair = pair
         self._amount = amount
         self._client_order_id = client_order_id
         self._kwargs = kwargs
 
     @abc.abstractmethod
-    async def create_order(self, spot_account_cli) -> dict:  # pragma: no cover
+    async def create_order(self, spot_account_cli) -> dict:
         raise NotImplementedError()
 
 
 class MarketOrder(ExchangeOrder):
     def __init__(
             self, operation: OrderOperation, pair: Pair, amount: Optional[Decimal] = None,
             quote_amount: Optional[Decimal] = None, client_order_id: Optional[str] = None, **kwargs: Dict[str, Any]
```

### Comparing `basana-1.2.2/basana/external/binance/tools/__init__.py` & `basana-1.3.0/basana/external/binance/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/tools/download_bars.py` & `basana-1.3.0/basana/external/binance/tools/download_bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/binance/trades.py` & `basana-1.3.0/basana/external/binance/trades.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,65 +15,83 @@
 # limitations under the License.
 
 from decimal import Decimal
 import datetime
 import logging
 
 from . import helpers
-from basana.core import dt, event, websockets as core_ws
+from basana.core import event, websockets as core_ws
 from basana.core.pair import Pair
 
 
 logger = logging.getLogger(__name__)
 
 
 class Trade:
     def __init__(self, pair: Pair, json: dict):
         assert json["e"] == "trade"
 
-        self.pair = pair
-        self.json = json
+        #: The trading pair.
+        self.pair: Pair = pair
+        #: The JSON representation.
+        self.json: dict = json
 
     @property
     def id(self) -> str:
+        """The trade id."""
         return str(self.json["t"])
 
     @property
     def datetime(self) -> datetime.datetime:
-        timestamp = self.json["T"] / 1e3
-        return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
+        """The trade datetime."""
+        return helpers.timestamp_to_datetime(int(self.json["T"]))
 
     @property
     def price(self) -> Decimal:
+        """The price."""
         return Decimal(self.json["p"])
 
     @property
     def amount(self) -> Decimal:
+        """The amount."""
         return Decimal(self.json["q"])
 
     @property
     def buy_order_id(self) -> str:
+        """The buyer order id."""
         return str(self.json["b"])
 
     @property
     def sell_order_id(self) -> str:
+        """The seller order id."""
         return str(self.json["a"])
 
 
 class TradeEvent(event.Event):
-    def __init__(self, trade: Trade):
-        super().__init__(dt.utc_now())
-        self.trade = trade
+    """An event for new trades.
+
+    :param when: The datetime when the event occurred. It must have timezone information set.
+    :param trade: The trade.
+    """
+
+    def __init__(self, when: datetime.datetime, trade: Trade):
+        super().__init__(when)
+        #: The trade.
+        self.trade: Trade = trade
 
 
 # Generate TradeEvent events from websocket messages.
 class WebSocketEventSource(core_ws.ChannelEventSource):
     def __init__(self, pair: Pair, producer: event.Producer):
         super().__init__(producer=producer)
-        self._pair = pair
+        self._pair: Pair = pair
 
     async def push_from_message(self, message: dict):
-        self.push(TradeEvent(Trade(self._pair, message["data"])))
+        event = message["data"]
+        self.push(TradeEvent(
+            helpers.timestamp_to_datetime(int(event["E"])),
+            Trade(self._pair, event)
+        ))
 
 
 def get_channel(pair: Pair) -> str:
     return "{}@trade".format(helpers.pair_to_order_book_symbol(pair).lower())
```

### Comparing `basana-1.2.2/basana/external/binance/websockets.py` & `basana-1.3.0/basana/external/binance/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/__init__.py` & `basana-1.3.0/basana/external/bitstamp/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/client.py` & `basana-1.3.0/basana/external/bitstamp/client.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/config.py` & `basana-1.3.0/basana/external/bitstamp/config.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/csv/__init__.py` & `basana-1.3.0/basana/external/bitstamp/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/csv/bars.py` & `basana-1.3.0/basana/external/bitstamp/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/helpers.py` & `basana-1.3.0/basana/external/bitstamp/helpers.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/order_book.py` & `basana-1.3.0/basana/external/bitstamp/order_book.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,74 +20,87 @@
 import asyncio
 import datetime
 import logging
 
 import aiohttp
 
 from . import client, helpers
-from basana.core import dt, event, logs, pair, token_bucket, websockets as core_ws
+from basana.core import dt, event, logs, token_bucket, websockets as core_ws
 from basana.core.pair import Pair
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Entry:
+    #: The price.
     price: Decimal
+    #: The volume.
     volume: Decimal
 
 
 # https://www.bitstamp.net/api/#order-book
 class OrderBook:
-    def __init__(self, pair: pair.Pair, json: dict):
-        self.pair = pair
-        self.json = json
+    def __init__(self, pair: Pair, json: dict):
+        #: The trading pair.
+        self.pair: Pair = pair
+        #: The JSON representation.
+        self.json: dict = json
 
     @property
     def datetime(self) -> datetime.datetime:
         timestamp = int(self.json["microtimestamp"]) / 1e6
         return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
 
     @property
     def bids(self) -> List[Entry]:
+        """Returns the top bid entries."""
         return [
             Entry(price=Decimal(entry[0]), volume=Decimal(entry[1])) for entry in self.json["bids"]
         ]
 
     @property
     def asks(self) -> List[Entry]:
+        """Returns the top ask entries."""
         return [
             Entry(price=Decimal(entry[0]), volume=Decimal(entry[1])) for entry in self.json["asks"]
         ]
 
 
 class OrderBookEvent(event.Event):
-    def __init__(self, order_book: OrderBook):
-        super().__init__(dt.utc_now())
-        self.order_book = order_book
+    """An event for order book updates.
+
+    :param when: The datetime when the event occurred. It must have timezone information set.
+    :param order_book: The updated order book.
+    """
+
+    def __init__(self, when: datetime.datetime, order_book: OrderBook):
+        super().__init__(when)
+        #: The order book.
+        self.order_book: OrderBook = order_book
 
 
 class PollOrderBook(event.FifoQueueEventSource, event.Producer):
     def __init__(
-            self, pair: pair.Pair, interval: float, group: Optional[int] = None,
+            self, pair: Pair, interval: float, group: Optional[int] = None,
             session: Optional[aiohttp.ClientSession] = None, tb: Optional[token_bucket.TokenBucketLimiter] = None,
             config_overrides: dict = {}
     ):
         assert interval > 0, "Invalid interval"
 
         super().__init__(producer=self)
         self.pair = pair
         self._interval = interval
         self._group = group
         self._client = client.APIClient(session=session, tb=tb, config_overrides=config_overrides)
 
     async def _fetch_and_push(self, currency_pair: str):
         order_book_json = await self._client.get_order_book(currency_pair, group=self._group)
-        self.push(OrderBookEvent(OrderBook(self.pair, order_book_json)))
+        self.push(OrderBookEvent(dt.utc_now(), OrderBook(self.pair, order_book_json)))
 
     async def main(self):
         currency_pair = helpers.pair_to_currency_pair(self.pair)
         while True:
             try:
                 await self._fetch_and_push(currency_pair)
             except Exception as e:
@@ -101,12 +114,12 @@
 # Generate OrderBookEvent events from websocket messages.
 class WebSocketEventSource(core_ws.ChannelEventSource):
     def __init__(self, pair: Pair, producer: event.Producer):
         super().__init__(producer=producer)
         self._pair = pair
 
     async def push_from_message(self, message: dict):
-        self.push(OrderBookEvent(OrderBook(self._pair, message["data"])))
+        self.push(OrderBookEvent(dt.utc_now(), OrderBook(self._pair, message["data"])))
 
 
 def get_channel(pair: Pair) -> str:
     return "order_book_{}".format(helpers.pair_to_currency_pair(pair))
```

### Comparing `basana-1.2.2/basana/external/bitstamp/orders.py` & `basana-1.3.0/basana/external/bitstamp/trades.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,57 +19,79 @@
 
 from . import helpers
 from basana.core import dt, event, websockets as core_ws
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
 
 
-class Order:
+class Trade:
     def __init__(self, pair: Pair, json: dict):
-        self.pair = pair
-        self.json = json
+        #: The trading pair.
+        self.pair: Pair = pair
+        #: The JSON representation.
+        self.json: dict = json
 
     @property
     def id(self) -> str:
+        """The trade id."""
         return str(self.json["id"])
 
     @property
     def datetime(self) -> datetime.datetime:
+        """The datetime when the trade occurred."""
         timestamp = int(self.json["microtimestamp"]) / 1e6
         return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
 
     @property
     def amount(self) -> Decimal:
+        """The amount."""
         return Decimal(self.json["amount_str"])
 
     @property
     def price(self) -> Decimal:
+        """The price."""
         return Decimal(self.json["price_str"])
 
     @property
     def type(self) -> OrderOperation:
-        return helpers.order_type_to_order_operation(int(self.json["order_type"]))
+        # TODO: Deprecate this property.
+        return self.operation
+
+    @property
+    def operation(self) -> OrderOperation:
+        """The operation."""
+        return helpers.order_type_to_order_operation(int(self.json["type"]))
+
+    @property
+    def buy_order_id(self) -> str:
+        """The buy order id."""
+        return str(self.json["buy_order_id"])
+
+    @property
+    def sell_order_id(self) -> str:
+        """The sell order id."""
+        return str(self.json["sell_order_id"])
 
 
-class OrderEvent(event.Event):
-    def __init__(self, type: str, order: Order):
-        super().__init__(dt.utc_now())
-        self.type = type
-        self.order = order
+class TradeEvent(event.Event):
+    def __init__(self, when: datetime.datetime, trade: Trade):
+        super().__init__(when)
+        #: The trade.
+        self.trade: Trade = trade
 
 
-# Generate Order events from websocket messages.
+# Generate Trade events from websocket messages.
 class WebSocketEventSource(core_ws.ChannelEventSource):
     def __init__(self, pair: Pair, producer: event.Producer):
         super().__init__(producer=producer)
-        self._pair = pair
+        self._pair: Pair = pair
 
     async def push_from_message(self, message: dict):
-        self.push(OrderEvent(message["event"], Order(self._pair, message["data"])))
+        self.push(TradeEvent(dt.utc_now(), Trade(self._pair, message["data"])))
 
 
 def get_public_channel(pair: Pair) -> str:
-    return "live_orders_{}".format(helpers.pair_to_currency_pair(pair))
+    return "live_trades_{}".format(helpers.pair_to_currency_pair(pair))
 
 
 def get_private_channel(pair: Pair) -> str:
-    return "private-my_orders_{}".format(helpers.pair_to_currency_pair(pair))
+    return "private-my_trades_{}".format(helpers.pair_to_currency_pair(pair))
```

### Comparing `basana-1.2.2/basana/external/bitstamp/requests.py` & `basana-1.3.0/basana/external/bitstamp/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         return self._amount
 
     @property
     def operation(self) -> OrderOperation:
         return self._operation
 
     @abc.abstractmethod
-    async def create_order(self, cli: client.APIClient) -> dict:  # pragma: no cover
+    async def create_order(self, cli: client.APIClient) -> dict:
         raise NotImplementedError()
 
 
 class MarketOrder(ExchangeOrder):
     """
     Market order request.
```

### Comparing `basana-1.2.2/basana/external/bitstamp/tools/__init__.py` & `basana-1.3.0/basana/external/bitstamp/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/tools/download_bars.py` & `basana-1.3.0/basana/external/bitstamp/tools/download_bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/bitstamp/trades.py` & `basana-1.3.0/basana/external/bitstamp/orders.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,64 +19,77 @@
 
 from . import helpers
 from basana.core import dt, event, websockets as core_ws
 from basana.core.enums import OrderOperation
 from basana.core.pair import Pair
 
 
-class Trade:
+class Order:
     def __init__(self, pair: Pair, json: dict):
-        self.pair = pair
-        self.json = json
+        #: The trading pair.
+        self.pair: Pair = pair
+        #: The JSON representation.
+        self.json: dict = json
 
     @property
     def id(self) -> str:
+        """The order id."""
         return str(self.json["id"])
 
     @property
     def datetime(self) -> datetime.datetime:
         timestamp = int(self.json["microtimestamp"]) / 1e6
         return datetime.datetime.utcfromtimestamp(timestamp).replace(tzinfo=datetime.timezone.utc)
 
     @property
     def amount(self) -> Decimal:
+        """The order amount."""
         return Decimal(self.json["amount_str"])
 
     @property
     def price(self) -> Decimal:
+        """The order price."""
         return Decimal(self.json["price_str"])
 
     @property
     def type(self) -> OrderOperation:
-        return helpers.order_type_to_order_operation(int(self.json["type"]))
+        # TODO: Deprecate this property.
+        return self.operation
 
     @property
-    def buy_order_id(self) -> str:
-        return str(self.json["buy_order_id"])
+    def operation(self) -> OrderOperation:
+        """The operation."""
+        return helpers.order_type_to_order_operation(int(self.json["order_type"]))
 
-    @property
-    def sell_order_id(self) -> str:
-        return str(self.json["sell_order_id"])
 
+class OrderEvent(event.Event):
+    """An event for order updates.
+
+    :param when: The datetime when the event occurred. It must have timezone information set.
+    :param type: The type of event. One of order_created, order_changed or order_deleted.
+    :param order: The order.
+    """
 
-class TradeEvent(event.Event):
-    def __init__(self, trade: Trade):
-        super().__init__(dt.utc_now())
-        self.trade = trade
+    def __init__(self, when: datetime.datetime, type: str, order: Order):
+        super().__init__(when)
+        #: The event type. One of order_created, order_changed or order_deleted.
+        self.type: str = type
+        #: The order.
+        self.order: Order = order
 
 
-# Generate Trade events from websocket messages.
+# Generate Order events from websocket messages.
 class WebSocketEventSource(core_ws.ChannelEventSource):
     def __init__(self, pair: Pair, producer: event.Producer):
         super().__init__(producer=producer)
         self._pair = pair
 
     async def push_from_message(self, message: dict):
-        self.push(TradeEvent(Trade(self._pair, message["data"])))
+        self.push(OrderEvent(dt.utc_now(), message["event"], Order(self._pair, message["data"])))
 
 
 def get_public_channel(pair: Pair) -> str:
-    return "live_trades_{}".format(helpers.pair_to_currency_pair(pair))
+    return "live_orders_{}".format(helpers.pair_to_currency_pair(pair))
 
 
 def get_private_channel(pair: Pair) -> str:
-    return "private-my_trades_{}".format(helpers.pair_to_currency_pair(pair))
+    return "private-my_orders_{}".format(helpers.pair_to_currency_pair(pair))
```

### Comparing `basana-1.2.2/basana/external/bitstamp/websockets.py` & `basana-1.3.0/basana/external/bitstamp/websockets.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/common/__init__.py` & `basana-1.3.0/basana/external/common/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/common/csv/__init__.py` & `basana-1.3.0/basana/external/common/csv/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/common/csv/bars.py` & `basana-1.3.0/basana/external/common/csv/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/yahoo/__init__.py` & `basana-1.3.0/basana/external/yahoo/__init__.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/basana/external/yahoo/bars.py` & `basana-1.3.0/basana/external/yahoo/bars.py`

 * *Files identical despite different names*

### Comparing `basana-1.2.2/setup.py` & `basana-1.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,25 +19,29 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp[speedups]>=3.8.4,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
+extras_require = \
+{'charts': ['plotly>=5.14.1,<6.0.0', 'kaleido==0.2.1']}
+
 setup_kwargs = {
     'name': 'basana',
-    'version': '1.2.2',
+    'version': '1.3.0',
     'description': 'A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.',
     'long_description': 'None',
     'author': 'Gabriel Becedillas',
     'author_email': 'gabriel.becedillas@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gbeced/basana',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `basana-1.2.2/PKG-INFO` & `basana-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: basana
-Version: 1.2.2
+Version: 1.3.0
 Summary: A Python async and event driven framework for algorithmic trading, with a focus on crypto currencies.
 Home-page: https://github.com/gbeced/basana
 License: Apache-2.0
 Author: Gabriel Becedillas
 Author-email: gabriel.becedillas@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: charts
 Requires-Dist: aiohttp[speedups] (>=3.8.4,<4.0.0)
+Requires-Dist: kaleido (==0.2.1) ; extra == "charts"
+Requires-Dist: plotly (>=5.14.1,<6.0.0) ; extra == "charts"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Documentation, https://basana.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/gbeced/basana
```

