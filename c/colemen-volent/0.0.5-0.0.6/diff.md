# Comparing `tmp/colemen_volent-0.0.5.tar.gz` & `tmp/colemen_volent-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colemen_volent-0.0.5.tar", last modified: Wed Apr 26 16:57:46 2023, max compression
+gzip compressed data, was "colemen_volent-0.0.6.tar", last modified: Fri Apr 28 20:34:39 2023, max compression
```

## Comparing `colemen_volent-0.0.5.tar` & `colemen_volent-0.0.6.tar`

### file list

```diff
@@ -1,75 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.389936 colemen_volent-0.0.5/
--rw-rw-rw-   0        0        0      469 2023-04-26 16:57:46.388936 colemen_volent-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.272935 colemen_volent-0.0.5/colemen_volent.egg-info/
--rw-rw-rw-   0        0        0      469 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1708 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-26 16:57:46.000000 colemen_volent-0.0.5/colemen_volent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 16:57:46.389936 colemen_volent-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1328 2023-04-26 16:57:45.000000 colemen_volent-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.282936 colemen_volent-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.0.5/tests/schema_dict_test.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.295936 colemen_volent-0.0.5/volent/
--rw-rw-rw-   0        0        0     5698 2023-04-26 16:27:55.000000 colemen_volent-0.0.5/volent/Column.py
--rw-rw-rw-   0        0        0     8710 2023-04-18 16:18:27.000000 colemen_volent-0.0.5/volent/Database.py
--rw-rw-rw-   0        0        0    12556 2023-04-26 16:48:34.000000 colemen_volent-0.0.5/volent/Field.py
--rw-rw-rw-   0        0        0    21292 2023-04-26 16:52:50.000000 colemen_volent-0.0.5/volent/Model.py
--rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.5/volent/NestedField.py
--rw-rw-rw-   0        0        0     2855 2023-04-21 13:13:13.000000 colemen_volent-0.0.5/volent/Relationship.py
--rw-rw-rw-   0        0        0    22862 2023-04-26 16:27:13.000000 colemen_volent-0.0.5/volent/Schema.py
--rw-rw-rw-   0        0        0     1478 2023-04-14 12:21:18.000000 colemen_volent-0.0.5/volent/UniqueConstraint.py
--rw-rw-rw-   0        0        0    15407 2023-04-26 16:53:59.000000 colemen_volent-0.0.5/volent/Volent.py
--rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.5/volent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.339935 colemen_volent-0.0.5/volent/data_types/
--rw-rw-rw-   0        0        0     2345 2023-04-26 13:07:40.000000 colemen_volent-0.0.5/volent/data_types/BigInt.py
--rw-rw-rw-   0        0        0     1376 2023-04-25 19:35:38.000000 colemen_volent-0.0.5/volent/data_types/Bool.py
--rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.0.5/volent/data_types/Decimal.py
--rw-rw-rw-   0        0        0     1793 2023-04-26 13:07:50.000000 colemen_volent-0.0.5/volent/data_types/EncodedPrimary.py
--rw-rw-rw-   0        0        0     1954 2023-04-26 16:26:49.000000 colemen_volent-0.0.5/volent/data_types/Integer.py
--rw-rw-rw-   0        0        0     1587 2023-04-11 19:39:38.000000 colemen_volent-0.0.5/volent/data_types/String.py
--rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.0.5/volent/data_types/TinyInt.py
--rw-rw-rw-   0        0        0     4404 2023-04-18 13:41:38.000000 colemen_volent-0.0.5/volent/data_types/TypeBase.py
--rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.5/volent/data_types/__init__.py
--rw-rw-rw-   0        0        0     1055 2023-04-25 19:27:57.000000 colemen_volent-0.0.5/volent/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.346936 colemen_volent-0.0.5/volent/mixins/
--rw-rw-rw-   0        0        0    22897 2023-04-26 13:08:22.000000 colemen_volent-0.0.5/volent/mixins/DatabaseConnection.py
--rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.5/volent/mixins/EntityName.py
--rw-rw-rw-   0        0        0    17876 2023-04-18 14:57:37.000000 colemen_volent-0.0.5/volent/mixins/MySQLGeneratorMixin.py
--rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.5/volent/mixins/OrderedClass.py
--rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.5/volent/mixins/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.355936 colemen_volent-0.0.5/volent/query/
--rw-rw-rw-   0        0        0     2579 2023-04-26 16:57:41.000000 colemen_volent-0.0.5/volent/query/Delete.py
--rw-rw-rw-   0        0        0     5324 2023-04-26 16:27:03.000000 colemen_volent-0.0.5/volent/query/Insert.py
--rw-rw-rw-   0        0        0    15281 2023-04-26 16:28:20.000000 colemen_volent-0.0.5/volent/query/Query.py
--rw-rw-rw-   0        0        0     7173 2023-04-26 13:08:42.000000 colemen_volent-0.0.5/volent/query/Select.py
--rw-rw-rw-   0        0        0     4232 2023-04-26 16:51:08.000000 colemen_volent-0.0.5/volent/query/Update.py
--rw-rw-rw-   0        0        0     5171 2023-04-25 16:18:28.000000 colemen_volent-0.0.5/volent/query/WhereMixin.py
--rw-rw-rw-   0        0        0      183 2023-04-26 16:50:07.000000 colemen_volent-0.0.5/volent/query/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.360937 colemen_volent-0.0.5/volent/settings/
--rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.5/volent/settings/__init__.py
--rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.0.5/volent/settings/control.py
--rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.5/volent/settings/globe.py
--rw-rw-rw-   0        0        0     2165 2023-04-18 18:20:43.000000 colemen_volent-0.0.5/volent/settings/types.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.370935 colemen_volent-0.0.5/volent/tests/
--rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.5/volent/tests/__init__.py
--rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.0.5/volent/tests/schema_dict_test.py
--rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.0.5/volent/tests/validators_test.py
-drwxrwxrwx   0        0        0        0 2023-04-26 16:57:46.387936 colemen_volent-0.0.5/volent/validate/
--rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.0.5/volent/validate/CreditCardNumber.py
--rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Email.py
--rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Equal.py
--rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.5/volent/validate/FutureUnixDate.py
--rw-rw-rw-   0        0        0     3993 2023-04-25 15:53:35.000000 colemen_volent-0.0.5/volent/validate/IpAddress.py
--rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/Length.py
--rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/NoneOf.py
--rw-rw-rw-   0        0        0     2771 2023-04-25 15:57:11.000000 colemen_volent-0.0.5/volent/validate/OneOf.py
--rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.5/volent/validate/PastUnixDate.py
--rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.0.5/volent/validate/PhoneNumber.py
--rw-rw-rw-   0        0        0     5995 2023-04-25 15:51:54.000000 colemen_volent-0.0.5/volent/validate/Range.py
--rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.0.5/volent/validate/Regex.py
--rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/SocialSecurityNumber.py
--rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.5/volent/validate/StrongPassword.py
--rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.5/volent/validate/Validator.py
--rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.0.5/volent/validate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.895717 colemen_volent-0.0.6/
+-rw-rw-rw-   0        0        0      469 2023-04-28 20:34:39.895717 colemen_volent-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.815715 colemen_volent-0.0.6/colemen_volent.egg-info/
+-rw-rw-rw-   0        0        0      469 2023-04-28 20:34:39.000000 colemen_volent-0.0.6/colemen_volent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1796 2023-04-28 20:34:39.000000 colemen_volent-0.0.6/colemen_volent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 20:34:39.000000 colemen_volent-0.0.6/colemen_volent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 20:34:39.000000 colemen_volent-0.0.6/colemen_volent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-04-28 20:34:39.000000 colemen_volent-0.0.6/colemen_volent.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 20:34:39.895717 colemen_volent-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1328 2023-04-28 20:34:38.000000 colemen_volent-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.817715 colemen_volent-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0     2077 2023-04-24 15:33:47.000000 colemen_volent-0.0.6/tests/schema_dict_test.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.839716 colemen_volent-0.0.6/volent/
+-rw-rw-rw-   0        0        0     9991 2023-04-28 16:46:19.000000 colemen_volent-0.0.6/volent/Column.py
+-rw-rw-rw-   0        0        0    10316 2023-04-28 16:26:09.000000 colemen_volent-0.0.6/volent/Database.py
+-rw-rw-rw-   0        0        0    14712 2023-04-27 19:22:06.000000 colemen_volent-0.0.6/volent/Field.py
+-rw-rw-rw-   0        0        0     2914 2023-04-28 15:52:22.000000 colemen_volent-0.0.6/volent/FullTextIndex.py
+-rw-rw-rw-   0        0        0    34744 2023-04-28 16:19:11.000000 colemen_volent-0.0.6/volent/Model.py
+-rw-rw-rw-   0        0        0     7361 2023-04-21 13:52:04.000000 colemen_volent-0.0.6/volent/NestedField.py
+-rw-rw-rw-   0        0        0     5037 2023-04-28 17:06:40.000000 colemen_volent-0.0.6/volent/Relationship.py
+-rw-rw-rw-   0        0        0    21549 2023-04-28 20:34:26.000000 colemen_volent-0.0.6/volent/ReverseEngineer.py
+-rw-rw-rw-   0        0        0    27181 2023-04-28 11:26:02.000000 colemen_volent-0.0.6/volent/Schema.py
+-rw-rw-rw-   0        0        0     2657 2023-04-28 15:48:09.000000 colemen_volent-0.0.6/volent/UniqueConstraint.py
+-rw-rw-rw-   0        0        0    16022 2023-04-28 14:04:59.000000 colemen_volent-0.0.6/volent/Volent.py
+-rw-rw-rw-   0        0        0       59 2023-04-11 20:23:11.000000 colemen_volent-0.0.6/volent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.849714 colemen_volent-0.0.6/volent/data_types/
+-rw-rw-rw-   0        0        0     2345 2023-04-26 13:07:40.000000 colemen_volent-0.0.6/volent/data_types/BigInt.py
+-rw-rw-rw-   0        0        0     1815 2023-04-27 19:22:16.000000 colemen_volent-0.0.6/volent/data_types/Bool.py
+-rw-rw-rw-   0        0        0     1738 2023-04-24 14:13:06.000000 colemen_volent-0.0.6/volent/data_types/Decimal.py
+-rw-rw-rw-   0        0        0     1793 2023-04-26 13:07:50.000000 colemen_volent-0.0.6/volent/data_types/EncodedPrimary.py
+-rw-rw-rw-   0        0        0     1954 2023-04-26 16:26:49.000000 colemen_volent-0.0.6/volent/data_types/Integer.py
+-rw-rw-rw-   0        0        0     2787 2023-04-27 19:21:56.000000 colemen_volent-0.0.6/volent/data_types/String.py
+-rw-rw-rw-   0        0        0      909 2023-04-24 14:13:20.000000 colemen_volent-0.0.6/volent/data_types/TinyInt.py
+-rw-rw-rw-   0        0        0     4455 2023-04-28 16:38:41.000000 colemen_volent-0.0.6/volent/data_types/TypeBase.py
+-rw-rw-rw-   0        0        0      472 2023-04-21 16:39:20.000000 colemen_volent-0.0.6/volent/data_types/__init__.py
+-rw-rw-rw-   0        0        0     3362 2023-04-27 21:05:39.000000 colemen_volent-0.0.6/volent/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.855714 colemen_volent-0.0.6/volent/mixins/
+-rw-rw-rw-   0        0        0    23375 2023-04-27 21:05:57.000000 colemen_volent-0.0.6/volent/mixins/DatabaseConnection.py
+-rw-rw-rw-   0        0        0      729 2023-04-11 19:34:06.000000 colemen_volent-0.0.6/volent/mixins/EntityName.py
+-rw-rw-rw-   0        0        0    19574 2023-04-28 16:18:26.000000 colemen_volent-0.0.6/volent/mixins/MySQLGeneratorMixin.py
+-rw-rw-rw-   0        0        0     3686 2023-04-13 19:47:45.000000 colemen_volent-0.0.6/volent/mixins/OrderedClass.py
+-rw-rw-rw-   0        0        0     1835 2023-04-28 20:31:20.000000 colemen_volent-0.0.6/volent/mixins/ReverseEngineerMixin.py
+-rw-rw-rw-   0        0        0      346 2023-04-18 13:01:17.000000 colemen_volent-0.0.6/volent/mixins/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.866716 colemen_volent-0.0.6/volent/query/
+-rw-rw-rw-   0        0        0     4801 2023-04-28 12:53:20.000000 colemen_volent-0.0.6/volent/query/Delete.py
+-rw-rw-rw-   0        0        0     9602 2023-04-28 12:52:12.000000 colemen_volent-0.0.6/volent/query/Insert.py
+-rw-rw-rw-   0        0        0    20393 2023-04-28 12:24:04.000000 colemen_volent-0.0.6/volent/query/Query.py
+-rw-rw-rw-   0        0        0     9303 2023-04-28 16:18:23.000000 colemen_volent-0.0.6/volent/query/Select.py
+-rw-rw-rw-   0        0        0     5321 2023-04-28 14:43:43.000000 colemen_volent-0.0.6/volent/query/Update.py
+-rw-rw-rw-   0        0        0    13145 2023-04-28 16:20:12.000000 colemen_volent-0.0.6/volent/query/WhereMixin.py
+-rw-rw-rw-   0        0        0      183 2023-04-26 16:50:07.000000 colemen_volent-0.0.6/volent/query/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.870716 colemen_volent-0.0.6/volent/settings/
+-rw-rw-rw-   0        0        0      129 2023-04-11 19:11:30.000000 colemen_volent-0.0.6/volent/settings/__init__.py
+-rw-rw-rw-   0        0        0     6183 2023-04-24 14:05:40.000000 colemen_volent-0.0.6/volent/settings/control.py
+-rw-rw-rw-   0        0        0      152 2023-04-11 20:12:31.000000 colemen_volent-0.0.6/volent/settings/globe.py
+-rw-rw-rw-   0        0        0     2331 2023-04-28 11:50:00.000000 colemen_volent-0.0.6/volent/settings/types.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.873715 colemen_volent-0.0.6/volent/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-24 14:58:16.000000 colemen_volent-0.0.6/volent/tests/__init__.py
+-rw-rw-rw-   0        0        0     4222 2023-04-24 17:14:04.000000 colemen_volent-0.0.6/volent/tests/schema_dict_test.py
+-rw-rw-rw-   0        0        0     8452 2023-04-24 17:01:23.000000 colemen_volent-0.0.6/volent/tests/validators_test.py
+drwxrwxrwx   0        0        0        0 2023-04-28 20:34:39.893720 colemen_volent-0.0.6/volent/validate/
+-rw-rw-rw-   0        0        0     3075 2023-04-24 16:59:56.000000 colemen_volent-0.0.6/volent/validate/CreditCardNumber.py
+-rw-rw-rw-   0        0        0     2866 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/Email.py
+-rw-rw-rw-   0        0        0     1620 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/Equal.py
+-rw-rw-rw-   0        0        0     1709 2023-04-21 16:10:49.000000 colemen_volent-0.0.6/volent/validate/FutureUnixDate.py
+-rw-rw-rw-   0        0        0     3993 2023-04-25 15:53:35.000000 colemen_volent-0.0.6/volent/validate/IpAddress.py
+-rw-rw-rw-   0        0        0     2448 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/Length.py
+-rw-rw-rw-   0        0        0     3658 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/NoneOf.py
+-rw-rw-rw-   0        0        0     2771 2023-04-25 15:57:11.000000 colemen_volent-0.0.6/volent/validate/OneOf.py
+-rw-rw-rw-   0        0        0     1721 2023-04-21 16:10:42.000000 colemen_volent-0.0.6/volent/validate/PastUnixDate.py
+-rw-rw-rw-   0        0        0     2394 2023-04-24 16:42:48.000000 colemen_volent-0.0.6/volent/validate/PhoneNumber.py
+-rw-rw-rw-   0        0        0     5995 2023-04-25 15:51:54.000000 colemen_volent-0.0.6/volent/validate/Range.py
+-rw-rw-rw-   0        0        0     2725 2023-04-24 17:08:33.000000 colemen_volent-0.0.6/volent/validate/Regex.py
+-rw-rw-rw-   0        0        0     2265 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/SocialSecurityNumber.py
+-rw-rw-rw-   0        0        0     2490 2023-04-14 13:23:23.000000 colemen_volent-0.0.6/volent/validate/StrongPassword.py
+-rw-rw-rw-   0        0        0     1414 2023-04-14 13:25:54.000000 colemen_volent-0.0.6/volent/validate/Validator.py
+-rw-rw-rw-   0        0        0      770 2023-04-24 16:48:21.000000 colemen_volent-0.0.6/volent/validate/__init__.py
```

### Comparing `colemen_volent-0.0.5/colemen_volent.egg-info/SOURCES.txt` & `colemen_volent-0.0.6/colemen_volent.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 colemen_volent.egg-info/requires.txt
 colemen_volent.egg-info/top_level.txt
 tests/__init__.py
 tests/schema_dict_test.py
 volent/Column.py
 volent/Database.py
 volent/Field.py
