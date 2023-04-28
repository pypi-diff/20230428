# Comparing `tmp/openget-0.1.9.tar.gz` & `tmp/openget-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openget-0.1.9.tar", last modified: Wed Apr 12 11:17:24 2023, max compression
+gzip compressed data, was "openget-0.2.0.tar", last modified: Fri Apr 28 03:33:33 2023, max compression
```

## Comparing `openget-0.1.9.tar` & `openget-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.865245 openget-0.1.9/
--rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.1.9/LICENSE
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-12 11:17:24.865134 openget-0.1.9/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      505 2023-01-14 16:55:04.000000 openget-0.1.9/README.md
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.861880 openget-0.1.9/openget/
--rw-r--r--   0 dytttf     (501) staff       (20)       40 2023-04-12 11:16:05.000000 openget-0.1.9/openget/__init__.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.863428 openget-0.1.9/openget/db/
--rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db.py
--rw-r--r--   0 dytttf     (501) staff       (20)    17596 2023-04-12 11:15:21.000000 openget-0.1.9/openget/db/db_mysql.py
--rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_oracle.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38448 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_oss.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_redis.py
--rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/db_sqlite.py
--rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.1.9/openget/db/util.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1765 2023-01-14 16:55:04.000000 openget-0.1.9/openget/env.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864057 openget-0.1.9/openget/network/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    17631 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/downloader.py
--rw-r--r--   0 dytttf     (501) staff       (20)    25746 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/proxy.py
--rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/request.py
--rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.1.9/openget/network/response.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-01-14 16:55:04.000000 openget-0.1.9/openget/setting.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864501 openget-0.1.9/openget/spiders/
--rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)    15507 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/base.py
--rw-r--r--   0 dytttf     (501) staff       (20)    54681 2023-01-14 16:55:04.000000 openget-0.1.9/openget/spiders/batch_spider.py
--rw-r--r--   0 dytttf     (501) staff       (20)    38777 2023-01-14 16:55:04.000000 openget-0.1.9/openget/util.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864773 openget-0.1.9/openget/utils/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     2605 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/log.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.864966 openget-0.1.9/openget/utils/message/
--rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/message/__init__.py
--rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.1.9/openget/utils/message/dingtalk.py
-drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-12 11:17:24.862452 openget-0.1.9/openget.egg-info/
--rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/PKG-INFO
--rw-r--r--   0 dytttf     (501) staff       (20)      776 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/SOURCES.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        1 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/dependency_links.txt
--rw-r--r--   0 dytttf     (501) staff       (20)       89 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/requires.txt
--rw-r--r--   0 dytttf     (501) staff       (20)        8 2023-04-12 11:17:24.000000 openget-0.1.9/openget.egg-info/top_level.txt
--rw-r--r--   0 dytttf     (501) staff       (20)      810 2023-04-12 11:15:21.000000 openget-0.1.9/pyproject.toml
--rw-r--r--   0 dytttf     (501) staff       (20)       38 2023-04-12 11:17:24.865275 openget-0.1.9/setup.cfg
--rw-r--r--   0 dytttf     (501) staff       (20)     1017 2023-04-12 11:15:21.000000 openget-0.1.9/setup.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251543 openget-0.2.0/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1514 2022-07-21 15:26:26.000000 openget-0.2.0/LICENSE
+-rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-28 03:33:33.251421 openget-0.2.0/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      505 2023-01-14 16:55:04.000000 openget-0.2.0/README.md
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.247490 openget-0.2.0/openget/
+-rw-r--r--   0 dytttf     (501) staff       (20)       40 2023-04-28 03:29:34.000000 openget-0.2.0/openget/__init__.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.249649 openget-0.2.0/openget/db/
+-rw-r--r--   0 dytttf     (501) staff       (20)      125 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2327 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    20309 2023-04-28 03:29:34.000000 openget-0.2.0/openget/db/db_mysql.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    12619 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_oracle.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    38448 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_oss.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3229 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_redis.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    14416 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/db_sqlite.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      837 2023-01-14 16:55:04.000000 openget-0.2.0/openget/db/util.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1096 2023-04-28 03:29:34.000000 openget-0.2.0/openget/env.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.250282 openget-0.2.0/openget/network/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    17631 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/downloader.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    25752 2023-04-28 03:29:34.000000 openget-0.2.0/openget/network/proxy.py
+-rw-r--r--   0 dytttf     (501) staff       (20)      811 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/request.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     3533 2023-01-14 16:55:04.000000 openget-0.2.0/openget/network/response.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1354 2023-04-28 02:48:09.000000 openget-0.2.0/openget/setting.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.250636 openget-0.2.0/openget/spiders/
+-rw-r--r--   0 dytttf     (501) staff       (20)      522 2023-01-14 16:55:04.000000 openget-0.2.0/openget/spiders/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    15789 2023-04-28 03:29:34.000000 openget-0.2.0/openget/spiders/base.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    54681 2023-01-14 16:55:04.000000 openget-0.2.0/openget/spiders/batch_spider.py
+-rw-r--r--   0 dytttf     (501) staff       (20)    38777 2023-01-14 16:55:04.000000 openget-0.2.0/openget/util.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251034 openget-0.2.0/openget/utils/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     2605 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/log.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.251243 openget-0.2.0/openget/utils/message/
+-rw-r--r--   0 dytttf     (501) staff       (20)        0 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/message/__init__.py
+-rw-r--r--   0 dytttf     (501) staff       (20)     1842 2023-01-14 16:55:04.000000 openget-0.2.0/openget/utils/message/dingtalk.py
+drwxr-xr-x   0 dytttf     (501) staff       (20)        0 2023-04-28 03:33:33.248459 openget-0.2.0/openget.egg-info/
+-rw-r--r--   0 dytttf     (501) staff       (20)     1013 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/PKG-INFO
+-rw-r--r--   0 dytttf     (501) staff       (20)      776 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/SOURCES.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        1 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/dependency_links.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)      103 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/requires.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)        8 2023-04-28 03:33:33.000000 openget-0.2.0/openget.egg-info/top_level.txt
+-rw-r--r--   0 dytttf     (501) staff       (20)      810 2023-04-28 03:29:34.000000 openget-0.2.0/pyproject.toml
+-rw-r--r--   0 dytttf     (501) staff       (20)       38 2023-04-28 03:33:33.251574 openget-0.2.0/setup.cfg
+-rw-r--r--   0 dytttf     (501) staff       (20)     1042 2023-04-28 03:29:34.000000 openget-0.2.0/setup.py
```

### Comparing `openget-0.1.9/LICENSE` & `openget-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/PKG-INFO` & `openget-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openget-0.1.9/openget/db/db.py` & `openget-0.2.0/openget/db/db.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/db/db_mysql.py` & `openget-0.2.0/openget/db/db_mysql.py`

 * *Files 14% similar despite different names*

```diff
@@ -613,7 +613,103 @@
         options = self.options.copy()
         if protocol:
             assert protocol in ["mysql+pymysql", "mysql+mysqldb"]
             options["type"] = protocol
         #
         db_opt = MySQLOpt(options, **_kwargs)
         return db_opt
