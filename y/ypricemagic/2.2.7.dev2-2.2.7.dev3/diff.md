# Comparing `tmp/ypricemagic-2.2.7.dev2.tar.gz` & `tmp/ypricemagic-2.2.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.2.7.dev2.tar", last modified: Fri Apr 28 06:38:20 2023, max compression
+gzip compressed data, was "ypricemagic-2.2.7.dev3.tar", last modified: Fri Apr 28 07:32:02 2023, max compression
```

## Comparing `ypricemagic-2.2.7.dev2.tar` & `ypricemagic-2.2.7.dev3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.454563 ypricemagic-2.2.7.dev2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.454563 ypricemagic-2.2.7.dev2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.458563 ypricemagic-2.2.7.dev2/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.462563 ypricemagic-2.2.7.dev2/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    21799 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     5110 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-28 06:38:06.000000 ypricemagic-2.2.7.dev2/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 06:38:20.466562 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-28 06:38:20.000000 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-28 06:38:20.000000 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 06:38:20.000000 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 06:38:20.000000 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 06:38:20.000000 ypricemagic-2.2.7.dev2/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.463161 ypricemagic-2.2.7.dev3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.467161 ypricemagic-2.2.7.dev3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2891 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.467161 ypricemagic-2.2.7.dev3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.467161 ypricemagic-2.2.7.dev3/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      143 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.467161 ypricemagic-2.2.7.dev3/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9873 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20058 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.471161 ypricemagic-2.2.7.dev3/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19844 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.475161 ypricemagic-2.2.7.dev3/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.479161 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23291 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.479161 ypricemagic-2.2.7.dev3/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.479161 ypricemagic-2.2.7.dev3/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11292 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.479161 ypricemagic-2.2.7.dev3/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21799 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3245 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3852 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.479161 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5106 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4343 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2560 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-04-28 07:31:40.000000 ypricemagic-2.2.7.dev3/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 07:32:02.483161 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-28 07:32:02.000000 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-04-28 07:32:02.000000 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 07:32:02.000000 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-28 07:32:02.000000 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-28 07:32:02.000000 ypricemagic-2.2.7.dev3/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.2.7.dev2/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.2.7.dev3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/.github/workflows/pytest.yaml` & `ypricemagic-2.2.7.dev3/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/.github/workflows/release.yaml` & `ypricemagic-2.2.7.dev3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/LICENSE.txt` & `ypricemagic-2.2.7.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/README.md` & `ypricemagic-2.2.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/setup.py` & `ypricemagic-2.2.7.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/classes/test_erc20.py` & `ypricemagic-2.2.7.dev3/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/classes/test_singleton.py` & `ypricemagic-2.2.7.dev3/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/fixtures.py` & `ypricemagic-2.2.7.dev3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.2.7.dev3/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/lending/test_aave.py` & `ypricemagic-2.2.7.dev3/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/lending/test_compound.py` & `ypricemagic-2.2.7.dev3/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/test_chainlink.py` & `ypricemagic-2.2.7.dev3/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/test_magic.py` & `ypricemagic-2.2.7.dev3/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/test_popsicle.py` & `ypricemagic-2.2.7.dev3/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/test_synthetix.py` & `ypricemagic-2.2.7.dev3/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/test_yearn.py` & `ypricemagic-2.2.7.dev3/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/tests/prices/utils/test_buckets.py` & `ypricemagic-2.2.7.dev3/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/__init__.py` & `ypricemagic-2.2.7.dev3/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/classes/common.py` & `ypricemagic-2.2.7.dev3/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/classes/singleton.py` & `ypricemagic-2.2.7.dev3/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/constants.py` & `ypricemagic-2.2.7.dev3/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/contracts.py` & `ypricemagic-2.2.7.dev3/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/datatypes.py` & `ypricemagic-2.2.7.dev3/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/decorators.py` & `ypricemagic-2.2.7.dev3/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/erc20.py` & `ypricemagic-2.2.7.dev3/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/exceptions.py` & `ypricemagic-2.2.7.dev3/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/ERC20.py` & `ypricemagic-2.2.7.dev3/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.2.7.dev3/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/compound/unitroller.py` & `ypricemagic-2.2.7.dev3/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.2.7.dev3/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/multicall2.py` & `ypricemagic-2.2.7.dev3/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.2.7.dev3/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.2.7.dev3/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/networks.py` & `ypricemagic-2.2.7.dev3/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/band.py` & `ypricemagic-2.2.7.dev3/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/chainlink.py` & `ypricemagic-2.2.7.dev3/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/convex.py` & `ypricemagic-2.2.7.dev3/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/balancer/v1.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/balancer/v2.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/genericamm.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/mooniswap.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.2.7.dev3/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/eth_derivs/creth.py` & `ypricemagic-2.2.7.dev3/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.2.7.dev3/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/gearbox.py` & `ypricemagic-2.2.7.dev3/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/lending/aave.py` & `ypricemagic-2.2.7.dev3/y/prices/lending/aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/lending/compound.py` & `ypricemagic-2.2.7.dev3/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/lending/ib.py` & `ypricemagic-2.2.7.dev3/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/magic.py` & `ypricemagic-2.2.7.dev3/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/one_to_one.py` & `ypricemagic-2.2.7.dev3/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/popsicle.py` & `ypricemagic-2.2.7.dev3/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/belt.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/curve.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/froyo.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/stable_swap/saddle.py` & `ypricemagic-2.2.7.dev3/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/synthetix.py` & `ypricemagic-2.2.7.dev3/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.2.7.dev3/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/utils/buckets.py` & `ypricemagic-2.2.7.dev3/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/utils/sense_check.py` & `ypricemagic-2.2.7.dev3/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/prices/utils/ypriceapi.py` & `ypricemagic-2.2.7.dev3/y/prices/utils/ypriceapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,19 +68,19 @@
         # NOTE: The reason we are here has already been logged.
         return None
 
     async with YPRICEAPI_SEMAPHORE:
         try:
             session = await get_session()
             response = await session.get(f'/get_price/{chain.id}/{token}?block={block}')
-            return await read_response(token, block, response)
         except asyncio.TimeoutError:
             logger.warning(f'ypriceAPI timed out for {token} at {block}.{FALLBACK_STR}')
         except ClientError as e:
             logger.warning(f'ypriceAPI {e.__class__.__name__} for {token} at {block}.{FALLBACK_STR}')
+        return await read_response(token, block, response)
 
 
 async def read_response(token: Address, block: Optional[Block], response: ClientResponse) -> Optional[UsdPrice]:
     # 200
     if response.status == HTTPStatus.OK:
         return await response.json()
```

### Comparing `ypricemagic-2.2.7.dev2/y/prices/yearn.py` & `ypricemagic-2.2.7.dev3/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/time.py` & `ypricemagic-2.2.7.dev3/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/client.py` & `ypricemagic-2.2.7.dev3/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/events.py` & `ypricemagic-2.2.7.dev3/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/fakes.py` & `ypricemagic-2.2.7.dev3/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/logging.py` & `ypricemagic-2.2.7.dev3/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/middleware.py` & `ypricemagic-2.2.7.dev3/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/multicall.py` & `ypricemagic-2.2.7.dev3/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/y/utils/raw_calls.py` & `ypricemagic-2.2.7.dev3/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/ypricemagic/magic.py` & `ypricemagic-2.2.7.dev3/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.2.7.dev2/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.2.7.dev3/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

