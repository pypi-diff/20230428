# Comparing `tmp/dagger_io-0.5.1.tar.gz` & `tmp/dagger_io-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagger_io-0.5.1.tar", max compression
+gzip compressed data, was "dagger_io-0.5.2.tar", max compression
```

## Comparing `dagger_io-0.5.1.tar` & `dagger_io-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    10758 2023-04-08 15:37:34.303780 dagger_io-0.5.1/LICENSE
--rw-r--r--   0        0        0     4727 2023-04-08 15:37:34.303780 dagger_io-0.5.1/README.md
--rw-r--r--   0        0        0     6344 2023-04-08 15:41:15.110275 dagger_io-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      313 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/__init__.py
--rw-r--r--   0        0        0       49 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/__main__.py
--rw-r--r--   0        0        0       69 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/api/.gitattributes
--rw-r--r--   0        0        0        0 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/api/__init__.py
--rw-r--r--   0        0        0    10234 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/api/base.py
--rw-r--r--   0        0        0    79297 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/api/gen.py
--rw-r--r--   0        0        0    78989 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/api/gen_sync.py
--rw-r--r--   0        0        0     1650 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/cli.py
--rw-r--r--   0        0        0    18459 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/codegen.py
--rw-r--r--   0        0        0     1291 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/config.py
--rw-r--r--   0        0        0     1585 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/connection.py
--rw-r--r--   0        0        0      964 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/context.py
--rw-r--r--   0        0        0       37 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/.gitattributes
--rw-r--r--   0        0        0       35 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/__init__.py
--rw-r--r--   0        0        0       64 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/_version.py
--rw-r--r--   0        0        0     4188 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/cli.py
--rw-r--r--   0        0        0     2068 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/conn.py
--rw-r--r--   0        0        0     8163 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/engine/download.py
--rw-r--r--   0        0        0     3042 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/exceptions.py
--rw-r--r--   0        0        0      677 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/log.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/py.typed
--rw-r--r--   0        0        0     2320 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/server/__init__.py
--rw-r--r--   0        0        0      849 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/server/cli.py
--rw-r--r--   0        0        0      865 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/server/converter.py
--rw-r--r--   0        0        0     3892 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/session.py
--rw-r--r--   0        0        0        0 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/transport/__init__.py
--rw-r--r--   0        0        0     5820 2023-04-08 15:37:34.307780 dagger_io-0.5.1/src/dagger/transport/httpx.py
--rw-r--r--   0        0        0     5922 1970-01-01 00:00:00.000000 dagger_io-0.5.1/setup.py
--rw-r--r--   0        0        0     6481 1970-01-01 00:00:00.000000 dagger_io-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    10758 2023-04-28 17:39:56.098465 dagger_io-0.5.2/LICENSE
+-rw-r--r--   0        0        0     4727 2023-04-28 17:39:56.098465 dagger_io-0.5.2/README.md
+-rw-r--r--   0        0        0     6344 2023-04-28 17:41:23.691286 dagger_io-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      313 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/__init__.py
+-rw-r--r--   0        0        0       49 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/__main__.py
+-rw-r--r--   0        0        0       69 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/.gitattributes
+-rw-r--r--   0        0        0        0 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/__init__.py
+-rw-r--r--   0        0        0    10984 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/base.py
+-rw-r--r--   0        0        0    83180 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/gen.py
+-rw-r--r--   0        0        0    82872 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/api/gen_sync.py
+-rw-r--r--   0        0        0     1650 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/cli.py
+-rw-r--r--   0        0        0    18459 2023-04-28 17:39:56.098465 dagger_io-0.5.2/src/dagger/codegen.py
+-rw-r--r--   0        0        0     1291 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/config.py
+-rw-r--r--   0        0        0     1585 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/connection.py
+-rw-r--r--   0        0        0      964 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/context.py
+-rw-r--r--   0        0        0       37 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/.gitattributes
+-rw-r--r--   0        0        0       35 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/__init__.py
+-rw-r--r--   0        0        0       64 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/_version.py
+-rw-r--r--   0        0        0     4188 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/cli.py
+-rw-r--r--   0        0        0     2068 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/conn.py
+-rw-r--r--   0        0        0     8163 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/engine/download.py
+-rw-r--r--   0        0        0     3042 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/exceptions.py
+-rw-r--r--   0        0        0      677 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/py.typed
+-rw-r--r--   0        0        0     2320 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/__init__.py
+-rw-r--r--   0        0        0      849 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/cli.py
+-rw-r--r--   0        0        0      865 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/server/converter.py
+-rw-r--r--   0        0        0     3892 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/session.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/transport/__init__.py
+-rw-r--r--   0        0        0     5820 2023-04-28 17:39:56.102465 dagger_io-0.5.2/src/dagger/transport/httpx.py
+-rw-r--r--   0        0        0     5951 1970-01-01 00:00:00.000000 dagger_io-0.5.2/setup.py
+-rw-r--r--   0        0        0     6524 1970-01-01 00:00:00.000000 dagger_io-0.5.2/PKG-INFO
```

### Comparing `dagger_io-0.5.1/LICENSE` & `dagger_io-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/README.md` & `dagger_io-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/pyproject.toml` & `dagger_io-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "dagger-io"
-version = "0.5.1"
+version = "0.5.2"
 description = "A client package for running Dagger pipelines in Python."
 license = "Apache-2.0"
 authors = ["Dagger <hello@dagger.io>"]
 readme = "README.md"
 homepage = "https://dagger.io"
 documentation = "https://docs.dagger.io/sdk/python"
 repository = "https://github.com/dagger/dagger/tree/main/sdk/python"
@@ -45,14 +45,15 @@
 graphql-core = ">=3.2.3"
 # FIXME: replace next two lines with the following when gql version 3.5.0 is released
 # gql = {version = ">=3.5.0", extras = ["httpx"]}
 gql = ">=3.4.0"
 httpx = ">=0.23.1"
 beartype = ">=0.11.0"
 platformdirs = ">=2.6.2"
+typing_extensions = ">=4.4.0"
 rich = ">=12.6.0"
 typer = {version = ">=0.6.1", extras = ["all"]}
 strawberry-graphql = {version = ">=0.133.5", optional = true}
 
 [tool.poetry.extras]
 server = ["strawberry-graphql"]
 
@@ -62,15 +63,14 @@
 pytest-subprocess = ">=1.4.2"
 pytest-lazy-fixture = "^0.6.3"
 pytest-httpx = ">=0.21.3"
 
 [tool.poetry.group.lint.dependencies]
 black = ">=22.3.0"
 mypy = ">=0.942"
-typing_extensions = ">=4.4.0"
 ruff = ">=0.0.218"
 
 [tool.poetry.group.dev.dependencies]
 poethepoet = ">=0.16.4"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=5.3.0"
```

### Comparing `dagger_io-0.5.1/src/dagger/api/base.py` & `dagger_io-0.5.2/src/dagger/api/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from gql.dsl import DSLField, DSLQuery, DSLSchema, DSLSelectable, DSLType, dsl_gql
 from gql.transport.exceptions import (
     TransportClosed,
     TransportProtocolError,
     TransportQueryError,
     TransportServerError,
 )
+from typing_extensions import Self
 
 from dagger.exceptions import (
     ExecuteTimeoutError,
     InvalidQueryError,
     QueryError,
     TransportError,
 )
@@ -232,14 +233,40 @@
 
     _ctx: Context
 
     def _select(self, field_name: str, args: typing.Sequence[Arg]) -> Context:
         _args = {arg.name: arg.value for arg in args if arg.value is not arg.default}
         return self._ctx.select(self.graphql_name, field_name, _args)
 
