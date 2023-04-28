# Comparing `tmp/vvault-0.0.2.tar.gz` & `tmp/vvault-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vvault-0.0.2.tar", max compression
+gzip compressed data, was "vvault-0.0.3.tar", max compression
```

## Comparing `vvault-0.0.2.tar` & `vvault-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11356 2023-04-04 22:10:51.980161 vvault-0.0.2/LICENSE
--rw-r--r--   0        0        0     1774 2023-04-04 22:10:51.980161 vvault-0.0.2/README.md
--rw-r--r--   0        0        0      750 2023-04-04 22:10:51.980161 vvault-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 22:10:51.980161 vvault-0.0.2/vvault/__init__.py
--rw-r--r--   0        0        0      157 2023-04-04 22:10:51.980161 vvault-0.0.2/vvault/logger.py
--rw-r--r--   0        0        0     9016 2023-04-04 22:10:51.984161 vvault-0.0.2/vvault/vault.py
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 vvault-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-04-28 12:54:50.063653 vvault-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1996 2023-04-28 12:54:50.063653 vvault-0.0.3/README.md
+-rw-r--r--   0        0        0      750 2023-04-28 12:54:50.063653 vvault-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/logger.py
+-rw-r--r--   0        0        0     9517 2023-04-28 12:54:50.063653 vvault-0.0.3/vvault/vault.py
+-rw-r--r--   0        0        0     2522 1970-01-01 00:00:00.000000 vvault-0.0.3/PKG-INFO
```

### Comparing `vvault-0.0.2/LICENSE` & `vvault-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vvault-0.0.2/README.md` & `vvault-0.0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 VVault
 ==
 
 
 # Stats
-
+<img src="https://img.shields.io/pypi/dm/vvault?style=for-the-badge" alt="pypi">
 
 Based on
 * hvac
 * vault
 
+Start
+==
+poetry
+```shell
+poetry add vvault
+```
+pip
+```shell
+pip install vvault
+```
+import
+```python
+from vvault.vault import VaultMaster
+```
+
 Config for vault (services.yaml)
 ==
 ```yaml
 ---
 environments:
   dev:
     services:
```

### Comparing `vvault-0.0.2/pyproject.toml` & `vvault-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vvault"
-version = "0.0.2"
+version = "0.0.3"
 readme = "README.md"
 packages = [{include = "vvault"}]
 authors = ["StepanGavrilov <gavrilovstepan78@gmail.com>"]
 description = "Python Client for vault"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `vvault-0.0.2/vvault/vault.py` & `vvault-0.0.3/vvault/vault.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,31 +35,53 @@
         return self.client.sys.list_policies()
 
     @property
     def userpasses(self) -> list:
         userpass_data = self.client.auth.userpass.list_user()
         return userpass_data.get("data", {}).get("keys")
 
+    def __initialize(self):
+        ...
+
+    def __unseal(self):
+        logger.info("Unsealing")
+        self.client.sys.submit_unseal_keys(self.__unseal_keys[0:3])
+        logger.info(f'initialized: {self.client.seal_status.get("initialized")}')
+        logger.info(f'sealed: {self.client.seal_status.get("sealed")}')
+        self.client = hvac.Client(url=self.url, token=self.__root_token)
+        logger.info(
+            f"Client authenticated (master token): {self.client.is_authenticated()}"
+        )
+
+        # enable auth methods
+        self.enable_auth_methods(auth_methods=self._auth_methods)
+
+        self.__init_config()
+
     def start(
         self,
         config_file: Path,
-        unseal_keys: tuple[str] | None = None,
+        unseal_keys: tuple[str, ...] | None = None,
         root_token=None,
+        update: bool = False,
     ) -> dict:
         """
         :param config_file: required
         :param unseal_keys:
         :param root_token: optional, if it's not first start
+        :param update: optional, set True if we need updates from config
         """
 
         if not config_file.exists():
             raise FileNotFoundError(f"No config file by path: {config_file}")
 
         self.__parse_config_file(config_file)
-        start_response = self.__start(root_token=root_token, unseal_keys=unseal_keys)
+        start_response = self.__start(
+            root_token=root_token, unseal_keys=unseal_keys, update=update
+        )
         return start_response
 
     def __parse_config_file(self, config_file: Path) -> None:
         logger.info(f"Config exists: {config_file}")
         with open(config_file) as stream:
             try:
                 self.config = yaml.safe_load(stream)
@@ -69,27 +91,21 @@
     def __init(self) -> None:
         """
         :return:
         """
         logger.info("Initializing")
         vault_init_data: dict[str, Any] = self.client.sys.initialize(5, 3)
         # Get vault init data
-        self.__unseal_keys: tuple[str] = tuple(
+        self.__unseal_keys: tuple[str, ...] = tuple(
             vault_init_data.get("keys", None)
         )  # type: ignore
         self.__root_token = vault_init_data.get("root_token", None)
         logger.info(f"root token: {self.__root_token}")
         logger.info(f"unseal keys (5): {self.__unseal_keys}")
 
-    def __unseal(self) -> None:
-        logger.info("Unsealing")
-        self.client.sys.submit_unseal_keys(self.__unseal_keys[0:3])
-        logger.info(f'initialized: {self.client.seal_status.get("initialized")}')
-        logger.info(f'sealed: {self.client.seal_status.get("sealed")}')
-
     def __init_config(self) -> None:
         """
         config settings to vault
         """
 
         # set kv
         logger.info("Start Installing ENVS")
@@ -215,15 +231,15 @@
         """
         self.client.sys.create_or_update_policy(
             name=area,
             policy=service,
         )
 
     def __start(
-        self, root_token: str | None, unseal_keys: tuple[str] | None
+        self, root_token: str | None, unseal_keys: tuple[str, ...] | None, update: bool
     ) -> dict[str, str | tuple[str, ...] | None]:
         if root_token:
             self.__root_token = root_token
         if unseal_keys:
             self.__unseal_keys = unseal_keys
 
         logger.info("Starting vault-master . . . .")
@@ -241,20 +257,22 @@
         # first start
         if not self.client.seal_status.get("initialized"):
             self.__init()
 
         # if init (need root token and unsealed keys from input)
         if self.client.seal_status.get("sealed"):
             self.__unseal()
+
         self.client = hvac.Client(url=self.url, token=self.__root_token)
+
+        if update:
+            logger.info(f"Updating config: {update}")
+            self.__init_config()
+
         logger.info(
             f"Client authenticated (master token): {self.client.is_authenticated()}"
         )
 
-        # enable auth methods
-        self.enable_auth_methods(auth_methods=self._auth_methods)
-        self.__init_config()
-
         return {
             "root_token": self.__root_token,
             "unseal_keys": self.__unseal_keys,
         }
```

### Comparing `vvault-0.0.2/PKG-INFO` & `vvault-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vvault
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Client for vault
 Author: StepanGavrilov
 Author-email: gavrilovstepan78@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -15,20 +15,35 @@
 Description-Content-Type: text/markdown
 
 VVault
 ==
 
 
 # Stats
-
+<img src="https://img.shields.io/pypi/dm/vvault?style=for-the-badge" alt="pypi">
 
 Based on
 * hvac
 * vault
 
+Start
+==
+poetry
+```shell
+poetry add vvault
+```
+pip
+```shell
+pip install vvault
+```
+import
+```python
+from vvault.vault import VaultMaster
+```
+
 Config for vault (services.yaml)
 ==
 ```yaml
 ---
 environments:
   dev:
     services:
```

