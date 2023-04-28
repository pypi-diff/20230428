# Comparing `tmp/quorum_eth_py-0.1.0.tar.gz` & `tmp/quorum_eth_py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quorum_eth_py-0.1.0.tar", last modified: Fri Apr 28 07:56:01 2023, max compression
+gzip compressed data, was "quorum_eth_py-0.1.1.tar", last modified: Fri Apr 28 08:33:35 2023, max compression
```

## Comparing `quorum_eth_py-0.1.0.tar` & `quorum_eth_py-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:56:01.005019 quorum_eth_py-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      834 2023-04-28 07:56:01.004019 quorum_eth_py-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:56:00.991447 quorum_eth_py-0.1.0/quorum_eth_py/
--rw-rw-rw-   0        0        0      310 2023-04-28 07:33:33.000000 quorum_eth_py-0.1.0/quorum_eth_py/__init__.py
--rw-rw-rw-   0        0        0     1783 2023-04-28 07:34:33.000000 quorum_eth_py-0.1.0/quorum_eth_py/_browser.py
--rw-rw-rw-   0        0        0     2596 2023-04-28 07:48:17.000000 quorum_eth_py-0.1.0/quorum_eth_py/_eth.py
--rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.1.0/quorum_eth_py/_http.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:56:01.001439 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/
--rw-rw-rw-   0        0        0      834 2023-04-28 07:56:00.000000 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-04-28 07:56:00.000000 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 07:56:00.000000 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 07:56:00.000000 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-28 07:56:00.000000 quorum_eth_py-0.1.0/quorum_eth_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-28 07:56:01.005019 quorum_eth_py-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1127 2023-04-28 07:54:18.000000 quorum_eth_py-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.427015 quorum_eth_py-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-04-28 08:33:35.426040 quorum_eth_py-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2023-04-28 06:27:56.000000 quorum_eth_py-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.415070 quorum_eth_py-0.1.1/quorum_eth_py/
+-rw-rw-rw-   0        0        0      310 2023-04-28 08:32:15.000000 quorum_eth_py-0.1.1/quorum_eth_py/__init__.py
+-rw-rw-rw-   0        0        0     1783 2023-04-28 07:34:33.000000 quorum_eth_py-0.1.1/quorum_eth_py/_browser.py
+-rw-rw-rw-   0        0        0     2703 2023-04-28 08:28:18.000000 quorum_eth_py-0.1.1/quorum_eth_py/_eth.py
+-rw-rw-rw-   0        0        0     1801 2023-04-28 06:34:10.000000 quorum_eth_py-0.1.1/quorum_eth_py/_http.py
+drwxrwxrwx   0        0        0        0 2023-04-28 08:33:35.424046 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 08:33:35.000000 quorum_eth_py-0.1.1/quorum_eth_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 08:33:35.428012 quorum_eth_py-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2023-04-28 08:32:15.000000 quorum_eth_py-0.1.1/setup.py
```

### Comparing `quorum_eth_py-0.1.0/LICENSE` & `quorum_eth_py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.1.0/PKG-INFO` & `quorum_eth_py-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum_eth_py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.1.0/quorum_eth_py/_browser.py` & `quorum_eth_py-0.1.1/quorum_eth_py/_browser.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.1.0/quorum_eth_py/_eth.py` & `quorum_eth_py-0.1.1/quorum_eth_py/_eth.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,44 +25,47 @@
         self.browser = RumEthChainBrowser(contract_address)
         self.owner = self.w3.eth.account.from_key(owner_pvtkey)
         self.w3.eth.default_account = self.owner.address
         self.contract_instance = self.w3.eth.contract(contract_address, abi=abi)
         contract_name = self.contract_instance.functions.name().call()
         logger.info("contract %s: %s", contract_name, contract_address)
 
-    def mint_nft(self, to_address, minter_pvtkey=None, unique_mint=True):
+    def mint_nft(self, to_address: str, unique_mint=True, minter_pvtkey=None):
         """mint nft to address"""
         to_address = self.w3.toChecksumAddress(to_address)
         if unique_mint:
             minted = self.browser.is_minted(to_address)
             logger.info(
                 "%s minted: %s of %s ",
                 to_address,
                 minted,
                 self.contract_instance.address,
             )
             if minted:
                 logger.info("%s already minted", to_address)
                 return True
-        minter = self.w3.eth.account.from_key(minter_pvtkey) or self.owner
+        minter = self.owner
+        if minter_pvtkey:
+            minter = self.w3.eth.account.from_key(minter_pvtkey)
         options = {
             "gas": 1000000,
             "gasPrice": self.w3.toWei("1", "gwei"),
             "from": minter.address,
             "nonce": self.w3.eth.getTransactionCount(minter.address),
         }
         tx = self.contract_instance.functions.mint(to_address).buildTransaction(options)
         signed = minter.signTransaction(tx)
         tx_id = self.w3.eth.sendRawTransaction(signed.rawTransaction)
         tx_id_hex = tx_id.hex()
         logger.info("mint to %s is done by trx: %s", to_address, tx_id_hex)
         return tx_id_hex
 
-    def get_balance(self, address):
+    def get_balance(self, address: str):
         """get balance of address"""
+        address = self.w3.toChecksumAddress(address)
         balance = self.contract_instance.functions.balanceOf(address).call()
         print("balance: ", balance)
         return balance
 
     def get_total_supply(self):
         """get total supply"""
         return self.contract_instance.functions.totalSupply().call()
```

### Comparing `quorum_eth_py-0.1.0/quorum_eth_py/_http.py` & `quorum_eth_py-0.1.1/quorum_eth_py/_http.py`

 * *Files identical despite different names*

### Comparing `quorum_eth_py-0.1.0/quorum_eth_py.egg-info/PKG-INFO` & `quorum_eth_py-0.1.1/quorum_eth_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quorum-eth-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python sdk for quorum-eth chain
 Home-page: https://github.com/liujuanjuan1984/quorum_eth_py
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/quorum_eth_py
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/quorum_eth_py/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `quorum_eth_py-0.1.0/setup.py` & `quorum_eth_py-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="quorum_eth_py",
-    version="0.1.0",
+    version="0.1.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A python sdk for quorum-eth chain",
     keywords=["rumsystem", "quorum", "eth", "sdk", "blockchain"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/quorum_eth_py",
```

