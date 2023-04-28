# Comparing `tmp/ypricemagic-2.2.5.tar.gz` & `tmp/ypricemagic-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.2.5.tar", last modified: Fri Apr 28 00:31:47 2023, max compression
+gzip compressed data, was "ypricemagic-2.2.6.tar", last modified: Fri Apr 28 04:38:50 2023, max compression
```

## Comparing `ypricemagic-2.2.5.tar` & `ypricemagic-2.2.6.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.283307 ypricemagic-2.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.287307 ypricemagic-2.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.287307 ypricemagic-2.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.287307 ypricemagic-2.2.5/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.291308 ypricemagic-2.2.5/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.295307 ypricemagic-2.2.5/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.299308 ypricemagic-2.2.5/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.299308 ypricemagic-2.2.5/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.299308 ypricemagic-2.2.5/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.299308 ypricemagic-2.2.5/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.303308 ypricemagic-2.2.5/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.303308 ypricemagic-2.2.5/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    21799 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.303308 ypricemagic-2.2.5/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.303308 ypricemagic-2.2.5/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     4813 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-28 00:31:30.000000 ypricemagic-2.2.5/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 00:31:47.307308 ypricemagic-2.2.5/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-28 00:31:47.000000 ypricemagic-2.2.5/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-28 00:31:47.000000 ypricemagic-2.2.5/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 00:31:47.000000 ypricemagic-2.2.5/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 00:31:47.000000 ypricemagic-2.2.5/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 00:31:47.000000 ypricemagic-2.2.5/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.841067 ypricemagic-2.2.6/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.817067 ypricemagic-2.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.821067 ypricemagic-2.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-28 04:38:50.841067 ypricemagic-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-28 04:38:50.841067 ypricemagic-2.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.821067 ypricemagic-2.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.825067 ypricemagic-2.2.6/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.829067 ypricemagic-2.2.6/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.833067 ypricemagic-2.2.6/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.837067 ypricemagic-2.2.6/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21799 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.837067 ypricemagic-2.2.6/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.837067 ypricemagic-2.2.6/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5463 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.837067 ypricemagic-2.2.6/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.837067 ypricemagic-2.2.6/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-28 04:38:29.000000 ypricemagic-2.2.6/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 04:38:50.841067 ypricemagic-2.2.6/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-04-28 04:38:50.000000 ypricemagic-2.2.6/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-28 04:38:50.000000 ypricemagic-2.2.6/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 04:38:50.000000 ypricemagic-2.2.6/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 04:38:50.000000 ypricemagic-2.2.6/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 04:38:50.000000 ypricemagic-2.2.6/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.2.5/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.2.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/.github/workflows/pytest.yaml` & `ypricemagic-2.2.6/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/.github/workflows/release.yaml` & `ypricemagic-2.2.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/LICENSE.txt` & `ypricemagic-2.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/README.md` & `ypricemagic-2.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/setup.py` & `ypricemagic-2.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/classes/test_erc20.py` & `ypricemagic-2.2.6/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/classes/test_singleton.py` & `ypricemagic-2.2.6/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/fixtures.py` & `ypricemagic-2.2.6/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.2.6/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/lending/test_aave.py` & `ypricemagic-2.2.6/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/lending/test_compound.py` & `ypricemagic-2.2.6/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/test_chainlink.py` & `ypricemagic-2.2.6/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/test_magic.py` & `ypricemagic-2.2.6/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/test_popsicle.py` & `ypricemagic-2.2.6/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/test_synthetix.py` & `ypricemagic-2.2.6/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/test_yearn.py` & `ypricemagic-2.2.6/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/tests/prices/utils/test_buckets.py` & `ypricemagic-2.2.6/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/__init__.py` & `ypricemagic-2.2.6/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/classes/common.py` & `ypricemagic-2.2.6/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/classes/singleton.py` & `ypricemagic-2.2.6/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/constants.py` & `ypricemagic-2.2.6/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/contracts.py` & `ypricemagic-2.2.6/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/datatypes.py` & `ypricemagic-2.2.6/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/decorators.py` & `ypricemagic-2.2.6/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/erc20.py` & `ypricemagic-2.2.6/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/exceptions.py` & `ypricemagic-2.2.6/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/ERC20.py` & `ypricemagic-2.2.6/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.2.6/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/compound/unitroller.py` & `ypricemagic-2.2.6/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.2.6/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/multicall2.py` & `ypricemagic-2.2.6/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.2.6/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.2.6/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/networks.py` & `ypricemagic-2.2.6/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/band.py` & `ypricemagic-2.2.6/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/chainlink.py` & `ypricemagic-2.2.6/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/convex.py` & `ypricemagic-2.2.6/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.2.6/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/balancer/v1.py` & `ypricemagic-2.2.6/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/balancer/v2.py` & `ypricemagic-2.2.6/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/genericamm.py` & `ypricemagic-2.2.6/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/mooniswap.py` & `ypricemagic-2.2.6/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.2.6/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.2.6/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.2.6/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.2.6/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.2.6/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/eth_derivs/creth.py` & `ypricemagic-2.2.6/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.2.6/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/gearbox.py` & `ypricemagic-2.2.6/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/lending/aave.py` & `ypricemagic-2.2.6/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/lending/compound.py` & `ypricemagic-2.2.6/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/lending/ib.py` & `ypricemagic-2.2.6/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/magic.py` & `ypricemagic-2.2.6/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/one_to_one.py` & `ypricemagic-2.2.6/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/popsicle.py` & `ypricemagic-2.2.6/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/belt.py` & `ypricemagic-2.2.6/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/curve.py` & `ypricemagic-2.2.6/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.2.6/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/froyo.py` & `ypricemagic-2.2.6/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.2.6/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/stable_swap/saddle.py` & `ypricemagic-2.2.6/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/synthetix.py` & `ypricemagic-2.2.6/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.2.6/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.2.6/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.2.6/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.2.6/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/utils/buckets.py` & `ypricemagic-2.2.6/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/utils/sense_check.py` & `ypricemagic-2.2.6/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/prices/utils/ypriceapi.py` & `ypricemagic-2.2.6/y/prices/utils/ypriceapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,19 @@
 auth_headers = {"X-Signer": YPRICEAPI_SIGNER, "X-Signature": YPRICEAPI_SIGNATURE} if YPRICEAPI_SIGNER and YPRICEAPI_SIGNATURE else {}
 
 # old
 YPRICEAPI_USER = os.environ.get("YPRICEAPI_USER")
 YPRICEAPI_PASS = os.environ.get("YPRICEAPI_PASS")
 old_auth = BasicAuth(YPRICEAPI_USER, YPRICEAPI_PASS) if YPRICEAPI_USER and YPRICEAPI_PASS else None
 