+
+    def create(
+        self,
+        fields: Dict[str, str] = None,
+        unique: List[str] = None,
+        table_name: str = "",
+        type="",
+        exists_ok=True,
+        sql="",
+        **kwargs,
+    ):
+        """
+            create table
+        Args:
+            table_name:
+            sql: DDL
+            **kwargs:
+
+        Returns:
+
+        """
+
+        assert type in ["", "task", "batch_record", "batch_value"]
+
+        # default fields
+        default_fields = [
+            "id",
+            "created_time",
+            "state",
+            "batch_date",
+        ]
+
+        # use translate
+        sql_list = [
+            "begin",
+        ]
+
+        if sql:
+            sql_list.append(sql)
+        else:
+            if not fields:
+                self.logger.warning("no fields")
+                return 0
+            fields_keys = [x.lower() for x in fields]
+
+            if "id" not in fields_keys:
+                fields["id"] = "bigint NOT NULL AUTO_INCREMENT"
+            if "created_time" not in fields_keys:
+                fields[
+                    "created_time"
+                ] = "datetime(0) NOT NULL  DEFAULT CURRENT_TIMESTAMP(0)"
+
+            if type == "task":
+                if "state" not in fields_keys:
+                    fields["state"] = "int DEFAULT 0"
+            elif type == "batch_value":
+                if "batch_date" not in fields_keys:
+                    fields["batch_date"] = "datetime(0) NULL"
+
+            # fields sorted
+            fields = fields.items()
+            fields = (
+                [x for x in fields if x[0].lower() == "id"]
+                + [x for x in fields if x[0].lower() not in default_fields]
+                + [
+                    x
+                    for x in fields
+                    if x[0].lower() in default_fields and x[0].lower() != "id"
+                ]
+            )
+
+            sql = """
+CREATE TABLE {}(
+    {},
+    PRIMARY KEY (`id`)
+) ENGINE=InnoDB DEFAULT CHARSET=utf8mb4 COLLATE=utf8mb4_0900_ai_ci;
+            """.format(
+                "IF NOT EXISTS {}".format(table_name) if exists_ok else table_name,
+                ",\n    ".join("{} {}".format(k, v) for k, v in fields),
+            )
+            sql_list.append(sql)
+
+            if unique:
+                unique = [x.strip("`") for x in unique]
+                sql = "ALTER TABLE {} ADD UNIQUE INDEX `{}_unique`(`{}`);".format(
+                    table_name, table_name, "`,`".join(unique)
+                )
+                sql_list.append(sql)
+
+        #
+        cursor = self.get_cursor()
+        for sql in sql_list:
+            self.logger.info(sql)
+            cursor.execute(sql)
+        cursor.connection.commit()
+        return 0
```

### Comparing `openget-0.1.9/openget/db/db_oracle.py` & `openget-0.2.0/openget/db/db_oracle.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/db/db_oss.py` & `openget-0.2.0/openget/db/db_oss.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/db/db_redis.py` & `openget-0.2.0/openget/db/db_redis.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/db/db_sqlite.py` & `openget-0.2.0/openget/db/db_sqlite.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/db/util.py` & `openget-0.2.0/openget/db/util.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/env.py` & `openget-0.2.0/openget/setting.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,54 @@
 # coding:utf8
 """
-Get all environment variable
-
+setting
 """
