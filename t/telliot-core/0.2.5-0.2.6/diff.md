# Comparing `tmp/telliot_core-0.2.5.tar.gz` & `tmp/telliot_core-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telliot_core-0.2.5.tar", last modified: Mon Apr 17 17:02:59 2023, max compression
+gzip compressed data, was "telliot_core-0.2.6.tar", last modified: Fri Apr 28 18:30:06 2023, max compression
```

## Comparing `telliot_core-0.2.5.tar` & `telliot_core-0.2.6.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.575097 telliot_core-0.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.555097 telliot_core-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.github/workflows/py39.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.github/workflows/typing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-17 17:02:50.000000 telliot_core-0.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-17 17:02:50.000000 telliot_core-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-17 17:02:59.575097 telliot_core-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-17 17:02:50.000000 telliot_core-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-17 17:02:50.000000 telliot_core-0.2.5/brownie-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/contracts/Integrations/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/Integrations/DIVAOracleMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/Integrations/DIVAProtocolMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/contracts/TellorFlex/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/TellorFlex/AutopayMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/TellorFlex/TellorFlex.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/contracts/TellorFlex/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/TellorFlex/testing/StakingToken.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/contracts/TellorX/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/TellorX/TellorXMasterMock.sol
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-17 17:02:50.000000 telliot_core-0.2.5/contracts/TellorX/TellorXOracleMock.sol
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/add-chain.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/assets/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)   160315 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/assets/tellor_swoosh.png
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-17 17:02:50.000000 telliot_core-0.2.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-17 17:02:50.000000 telliot_core-0.2.5/interfaces/IERC20.sol
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-17 17:02:50.000000 telliot_core-0.2.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-17 17:02:50.000000 telliot_core-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-17 17:02:50.000000 telliot_core-0.2.5/requirements-dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-17 17:02:50.000000 telliot_core-0.2.5/scripts/morphware_data_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-17 17:02:50.000000 telliot_core-0.2.5/scripts/query_catalog.md
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-17 17:02:50.000000 telliot_core-0.2.5/scripts/query_catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-17 17:02:59.575097 telliot_core-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:02:50.000000 telliot_core-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.555097 telliot_core-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.559097 telliot_core-0.2.5/src/telliot_core/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core/apps/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/apps/telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/asset_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/commands/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/commands/listen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/commands/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core/contract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/contract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/contract/contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/contract/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/data/abi/
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/diva-protocol-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/fuse-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellor-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellor-mesosphere-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-playground.json
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorflex-autopay-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorflex-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-governance-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-lens-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-master-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-oracle-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-treasury-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/abi/trb-token-abi.json
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/assets.json
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/data/contract_directory.json
--rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/gas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/gas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/gas/legacy_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/model/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/api_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/model/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/reporters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/reporters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/tellor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.567098 telliot_core-0.2.5/src/telliot_core/tellor/tellor360/
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellor360/autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellor360/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.571097 telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.571097 telliot_core-0.2.5/src/telliot_core/tellor/tellorx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorx/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/tellor/tellorx/oracle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.571097 telliot_core-0.2.5/src/telliot_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/key_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/pyutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-17 17:02:50.000000 telliot_core-0.2.5/src/telliot_core/utils/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.563097 telliot_core-0.2.5/src/telliot_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-17 17:02:59.000000 telliot_core-0.2.5/src/telliot_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:02:59.575097 telliot_core-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_app_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_asset_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_autopay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_gas.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_master_read.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_model_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_oracle_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_rpc_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_telliot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_tellorflex.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-17 17:02:50.000000 telliot_core-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.381533 telliot_core-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.349531 telliot_core-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/py39.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.github/workflows/typing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-28 18:29:54.000000 telliot_core-0.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-28 18:29:54.000000 telliot_core-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-28 18:30:06.381533 telliot_core-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-28 18:29:54.000000 telliot_core-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-28 18:29:54.000000 telliot_core-0.2.6/brownie-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/Integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/Integrations/DIVAOracleMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/Integrations/DIVAProtocolMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorFlex/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/AutopayMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)    20244 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/TellorFlex.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorFlex/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorFlex/testing/StakingToken.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.361531 telliot_core-0.2.6/contracts/TellorX/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorX/TellorXMasterMock.sol
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-28 18:29:54.000000 telliot_core-0.2.6/contracts/TellorX/TellorXOracleMock.sol
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/add-chain.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/assets/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)   160315 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/assets/tellor_swoosh.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-28 18:29:54.000000 telliot_core-0.2.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-28 18:29:54.000000 telliot_core-0.2.6/interfaces/IERC20.sol
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-28 18:29:54.000000 telliot_core-0.2.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-28 18:29:54.000000 telliot_core-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-28 18:29:54.000000 telliot_core-0.2.6/requirements-dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/morphware_data_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/query_catalog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-28 18:29:54.000000 telliot_core-0.2.6/scripts/query_catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-28 18:30:06.385533 telliot_core-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:29:54.000000 telliot_core-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.353531 telliot_core-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/src/telliot_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/apps/telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/asset_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/listen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/commands/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/contract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/contract/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.369532 telliot_core-0.2.6/src/telliot_core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/data/abi/
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/diva-oracle-tellor-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28088 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/diva-protocol-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/fuse-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor-mesosphere-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35232 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26675 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21821 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-playground.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-autopay-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11824 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-governance-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-lens-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23746 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-master-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11141 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-oracle-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-treasury-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13989 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/abi/trb-token-abi.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/data/contract_directory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/gas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/gas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/gas/legacy_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/api_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/model/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/reporters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/reporters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/tellor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.373532 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellor360/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/tellor/tellorx/oracle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.377532 telliot_core-0.2.6/src/telliot_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/key_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/pyutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-28 18:29:54.000000 telliot_core-0.2.6/src/telliot_core/utils/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.365532 telliot_core-0.2.6/src/telliot_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 18:30:06.000000 telliot_core-0.2.6/src/telliot_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:30:06.381533 telliot_core-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_app_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_asset_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_autopay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_gas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_master_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_oracle_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_rpc_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_telliot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_tellorflex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-28 18:29:54.000000 telliot_core-0.2.6/tox.ini
```

### Comparing `telliot_core-0.2.5/.github/workflows/docs.yml` & `telliot_core-0.2.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.github/workflows/py39.yml` & `telliot_core-0.2.6/.github/workflows/py39.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.github/workflows/release.yml` & `telliot_core-0.2.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.github/workflows/style.yml` & `telliot_core-0.2.6/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.github/workflows/typing.yml` & `telliot_core-0.2.6/.github/workflows/typing.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.gitignore` & `telliot_core-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.pre-commit-config.yaml` & `telliot_core-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/.readthedocs.yaml` & `telliot_core-0.2.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/LICENSE` & `telliot_core-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/PKG-INFO` & `telliot_core-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot_core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.2.5/README.md` & `telliot_core-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/contracts/Integrations/DIVAProtocolMock.sol` & `telliot_core-0.2.6/contracts/Integrations/DIVAProtocolMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/contracts/TellorFlex/TellorFlex.sol` & `telliot_core-0.2.6/contracts/TellorFlex/TellorFlex.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/contracts/TellorX/TellorXMasterMock.sol` & `telliot_core-0.2.6/contracts/TellorX/TellorXMasterMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/contracts/TellorX/TellorXOracleMock.sol` & `telliot_core-0.2.6/contracts/TellorX/TellorXOracleMock.sol`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/docs/add-chain.md` & `telliot_core-0.2.6/docs/add-chain.md`

 * *Files 21% similar despite different names*