+volent/FullTextIndex.py
 volent/Model.py
 volent/NestedField.py
 volent/Relationship.py
+volent/ReverseEngineer.py
 volent/Schema.py
 volent/UniqueConstraint.py
 volent/Volent.py
 volent/__init__.py
 volent/exceptions.py
 volent/data_types/BigInt.py
 volent/data_types/Bool.py
@@ -26,14 +28,15 @@
 volent/data_types/TinyInt.py
 volent/data_types/TypeBase.py
 volent/data_types/__init__.py
 volent/mixins/DatabaseConnection.py
 volent/mixins/EntityName.py
 volent/mixins/MySQLGeneratorMixin.py
 volent/mixins/OrderedClass.py
+volent/mixins/ReverseEngineerMixin.py
 volent/mixins/__init__.py
 volent/query/Delete.py
 volent/query/Insert.py
 volent/query/Query.py
 volent/query/Select.py
 volent/query/Update.py
 volent/query/WhereMixin.py
```

### Comparing `colemen_volent-0.0.5/setup.py` & `colemen_volent-0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from glob import glob
 from setuptools import setup, find_packages
 import colemen_utilities.build_utils.general as _gen
 
 
-VERSION='0.0.5'
+VERSION='0.0.6'
 DESCRIPTION = 'volent'
 LONG_DESCRIPTION = 'None'
 
 
 _root_path = f"{os.getcwd()}/volent"
 PY_MODULES = _gen.list_py_modules(
     _root_path,
```

### Comparing `colemen_volent-0.0.5/tests/schema_dict_test.py` & `colemen_volent-0.0.6/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/Database.py` & `colemen_volent-0.0.6/volent/Database.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Iterable
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
-import volent.settings as _settings
+# import volent.settings as _settings
 # from volent.Column import Column as _column
 # from volent.Relationship import Relationship as _relationship
 # from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 # from volent.mixins import OrderedClass,MySQLGeneratorMixin
 # from volent.query.Insert import Insert as _insert
 from volent.mixins.DatabaseConnection import DatabaseConnection as _DatabaseConnection
 
@@ -40,15 +40,41 @@
 
     def __init__(self,main:_t._main_type,name:str) -> None:
         self.main = main
         self._name = name
         self._models = []
         self._models_lookup = {}
 
-    def generate_sql(self,file_path:str=None,drops:bool=True):
+    def generate_sql(self,file_path:str=None,drops:bool=True)->str:
+        '''
+            Generates the master sql for all tables in this database.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`file_path`=None] {str}
+                The path to where the sql will be saved, defaults to {cwd}/master.sql
+            [`drops`=True] {bool}
+                If False, the drop statements will not be added to the sql.
+
+
+            Return {str}
+            ----------------------
+            The sql content.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:41:21
+            `memberOf`: Database
+            `version`: 1.0
+            `method_name`: generate_sql
+            * @xxx [04-28-2023 09:42:56]: documentation for generate_sql
+        '''
         if file_path is None:
             file_path = f"{os.getcwd()}/{self.name}.sql"
         sql = self.master_sql(file_path,drops)
         return sql
 
     @property
     def summary(self):
@@ -62,34 +88,33 @@
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-18-2023 08:24:31
             `@memberOf`: Database
             `@property`: summary
         '''
         value = {
+            "name":self.name,
             "models":[x.summary for x in self.models]
         }
 
-        # for m in self.models:
-        #     value["models"][m.name] = m.summary
         return value
 
     @property
-    def name(self):
+    def name(self)->str:
         '''
-            Get this Model's name
+            Get this Database's name
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-11-2023 14:15:56
-            `@memberOf`: Model
+            `@memberOf`: Database
             `@property`: name
         '''
         return self._name
 
     @property
     def models(self):
         '''
@@ -104,16 +129,41 @@
             `@created`: 04-18-2023 08:15:08
             `@memberOf`: Database
             `@property`: models
         '''
         value = self._models
         return value
 
-    def get_model(self,name:str):
+    def get_model(self,name:str)->_t.model_type:
+        '''
+            Retrieve a model by searching its name.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `name` {str}
+                The name of the model to search for.
+
+            Return {model}
+            ----------------------
+            The model instance if successful, None otherwise.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:57:12
+            `memberOf`: Database
+            `version`: 1.0
+            `method_name`: get_model
+            * @xxx [04-28-2023 09:57:59]: documentation for get_model
+        '''
         model = None
+        if name in self._models_lookup:
+            return self._models_lookup[name]
         for m in self.models:
             if m.name == name:
                 return m
 
         return model
 
 
@@ -133,22 +183,22 @@
             `memberOf`: Database
             `version`: 1.0
             `method_name`: register_models
             * @xxx [04-18-2023 08:13:08]: documentation for register_models
         '''
         for mdl in self.main.models:
             if mdl.database_name == self.name:
-                print(f"associating")
+                # print(f"associating model {mdl.name} to database {self.name}")
                 mdl._database = self
                 self._models.append(mdl)
                 self._models_lookup[mdl.name] = mdl
 
     def existing_tables(self):
         sql = f"""SELECT * FROM information_schema.tables WHERE table_type = 'base table' AND TABLE_SCHEMA = '{self.name}'"""
-        print(f"sql:{sql}")
+        # print(f"sql:{sql}")
         self.run(sql)
         result = self.fetchall()
         # print(f"result:{result}")
         c.file.writer.to_json("live_db.json",result)
         for x in result:
             # if x['TABLE_SCHEMA'] == self.name:
             table_name = x['TABLE_NAME']
@@ -244,16 +294,14 @@
             * @xxx [04-18-2023 10:18:44]: documentation for create_model_tables
         '''
         for m in self.models:
             if force is True:
                 self.run(m.drop_statement,foreign_key_checks=foreign_key_checks)
             self.run(m.create_statement,foreign_key_checks=foreign_key_checks)
 
-
-
     def last_id(self)->int:
         '''
             Retrieve the last insert id committed to the database.
             ----------
 
             Return {int}
             ----------------------
```

### Comparing `colemen_volent-0.0.5/volent/Field.py` & `colemen_volent-0.0.6/volent/Field.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 
 from dataclasses import dataclass
-from typing import Iterable,OrderedDict
+from typing import Iterable,OrderedDict, Union
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
@@ -36,20 +36,23 @@
     _example:str = None
     _ignore_null:bool = False
     column:_t.column_type = None
 
 
     required:bool = False
     nullable:bool = True
-    default = None
+    default = _settings.types.no_default
     validators = None
+    _aliases = None
     _data_type:_t.type_base_type = None
-    _value = None
+    # _value = None
+    _value = _t.undefined
     '''The value associated to this field if there is no column'''
     _open_api_location:str = None
+    _not_provided:bool = False
 
 
     def __init__(
         self,
         column:str=None,
         required:bool=False,
         nullable:bool=True,
@@ -57,14 +60,15 @@
         ignore_null:bool=False,
         default=_settings.types.no_default,
         validate=None,
         data_type:_t.type_base_type=None,
         description:str=None,
         example=None,
         open_api_location=None,
+        aliases:Union[list,str]=None,
         ):
         '''
             Create a schema Field
             ----------
 
             Arguments
             -------------------------
@@ -113,14 +117,16 @@
         self._example = example
         self.required = required
         self.nullable = nullable
         self.empty_string_is_null = empty_string_is_null
         self._ignore_null = ignore_null
         self._data_type = data_type
         self._open_api_location = open_api_location
+        self.aliases = aliases
+        
 
         self.validators = c.arr.force_list(validate,allow_nulls=False)
 
 
     @property
     def summary(self):
         '''
@@ -176,15 +182,20 @@
             `@memberOf`: Field
             `@property`: value
         '''
         value = None
         if self.column is not None:
             value = self.column.value
         else:
-            value = self._value
+            if self._value != _t.undefined:
+                value = self._value
+            else:
+                if self.default != _t.no_default:
+                    value=self._value = self.default
+                    # value = self.default
 
         if isinstance(value,(str)):
             if len(value)==0 and self.empty_string_is_null:
                 value = None
         return value
 
     @value.setter
@@ -246,14 +257,58 @@
         if self._data_type is not None:
             if hasattr(self._data_type,"open_api_data_type"):
                 value = self._data_type.open_api_data_type
         elif self.column is not None:
             value = self.column.deserialized_value()
         return value
 
+    @property
+    def aliases(self):
+        '''
+            Get this Field's aliases
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-27-2023 12:58:05
+            `@memberOf`: Field
+            `@property`: aliases
+        '''
+        value = self._aliases
+        if value is None:
+            value = []
+            self._aliases = value
+        return value
+
+    @aliases.setter
+    def aliases(self,value):
+        '''
+            Set the Field's aliases property
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-27-2023 12:58:24
+            `@memberOf`: Field
+            `@property`: aliases
+        '''
+        if isinstance(value,(str)):
+            self._aliases = c.arr.force_list(str)
+        if isinstance(value,(list)):
+            self._aliases = value
+        if value is None:
+            self._aliases = []
+
+
     def validate_value(self,value):
         val = value
         if self._data_type is not None:
             if hasattr(self._data_type,"serializer"):
                 val = self._data_type.serializer(val,self.name)
             if hasattr(self._data_type,"deserialized_value"):
                 val = self._data_type.deserialized_value(val)
@@ -407,16 +462,43 @@
 
     @property
     def should_ignore(self):
         if self.value is None and self._ignore_null is True:
             return True
         return False
 
+    @property
+    def not_provided(self)->bool:
+        return self._not_provided
+
+    @not_provided.setter
+    def not_provided(self,value):
+        '''
+            Set the Field's not_provided property
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-27-2023 13:42:47
+            `@memberOf`: Field
+            `@property`: not_provided
+        '''
+        self._not_provided = value
+
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} : {self.name}>"
 
 
-
+    def name_in_dict(self,data):
+        if self.name in data:
+            return self.name
+        for k,_ in data.items():
+            if k in self.aliases:
+                return k
+        return False
```

### Comparing `colemen_volent-0.0.5/volent/Model.py` & `colemen_volent-0.0.6/volent/Model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+'''
+    The model (table) module
+
+    ----------
+
+    Meta
+    ----------
+    `author`: Colemen Atwood
+    `created`: 04-28-2023 06:59:46
+    `name`: model
+    * @xxx [04-28-2023 06:59:59]: documentation for model
+'''
+
+
+
+
 
 
 from dataclasses import dataclass
 from typing import Iterable, Union
-import operator
+from datetime import datetime
+from datetime import timezone
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.Column import Column as _column
 from volent.Relationship import Relationship as _relationship
 from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
+from volent.FullTextIndex import FullTextIndex as _fullTextIndex
 from volent.mixins import OrderedClass,MySQLGeneratorMixin
 from volent.query.Insert import Insert as _insert
 from volent.query.Select import Select as _select
 from volent.query.Update import Update as _update
 from volent.query.Delete import Delete as _delete
 
 @dataclass
@@ -32,71 +50,168 @@
     _database_name:str = None
     '''The name of the database that this model belongs to.'''
     _database:_t.database_type = None
     '''A reference to the database instance.'''
     _description:str = None
     '''A description of this model that is applied to the database table.'''
     _columns:Iterable[_t.column_type] = None
+    '''A list of column instances'''
+    _column_lookup:dict[str,_t.column_type] = None
+    '''A list of primary column instances.'''
     _relationships:Iterable[_t.relationship_type] = None
     '''A list of relationship instances'''
     _unique_constraints:Iterable[_t.unique_constraint_type] = None
+    _unique_constraint_lookup:dict[str,_t.unique_constraint_type] = None
+    '''A list of full unique constraint instances'''
+    _full_text_indexes:Iterable[_t.full_text_index_type] = None
+    '''A list of full text index instances'''
     primary_column:_t.column_type = None
+    _primary_columns:list[_t.column_type] = None
 
     __unique_prop_keys = None
     _saved:bool = False
-    
+
     _parent_models:Iterable[_t.model_type] = None
     '''A list of models that are a parent to this model.'''
     _child_models:Iterable[_t.model_type] = None
     '''A list of models that children of this model.'''
 
+    _longest_column_name:tuple[int,str] = None
+    _relationships_updated:bool = False
+    '''True if all relationships have had their parent models assigned.'''
+
+    _gen_meta_columns:bool = None
     # _should_create:bool = False
     # _existing_table_data:dict = None
 
     def __init__(self,_is_root=False,**kwargs) -> None:
+        '''
+            Create a new model instance.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`_is_root`=False] {bool}
+                This is used internally to determine if this model instance is the first of its kind.
+                You really don't need to worry about it.
+
+            Keyword Arguments
+            -------------------------
+            The keyword arguments are used to apply values to the columns being created for this model.
+
+            So you can supply a spread dictionary with keys that match column names, and the values will
+            be automatically applied to the columns.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:00:11
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: model
+            * @xxx [04-28-2023 07:02:43]: documentation for model
+        '''
         if _is_root is True:
             # _new_get_cls_vars(self)
             _settings.globe.Volent.register(self)
         else:
             self._is_root = False
             # _settings.globe.Volent.register(self)
             # print(f"self.name:{self.name}")
             # mdl = _settings.globe.Volent.get_model(self.name)
             # self.database = mdl.database
 
 
-
         for k,v in kwargs.items():
             col = self.get_column(k)
             if col is not None:
                 if col.is_primary is True and v is None:
                     continue
                 if v != _t.no_default:
                     col.value = v
         self._parent_models = []
         self._child_models = []
-
-
+        self.__gen_auto_columns()
 
     def _get_attrs_from_parent(self):
         '''Used internally to apply the root model attributes to this instance.