-import sys
 import os
-from os import path
+from os import path, getenv
+
+#
+OPENGET_ENV = getenv("OPENGET_ENV", "DEV")
 
+if 1:
 
-# All env defines
-env = {
-    # PROD / DEV / ...
-    "OPENGET_ENV": "DEV",
-    # default mysql config
-    "OPENGET_MYSQL_HOST": None,
-    "OPENGET_MYSQL_PORT": "3306",
-    "OPENGET_MYSQL_USER": None,
-    "OPENGET_MYSQL_PASSWD": None,
-    "OPENGET_MYSQL_CHARSET": "utf8mb4",
-    "OPENGET_MYSQL_DB": "openget",
-    # default redis config
-    "OPENGET_REDIS_URI": "redis://localhost:6379/0",
-    # default proxy service url
-    "OPENGET_PROXY_SERVICE_URL": None,
-    # docker mode
-    "OPENGET_IN_DOCKER": "false",
-    # logging
-    # forbidden better_exceptions
-    "OPENGET_FORBIDDED_BETTER_EXCEPTIONS": None,
-}
-
-
-def parse_env_from_file(filepath):
-    _env = {}
-    if path.isfile(filepath):
-        with open(
-            filepath,
-            "r",
-            encoding="utf8",
-        ) as f:
-            for line in f.readlines():
-                line = line.strip()
-                if not line:
-                    continue
-                # parse comment line
-                if line.startswith(("#", "'", '"')):
-                    continue
-                # parse k,v line
-                k, v = line.split("=", 1)
-                if v.startswith(("'", '"')):
-                    v = v[1:-1]
-                _env[k] = v
-    return _env
-
-
-# from ~/.openget/.env
-GLOBAL_ENV_FILE = path.join(path.expanduser("~"), ".openget/.env")
-env.update(parse_env_from_file(GLOBAL_ENV_FILE))
-
-# from $(pwd)/.env
-if sys.argv[0]:
-    LOCAL_ENV_FILE = path.join(
-        path.dirname(path.join(os.getcwd(), sys.argv[0])), ".env"
-    )
-    env.update(parse_env_from_file(LOCAL_ENV_FILE))
-
-for env_k, env_v in env.items():
-    if env_v is not None:
-        os.environ[env_k] = env_v
+    def get_mysql_uri(x, protocol="mysql"):
+        return (
+            "{protocol}://{user}:{passwd}@{host}:{port}/{db}?charset={charset}".format(
+                protocol=protocol, **x
+            )
+        )
+
+    # mysql config
+    default_mysql_setting_dict = {
+        "host": getenv("OPENGET_MYSQL_HOST", "localhost"),
+        "port": int(getenv("OPENGET_MYSQL_PORT", "3306")),
+        "user": getenv("OPENGET_MYSQL_USER"),
+        "passwd": getenv("OPENGET_MYSQL_PASSWD"),
+        "charset": getenv("OPENGET_MYSQL_CHARSET", "utf8mb4"),
+        "db": getenv("OPENGET_MYSQL_DB", "openget"),
+    }
+
+    default_mysql_uri = get_mysql_uri(default_mysql_setting_dict)
+
+if 1:
+    # redis config
+    def get_redis_uri(db, host, password=""):
+        return "redis://{}{}/{}".format(f":{password}@" if password else "", host, db)
+
+    #
+    default_redis_uri = getenv("OPENGET_REDIS_URI", "redis://localhost:6379/0")
+
+    # for redis lock
+    redis_util_cluster = {
+        0: default_redis_uri,
+    }
+
+if 1:
+    # proxy config
+    proxy_service_url = getenv("OPENGET_PROXY_SERVICE_URL")
+
+# import setting from execute dir
+try:
+    if path.dirname(__file__) != os.getcwd():
+        from setting import *
+except ImportError:
+    pass
```

### Comparing `openget-0.1.9/openget/network/downloader.py` & `openget-0.2.0/openget/network/downloader.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/network/proxy.py` & `openget-0.2.0/openget/network/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -870,15 +870,17 @@
         if not isinstance(proxies, list):
             proxies = [proxies]
         self.vip_proxy_list.extend(proxies)
         return True
 
 
 #