```diff
@@ -4,9 +4,10 @@
 2. Add chain ID & name to `telliot_core.apps.core.NETWORKS`.
 3. Add chain info to `telliot_core.model.chain.default_chains_list`.
 4. Add chain ID & gas/fee info retrieval to `telliot_core.gas.legacy_gas.gas_station`.
 5. Add endpoint info to `telliot_core.model.endpoints.default_endpoint_list`.
 6. Add deployed oracle contract and autopay info to `telliot_core.data.contract_directory.json`:
     - Add address for `tellor360-autopay`.
     - Add address for `tellor360-oracle`.
-    - If using testnet, add a tellor playground address for `trb-token`. If using mainnet, add the address of the bridged TRB token contract.
+    - Add address for `trb-token`.
+    - Add address for `tellor-governance`. 
 7. Follow steps to support a new chain in [telliot-feeds](https://tellor-io.github.io/telliot-feeds/add-chain/).
```

### Comparing `telliot_core-0.2.5/docs/assets/favicon-32x32.png` & `telliot_core-0.2.6/docs/assets/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/docs/assets/tellor_swoosh.png` & `telliot_core-0.2.6/docs/assets/tellor_swoosh.png`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/docs/contributing.md` & `telliot_core-0.2.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/docs/documentation.md` & `telliot_core-0.2.6/docs/documentation.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/mkdocs.yml` & `telliot_core-0.2.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/scripts/morphware_data_sizes.py` & `telliot_core-0.2.6/scripts/morphware_data_sizes.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/scripts/query_catalog.md` & `telliot_core-0.2.6/scripts/query_catalog.md`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/scripts/query_catalog.yaml` & `telliot_core-0.2.6/scripts/query_catalog.yaml`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/setup.cfg` & `telliot_core-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/apps/app.py` & `telliot_core-0.2.6/src/telliot_core/apps/app.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/apps/config.py` & `telliot_core-0.2.6/src/telliot_core/apps/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/apps/core.py` & `telliot_core-0.2.6/src/telliot_core/apps/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     941: "pulsechain-testnet",
     42161: "arbitrum",
     1337: "brownie-local-network",
     10200: "chiado-testnet",
     100: "gnosis",
     10: "optimism",
     3141: "filecoin-hyperspace",