-        
+
         Essentially this just copies the database reference to all child instances of a model.
         '''
         if self._is_root is False:
             # print(f"self.name:{self.name}")
             mdl = _settings.globe.Volent.get_model(self.name)
             self._database = mdl.database
 
-
     def __setattr__(self, name, value):
         super().__setattr__(name, value)
 
         if not name in self._order:
             self._order.append(name)
+            if isinstance(value,_column):
+                cols = [] if self._columns is None else self._columns
+                col_lookup = {} if self._column_lookup is None else self._column_lookup
+                primes = [] if self._primary_columns is None else self._primary_columns
+                if value.name is None:
+                    value.name = name
+                value.model = self
+                cols.append(value)
+                if value.is_primary is True:
+                    self.primary_column = value
+                    primes.append(value)
+                _=value.unique
+                _=value.fulltext
+                col_lookup[name] = value
+                self._primary_columns = primes
+                self._column_lookup = col_lookup
+                self._columns = cols
+                self._longest_column_name = c.arr.longest_string(list(col_lookup.keys()))
+
+            self._unique_constraints = [] if self._unique_constraints is None else self._unique_constraints
+            self._unique_constraint_lookup = {} if self._unique_constraint_lookup is None else self._unique_constraint_lookup
+            if isinstance(value,_uniqueConstraint):
+                # print(f"registering unique constraint")
+
+                value.model = self
+                if value.name is None:
+                    value.name = name
+                skip = False
+                for uq in self._unique_constraints:
+                    if uq == value:
+                        print(f"Duplicate unique constraint found: {name} and {uq.name}")
+                        skip = True
+                if skip is False:
+                    self._unique_constraint_lookup[name] = value
+                    self._unique_constraints.append(value)
+
+            self._full_text_indexes = [] if self._full_text_indexes is None else self._full_text_indexes
+            if isinstance(value,_fullTextIndex):
+
+                value.model = self
+                if value.name is None:
+                    value.name = name
+
+                skip = False
+                for uq in self._full_text_indexes:
+                    if uq == value:
+                        print(f"Duplicate fulltext index found: {name} and {uq.name}")
+                        skip = True
+                if skip is False:
+                    self._full_text_indexes.append(value)
+
+
+            self._relationships = [] if self._relationships is None else self._relationships
+            if isinstance(value,_relationship):
+
+                value.child_model = self
+                if value.name is None:
+                    value.name = name
+                self._relationships.append(value)
+
 
         return value
 
     def ordered_attrs(self, with_order=False):
         return [(k,getattr(self, k)) for k in self._order if k != '_order' or with_order]
 
     @property
@@ -112,25 +227,28 @@
             `@author`: Colemen Atwood
             `@created`: 04-18-2023 08:25:40
             `@memberOf`: Model
             `@property`: summary
         '''
         value = {
             "name":self.name,
-            "description":self._description,
+            "description":self.model_description,
             "columns":[x.summary for x in self.columns],
             "relationships":[x.summary for x in self.relationships],
+            "unique_constraints":[x.summary for x in self.unique_constraints],
+            "fulltext_indexes":[x.summary for x in self.full_text_indexes],
+            "parent_tables":[x.name for x in self._parent_models],
+            "child_tables":[x.name for x in self._child_models],
         }
 
 
         return value
 
-
     @property
-    def name(self):
+    def name(self)->str:
         '''
             Get this Model's name
 
             `default`:None
 
 
             Meta
@@ -149,15 +267,15 @@
                     break
             # if hasattr(self,"__table_name__"):
                 # value = getattr(self,"__table_name__")
             self._name = value
         return value
 
     @property
-    def database_name(self):
+    def database_name(self)->str:
         '''
             Get this Model's database_name
 
             `default`:None
 
 
             Meta
@@ -190,15 +308,15 @@
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 04-18-2023 09:48:39
             `@memberOf`: Model
             `@property`: database
         '''
-        
+
         value = self._database
         if value is None:
             self._get_attrs_from_parent()
             value = self._database
         return value
 
     @property
@@ -222,17 +340,17 @@
                 value = getattr(self,"__description__")
             else:
                 value = self.__class__.__doc__
             self._description = value
         return value
 
     @property
-    def data(self):
+    def data(self)->dict:
         '''
-            Get this Model's data
+            Retrieve a dictionary of columns and their values.
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
@@ -241,15 +359,120 @@
             `@property`: data
         '''
         value = {}
         for col in self.columns:
             value[col.name] = col.value
         return value
 
+
+    @property
+    def gen_meta_columns(self):
+        '''
+            Get this Model's gen_meta_columns setting
+            
+            if True, the timestamp,deleted and modified_timestamp columns are automatically created on 
+            this model.
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-28-2023 10:57:56
+            `@memberOf`: Model
+            `@property`: gen_meta_columns
+        '''
+        value = self._gen_meta_columns
+        if value is None:
+            val = False
+            keys = ["__gen_meta_columns__","__meta_columns__"]
+            for key in keys:
+                if hasattr(self,key):
+                    val = getattr(self,key)
+                    break
+            # if hasattr(self,"__table_name__"):
+                # value = getattr(self,"__table_name__")
+            self._gen_meta_columns = val
+        return value
+
+    def __gen_auto_columns(self):
+        '''
+            If the __meta_columns__ key is True, this will create the
+            timestamp,deleted and modified_timestamp columns on this model automatically.
+
+            ----------
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 11:07:25
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: __gen_auto_columns
+            * @xxx [04-28-2023 11:08:31]: documentation for __gen_auto_columns
+        '''
+        if self.gen_meta_columns is False:
+            return
+
+        from volent.data_types import Integer
+        cut = round(datetime.now(tz=timezone.utc).timestamp())
+
+        ct = _column(Integer(), nullable=True, on_insert=cut, comment='The unix timestamp of when this was created.')
+        dt = _column(Integer(), nullable=True, default=None, comment='The unix timestamp of when this was deleted, null otherwise.')
+        mt = _column(Integer(), nullable=True, default=None, on_update=cut,on_insert=cut, comment='The unix timestamp of when this was last modified, null otherwise.')
+        setattr(self,"timestamp",ct)
+        setattr(self,"modified_timestamp",mt)
+        setattr(self,"deleted",dt)
+
+    def __gen_col_sums(self):
+        primes = []
+        col_lookup = {}
+
+        for col in self.columns:
+            # col_lookup[col.name] = col
+            if col.is_primary is True:
+                primes.append(col)
+
+        self._primary_columns = primes
+        # self._column_lookup = col_lookup
+        self._longest_column_name = c.arr.longest_string(list(col_lookup.keys()))
+
     def get_column(self,name:str)->_t.column_type:
+        '''
+            Retrieve a column by searching its name.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `name` {str}
+                The name of the column to search for.
+
+            Return {column,None}
+            ----------------------
+            THe column instance if successful, None otherwise
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:46:53
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: get_column
+            * @xxx [04-28-2023 09:47:36]: documentation for get_column
+        '''
+        value = None
+        if self._column_lookup is None:
+            print(f"GENERATING COLUMN LOOKUP {'-'*80}")
+            self.__gen_col_sums()
+
+        if name in self._column_lookup:
+            return self._column_lookup[name]
+
         for col in self.columns:
             if col.name == name:
                 return col
 
         return None
 
     @property
@@ -266,14 +489,15 @@
             `@created`: 04-11-2023 14:07:35
             `@memberOf`: Model
             `@property`: columns
         '''
         value = self._columns
 
         if value is None:
+            print(f"GENERATING COLUMN LIST {'-'*80}")
             dif = self._unique_prop_keys
             # df_props = dir(Model(_is_root=False))
             # # # @Mstep [] gather the props of this instance.
             # props = dir(self)
             # # # @Mstep [] find the props that exist on this instance and not on the base.
             # dif = c.arr.find_list_diff(props,df_props)
             # dif = dir(self)
@@ -288,14 +512,15 @@
                     # c.con.log(f"located Column: {name}","green")
                     val.name = name
                     val.model = self
                     if val.is_primary is True:
                         self.primary_column = val
                     value.append(val)
 
+        return value
 
 
         order_cols = []
         for k in list(self.ordered_attrs(True)):
             for col in value:
                 if col.name == k[0]:
                     order_cols.append(col)
@@ -326,23 +551,59 @@
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 03-24-2023 09:17:42
             `@memberOf`: Model
             `@property`: primary_columns
         '''
+        if self._primary_columns is None:
+            print(f"GENERATING PRIMARY COLUMNS {'-'*80}")
+            self.__gen_col_sums()
+        # print(f"self._primary_columns: {self._primary_columns}")
+        return self._primary_columns
         value = []
         # print(f"self.columns: {self.columns}")
         for col in self.columns:
             # c.con.log(f"col.name:{col.name}")
             if col.is_primary is True:
                 # print(f"{col.name}.is_primary: {col.is_primary} {type(col.is_primary)}")
                 value.append(col)
         return value
 
+    def get_unique_constraint(self,name:str)->_t.unique_constraint_type:
+        '''
+            Retrieve a unique constraint by its name.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `name` {str}
+                The name of the unique constraint to search for.
+
+            Return {UniqueConstraint}
+            ----------------------
+            The unique constraint instance if successful, None otherwise.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 08:29:07
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: get_unique_constraint
+            * @xxx [04-28-2023 08:30:04]: documentation for get_unique_constraint
+        '''
+        if name in self._unique_constraint_lookup:
+            return self._unique_constraint_lookup[name]
+        for u in self.unique_constraints:
+            if u.name == name:
+                return u
+        return None
+
     @property
     def unique_constraints(self)->Iterable[_t.unique_constraint_type]:
         '''
             Get a list of unique constraint instances from this model.
 
             `default`:None
 