+ONE_MINUTE = 60  # some arbitrary amount of time in case the header is missing on unexpected 5xx responses
 YPRICEAPI_SEMAPHORE = asyncio.Semaphore(int(os.environ.get("YPRICEAPI_SEMAPHORE", 100)))
 
+read_retry_header = lambda x: x.headers.get("Retry-After", ONE_MINUTE)
+
 notified = set()
 
 resume_at = 0
 
 FALLBACK_STR = "Falling back to your node for pricing."
 
 # NOTE: if you want to bypass ypriceapi for specific tokens, have your program add the addresses to this set.
@@ -90,32 +93,46 @@
             logger.error(f'Your provided ypriceAPI credentials are not authorized for use.{FALLBACK_STR}')
             notified.add(HTTPStatus.UNAUTHORIZED)
                 
     # 404
     elif response.status == HTTPStatus.NOT_FOUND:
         logger.debug(f"Failed to get price from API: {token} at {block}")
 
+
+    # Server Errors
+    
+    # 502
+    elif response.status == HTTPStatus.BAD_GATEWAY:
+        logger.warning(f"ypriceAPI returned status code {_get_err_reason(response)}:")
+        try:
+            logger.warning(await response.json(content_type=None) or await response.text())
+        except Exception:
+            logger.warning(f'exception decoding ypriceapi 502 response.{FALLBACK_STR}', exc_info=True)
+        _set_resume_at(read_retry_header(response))
+    
     # 503
     elif response.status == HTTPStatus.SERVICE_UNAVAILABLE:
         logger.warning(f"ypriceAPI returned status code {_get_err_reason(response)}:")
         try:
-            logger.warning(await response.json(content_type=None))
-        except Exception as e:
+            logger.warning(await response.json(content_type=None) or await response.text())
+        except Exception:
             logger.warning(f'exception decoding ypriceapi 503 response.{FALLBACK_STR}', exc_info=True)
-        five_minutes = 60 * 5  # some arbitrary amount of time in case the header is missing on unexpected 503s
-        retry_after = response.headers.get("Retry-After", five_minutes)
-        logger.info(f"Falling back to your node for {retry_after/60} minutes.")
-        global resume_at
-        resume_at = time() + retry_after
-                    
+        _set_resume_at(read_retry_header(response))
+
     else:
         logger.warning(f'ypriceAPI returned status code {_get_err_reason(response)} for {token} at {block}.{FALLBACK_STR}')
             
 
 def _get_err_reason(response: ClientResponse) -> str:
     if response.reason is None:
         return f"[{response.status}]"
     ascii_encodable_reason = response.reason.encode(
         "ascii", "backslashreplace"
     ).decode("ascii")
     return f"[{response.status} {ascii_encodable_reason}]"
     
+def _set_resume_at(retry_after: float) -> None:
+    global resume_at
+    logger.info(f"Falling back to your node for {retry_after/60} minutes.")
+    resume_from_this_err_at = time() + retry_after
+    if resume_from_this_err_at > resume_at:
+        resume_at = resume_from_this_err_at
```

### Comparing `ypricemagic-2.2.5/y/prices/yearn.py` & `ypricemagic-2.2.6/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/time.py` & `ypricemagic-2.2.6/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/client.py` & `ypricemagic-2.2.6/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/events.py` & `ypricemagic-2.2.6/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/fakes.py` & `ypricemagic-2.2.6/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/logging.py` & `ypricemagic-2.2.6/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/middleware.py` & `ypricemagic-2.2.6/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/multicall.py` & `ypricemagic-2.2.6/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/y/utils/raw_calls.py` & `ypricemagic-2.2.6/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/ypricemagic/magic.py` & `ypricemagic-2.2.6/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.5/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.2.6/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

