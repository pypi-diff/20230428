# Comparing `tmp/techbureau-symbol-sdk-python-3.0.3.dev3.tar.gz` & `tmp/techbureau-symbol-sdk-python-3.0.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "techbureau-symbol-sdk-python-3.0.3.dev3.tar", last modified: Wed Mar 29 08:36:10 2023, max compression
+gzip compressed data, was "techbureau-symbol-sdk-python-3.0.7.dev1.tar", last modified: Fri Apr 28 03:51:36 2023, max compression
```

## Comparing `techbureau-symbol-sdk-python-3.0.3.dev3.tar` & `techbureau-symbol-sdk-python-3.0.7.dev1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.038034 techbureau-symbol-sdk-python-3.0.3.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-29 08:36:10.038034 techbureau-symbol-sdk-python-3.0.3.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 08:36:10.038034 techbureau-symbol-sdk-python-3.0.3.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/ArrayHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BaseValue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Bip32.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BlockchainSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BufferReader.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BufferWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/ByteArray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/CryptoTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/NetworkTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/QrSignatureStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/QrStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/external/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/external/ed25519.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/
--rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/BatchOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/NemFacade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nc/
--rw-r--r--   0 runner    (1001) docker     (123)   178806 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/KeyPair.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/ripemd160.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.034034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/sc/
--rw-r--r--   0 runner    (1001) docker     (123)   477712 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/sc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.038034 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/KeyPair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Merkle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/SharedKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:03.000000 techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 08:36:10.038034 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-29 08:36:10.000000 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-29 08:36:10.000000 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 08:36:10.000000 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-29 08:36:10.000000 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-29 08:36:10.000000 techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ArrayHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BaseValue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Bip32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BlockchainSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferReader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ByteArray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CryptoTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/ed25519.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/NemFacade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)   178806 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/KeyPair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ripemd160.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.053877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/
+-rw-r--r--   0 runner    (1001) docker     (123)   477712 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Merkle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:26.000000 techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 03:51:36.057877 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 03:51:36.000000 techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/top_level.txt
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/setup.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,35 +9,27 @@
    'symbolchain.external',
    'symbolchain.sc',
    'symbolchain.symbol']
 
 package_data = \
 {'': ['*']}
 
-install_requires = \
-['cryptography==38.0.1',
-    'mnemonic==0.20',
-    'Pillow==9.2.0',
-    'pynacl==1.5.0',
-    'pysha3==1.0.2',
-    'PyYAML==6.0',
-    'pyzbar==0.1.9',
-    'ripemd-hash==1.0.0',
-    'qrcode==7.3.1']
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
 
 setup_kwargs = {
     'name': 'techbureau-symbol-sdk-python',
-    'version': '3.0.3.dev3',
+    'version': '3.0.7.dev1',
     'description': 'Symbol SDK',
     'long_description': 'This is symbol project core sdk python library.',
     'author': 'Techbureau Contributors',
     'author_email': 'development@techbureau.jp',
     'maintainer': 'Techbureau Contributors',
     'maintainer_email': 'development@techbureau.jp',
     'url': 'https://github.com/tech-bureau-jp/symbol/tree/dev/sdk/python',
     'packages': packages,
     'package_data': package_data,
-    'install_requires': install_requires,
+    'install_requires': requirements,
     'python_requires': '>=3.7,<4.0',
 }
 
 setup(**setup_kwargs)
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/AccountDescriptorRepository.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/ArrayHelpers.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BaseValue.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Bip32.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BlockchainSettings.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BufferReader.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/BufferWriter.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/ByteArray.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Cipher.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/CodeWordsEncoder.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/CryptoTypes.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/DiceMnemonicGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/NetworkTimestamp.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/NodeDescriptorRepository.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/PrivateKeyStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/QrSignatureStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/QrStorage.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/RuleBasedTransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/SharedKey.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/TransactionDescriptorProcessor.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/TransactionDescriptorProcessor.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/external/ed25519.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/BatchOperations.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/NemFacade.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/NemFacade.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/facade/SymbolFacade.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/facade/SymbolFacade.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import sha3
+import hashlib
 
 from .. import sc
 from ..CryptoTypes import Hash256, PublicKey, Signature
 from ..Network import NetworkLocator
 from ..symbol.KeyPair import KeyPair, Verifier
 from ..symbol.Merkle import MerkleHashBuilder
 from ..symbol.Network import Address, Network
@@ -56,15 +56,15 @@
 		return {
 			Address: 'address',
 			PublicKey: 'public_key',
 		}
 
 	def hash_transaction(self, transaction):
 		"""Hashes a Symbol transaction."""