@@ -354,36 +615,65 @@
             `@memberOf`: Model
             `@property`: unique_constraints
         '''
         # return None
         value = self._unique_constraints
 
         if value is None:
+            print(f"GENERATING UNIQUE_CONSTRAINTS LIST {self.name} {'-'*80}")
             dif = self._unique_prop_keys
             # dif = dir(self)
             value = []
             # color = c.rand.option(["magenta","yellow","green","cyan"])
             for prop in dif:
                 name = prop
                 val = getattr(self,prop)
                 if isinstance(val,(_uniqueConstraint)):
                     c.con.log(f"located unique constraint","magenta")
                     val.name = name
                     val.model = self
-
-                    # parent_str = val.parent
-                    # val.parent_model = _settings.globe.Volent.get_model(val.parent)
-                    # val.parent_column = _settings.globe.Volent.get_column(val.parent)
-                    # val.child_column = self.get_column()
                     value.append(val)
 
             self._unique_constraints = value
         return value
 
     @property
+    def full_text_indexes(self)->Iterable[_t.full_text_index_type]:
+        '''
+            Get a list of fulltext index instances from this model.
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 04-28-2023 06:49:39
+            `@memberOf`: Model
+            `@property`: full_text_indexes
+        '''
+        value = self._full_text_indexes
+
+        if value is None:
+            print(f"GENERATING FULL_TEXT_INDEX LIST {'-'*80}")
+            dif = self._unique_prop_keys
+            value = []
+            for prop in dif:
+                name = prop
+                val = getattr(self,prop)
+                if isinstance(val,(_fullTextIndex)):
+                    c.con.log(f"located full text index","magenta")
+                    val.name = name
+                    val.model = self
+                    value.append(val)
+
+            self._full_text_indexes = value
+        return value
+
+    @property
     def relationships(self)->Iterable[_t.relationship_type]:
         '''
             Get a list of relationships instances associated to this table.
 
             `default`:None
 
 
@@ -393,15 +683,31 @@
             `@created`: 03-11-2023 13:47:00
             `@memberOf`: Model
             `@property`: columns
         '''
 
         value = self._relationships
 
+        if self._relationships_updated is False:
+            # @Mstep [LOOP] iterate all relationship instances
+            for val in value:
+                # @Mstep [] assign the parent_model and parent_column to the relationship.
+                # val.name = name
+                val.child_model = self
+                val.parent_model = _settings.globe.Volent.get_model(val.parent)
+                val.parent_column = _settings.globe.Volent.get_column(val.parent)
+
+                # value.append(val)
+                val.parent_model.add_child_model(self)
+                self.add_parent_model(val.parent_model)
+            self._relationships_updated = True
+
+
         if value is None:
+            # This should pretty much never execute, the registration of relationships is handled in __setattr__
             c.con.log(f"Model.relationships","magenta")
             dif = self._unique_prop_keys
 
             value = []
             for prop in dif:
                 name = prop
                 val:_t.relationship_type = getattr(self,prop)
@@ -459,91 +765,164 @@
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 03-24-2023 05:53:18
             `@memberOf`: Model
             `@property`: longest_column_name
         '''
+        if self._longest_column_name is None:
+            self.__gen_col_sums()
+        return self._longest_column_name
         cnames = []
         for col in self.columns:
             cnames.append(col.name)
         return c.arr.longest_string(cnames)
 
-
-    # def set_instance_var(self,name,value):
-    #     self.__dict__[name] = value
-
     def volent_register_subs(self):
         '''Have this model register its child entities
 
         - Columns
         - Unique Constraints
         - Relationships
         '''
-        
+
         for uc in self.unique_constraints:
             _settings.globe.Volent.register(uc)
-            
+
         for rel in self.relationships:
             _settings.globe.Volent.register(rel)
-            
+
         for col in self.columns:
             _settings.globe.Volent.register(col)
 
 
-    # def from_schema(self,schema:_t.schema_type):
-    #     data= schema.dump()
 
-    # def drop(self):
-    #     self.database.run(self.drop_statement,foreign_key_checks=False)
+    # ---------------------------------------------------------------------------- #
+    #                                 QUERY METHODS                                #
+    # ---------------------------------------------------------------------------- #
 
-    # def save(self):
-    #     if self._saved is False:
-    #         if self.primary_column.value is None:
-    #             print(f"SAVING MODEL: {self.name}")
-                
-    #             self.insert(self.data)
-    #         if self.primary_column.value is not None:
-    #             print(f"UPDATING MODEL: {self.name}")
-    #             self.update(**self.data).is_(self.primary_column.name,self.primary_column.value)
+    def insert(self,data:Union[dict,_t.schema_type]=None)->_insert:
+        '''
+            Create an insert query on this model.
 
-    def insert(self,data:Union[dict,_t.schema_type]=None)->bool:
+            ----------
+
+            Arguments
+            -------------------------
+            `data` {dict,schema}
+                The data to be inserted.
+
+            Return {insert}
+            ----------------------
+            An insert query instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:48:39
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: insert
+            * @xxx [04-28-2023 09:49:25]: documentation for insert
+        '''
         # self.database.run('show variables like "max_connections";')
         # print(self.database.fetchall())
         if isinstance(data,(dict)) is False:
             from volent.Schema import Schema as _schema
             if isinstance(data,_schema):
                 data.model = self
                 data = data.dump(self)
+
         ins = _insert(self,data)
-        # print(f"{self.__class__.__name__}.insert - self.name: {self.name}")
-        # print(f"{self.__class__.__name__}.insert - self.database: {self.database}")
-        ins.database = self.database
-        result = ins.execute()
-        # print(f"result:{result}")
+        # ins.database = self.database
+        # result = ins.execute()
+        return ins
 
     def select(self,*columns)->_select:
-        # print(f"columns: {columns}")
+        '''
+            Create a select query on this model.
+
+            ----------
+
+            Arguments
+            -------------------------
+            [`*columns`] {}
+                The columns to select if None are provided, all columns are selected.
+
+            Return {select}
+            ----------------------
+            A select query instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:49:36
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: select
+            * @xxx [04-28-2023 09:51:05]: documentation for select
+        '''
         s = _select(self,columns=columns)
         return s
 
     def update(self,**columns)->_update:
+        '''
+            Create an update query on this model.
+
+            ----------
+
+            Keyword Arguments
+            -------------------------
+            [`*columns`] {}
+                The columns to update and their values.
+
+            Return {update}
+            ----------------------
+            An update query instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:49:36
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: update
+            * @xxx [04-28-2023 09:51:05]: documentation for update
+        '''
         # print(f"columns: {columns}")
         s = _update(self,columns=columns)
         return s
+
     def delete(self)->_delete:
+        '''
+            Create a delete query on this model.
+
+            ----------
+
+            Return {delete}
+            ----------------------
+            An delete query instance.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:49:36
+            `memberOf`: Model
+            `version`: 1.0
+            `method_name`: delete
+            * @xxx [04-28-2023 09:51:05]: documentation for delete
+        '''
         # print(f"columns: {columns}")
         s = _delete(self)
         return s
 
-
     def add_parent_model(self,model:_t.model_type):
         '''
             Add a parent model to this model.
-            
+
             This is for internal use do not arbitrarily add models here, they wont do anything.
             ----------
 
             Arguments
             -------------------------
             `model` {model}
                 The parent model to add.
@@ -557,19 +936,18 @@
             `method_name`: add_parent_model
             * @xxx [04-21-2023 08:26:12]: documentation for add_parent_model
         '''
         if isinstance(model,Model) is False:
             raise TypeError(f"Expects Model type, received {type(model)}")
         self._parent_models.append(model)
 
-
     def add_child_model(self,model:_t.model_type):
         '''
             Add a child model to this model.
-            
+
             This is for internal use do not arbitrarily add models here, they wont do anything.
             ----------
 
             Arguments
             -------------------------
             `model` {model}
                 The child model to add.
@@ -646,15 +1024,15 @@
 #         val = getattr(instance,prop)
 #         if isinstance(val,(_column,_uniqueConstraint,_relationship)):
 #             # print(f"prop: {prop}")
 #             # if name in instance.__dict__:
 #                 # c.con.log(f"adding {name} to instance dict")
 #                 # instance.__dict__[name] = value
 #             # print(f"instance.__dict__: {instance.__dict__}")
-            
+
 #             setattr(instance,name,val)
 #             # instance.set_instance_var(instance,name,val)
 #             # val.name = name
 #             # val.model = instance
 #             # if val.is_primary is True:
 #             #     self.primary_column = val
 #             # value.append(val)
```

### Comparing `colemen_volent-0.0.5/volent/NestedField.py` & `colemen_volent-0.0.6/volent/NestedField.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/Schema.py` & `colemen_volent-0.0.6/volent/Schema.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 
 from dataclasses import dataclass
-from typing import Iterable,OrderedDict
+from typing import Iterable,OrderedDict, Union
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
 import volent.settings as _settings
@@ -18,29 +18,33 @@
 from volent.mixins import OrderedClass
 from volent.exceptions import ValidationError
 
 
 
 @dataclass
 class Schema(metaclass=OrderedClass):
+
     main = None
     # database:_t.database_type = None
     model:_t.model_type = None
     _name:str = None
     _fields:Iterable[_t.field_type] = None
     _schema_description:str = None
     _schema_crud_type:str = None
 
     __unique_prop_keys = None
 
     # _field_aliases = None
 
 
 
-    def __init__(self,model:_t.model_type=None) -> None:
+    def __init__(
+        self,
+        model:_t.model_type=None
+        ) -> None:
         from volent.Model import Model as _model
         if isinstance(model,_model):
             self.model = model
         else:
             if model is not None:
                 md = model()
 
@@ -330,14 +334,16 @@
                 # @Mstep [] set the field's value to the "value"'s value.
                 f.value = value
 
         # @Mstep [] Execute any custom validation methods on this schema
         self.__call_custom_validations()
         # @Mstep [LOOP] iterate the fields associated to this schema
         for f in self.fields:
+            if f.not_provided is True:
+                continue
             # @Mstep [IF] if the field should NOT be skipped
             if f.should_ignore is False:
                 # @Mstep [] have the field self-validate
                 f.validate()
 
     def get_field(self,name:str)->_t.field_type:
         '''
@@ -443,19 +449,103 @@
         value = []
         if loc not in _settings.control.open_api_param_locations:
             raise ValueError(f"{loc} is not a valid param location, expected: {','.join(_settings.control.open_api_param_locations)}")
         for f in self.fields:
             value.append(f.open_api_data(loc))
         return value
 
+    # def serialized(self,model:Union[list,dict,_t.model_type]=None):
+
+
+    def __deserialize_dictionary(
+        self,
+        data:dict,
+        ignore_unprovided:bool=False,
+        )->dict:
+        # c.con.log(f"Deserializing dictionary - raw: {data}","magenta")
+        data = self._remove_missing_fields(data)
+        # data = self._correlate_to_dict(data)
+        # c.con.log(f"Deserializing dictionary - correlated: {data}","info")
+        self.__validate_dict(data)
+        out_data = {}
+        for f in self.fields:
+            if hasattr(f.data_type_instance,"deserialized_value"):
+                if f.name in data:
+                    out_data[f.name] = f.data_type_instance.deserialized_value(data[f.name],f.name)
+                continue
+        # c.con.log(f"Deserializing dictionary - out_data: {out_data}","green")
+        return out_data
+
+    def __deserialize_model(self,model:_t.model_type):
+        out_data = {}
+
+        self.model = model
+        model = self._correlate_to_columns()
+        self.__validate()
+        # data = {}
+        for f in self.fields:
+            # if hasattr(f.data_type_instance,"serializer"):
+            #     v = f.data_type_instance.serializer(f.value,f.name)
+            #     out_data[f.name] = v
+            #     continue
+            if hasattr(f.data_type_instance,"deserialized_value"):
+                v = f.data_type_instance.deserialized_value(f.value)
+                out_data[f.name] = v
+                continue
+            v = f.value
+            out_data[f.name] = v
+
+        return out_data
+
+    def deserialized(
+        self,
+        model:Union[list,dict,_t.model_type]=None,
+        many:bool=False,
+        ignore_unprovided=False
+        ):
+        from volent.Model import Model as _model
+
+        if isinstance(model,(dict)) is True:
+            dr = self.__deserialize_dictionary(model,ignore_unprovided)
+            if many:
+                dr = c.arr.force_list(dr)
+            return dr
+
+        if isinstance(model,(list)) is True:
+            out_data = []
+            for mdl in model:
+                data = {}
+                if isinstance(mdl,dict):
+                    data = self.__deserialize_dictionary(mdl)
+                    out_data.append(data)
+                    continue
+
+                if isinstance(mdl,_model):
+                    data = self.__deserialize_model(mdl)
+                    out_data.append(data)
+                    continue
+
+                # out_data.append(data)
+
+            if many:
+                out_data = c.arr.force_list(out_data)
+            return out_data
+
+        if isinstance(model,(_model)) is True:
+            out_data = self.__deserialize_model(mdl)
+            if many:
+                out_data = c.arr.force_list(out_data)
+            return out_data
+    load = deserialized
+
     def dump(self,model:_t.model_type=None,many=False,ignore_unprovided=False)->dict:
         '''Dump the contents of the model(s) using the fields to filter.'''
 
         if isinstance(model,(dict)):
-            print(f"dictionary provided for dumping.")
+            # print(f"dictionary provided for dumping.")
             data = self._correlate_to_dict(model,ignore_unprovided)
             self.__validate_dict(model)
             out_data = {}
             for f in self.fields:
                 if f.name in data:
                     # print(f"f.value:{f.value}")
                     if hasattr(f.data_type_instance,"serializer"):
@@ -618,32 +708,69 @@
             props = dir(self)
             # # @Mstep [] find the props that exist on this instance and not on the base.
             value = c.arr.find_list_diff(props,df_props)
             self.__unique_prop_keys = value
 
         return value
 