+    314159: "filecoin-calibration",
     314: "filecoin",
     11155111: "sepolia",
 }
 
 LOGLEVEL_MAP = {
     "CRITICAL": logging.CRITICAL,
     "ERROR": logging.ERROR,
```

### Comparing `telliot_core-0.2.5/src/telliot_core/apps/session_manager.py` & `telliot_core-0.2.6/src/telliot_core/apps/session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/apps/telliot_config.py` & `telliot_core-0.2.6/src/telliot_core/apps/telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/asset_registry.py` & `telliot_core-0.2.6/src/telliot_core/asset_registry.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/commands/account.py` & `telliot_core-0.2.6/src/telliot_core/cli/commands/account.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/commands/config.py` & `telliot_core-0.2.6/src/telliot_core/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/commands/listen.py` & `telliot_core-0.2.6/src/telliot_core/cli/commands/listen.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/commands/read.py` & `telliot_core-0.2.6/src/telliot_core/cli/commands/read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/main.py` & `telliot_core-0.2.6/src/telliot_core/cli/main.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/cli/utils.py` & `telliot_core-0.2.6/src/telliot_core/cli/utils.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/contract/contract.py` & `telliot_core-0.2.6/src/telliot_core/contract/contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/contract/listener.py` & `telliot_core-0.2.6/src/telliot_core/contract/listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/diva-oracle-tellor-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/diva-oracle-tellor-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/diva-protocol-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/diva-protocol-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/fuse-token-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/fuse-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellor-governance-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellor-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellor-mesosphere-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellor-mesosphere-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-autopay-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-oracle-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellor360-playground.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellor360-playground.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorflex-autopay-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-autopay-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorflex-oracle-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorflex-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-governance-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-governance-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-lens-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-lens-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-master-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-master-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-oracle-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-oracle-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/tellorx-treasury-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/tellorx-treasury-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/abi/trb-token-abi.json` & `telliot_core-0.2.6/src/telliot_core/data/abi/trb-token-abi.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/assets.json` & `telliot_core-0.2.6/src/telliot_core/data/assets.json`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/data/contract_directory.json` & `telliot_core-0.2.6/src/telliot_core/data/contract_directory.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998671679197995%*

 * *Differences: {'18': "{'address': {'314159': '0xb55bB55f7D8b4F26Bd18198088C96488D95cab39'}}",*

 * * '7': "{'address': {'314159': '0xb2CB696fE5244fB9004877e58dcB680cB86Ba444'}}",*

 * * '8': "{'address': {'314159': '0x60cBf3991F05a0671250e673Aa166e9D1A0C662E'}}",*

 * * '9': "{'address': {'314159': '0x15e6Cc0D69A162151Cadfba035aa10b82b12b970'}}"}*

```diff
@@ -98,14 +98,15 @@
             "10": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "100": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "10200": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "11155111": "0x199839a4907ABeC8240D119B606C98c405Bb0B33",
             "137": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "314": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "3141": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
+            "314159": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "4": "0xDb7923FA7D8959A5aDCAA2B652508420f9E47541",
             "420": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "42161": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "421613": "0xb2CB696fE5244fB9004877e58dcB680cB86Ba444",
             "5": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0",
             "80001": "0xD9157453E2668B2fc45b7A803D3FEF3642430cC0"
         },