+    def with_(self, cb: Callable[[Self], Self]) -> Self:
+        """
+        Use a callable to add to the current object.
+
+        This allows reusing funcionality (e.g., adding mounts)
+        without breaking the pipeline chain.
+
+        Example
+        -------
+        For a :py:class:`Container` type:
+
+        >>> def foobar(c: dagger.Container) -> dagger.Container:
+        ...     return c.with_env_variable("FOO", "bar")
+
+        It can be used like this:
+
+        >>> out = await (
+        ...     client.container()
+        ...     .from_("alpine")
+        ...     .with_(foobar)
+        ...     .with_exec(["printenv", "FOO"])
+        ...     .stdout()
+        ... )
+        """
+        return cb(self)
+
 
 class Root(Type):
     """Top level query object type (a.k.a. Query)."""
 
     @classmethod
     def from_session(cls, session: AsyncClientSession):
         assert (
```

### Comparing `dagger_io-0.5.1/src/dagger/api/gen.py` & `dagger_io-0.5.2/src/dagger/api/gen_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     """Label value."""
 
 
 class CacheVolume(Type):
     """A directory whose contents persist across runs."""
 
     @typecheck
-    async def id(self) -> CacheID:
+    def id(self) -> CacheID:
         """Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
         CacheID
@@ -105,53 +105,58 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(CacheID)
+        return _ctx.execute_sync(CacheID)
 
 
 class Container(Type):
     """An OCI-compatible container, also known as a docker container."""
 
     @typecheck
     def build(
         self,
         context: "Directory",
         dockerfile: Optional[str] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
+        secrets: Optional[Sequence["Secret"]] = None,
     ) -> "Container":
         """Initializes this container from a Dockerfile build.
 
         Parameters
         ----------
         context:
             Directory context used by the Dockerfile.
         dockerfile:
             Path to the Dockerfile to use.
             Default: './Dockerfile'.
         build_args:
             Additional build arguments.
         target:
             Target build stage to build.
+        secrets:
+            Secrets to pass to the build.
+            They will be mounted at /run/secrets/[secret-name].
         """
         _args = [
             Arg("context", context),
             Arg("dockerfile", dockerfile, None),
             Arg("buildArgs", build_args, None),
             Arg("target", target, None),
+            Arg("secrets", secrets, None),
         ]
         _ctx = self._select("build", _args)
         return Container(_ctx)
 
     @typecheck
-    async def default_args(self) -> Optional[list[str]]:
+    def default_args(self) -> Optional[list[str]]:
         """Retrieves default arguments for future commands.
 
         Returns
         -------
         Optional[list[str]]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -162,15 +167,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("defaultArgs", _args)
-        return await _ctx.execute(Optional[list[str]])
+        return _ctx.execute_sync(Optional[list[str]])
 
     @typecheck
     def directory(self, path: str) -> "Directory":
         """Retrieves a directory at the given path.
 
         Mounts are included.
 
@@ -182,15 +187,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
     @typecheck
-    async def endpoint(
+    def endpoint(
         self,
         port: Optional[int] = None,
         scheme: Optional[str] = None,
     ) -> str:
         """Retrieves an endpoint that clients can use to reach this container.
 
         If no port is specified, the first exposed port is used. If none exist
@@ -224,18 +229,18 @@
             If the API returns an error.
         """
         _args = [
             Arg("port", port, None),
             Arg("scheme", scheme, None),
         ]
         _ctx = self._select("endpoint", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def entrypoint(self) -> Optional[list[str]]:
+    def entrypoint(self) -> Optional[list[str]]:
         """Retrieves entrypoint to be prepended to the arguments of all commands.
 
         Returns
         -------
         Optional[list[str]]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -246,18 +251,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("entrypoint", _args)
-        return await _ctx.execute(Optional[list[str]])
+        return _ctx.execute_sync(Optional[list[str]])
 
     @typecheck
-    async def env_variable(self, name: str) -> Optional[str]:
+    def env_variable(self, name: str) -> Optional[str]:
         """Retrieves the value of the specified environment variable.
 
         Parameters
         ----------
         name:
             The name of the environment variable to retrieve (e.g., "PATH").
 
@@ -275,15 +280,15 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def env_variables(self) -> "EnvVariable":
         """Retrieves the list of environment variables passed to commands."""
         _args: list[Arg] = []
         _ctx = self._select("envVariables", _args)
         return EnvVariable(_ctx)
@@ -331,17 +336,19 @@
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
         ]
         _ctx = self._select("exec", _args)
         return Container(_ctx)
 
     @typecheck
-    async def exit_code(self) -> int:
+    def exit_code(self) -> int:
         """Exit code of the last executed command. Zero means success.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
             - 1.
@@ -351,18 +358,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("exitCode", _args)
-        return await _ctx.execute(int)
+        return _ctx.execute_sync(int)
 
     @typecheck
-    async def export(
+    def export(
         self,
         path: str,
         platform_variants: Optional[Sequence["Container"]] = None,
     ) -> bool:
         """Writes the container as an OCI tarball to the destination file path on
         the host for the specified platform variants.
 
@@ -391,15 +398,15 @@
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
             Arg("platformVariants", platform_variants, None),
         ]
         _ctx = self._select("export", _args)
-        return await _ctx.execute(bool)
+        return _ctx.execute_sync(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
@@ -450,15 +457,15 @@
             Replaced by :py:meth:`rootfs`.
         """
         _args: list[Arg] = []
         _ctx = self._select("fs", _args)
         return Directory(_ctx)
 
     @typecheck
-    async def hostname(self) -> str:
+    def hostname(self) -> str:
         """Retrieves a hostname which can be used by clients to reach this
         container.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
 
         Returns
@@ -473,18 +480,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("hostname", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def id(self) -> ContainerID:
+    def id(self) -> ContainerID:
         """A unique identifier for this container.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -498,18 +505,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(ContainerID)
+        return _ctx.execute_sync(ContainerID)
 
     @typecheck
-    async def image_ref(self) -> Optional[str]:
+    def image_ref(self) -> Optional[str]:
         """The unique image reference which can only be retrieved immediately
         after the 'Container.From' call.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
@@ -521,15 +528,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("imageRef", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def import_(
         self,
         source: "File",
         tag: Optional[str] = None,
     ) -> "Container":
@@ -553,15 +560,15 @@
             Arg("source", source),
             Arg("tag", tag, None),
         ]
         _ctx = self._select("import", _args)
         return Container(_ctx)
 
     @typecheck
-    async def label(self, name: str) -> Optional[str]:
+    def label(self, name: str) -> Optional[str]:
         """Retrieves the value of the specified label.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -574,25 +581,25 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("label", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def labels(self) -> "Label":
         """Retrieves the list of labels passed to container."""
         _args: list[Arg] = []
         _ctx = self._select("labels", _args)
         return Label(_ctx)
 
     @typecheck
-    async def mounts(self) -> list[str]:
+    def mounts(self) -> list[str]:
         """Retrieves the list of paths where a directory is mounted.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -603,15 +610,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("mounts", _args)
-        return await _ctx.execute(list[str])
+        return _ctx.execute_sync(list[str])
 
     @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
@@ -632,15 +639,15 @@
             Arg("description", description, None),
             Arg("labels", labels, None),
         ]
         _ctx = self._select("pipeline", _args)
         return Container(_ctx)
 
     @typecheck
-    async def platform(self) -> Platform:
+    def platform(self) -> Platform:
         """The platform this container executes and publishes as.
 
         Returns
         -------
         Platform
             The platform config OS and architecture in a Container.  The
             format is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
@@ -651,18 +658,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("platform", _args)
-        return await _ctx.execute(Platform)
+        return _ctx.execute_sync(Platform)
 
     @typecheck
-    async def publish(
+    def publish(
         self,
         address: str,
         platform_variants: Optional[Sequence["Container"]] = None,
     ) -> str:
         """Publishes this container as a new image to the specified address.
 
         Publish returns a fully qualified ref.
@@ -693,27 +700,29 @@
             If the API returns an error.
         """
         _args = [
             Arg("address", address),
             Arg("platformVariants", platform_variants, None),
         ]
         _ctx = self._select("publish", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
     def rootfs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included."""
         _args: list[Arg] = []
         _ctx = self._select("rootfs", _args)
         return Directory(_ctx)
 
     @typecheck
-    async def stderr(self) -> str:
+    def stderr(self) -> str:
         """The error stream of the last executed command.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -723,20 +732,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stderr", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def stdout(self) -> str:
+    def stdout(self) -> str:
         """The output stream of the last executed command.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -746,18 +757,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stdout", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def user(self) -> Optional[str]:
+    def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -768,15 +779,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("user", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
     def with_default_args(
         self,
         args: Optional[Sequence[str]] = None,
     ) -> "Container":
         """Configures default arguments for future commands.
@@ -796,14 +807,15 @@
     @typecheck
     def with_directory(
         self,
         path: str,
         directory: "Directory",
         exclude: Optional[Sequence[str]] = None,
         include: Optional[Sequence[str]] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a directory written at the given path.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "/tmp/directory").
@@ -811,20 +823,26 @@
             Identifier of the directory to write
         exclude:
             Patterns to exclude in the written directory (e.g.,
             ["node_modules/**", ".gitignore", ".git/"]).
         include:
             Patterns to include in the written directory (e.g., ["*.go",
             "go.mod", "go.sum"]).
+        owner:
+            A user:group to set for the directory and its contents.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("directory", directory),
             Arg("exclude", exclude, None),
             Arg("include", include, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withDirectory", _args)
         return Container(_ctx)
 
     @typecheck
     def with_entrypoint(self, args: Sequence[str]) -> "Container":
         """Retrieves this container but with a different command entrypoint.
@@ -858,28 +876,33 @@
         _ctx = self._select("withEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exec(
         self,
         args: Sequence[str],
+        skip_entrypoint: Optional[bool] = None,
         stdin: Optional[str] = None,
         redirect_stdout: Optional[str] = None,
         redirect_stderr: Optional[str] = None,
         experimental_privileged_nesting: Optional[bool] = None,
         insecure_root_capabilities: Optional[bool] = None,
     ) -> "Container":
         """Retrieves this container after executing the specified command inside
         it.
 
         Parameters
         ----------
         args:
             Command to run instead of the container's default command (e.g.,
             ["run", "main.go"]).
+            If empty, the container's default command is used.
+        skip_entrypoint:
+            If the container has an entrypoint, ignore it for args rather than
+            using it to wrap them.
         stdin:
             Content to write to the command's standard input before closing
             (e.g., "Hello world").
         redirect_stdout:
             Redirect the command's standard output to a file in the container
             (e.g., "/tmp/stdout").
         redirect_stderr:
@@ -898,14 +921,15 @@
             flag. Containerization
             does not provide any security guarantees when using this option.
             It should only be used
             when absolutely necessary and only with trusted commands.
         """
         _args = [
             Arg("args", args),
+            Arg("skipEntrypoint", skip_entrypoint, None),
             Arg("stdin", stdin, None),
             Arg("redirectStdout", redirect_stdout, None),
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
             Arg("insecureRootCapabilities", insecure_root_capabilities, None),
         ]
         _ctx = self._select("withExec", _args)
@@ -959,32 +983,39 @@
 
     @typecheck
     def with_file(
         self,
         path: str,
         source: "File",
         permissions: Optional[int] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus the contents of the given file copied to
         the given path.
 
         Parameters
         ----------
         path:
             Location of the copied file (e.g., "/tmp/file.txt").
         source:
             Identifier of the file to copy.
         permissions:
             Permission given to the copied file (e.g., 0600).
             Default: 0644.
+        owner:
+            A user:group to set for the file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
             Arg("permissions", permissions, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withFile", _args)
         return Container(_ctx)
 
     @typecheck
     def with_label(self, name: str, value: str) -> "Container":
         """Retrieves this container plus the given label.
@@ -1007,89 +1038,134 @@
     @typecheck
     def with_mounted_cache(
         self,
         path: str,
         cache: CacheVolume,
         source: Optional["Directory"] = None,
         sharing: Optional[CacheSharingMode] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a cache volume mounted at the given
         path.
 
         Parameters
         ----------
         path:
             Location of the cache directory (e.g., "/cache/node_modules").
         cache:
             Identifier of the cache volume to mount.
         source:
             Identifier of the directory to use as the cache volume's root.
         sharing:
             Sharing mode of the cache volume.
+        owner:
+            A user:group to set for the mounted cache directory.
+            Note that this changes the ownership of the specified mount along
+            with the
+            initial filesystem provided by source (if any). It does not have
+            any effect
+            if/when the cache has already been created.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("cache", cache),
             Arg("source", source, None),
             Arg("sharing", sharing, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedCache", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_directory(self, path: str, source: "Directory") -> "Container":
+    def with_mounted_directory(
+        self,
+        path: str,
+        source: "Directory",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a directory mounted at the given path.
 
         Parameters
         ----------
         path:
             Location of the mounted directory (e.g., "/mnt/directory").
         source:
             Identifier of the mounted directory.
+        owner:
+            A user:group to set for the mounted directory and its contents.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedDirectory", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_file(self, path: str, source: "File") -> "Container":
+    def with_mounted_file(
+        self,
+        path: str,
+        source: "File",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a file mounted at the given path.
 
         Parameters
         ----------
         path:
             Location of the mounted file (e.g., "/tmp/file.txt").
         source:
             Identifier of the mounted file.
+        owner:
+            A user or user:group to set for the mounted file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedFile", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_secret(self, path: str, source: "Secret") -> "Container":
+    def with_mounted_secret(
+        self,
+        path: str,
+        source: "Secret",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a secret mounted into a file at the
         given path.
 
         Parameters
         ----------
         path:
             Location of the secret file (e.g., "/tmp/secret.txt").
         source:
             Identifier of the secret to mount.
+        owner:
+            A user:group to set for the mounted secret.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedSecret", _args)
         return Container(_ctx)
 
     @typecheck
     def with_mounted_temp(self, path: str) -> "Container":
         """Retrieves this container plus a temporary directory mounted at the
@@ -1108,31 +1184,38 @@
 
     @typecheck
     def with_new_file(
         self,
         path: str,
         contents: Optional[str] = None,
         permissions: Optional[int] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a new file written at the given path.
 
         Parameters
         ----------
         path:
             Location of the written file (e.g., "/tmp/file.txt").
         contents:
             Content of the file to write (e.g., "Hello world!").
         permissions:
             Permission given to the written file (e.g., 0600).
             Default: 0644.
+        owner:
+            A user:group to set for the file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("contents", contents, None),
             Arg("permissions", permissions, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withNewFile", _args)
         return Container(_ctx)
 
     @typecheck
     def with_registry_auth(
         self,
@@ -1188,17 +1271,19 @@
             Arg("secret", secret),
         ]
         _ctx = self._select("withSecretVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_service_binding(self, alias: str, service: "Container") -> "Container":
-        """Establish a runtime dependency on a service. The service will be
-        started automatically when needed and detached when it is no longer
-        needed.
+        """Establish a runtime dependency on a service.
+
+        The service will be started automatically when needed and detached
+        when it is
+        no longer needed, executing the default command if none is set.
 
         The service will be reachable from the container via the provided
         hostname alias.
 
         The service dependency will also convey to any files or directories
         produced by the container.
 
@@ -1216,28 +1301,39 @@
             Arg("alias", alias),
             Arg("service", service),
         ]
         _ctx = self._select("withServiceBinding", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_unix_socket(self, path: str, source: "Socket") -> "Container":
+    def with_unix_socket(
+        self,
+        path: str,
+        source: "Socket",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a socket forwarded to the given Unix
         socket path.
 
         Parameters
         ----------
         path:
             Location of the forwarded Unix socket (e.g., "/tmp/socket").
         source:
             Identifier of the socket to forward.
+        owner:
+            A user:group to set for the mounted socket.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withUnixSocket", _args)
         return Container(_ctx)
 
     @typecheck
     def with_user(self, name: str) -> "Container":
         """Retrieves this container with a different command user.
@@ -1370,15 +1466,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("withoutUnixSocket", _args)
         return Container(_ctx)
 
     @typecheck
-    async def workdir(self) -> Optional[str]:
+    def workdir(self) -> Optional[str]:
         """Retrieves the working directory for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1389,15 +1485,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("workdir", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
 
 class Directory(Type):
     """A directory."""
 
     @typecheck
     def diff(self, other: "Directory") -> "Directory":
@@ -1432,40 +1528,45 @@
     @typecheck
     def docker_build(
         self,
         dockerfile: Optional[str] = None,
         platform: Optional[Platform] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
+        secrets: Optional[Sequence["Secret"]] = None,
     ) -> Container:
         """Builds a new Docker container from this directory.
 
         Parameters
         ----------
         dockerfile:
             Path to the Dockerfile to use (e.g., "frontend.Dockerfile").
             Defaults: './Dockerfile'.
         platform:
             The platform to build.
         build_args:
             Build arguments to use in the build.
         target:
             Target build stage to build.
+        secrets:
+            Secrets to pass to the build.
+            They will be mounted at /run/secrets/[secret-name].
         """
         _args = [
             Arg("dockerfile", dockerfile, None),
             Arg("platform", platform, None),
             Arg("buildArgs", build_args, None),
             Arg("target", target, None),
+            Arg("secrets", secrets, None),
         ]
         _ctx = self._select("dockerBuild", _args)
         return Container(_ctx)
 
     @typecheck
-    async def entries(self, path: Optional[str] = None) -> list[str]:
+    def entries(self, path: Optional[str] = None) -> list[str]:
         """Returns a list of files and directories at the given path.
 
         Parameters
         ----------
         path:
             Location of the directory to look at (e.g., "/src").
 
@@ -1483,18 +1584,18 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path, None),
         ]
         _ctx = self._select("entries", _args)
-        return await _ctx.execute(list[str])
+        return _ctx.execute_sync(list[str])
 
     @typecheck
-    async def export(self, path: str) -> bool:
+    def export(self, path: str) -> bool:
         """Writes the contents of the directory to a path on the host.
 
         Parameters
         ----------
         path:
             Location of the copied directory (e.g., "logs/").
 
@@ -1510,15 +1611,15 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("export", _args)
-        return await _ctx.execute(bool)
+        return _ctx.execute_sync(bool)
 
     @typecheck
     def file(self, path: str) -> "File":
         """Retrieves a file at the given path.
 
         Parameters
         ----------
@@ -1528,15 +1629,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("file", _args)
         return File(_ctx)
 
     @typecheck
-    async def id(self) -> DirectoryID:
+    def id(self) -> DirectoryID:
         """The content-addressed identifier of the directory.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -1549,15 +1650,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(DirectoryID)
+        return _ctx.execute_sync(DirectoryID)
 
     @typecheck
     def load_project(self, config_path: str) -> "Project":
         """load a project's metadata"""
         _args = [
             Arg("configPath", config_path),
         ]
@@ -1750,15 +1851,15 @@
 
 
 class EnvVariable(Type):
     """A simple key value object that represents an environment
     variable."""
 
     @typecheck
-    async def name(self) -> str:
+    def name(self) -> str:
         """The environment variable name.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1769,18 +1870,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def value(self) -> str:
+    def value(self) -> str:
         """The environment variable value.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1791,22 +1892,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
 
 class File(Type):
     """A file."""
 
     @typecheck
-    async def contents(self) -> str:
+    def contents(self) -> str:
         """Retrieves the contents of the file.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1817,18 +1918,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("contents", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def export(self, path: str) -> bool:
+    def export(self, path: str) -> bool:
         """Writes the file to a file path on the host.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "output.txt").
 
@@ -1844,18 +1945,18 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("export", _args)
-        return await _ctx.execute(bool)
+        return _ctx.execute_sync(bool)
 
     @typecheck
-    async def id(self) -> FileID:
+    def id(self) -> FileID:
         """Retrieves the content-addressed identifier of the file.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -1868,30 +1969,30 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(FileID)
+        return _ctx.execute_sync(FileID)
 
     @typecheck
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
-    async def size(self) -> int:
+    def size(self) -> int:
         """Gets the size of the file, in bytes.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
@@ -1902,15 +2003,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("size", _args)
-        return await _ctx.execute(int)
+        return _ctx.execute_sync(int)
 
     @typecheck
     def with_timestamps(self, timestamp: int) -> "File":
         """Retrieves this file with its created/modified timestamps set to the
         given time.
 
         Parameters
@@ -1926,15 +2027,15 @@
         return File(_ctx)
 
 
 class GitRef(Type):
     """A git ref (tag, branch or commit)."""
 
     @typecheck
-    async def digest(self) -> str:
+    def digest(self) -> str:
         """The digest of the current value of this ref.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1945,15 +2046,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("digest", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
     def tree(
         self,
         ssh_known_hosts: Optional[str] = None,
         ssh_auth_socket: Optional["Socket"] = None,
     ) -> Directory:
@@ -1981,15 +2082,15 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("branch", _args)
         return GitRef(_ctx)
 
     @typecheck
-    async def branches(self) -> list[str]:
+    def branches(self) -> list[str]:
         """Lists of branches on the repository.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2000,15 +2101,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("branches", _args)
-        return await _ctx.execute(list[str])
+        return _ctx.execute_sync(list[str])
 
     @typecheck
     def commit(self, id: str) -> GitRef:
         """Returns details on one commit.
 
         Parameters
         ----------
@@ -2034,15 +2135,15 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("tag", _args)
         return GitRef(_ctx)
 
     @typecheck
-    async def tags(self) -> list[str]:
+    def tags(self) -> list[str]:
         """Lists of tags on the repository.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2053,15 +2154,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("tags", _args)
-        return await _ctx.execute(list[str])
+        return _ctx.execute_sync(list[str])
 
 
 class Host(Type):
     """Information about the host execution environment."""
 
     @typecheck
     def directory(
@@ -2160,15 +2261,15 @@
             been superseded by :py:meth:`set_secret`
         """
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
-    async def value(self) -> str:
+    def value(self) -> str:
         """The value of this variable.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2179,22 +2280,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
 
 class Label(Type):
     """A simple key value object that represents a label."""
 
     @typecheck
-    async def name(self) -> str:
+    def name(self) -> str:
         """The label name.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2205,18 +2306,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def value(self) -> str:
+    def value(self) -> str:
         """The label value.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2227,22 +2328,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
 
 class Port(Type):
     """A port exposed by a container."""
 
     @typecheck
-    async def description(self) -> Optional[str]:
+    def description(self) -> Optional[str]:
         """The port description.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2253,18 +2354,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    async def port(self) -> int:
+    def port(self) -> int:
         """The port number.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
@@ -2275,18 +2376,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("port", _args)
-        return await _ctx.execute(int)
+        return _ctx.execute_sync(int)
 
     @typecheck
-    async def protocol(self) -> NetworkProtocol:
+    def protocol(self) -> NetworkProtocol:
         """The transport layer network protocol.
 
         Returns
         -------
         NetworkProtocol
             Transport layer network protocol associated to a port.
 
@@ -2295,15 +2396,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
-        return await _ctx.execute(NetworkProtocol)
+        return _ctx.execute_sync(NetworkProtocol)
 
 
 class Project(Type):
     """A set of scripts and/or extensions"""
 
     @typecheck
     def extensions(self) -> "Project":
@@ -2316,15 +2417,15 @@
     def generated_code(self) -> Directory:
         """Code files generated by the SDKs in the project"""
         _args: list[Arg] = []
         _ctx = self._select("generatedCode", _args)
         return Directory(_ctx)
 
     @typecheck
-    async def install(self) -> bool:
+    def install(self) -> bool:
         """install the project's schema
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
@@ -2333,18 +2434,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("install", _args)
-        return await _ctx.execute(bool)
+        return _ctx.execute_sync(bool)
 
     @typecheck
-    async def name(self) -> str:
+    def name(self) -> str:
         """name of the project
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2355,18 +2456,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
     @typecheck
-    async def schema(self) -> Optional[str]:
+    def schema(self) -> Optional[str]:
         """schema provided by the project
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2377,18 +2478,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("schema", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
     @typecheck
-    async def sdk(self) -> Optional[str]:
+    def sdk(self) -> Optional[str]:
         """sdk used to generate code for and/or execute this project
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2399,15 +2500,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sdk", _args)
-        return await _ctx.execute(Optional[str])
+        return _ctx.execute_sync(Optional[str])
 
 
 class Client(Root):
     @typecheck
     def cache_volume(self, key: str) -> CacheVolume:
         """Constructs a cache volume for a given cache key.
 
@@ -2440,15 +2541,15 @@
             Arg("id", id, None),
             Arg("platform", platform, None),
         ]
         _ctx = self._select("container", _args)
         return Container(_ctx)
 
     @typecheck
-    async def default_platform(self) -> Platform:
+    def default_platform(self) -> Platform:
         """The default platform of the builder.
 
         Returns
         -------
         Platform
             The platform config OS and architecture in a Container.  The
             format is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
@@ -2459,15 +2560,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("defaultPlatform", _args)
-        return await _ctx.execute(Platform)
+        return _ctx.execute_sync(Platform)
 
     @typecheck
     def directory(self, id: Optional[DirectoryID] = None) -> Directory:
         """Load a directory by ID. No argument produces an empty directory."""
         _args = [
             Arg("id", id, None),
         ]
@@ -2615,15 +2716,15 @@
 
 
 class Secret(Type):
     """A reference to a secret value, which can be handled more safely
     than the value itself."""
 
     @typecheck
-    async def id(self) -> SecretID:
+    def id(self) -> SecretID:
         """The identifier for this secret.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -2636,18 +2737,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(SecretID)
+        return _ctx.execute_sync(SecretID)
 
     @typecheck
-    async def plaintext(self) -> str:
+    def plaintext(self) -> str:
         """The value of this secret.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2658,20 +2759,20 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("plaintext", _args)
-        return await _ctx.execute(str)
+        return _ctx.execute_sync(str)
 
 
 class Socket(Type):
     @typecheck
-    async def id(self) -> SocketID:
+    def id(self) -> SocketID:
         """The content-addressed identifier of the socket.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -2684,15 +2785,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return await _ctx.execute(SocketID)
+        return _ctx.execute_sync(SocketID)
 
 
 __all__ = [
     "CacheID",
     "ContainerID",
     "DirectoryID",
     "FileID",
```

### Comparing `dagger_io-0.5.1/src/dagger/api/gen_sync.py` & `dagger_io-0.5.2/src/dagger/api/gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     """Label value."""
 
 
 class CacheVolume(Type):
     """A directory whose contents persist across runs."""
 
     @typecheck
-    def id(self) -> CacheID:
+    async def id(self) -> CacheID:
         """Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
         -------
         CacheID
@@ -105,53 +105,58 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(CacheID)
+        return await _ctx.execute(CacheID)
 
 
 class Container(Type):
     """An OCI-compatible container, also known as a docker container."""
 
     @typecheck
     def build(
         self,
         context: "Directory",
         dockerfile: Optional[str] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
+        secrets: Optional[Sequence["Secret"]] = None,
     ) -> "Container":
         """Initializes this container from a Dockerfile build.
 
         Parameters
         ----------
         context:
             Directory context used by the Dockerfile.
         dockerfile:
             Path to the Dockerfile to use.
             Default: './Dockerfile'.
         build_args:
             Additional build arguments.
         target:
             Target build stage to build.
+        secrets:
+            Secrets to pass to the build.
+            They will be mounted at /run/secrets/[secret-name].
         """
         _args = [
             Arg("context", context),
             Arg("dockerfile", dockerfile, None),
             Arg("buildArgs", build_args, None),
             Arg("target", target, None),
+            Arg("secrets", secrets, None),
         ]
         _ctx = self._select("build", _args)
         return Container(_ctx)
 
     @typecheck
-    def default_args(self) -> Optional[list[str]]:
+    async def default_args(self) -> Optional[list[str]]:
         """Retrieves default arguments for future commands.
 
         Returns
         -------
         Optional[list[str]]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -162,15 +167,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("defaultArgs", _args)
-        return _ctx.execute_sync(Optional[list[str]])
+        return await _ctx.execute(Optional[list[str]])
 
     @typecheck
     def directory(self, path: str) -> "Directory":
         """Retrieves a directory at the given path.
 
         Mounts are included.
 
@@ -182,15 +187,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("directory", _args)
         return Directory(_ctx)
 
     @typecheck
-    def endpoint(
+    async def endpoint(
         self,
         port: Optional[int] = None,
         scheme: Optional[str] = None,
     ) -> str:
         """Retrieves an endpoint that clients can use to reach this container.
 
         If no port is specified, the first exposed port is used. If none exist
@@ -224,18 +229,18 @@
             If the API returns an error.
         """
         _args = [
             Arg("port", port, None),
             Arg("scheme", scheme, None),
         ]
         _ctx = self._select("endpoint", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def entrypoint(self) -> Optional[list[str]]:
+    async def entrypoint(self) -> Optional[list[str]]:
         """Retrieves entrypoint to be prepended to the arguments of all commands.
 
         Returns
         -------
         Optional[list[str]]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -246,18 +251,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("entrypoint", _args)
-        return _ctx.execute_sync(Optional[list[str]])
+        return await _ctx.execute(Optional[list[str]])
 
     @typecheck
-    def env_variable(self, name: str) -> Optional[str]:
+    async def env_variable(self, name: str) -> Optional[str]:
         """Retrieves the value of the specified environment variable.
 
         Parameters
         ----------
         name:
             The name of the environment variable to retrieve (e.g., "PATH").
 
@@ -275,15 +280,15 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("envVariable", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
     def env_variables(self) -> "EnvVariable":
         """Retrieves the list of environment variables passed to commands."""
         _args: list[Arg] = []
         _ctx = self._select("envVariables", _args)
         return EnvVariable(_ctx)
@@ -331,17 +336,19 @@
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
         ]
         _ctx = self._select("exec", _args)
         return Container(_ctx)
 
     @typecheck
-    def exit_code(self) -> int:
+    async def exit_code(self) -> int:
         """Exit code of the last executed command. Zero means success.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
             - 1.
@@ -351,18 +358,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("exitCode", _args)
-        return _ctx.execute_sync(int)
+        return await _ctx.execute(int)
 
     @typecheck
-    def export(
+    async def export(
         self,
         path: str,
         platform_variants: Optional[Sequence["Container"]] = None,
     ) -> bool:
         """Writes the container as an OCI tarball to the destination file path on
         the host for the specified platform variants.
 
@@ -391,15 +398,15 @@
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
             Arg("platformVariants", platform_variants, None),
         ]
         _ctx = self._select("export", _args)
-        return _ctx.execute_sync(bool)
+        return await _ctx.execute(bool)
 
     @typecheck
     def exposed_ports(self) -> "Port":
         """Retrieves the list of exposed ports.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
@@ -450,15 +457,15 @@
             Replaced by :py:meth:`rootfs`.
         """
         _args: list[Arg] = []
         _ctx = self._select("fs", _args)
         return Directory(_ctx)
 
     @typecheck
-    def hostname(self) -> str:
+    async def hostname(self) -> str:
         """Retrieves a hostname which can be used by clients to reach this
         container.
 
         Currently experimental; set _EXPERIMENTAL_DAGGER_SERVICES_DNS=0 to
         disable.
 
         Returns
@@ -473,18 +480,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("hostname", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def id(self) -> ContainerID:
+    async def id(self) -> ContainerID:
         """A unique identifier for this container.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -498,18 +505,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(ContainerID)
+        return await _ctx.execute(ContainerID)
 
     @typecheck
-    def image_ref(self) -> Optional[str]:
+    async def image_ref(self) -> Optional[str]:
         """The unique image reference which can only be retrieved immediately
         after the 'Container.From' call.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
@@ -521,15 +528,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("imageRef", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
     def import_(
         self,
         source: "File",
         tag: Optional[str] = None,
     ) -> "Container":
@@ -553,15 +560,15 @@
             Arg("source", source),
             Arg("tag", tag, None),
         ]
         _ctx = self._select("import", _args)
         return Container(_ctx)
 
     @typecheck
-    def label(self, name: str) -> Optional[str]:
+    async def label(self, name: str) -> Optional[str]:
         """Retrieves the value of the specified label.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -574,25 +581,25 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("label", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
     def labels(self) -> "Label":
         """Retrieves the list of labels passed to container."""
         _args: list[Arg] = []
         _ctx = self._select("labels", _args)
         return Label(_ctx)
 
     @typecheck
-    def mounts(self) -> list[str]:
+    async def mounts(self) -> list[str]:
         """Retrieves the list of paths where a directory is mounted.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -603,15 +610,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("mounts", _args)
-        return _ctx.execute_sync(list[str])
+        return await _ctx.execute(list[str])
 
     @typecheck
     def pipeline(
         self,
         name: str,
         description: Optional[str] = None,
         labels: Optional[Sequence[PipelineLabel]] = None,
@@ -632,15 +639,15 @@
             Arg("description", description, None),
             Arg("labels", labels, None),
         ]
         _ctx = self._select("pipeline", _args)
         return Container(_ctx)
 
     @typecheck
-    def platform(self) -> Platform:
+    async def platform(self) -> Platform:
         """The platform this container executes and publishes as.
 
         Returns
         -------
         Platform
             The platform config OS and architecture in a Container.  The
             format is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
@@ -651,18 +658,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("platform", _args)
-        return _ctx.execute_sync(Platform)
+        return await _ctx.execute(Platform)
 
     @typecheck
-    def publish(
+    async def publish(
         self,
         address: str,
         platform_variants: Optional[Sequence["Container"]] = None,
     ) -> str:
         """Publishes this container as a new image to the specified address.
 
         Publish returns a fully qualified ref.
@@ -693,27 +700,29 @@
             If the API returns an error.
         """
         _args = [
             Arg("address", address),
             Arg("platformVariants", platform_variants, None),
         ]
         _ctx = self._select("publish", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
     def rootfs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included."""
         _args: list[Arg] = []
         _ctx = self._select("rootfs", _args)
         return Directory(_ctx)
 
     @typecheck
-    def stderr(self) -> str:
+    async def stderr(self) -> str:
         """The error stream of the last executed command.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -723,20 +732,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stderr", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def stdout(self) -> str:
+    async def stdout(self) -> str:
         """The output stream of the last executed command.
-        Errors if no command has been executed.
+
+        Will execute default command if none is set, or error if there's no
+        default.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -746,18 +757,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("stdout", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def user(self) -> Optional[str]:
+    async def user(self) -> Optional[str]:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -768,15 +779,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("user", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
     def with_default_args(
         self,
         args: Optional[Sequence[str]] = None,
     ) -> "Container":
         """Configures default arguments for future commands.
@@ -796,14 +807,15 @@
     @typecheck
     def with_directory(
         self,
         path: str,
         directory: "Directory",
         exclude: Optional[Sequence[str]] = None,
         include: Optional[Sequence[str]] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a directory written at the given path.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "/tmp/directory").
@@ -811,20 +823,26 @@
             Identifier of the directory to write
         exclude:
             Patterns to exclude in the written directory (e.g.,
             ["node_modules/**", ".gitignore", ".git/"]).
         include:
             Patterns to include in the written directory (e.g., ["*.go",
             "go.mod", "go.sum"]).
+        owner:
+            A user:group to set for the directory and its contents.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("directory", directory),
             Arg("exclude", exclude, None),
             Arg("include", include, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withDirectory", _args)
         return Container(_ctx)
 
     @typecheck
     def with_entrypoint(self, args: Sequence[str]) -> "Container":
         """Retrieves this container but with a different command entrypoint.
@@ -858,28 +876,33 @@
         _ctx = self._select("withEnvVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_exec(
         self,
         args: Sequence[str],
+        skip_entrypoint: Optional[bool] = None,
         stdin: Optional[str] = None,
         redirect_stdout: Optional[str] = None,
         redirect_stderr: Optional[str] = None,
         experimental_privileged_nesting: Optional[bool] = None,
         insecure_root_capabilities: Optional[bool] = None,
     ) -> "Container":
         """Retrieves this container after executing the specified command inside
         it.
 
         Parameters
         ----------
         args:
             Command to run instead of the container's default command (e.g.,
             ["run", "main.go"]).
+            If empty, the container's default command is used.
+        skip_entrypoint:
+            If the container has an entrypoint, ignore it for args rather than
+            using it to wrap them.
         stdin:
             Content to write to the command's standard input before closing
             (e.g., "Hello world").
         redirect_stdout:
             Redirect the command's standard output to a file in the container
             (e.g., "/tmp/stdout").
         redirect_stderr:
@@ -898,14 +921,15 @@
             flag. Containerization
             does not provide any security guarantees when using this option.
             It should only be used
             when absolutely necessary and only with trusted commands.
         """
         _args = [
             Arg("args", args),
+            Arg("skipEntrypoint", skip_entrypoint, None),
             Arg("stdin", stdin, None),
             Arg("redirectStdout", redirect_stdout, None),
             Arg("redirectStderr", redirect_stderr, None),
             Arg("experimentalPrivilegedNesting", experimental_privileged_nesting, None),
             Arg("insecureRootCapabilities", insecure_root_capabilities, None),
         ]
         _ctx = self._select("withExec", _args)
@@ -959,32 +983,39 @@
 
     @typecheck
     def with_file(
         self,
         path: str,
         source: "File",
         permissions: Optional[int] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus the contents of the given file copied to
         the given path.
 
         Parameters
         ----------
         path:
             Location of the copied file (e.g., "/tmp/file.txt").
         source:
             Identifier of the file to copy.
         permissions:
             Permission given to the copied file (e.g., 0600).
             Default: 0644.
+        owner:
+            A user:group to set for the file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
             Arg("permissions", permissions, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withFile", _args)
         return Container(_ctx)
 
     @typecheck
     def with_label(self, name: str, value: str) -> "Container":
         """Retrieves this container plus the given label.
@@ -1007,89 +1038,134 @@
     @typecheck
     def with_mounted_cache(
         self,
         path: str,
         cache: CacheVolume,
         source: Optional["Directory"] = None,
         sharing: Optional[CacheSharingMode] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a cache volume mounted at the given
         path.
 
         Parameters
         ----------
         path:
             Location of the cache directory (e.g., "/cache/node_modules").
         cache:
             Identifier of the cache volume to mount.
         source:
             Identifier of the directory to use as the cache volume's root.
         sharing:
             Sharing mode of the cache volume.
+        owner:
+            A user:group to set for the mounted cache directory.
+            Note that this changes the ownership of the specified mount along
+            with the
+            initial filesystem provided by source (if any). It does not have
+            any effect
+            if/when the cache has already been created.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("cache", cache),
             Arg("source", source, None),
             Arg("sharing", sharing, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedCache", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_directory(self, path: str, source: "Directory") -> "Container":
+    def with_mounted_directory(
+        self,
+        path: str,
+        source: "Directory",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a directory mounted at the given path.
 
         Parameters
         ----------
         path:
             Location of the mounted directory (e.g., "/mnt/directory").
         source:
             Identifier of the mounted directory.
+        owner:
+            A user:group to set for the mounted directory and its contents.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedDirectory", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_file(self, path: str, source: "File") -> "Container":
+    def with_mounted_file(
+        self,
+        path: str,
+        source: "File",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a file mounted at the given path.
 
         Parameters
         ----------
         path:
             Location of the mounted file (e.g., "/tmp/file.txt").
         source:
             Identifier of the mounted file.
+        owner:
+            A user or user:group to set for the mounted file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedFile", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_mounted_secret(self, path: str, source: "Secret") -> "Container":
+    def with_mounted_secret(
+        self,
+        path: str,
+        source: "Secret",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a secret mounted into a file at the
         given path.
 
         Parameters
         ----------
         path:
             Location of the secret file (e.g., "/tmp/secret.txt").
         source:
             Identifier of the secret to mount.
+        owner:
+            A user:group to set for the mounted secret.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withMountedSecret", _args)
         return Container(_ctx)
 
     @typecheck
     def with_mounted_temp(self, path: str) -> "Container":
         """Retrieves this container plus a temporary directory mounted at the
@@ -1108,31 +1184,38 @@
 
     @typecheck
     def with_new_file(
         self,
         path: str,
         contents: Optional[str] = None,
         permissions: Optional[int] = None,
+        owner: Optional[str] = None,
     ) -> "Container":
         """Retrieves this container plus a new file written at the given path.
 
         Parameters
         ----------
         path:
             Location of the written file (e.g., "/tmp/file.txt").
         contents:
             Content of the file to write (e.g., "Hello world!").
         permissions:
             Permission given to the written file (e.g., 0600).
             Default: 0644.
+        owner:
+            A user:group to set for the file.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("contents", contents, None),
             Arg("permissions", permissions, None),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withNewFile", _args)
         return Container(_ctx)
 
     @typecheck
     def with_registry_auth(
         self,
@@ -1188,17 +1271,19 @@
             Arg("secret", secret),
         ]
         _ctx = self._select("withSecretVariable", _args)
         return Container(_ctx)
 
     @typecheck
     def with_service_binding(self, alias: str, service: "Container") -> "Container":
-        """Establish a runtime dependency on a service. The service will be
-        started automatically when needed and detached when it is no longer
-        needed.
+        """Establish a runtime dependency on a service.
+
+        The service will be started automatically when needed and detached
+        when it is
+        no longer needed, executing the default command if none is set.
 
         The service will be reachable from the container via the provided
         hostname alias.
 
         The service dependency will also convey to any files or directories
         produced by the container.
 
@@ -1216,28 +1301,39 @@
             Arg("alias", alias),
             Arg("service", service),
         ]
         _ctx = self._select("withServiceBinding", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_unix_socket(self, path: str, source: "Socket") -> "Container":
+    def with_unix_socket(
+        self,
+        path: str,
+        source: "Socket",
+        owner: Optional[str] = None,
+    ) -> "Container":
         """Retrieves this container plus a socket forwarded to the given Unix
         socket path.
 
         Parameters
         ----------
         path:
             Location of the forwarded Unix socket (e.g., "/tmp/socket").
         source:
             Identifier of the socket to forward.
+        owner:
+            A user:group to set for the mounted socket.
+            The user and group can either be an ID (1000:1000) or a name
+            (foo:bar).
+            If the group is omitted, it defaults to the same as the user.
         """
         _args = [
             Arg("path", path),
             Arg("source", source),
+            Arg("owner", owner, None),
         ]
         _ctx = self._select("withUnixSocket", _args)
         return Container(_ctx)
 
     @typecheck
     def with_user(self, name: str) -> "Container":
         """Retrieves this container with a different command user.
@@ -1370,15 +1466,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("withoutUnixSocket", _args)
         return Container(_ctx)
 
     @typecheck
-    def workdir(self) -> Optional[str]:
+    async def workdir(self) -> Optional[str]:
         """Retrieves the working directory for all commands.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1389,15 +1485,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("workdir", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
 
 class Directory(Type):
     """A directory."""
 
     @typecheck
     def diff(self, other: "Directory") -> "Directory":
@@ -1432,40 +1528,45 @@
     @typecheck
     def docker_build(
         self,
         dockerfile: Optional[str] = None,
         platform: Optional[Platform] = None,
         build_args: Optional[Sequence[BuildArg]] = None,
         target: Optional[str] = None,
+        secrets: Optional[Sequence["Secret"]] = None,
     ) -> Container:
         """Builds a new Docker container from this directory.
 
         Parameters
         ----------
         dockerfile:
             Path to the Dockerfile to use (e.g., "frontend.Dockerfile").
             Defaults: './Dockerfile'.
         platform:
             The platform to build.
         build_args:
             Build arguments to use in the build.
         target:
             Target build stage to build.
+        secrets:
+            Secrets to pass to the build.
+            They will be mounted at /run/secrets/[secret-name].
         """
         _args = [
             Arg("dockerfile", dockerfile, None),
             Arg("platform", platform, None),
             Arg("buildArgs", build_args, None),
             Arg("target", target, None),
+            Arg("secrets", secrets, None),
         ]
         _ctx = self._select("dockerBuild", _args)
         return Container(_ctx)
 
     @typecheck
-    def entries(self, path: Optional[str] = None) -> list[str]:
+    async def entries(self, path: Optional[str] = None) -> list[str]:
         """Returns a list of files and directories at the given path.
 
         Parameters
         ----------
         path:
             Location of the directory to look at (e.g., "/src").
 
@@ -1483,18 +1584,18 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path, None),
         ]
         _ctx = self._select("entries", _args)
-        return _ctx.execute_sync(list[str])
+        return await _ctx.execute(list[str])
 
     @typecheck
-    def export(self, path: str) -> bool:
+    async def export(self, path: str) -> bool:
         """Writes the contents of the directory to a path on the host.
 
         Parameters
         ----------
         path:
             Location of the copied directory (e.g., "logs/").
 
@@ -1510,15 +1611,15 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("export", _args)
-        return _ctx.execute_sync(bool)
+        return await _ctx.execute(bool)
 
     @typecheck
     def file(self, path: str) -> "File":
         """Retrieves a file at the given path.
 
         Parameters
         ----------
@@ -1528,15 +1629,15 @@
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("file", _args)
         return File(_ctx)
 
     @typecheck
-    def id(self) -> DirectoryID:
+    async def id(self) -> DirectoryID:
         """The content-addressed identifier of the directory.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -1549,15 +1650,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(DirectoryID)
+        return await _ctx.execute(DirectoryID)
 
     @typecheck
     def load_project(self, config_path: str) -> "Project":
         """load a project's metadata"""
         _args = [
             Arg("configPath", config_path),
         ]
@@ -1750,15 +1851,15 @@
 
 
 class EnvVariable(Type):
     """A simple key value object that represents an environment
     variable."""
 
     @typecheck
-    def name(self) -> str:
+    async def name(self) -> str:
         """The environment variable name.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1769,18 +1870,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def value(self) -> str:
+    async def value(self) -> str:
         """The environment variable value.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1791,22 +1892,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
 
 class File(Type):
     """A file."""
 
     @typecheck
-    def contents(self) -> str:
+    async def contents(self) -> str:
         """Retrieves the contents of the file.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1817,18 +1918,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("contents", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def export(self, path: str) -> bool:
+    async def export(self, path: str) -> bool:
         """Writes the file to a file path on the host.
 
         Parameters
         ----------
         path:
             Location of the written directory (e.g., "output.txt").
 
@@ -1844,18 +1945,18 @@
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("path", path),
         ]
         _ctx = self._select("export", _args)
-        return _ctx.execute_sync(bool)
+        return await _ctx.execute(bool)
 
     @typecheck
-    def id(self) -> FileID:
+    async def id(self) -> FileID:
         """Retrieves the content-addressed identifier of the file.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -1868,30 +1969,30 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(FileID)
+        return await _ctx.execute(FileID)
 
     @typecheck
     def secret(self) -> "Secret":
         """Retrieves a secret referencing the contents of this file.
 
         .. deprecated::
             insecure, leaves secret in cache. Superseded by
             :py:meth:`set_secret`
         """
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
-    def size(self) -> int:
+    async def size(self) -> int:
         """Gets the size of the file, in bytes.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
@@ -1902,15 +2003,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("size", _args)
-        return _ctx.execute_sync(int)
+        return await _ctx.execute(int)
 
     @typecheck
     def with_timestamps(self, timestamp: int) -> "File":
         """Retrieves this file with its created/modified timestamps set to the
         given time.
 
         Parameters
@@ -1926,15 +2027,15 @@
         return File(_ctx)
 
 
 class GitRef(Type):
     """A git ref (tag, branch or commit)."""
 
     @typecheck
-    def digest(self) -> str:
+    async def digest(self) -> str:
         """The digest of the current value of this ref.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -1945,15 +2046,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("digest", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
     def tree(
         self,
         ssh_known_hosts: Optional[str] = None,
         ssh_auth_socket: Optional["Socket"] = None,
     ) -> Directory:
@@ -1981,15 +2082,15 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("branch", _args)
         return GitRef(_ctx)
 
     @typecheck
-    def branches(self) -> list[str]:
+    async def branches(self) -> list[str]:
         """Lists of branches on the repository.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2000,15 +2101,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("branches", _args)
-        return _ctx.execute_sync(list[str])
+        return await _ctx.execute(list[str])
 
     @typecheck
     def commit(self, id: str) -> GitRef:
         """Returns details on one commit.
 
         Parameters
         ----------
@@ -2034,15 +2135,15 @@
         _args = [
             Arg("name", name),
         ]
         _ctx = self._select("tag", _args)
         return GitRef(_ctx)
 
     @typecheck
-    def tags(self) -> list[str]:
+    async def tags(self) -> list[str]:
         """Lists of tags on the repository.
 
         Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2053,15 +2154,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("tags", _args)
-        return _ctx.execute_sync(list[str])
+        return await _ctx.execute(list[str])
 
 
 class Host(Type):
     """Information about the host execution environment."""
 
     @typecheck
     def directory(
@@ -2160,15 +2261,15 @@
             been superseded by :py:meth:`set_secret`
         """
         _args: list[Arg] = []
         _ctx = self._select("secret", _args)
         return Secret(_ctx)
 
     @typecheck
-    def value(self) -> str:
+    async def value(self) -> str:
         """The value of this variable.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2179,22 +2280,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
 
 class Label(Type):
     """A simple key value object that represents a label."""
 
     @typecheck
-    def name(self) -> str:
+    async def name(self) -> str:
         """The label name.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2205,18 +2306,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def value(self) -> str:
+    async def value(self) -> str:
         """The label value.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2227,22 +2328,22 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("value", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
 
 class Port(Type):
     """A port exposed by a container."""
 
     @typecheck
-    def description(self) -> Optional[str]:
+    async def description(self) -> Optional[str]:
         """The port description.
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2253,18 +2354,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
-    def port(self) -> int:
+    async def port(self) -> int:
         """The port number.
 
         Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
@@ -2275,18 +2376,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("port", _args)
-        return _ctx.execute_sync(int)
+        return await _ctx.execute(int)
 
     @typecheck
-    def protocol(self) -> NetworkProtocol:
+    async def protocol(self) -> NetworkProtocol:
         """The transport layer network protocol.
 
         Returns
         -------
         NetworkProtocol
             Transport layer network protocol associated to a port.
 
@@ -2295,15 +2396,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("protocol", _args)
-        return _ctx.execute_sync(NetworkProtocol)
+        return await _ctx.execute(NetworkProtocol)
 
 
 class Project(Type):
     """A set of scripts and/or extensions"""
 
     @typecheck
     def extensions(self) -> "Project":
@@ -2316,15 +2417,15 @@
     def generated_code(self) -> Directory:
         """Code files generated by the SDKs in the project"""
         _args: list[Arg] = []
         _ctx = self._select("generatedCode", _args)
         return Directory(_ctx)
 
     @typecheck
-    def install(self) -> bool:
+    async def install(self) -> bool:
         """install the project's schema
 
         Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
@@ -2333,18 +2434,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("install", _args)
-        return _ctx.execute_sync(bool)
+        return await _ctx.execute(bool)
 
     @typecheck
-    def name(self) -> str:
+    async def name(self) -> str:
         """name of the project
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2355,18 +2456,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
     @typecheck
-    def schema(self) -> Optional[str]:
+    async def schema(self) -> Optional[str]:
         """schema provided by the project
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2377,18 +2478,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("schema", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
     @typecheck
-    def sdk(self) -> Optional[str]:
+    async def sdk(self) -> Optional[str]:
         """sdk used to generate code for and/or execute this project
 
         Returns
         -------
         Optional[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2399,15 +2500,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("sdk", _args)
-        return _ctx.execute_sync(Optional[str])
+        return await _ctx.execute(Optional[str])
 
 
 class Client(Root):
     @typecheck
     def cache_volume(self, key: str) -> CacheVolume:
         """Constructs a cache volume for a given cache key.
 
@@ -2440,15 +2541,15 @@
             Arg("id", id, None),
             Arg("platform", platform, None),
         ]
         _ctx = self._select("container", _args)
         return Container(_ctx)
 
     @typecheck
-    def default_platform(self) -> Platform:
+    async def default_platform(self) -> Platform:
         """The default platform of the builder.
 
         Returns
         -------
         Platform
             The platform config OS and architecture in a Container.  The
             format is [os]/[platform]/[version] (e.g., "darwin/arm64/v7",
@@ -2459,15 +2560,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("defaultPlatform", _args)
-        return _ctx.execute_sync(Platform)
+        return await _ctx.execute(Platform)
 
     @typecheck
     def directory(self, id: Optional[DirectoryID] = None) -> Directory:
         """Load a directory by ID. No argument produces an empty directory."""
         _args = [
             Arg("id", id, None),
         ]
@@ -2615,15 +2716,15 @@
 
 
 class Secret(Type):
     """A reference to a secret value, which can be handled more safely
     than the value itself."""
 
     @typecheck
-    def id(self) -> SecretID:
+    async def id(self) -> SecretID:
         """The identifier for this secret.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -2636,18 +2737,18 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(SecretID)
+        return await _ctx.execute(SecretID)
 
     @typecheck
-    def plaintext(self) -> str:
+    async def plaintext(self) -> str:
         """The value of this secret.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
@@ -2658,20 +2759,20 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("plaintext", _args)
-        return _ctx.execute_sync(str)
+        return await _ctx.execute(str)
 
 
 class Socket(Type):
     @typecheck
-    def id(self) -> SocketID:
+    async def id(self) -> SocketID:
         """The content-addressed identifier of the socket.
 
         Note
         ----
         This is lazyly evaluated, no operation is actually run.
 
         Returns
@@ -2684,15 +2785,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
-        return _ctx.execute_sync(SocketID)
+        return await _ctx.execute(SocketID)
 
 
 __all__ = [
     "CacheID",
     "ContainerID",
     "DirectoryID",
     "FileID",
```

### Comparing `dagger_io-0.5.1/src/dagger/cli.py` & `dagger_io-0.5.2/src/dagger/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/codegen.py` & `dagger_io-0.5.2/src/dagger/codegen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/config.py` & `dagger_io-0.5.2/src/dagger/config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/connection.py` & `dagger_io-0.5.2/src/dagger/connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/context.py` & `dagger_io-0.5.2/src/dagger/context.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/engine/cli.py` & `dagger_io-0.5.2/src/dagger/engine/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/engine/conn.py` & `dagger_io-0.5.2/src/dagger/engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/engine/download.py` & `dagger_io-0.5.2/src/dagger/engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/exceptions.py` & `dagger_io-0.5.2/src/dagger/exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/log.py` & `dagger_io-0.5.2/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/server/__init__.py` & `dagger_io-0.5.2/src/dagger/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/server/cli.py` & `dagger_io-0.5.2/src/dagger/server/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/server/converter.py` & `dagger_io-0.5.2/src/dagger/server/converter.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/session.py` & `dagger_io-0.5.2/src/dagger/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/src/dagger/transport/httpx.py` & `dagger_io-0.5.2/src/dagger/transport/httpx.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.5.1/setup.py` & `dagger_io-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,23 @@
  'beartype>=0.11.0',
  'cattrs>=22.2.0',
  'gql>=3.4.0',
  'graphql-core>=3.2.3',
  'httpx>=0.23.1',
  'platformdirs>=2.6.2',
  'rich>=12.6.0',
- 'typer[all]>=0.6.1']
+ 'typer[all]>=0.6.1',
+ 'typing_extensions>=4.4.0']
 
 extras_require = \
 {'server': ['strawberry-graphql>=0.133.5']}
 
 setup_kwargs = {
     'name': 'dagger-io',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'A client package for running Dagger pipelines in Python.',
     'long_description': '# Dagger Python SDK\n\n[![PyPI Version](https://img.shields.io/pypi/v/dagger-io)](https://pypi.org/project/dagger-io/) \n[![Conda Version](https://img.shields.io/conda/vn/conda-forge/dagger-io.svg)](https://anaconda.org/conda-forge/dagger-io)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/dagger-io.svg)](https://pypi.org/project/dagger-io/)\n[![License](https://img.shields.io/pypi/l/dagger-io.svg)](https://pypi.python.org/pypi/dagger-io)\n[![Code style](https://img.shields.io/badge/code%20style-black-black.svg)](https://github.com/psf/black)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)\n\nA client package for running [Dagger](https://dagger.io/) pipelines.\n\n## What is the Dagger Python SDK?\n\nThe Dagger Python SDK contains everything you need to develop CI/CD pipelines in Python, and run them on any OCI-compatible container runtime.\n\n## Requirements\n\n- Python 3.10 or later\n- [Docker](https://docs.docker.com/engine/install/), or another OCI-compatible container runtime\n\nA compatible version of the  [Dagger CLI](https://docs.dagger.io/cli) is automatically downloaded and run by the SDK for you, although it’s possible to manage it manually.\n\n## Installation\n\nFrom [PyPI](https://pypi.org/project/dagger-io/), using `pip`:\n\n```shell\npip install dagger-io\n```\n\nYou can also install via [Conda](https://anaconda.org/conda-forge/dagger-io), from the [conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-conda-forge) channel:\n\n```shell\nconda install dagger-io\n```\n\n## Example\n\nCreate a `main.py` file:\n\n```python\nimport sys\n\nimport anyio\nimport dagger\n\n\nasync def main(args: list[str]):\n    async with dagger.Connection() as client:\n        # build container with cowsay entrypoint\n        ctr = (\n            client.container()\n            .from_("python:alpine")\n            .with_exec(["pip", "install", "cowsay"])\n            .with_entrypoint(["cowsay"])\n        )\n\n        # run cowsay with requested message\n        result = await ctr.with_exec(args).stdout()\n\n    print(result)\n\n\nanyio.run(main, sys.argv[1:])\n```\n\nRun with:\n\n```console\n$ python main.py "Simple is better than complex"\n  _____________________________\n| Simple is better than complex |\n  =============================\n                             \\\n                              \\\n                                ^__^\n                                (oo)\\_______\n                                (__)\\       )\\/\\\n                                    ||----w |\n                                    ||     ||\n```\n\n> **Note**\n> It may take a while for it to finish, especially on first run with cold cache.\n\nIf you need to debug, you can stream the logs from the engine with the `log_output`  config:\n\n```python\nconfig = dagger.Config(log_output=sys.stderr)\nasync with dagger.Connection(config) as client:\n    ...\n```\n\n## Learn more\n\n- [Documentation](https://docs.dagger.io/sdk/python)\n- [API Reference](https://dagger-io.readthedocs.org)\n- [Source code](https://github.com/dagger/dagger/tree/main/sdk/python)\n\n## Development\n\nThis library is maintained with [Poetry](https://python-poetry.org/docs/).\n\nIf you already have a [Python 3.10 or later](https://docs.python.org/3/using/index.html) interpreter in your `$PATH`, you can let [Poetry manage](https://python-poetry.org/docs/basic-usage/#using-your-virtual-environment) the [virtual environment](https://packaging.python.org/en/latest/tutorials/installing-packages/#creating-virtual-environments) automatically. Otherwise you need to activate it first, before installing dependencies:\n\n```shell\npoetry install\n```\n\nThe following commands are available:\n- `poe test`: Run tests.\n- `poe fmt`: Re-format code following common styling conventions.\n- `poe lint`: Check for linting violations.\n- `poe generate`: Regenerate API client after changes to the codegen.\n- `poe docs`: Build reference docs locally.\n\n### Engine changes\n\nTesting and regenerating the client may fail if there’s changes in the engine code that haven’t been released yet. \n\nThe simplest way to run those commands locally with the most updated engine version is to build it using [Dagger’s CI pipelines](https://github.com/dagger/dagger/blob/main/internal/mage/sdk/python.go) :\n\n```shell\n../../hack/make sdk:python:test\n../../hack/make sdk:python:generate\n```\n\nYou can also build the CLI and use it directly within the Python SDK:\n\n```shell\n../../hack/dev poe test\n```\n\nOr build it separately and tell the SDK to use it directly (or any other CLI binary):\n\n```shell\n../../hack/make\n_EXPERIMENTAL_DAGGER_CLI_BIN=../../bin/dagger poe test\n```\n\n',
     'author': 'Dagger',
     'author_email': 'hello@dagger.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://dagger.io',
```

### Comparing `dagger_io-0.5.1/PKG-INFO` & `dagger_io-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.5.1
+Version: 0.5.2
 Summary: A client package for running Dagger pipelines in Python.
 Home-page: https://dagger.io
 License: Apache-2.0
 Author: Dagger
 Author-email: hello@dagger.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -29,14 +29,15 @@
 Requires-Dist: gql (>=3.4.0)
 Requires-Dist: graphql-core (>=3.2.3)
 Requires-Dist: httpx (>=0.23.1)
 Requires-Dist: platformdirs (>=2.6.2)
 Requires-Dist: rich (>=12.6.0)
 Requires-Dist: strawberry-graphql (>=0.133.5) ; extra == "server"
 Requires-Dist: typer[all] (>=0.6.1)
+Requires-Dist: typing_extensions (>=4.4.0)
 Project-URL: Community, https://discord.gg/ufnyBtc8uY
 Project-URL: Documentation, https://docs.dagger.io/sdk/python
 Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
 Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
 Project-URL: Tracker, https://github.com/dagger/dagger/issues
 Project-URL: Twitter, https://twitter.com/dagger_io
 Description-Content-Type: text/markdown
```