+
+    def _remove_missing_fields(self,data:dict):
+        out = {}
+        data = c.obj.keys_to_snake_case(data)
+        for f in self.fields:
+            key = f.name_in_dict(data)
+            if key is not False:
+                out[f.name] = data[key]
+            else:
+                f.not_provided = True
+        return out
+
     def _correlate_to_dict(self,data:dict,ignore_unprovided=False):
         out_data = {}
         data = c.obj.keys_to_snake_case(data)
         # print(f"_correlate_to_dict: data:{data}")
         for f in self.fields:
             # snake_field = c.string.to_snake_case(f.name)
             # print(f"_correlate_to_dict: snake_field:{snake_field}")
-            if f.name in data:
-                out_data[f.name] = data[f.name]
+            # if self.schema_crud_type == "update":
+            #     # print(f"setting schema for update settings.")
+            #     for f in self.fields:
+
+
+            key = f.name_in_dict(data)
+            if key is not False:
+                out_data[f.name] = data[key]
+                f.value = data[key]
+                continue
+            if key is False:
+                out_data[f.name] = None
+                # out_data[f.name] = _t.undefined
+                f.value= None
+                if self.schema_crud_type in ['update']:
+                    f._ignore_null = True
+                    f.default = None
                 continue
+            # if f.name in data:
+
+            #     # out_data[f.name] = f.data_type_instance.deserialized_value(data[f.name])
+            #     out_data[f.name] = data[f.name]
+            #     f.value = data[f.name]
+            #     continue
             if ignore_unprovided is False:
                 if f.default != _t.no_default:
-                    out_data[f.name] = f.value
-                
-            # if snake_field in data:
-            #     print(f"snake case field match: {c.string.to_snake_case(f.name)}")
-            #     out_data[c.string.to_snake_case(f.name)] = data[c.string.to_snake_case(f.name)]
-            #     continue
+                    f.value = f.default
+                    out_data[f.name] = f.default
+            # @Mstep [IF] if the field is located in the path
+            if f._open_api_location == "path":
+                # @Mstep [IF] if the field has a default value.
+                if f.default != _t.no_default:
+                    # @Mstep [] set the fields value to its default
+                    f.value = f.default
+                    out_data[f.name] = f.default
+
 
         return out_data
 
     def _correlate_to_columns(self):
         '''
             Iterate all fields to find their corresponding columns in the current model.
             ----------
```

### Comparing `colemen_volent-0.0.5/volent/UniqueConstraint.py` & `colemen_volent-0.0.6/volent/UniqueConstraint.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,38 +25,76 @@
 
     def __init__(
         self,
         columns:Iterable[_t.column_type],
         name:str=None,
         comment:str=None,
         ):
+        '''
+            Create a unique constraint instance.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `Columns` {list,column}
+                A column or list of columns to create a unique constraint on.
+
+            `name` {str}
+                The name of this unique constraint. This name must be unique through out the database.
+
+            `comment` {str}
+                The comment to add to the unique constraint in the database.
+
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 09:59:09
+            `memberOf`: UniqueConstraint
+            `version`: 1.0
+            `method_name`: UniqueConstraint
+            * @xxx [04-28-2023 10:01:29]: documentation for UniqueConstraint
+        '''
         self.name = name
         self.comment = comment
-        self.columns = columns
+        self.columns = c.arr.force_list(columns)
 
 
 
         # _parse_parent(self,parent)
 
 
     @property
     def summary(self):
         '''
-            Get this Relationship's summary
+            Get this UniqueConstraint's summary
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
             `@created`: 03-23-2023 14:53:39
-            `@memberOf`: Relationship
+            `@memberOf`: UniqueConstraint
             `@property`: summary
         '''
         value = {
             "name":self.name,
             "comment":self.comment,
             "columns":[x.name for x in self.columns],
         }
         return value
 
+
+
+    def __hash__(self):
+        col_names = [x.name for x in self.columns]
+        val = col_names.append(self.name)
+        return hash(val)
+
+    def __eq__(self,other):
+        if isinstance(other,UniqueConstraint):
+            return self.__hash__() == other.__hash__()
+        return False
+
```

### Comparing `colemen_volent-0.0.5/volent/Volent.py` & `colemen_volent-0.0.6/volent/Volent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,53 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+'''
+    The main module of the volent library.
+
+    ----------
+
+    Meta
+    ----------
+    `author`: Colemen Atwood
+    `created`: 04-28-2023 07:03:18
+    `name`: volent
+    * @xxx [04-28-2023 07:03:34]: documentation for volent
+'''
+
+
 
 import os
 from typing import Iterable
 import colemen_utils as c
 import volent.settings as _settings
 from volent.Model import Model as Model
 from volent.Schema import Schema as Schema
 from volent.Field import Field as Field
 from volent.NestedField import NestedField as NestedField
 from volent.Column import Column as Column
 from volent.Relationship import Relationship as Relationship
 from volent.UniqueConstraint import UniqueConstraint as UniqueConstraint
+from volent.FullTextIndex import FullTextIndex as FullTextIndex
 from volent.Database import Database as _Database
 import volent.validate as validators
 import volent.exceptions as exc
 import volent.data_types as data_types
 import volent.settings.types as _t
 from volent.mixins.DatabaseConnection import DatabaseConnection as _DatabaseConnection
 from volent.mixins.MySQLGeneratorMixin import MySQLGeneratorMixin as _MySQLGeneratorMixin
-
+from volent.settings.types import no_default as noDefault
+from volent.settings.types import undefined
 
 class Volent(_DatabaseConnection,_MySQLGeneratorMixin):
-    def __init__(self):
+    def __init__(
+        self,
+        index_existing_tables:bool=False
+        ):
         self.models:Iterable[_t.model_type] = []
         '''A list of all registered model instances'''
 
         self.model_names:Iterable[str] = []
         '''A list of all registered model/table names'''
 
         self.unique_constraints:Iterable[_t.unique_constraint_type] = []
@@ -43,14 +62,16 @@
         self.relationship_names:Iterable[str] = []
         '''A list of all registered relationship names'''
 
         self.columns:Iterable[_t.column_type] = []
         '''A list of all registered column instances'''
 
         self._databases = []
+        
+        self._index_existing_table:bool = index_existing_tables
         _settings.globe.Volent = self
         super().__init__()
         # self.set_defaults()
 
     # def set_defaults(self):
     #     self.settings = c.file.import_project_settings("volent.settings.json")
 
@@ -111,16 +132,17 @@
         self._deep_registration()
         self._determine_relationships()
         self._generate_databases()
         # result = self.connect()
         if self.connect() is False:
             raise RuntimeError("Failed to connect to the database.")
         else:
-            for db in self.databases:
-                db.existing_tables()
+            if self._index_existing_table is True:
+                for db in self.databases:
+                    db.existing_tables()
 
 
     def register(self,instance):
         '''
             Used internally for registration and mapping of the database structure.
 
             ----------
```

### Comparing `colemen_volent-0.0.5/volent/data_types/BigInt.py` & `colemen_volent-0.0.6/volent/data_types/BigInt.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/data_types/Bool.py` & `colemen_volent-0.0.6/volent/data_types/Bool.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,33 +21,48 @@
         self.sql_type_name = "BOOLEAN"
         self.python_data_type = (bool)
         self.open_api_data_type = "boolean"
 
 
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__} >"
-    
-    
 
-    def serialized_value(self,value):
+
+    def serializer(self,value,field_name:str=None):
+
+        if isinstance(value,(bool)) is False:
+            return self.deserialized_value(value,field_name)
+
+        else:
+            return self.serialized_value(value,field_name)
+
+
+
+    def serialized_value(self,value,field_name:str=None):
 
         if isinstance(value,(bool)):
             return value
-        value = c.types.to_bool(value)
 
-        if isinstance(value,(bool)) is False:
-            raise ValidationError(f"Failed to serialize {value} to a boolean.")
+        value = c.types.bool_to_int(value)
+
+        if isinstance(value,(int)) is False:
+            raise ValidationError(f"Failed to serialize {value} to an integer.",field_name)
 
         return value
 
-    def deserialized_value(self,value):
+    def deserialized_value(self,value,field_name:str=None):
 
         if isinstance(value,(bool)):
             return value
+        if value == _t.undefined or value == _t.no_default:
+            return value
+        if value is None:
+            return value
+
         value = c.types.to_bool(value)
 
         if isinstance(value,(bool)) is False:
-            raise ValidationError(f"Failed to serialize {value} to a boolean.")
-        
+            raise ValidationError(f"Failed to serialize {value} to a boolean.",field_name)
+
         return value
```

### Comparing `colemen_volent-0.0.5/volent/data_types/Decimal.py` & `colemen_volent-0.0.6/volent/data_types/Decimal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/data_types/EncodedPrimary.py` & `colemen_volent-0.0.6/volent/data_types/EncodedPrimary.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/data_types/Integer.py` & `colemen_volent-0.0.6/volent/data_types/Integer.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/data_types/TinyInt.py` & `colemen_volent-0.0.6/volent/data_types/TinyInt.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/data_types/TypeBase.py` & `colemen_volent-0.0.6/volent/data_types/TypeBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
             `@memberOf`: TypeBase
             `@property`: summary
         '''
         value = {
             "sql_type_name":self.sql_type_name,
             "data_length":self.data_length,
             "python_type_name":self.python_type_name,
+            "class_name":self.__class__.__name__,
             # "max_data_length":self.max_data_length,
             # "min_data_length":self.min_data_length,
         }
         return value
 
     def _validate_data_length(self,data_length:int=None,default_value:int=None):
         if data_length is None:
```

### Comparing `colemen_volent-0.0.5/volent/mixins/DatabaseConnection.py` & `colemen_volent-0.0.6/volent/mixins/DatabaseConnection.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import Iterable
 import mysql.connector as _mysqlConnnector
 from mysql.connector.errors import ProgrammingError
 import traceback as _traceback
 import colemen_utils as c
 import volent.settings as _settings
 import volent.settings.types as _t
+import volent.exceptions as _e
 from volent.mixins.MySQLGeneratorMixin import MySQLGeneratorMixin as _MySQLGeneratorMixin
 
 _log = c.con.log
 
 
 class DatabaseConnection(_MySQLGeneratorMixin):
     '''Class used as a mixin to allow database connections and the general CRUD procedures.'''
@@ -399,33 +400,34 @@
 
             self.connection.commit()
             success = True
             if foreign_key_checks is False:
                 self.execute_single_statement("SET FOREIGN_KEY_CHECKS = 1;")
 
 
-        except _mysqlConnnector.errors.IntegrityError:
-            _log(f"{_traceback.format_exc()}","error")
-            _log(f"SQL: {sql}","error")
+        except _mysqlConnnector.errors.IntegrityError as e:
+            # _log(f"{_traceback.format_exc()}","error")
+            # _log(f"SQL: {sql}","error")
+            self._parse_interface_error(e)
 
-        except _mysqlConnnector.errors.InterfaceError:
+        except _mysqlConnnector.errors.InterfaceError as e:
             if isTimeoutRetry is True:
-                _log(f"{_traceback.format_exc()}","error")
-                _log(f"SQL: {sql}","error")
+                # _log(f"{_traceback.format_exc()}","error")
+                # _log(f"SQL: {sql}","error")
+                self._parse_interface_error(e)
             if isTimeoutRetry is False:
-                # _log(f"CONNECTION TIMED OUT")
                 self.cursor = None
                 self.connection = None
                 self.connect()
                 return self.execute_single_statement(sql,args,True)
 
-        except _mysqlConnnector.errors.DatabaseError:
-            # print(f"ERROR: {err}", PRESET="FATAL_ERROR_INVERT")
+        except _mysqlConnnector.errors.DatabaseError as e:
             _log(f"{_traceback.format_exc()}","error")
             _log(f"SQL: {sql}","error")
+            self._parse_interface_error(e)
 
         
         # except sqlite3.Warning as error:
         #     _log(f"Warning: {error}","error")
         #     _log(_traceback.format_exc(),"error")
 
         # except sqlite3.OperationalError as error:
@@ -434,14 +436,25 @@
 
         except AttributeError:
             _log(f"{_traceback.format_exc()}\n","error")
             _log(f"{print(sys.exc_info()[2])}\n\n","error")
             _log(f"SQL: \033[38;2;(235);(64);(52)m{sql}")
         return success
 
+    def _parse_interface_error(self,e):
+        if "duplicate" in e.msg.lower():
+            # Duplicate entry 'act_succesboobers' for key 'uq_hash_id'
+            raise _e.DuplicateEntryError(e)
+        # print(f"error:{e}")
+        # print(f"e.args: {e.args}")
+        # print(f"e.errno: {e.errno}")
+        # print(f"e.msg: {e.msg}")
+        # print(f"e.sqlstate: {e.sqlstate}")
+        
+
     def run_from_list(self, query_list,**kwargs):
         '''
             Execute SQL statements from a list.
 
             ----------
 
             Arguments
```

### Comparing `colemen_volent-0.0.5/volent/mixins/EntityName.py` & `colemen_volent-0.0.6/volent/mixins/EntityName.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/mixins/MySQLGeneratorMixin.py` & `colemen_volent-0.0.6/volent/mixins/MySQLGeneratorMixin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
 
 from dataclasses import dataclass
 from string import Template
-from typing import Iterable
+from typing import Iterable, Union
 # from typing import Iterable
 
 import colemen_utils as c
 import sqlite3
 import mysql.connector as _mysqlConnnector
 
 
@@ -120,17 +120,14 @@
     def gen_quoted_name(self,table_name:str,database_name:str=None):
         if isinstance(database_name,(str)):
             database_name = f"{qc}{database_name}{qc}."
         else:
             database_name = ""
         value = f"{database_name}{qc}{table_name}{qc}"
         return value
