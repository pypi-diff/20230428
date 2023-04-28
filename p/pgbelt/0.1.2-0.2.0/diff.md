# Comparing `tmp/pgbelt-0.1.2.tar.gz` & `tmp/pgbelt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.1.2.tar", max compression
+gzip compressed data, was "pgbelt-0.2.0.tar", max compression
```

## Comparing `pgbelt-0.1.2.tar` & `pgbelt-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    10758 2022-10-04 22:54:52.886362 pgbelt-0.1.2/LICENSE
--rw-r--r--   0        0        0     2047 2022-10-04 22:54:52.886362 pgbelt-0.1.2/README.md
--rw-r--r--   0        0        0      137 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     2301 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5217 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3035 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/login.py
--rw-r--r--   0        0        0     8206 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     3139 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     5074 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     3182 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     8071 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3746 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3743 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/config/config.py
--rw-r--r--   0        0        0     5363 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/config/models.py
--rw-r--r--   0        0        0     5189 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/config/remote.py
--rw-r--r--   0        0        0      187 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/main.py
--rw-r--r--   0        0        0       40 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0     9911 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1424 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/logs.py
--rw-r--r--   0        0        0    12309 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    13694 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1205 2022-10-04 22:54:52.890362 pgbelt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3144 1970-01-01 00:00:00.000000 pgbelt-0.1.2/setup.py
--rw-r--r--   0        0        0     2732 1970-01-01 00:00:00.000000 pgbelt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-04-28 19:32:49.082422 pgbelt-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2047 2023-04-28 19:32:49.086422 pgbelt-0.2.0/README.md
+-rw-r--r--   0        0        0      137 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     2275 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5191 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0     8215 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     3148 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     5082 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     3190 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     8080 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3754 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3724 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/config.py
+-rw-r--r--   0        0        0     5311 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5152 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0     9698 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1424 2023-04-28 19:32:49.086422 pgbelt-0.2.0/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    12309 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    13669 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1202 2023-04-28 19:32:49.090422 pgbelt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 pgbelt-0.2.0/PKG-INFO
```

### Comparing `pgbelt-0.1.2/LICENSE` & `pgbelt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.1.2/README.md` & `pgbelt-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.1.2/pgbelt/cmd/convenience.py` & `pgbelt-0.2.0/pgbelt/cmd/convenience.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from asyncio import run
 from logging import Logger
-from typing import Tuple
 
 from asyncpg import create_pool
-from typer import echo
-from typer import Option
-
 from pgbelt.config.config import get_config
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.logs import get_logger
 from pgbelt.util.postgres import analyze_table_pkeys
+from typer import echo
+from typer import Option
 
 
 def src_dsn(
     db: str,
     dc: str,
     owner: bool = Option(False, help="Use the owner credentials"),
     pglogical: bool = Option(False, help="Use the pglogical credentials."),
@@ -54,15 +52,15 @@
         if pglogical
         else conf.dst.root_dsn
     )
 
 
 async def _check_pkeys(
     conf: DbupgradeConfig, logger: Logger
-) -> Tuple[list[str], list[str]]:
+) -> tuple[list[str], list[str]]:
     async with create_pool(conf.src.root_uri, min_size=1) as pool:
         pkey_tables, no_pkey_tables, _ = await analyze_table_pkeys(pool, logger)
     return pkey_tables, no_pkey_tables
 
 
 def check_pkeys(db: str, dc: str) -> None:
     """
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/helpers.py` & `pgbelt-0.2.0/pgbelt/cmd/helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from asyncio import gather
 from asyncio import run
+from collections.abc import Awaitable
+from collections.abc import Callable
 from functools import wraps
 from inspect import iscoroutinefunction
 from inspect import Parameter
 from inspect import signature
 from typing import Any
-from typing import Awaitable
-from typing import Callable
-from typing import Optional
 from typing import TypeVar
 
-from typer import Argument
-from typer import Typer
-
 from pgbelt.config import get_all_configs_async
 from pgbelt.config import get_config_async
+from typer import Argument
+from typer import Typer
 
 
 T = TypeVar("T")
 
 
 def run_with_configs(
-    decorated_func: Callable[..., Awaitable[Optional[T]]] = None,
+    decorated_func: Callable[..., Awaitable[T | None]] = None,
     skip_src: bool = False,
     skip_dst: bool = False,
-    results_callback: Optional[Callable[[list[T]], Awaitable[Optional[Any]]]] = None,
+    results_callback: Callable[[list[T]], Awaitable[Any | None]] | None = None,
 ) -> Callable:
     """
     Decorator for async commands. Implementations should take one Awaitable[DbupgradeConfig] arg
     and do some operation on the databases in it. This wrapper handles looking up the
     config and executing the command. The decorated result can be run either on one db only
     or on the entire datacenter concurrently.
 
