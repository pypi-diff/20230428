# Comparing `tmp/csvthd-0.4.0b0.tar.gz` & `tmp/csvthd-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvthd-0.4.0b0.tar", max compression
+gzip compressed data, was "csvthd-0.5.0b0.tar", max compression
```

## Comparing `csvthd-0.4.0b0.tar` & `csvthd-0.5.0b0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     4515 2023-04-26 04:46:52.053337 csvthd-0.4.0b0/README.md
--rw-r--r--   0        0        0        0 2023-04-23 14:03:39.147538 csvthd-0.4.0b0/csvthd/__init__.py
--rw-r--r--   0        0        0       59 2023-04-24 05:21:37.075961 csvthd-0.4.0b0/csvthd/__main__.py
--rw-r--r--   0        0        0      114 2023-04-26 05:28:34.442698 csvthd-0.4.0b0/csvthd/__version__.py
--rw-r--r--   0        0        0     3495 2023-04-26 05:02:47.807005 csvthd-0.4.0b0/csvthd/cli.py
--rw-r--r--   0        0        0      623 2023-04-25 14:26:47.536086 csvthd-0.4.0b0/csvthd/commandline.py
--rw-r--r--   0        0        0      683 2023-04-25 14:29:47.324668 csvthd-0.4.0b0/csvthd/config.py
--rw-r--r--   0        0        0     2904 2023-04-26 04:32:58.115627 csvthd-0.4.0b0/csvthd/filters.py
--rw-r--r--   0        0        0      959 2023-04-26 05:03:30.975285 csvthd-0.4.0b0/csvthd/reducers.py
--rw-r--r--   0        0        0     1709 2023-04-26 05:03:13.125557 csvthd-0.4.0b0/csvthd/transactions.py
--rw-r--r--   0        0        0     1046 2023-04-26 05:28:28.798642 csvthd-0.4.0b0/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 csvthd-0.4.0b0/PKG-INFO
+-rw-r--r--   0        0        0     6001 2023-04-28 08:39:38.362620 csvthd-0.5.0b0/README.md
+-rw-r--r--   0        0        0        0 2023-04-23 14:03:39.147538 csvthd-0.5.0b0/csvthd/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-24 05:21:37.075961 csvthd-0.5.0b0/csvthd/__main__.py
+-rw-r--r--   0        0        0      114 2023-04-28 12:35:05.335500 csvthd-0.5.0b0/csvthd/__version__.py
+-rw-r--r--   0        0        0     4254 2023-04-28 12:19:28.691985 csvthd-0.5.0b0/csvthd/cli.py
+-rw-r--r--   0        0        0      623 2023-04-28 09:47:12.927840 csvthd-0.5.0b0/csvthd/commandline.py
+-rw-r--r--   0        0        0     1440 2023-04-28 07:31:31.665120 csvthd-0.5.0b0/csvthd/config.py
+-rw-r--r--   0        0        0      305 2023-04-28 08:57:51.062618 csvthd-0.5.0b0/csvthd/exceptions.py
+-rw-r--r--   0        0        0     3906 2023-04-28 04:48:33.543968 csvthd-0.5.0b0/csvthd/filters.py
+-rw-r--r--   0        0        0      959 2023-04-28 12:25:44.293900 csvthd-0.5.0b0/csvthd/reducers.py
+-rw-r--r--   0        0        0     2103 2023-04-28 08:53:09.283365 csvthd-0.5.0b0/csvthd/transactions.py
+-rw-r--r--   0        0        0     1046 2023-04-28 12:34:52.206250 csvthd-0.5.0b0/pyproject.toml
+-rw-r--r--   0        0        0     6926 1970-01-01 00:00:00.000000 csvthd-0.5.0b0/PKG-INFO
```

### Comparing `csvthd-0.4.0b0/README.md` & `csvthd-0.5.0b0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,18 @@
+[![pipeline status](https://gitlab.com/DrTexx/csv-transaction-history-detective/badges/main/pipeline.svg)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/commits/main)
+[![coverage report](https://gitlab.com/DrTexx/csv-transaction-history-detective/badges/main/coverage.svg)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/commits/main)
+[![GitLab issues](https://img.shields.io/gitlab/issues/open/drtexx/csv-transaction-history-detective?logo=gitlab)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/issues)
+[![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open/drtexx/csv-transaction-history-detective?logo=gitlab)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/merge_requests)
+
 # CSV Transaction History Detective
 
+[![PyPI Release](https://img.shields.io/pypi/v/csvthd?logo=python)](https://pypi.org/project/csvthd)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/csvthd?logo=Python)](https://pypi.org/project/csvthd)
+[![PyPI - License](https://img.shields.io/pypi/l/csvthd?color=orange&logo=Python)](https://pypi.org/project/csvthd)
+
 ## Getting started
 
 <!-- TODO: add an example `config.json` file called `config.json.example.json` -->
 
 <!-- TODO: add an example csv file to give more context to why `config.json.example.md` is laid out how it is -->
 
 <!-- TODO: mention in `config.json.template.md` to look at `config.json.example.md` for an example config. -->
@@ -83,14 +92,34 @@
 # only show transactions between $20.00 to $30.00
 csvthd -a over 20 -a under 30
 
 # only show transactions of exactly $25.00
 csvthd -a equal 25
 ```
 
+#### Date
+
+`-d/--date`
+
+Only show transactions before/after/on a given date.
+
+```bash
+# only show transactions after 1 Jan 2022
+csvthd -d after 01/01/2022
+
+# only show transactions before 21 Feb 2022
+csvthd -d before 21/02/2022
+
+# only show transactions on 10 Apr 2022
+csvthd -d on 10/04/2022
+
+# only show transactions from 1 Jan 2022 - 1 Feb 2022
+csvthd -d after 01/01/2022 -d before 01/02/2022
+```
+
 #### Type
 
 `-t/--transaction-type`
 
 Only show transactions where money is sent/received
 
 ```bash
```

### Comparing `csvthd-0.4.0b0/csvthd/cli.py` & `csvthd-0.5.0b0/csvthd/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # built in
 from datetime import datetime
 from functools import reduce
+import os
 
 # site
 import click
 
 # package
 from .filters import (
     details_include_filter,
     details_exclude_filter,
     amount_is_filter,
+    date_filter,
     transaction_type_filter,
     account_name_filter,
 )
-from .commandline import print_transaction, style_amount
+from .commandline import print_transaction, style_amount, RED, ANSI_RESET
 from .transactions import get_transactions
 from .config import load_config
 from .reducers import sum_transaction_amount
+from .exceptions import EmptyTransactionFile
 
 # TODO: consider looking into (odx?) other formats because someone mentioned apparently there
 # ... are some other commons ones that are standardized.
 
+DEFAULT_CONFIG_FILEPATH = "./config.json"
+
 
 @click.command()
 @click.option(
     "-i",
     "--include",
     multiple=True,
     help="Only show transactions that contain the given substring in their details.",
@@ -39,14 +44,21 @@
     "-a",
     "--amount",
     multiple=True,
     nargs=2,
     help="Only show transactions with amounts under/over/equal to value.",
 )
 @click.option(
+    "-d",
+    "--date",
+    multiple=True,
+    nargs=2,
+    help="Only show transactions before/after/on given date",
+)
+@click.option(
     "-t",
     "--transaction-type",
     type=click.Choice(["out", "in"]),
     help="Only show transactions where money is sent/received.",
 )
 @click.option(
     "-A",
@@ -69,41 +81,57 @@
     is_flag=True,
     help="Give a sum of all transaction amounts after filtering.",
 )
 def cli(
     include,
     exclude,
     amount,
+    date,
     transaction_type,
     account_name,
     sort_by,
     reverse_sort,
     sum,
 ):
+    # set config filepath based on env var if defined, otherwise use default
+    config_filepath = os.environ.get(
+        "CSVTHD_CONFIG_FILEPATH", DEFAULT_CONFIG_FILEPATH
+    )
+
     filters = []
 
     # create transaction type filter
     if transaction_type is not None:
         filters.append(transaction_type_filter(transaction_type))
 
     # create account name filter
     if account_name is not None:
         filters.append(account_name_filter(account_name))
 
+    # create date filters
+    [filters.append(date_filter(_d[0], _d[1])) for _d in date]
+
     # create include filters
     filters.append(details_include_filter(include))
 
     # create exclude filters
     filters.append(details_exclude_filter(exclude))
 
-    # create amount is filters
+    # create amount filters
     [filters.append(amount_is_filter(_amt[0], _amt[1])) for _amt in amount]
 
-    config = load_config()
-    transactions = get_transactions(config["files"])
+    config = load_config(config_filepath)
+
+    try:
+        transactions = get_transactions(config["files"])
+    except EmptyTransactionFile as err:
+        print(
+            f"{RED}ERROR: Transaction file doesn't contain any transactions: {err.filepath}{ANSI_RESET}"
+        )
+        exit(1)
 
     # sort transactions
     if sort_by == "date":
         transactions.sort(
             key=lambda t: datetime.strptime(t["date"], "%d/%m/%Y").timestamp(),
             reverse=reverse_sort,
         )
```

### Comparing `csvthd-0.4.0b0/csvthd/commandline.py` & `csvthd-0.5.0b0/csvthd/commandline.py`

 * *Files identical despite different names*

### Comparing `csvthd-0.4.0b0/csvthd/filters.py` & `csvthd-0.5.0b0/csvthd/filters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+from datetime import datetime
+
+DATE_STRING_FORMAT = "%d/%m/%Y"
+
+
 def details_include_filter(substrings):
     """Only return transactions matching ALL substrings (case insensitive)."""
     # lowercase all substrings
     substrings = [ss.lower() for ss in substrings]
 
     def _func(transaction):
         # get lowercase version of transaction details
@@ -63,14 +68,44 @@
             return _amount == value
         else:
             raise ValueError("Operator must by `above`, `below` or `equal`")
 
     return _func
 
 
+def date_filter(operator, date_str):
+    """Filter out transactions based on dates.
+
+    Operator is `before`, `after` or `on`.
+    Date is a string of format DD/MM/YYYY.
+    """
+
+    # convert date_str to unix timestamp for simple comparison
+    _filter_timestamp = datetime.strptime(
+        date_str, DATE_STRING_FORMAT
+    ).timestamp()
+
+    def _func(transaction):
+        # convert transaction date to timestamp for simple comparison
+        _trans_timestamp = datetime.strptime(
+            transaction["date"], DATE_STRING_FORMAT
+        ).timestamp()
+
+        if operator == "before":
+            return _trans_timestamp < _filter_timestamp
+        elif operator == "after":
+            return _trans_timestamp > _filter_timestamp
+        elif operator == "on":
+            return _trans_timestamp == _filter_timestamp
+        else:
+            raise ValueError("Operator must by `before`, `after` or `on`")
+
+    return _func
+
+
 def transaction_type_filter(transaction_type):
     """Only return transactions of a give type (i.e. money sent/recieved)."""
 
     def _func(transaction):
         # convert amount to float
         _amount = float(transaction["amount"])
```

### Comparing `csvthd-0.4.0b0/csvthd/reducers.py` & `csvthd-0.5.0b0/csvthd/reducers.py`

 * *Files identical despite different names*

### Comparing `csvthd-0.4.0b0/pyproject.toml` & `csvthd-0.5.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "csvthd"
-version = "0.4.0b0"
+version = "0.5.0b0"
 description = "CSV Transaction History Detective"
 authors = ["DrTexx <denver.opensource@tutanota.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 repository = "https://gitlab.com/DrTexx/csv-transaction-history-detective/"
 documentation = "https://gitlab.com/DrTexx/csv-transaction-history-detective/#getting-started"
 keywords = ["finance", "csv", "transactions", "tax", "accounting"]
```

### Comparing `csvthd-0.4.0b0/PKG-INFO` & `csvthd-0.5.0b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvthd
-Version: 0.4.0b0
+Version: 0.5.0b0
 Summary: CSV Transaction History Detective
 Home-page: https://gitlab.com/DrTexx/csv-transaction-history-detective/
 License: AGPL-3.0-only
 Keywords: finance,csv,transactions,tax,accounting
 Author: DrTexx
 Author-email: denver.opensource@tutanota.com
 Requires-Python: >=3.8,<4.0
@@ -15,16 +15,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Project-URL: Documentation, https://gitlab.com/DrTexx/csv-transaction-history-detective/#getting-started
 Project-URL: Repository, https://gitlab.com/DrTexx/csv-transaction-history-detective/
 Description-Content-Type: text/markdown
 
+[![pipeline status](https://gitlab.com/DrTexx/csv-transaction-history-detective/badges/main/pipeline.svg)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/commits/main)
+[![coverage report](https://gitlab.com/DrTexx/csv-transaction-history-detective/badges/main/coverage.svg)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/commits/main)
+[![GitLab issues](https://img.shields.io/gitlab/issues/open/drtexx/csv-transaction-history-detective?logo=gitlab)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/issues)
+[![GitLab merge requests](https://img.shields.io/gitlab/merge-requests/open/drtexx/csv-transaction-history-detective?logo=gitlab)](https://gitlab.com/DrTexx/csv-transaction-history-detective/-/merge_requests)
+
 # CSV Transaction History Detective
 
+[![PyPI Release](https://img.shields.io/pypi/v/csvthd?logo=python)](https://pypi.org/project/csvthd)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/csvthd?logo=Python)](https://pypi.org/project/csvthd)
+[![PyPI - License](https://img.shields.io/pypi/l/csvthd?color=orange&logo=Python)](https://pypi.org/project/csvthd)
+
 ## Getting started
 
 <!-- TODO: add an example `config.json` file called `config.json.example.json` -->
 
 <!-- TODO: add an example csv file to give more context to why `config.json.example.md` is laid out how it is -->
 
 <!-- TODO: mention in `config.json.template.md` to look at `config.json.example.md` for an example config. -->
@@ -104,14 +113,34 @@
 # only show transactions between $20.00 to $30.00
 csvthd -a over 20 -a under 30
 
 # only show transactions of exactly $25.00
 csvthd -a equal 25
 ```
 
+#### Date
+
+`-d/--date`
+
+Only show transactions before/after/on a given date.
+
+```bash
+# only show transactions after 1 Jan 2022
+csvthd -d after 01/01/2022
+
+# only show transactions before 21 Feb 2022
+csvthd -d before 21/02/2022
+
+# only show transactions on 10 Apr 2022
+csvthd -d on 10/04/2022
+
+# only show transactions from 1 Jan 2022 - 1 Feb 2022
+csvthd -d after 01/01/2022 -d before 01/02/2022
+```
+
 #### Type
 
 `-t/--transaction-type`
 
 Only show transactions where money is sent/received
 
 ```bash
```