-        
-
-
 
     @property
     def drop_statement(self):
         from volent.Database import Database as _database
         from volent.Model import Model as _model
 
         if isinstance(self,_database):
@@ -140,45 +137,45 @@
             exists = _gen_safe_script_exists()
             return f"DROP TABLE {exists}{self.quoted_name};"
 
     def gen_drop_table_statement(self,table_name,database_name:str=None):
         qn = self.gen_quoted_name(table_name,database_name)
         value = f"DROP TABLE IF EXISTS {qn}"
         return value
-        
+
 
     @property
     def create_statement(self):
         from volent.Database import Database as _database
         from volent.Model import Model as _model
         from volent.Column import Column as _column
         from volent.UniqueConstraint import UniqueConstraint as _unique_constraint
+        from volent.FullTextIndex import FullTextIndex as _full_text_index
         from volent.Relationship import Relationship as _relationship
 
 
         if isinstance(self,_database):
             exists = _gen_safe_script_not_exists()
             return f"CREATE SCHEMA {exists}{self.quoted_name};"
 
         if isinstance(self,_column):
             return _gen_column_declaration(self)
 
         if isinstance(self,_unique_constraint):
             return _gen_unique_constraint_create(self)
 
+        if isinstance(self,_full_text_index):
+            return _gen_full_text_index_create(self)
+
         if isinstance(self,_relationship):
             return _gen_relationship_create(self)
 
         if isinstance(self,_model):
             return _gen_table_create_statement(self)
 
-
-
-
-
     @property
     def show_columns(self):
         '''
             Get this MySQLGeneratorMixin's show_columns
 
             `default`:None
 
@@ -192,15 +189,14 @@
         '''
         
         from volent.Model import Model as _model
         if isinstance(self,_model):
             sql = f"SHOW FULL COLUMNS FROM {self.quoted_name}"
             return sql
 
-
     @property
     def describe(self):
         '''
             Get the 
 
             `default`:None
 
@@ -378,32 +374,59 @@
 
 
 # ---------------------------------------------------------------------------- #
 #                               UNIQUE CONSTRAINT                              #
 # ---------------------------------------------------------------------------- #
 
 
-_UNIQUE_CONSTRAINT_TEMPLATE = '''${indent}UNIQUE KEY $name ($columns)$comment'''
+_UNIQUE_CONSTRAINT_TEMPLATE = '''${indent}UNIQUE KEY $name ($columns) $comment'''
 def _gen_unique_constraint_create(u:_t.unique_constraint_type)->str:
     s = Template(_UNIQUE_CONSTRAINT_TEMPLATE)
-    col_list = []
-    for col in u.columns:
-        col_list.append(col.quoted_name)
-    columns = ','.join(col_list)
-
+    # col_list = []
+    # for col in u.columns:
+    #     col_list.append(col.quoted_name)
+    # columns = ','.join(col_list)
+    columns = __quoted_col_name_list(u)
+    # comment = _gen_column_comment(u.comment) or ""
+    # if len(comment) > 0:
+    #     comment = f" {comment}"
     val = s.substitute(
         indent=indent,
         name=u.quoted_name,
         columns=columns,
         comment=_gen_column_comment(u.comment) or ""
     )
+    val = c.string.strip(val,[" "],"right")
     return val
 
+# ---------------------------------------------------------------------------- #
+#                               INDEX GENERATORS                               #
+# ---------------------------------------------------------------------------- #
+
+_FULLTEXT_TEMPLATE = '''${indent}FULLTEXT ($columns)'''
+def _gen_full_text_index_create(ft:_t.full_text_index_type)->str:
+    s = Template(_FULLTEXT_TEMPLATE)
+    # col_list = []
+    # for col in ft.columns:
+    #     col_list.append(col.quoted_name)
+    # columns = ','.join(col_list)
+    columns = __quoted_col_name_list(ft)
 
+    val = s.substitute(
+        indent=indent,
+        columns=columns,
+    )
+    return val
 
+def __quoted_col_name_list(entity:Union[_t.unique_constraint_type,_t.full_text_index_type]):
+    col_list = []
+    for col in entity.columns:
+        col_list.append(col.quoted_name)
+    columns = ','.join(col_list)
+    return columns
 
 # ---------------------------------------------------------------------------- #
 #                            FOREIGN KEY GENERATORS                            #
 # ---------------------------------------------------------------------------- #
 
 
 _RELATIONSHIP_TEMPLATE = '''${indent}KEY ${qc}$fk_name${qc} ($child_column_name),
@@ -416,15 +439,16 @@
         on_update = f" ON UPDATE {r.on_update}"
     if r.on_delete is not None:
         on_delete = f" ON DELETE {r.on_delete}"
     s = Template(_RELATIONSHIP_TEMPLATE)
     december= s.substitute(
         indent=indent,
         qc=qc,
-        fk_name=f"FK_{c.rand.rand()}",
+        # fk_name=f"FK_{c.rand.rand()}",
+        fk_name=r.fk_name,
         child_column_name=r.child_column.quoted_name,
         relationship_name=r.quoted_name,
         parent_table=r.parent_model.quoted_name,
         parent_column=r.parent_column.quoted_name,
         on_delete=on_delete,
         on_update=on_update,
     )
@@ -490,14 +514,23 @@
     uqs = []
     uc = model.unique_constraints
     if isinstance(uc,(list)):
         for u in uc:
             uqs.append(u.create_statement)
     return uqs
 
+def _gen_fulltext_indexes(model:_t.model_type)->Iterable[str]:
+    '''Generates a list of fulltext index statements for a table'''
+    ftis = []
+    fts = model.full_text_indexes
+    if isinstance(fts,(list)):
+        for ft in fts:
+            ftis.append(ft.create_statement)
+    return ftis
+
 def _gen_relationship_decs(model:_t.model_type)->Iterable[str]:
     '''Generates a list of foreign key statements for a table'''
     value = []
     rels = model.relationships
     if isinstance(rels,(list)):
         for r in rels:
             value.append(r.create_statement)
@@ -530,14 +563,15 @@
         `method_name`: _gen_table_create_contents
         * @xxx [03-25-2023 08:28:07]: documentation for _gen_table_create_contents
     '''
     value = []
     value = c.arr.append(value,_gen_table_create_columns(model),skip_nulls=True)
     value = c.arr.append(value,_gen_primary_columns(model),skip_nulls=True)
     value = c.arr.append(value,_gen_unique_constraints(model),skip_nulls=True)
+    value = c.arr.append(value,_gen_fulltext_indexes(model),skip_nulls=True)
     value = c.arr.append(value,_gen_relationship_decs(model),skip_nulls=True)
 
     value = c.arr.strip_list_nulls(value)
 
     return ',\n'.join(value)
```

### Comparing `colemen_volent-0.0.5/volent/mixins/OrderedClass.py` & `colemen_volent-0.0.6/volent/mixins/OrderedClass.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/query/Insert.py` & `colemen_volent-0.0.6/volent/query/Update.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,154 +13,170 @@
 
 import volent.settings.types as _t
 import volent.settings as _settings
 from volent.Field import Field as _field
 # from volent.Relationship import Relationship as _relationship
 # from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 from volent.query.Query import Query
+from volent.query.WhereMixin import WhereMixin
 
 
 @dataclass
-class Insert(Query):
-    def __init__(self,model:_t.model_type,data:dict) -> None:
-        self._inserts = {}
-        super().__init__(model,data)
+class Update(Query,WhereMixin):
+    def __init__(self,model:_t.model_type,columns=None) -> None:
+        self._params = {}
+        self._updates = []
+        self.limit = 100
+        self.offset = 0
 
-    @property
-    def query(self):
-        if isinstance(self.data,(dict)) is False:
-            raise ValueError("Data should be a dictionary.")
-        data = self._inserts_from_data()
-        # data = self.data
-        if len(list(self._inserts.keys())) == 0:
-            return (False,False)
-
-
-        # # data = self.filter_dict_by_columns(data)
-        # column_list = ', '.join(list(data.keys()))
-        # # total_keys = len(list(data.keys()))
-        # ph = []
-        # for k in list(data.keys()):
-        #     ph.append(f"%({k})s")
-        # placeholders = ', '.join(ph)
-        template = f"""INSERT INTO {self.model.quoted_name} ({self.column_list_string}) VALUES ({self.placeholder_string})"""
-        # data_tuple = data.values()
-        # print(f"template: {template}")
-        # print(f"data_tuple: {data_tuple}")
-        return (template,data)
+        self.query_crud_type = "update"
+        super().__init__(model,update_columns=columns)
 
     @property
-    def placeholder_string(self)->str:
+    def select_string(self)->str:
         '''
-            Get this Insert's placeholder_string
-
-            This is the list of value placeholders used to parameterize the query.
-
-            "%(beep)s,%(boop)s"
+            Get the compiled select string for this query.
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
-            `@created`: 04-26-2023 11:15:02
-            `@memberOf`: Insert
-            `@property`: placeholder_string
-        '''
-        ph = []
-        for k in list(self._inserts.keys()):
-            ph.append(f"%({k})s")
-        return ', '.join(ph)
+            `@created`: 12-09-2022 15:56:15
+            `@memberOf`: SelectQuery
+            `@property`: select_string
+        '''
+        if len(self._selects) == 0:
+            value = "*"
+        else:
+            selects = []
+            for sel in self._selects:
+                value = None
+                if sel['alias'] is not None:
+                    value = f"{sel['column_name']} as {sel['alias']}"
+                else:
+                    value = f"{sel['column_name']}"
+                if value is not None:
+                    selects.append(value)
+            value = ', '.join(selects)
+
+        if self._count is True:
+            value = f"COUNT({value})"
+        if self._average is True:
+            value = f"AVG({value})"
+        if self.sum_ is True:
+            value = f"SUM({value})"
         return value
 
+
     @property
-    def column_list_string(self):
-        '''
-            Get this Insert's column_list_string
+    def query(self):
 
-            `default`:None
 
+        value = f"UPDATE {self.model.quoted_name} SET {self.update_string}{self.where_string}"
 
-            Meta
+        value = self._paginate_select_query(value)
+        value = self._format_query_params(value,self._params)
+        return value,self._params
+        # return value,self._params
+
+    def execute(
+        self,
+        foreign_key_checks:bool=True
+        )->Union[bool,dict,int]:
+        '''
+            Execute this update operation on the model.
+            
             ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-26-2023 11:13:45
-            `@memberOf`: Insert
-            `@property`: column_list_string
-        '''
-        return ', '.join(list(self._inserts.keys()))
-
-    # @property
-    # def query(self):
-    #     data = self.data
-
-    #     if isinstance(data,(dict)) is False:
-    #         raise ValueError("Data should be a dictionary.")
-
-    #     data = self.filter_dict_by_columns(data)
-    #     if len(list(data.keys())) == 0:
-    #         return (False,False)
-    #     column_list = ', '.join(list(data.keys()))
-    #     # total_keys = len(list(data.keys()))
-    #     ph = []
-    #     for k in list(data.keys()):
-    #         ph.append(f"%({k})s")
-    #     placeholders = ', '.join(ph)
-    #     template = f"""INSERT INTO {self.model.quoted_name} ({column_list}) VALUES ({placeholders})"""
-    #     # data_tuple = data.values()
-    #     # print(f"template: {template}")
-    #     # print(f"data_tuple: {data_tuple}")
-    #     return (template,data)
-    #     # return (template,data_tuple)
-
-
-    def _inserts_from_data(self):
-        data = self.data
-        data = self.filter_dict_by_columns(data)
-        for k,v in data.items():
-            if v != _t.undefined:
-                self.add_insert(k,v)
-        for col in self.model.columns:
-            if col.on_insert != _t.undefined:
-                if col.name not in self._inserts:
-                    self.add_insert(col.name,col.on_insert)
-        return self._inserts
 
-    def add_insert(self,column_name,value):
-        self._inserts[column_name] = value
+            Arguments
+            -------------------------
 
+            [`foreign_key_checks`=True] {bool}
+                If False, the query will not perform foreign key checks before executing the update.
+                Be careful, this can cause integrity issues and will NOT warn you about it.
 
 
+            Return {type}
+            ----------------------
+            return_description
 
-    def execute(self)->Union[bool,dict,int]:
-
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 08:01:22
+            `memberOf`: Update
+            `version`: 1.0
+            `method_name`: execute
+            * @TODO []: documentation for execute
+        '''
         sql,args= self.query
+
         if sql is False:
             return False
 
-        print(f"sql:{sql}")
-        print(f"args:{args}")
+        # print(f"sql:{sql}")
+        # print(f"args:{args}")
 
-        # @Mstep [] execute the insert query.
-        result = self.database.run(sql,args)
-        # @Mstep [IF] if the query was successful.
-        if result is True:
-            # @Mstep [] get the id of the inserted role.
-            result = self.database.last_id()
-            self.model.primary_column.value = result
+        # @Mstep [] execute the update query.
+        result = self.database.run(sql,args,foreign_key_checks=foreign_key_checks)
+        # @Mstep [] select the updated row as a dictionary.
+        data = self.model.select().add_where_from_wheres(self._wheres).execute(return_models=False)
+        data = data[0]
+        # @Mstep [LOOP] iterate the dictionary.
+        for k,v in data.items():
+            # @Mstep [] retrieve the column with a matching name from the model.
+            col = self.model.get_column(k)
+            col.value = v
             self.model._saved = True
-            # result = self.model.select().is_(self.model.primary_column.name,result).execute()
+        return data
+        models = []
+        for r in result:
+            mdl = self.model.__class__(**r)
+            mdl.__doc__ = self.model.__doc__
+            mdl._name = self.model.name
+            mdl._database_name = self.model._database_name
+            mdl._database = self.model._database
+            models.append(mdl)
+        return models
+        return result
 