-		hasher = sha3.sha3_256()
+		hasher = hashlib.sha3_256()
 		hasher.update(transaction.signature.bytes)
 		hasher.update(transaction.signer_public_key.bytes)
 		hasher.update(self.network.generation_hash_seed.bytes)
 		hasher.update(self._transaction_data_buffer(transaction.serialize()))
 		return Hash256(hasher.digest())
 
 	def sign_transaction(self, key_pair, transaction):
@@ -93,15 +93,15 @@
 		return cosignature
 
 	@staticmethod
 	def hash_embedded_transactions(embedded_transactions):
 		"""Hashes embedded transactions of an aggregate."""
 		hash_builder = MerkleHashBuilder()
 		for embedded_transaction in embedded_transactions:
-			hash_builder.update(Hash256(sha3.sha3_256(embedded_transaction.serialize()).digest()))
+			hash_builder.update(Hash256(hashlib.sha3_256(embedded_transaction.serialize()).digest()))
 
 		return hash_builder.final()
 
 	def bip32_path(self, account_id):
 		"""Creates a network compatible BIP32 path for the specified account."""
 		return [44, 4343 if 'mainnet' == self.network.name else 1, account_id, 0, 0]
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nc/__init__.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nc/__init__.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/KeyPair.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/MessageEncoder.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/SharedKey.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/nem/TransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/nem/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/sc/__init__.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/IdGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/IdGenerator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import sha3
+import hashlib
 
 NAMESPACE_FLAG = 1 << 63
 
 
 def generate_mosaic_id(owner_address, nonce):
 	"""Generates a mosaic id from an owner address and a nonce."""
-	hasher = sha3.sha3_256()
+	hasher = hashlib.sha3_256()
 	hasher.update(nonce.to_bytes(4, 'little'))
 	hasher.update(owner_address.bytes)
 	digest = hasher.digest()
 
 	result = int.from_bytes(digest[0:8], 'little')
 	if result & NAMESPACE_FLAG:
 		result -= NAMESPACE_FLAG
 
 	return result
 
 
 def generate_namespace_id(name, parent_namespace_id=0):
 	"""Generates a namespace id from a name and an optional parent namespace id."""
-	hasher = sha3.sha3_256()
+	hasher = hashlib.sha3_256()
 	hasher.update(parent_namespace_id.to_bytes(8, 'little'))
 	hasher.update(name.encode('utf8'))
 	digest = hasher.digest()
 
 	result = int.from_bytes(digest[0:8], 'little')
 	return result | NAMESPACE_FLAG
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/KeyPair.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Merkle.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Merkle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import hashlib
 from binascii import hexlify
 from collections import namedtuple
 from enum import Enum
 from functools import reduce
 
-import sha3
-
 from ..BufferReader import BufferReader
 from ..CryptoTypes import Hash256
 
 MerklePart = namedtuple('MerklePart', ['hash', 'is_left'])
 PatriciaTreePath = namedtuple('PatriciaTreePath', ['path', 'size'])
 
 # region MerkleHashBuilder
@@ -30,15 +29,15 @@
 		if not self.hashes:
 			return Hash256.zero()
 
 		num_remaining_hashes = len(self.hashes)
 		while num_remaining_hashes > 1:
 			i = 0
 			while i < num_remaining_hashes:
-				hasher = sha3.sha3_256()
+				hasher = hashlib.sha3_256()
 				hasher.update(self.hashes[i])
 
 				if i + 1 < num_remaining_hashes:
 					hasher.update(self.hashes[i + 1])
 				else:
 					# if there is an odd number of hashes, duplicate the last one
 					hasher.update(self.hashes[i])
@@ -59,15 +58,15 @@
 def prove_merkle(leaf_hash, merkle_path, root_hash):
 	"""
 	Proves a merkle hash.
 	Merkle *hash chain* path is ordered from leaf to root, where each element is MerklePart.
 	"""
 
 	def calculate_next_hash(working_hash, merkle_part):
-		hasher = sha3.sha3_256()
+		hasher = hashlib.sha3_256()
 		if merkle_part.is_left:
 			hasher.update(merkle_part.hash.bytes)
 			hasher.update(working_hash.bytes)
 		else:
 			hasher.update(working_hash.bytes)
 			hasher.update(merkle_part.hash.bytes)
 
@@ -96,41 +95,54 @@
 	while i < path.size:
 		buffer.append((_get_nibble_at(path, i) << 4) + _get_nibble_at(path, i + 1))
 		i += 2
 
 	return bytes(buffer)
 
 