-default_proxy_pool = ProxyPool(proxy_source_uri=[os.getenv("OPENGET_PROXY_SERVICE_URL")])
+default_proxy_pool = ProxyPool(
+    proxy_source_uri=[os.getenv("OPENGET_PROXY_SERVICE_URL")]
+)
 
 
 if __name__ == "__main__":
     #
     fake_proxy_file = path.join(os.getcwd(), "fake_proxy.txt")
     with open(fake_proxy_file, "w") as f:
         f.write("1.1.1.1:8888")
```

### Comparing `openget-0.1.9/openget/network/request.py` & `openget-0.2.0/openget/network/request.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/network/response.py` & `openget-0.2.0/openget/network/response.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/spiders/__init__.py` & `openget-0.2.0/openget/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/spiders/base.py` & `openget-0.2.0/openget/spiders/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,15 +97,17 @@
 
         self._closed = False
         #
         self._close_reason = ""
 
         # Is in docker runing
         self._in_docker = (
-            True if os.getenv("OPENGET_IN_DOCKER", "false").lower() != "false" else False
+            True
+            if os.getenv("OPENGET_IN_DOCKER", "false").lower() != "false"
+            else False
         )
 
         self._stop = False
 
     def __enter__(self):
         return self
 
@@ -353,18 +355,18 @@
             except Exception as e:
                 logger.exception(e)
 
         #
         raise_exception = None
         #
         spider_break = 0
+        # 减少日志量
+        _last_show_qsize_ts = 0
         # 此处若不捕获异常 可能卡死爬虫
         try:
-            # 减少日志量
-            _last_show_qsize_ts = 0
             if self._break_spider() != 1 and not self._killed:
                 for item in self.start_requests():
                     if isinstance(item, Request):
                         self.request_queue.put(item)
                     else:
                         if item is None:
                             logger.warning("Got a None Request")
@@ -402,19 +404,26 @@
                         self.suicide()
                         break
             else:
                 logger.debug("break spider")
         except Exception as e:
             raise_exception = e
         while 1:
-            if self.request_queue.qsize() <= 0:
+            qsize = self.request_queue.qsize()
+            if qsize <= 0:
                 # when all thread is stopped, stop self
                 if sum(self._thread_status.values()) == 0:
                     self.event_exit.set()
                     break
+            else:
+                _t = time.time()
+                if _t - _last_show_qsize_ts > 10:
+                    logger.debug("waiting Request count: {} ...".format(qsize))
+                    _last_show_qsize_ts = _t
+            #
             if spider_break:
                 logger.debug(
                     "main thread was stopped, "
                     "waiting for sub thread stoping... "
                     "remain tasks: {} "
                     "active threads: {} "
                     "stop reason: {}".format(
```

### Comparing `openget-0.1.9/openget/spiders/batch_spider.py` & `openget-0.2.0/openget/spiders/batch_spider.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/util.py` & `openget-0.2.0/openget/util.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/utils/log.py` & `openget-0.2.0/openget/utils/log.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget/utils/message/dingtalk.py` & `openget-0.2.0/openget/utils/message/dingtalk.py`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/openget.egg-info/PKG-INFO` & `openget-0.2.0/openget.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openget
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Spider FrameWork
 Home-page: https://github.com/dytttf/openget
 Author: Dytttf
 Author-email: dytttf@foxmail.com
 License: BSD
 Keywords: openget,spider,batch-spider
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openget-0.1.9/openget.egg-info/SOURCES.txt` & `openget-0.2.0/openget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/pyproject.toml` & `openget-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openget-0.1.9/setup.py` & `openget-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         "redis>=3.0.0",
         "better-exceptions",
         "tqdm",
         "httpx[http2]",
         "user-agent2",
         "urllib3",
         "oss2",
+        "python-dotenv",
     ],
     license="BSD",
     # https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Scrapy",
         "Operating System :: POSIX",
```