-            # if self.return_row is True:
-            #     query = f"""SELECT * FROM {self.model.quoted_name} WHERE {self.model.primary_column.name}={result}"""
-            #     # s = self.model.select_query()
-
-            #     # s.correlate_to_table = False
-            #     # s.add_where(self.table.primary_id.name,result,"=")
-            #     # row = s.execute()
-            #     if isinstance(row,(list)):
-            #         result = row[0]
 
-        # print(f"sql: {sql}")
-        # print(f"args: {args}")
-        return result
+
+    @property
+    def update_string(self):
+        '''
+            Get this UpdateQuery's update_string
+
+            `default`:None
+
+
+            Meta
+            ----------
+            `@author`: Colemen Atwood
+            `@created`: 12-09-2022 15:56:15
+            `@memberOf`: UpdateQuery
+            `@property`: update_string
+        '''
+        if len(self._updates) == 0:
+            return None
+        else:
+            selects = []
+            for k,v in self._updates.items():
+                value = None
+                value = f"{k}=:{k}"
+                self._params[k] = v
+                selects.append(value)
+            value = ', '.join(selects)
+
+        return value
+
+    def add_update(self,column_name:str,value):
+        self._updates[column_name] = value
+
+
+def format_null(value):
+    if value is None:
+        return "NULL"
+    return value
+
```

### Comparing `colemen_volent-0.0.5/volent/query/Query.py` & `colemen_volent-0.0.6/volent/query/Query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+'''
+    The Query module
+
+    ----------
+
+    Meta
+    ----------
+    `author`: Colemen Atwood
+    `created`: 04-28-2023 07:04:20
+    `name`: query
+    * @xxx [04-28-2023 07:04:34]: documentation for query
+'''
+
 
 
 from dataclasses import dataclass
 import re
-from typing import Iterable,OrderedDict, Union
+from typing import Iterable, Union
 from datetime import datetime
 from datetime import timezone
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
-import volent.settings as _settings
-from volent.Field import Field as _field
-# from volent.Relationship import Relationship as _relationship
-# from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
-from volent.mixins import MySQLGeneratorMixin,OrderedClass
-# from collections import OrderedClass
-
-
-
-# class OrderedClass(type):
-#     @classmethod
-#     def __prepare__(mcs, name, bases):
-#         return OrderedDict()
-
-#     def __new__(cls, name, bases, classdict):
-#         result = type.__new__(cls, name, bases, dict(classdict))
-#         result.__fields__ = list(classdict.keys())
-#         return result
+# import volent.settings as _settings
+# from volent.Field import Field as _field
+from volent.mixins import OrderedClass
 
 
 @dataclass
 class Query(metaclass=OrderedClass):
     main = None
     # database:_t.database_type = None
     model:_t.model_type = None
@@ -55,14 +53,40 @@
     def __init__(
         self,
         model:_t.model_type,
         data:dict=None,
         select_columns=None,
         update_columns=None
         ):
+        '''
+            Create a new query instance.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `model` {model}
+                The model instance that this query will act on.
+            `data` {dict}
+                A dictionary of data that is used in the query operation.
+            `select_columns` {list}
+                A list of column names or column instances that should be "selected" in a select query
+            `update_columns` {list}
+                A list of column names or column instances that should be updated in an update query
+
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:04:55
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: query
+            * @xxx [04-28-2023 07:07:59]: documentation for query
+        '''
         self.model = model
         self.data = data
         self.database = model.database
         self._wheres = []
         self._selects = []
         self._updates = {}
 
@@ -74,15 +98,46 @@
         #                 name,value = col
         #                 self.add_update(name,value)
             #     if len(col) == 1:
             #         col = col[0]
             # if isinstance(col,(str)):
             #     self.add_select(col)
 
-    def __parse_col_data(self,select_columns,update_columns):
+    def __parse_col_data(
+        self,
+        select_columns:Iterable[Union[str,_t.column_type]],
+        update_columns:Iterable[Union[str,_t.column_type]]
+        ):
+        '''
+            Parse the select and update columns into this query for later use.
+
+            Essentially take a bunch of column names/instances and store them in a useful way.
+            ----------
+
+            Arguments
+            -------------------------
+            `select_columns` {list}
+                A list of column names or column instances that should be "selected" in a select query
+
+            `update_columns` {list}
+                A list of column names or column instances that should be updated in an update query
+
+            Return
+            ----------------------
+            Doesn't return shit.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:08:04
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: __parse_col_data
+            * @xxx [04-28-2023 07:10:20]: documentation for __parse_col_data
+        '''
         if isinstance(select_columns,(list)):
             for col in select_columns:
                 if isinstance(col,(list,tuple)):
                     if len(col) >= 2:
                         name,alias = col
                         self.add_select(name,alias)
                     if len(col) == 1:
@@ -110,25 +165,110 @@
                 if col.on_update != _t.undefined:
                     # @Mstep [IF] if the column is not already being updated.
                     if col.name not in self._updates:
                         # @Mstep [] add a new update clause to this query.
                         self.add_update(col.name,col.on_update)
 
     def filter_dict_by_columns(self,data:dict)->dict:
+        '''
+            Iterate a dictionary to remove key's that do not have a corresponding column in this query's model
+            ----------
+
+            Arguments
+            -------------------------
+            `data` {dict}
+                The dictionary to filter.
+
+            Return {dict}
+            ----------------------
+            The dictionary with only keys that match a column.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:10:41
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: filter_dict_by_columns
+            * @xxx [04-28-2023 07:11:51]: documentation for filter_dict_by_columns
+        '''
         output = {}
         for k,v in data.items():
             col = self.model.get_column(k)
             if col is not None:
                 if v is None and col.nullable is False:
                     continue
                 output[k] = v
         return output
 
+    def sort_dict_by_columns(self,data:dict)->dict:
+        '''
+            Sort the keys of dictionary to match the order of columns in this query's model.
+            
+            This is primarily useful for parameterized insert statements, where the order of the columns
+            is critical to inserting the correct data.
+            
+            This will sort them into the same order that the columns were declared in.
+            
+            ----------
+
+            Arguments
+            -------------------------
+            `data` {dict}
+                The dictionary to sort.
+
+
+            Return {dict}
+            ----------------------
+            The dictionary with all keys reordered to match the model's columns.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:11:58
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: sort_dict_by_columns
+            * @xxx [04-28-2023 07:13:57]: documentation for sort_dict_by_columns
+        '''
+        output = {}
+        for col in self.model.columns:
+            if col.name in data:
+                output[col.name] = data[col.name]
+        return output
+
 
     def add_where(self,column_name,value,comparison):
+        '''
+            Add a where clause to this query.
+
+            ----------
+
+            Arguments
+            -------------------------
+            `column_name` {str}
+                The name of the column that this clause applies to.
+            `value` {any}
+                The value that the column is compared to
+            `comparison` {str}
+                The comparison/operator to use.
+
+            Return {type}
+            ----------------------
+            no returned value
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:14:41
+            `memberOf`: Query
+            `version`: 1.0
+            `method_name`: add_where
+            * @xxx [04-28-2023 07:19:24]: documentation for add_where
+        '''
         if value is None:
             value = "NULL"
         # self.wheres.append(f"{column_name} {comparison} {value}")
 
         if c.string.to_snake_case(comparison) in ["!","!=","isnt","isnot","is_not","<>"]:
             comparison = "is not"
 
@@ -167,17 +307,17 @@
 
                 data['value'] = items
 
         self._wheres.append(data)
 
 
     @property
-    def where_string(self):
+    def where_string(self)->str:
         '''
-            Get this UpdateQuery's where_string
+            Generate this query's where string.
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
@@ -295,15 +435,14 @@
             `memberOf`: QueryBase
             `version`: 1.0
             `method_name`: __paginate_select_query
             * @xxx [12-14-2022 11:46:12]: documentation for __paginate_select_query
         '''
         return _paginate_select_query(sql,self.limit,self.offset)
 
-
     def add_where_from_wheres(self,wheres:Iterable[dict]):
         for w in wheres:
             column_name = w["column_name"]
             value = w["value"]
             max_value = w["max_value"]
             comparison = w["comparison"]
 
@@ -328,14 +467,37 @@
 
 
 
 
 
 
 def format_null(value):
+    '''
+        convert a None value to a "null" string.
+
+        ----------
+
+        Arguments
+        -------------------------
+        `value` {any}
+            The value to test.
+
+        Return {any}
+        ----------------------
+        "NULL" if the value is None, the original value otherwise.
+
+        Meta
+        ----------
+        `author`: Colemen Atwood
+        `created`: 04-28-2023 07:20:50
+        `memberOf`: Query
+        `version`: 1.0
+        `method_name`: format_null
+        * @xxx [04-28-2023 07:22:36]: documentation for format_null
+    '''
     if value is None:
         return "NULL"
     return value
```

### Comparing `colemen_volent-0.0.5/volent/query/Select.py` & `colemen_volent-0.0.6/volent/query/Delete.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,68 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+'''
+    The query delete module.
+
+    ----------
+
+    Meta
+    ----------
+    `author`: Colemen Atwood
+    `created`: 04-28-2023 07:24:17
+    `name`: delete
+    * @xxx [04-28-2023 07:24:33]: documentation for delete
+'''
+
 
 
 from dataclasses import dataclass
-from typing import Iterable,OrderedDict, Union
+from typing import Iterable, Union
 
 
 import colemen_utils as c
 
 
 import volent.settings.types as _t
-import volent.settings as _settings
-from volent.Field import Field as _field
+# import volent.settings as _settings
+# from volent.Field import Field as _field
 # from volent.Relationship import Relationship as _relationship
 # from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
 from volent.query.Query import Query
 from volent.query.WhereMixin import WhereMixin
-from mysql.connector.errors import OperationalError,InterfaceError
 
-@dataclass
-class Select(Query,WhereMixin):
-    def __init__(self,model:_t.model_type,columns=None,limit:int=100,offset:int=0) -> None:
-        self._params = {}
-        self._selects = []
-        self._joins = []
-        self._limit = limit
-        self._offset = offset
-
-        self.query_crud_type = "read"
-        super().__init__(model,select_columns=columns)
-
-    def paginate(self,limit,offset):
-        self.limit = limit
-        self.offset = offset
-        return self
 
-    @property
-    def limit(self):
-        return self._limit
-    @limit.setter
-    def limit(self,value:int):
+@dataclass
+class Delete(Query,WhereMixin):
+    def __init__(self,model:_t.model_type) -> None:
         '''
-            Set the Select's limit property
+            Create a delete query instance.
 
-            `default`:None
-
-
-            Meta
             ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-21-2023 10:14:11
-            `@memberOf`: Select
-            `@property`: limit
-        '''
-        self._limit = value
-
-    @property
-    def offset(self):
-        return self._offset
-    @offset.setter
-    def offset(self,value:int):
-        '''
-            Set the Select's offset property
-
-            `default`:None
 
+            Arguments
+            -------------------------
+            `model` {model}
+                The model instance to execute a delete operation on.
 
             Meta
             ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-21-2023 10:14:11
-            `@memberOf`: Select
-            `@property`: offset
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:24:53
+            `memberOf`: Delete
+            `version`: 1.0
+            `method_name`: Delete
+            * @xxx [04-28-2023 07:26:55]: documentation for Delete
         '''
-        self._offset = value
+        self._params = {}
+
+        self.query_crud_type = "delete"
+        super().__init__(model)
 
     @property
     def select_string(self)->str:
         '''
             Get the compiled select string for this query.
 
             `default`:None
@@ -112,133 +95,77 @@
             value = f"AVG({value})"
         if self.sum_ is True:
             value = f"SUM({value})"
         return value
 
 
     @property
-    def query(self):
+    def query(self)->tuple:
+        '''
+            Generate this delete query's SQL.
 
-        # print(f"self.select_string: {self.select_string}")
+            ----------
 
-        value = f"""SELECT {self.select_string} FROM {self.model.quoted_name}{self.where_string}"""
+            Return {tuple}
+            ----------------------
+            A tuple containing the query string and a dictionary of query params.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 07:27:18
+            `memberOf`: Delete
+            `version`: 1.0
+            `method_name`: query
+            * @xxx [04-28-2023 07:33:51]: documentation for query
+        '''
+
+        value = f"DELETE {self.model.quoted_name} {self.where_string}"
 
         value = self._paginate_select_query(value)
         value = self._format_query_params(value,self._params)
-        # print(f"value: {value}")
-        # print(f"self._params: {self._params}")
         return value,self._params
+        # return value,self._params
 
-    def execute(self,return_models=True)->Union[bool,dict,int,_t.model_type]:
-    # def execute(self)->Union[bool,dict,int]:
-        # _mysql_connector.MySQLInterfaceError: Lost connection to MySQL server during query
-        sql,args= self.query
-
-        if sql is False:
-            return False
-
-        # print(f"sql:{sql}")
-        # print(f"args:{args}")
-        try:
-            # @Mstep [] execute the insert query.
-            result = self.database.run_select(sql,args)
-            if return_models:
-                models = []
-                for r in result:
-                    mdl = self.model.__class__(**r)
-                    mdl.__doc__ = self.model.__doc__
-                    mdl._name = self.model.name
-                    mdl._database_name = self.model._database_name
-                    mdl._database = self.model._database
-                    models.append(mdl)
-                return models
-        except OperationalError as e:
-            c.con.log(e,"red")
-        except InterfaceError as e:
-            c.con.log(e,"red")
-        return result
-
-    def count(self)->_t.query_type:
-        self._count = True
-        return self
-
-    def average(self)->_t.query_type:
-        self._average = True
-        return self
-
-    def sum_(self)->_t.query_type:
-        self._sum = True
-        return self
-
-    def add_select(self,column_name,alias=None)->_t.query_type:
+    def execute(self,foreign_key_checks:bool=True)->Union[bool,dict,int]:
         '''