@@ -120,14 +121,15 @@
             "10": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "100": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "10200": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "11155111": "0x7E7b96d13D75bc7DaF270A491e2f1e571147d4DA",
             "137": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "314": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "3141": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
+            "314159": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "4": "0xb4a418153039eECcaEE2d74D57766BF943aA8d53",
             "420": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "42161": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "421613": "0x60cBf3991F05a0671250e673Aa166e9D1A0C662E",
             "5": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0",
             "80001": "0x9BE9B0CFA89Ea800556C6efbA67b455D336db1D0"
         },
@@ -145,14 +147,15 @@
             "11155111": "0x80fc34a2f9FfE86F41580F47368289C402DEc660",
             "137": "0xE3322702BEdaaEd36CdDAb233360B939775ae5f1",
             "1666600000": "0xd4b28ecb7b765C89F1e67dE3359d09A3520f794E",
             "1666700000": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "3": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
             "314": "0x045CE60839d108B43dF9e703d4b25402a6a28a0d",
             "3141": "0xe7147C5Ed14F545B4B17251992D1DB2bdfa26B6d",
+            "314159": "0x15e6Cc0D69A162151Cadfba035aa10b82b12b970",
             "4": "0x88dF592F8eb5D7Bd38bFeF7dEb0fBc02cf3778a0",
             "420": "0xd71F72C18767083e4e3FE84F9c62b8038C1Ef4f6",
             "42161": "0xd58D345Fd9c82262E087d2D0607624B410D88242",
             "421611": "0x126f5C4802c10848Eb66ce2F74380B7ADeFF36Cb",
             "421613": "0x8d1bB5eDdFce08B92dD47c9871d1805211C3Eb3C",
             "5": "0x51c59c6cAd28ce3693977F2feB4CfAebec30d8a2",
             "69": "0x7B8AC044ebce66aCdF14197E8De38C1Cc802dB4A",
@@ -249,14 +252,15 @@
             "10": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "100": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "10200": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "11155111": "0x8C9057FA16D3Debb703ADBac0A097d2E5577AA6b",
             "137": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "314": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "3141": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
+            "314159": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "420": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "42161": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "421613": "0xb55bB55f7D8b4F26Bd18198088C96488D95cab39",
             "5": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45",
             "80001": "0x46038969D7DC0b17BC72137D07b4eDe43859DA45"
         },
         "name": "tellor-governance",
```

### Comparing `telliot_core-0.2.5/src/telliot_core/directory.py` & `telliot_core-0.2.6/src/telliot_core/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,17 @@
                 elif chain_id == 10200:
                     url = "https://blockscout.chiadochain.net/"
                 elif chain_id == 100:
                     url = "https://api.gnosisscan.io"
                 elif chain_id == 10:
                     url = "https://optimistic.etherscan.io/"
                 elif chain_id == 3141:
-                    url = "https://hyperspace.filfox.info/"
+                    url = "https://hyperspace.filfox.info/en"
+                elif chain_id == 314159:
+                    url = "https://calibration.filfox.info/en"
                 elif chain_id == 314:
                     url = "https://filfox.info/en"
                 elif chain_id == 11155111:
                     url = "https://api-sepolia.etherscan.io"
                 else:
                     raise ValueError(f"Could not retrieve ABI using chain_id {chain_id}")