-class LeafNode:
+class TreeNode:
+	"""Node in a compact patricia tree."""
+
+	def __init__(self, path):
+		self.path = path
+
+	@property
+	def hex_path(self):
+		"""Gets hex representation of path."""
+
+		return hexlify(self.path.path).decode('utf8').upper()[:self.path.size]
+
+
+class LeafNode(TreeNode):
 	"""Leaf node in a compact patricia tree."""
 
 	def __init__(self, path, value):
-		self.path = path
+		super().__init__(path)
 		self.value = value
 
 	def calculate_hash(self):
 		"""Calculates node hash."""
 
-		hasher = sha3.sha3_256()
+		hasher = hashlib.sha3_256()
 		hasher.update(_encode_path(self.path, True))
 		hasher.update(self.value.bytes)
 		return Hash256(hasher.digest())
 
 
-class BranchNode:
+class BranchNode(TreeNode):
 	"""Branch node in a compact patricia tree."""
 
 	def __init__(self, path, links):
-		self.path = path
+		super().__init__(path)
 		self.links = links
 
 	def calculate_hash(self):
 		"""Calculates node hash."""
 
-		hasher = sha3.sha3_256()
+		hasher = hashlib.sha3_256()
 		hasher.update(_encode_path(self.path, False))
 		for link in self.links:
 			hasher.update((link if link else Hash256.zero()).bytes)
 
 		return Hash256(hasher.digest())
 
 # endregion
@@ -194,15 +206,15 @@
 	UNANCHORED_PATH_TREE = 0x8002  # root of the path tree being proven is not a subcache merkle root
 	LEAF_VALUE_MISMATCH = 0x8003  # leaf value does not match expected value
 	UNLINKED_NODE = 0x8004  # provided merkle hash contains an unlinked node
 	PATH_MISMATCH = 0x8005  # actual merkle path does not match encoded key
 
 
 def _check_state_hash(state_hash, subcache_merkle_roots):
-	hasher = sha3.sha3_256()
+	hasher = hashlib.sha3_256()
 	for root in subcache_merkle_roots:
 		hasher.update(root.bytes)
 
 	return state_hash == Hash256(hasher.digest())
 
 
 def prove_patricia_merkle(encoded_key, value_to_test, merkle_path, state_hash, subcache_merkle_roots):
@@ -233,15 +245,15 @@
 		if child_hash:
 			if child_hash not in node.links:
 				return PatriciaMerkleProofResult.UNLINKED_NODE
 
 			formatted_link_index = f'{node.links.index(child_hash):01X}'
 
 		child_hash = node_hash
-		actual_path = f'{formatted_link_index}{hexlify(node.path.path).decode("utf8").upper()}{actual_path}'
+		actual_path = f'{formatted_link_index}{node.hex_path}{actual_path}'
 
 	if is_positive_proof:
 		# for positive proof, expected and calculated paths must match exactly
 		return PatriciaMerkleProofResult.PATH_MISMATCH if actual_path != str(encoded_key) else PatriciaMerkleProofResult.VALID_POSITIVE
 
 	# for negative proof, expected path must start with calculated path and next nibble must be a dead end
 	if not str(encoded_key).startswith(actual_path):
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/MessageEncoder.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/MessageEncoder.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Metadata.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Metadata.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/Network.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/Network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import base64
 import datetime
-
-import sha3
+import hashlib
 
 from ..ByteArray import ByteArray
 from ..CryptoTypes import Hash256
 from ..Network import Network as BasicNetwork
 from ..NetworkTimestamp import NetworkTimestamp as BasicNetworkTimestamp
 from ..NetworkTimestamp import NetworkTimestampDatetimeConverter
 
@@ -49,15 +48,15 @@
 
 	def __init__(self, name, identifier, epoch_time, generation_hash_seed=None):
 		"""Creates a new network with the specified properties."""
 		super().__init__(name, identifier, NetworkTimestampDatetimeConverter(epoch_time, 'milliseconds'), Address, NetworkTimestamp)
 		self.generation_hash_seed = generation_hash_seed
 
 	def address_hasher(self):
-		return sha3.sha3_256()
+		return hashlib.sha3_256()
 
 	def create_address(self, address_without_checksum, checksum):
 		return Address(address_without_checksum + checksum[0:3])
 
 
 Network.MAINNET = Network(
 	'mainnet',
```

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/TransactionFactory.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/TransactionFactory.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/symbolchain/symbol/VotingKeysGenerator.py` & `techbureau-symbol-sdk-python-3.0.7.dev1/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*

### Comparing `techbureau-symbol-sdk-python-3.0.3.dev3/techbureau_symbol_sdk_python.egg-info/SOURCES.txt` & `techbureau-symbol-sdk-python-3.0.7.dev1/techbureau_symbol_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