@@ -48,15 +46,15 @@
         else:
             func.__doc__ += (
                 "\n\n    Requires both src and dst to be not null in the config file."
             )
 
         # The name, docstring, and signature of the implementation is preserved. Important for add_command
         @wraps(func)
-        async def wrapper(dc: str, db: Optional[str], **kwargs):
+        async def wrapper(dc: str, db: str | None, **kwargs):
             # If db is specified we only want to run on one of them
             if db is not None:
                 results = [
                     await func(
                         get_config_async(db, dc, skip_src=skip_src, skip_dst=skip_dst),
                         **kwargs
                     )
@@ -98,15 +96,15 @@
     # Give typer the name of the actual implementing function
     name = command.__name__.replace("_", "-")
 
     # If async assume command can be run on a whole datacenter and make db optional
     if iscoroutinefunction(command):
 
         @app.command(name=name)
-        def cmdwrapper(dc: str, db: Optional[str] = Argument(None), **kwargs):
+        def cmdwrapper(dc: str, db: str | None = Argument(None), **kwargs):
             run(command(dc, db, **kwargs))
 
     # Synchronous commands can only be run on one db at a time
     else:
 
         @app.command(name=name)
         def cmdwrapper(dc: str, db: str, **kwargs):
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/login.py` & `pgbelt-0.2.0/pgbelt/cmd/login.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
+from collections.abc import Awaitable
 from logging import Logger
-from typing import Awaitable
 
 from asyncpg import create_pool
 from asyncpg import Pool
-
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbConfig
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.config.models import User
 from pgbelt.util import get_logger
 from pgbelt.util.postgres import disable_login_users
 from pgbelt.util.postgres import enable_login_users
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/preflight.py` & `pgbelt-0.2.0/pgbelt/cmd/preflight.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from asyncio import gather
+from collections.abc import Awaitable
+
+from asyncpg import create_pool
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.logs import get_logger
 from pgbelt.util.postgres import analyze_table_pkeys
 from pgbelt.util.postgres import precheck_info
-from typing import Awaitable
-
-from asyncpg import create_pool
 from tabulate import tabulate
 from typer import echo
 from typer import style
 
 
 async def _print_prechecks(results: list[dict]) -> list[list]:
     summary_table = [
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/schema.py` & `pgbelt-0.2.0/pgbelt/cmd/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Awaitable
+from collections.abc import Awaitable
 
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.dump import apply_target_constraints
 from pgbelt.util.dump import apply_target_schema
 from pgbelt.util.dump import dump_dst_not_valid_constraints
 from pgbelt.util.dump import dump_source_schema
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/setup.py` & `pgbelt-0.2.0/pgbelt/cmd/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from asyncio import create_task
 from asyncio import gather
+from collections.abc import Awaitable
 from logging import Logger
-from typing import Awaitable
 
 from asyncpg import create_pool
 from asyncpg import Pool
-from typer import Option
-
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.dump import apply_target_schema
 from pgbelt.util.dump import dump_source_schema
 from pgbelt.util.logs import get_logger
 from pgbelt.util.pglogical import configure_node
 from pgbelt.util.pglogical import configure_pgl
 from pgbelt.util.pglogical import configure_replication_set
 from pgbelt.util.pglogical import configure_subscription
 from pgbelt.util.pglogical import grant_pgl
 from pgbelt.util.postgres import analyze_table_pkeys
+from typer import Option
 
 
 async def _dump_and_load_schema(
     conf: DbupgradeConfig, src_logger: Logger, dst_logger: Logger
 ) -> None:
     await dump_source_schema(conf, src_logger)
     await apply_target_schema(conf, dst_logger)
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/status.py` & `pgbelt-0.2.0/pgbelt/cmd/status.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from asyncio import gather
-from typing import Awaitable
+from collections.abc import Awaitable
 
 from asyncpg import create_pool
-from tabulate import tabulate
-from typer import echo
-from typer import style
-
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util import get_logger
 from pgbelt.util.pglogical import dst_status
 from pgbelt.util.pglogical import src_status
+from tabulate import tabulate
+from typer import echo
+from typer import style
 
 
 async def _print_status_table(results: list[dict[str, str]]) -> list[list[str]]:
     table = [
         [
             style("database", "yellow"),
             style("src -> dst", "yellow"),
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/sync.py` & `pgbelt-0.2.0/pgbelt/cmd/sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from asyncio import gather
+from collections.abc import Awaitable
 from logging import Logger
+
+from asyncpg import create_pool
+from asyncpg import Pool
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.dump import apply_target_constraints
 from pgbelt.util.dump import dump_source_tables
 from pgbelt.util.dump import load_dumped_tables
 from pgbelt.util.logs import get_logger
 from pgbelt.util.postgres import analyze_table_pkeys
 from pgbelt.util.postgres import compare_100_rows
 from pgbelt.util.postgres import compare_latest_100_rows
 from pgbelt.util.postgres import dump_sequences
 from pgbelt.util.postgres import load_sequences
 from pgbelt.util.postgres import run_analyze
-from typing import Awaitable
-
-from asyncpg import create_pool
-from asyncpg import Pool
 from typer import Option
 
 
 async def _sync_sequences(
     targeted_sequences: list[str],
     src_pool: Pool,
     dst_pool: Pool,
```

### Comparing `pgbelt-0.1.2/pgbelt/cmd/teardown.py` & `pgbelt-0.2.0/pgbelt/cmd/teardown.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from asyncio import gather
 from asyncio import sleep
-from typing import Awaitable
+from collections.abc import Awaitable
 
 from asyncpg import create_pool
-from typer import Option
-
 from pgbelt.cmd.helpers import run_with_configs
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.logs import get_logger
 from pgbelt.util.pglogical import revoke_pgl
 from pgbelt.util.pglogical import teardown_node
 from pgbelt.util.pglogical import teardown_pgl
 from pgbelt.util.pglogical import teardown_replication_set
 from pgbelt.util.pglogical import teardown_subscription
+from typer import Option
 
 
 @run_with_configs(skip_dst=True)
 async def teardown_back_replication(config_future: Awaitable[DbupgradeConfig]):
     """
     Stops pglogical replication from the destination database to the source.
     You should only do this once you are certain a rollback will not be required.
```

### Comparing `pgbelt-0.1.2/pgbelt/config/config.py` & `pgbelt-0.2.0/pgbelt/config/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import asyncio
+from collections.abc import AsyncGenerator
+from collections.abc import Awaitable
 from os.path import join
-from typing import AsyncGenerator
-from typing import Awaitable
-from typing import Optional
 
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.config.remote import resolve_remote_config
 from pgbelt.util import get_logger
 from pgbelt.util.asyncfuncs import isdir
 from pgbelt.util.asyncfuncs import isfile
 from pgbelt.util.asyncfuncs import listdir
 
 
 def get_config(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> Optional[DbupgradeConfig]:
+) -> DbupgradeConfig | None:
     """
     Get a configuration for one database pair synchronously.
     """
     config = asyncio.run(get_config_async(db, dc, skip_src, skip_dst))
 
     if config is None:
         exit(1)
 
     return config
 
 
 async def get_config_async(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> Optional[DbupgradeConfig]:
+) -> DbupgradeConfig | None:
     """
     Get configuration for one database pair asynchronously. Always prefers
     locally cached configuration but attempts to resolve any uncached configuration
     if it is required. Locally cached config never expires, so it may become stale.
     """
     logger = get_logger(db, dc, "config")
     logger.info("Getting configuration...")
@@ -80,15 +79,15 @@
         ):
             result.add(db)
     return result
 
 
 async def get_all_configs_async(
     dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> AsyncGenerator[Awaitable[Optional[DbupgradeConfig]], None]:
+) -> AsyncGenerator[Awaitable[DbupgradeConfig | None], None]:
     """
     A generator that produces Awaitables that resolve to DbupgradeConfigs or None
 
     Will produce all possible configs in the given dc whether they are remote
     or already resolved and cached.
     """
     logger = get_logger("all", dc, "config")
```

### Comparing `pgbelt-0.1.2/pgbelt/config/models.py` & `pgbelt-0.2.0/pgbelt/config/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from __future__ import annotations
 
 from os.path import join
-from pgbelt.util import get_logger
-from pgbelt.util.asyncfuncs import makedirs
-from typing import Optional
 
 from aiofiles import open as aopen
 from aiofiles.os import remove
+from pgbelt.util import get_logger
+from pgbelt.util.asyncfuncs import makedirs
 from pydantic import BaseModel
 from pydantic import ValidationError
 from pydantic import validator
 
 
 def config_dir(db: str, dc: str) -> str:
     return f"configs/{dc}/{db}"
 
 
 def config_file(db: str, dc: str) -> str:
     return join(config_dir(db, dc), "config.json")
 
 
-def not_empty(v) -> Optional[str]:
+def not_empty(v) -> str | None:
     if v == "":
         raise ValueError
     return v
 
 
 class User(BaseModel):
     """
     Represents a user in a postgres db.
 
     name: str The user name.
     pw: str The user's password. Only required for users pgbelt needs to log in as.
     """
 
     name: str
-    pw: Optional[str] = None
+    pw: str | None = None
 
     _not_empty = validator("name", "pw", allow_reuse=True)(not_empty)
 
 
 class DbConfig(BaseModel):
     """
     Represents a postgres db instance.
@@ -58,15 +57,15 @@
     host: str
     ip: str
     db: str
     port: str
     root_user: User
     owner_user: User
     pglogical_user: User
-    other_users: Optional[list[User]] = None
+    other_users: list[User] | None = None
 
     _not_empty = validator("host", "ip", "db", "port", allow_reuse=True)(not_empty)
 
     @validator("root_user", "owner_user", "pglogical_user")
     def has_password(cls, v) -> User:  # noqa: N805
         if not v.pw:
             raise ValueError
@@ -105,18 +104,18 @@
     dc: str A name used to identify the environment this database pair is in. Used in cli commands.
     src: DbConfig The database we are moving data out of.
     dst: DbConfig The database we are moving data into.
     """
 
     db: str
     dc: str
-    src: Optional[DbConfig] = None
-    dst: Optional[DbConfig] = None
-    tables: Optional[list[str]] = None
-    sequences: Optional[list[str]] = None
+    src: DbConfig | None = None
+    dst: DbConfig | None = None
+    tables: list[str] | None = None
+    sequences: list[str] | None = None
 
     _not_empty = validator("db", "dc", allow_reuse=True)(not_empty)
 
     @property
     def file(self) -> str:
         return config_file(self.db, self.dc)
 
@@ -143,15 +142,15 @@
 
         async with aopen(self.file, "w") as f:
             await f.write(self.json(indent=4))
 
         logger.info("Cached config to disk.")
 
     @classmethod
-    async def load(cls, db: str, dc: str) -> Optional[DbupgradeConfig]:
+    async def load(cls, db: str, dc: str) -> DbupgradeConfig | None:
         """
         Load the specified configuration from disk if present.
         If the existing config is invalid or does not exist return None.
         """
         logger = get_logger(db, dc, "config")
         logger.debug("Trying to load cached config...")
```

### Comparing `pgbelt-0.1.2/pgbelt/config/remote.py` & `pgbelt-0.2.0/pgbelt/config/remote.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from importlib import import_module
 from json import JSONDecodeError
 from logging import Logger
-from pgbelt.config.models import DbupgradeConfig
-from pgbelt.util.logs import get_logger
-from typing import Optional
 
 from aiofiles import open as aopen
+from pgbelt.config.models import DbupgradeConfig
+from pgbelt.util.logs import get_logger
 from pydantic import BaseModel
 from pydantic import ValidationError
 
 
 def remote_conf_path(db: str, dc: str) -> str:
     return f"remote-configs/{dc}/{db}/config.json"
 
@@ -56,28 +55,28 @@
     skip_dst: bool
     logger: Logger
 
     class Config:
         arbitrary_types_allowed = True
         extra = "ignore"
 
-    async def resolve(self) -> Optional[DbupgradeConfig]:
+    async def resolve(self) -> DbupgradeConfig | None:
         """
         Called to retrieve the configuration from wherever your resolver gets it.
         Return configuration as a DbupgradeConfig.
 
         If you should have been able to get configuration but encountered an error
         then throw a RemoteConfigError. If there was no config and no error return None
         """
         raise NotImplementedError
 
 
 async def load_remote_conf_def(
     config_file: str, logger: Logger
-) -> Optional[RemoteConfigDefinition]:
+) -> RemoteConfigDefinition | None:
     try:
         logger.debug(f"Reading remote config definition from file {config_file}")
         async with aopen(config_file, mode="r") as f:
             raw_json = await f.read()
 
         return RemoteConfigDefinition.parse_raw(raw_json)
     except FileNotFoundError:
@@ -86,15 +85,15 @@
         logger.error(f"Remote config definition in {config_file} was malformed JSON.")
     except ValidationError:
         logger.error(f"Remote config definition in {config_file} was not valid.")
 
 
 async def resolve_remote_config(
     db: str, dc: str, skip_src: bool = False, skip_dst: bool = False
-) -> Optional[DbupgradeConfig]:
+) -> DbupgradeConfig | None:
     """
     Loads the referenced remote configuration json file, tries to import the
     specified resolver class, executes its resolve method, and returns the
     resulting DbupgradeConfig or None if there was an error
     """
 
     # set up the logger
```

### Comparing `pgbelt-0.1.2/pgbelt/util/asyncfuncs.py` & `pgbelt-0.2.0/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.1.2/pgbelt/util/dump.py` & `pgbelt-0.2.0/pgbelt/util/dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import asyncio
 from logging import Logger
 from os.path import join
-from re import search
-
-from aiofiles import open as aopen
-from asyncpg import create_pool
-
 from pgbelt.config.models import DbupgradeConfig
 from pgbelt.util.asyncfuncs import isfile
 from pgbelt.util.asyncfuncs import listdir
 from pgbelt.util.asyncfuncs import makedirs
 from pgbelt.util.postgres import table_empty
+from re import search
+
+from aiofiles import open as aopen
+from asyncpg import create_pool
 
 RAW = "schema"
 NO_INVALID = "no_invalid_constraints"
 ONLY_INVALID = "invalid_constraints"
 
 
 def schema_dir(db: str, dc: str) -> str:
@@ -29,31 +28,28 @@
     return f"tables/{dc}/{db}"
 
 
 def table_file(db: str, dc: str, name: str) -> str:
     return join(table_dir(db, dc), f"{name}.sql")
 
 
-def _parse_dump_commands(out: str, src_owner: str, dst_owner: str) -> list[str]:
+def _parse_dump_commands(out: str) -> list[str]:
     """
     Given a string containing output from pg_dump, return a list of strings where
     each is a complete postgres command. Commands may be multi-line.
     """
     lines = out.split("\n")
     commands = []
 
     for line in lines:
         stripped = line.strip()
         # if the line is whitespace only or a comment then ignore it
         if not stripped or stripped.startswith("--"):
             continue
 
-        # replace source owner user with target owner user
-        line = line.replace(src_owner, dst_owner)
-
         # if the last command is terminated or we don't have any yet start a new one
         if not commands or commands[-1].endswith(";\n"):
             commands.append(line + "\n")
         # otherwise we append to the last command because it must be multi-line
         else:
             commands[-1] += line + "\n"
 
@@ -168,17 +164,15 @@
         "-n",
         "public",
         config.src.pglogical_dsn,
     ]
 
     out = await _execute_subprocess(command, "Retrieved source schema", logger)
 
-    commands_raw = _parse_dump_commands(
-        out.decode("utf-8"), config.src.owner_user.name, config.dst.owner_user.name
-    )
+    commands_raw = _parse_dump_commands(out.decode("utf-8"))
 
     commands = []
     for c in commands_raw:
         if "EXTENSION " not in c and "GRANT " not in c and "REVOKE " not in c:
             commands.append(c)
 
     try:
```

### Comparing `pgbelt-0.1.2/pgbelt/util/logs.py` & `pgbelt-0.2.0/pgbelt/util/logs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.1.2/pgbelt/util/pglogical.py` & `pgbelt-0.2.0/pgbelt/util/pglogical.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.1.2/pgbelt/util/postgres.py` & `pgbelt-0.2.0/pgbelt/util/postgres.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from logging import Logger
-from typing import Tuple
 
 from asyncpg import Pool
 from asyncpg import Record
 from asyncpg.exceptions import UndefinedObjectError
 
 
 async def dump_sequences(
@@ -207,15 +206,15 @@
     logger.info(f"Checking if table {table} is empty...")
     result = await pool.fetch(f"SELECT * FROM {table} LIMIT 1;")
     return len(result) == 0
 
 
 async def analyze_table_pkeys(
     pool: Pool, logger: Logger
-) -> Tuple[list[str], list[str], Record]:
+) -> tuple[list[str], list[str], Record]:
     """
     return three lists of table names. the first element is all tables
     with pkeys in public and the second is all tables without pkeys in public.
     The third list is the raw rows of the primary key query with the table name,
     constraint name, position and column name for the primary key.
     """
     logger.info("Checking table primary keys...")
```

### Comparing `pgbelt-0.1.2/pyproject.toml` & `pgbelt-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.1.2"
+version = "0.2.0"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-aiofiles = ">=0.8,<22.2"
-asyncpg = "~0.26.0"
-pydantic = "~1.10.1"
-tabulate = "~0.8.9"
-typer = "~0.6.1"
+python = "^3.11"
+aiofiles = ">=0.8,<23.2"
+asyncpg = "^0.27.0"
+pydantic = "^1.10.0"
+tabulate = "^0.9.0"
+typer = "^0.7.0"
 
 [tool.poetry.dev-dependencies]
-black = "~22.8.0"
-pre-commit = "~2.20.0"
-flake8 = "~5.0.4"
+black = "~23.3.0"
+pre-commit = "~3.2.1"
+flake8 = "^6.0.0"
 pytest-cov = "~4.0.0"
 pytest = "^7.1.3"
 coverage = {extras = ["toml"], version = "^6.5"}
-safety = "^2.2.0"
-mypy = "^0.981"
+safety = "^2.3.1"
+mypy = "^1.1"
 xdoctest = {extras = ["colors"], version = "^1.1.0"}
 flake8-bandit = "~4.1.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = "^1.6.0"
-flake8-rst-docstrings = "^0.2.7"
+flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.2"
 darglint = "^1.8.1"
-reorder-python-imports = "^3.8.2"
+reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.2.0"
 Pygments = "^2.13.0"
-pyupgrade = "^2.38.2"
-pylint = "^2.15.3"
-pytest-asyncio = "~0.19.0"
+pyupgrade = "^3.3.1"
+pylint = "^2.17.2"
+pytest-asyncio = "~0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 belt = "pgbelt.main:app"
```

### Comparing `pgbelt-0.1.2/setup.py` & `pgbelt-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,68 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pgbelt
+Version: 0.2.0
+Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
+Author: Varjitt Jeeva
+Author-email: varjitt.jeeva@autodesk.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=0.8,<23.2)
+Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': '.'}
+# Pgbelt
 
-packages = \
-['pgbelt', 'pgbelt.cmd', 'pgbelt.config', 'pgbelt.util']
+<p align="center">
+    <img src="https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true" width="400">
+</p>
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['aiofiles>=0.8,<22.2',
- 'asyncpg>=0.26.0,<0.27.0',
- 'pydantic>=1.10.1,<1.11.0',
- 'tabulate>=0.8.9,<0.9.0',
- 'typer>=0.6.1,<0.7.0']
-
-entry_points = \
-{'console_scripts': ['belt = pgbelt.main:app']}
-
-setup_kwargs = {
-    'name': 'pgbelt',
-    'version': '0.1.2',
-    'description': 'A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.',
-    'long_description': '# Pgbelt\n\n<p align="center">\n    <img src="https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true" width="400">\n</p>\n\n<p align="center">\n    <a href="https://github.com/autodesk/pgbelt" target="_blank">\n        <img src="https://img.shields.io/github/last-commit/autodesk/pgbelt" alt="Latest Commit">\n    </a>\n    <img src="https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/badge.svg">\n    <a href="http://www.apache.org/licenses/LICENSE-2.0" target="_blank">\n        <img src="https://img.shields.io/github/license/Autodesk/pgbelt">\n    </a>\n</p>\n\nPgBelt is a CLI tool used to manage Postgres data migrations from beginning to end,\nfor a single database or a fleet, leveraging pglogical replication.\n\nIt was built to assist in migrating data between postgres databases with as\nlittle application downtime as possible. It works in databases running different versions\nof postgres and makes it easy to run many migrations in parallel during a single downtime.\n\n| :exclamation: This is very important                                                                                                            |\n| :---------------------------------------------------------------------------------------------------------------------------------------------- |\n| As with all Data Migration tasks, **there is a risk of data loss**. Please ensure you have backed up your data before attempting any migrations |\n\n## Installation\n\n### Install From PyPi\n\nIt is recommended to install pgbelt inside a virtual environment:\n\n- [pyenv](https://github.com/pyenv/pyenv)\n- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)\n\nYou must also have:\n\n- Postgres Client Tools (pg_dump, pg_restore). Mac: `brew install libpq`. Ubuntu: `sudo apt-get install postgresql-client`\n\nInstall pgbelt locally:\n\n    pip3 install pgbelt\n\n## Quickstart with Pgbelt\n\nSee [this doc](docs/quickstart.md)!\n\n## Contributing\n\nWe welcome contributions! See [this doc](CONTRIBUTING.md) on how to do so, including setting up your local development environment.\n',
-    'author': 'Varjitt Jeeva',
-    'author_email': 'varjitt.jeeva@autodesk.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+<p align="center">
+    <a href="https://github.com/autodesk/pgbelt" target="_blank">
+        <img src="https://img.shields.io/github/last-commit/autodesk/pgbelt" alt="Latest Commit">
+    </a>
+    <img src="https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/badge.svg">
+    <a href="http://www.apache.org/licenses/LICENSE-2.0" target="_blank">
+        <img src="https://img.shields.io/github/license/Autodesk/pgbelt">
+    </a>
+</p>
 
+PgBelt is a CLI tool used to manage Postgres data migrations from beginning to end,
+for a single database or a fleet, leveraging pglogical replication.
+
+It was built to assist in migrating data between postgres databases with as
+little application downtime as possible. It works in databases running different versions
+of postgres and makes it easy to run many migrations in parallel during a single downtime.
+
+| :exclamation: This is very important                                                                                                            |
+| :---------------------------------------------------------------------------------------------------------------------------------------------- |
+| As with all Data Migration tasks, **there is a risk of data loss**. Please ensure you have backed up your data before attempting any migrations |
+
+## Installation
+
+### Install From PyPi
+
+It is recommended to install pgbelt inside a virtual environment:
+
+- [pyenv](https://github.com/pyenv/pyenv)
+- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)
+
+You must also have:
+
+- Postgres Client Tools (pg_dump, pg_restore). Mac: `brew install libpq`. Ubuntu: `sudo apt-get install postgresql-client`
+
+Install pgbelt locally:
+
+    pip3 install pgbelt
+
+## Quickstart with Pgbelt
+
+See [this doc](docs/quickstart.md)!
+
+## Contributing
+
+We welcome contributions! See [this doc](CONTRIBUTING.md) on how to do so, including setting up your local development environment.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,38 +1,30 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': '.'}
-packages = \ ['pgbelt', 'pgbelt.cmd', 'pgbelt.config', 'pgbelt.util']
-package_data = \ {'': ['*']} install_requires = \ ['aiofiles>=0.8,<22.2',
-'asyncpg>=0.26.0,<0.27.0', 'pydantic>=1.10.1,<1.11.0',
-'tabulate>=0.8.9,<0.9.0', 'typer>=0.6.1,<0.7.0'] entry_points = \
-{'console_scripts': ['belt = pgbelt.main:app']} setup_kwargs = { 'name':
-'pgbelt', 'version': '0.1.2', 'description': 'A CLI tool used to manage
-Postgres data migrations from beginning to end, for a single database or a
-fleet, leveraging pglogical replication.', 'long_description': '# Pgbelt\n\n
-    \n [https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true]\n
-\n\n
-    \n \n_[Latest_Commit]\n\n [https://github.com/Autodesk/pgbelt/actions/
-   workflows/ci.yml/badge.svg]\n \n_[https://img.shields.io/github/license/
-                             Autodesk/pgbelt]\n\n
-\n\nPgBelt is a CLI tool used to manage Postgres data migrations from beginning
-to end,\nfor a single database or a fleet, leveraging pglogical
-replication.\n\nIt was built to assist in migrating data between postgres
-databases with as\nlittle application downtime as possible. It works in
-databases running different versions\nof postgres and makes it easy to run many
-migrations in parallel during a single downtime.\n\n| :exclamation: This is
-very important |\n| :----------------------------------------------------------
+Metadata-Version: 2.1 Name: pgbelt Version: 0.2.0 Summary: A CLI tool used to
+manage Postgres data migrations from beginning to end, for a single database or
+a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
+varjitt.jeeva@autodesk.com Requires-Python: >=3.11,<4.0 Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=0.8,<23.2) Requires-Dist: asyncpg (>=0.27.0,<0.28.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0) Requires-Dist: tabulate
+(>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.7.0,<0.8.0) Description-Content-
+Type: text/markdown # Pgbelt
+      [https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true]
+ [Latest_Commit] [https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/
+      badge.svg] [https://img.shields.io/github/license/Autodesk/pgbelt]
+PgBelt is a CLI tool used to manage Postgres data migrations from beginning to
+end, for a single database or a fleet, leveraging pglogical replication. It was
+built to assist in migrating data between postgres databases with as little
+application downtime as possible. It works in databases running different
+versions of postgres and makes it easy to run many migrations in parallel
+during a single downtime. | :exclamation: This is very important | | :---------
 -------------------------------------------------------------------------------
------ |\n| As with all Data Migration tasks, **there is a risk of data loss**.
-Please ensure you have backed up your data before attempting any migrations
-|\n\n## Installation\n\n### Install From PyPi\n\nIt is recommended to install
-pgbelt inside a virtual environment:\n\n- [pyenv](https://github.com/pyenv/
-pyenv)\n- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv)\n\nYou
-must also have:\n\n- Postgres Client Tools (pg_dump, pg_restore). Mac: `brew
-install libpq`. Ubuntu: `sudo apt-get install postgresql-client`\n\nInstall
-pgbelt locally:\n\n pip3 install pgbelt\n\n## Quickstart with Pgbelt\n\nSee
-[this doc](docs/quickstart.md)!\n\n## Contributing\n\nWe welcome contributions!
-See [this doc](CONTRIBUTING.md) on how to do so, including setting up your
-local development environment.\n', 'author': 'Varjitt Jeeva', 'author_email':
-'varjitt.jeeva@autodesk.com', 'maintainer': 'None', 'maintainer_email': 'None',
-'url': 'None', 'package_dir': package_dir, 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'entry_points': entry_points, 'python_requires': '>=3.9,<4.0', } setup
-(**setup_kwargs)
+------------------------------------------------------ | | As with all Data
+Migration tasks, **there is a risk of data loss**. Please ensure you have
+backed up your data before attempting any migrations | ## Installation ###
+Install From PyPi It is recommended to install pgbelt inside a virtual
+environment: - [pyenv](https://github.com/pyenv/pyenv) - [pyenv-virtualenv]
+(https://github.com/pyenv/pyenv-virtualenv) You must also have: - Postgres
+Client Tools (pg_dump, pg_restore). Mac: `brew install libpq`. Ubuntu: `sudo
+apt-get install postgresql-client` Install pgbelt locally: pip3 install pgbelt
+## Quickstart with Pgbelt See [this doc](docs/quickstart.md)! ## Contributing
+We welcome contributions! See [this doc](CONTRIBUTING.md) on how to do so,
+including setting up your local development environment.
```