```

### Comparing `telliot_core-0.2.5/src/telliot_core/gas/legacy_gas.py` & `telliot_core-0.2.6/src/telliot_core/gas/legacy_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/logs.py` & `telliot_core-0.2.6/src/telliot_core/logs.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/model/api_keys.py` & `telliot_core-0.2.6/src/telliot_core/model/api_keys.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/model/chain.py` & `telliot_core-0.2.6/src/telliot_core/model/chain.py`

 * *Files 7% similar despite different names*

```diff
@@ -137,15 +137,22 @@
         currency=EVMCurrency(name="Optimism Ether", symbol="ETH", decimals=18),
     ),
     Chain(
         chain_id=3141,
         name="filecoin-hyperspace",
         chain="filecoin-hyperspace",
         network="testnet",
-        currency=EVMCurrency(name="Testnet Filecoin", symbol="TFIL", decimals=18),
+        currency=EVMCurrency(name="Testnet Filecoin", symbol="FIL", decimals=18),
+    ),
+    Chain(
+        chain_id=314159,
+        name="filecoin-calibration",
+        chain="filecoin-calibration",
+        network="testnet",
+        currency=EVMCurrency(name="Testnet Filecoin", symbol="FIL", decimals=18),
     ),
     Chain(
         chain_id=314,
         name="filecoin",
         chain="filecoin",
         network="mainnet",
         currency=EVMCurrency(name="Filecoin", symbol="FIL", decimals=18),
```

### Comparing `telliot_core-0.2.5/src/telliot_core/model/endpoints.py` & `telliot_core-0.2.6/src/telliot_core/model/endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,22 @@
         explorer="https://goerli-optimism.etherscan.io/",
     ),
     RPCEndpoint(
         chain_id=3141,
         provider="Filecoin",
         network="filecoin-hyperspace",
         url="https://api.hyperspace.node.glif.io/rpc/v1",
-        explorer="https://hyperspace.filfox.info/",
+        explorer="https://hyperspace.filfox.info/en",
+    ),
+    RPCEndpoint(
+        chain_id=314159,
+        provider="Filecoin",
+        network="filecoin-calibration",
+        url="https://api.calibration.node.glif.io/rpc/v1",
+        explorer="https://calibration.filfox.info/en",
     ),
     RPCEndpoint(
         chain_id=314,
         provider="Filecoin",
         network="filecoin",
         url="https://api.node.glif.io/rpc/v1",
         explorer="https://filfox.info/en",
```

### Comparing `telliot_core-0.2.5/src/telliot_core/model/tokens.py` & `telliot_core-0.2.6/src/telliot_core/model/tokens.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellor360/autopay.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellor360/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellor360/oracle.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellor360/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/autopay.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/oracle.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellorflex/token.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellorflex/token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellorx/master.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellorx/master.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/tellor/tellorx/oracle.py` & `telliot_core-0.2.6/src/telliot_core/tellor/tellorx/oracle.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/utils/home.py` & `telliot_core-0.2.6/src/telliot_core/utils/home.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/utils/key_helpers.py` & `telliot_core-0.2.6/src/telliot_core/utils/key_helpers.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/utils/response.py` & `telliot_core-0.2.6/src/telliot_core/utils/response.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/utils/timestamp.py` & `telliot_core-0.2.6/src/telliot_core/utils/timestamp.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core/utils/versions.py` & `telliot_core-0.2.6/src/telliot_core/utils/versions.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/src/telliot_core.egg-info/PKG-INFO` & `telliot_core-0.2.6/src/telliot_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telliot-core
-Version: 0.2.5
+Version: 0.2.6
 Summary: Telliot is a Python framework for interacting with the decentralized TellorX network.
 Home-page: https://github.com/tellor-io/telliot-core
 Author: Tellor Development Community
 Author-email: info@tellor.io
 License: MIT
 Keywords: oracle,etherium,blockchain
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `telliot_core-0.2.5/src/telliot_core.egg-info/SOURCES.txt` & `telliot_core-0.2.6/src/telliot_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/conftest.py` & `telliot_core-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_app_core.py` & `telliot_core-0.2.6/tests/test_app_core.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_autopay.py` & `telliot_core-0.2.6/tests/test_autopay.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_cli.py` & `telliot_core-0.2.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_config.py` & `telliot_core-0.2.6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_contract.py` & `telliot_core-0.2.6/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_directory.py` & `telliot_core-0.2.6/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_gas.py` & `telliot_core-0.2.6/tests/test_gas.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_listener.py` & `telliot_core-0.2.6/tests/test_listener.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_master_read.py` & `telliot_core-0.2.6/tests/test_master_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_model_chain.py` & `telliot_core-0.2.6/tests/test_model_chain.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_oracle_read.py` & `telliot_core-0.2.6/tests/test_oracle_read.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_rpc_endpoint.py` & `telliot_core-0.2.6/tests/test_rpc_endpoint.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_session_manager.py` & `telliot_core-0.2.6/tests/test_session_manager.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_telliot_config.py` & `telliot_core-0.2.6/tests/test_telliot_config.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_tellorflex.py` & `telliot_core-0.2.6/tests/test_tellorflex.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tests/test_token.py` & `telliot_core-0.2.6/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `telliot_core-0.2.5/tox.ini` & `telliot_core-0.2.6/tox.ini`

 * *Files identical despite different names*