-            Add a column to the selection of this query.
+            Execute the delete operation on the model.
 
-            By default "*" is used to select all columns if None are specified.
             ----------
 
             Arguments
             -------------------------
-            `column_name` {str}
-                The name of the column to select
-            [`alias`=None] {str}
-                An alias to use for this column
+            [`foreign_key_checks`=True] {bool}
+                If False, the query will not perform foreign key checks before executing the deletion.
+                Be careful, this can cause integrity issues and will NOT warn you about it.
 
-            Return {None}
+
+            Return {bool}
             ----------------------
-            returns nothing
+            True if execution was successful,False otherwise.
+
 
             Meta
             ----------
             `author`: Colemen Atwood
-            `created`: 12-13-2022 12:04:31
-            `memberOf`: SelectQuery
+            `created`: 04-28-2023 07:34:05
+            `memberOf`: Delete
             `version`: 1.0
-            `method_name`: add_select
-            * @xxx [12-13-2022 12:06:00]: documentation for add_select
+            `method_name`: execute
+            * @xxx [04-28-2023 07:40:57]: documentation for execute
         '''
-        if self.model is not None:
-            if self.model.get_column(column_name) is None:
-                c.con.log(f"Column {column_name} does not exist in table: {self.model.name}","warning")
-                return
-        data = {
-            "column_name":column_name,
-            "alias":alias,
-        }
-        self._selects.append(data)
-        return self
-
-    def left_join(self,table_name:str,column_name:str):
-        data = {
-            "join_type":"LEFT",
-            "table_name":table_name,
-            "column_name":column_name,
-        }
-        self._joins.append(data)
 
+        sql,args= self.query
 
-    @property
-    def left_join_string(self):
-        '''
-            Get this Select's left_join_string
-
-            `default`:None
-
+        if sql is False:
+            return False
+        # @Mstep [] execute the delete query.
+        result = self.database.run(sql,args,foreign_key_checks=foreign_key_checks)
+        return result
 
-            Meta
-            ----------
-            `@author`: Colemen Atwood
-            `@created`: 04-21-2023 08:58:54
-            `@memberOf`: Select
-            `@property`: left_join_string
-        '''
-        out_list = []
-        for join in self._joins:
-            template = f"""{join['join_type']} JOIN {join['table_name']}
-    ON {self.model.name}.{join['table_name']} = {join['table_name']}.{join['table_name']}"""
 
 
 
 def format_null(value):
     if value is None:
         return "NULL"
     return value
```

### Comparing `colemen_volent-0.0.5/volent/query/Update.py` & `colemen_volent-0.0.6/volent/Relationship.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,151 +1,167 @@
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 # pylint: disable=line-too-long
 # pylint: disable=unused-import
+'''
+    The relationship module.
 
+    ----------
 
-from dataclasses import dataclass
-from typing import Iterable,OrderedDict, Union
+    Meta
+    ----------
+    `author`: Colemen Atwood
+    `created`: 04-28-2023 10:06:56
+    `name`: relationship
+    * @xxx [04-28-2023 10:07:06]: documentation for relationship
+'''
 
 
+from dataclasses import dataclass
+from typing import Iterable, Union
 import colemen_utils as c
-
-
-import volent.settings.types as _t
 import volent.settings as _settings
-from volent.Field import Field as _field
-# from volent.Relationship import Relationship as _relationship
-# from volent.UniqueConstraint import UniqueConstraint as _uniqueConstraint
-from volent.query.Query import Query
-from volent.query.WhereMixin import WhereMixin
+import volent.settings.types as _t
 
+from volent.mixins.MySQLGeneratorMixin import MySQLGeneratorMixin
 
 @dataclass
-class Update(Query,WhereMixin):
-    def __init__(self,model:_t.model_type,columns=None) -> None:
-        self._params = {}
-        self._updates = []
-        self.limit = 100
-        self.offset = 0
+class Relationship(MySQLGeneratorMixin):
+    main:_t._main_type = None
+    # database:_t.database_type = None
+    model:_t.model_type = None
+    name:str = None
+    '''The name of this relationship'''
+    on_delete:str = None
+    '''The action to perform with the parent is deleted'''
+    on_update:str = None
+    '''The action to perform with the parent is updated'''
+    fk_name:str = None
+    '''The name used to uniquely identify this relationship in the database.'''
+
+    # _parent_database_name:str = None
+    # _parent_model_name:str = None
+    # _parent_column_name:str = None
+
+    parent_model:_t.model_type = None
+    '''A reference to the parent model instance'''
+    parent_column:_t.column_type = None
+    '''A reference to the parent model's column instance'''
+
+    child_model:_t.model_type = None
+    '''A reference to the child model instance'''
+    child_column:_t.model_type = None
+    '''A reference to the child model's column instance'''
+    # schemas:Iterable[_t.schema_type] = None
 
-        self.query_crud_type = "update"
-        super().__init__(model,update_columns=columns)
 
-    @property
-    def select_string(self)->str:
+
+    def __init__(
+        self,
+        child:Union[str,_t.column_type],
+        parent:str,
+        name:str=None,
+        on_delete:str = None,
+        on_update:str = None,
+        fk_name:str = None,
+        ):
         '''
-            Get the compiled select string for this query.
+            Create a relationship instance.
 
-            `default`:None
+            ----------
 
+            Arguments
+            -------------------------
+            `child` {column}
+                The child column of this relationship
 
-            Meta
-            ----------
-            `@author`: Colemen Atwood
-            `@created`: 12-09-2022 15:56:15
-            `@memberOf`: SelectQuery
-            `@property`: select_string
-        '''
-        if len(self._selects) == 0:
-            value = "*"
-        else:
-            selects = []
-            for sel in self._selects:
-                value = None
-                if sel['alias'] is not None:
-                    value = f"{sel['column_name']} as {sel['alias']}"
-                else:
-                    value = f"{sel['column_name']}"
-                if value is not None:
-                    selects.append(value)
-            value = ', '.join(selects)
-
-        if self._count is True:
-            value = f"COUNT({value})"
-        if self._average is True:
-            value = f"AVG({value})"
-        if self.sum_ is True:
-            value = f"SUM({value})"
-        return value
+            `parent` {str}
+                The name (dot path) of the parent column that this relationship represents.
 
+                "tasks.task_id"
 
-    @property
-    def query(self):
+            [`name`=None] {str}
+                The name of this relationship, if not provided, the variable name is used from its declaration
+                in the model.
+
+            [`on_delete`=None] {str}
+                The action to perform when the parent row is deleted.
 
+            [`on_update`=None] {str}
+                The action to perform when the parent row is updated.
 
-        value = f"UPDATE {self.model.quoted_name} SET {self.update_string}{self.where_string}"
+            [`fk_name`=None] {str}
+                The name used to uniquely identify this relationship in the database.
+                If not provided, a random one will be generated.
+
+            Meta
+            ----------
+            `author`: Colemen Atwood
+            `created`: 04-28-2023 10:07:32
+            `memberOf`: Relationship
+            `version`: 1.0
+            `method_name`: relationship
+            * @xxx [04-28-2023 10:11:24]: documentation for relationship
+        '''
+        self.name = name
+        self.on_delete = on_delete
+        self.on_update = on_update
+        self.parent = parent
+        self.child_column = child
+        self.fk_name = f"FK_{c.rand.rand()}" if fk_name is None else fk_name
 
-        value = self._paginate_select_query(value)
-        value = self._format_query_params(value,self._params)
-        return value,self._params
-        # return value,self._params
-
-    def execute(self)->Union[bool,dict,int]:
-
-        sql,args= self.query
-
-        if sql is False:
-            return False
-
-        # print(f"sql:{sql}")
-        # print(f"args:{args}")
-
-        # @Mstep [] execute the update query.
-        result = self.database.run(sql,args)
-        data = self.model.select().add_where_from_wheres(self._wheres).execute(return_models=False)
-        data = data[0]
-        for k,v in data.items():
-            col = self.model.get_column(k)
-            col.value = v
-            self.model._saved = True
-        return data
-        models = []
-        for r in result:
-            mdl = self.model.__class__(**r)
-            mdl.__doc__ = self.model.__doc__
-            mdl._name = self.model.name
-            mdl._database_name = self.model._database_name
-            mdl._database = self.model._database
-            models.append(mdl)
-        return models
-        return result
 
 
 
     @property
-    def update_string(self):
+    def summary(self):
         '''
-            Get this UpdateQuery's update_string
+            Get this Relationship's summary
 
             `default`:None
 
 
             Meta
             ----------
             `@author`: Colemen Atwood
-            `@created`: 12-09-2022 15:56:15
-            `@memberOf`: UpdateQuery
-            `@property`: update_string
+            `@created`: 03-23-2023 14:53:39
+            `@memberOf`: Relationship
+            `@property`: summary
         '''
-        if len(self._updates) == 0:
-            return None
-        else:
-            selects = []
-            for k,v in self._updates.items():
-                value = None
-                value = f"{k}=:{k}"
-                self._params[k] = v
-                selects.append(value)
-            value = ', '.join(selects)
-
+        value = {
+            "name":self.name,
+            "fk_name":self.fk_name,
+            "on_delete":self.on_delete,
+            "on_update":self.on_update,
+            "parent_model":self.parent_model.name,
+            "parent_column":self.parent_column.name,
+            "child_model":self.child_model.name,
+            "child_column":self.child_column.name,
+            "parent_string":self.parent,
+        }
         return value
 
-    def add_update(self,column_name:str,value):
-        self._updates[column_name] = value
+
+    # def locate_parent(self):
+    #     database = self._parent_database_name
+    #     model = self._parent_model_name
+    #     column = self._parent_column_name
+    #     if database is not None:
+    #         self.main
+
+
+
 
 
-def format_null(value):
-    if value is None:
-        return "NULL"
-    return value
 
+# def _parse_parent(relationship:Relationship,value):
+#     value = c.string.strip_excessive_chars(value,["."])
+#     pl = value.split(".")
+#     if len(pl) == 3:
+#         relationship._parent_database_name = pl[0]
+#         relationship._parent_model_name = pl[1]
+#         relationship._parent_column_name = pl[2]
+#     if len(pl) == 2:
+#         relationship._parent_model_name = pl[0]
+#         relationship._parent_column_name = pl[1]
+#     if len(pl) == 1:
+#         relationship._parent_column_name = pl[0]
```

### Comparing `colemen_volent-0.0.5/volent/settings/control.py` & `colemen_volent-0.0.6/volent/settings/control.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/settings/types.py` & `colemen_volent-0.0.6/volent/settings/types.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 type_base_type = None
 query_type = None
 
 relationship_type = None
 schema_type = None
 field_type = None
 unique_constraint_type = None
+full_text_index_type = None
 
 
 
 if TYPE_CHECKING:
 
     from volent.Volent import Volent as _m
     _main_type = _TypeVar('_main_type', bound=_m)
@@ -50,14 +51,17 @@
     from volent.UniqueConstraint import UniqueConstraint as _xbst
     unique_constraint_type = _TypeVar('unique_constraint_type', bound=_xbst)
 
 
     from volent.query.Query import Query as _PsBw
     query_type = _TypeVar('query_type', bound=_PsBw)
 
+    from volent.FullTextIndex import FullTextIndex as _eMkA
+    full_text_index_type = _TypeVar('full_text_index_type', bound=_eMkA)
+
 
 class NoDefault:
     def __init__(self, value):
         self.value = value
 
     def __str__(self):
         return self.value
```

### Comparing `colemen_volent-0.0.5/volent/tests/schema_dict_test.py` & `colemen_volent-0.0.6/volent/tests/schema_dict_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/tests/validators_test.py` & `colemen_volent-0.0.6/volent/tests/validators_test.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/CreditCardNumber.py` & `colemen_volent-0.0.6/volent/validate/CreditCardNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Email.py` & `colemen_volent-0.0.6/volent/validate/Email.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Equal.py` & `colemen_volent-0.0.6/volent/validate/Equal.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/FutureUnixDate.py` & `colemen_volent-0.0.6/volent/validate/FutureUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/IpAddress.py` & `colemen_volent-0.0.6/volent/validate/IpAddress.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Length.py` & `colemen_volent-0.0.6/volent/validate/Length.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/NoneOf.py` & `colemen_volent-0.0.6/volent/validate/NoneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/OneOf.py` & `colemen_volent-0.0.6/volent/validate/OneOf.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/PastUnixDate.py` & `colemen_volent-0.0.6/volent/validate/PastUnixDate.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/PhoneNumber.py` & `colemen_volent-0.0.6/volent/validate/PhoneNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Range.py` & `colemen_volent-0.0.6/volent/validate/Range.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Regex.py` & `colemen_volent-0.0.6/volent/validate/Regex.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/SocialSecurityNumber.py` & `colemen_volent-0.0.6/volent/validate/SocialSecurityNumber.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/StrongPassword.py` & `colemen_volent-0.0.6/volent/validate/StrongPassword.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/Validator.py` & `colemen_volent-0.0.6/volent/validate/Validator.py`

 * *Files identical despite different names*

### Comparing `colemen_volent-0.0.5/volent/validate/__init__.py` & `colemen_volent-0.0.6/volent/validate/__init__.py`

 * *Files identical despite different names*

