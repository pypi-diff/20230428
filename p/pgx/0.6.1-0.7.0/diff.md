# Comparing `tmp/pgx-0.6.1.tar.gz` & `tmp/pgx-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-0.6.1.tar", last modified: Thu Apr 27 20:29:08 2023, max compression
+gzip compressed data, was "pgx-0.7.0.tar", last modified: Fri Apr 28 04:29:48 2023, max compression
```

## Comparing `pgx-0.6.1.tar` & `pgx-0.7.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.717471 pgx-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-27 20:28:55.000000 pgx-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-27 20:29:08.717471 pgx-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-04-27 20:28:55.000000 pgx-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.693471 pgx-0.6.1/pgx/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.693471 pgx-0.6.1/pgx/_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/_hand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/_meld.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/_shanten.py
--rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_mahjong/_yaku.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.697471 pgx-0.6.1/pgx/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/chess_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.701471 pgx-0.6.1/pgx/_src/dwg/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/animalshogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.701471 pgx-0.6.1/pgx/_src/dwg/images/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.705471 pgx-0.6.1/pgx/_src/dwg/images/chess/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/bRook.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wBishop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wKing.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wKnight.svg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wPawn.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wQueen.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/chess/wRook.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.709471 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/
--rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/dwg/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/shogi_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/_src/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    18349 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)    37400 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29176 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4479 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/connect_four.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.709471 pgx-0.6.1/pgx/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/pettingzoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/experimental/visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/leduc_holdem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.713471 pgx-0.6.1/pgx/minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12789 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     8952 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    26107 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10015 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/minatar/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)    20450 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/tic_tac_toe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15923 2023-04-27 20:28:55.000000 pgx-0.6.1/pgx/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.693471 pgx-0.6.1/pgx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-04-27 20:29:08.000000 pgx-0.6.1/pgx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-27 20:29:08.000000 pgx-0.6.1/pgx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:29:08.000000 pgx-0.6.1/pgx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-27 20:29:08.000000 pgx-0.6.1/pgx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-27 20:29:08.000000 pgx-0.6.1/pgx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-27 20:28:55.000000 pgx-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:29:08.717471 pgx-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-27 20:28:55.000000 pgx-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:29:08.717471 pgx-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/minatar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_animal_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_backgammon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)    61899 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_bridge_bidding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29758 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_chess.py
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_connect_four.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    39651 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_kuhn_poker.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_leduc_holdem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_othello.py
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_play2048.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_shogi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    22439 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_sparrow_mahjong.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-27 20:28:55.000000 pgx-0.6.1/tests/test_tic_tac_toe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.838286 pgx-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-28 04:29:38.000000 pgx-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-04-28 04:29:48.838286 pgx-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-04-28 04:29:38.000000 pgx-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.814286 pgx-0.7.0/pgx/
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.818286 pgx-0.7.0/pgx/_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/_hand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/_meld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/_shanten.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15713 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_mahjong/_yaku.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.818286 pgx-0.7.0/pgx/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5836 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/chess_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.822286 pgx-0.7.0/pgx/_src/dwg/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/animalshogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.822286 pgx-0.7.0/pgx/_src/dwg/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.826286 pgx-0.7.0/pgx/_src/dwg/images/chess/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/bRook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wBishop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wKing.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wKnight.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wPawn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wQueen.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/chess/wRook.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.830286 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/
+-rw-r--r--   0 runner    (1001) docker     (123)    45499 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45511 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10449 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15112 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15124 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    13139 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15152 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16652 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/dwg/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/shogi_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8746 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/_src/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37353 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29164 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/connect_four.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.830286 pgx-0.7.0/pgx/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/pettingzoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/experimental/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18487 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/leduc_holdem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.834286 pgx-0.7.0/pgx/minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12771 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26089 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/minatar/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20426 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21398 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/tic_tac_toe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14260 2023-04-28 04:29:38.000000 pgx-0.7.0/pgx/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.818286 pgx-0.7.0/pgx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-04-28 04:29:48.000000 pgx-0.7.0/pgx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-28 04:29:48.000000 pgx-0.7.0/pgx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 04:29:48.000000 pgx-0.7.0/pgx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 04:29:48.000000 pgx-0.7.0/pgx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 04:29:48.000000 pgx-0.7.0/pgx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-28 04:29:38.000000 pgx-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 04:29:48.838286 pgx-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-28 04:29:38.000000 pgx-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:48.838286 pgx-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/minatar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_animal_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17465 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_backgammon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61927 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_bridge_bidding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29776 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_chess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_connect_four.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39655 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_kuhn_poker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_leduc_holdem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_othello.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_play2048.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_shogi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22440 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_sparrow_mahjong.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-28 04:29:38.000000 pgx-0.7.0/tests/test_tic_tac_toe.py
```

### Comparing `pgx-0.6.1/LICENSE` & `pgx-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/PKG-INFO` & `pgx-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.6.1
+Version: 0.7.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,15 +58,15 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not state.terminated.all():
+while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
 > ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
 
 <!---
@@ -90,15 +90,15 @@
 ## Supported games
 
 | Backgammon | Chess | Shogi | Go |
 |:---:|:---:|:---:|:---:|
 |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only" width="158px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-light-mode-only" width="158px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-dark-mode-only" width="160px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only" width="160px">|
 
 
-Use `pgx.available_games() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
+Use `pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
 
 ```py
 >>> env = pgx.make(<EnvId>)
 ```
 
 You can check the current version of each environment by
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.6.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.7.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -27,36 +27,37 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not state.terminated.all(): action = model
-(state.current_player, state.observation, state.legal_action_mask) state = step
-(state, action) # state.reward (2,) ``` > â ï¸ Pgx is currently in the beta
-version. Therefore, API is subject to change without notice. We aim to release
-v1.0.0 in April 2023. Opinions and comments are more than welcome!  ##
-Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |
-[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+# vectorized states while not (state.terminated | state.terminated).all():
+action = model(state.current_player, state.observation,
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
+â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
+change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+comments are more than welcome!  ## Supported games | Backgammon | Chess |
+Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_games() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
 friendly shogi.* | |Backgammon
```

### Comparing `pgx-0.6.1/README.md` & `pgx-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not state.terminated.all():
+while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
 > ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
 
 <!---
@@ -77,15 +77,15 @@
 ## Supported games
 
 | Backgammon | Chess | Shogi | Go |
 |:---:|:---:|:---:|:---:|
 |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only" width="158px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-light-mode-only" width="158px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-dark-mode-only" width="160px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only" width="160px">|
 
 
-Use `pgx.available_games() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
+Use `pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
 
 ```py
 >>> env = pgx.make(<EnvId>)
 ```
 
 You can check the current version of each environment by
```

#### html2text {}

```diff
@@ -21,36 +21,37 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not state.terminated.all(): action = model
-(state.current_player, state.observation, state.legal_action_mask) state = step
-(state, action) # state.reward (2,) ``` > â ï¸ Pgx is currently in the beta
-version. Therefore, API is subject to change without notice. We aim to release
-v1.0.0 in April 2023. Opinions and comments are more than welcome!  ##
-Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |
-[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+# vectorized states while not (state.terminated | state.terminated).all():
+action = model(state.current_player, state.observation,
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
+â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
+change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+comments are more than welcome!  ## Supported games | Backgammon | Chess |
+Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_games() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
 friendly shogi.* | |Backgammon
```

### Comparing `pgx-0.6.1/pgx/_mahjong/_hand.py` & `pgx-0.7.0/pgx/_mahjong/_hand.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_mahjong/_meld.py` & `pgx-0.7.0/pgx/_mahjong/_meld.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_mahjong/_shanten.py` & `pgx-0.7.0/pgx/_mahjong/_shanten.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_mahjong/_yaku.py` & `pgx-0.7.0/pgx/_mahjong/_yaku.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/api_test.py` & `pgx-0.7.0/pgx/_src/api_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,50 +116,51 @@
 
 def _validate_taking_action_after_terminal(state: State, step_fn):
     prev_state = state
     if not state.terminated:
         return
     action = 0
     state = step_fn(state, action)
-    assert (state.reward == 0).all()
+    assert (state.rewards == 0).all()
     for field in fields(state):
-        if field.name in ["reward", "steps"]:
+        if field.name in ["rewards", "steps"]:
             continue
         assert (
             getattr(state, field.name) == getattr(prev_state, field.name)
         ).all(), f"{field.name} : \n{getattr(state, field.name)}\n{getattr(prev_state, field.name)}"
 
 
 def _validate_init_reward(state: State):
-    assert (state.reward == jnp.zeros_like(state.reward)).all()
+    assert (state.rewards == jnp.zeros_like(state.rewards)).all()
 
 
 def _validate_state(state: State):
     """validate_state checks these items:
 
     - current_player is int8
     - terminated is bool_
     - reward is float
     - legal_action_mask is bool_
     - TODO: observation is bool_ or int8 (can promote to any other types)
     """
     assert state.env_id in get_args(EnvId)
     assert state.current_player.dtype == jnp.int8, state.current_player.dtype
     assert state.terminated.dtype == jnp.bool_, state.terminated.dtype
-    assert state.reward.dtype == jnp.float32, state.reward.dtype
+    assert state.rewards.dtype == jnp.float32, state.rewards.dtype
     assert (
         state.legal_action_mask.dtype == jnp.bool_
     ), state.legal_action_mask.dtype
 
     # check public attributes
     public_attributes = [
         "current_player",
         "observation",
-        "reward",
+        "rewards",
         "terminated",
+        "truncated",
         "legal_action_mask",
     ]
     for k, v in state.__dict__.items():
         if k.startswith("_"):  # internal
             continue
         assert k in public_attributes
```

### Comparing `pgx-0.6.1/pgx/_src/chess_utils.py` & `pgx-0.7.0/pgx/_src/chess_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/animalshogi.py` & `pgx-0.7.0/pgx/_src/dwg/animalshogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/backgammon.py` & `pgx-0.7.0/pgx/_src/dwg/backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/bridge_bidding.py` & `pgx-0.7.0/pgx/_src/dwg/bridge_bidding.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/chess.py` & `pgx-0.7.0/pgx/_src/dwg/chess.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/connect_four.py` & `pgx-0.7.0/pgx/_src/dwg/connect_four.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/go.py` & `pgx-0.7.0/pgx/_src/dwg/go.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/hex.py` & `pgx-0.7.0/pgx/_src/dwg/hex.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/LICENSE` & `pgx-0.7.0/pgx/_src/dwg/images/chess/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bBishop.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bKing.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bKnight.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bPawn.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bQueen.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/bRook.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/bRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wBishop.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wBishop.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wKing.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wKing.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wKnight.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wKnight.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wPawn.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wPawn.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wQueen.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wQueen.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/chess/wRook.svg` & `pgx-0.7.0/pgx/_src/dwg/images/chess/wRook.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/1p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/1p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/1pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/2p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/2p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/2pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/3p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/3p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/3pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/4p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/4p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/4pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/5p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/5p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/5pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/6p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/6p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/6pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/7p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/7p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/7pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/8p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/8p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/8pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/9p.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/9p.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/9pr.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/b.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/b.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/gd.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/gd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/oya.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/oya.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/images/sparrow_mahjong/rd.svg` & `pgx-0.7.0/pgx/_src/dwg/images/sparrow_mahjong/rd.svg`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/kuhn_poker.py` & `pgx-0.7.0/pgx/_src/dwg/kuhn_poker.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/leduc_holdem.py` & `pgx-0.7.0/pgx/_src/dwg/leduc_holdem.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/othello.py` & `pgx-0.7.0/pgx/_src/dwg/othello.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/play2048.py` & `pgx-0.7.0/pgx/_src/dwg/play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/shogi.py` & `pgx-0.7.0/pgx/_src/dwg/shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/sparrow_mahjong.py` & `pgx-0.7.0/pgx/_src/dwg/sparrow_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/dwg/tictactoe.py` & `pgx-0.7.0/pgx/_src/dwg/tictactoe.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/shogi_utils.py` & `pgx-0.7.0/pgx/_src/shogi_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/struct.py` & `pgx-0.7.0/pgx/_src/struct.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/_src/visualizer.py` & `pgx-0.7.0/pgx/_src/visualizer.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/animal_shogi.py` & `pgx-0.7.0/pgx/animal_shogi.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,17 @@
 #  9: OPP_GOLD
 INIT_BOARD = jnp.int8([6, -1, -1, 2, 8, 5, 0, 3, 7, -1, -1, 1])  # (12,)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(132, dtype=jnp.bool_)  # (132,)
     observation: jnp.ndarray = jnp.zeros((4, 3, 22), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Animal Shogi specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     _board: jnp.ndarray = INIT_BOARD  # (12,)
@@ -75,16 +76,16 @@
             is_drop,
             lambda: Action(is_drop=TRUE, to=sq, drop_piece=x - 8),  # type: ignore
             lambda: Action(is_drop=FALSE, from_=sq, to=_to(sq, x)),  # type: ignore
         )
 
 
 class AnimalShogi(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
         self.max_termination_steps: int = 200
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         state = State(current_player=current_player)  # type: ignore
         state = state.replace(legal_action_mask=_legal_action_mask(state))  # type: ignore
@@ -135,15 +136,15 @@
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
         jnp.zeros(2, dtype=jnp.float32),
     )
     # fmt: on
     return state.replace(  # type: ignore
         legal_action_mask=legal_action_mask,
         terminated=terminated,
-        reward=reward,
+        rewards=reward,
     )
 
 
 def _observe(state: State, player_id: jnp.ndarray) -> jnp.ndarray:
     state, flip_state = jax.lax.cond(
         state.current_player == player_id,
         lambda: (state, _flip(state)),
```

### Comparing `pgx-0.6.1/pgx/backgammon.py` & `pgx-0.7.0/pgx/backgammon.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 FALSE = jnp.bool_(False)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(34, dtype=jnp.int8)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     # micro action = 6 * src + die
     legal_action_mask: jnp.ndarray = jnp.zeros(6 * 26 + 6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Backgammon specific ---
     # 各point(24) bar(2) off(2)にあるcheckerの数. 黒+, 白-
     _board: jnp.ndarray = jnp.zeros(28, dtype=jnp.int8)
@@ -50,16 +51,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "backgammon"
 
 
 class Backgammon(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -164,19 +165,19 @@
 ) -> State:
     """
     勝利者がいる場合のstep.
     """
     win_score = _calc_win_score(state._board)
     winner = state.current_player
     loser = 1 - winner
-    reward = jnp.ones_like(state.reward)
+    reward = jnp.ones_like(state.rewards)
     reward = reward.at[winner].set(win_score)
     reward = reward.at[loser].set(-win_score)
     state = state.replace(terminated=TRUE)  # type: ignore
-    return state.replace(reward=reward)  # type: ignore
+    return state.replace(rewards=reward)  # type: ignore
 
 
 def _no_winning_step(state: State, action: jnp.ndarray) -> State:
     """
     勝利者がいない場合のstep, ターン終了の条件を満たせばターンを変更する.
     """
     return jax.lax.cond(
```

### Comparing `pgx-0.6.1/pgx/bridge_bidding.py` & `pgx-0.7.0/pgx/bridge_bidding.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,17 @@
 TO_CARD = ["A", "2", "3", "4", "5", "6", "7", "8", "9", "T", "J", "Q", "K"]
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(-1)
     observation: jnp.ndarray = jnp.zeros(478, dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0, 0, 0, 0])
+    rewards: jnp.ndarray = jnp.float32([0, 0, 0, 0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(38, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # turn 現在のターン数
     _turn: jnp.ndarray = jnp.int16(0)
     # シャッフルされたプレイヤーの並び
     _shuffled_players: jnp.ndarray = jnp.zeros(4, dtype=jnp.int8)
@@ -86,21 +87,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "bridge_bidding"
 
 
 class BridgeBidding(v1.Env):
-    def __init__(
-        self,
-        *,
-        auto_reset: bool = False,
-        dds_hash_table_path: Optional[str] = None
-    ):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self, *, dds_hash_table_path: Optional[str] = None):
+        super().__init__()
         if dds_hash_table_path is None:
             dds_hash_table_path = os.path.join(
                 os.getcwd(), "dds_hash_table.npz"
             )
         try:
             self.hash_keys, self.hash_values = jnp.load(dds_hash_table_path)
         except FileNotFoundError as e:
@@ -378,15 +374,15 @@
     hash_keys: jnp.ndarray,
     hash_values: jnp.ndarray,
 ) -> State:
     """Return state if the game is successfully completed"""
     terminated = jnp.bool_(True)
     reward = _reward(state, hash_keys, hash_values)
     # fmt: off
-    return state.replace(terminated=terminated, reward=reward)  # type: ignore
+    return state.replace(terminated=terminated, rewards=reward)  # type: ignore
     # fmt: on
 
 
 @jax.jit
 def _continue_step(
     state: State,
 ) -> State:
@@ -397,15 +393,15 @@
         current_player=state._shuffled_players[(state._dealer + state._turn + 1) % 4],
         _turn=state._turn + 1
     )
     # 次のターンにX, XXが合法手か判断
     x_mask, xx_mask = _update_legal_action_X_XX(state)
     return state.replace(  # type: ignore
         legal_action_mask=state.legal_action_mask.at[36].set(x_mask).at[37].set(xx_mask),
-        reward=jnp.zeros(4, dtype=jnp.float32)
+        rewards=jnp.zeros(4, dtype=jnp.float32)
     )
     # fmt: on
 
 
 @jax.jit
 def _is_terminated(state: State) -> bool:
     """Check if the game is finished
```

### Comparing `pgx-0.6.1/pgx/chess.py` & `pgx-0.7.0/pgx/chess.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,17 @@
 #    38                10                64
 # 37                    9                   64
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # 64 * 73 = 4672
     observation: jnp.ndarray = jnp.zeros((8, 8, 19), dtype=jnp.float32)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Chess specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     _board: jnp.ndarray = INIT_BOARD  # 左上からFENと同じ形式で埋めていく
@@ -179,16 +180,16 @@
     def _to_label(self):
         plane = PLANE_MAP[self.from_, self.to]
         # plane = jax.lax.select(self.underpromotion >= 0, ..., plane)
         return jnp.int32(self.from_) * 73 + jnp.int32(plane)
 
 
 class Chess(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
         # AlphaZero paper does not mention the number of max termination steps
         # but we believe 1000 is large enough for Chess.
         self.max_termination_steps = 1000
 
     def _init(self, key: jax.random.KeyArray) -> State:
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
@@ -250,15 +251,15 @@
         is_checkmate,
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
         jnp.zeros(2, dtype=jnp.float32),
     )
     # fmt: on
     return state.replace(  # type: ignore
         terminated=terminated,
-        reward=reward,
+        rewards=reward,
     )
 
 
 def has_insufficient_pieces(state: State):
     # Uses the same condition as OpenSpiel.
     # See https://github.com/deepmind/open_spiel/blob/master/open_spiel/games/chess/chess_board.cc#L724
     num_pieces = (state._board != EMPTY).sum()
```

### Comparing `pgx-0.6.1/pgx/connect_four.py` & `pgx-0.7.0/pgx/connect_four.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((6, 7, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(7, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Connect Four specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 6x7 board
     # [[ 0,  1,  2,  3,  4,  5,  6],
@@ -45,16 +46,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "connect_four"
 
 
 class ConnectFour(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -124,15 +125,15 @@
     return state.replace(  # type: ignore
         current_player=1 - state.current_player,
         legal_action_mask=blank_row >= 0,
         _turn=1 - state._turn,
         _board=board,
         _blank_row=blank_row,
         terminated=won | jnp.all(blank_row == -1),
-        reward=reward,
+        rewards=reward,
     )
 
 
 def _to_idx(row, col):
     return row * 7 + col
```

### Comparing `pgx-0.6.1/pgx/experimental/bridge_bidding.py` & `pgx-0.7.0/pgx/experimental/bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
     return jax.lax.cond(
         ~state.terminated,
         lambda: (state, table_a_reward, has_duplicate_result),
         lambda: jax.lax.cond(
             has_duplicate_result,
             lambda: (
                 state.replace(  # type: ignore
-                    reward=_imp_reward(table_a_reward, state.reward)
+                    reward=_imp_reward(table_a_reward, state.rewards)
                 ),
                 jnp.zeros(4, dtype=jnp.float32),
                 jnp.bool_(True),
             ),
-            lambda: (_duplicate_init(state), state.reward, jnp.bool_(True)),
+            lambda: (_duplicate_init(state), state.rewards, jnp.bool_(True)),
         ),
     )
```

### Comparing `pgx-0.6.1/pgx/experimental/gym.py` & `pgx-0.7.0/pgx/experimental/gym.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/experimental/pettingzoo.py` & `pgx-0.7.0/pgx/experimental/pettingzoo.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self._state = self._step_fn(self._state, jnp.int32(action))
 
         next_agent = f"player_{self._state.current_player}"
 
         if self._state.terminated:
             for i in range(self._num_players):
-                self.rewards[f"player_{i}"] = float(self._state.reward[i])
+                self.rewards[f"player_{i}"] = float(self._state.rewards[i])
             self.terminations = {i: True for i in self.agents}
 
         self._cumulative_rewards[self.agent_selection] = 0
         self.agent_selection = next_agent
 
         self._accumulate_rewards()
         if self.render_mode == "svg":
```

### Comparing `pgx-0.6.1/pgx/experimental/visualize.py` & `pgx-0.7.0/pgx/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/go.py` & `pgx-0.7.0/pgx/go.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,17 @@
 FALSE = jnp.bool_(False)
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(19 * 19 + 1, dtype=jnp.bool_)
     observation: jnp.ndarray = jnp.zeros((19, 19, 17), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Go specific ---
     _size: jnp.ndarray = jnp.int32(19)  # NOTE: require 19 * 19 > int8
     # ids of representative stone id (smallest) in the connected stones
@@ -58,20 +59,19 @@
         return f"go_{size}x{size}"  # type: ignore
 
 
 class Go(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         size: int = 19,
         komi: float = 7.5,
         history_length: int = 8,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         assert isinstance(size, int)
         self.size = size
         self.komi = komi
         self.history_length = history_length
         self.max_termination_steps = self.size * self.size * 2
 
     def _init(self, key: jax.random.KeyArray) -> State:
@@ -82,15 +82,15 @@
         state = partial(_step, size=self.size)(state, action)
         # terminates if size * size * 2 (722 if size=19) steps are elapsed
         state = jax.lax.cond(
             (0 <= self.max_termination_steps)
             & (self.max_termination_steps <= state._step_count),
             lambda: state.replace(  # type: ignore
                 terminated=TRUE,
-                reward=partial(_get_reward, size=self.size)(state),
+                rewards=partial(_get_reward, size=self.size)(state),
             ),
             lambda: state,
         )
         return state  # type: ignore
 
     def _observe(self, state: v1.State, player_id: jnp.ndarray) -> jnp.ndarray:
         assert isinstance(state, State)
@@ -207,17 +207,17 @@
     return state
 
 
 def _pass_move(state: State, size) -> State:
     return jax.lax.cond(
         state._passed,
         # consecutive passes results in the game end
-        lambda: state.replace(terminated=TRUE, reward=_get_reward(state, size)),  # type: ignore
+        lambda: state.replace(terminated=TRUE, rewards=_get_reward(state, size)),  # type: ignore
         # One pass continues the game
-        lambda: state.replace(_passed=TRUE, reward=jnp.zeros(2, dtype=jnp.float32)),  # type: ignore
+        lambda: state.replace(_passed=TRUE, rewards=jnp.zeros(2, dtype=jnp.float32)),  # type: ignore
     )
 
 
 def _not_pass_move(state: State, action, size) -> State:
     state = state.replace(_passed=FALSE)  # type: ignore
     xy = action
     num_captured_stones_before = state._num_captured_stones[state._turn]
@@ -262,15 +262,15 @@
     state = jax.lax.cond(
         state._num_captured_stones[state._turn] - num_captured_stones_before == 1,
         lambda: state,
         lambda: state.replace(_ko=jnp.int32(-1)),  # type:ignore
     )
     # fmt: on
 
-    return state.replace(reward=jnp.zeros(2, dtype=jnp.float32))  # type: ignore
+    return state.replace(rewards=jnp.zeros(2, dtype=jnp.float32))  # type: ignore
 
 
 def _merge_around_xy(i, state: State, xy, size):
     my_color = _my_color(state)
     adj_xy = _neighbour(xy, size)[i]
     is_off = adj_xy == -1
     is_my_chain = state._chain_id_board[adj_xy] * my_color > 0
@@ -518,15 +518,15 @@
     # fmt: off
     is_psk = ~state._passed & (jnp.abs(state._board_history[0] - state._board_history[1:]).sum(axis=1) == 0).any()
     winner = state.current_player
     state = jax.lax.cond(
         is_psk,
         lambda: state.replace(  # type: ignore
             terminated=TRUE,
-            reward=jnp.float32([-1, -1]).at[winner].set(1.0),
+            rewards=jnp.float32([-1, -1]).at[winner].set(1.0),
         ),
         lambda: state,
     )
     # fmt: on
     return state
```

### Comparing `pgx-0.6.1/pgx/hex.py` & `pgx-0.7.0/pgx/hex.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((11, 11, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(11 * 11, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Hex specific ---
     _size: jnp.ndarray = jnp.int8(11)
     # 0(black), 1(white)
     _turn: jnp.ndarray = jnp.int8(0)
@@ -50,16 +51,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "hex"
 
 
 class Hex(v1.Env):
-    def __init__(self, *, size: int = 11, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self, *, size: int = 11):
+        super().__init__()
         assert isinstance(size, int)
         self.size = size
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return partial(_init, size=self.size)(rng=key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
@@ -111,15 +112,15 @@
     )
 
     legal_action_mask = board == 0
     state = state.replace(  # type:ignore
         current_player=1 - state.current_player,
         _turn=1 - state._turn,
         _board=board * -1,
-        reward=reward,
+        rewards=reward,
         terminated=won,
         legal_action_mask=legal_action_mask,
     )
 
     return state
```

### Comparing `pgx-0.6.1/pgx/kuhn_poker.py` & `pgx-0.7.0/pgx/kuhn_poker.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 CHECK = jnp.int8(3)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Kuhn poker specific ---
     _cards: jnp.ndarray = jnp.int8([-1, -1])
     # [(player 0),(player 1)]
     _last_action: jnp.ndarray = jnp.int8(-1)
@@ -44,16 +45,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "kuhn_poker"
 
 
 class KuhnPoker(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -126,15 +127,15 @@
     )
 
     return state.replace(  # type:ignore
         current_player=1 - state.current_player,
         _last_action=action,
         legal_action_mask=legal_action,
         terminated=terminated,
-        reward=reward,
+        rewards=reward,
         _pot=pot,
     )
 
 
 def _get_unit_reward(state: State):
     return jax.lax.cond(
         state._cards[state.current_player]
```

### Comparing `pgx-0.6.1/pgx/leduc_holdem.py` & `pgx-0.7.0/pgx/leduc_holdem.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 MAX_RAISE = jnp.int8(2)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Leduc Hold'Em specific ---
     _first_player: jnp.ndarray = jnp.int8(0)
     # [(player 0), (player 1), (public)]
     _cards: jnp.ndarray = jnp.int8([-1, -1, -1])
@@ -50,16 +51,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "leduc_holdem"
 
 
 class LeducHoldem(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -134,15 +135,15 @@
     legal_action = legal_action.at[RAISE].set(raise_count < MAX_RAISE)
 
     return state.replace(  # type:ignore
         current_player=current_player,
         _last_action=last_action,
         legal_action_mask=legal_action,
         terminated=terminated,
-        reward=reward,
+        rewards=reward,
         _round=state._round + jnp.int8(round_over),
         _chips=chips,
         _raise_count=raise_count,
     )
 
 
 def _check_round_over(state, action):
```

### Comparing `pgx-0.6.1/pgx/minatar/asterix.py` & `pgx-0.7.0/pgx/minatar/asterix.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,17 @@
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
+    rewards: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(5, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Asterix specific ---
     _player_x: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _player_y: jnp.ndarray = jnp.array(5, dtype=jnp.int32)
     _entities: jnp.ndarray = jnp.ones((8, 4), dtype=jnp.int32) * INF
@@ -73,19 +74,18 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarAsterix(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
@@ -267,15 +267,15 @@
             state._ramp_timer,
             state._ramp_index,
         ),
     )
     state = state.replace(_spawn_speed=spawn_speed, _move_speed=move_speed, _ramp_timer=ramp_timer, _ramp_index=ramp_index)  # type: ignore
 
     state = state.replace(  # type: ignore
-        reward=r[jnp.newaxis],
+        rewards=r[jnp.newaxis],
         _last_action=action,  # 1-d array
         terminated=terminal,
     )
     return state
 
 
 # Spawn a new enemy or treasure at a random location with random direction (if all rows are filled do nothing)
```

### Comparing `pgx-0.6.1/pgx/minatar/breakout.py` & `pgx-0.7.0/pgx/minatar/breakout.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 NINE = jnp.array(9, dtype=jnp.int32)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 4), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
+    rewards: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Breakout specific ---
     _ball_y: jnp.ndarray = THREE
     _ball_x: jnp.ndarray = ZERO
     _ball_dir: jnp.ndarray = TWO
@@ -68,19 +69,18 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarBreakout(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 3])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
@@ -198,15 +198,15 @@
         _pos=pos,
         _brick_map=brick_map,
         _strike=strike,
         _last_x=last_x,
         _last_y=last_y,
         _terminal=terminal,
         _last_action=action,
-        reward=r[jnp.newaxis],
+        rewards=r[jnp.newaxis],
         terminated=terminal,
     )
     return state
 
 
 def _apply_action(pos, action):
     pos = jax.lax.cond(
```

### Comparing `pgx-0.6.1/pgx/minatar/freeway.py` & `pgx-0.7.0/pgx/minatar/freeway.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 NINE = jnp.array(9, dtype=jnp.int32)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 7), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
+    rewards: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(3, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Freeway specific ---
     _cars: jnp.ndarray = jnp.zeros((8, 4), dtype=jnp.int32)
     _pos: jnp.ndarray = jnp.array(9, dtype=jnp.int32)
     _move_timer: jnp.ndarray = jnp.array(player_speed, dtype=jnp.int32)
@@ -62,19 +63,18 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarFreeway(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 2, 4])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
@@ -183,15 +183,15 @@
     next_state = state.replace(  # type: ignore
         _cars=cars,
         _pos=pos,
         _move_timer=move_timer,
         _terminate_timer=terminate_timer,
         _terminal=terminal,
         _last_action=last_action,
-        reward=r[jnp.newaxis],
+        rewards=r[jnp.newaxis],
         terminated=terminal,
     )
 
     return next_state
 
 
 def _update_cars(pos, cars):
```

### Comparing `pgx-0.6.1/pgx/minatar/seaquest.py` & `pgx-0.7.0/pgx/minatar/seaquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 FALSE: jnp.ndarray = jnp.bool_(False)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 10), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
+    rewards: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(6, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar Seaquest specific ---
     _oxygen: jnp.ndarray = MAX_OXYGEN
     _diver_count: jnp.ndarray = ZERO
     _sub_x: jnp.ndarray = jnp.int32(5)
@@ -85,19 +86,18 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSeaquest(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 2, 3, 4, 5])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
@@ -293,15 +293,15 @@
         _d_spawn_timer=d_spawn_timer,
         _move_speed=move_speed,
         _ramp_index=ramp_index,
         _shot_timer=shot_timer,
         _surface=surface,
         _terminal=terminal,
         _last_action=action,
-        reward=r[jnp.newaxis],
+        rewards=r[jnp.newaxis],
         terminated=terminal,
     )
     return state
 
 
 def find_ix(arr):
     ix = lax.while_loop(lambda i: arr[i][0] != -1, lambda i: i + 1, 0)
```

### Comparing `pgx-0.6.1/pgx/minatar/space_invaders.py` & `pgx-0.7.0/pgx/minatar/space_invaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 NINE = jnp.int32(9)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((10, 10, 6), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
+    rewards: jnp.ndarray = jnp.zeros(1, dtype=jnp.float32)  # (1,)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- MinAtar SpaceInvaders specific ---
     _pos: jnp.ndarray = jnp.int32(5)
     _f_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
     _e_bullet_map: jnp.ndarray = jnp.zeros((10, 10), dtype=jnp.bool_)
@@ -72,19 +73,18 @@
         visualize_minatar(self, filename)
 
 
 class MinAtarSpaceInvaders(v1.Env):
     def __init__(
         self,
         *,
-        auto_reset: bool = False,
         use_minimal_action_set: bool = True,
         sticky_action_prob: float = 0.1,
     ):
-        super().__init__(auto_reset=auto_reset)
+        super().__init__()
         self.use_minimal_action_set = use_minimal_action_set
         self.sticky_action_prob: float = sticky_action_prob
         self.minimal_action_set = jnp.int32([0, 1, 3, 5])
         self.legal_action_mask = jnp.ones(6, dtype=jnp.bool_)
         if self.use_minimal_action_set:
             self.legal_action_mask = jnp.ones(
                 self.minimal_action_set.shape[0], dtype=jnp.bool_
@@ -250,15 +250,15 @@
         _enemy_move_interval=enemy_move_interval,
         _alien_move_timer=alien_move_timer,
         _alien_shot_timer=alien_shot_timer,
         _ramp_index=ramp_index,
         _shot_timer=shot_timer,
         _terminal=terminal,
         _last_action=action,
-        reward=r[jnp.newaxis],
+        rewards=r[jnp.newaxis],
         terminated=terminal,
     )
 
 
 def _resole_action(pos, f_bullet_map, shot_timer, action):
     f_bullet_map = lax.cond(
         (action == 5) & (shot_timer == 0),
```

### Comparing `pgx-0.6.1/pgx/minatar/utils.py` & `pgx-0.7.0/pgx/minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/pgx/othello.py` & `pgx-0.7.0/pgx/othello.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((8, 8, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(64 + 1, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Othello specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 8x8 board
     # [[ 0,  1,  2,  3,  4,  5,  6,  7],
@@ -47,16 +48,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "othello"
 
 
 class Othello(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -188,15 +189,15 @@
     return state.replace(
         current_player=1 - state.current_player,
         _turn=1 - state._turn,
         legal_action_mask=state.legal_action_mask.at[:64]
         .set(legal_action)
         .at[64]
         .set(~legal_action.any()),
-        reward=reward,
+        rewards=reward,
         terminated=terminated,
         _board=-jnp.where(jnp.int8(opp), -1, jnp.int8(my)),
         _passed=action == 64,
     )
 
 
 def _check_line(pos, opp, shift, mask):
```

### Comparing `pgx-0.6.1/pgx/play2048.py` & `pgx-0.7.0/pgx/play2048.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,16 +24,17 @@
 ZERO = jnp.int8(0)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros(16, dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(4, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- 2048 specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 4x4 board
     # [[ 0,  1,  2,  3],
@@ -55,16 +56,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "2048"
 
 
 class Play2048(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -129,15 +130,15 @@
             ]
         )
     )
 
     return state.replace(  # type:ignore
         _rng_key=_rng_key,
         _board=board_2d.ravel(),
-        reward=jnp.float32([reward.sum()]),
+        rewards=jnp.float32([reward.sum()]),
         legal_action_mask=legal_action.ravel(),
         terminated=~legal_action.any(),
     )
 
 
 def _observe(state: State, player_id) -> jnp.ndarray:
     obs = jnp.zeros((16, 31), dtype=jnp.bool_)
```

### Comparing `pgx-0.6.1/pgx/shogi.py` & `pgx-0.7.0/pgx/shogi.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,16 +68,17 @@
 
 ALL_SQ = jnp.arange(81)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = INIT_LEGAL_ACTION_MASK  # (27 * 81,)
     observation: jnp.ndarray = jnp.zeros((119, 9, 9), dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Shogi specific ---
     _turn: jnp.ndarray = jnp.int8(0)  # 0 or 1
     _board: jnp.ndarray = INIT_PIECE_BOARD  # (81,) 後手のときにはflipする
@@ -110,18 +111,16 @@
 
     def _to_sfen(self):
         state = self if self._turn % 2 == 0 else _flip(self)
         return _to_sfen(state)
 
 
 class Shogi(v1.Env):
-    def __init__(
-        self, *, auto_reset: bool = False, max_termination_steps: int = 1000
-    ):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self, *, max_termination_steps: int = 1000):
+        super().__init__()
         self.max_termination_steps = max_termination_steps
 
     def _init(self, key: jax.random.KeyArray) -> State:
         state = _init_board()
         rng, subkey = jax.random.split(key)
         current_player = jnp.int8(jax.random.bernoulli(subkey))
         return state.replace(current_player=current_player)  # type: ignore
@@ -252,15 +251,15 @@
         jnp.ones(2, dtype=jnp.float32).at[state.current_player].set(-1),
         jnp.zeros(2, dtype=jnp.float32),
     )
     # fmt: on
     return state.replace(  # type: ignore
         legal_action_mask=legal_action_mask,
         terminated=terminated,
-        reward=reward,
+        rewards=reward,
     )
 
 
 def _step_move(state: State, action: Action) -> State:
     pb = state._board
     # remove piece from the original position
     pb = pb.at[action.from_].set(EMPTY)
```

### Comparing `pgx-0.6.1/pgx/sparrow_mahjong.py` & `pgx-0.7.0/pgx/sparrow_mahjong.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,17 @@
 MAX_SCORE = 26  # 親の中含むスーパーレッド自摸和了 (1 + 2 + 20 + 2) // 2 * 2
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((15, 11), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.zeros(3, dtype=jnp.float32)
+    rewards: jnp.ndarray = jnp.zeros(3, dtype=jnp.float32)
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.zeros(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Sparrow Mahjong specific ---
     _turn: jnp.ndarray = jnp.int32(0)  # 0 = dealer
     _rivers: jnp.ndarray = -jnp.ones(
         (N_PLAYER, MAX_RIVER_LENGTH), dtype=jnp.int32
@@ -89,16 +90,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "sparrow_mahjong"
 
 
 class SparrowMahjong(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         key, subkey = jax.random.split(key)
         state = _init(subkey)
 
         def f(x):
             k, _subkey = jax.random.split(x[0])
@@ -301,15 +302,15 @@
     )
     r = (
         _order_by_player_idx(scores, state._shuffled_players).astype(
             jnp.float32
         )
         / MAX_SCORE
     )
-    return state.replace(reward=r)  # type: ignore
+    return state.replace(rewards=r)  # type: ignore
 
 
 def _step_by_tsumo(state: State, scores):
     scores = scores.at[0].add(2)
     winner_score = scores[state._turn]
     loser_score = jnp.ceil(winner_score / (N_PLAYER - 1)).astype(jnp.int32)
     winner_score = loser_score * (N_PLAYER - 1)
@@ -322,23 +323,23 @@
     )
     r = (
         _order_by_player_idx(scores, state._shuffled_players).astype(
             jnp.float32
         )
         / MAX_SCORE
     )
-    return state.replace(reward=r)  # type: ignore
+    return state.replace(rewards=r)  # type: ignore
 
 
 def _step_by_tie(state):
     state = state.replace(  # type: ignore
         terminated=jnp.bool_(True),
         legal_action_mask=jnp.zeros_like(state.legal_action_mask),
     )
-    return state.replace(reward=jnp.zeros(3, dtype=jnp.float32))  # type: ignore
+    return state.replace(rewards=jnp.zeros(3, dtype=jnp.float32))  # type: ignore
 
 
 def _draw_tile(state: State) -> State:
     turn = state._turn + 1
     current_player = state._shuffled_players[turn % N_PLAYER]
     tile_id = state._wall[state._draw_ix]
     tile_type = tile_id // 4
@@ -360,15 +361,15 @@
         _draw_ix=draw_ix,
     )
     return state
 
 
 def _step_non_terminal(state: State):
     r = jnp.zeros(3, dtype=jnp.float32)
-    return state.replace(reward=r)  # type: ignore
+    return state.replace(rewards=r)  # type: ignore
 
 
 def _step_non_tied(state: State, scores):
     state = _draw_tile(state)
     scores = _hands_to_score(state)
     is_tsumo = _check_tsumo(state, scores)
     return lax.cond(
```

### Comparing `pgx-0.6.1/pgx/tic_tac_toe.py` & `pgx-0.7.0/pgx/tic_tac_toe.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 TRUE = jnp.bool_(True)
 
 
 @dataclass
 class State(v1.State):
     current_player: jnp.ndarray = jnp.int8(0)
     observation: jnp.ndarray = jnp.zeros((3, 3, 2), dtype=jnp.bool_)
-    reward: jnp.ndarray = jnp.float32([0.0, 0.0])
+    rewards: jnp.ndarray = jnp.float32([0.0, 0.0])
     terminated: jnp.ndarray = FALSE
+    truncated: jnp.ndarray = FALSE
     legal_action_mask: jnp.ndarray = jnp.ones(9, dtype=jnp.bool_)
     _rng_key: jax.random.KeyArray = jax.random.PRNGKey(0)
     _step_count: jnp.ndarray = jnp.int32(0)
     # --- Tic-tac-toe specific ---
     _turn: jnp.ndarray = jnp.int8(0)
     # 0 1 2
     # 3 4 5
@@ -40,16 +41,16 @@
 
     @property
     def env_id(self) -> v1.EnvId:
         return "tic_tac_toe"
 
 
 class TicTacToe(v1.Env):
-    def __init__(self, *, auto_reset: bool = False):
-        super().__init__(auto_reset=auto_reset)
+    def __init__(self):
+        super().__init__()
 
     def _init(self, key: jax.random.KeyArray) -> State:
         return _init(key)
 
     def _step(self, state: v1.State, action: jnp.ndarray) -> State:
         assert isinstance(state, State)
         return _step(state, action)
@@ -84,15 +85,15 @@
         won,
         lambda: jnp.float32([-1, -1]).at[state.current_player].set(1),
         lambda: jnp.zeros(2, jnp.float32),
     )
     return state.replace(  # type: ignore
         current_player=(state.current_player + 1) % 2,
         legal_action_mask=state._board < 0,
-        reward=reward,
+        rewards=reward,
         terminated=won | jnp.all(state._board != -1),
         _turn=(state._turn + 1) % 2,
     )
 
 
 def _win_check(board, turn) -> jnp.ndarray:
     idx = jnp.int8([[0, 1, 2], [3, 4, 5], [6, 7, 8], [0, 3, 6], [1, 4, 7], [2, 5, 8], [0, 4, 8], [2, 4, 6]])  # type: ignore
```

### Comparing `pgx-0.6.1/pgx/v1.py` & `pgx-0.7.0/pgx/v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,28 +77,33 @@
 
     Attributes:
         current_player (jnp.ndarray): id of agent to play.
             Note that this does NOT represent the turn (e.g., black/white in Go).
             This ID is consistent over the parallel vmapped states.
         observation (jnp.ndarray): observation for the current state.
             `Env.observe` is called to compute.
-        reward (jnp.ndarray): the `i`-th element indicates the intermediate reward for
+        rewards (jnp.ndarray): the `i`-th element indicates the intermediate reward for
             the agent with player-id `i`. If `Env.step` is called for a terminal state,
-            the following `state.reward` is zero for all players.
-        terminated (jnp.ndarray): denotes that the state is termianl state. Note that
+            the following `state.rewards` is zero for all players.
+        terminated (jnp.ndarray): denotes that the state is terminal state. Note that
             some environments (e.g., Go) have an `max_termination_steps` parameter inside
-            and will terminates within a limited number of states (following AlphaGo).
+            and will terminate within a limited number of states (following AlphaGo).
+        truncated (jnp.ndarray): indicates that the episode ends with the reason other than termination.
+            Note that current Pgx environments do not invoke truncation but users can use `TimeLimit` wrapper
+            to truncate the environment. In Pgx environments, some MinAtar games may not terminate within a finite timestep.
+            However, the other environments are supposed to terminate within a finite timestep with probability one.
         legal_action_mask (jnp.ndarray): Boolean array of legal actions. If illegal action is taken,
             the game will terminate immediately with the penalty to the palyer.
     """
 
     current_player: jnp.ndarray
     observation: jnp.ndarray
-    reward: jnp.ndarray
+    rewards: jnp.ndarray
     terminated: jnp.ndarray
+    truncated: jnp.ndarray
     legal_action_mask: jnp.ndarray
     # NOTE: _rng_key is
     #   - used for stochastic env and auto reset
     #   - updated only when actually used
     #   - supposed NOT to be used by agent
     _rng_key: jax.random.KeyArray
     _step_count: jnp.ndarray
@@ -164,16 +169,16 @@
         state = env.init(jax.random.PRNGKey(0))
         action = jax.random.int32(4)
         state = env.step(state, action)
         ```
 
     """
 
-    def __init__(self, *, auto_reset: bool = False):
-        self.auto_reset = auto_reset
+    def __init__(self):
+        ...
 
     def init(self, key: jax.random.KeyArray) -> State:
         """Return the initial state. Note that no internal state of
         environment changes.
 
         Args:
             key: pseudo-random generator key in JAX
@@ -189,30 +194,19 @@
         return state.replace(observation=observation)  # type: ignore
 
     def step(self, state: State, action: jnp.ndarray) -> State:
         """Step function."""
         is_illegal = ~state.legal_action_mask[action]
         current_player = state.current_player
 
-        # auto reset
-        state = jax.lax.cond(
-            self.auto_reset & state.terminated,
-            lambda: state.replace(  # type: ignore
-                _step_count=jnp.int32(0),
-                terminated=FALSE,
-                reward=jnp.zeros_like(state.reward),
-            ),
-            lambda: state,
-        )
-
         # If the state is already terminated or truncated, environment does not take usual step,
         # but return the same state with zero-rewards for all players
         state = jax.lax.cond(
-            state.terminated,
-            lambda: state.replace(reward=jnp.zeros_like(state.reward)),  # type: ignore
+            (state.terminated | state.truncated),
+            lambda: state.replace(rewards=jnp.zeros_like(state.rewards)),  # type: ignore
             lambda: self._step(state.replace(_step_count=state._step_count + 1), action),  # type: ignore
         )
 
         # Taking illegal action leads to immediate game terminal with negative reward
         state = jax.lax.cond(
             is_illegal,
             lambda: self._step_with_illegal_action(state, current_player),
@@ -229,38 +223,14 @@
             ),
             lambda: state,
         )
 
         observation = self.observe(state, state.current_player)
         state = state.replace(observation=observation)  # type: ignore
 
-        # auto reset
-        state = jax.lax.cond(
-            self.auto_reset & state.terminated,
-            # state is replaced by initial state,
-            # but preserve (terminated, truncated, reward)
-            lambda: self.init(state._rng_key).replace(  # type: ignore
-                terminated=state.terminated,
-                reward=state.reward,
-            ),
-            lambda: state,
-        )
-        # NOTE on final observation
-        # When auto reset happened, the terminal (or truncated) observation is replaced by initial observation,
-        # This is NOT problematic if it's termination.
-        # However, when truncation happened, final observation might be used by agent (for bootstrap)
-        # So we have to preserve the final observation somewhere. For example, in Gymnasium,
-        #
-        # https://github.com/Farama-Foundation/Gymnasium/blob/main/gymnasium/wrappers/autoreset.py#L59
-        #
-        # However, currently, truncation does **NOT** actually happens in Pgx environments because
-        # all of Pgx environments (games) are finite-horizon and terminates within reasonable # of steps.
-        # (NOTE: Chess, Shogi, and Go have `max_termination_steps` parameter following AlphaZero paper)
-        # So we believe current implementation is sufficient (final observation is not necessary).
-
         return state
 
     def observe(self, state: State, player_id: jnp.ndarray) -> jnp.ndarray:
         """Observation function."""
         obs = self._observe(state, player_id)
         return jax.lax.stop_gradient(obs)
 
@@ -318,29 +288,29 @@
         return -1.0
 
     def _step_with_illegal_action(
         self, state: State, loser: jnp.ndarray
     ) -> State:
         penalty = self._illegal_action_penalty
         reward = (
-            jnp.ones_like(state.reward)
+            jnp.ones_like(state.rewards)
             * (-1 * penalty)
             * (self.num_players - 1)
         )
         reward = reward.at[loser].set(penalty)
-        return state.replace(reward=reward, terminated=TRUE)  # type: ignore
+        return state.replace(rewards=reward, terminated=TRUE)  # type: ignore
 
 
-def available_games() -> Tuple[EnvId, ...]:
+def available_envs() -> Tuple[EnvId, ...]:
     """List up all environment id available in `pgx.make` function.
 
     !!! example "Example usage"
 
         ```py
-        pgx.available_games()
+        pgx.available_envs()
         ('2048', 'animal_shogi', 'backgammon', 'chess', 'connect_four', 'go_9x9', 'go_19x19', 'hex', 'kuhn_poker', 'leduc_holdem', 'minatar-asterix', 'minatar-breakout', 'minatar-freeway', 'minatar-seaquest', 'minatar-space_invaders', 'othello', 'shogi', 'sparrow_mahjong', 'tic_tac_toe')
         ```
 
 
     !!! note "`BridgeBidding` environment"
 
         `BridgeBidding` environment requires the domain knowledge of bridge game.
@@ -349,15 +319,15 @@
 
     """
     games = get_args(EnvId)
     games = tuple(filter(lambda x: x != "bridge_bidding", games))
     return games
 
 
-def make(env_id: EnvId, *, auto_reset: bool = False):  # noqa: C901
+def make(env_id: EnvId):  # noqa: C901
     """Load the specified environment.
 
     !!! example "Example usage"
 
         ```py
         env = pgx.make("tic_tac_toe")
         ```
@@ -370,85 +340,85 @@
 
     """
     # NOTE: BridgeBidding environment requires the domain knowledge of bridge
     # So we forbid users to load the bridge environment by `make("bridge_bidding")`.
     if env_id == "2048":
         from pgx.play2048 import Play2048
 
-        return Play2048(auto_reset=auto_reset)
+        return Play2048()
     elif env_id == "animal_shogi":
         from pgx.animal_shogi import AnimalShogi
 
-        return AnimalShogi(auto_reset=auto_reset)
+        return AnimalShogi()
     elif env_id == "backgammon":
         from pgx.backgammon import Backgammon
 
-        return Backgammon(auto_reset=auto_reset)
+        return Backgammon()
     elif env_id == "chess":
         from pgx.chess import Chess
 
-        return Chess(auto_reset=auto_reset)
+        return Chess()
     elif env_id == "connect_four":
         from pgx.connect_four import ConnectFour
 
-        return ConnectFour(auto_reset=auto_reset)
+        return ConnectFour()
     elif env_id == "go_9x9":
         from pgx.go import Go
 
-        return Go(auto_reset=auto_reset, size=9, komi=7.5)
+        return Go(size=9, komi=7.5)
     elif env_id == "go_19x19":
         from pgx.go import Go
 
-        return Go(auto_reset=auto_reset, size=19, komi=7.5)
+        return Go(size=19, komi=7.5)
     elif env_id == "hex":
         from pgx.hex import Hex
 
-        return Hex(auto_reset=auto_reset)
+        return Hex()
     elif env_id == "kuhn_poker":
         from pgx.kuhn_poker import KuhnPoker
 
-        return KuhnPoker(auto_reset=auto_reset)
+        return KuhnPoker()
     elif env_id == "leduc_holdem":
         from pgx.leduc_holdem import LeducHoldem
 
-        return LeducHoldem(auto_reset=auto_reset)
+        return LeducHoldem()
     elif env_id == "minatar-asterix":
         from pgx.minatar.asterix import MinAtarAsterix
 
-        return MinAtarAsterix(auto_reset=auto_reset)
+        return MinAtarAsterix()
     elif env_id == "minatar-breakout":
         from pgx.minatar.breakout import MinAtarBreakout
 
-        return MinAtarBreakout(auto_reset=auto_reset)
+        return MinAtarBreakout()
     elif env_id == "minatar-freeway":
         from pgx.minatar.freeway import MinAtarFreeway
 
-        return MinAtarFreeway(auto_reset=auto_reset)
+        return MinAtarFreeway()
     elif env_id == "minatar-seaquest":
         from pgx.minatar.seaquest import MinAtarSeaquest
 
-        return MinAtarSeaquest(auto_reset=auto_reset)
+        return MinAtarSeaquest()
     elif env_id == "minatar-space_invaders":
         from pgx.minatar.space_invaders import MinAtarSpaceInvaders
 
-        return MinAtarSpaceInvaders(auto_reset=auto_reset)
+        return MinAtarSpaceInvaders()
     elif env_id == "othello":
         from pgx.othello import Othello
 
-        return Othello(auto_reset=auto_reset)
+        return Othello()
     elif env_id == "shogi":
         from pgx.shogi import Shogi
 
-        return Shogi(auto_reset=auto_reset)
+        return Shogi()
     elif env_id == "sparrow_mahjong":
         from pgx.sparrow_mahjong import SparrowMahjong
 
-        return SparrowMahjong(auto_reset=auto_reset)
+        return SparrowMahjong()
     elif env_id == "tic_tac_toe":
         from pgx.tic_tac_toe import TicTacToe
 
-        return TicTacToe(auto_reset=auto_reset)
+        return TicTacToe()
     else:
-        available_envs = "\n".join(available_games())
+        envs = "\n".join(available_envs())
         raise ValueError(
-            f"Wrong env_id is passed. Available ids are: \n{available_envs}"
+            f"Wrong env_id '{env_id}' is passed. Available ids are: \n{envs}"
         )
```

### Comparing `pgx-0.6.1/pgx.egg-info/PKG-INFO` & `pgx-0.7.0/pgx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgx
-Version: 0.6.1
+Version: 0.7.0
 Summary: GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)
 Home-page: https://github.com/sotetsuk/pgx
 Author: Sotetsu KOYAMADA
 Author-email: sotetsu.koyamada@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -58,15 +58,15 @@
 env = pgx.make("go_19x19")
 init = jax.jit(jax.vmap(env.init))  # vectorize and JIT-compile
 step = jax.jit(jax.vmap(env.step))
 
 batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size)
 state = init(keys)  # vectorized states
-while not state.terminated.all():
+while not (state.terminated | state.terminated).all():
     action = model(state.current_player, state.observation, state.legal_action_mask)
     state = step(state, action)  # state.reward (2,)
 ```
 
 > ⚠️ Pgx is currently in the beta version. Therefore, API is subject to change without notice. We aim to release v1.0.0 in April 2023. Opinions and comments are more than welcome!
 
 <!---
@@ -90,15 +90,15 @@
 ## Supported games
 
 | Backgammon | Chess | Shogi | Go |
 |:---:|:---:|:---:|:---:|
 |<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only" width="158px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-light-mode-only" width="158px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only" width="170px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only" width="170px">|<img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-dark-mode-only" width="160px"><img src="https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only" width="160px">|
 
 
-Use `pgx.available_games() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
+Use `pgx.available_envs() -> Tuple[EnvId]` to see the list of currently available games. Given an `<EnvId>`, you can create the environment via
 
 ```py
 >>> env = pgx.make(<EnvId>)
 ```
 
 You can check the current version of each environment by
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pgx Version: 0.6.1 Summary: GPU/TPU-accelerated
+Metadata-Version: 2.1 Name: pgx Version: 0.7.0 Summary: GPU/TPU-accelerated
 parallel game simulators for reinforcement learning (RL) Home-page: https://
 github.com/sotetsuk/pgx Author: Sotetsu KOYAMADA Author-email:
 sotetsu.koyamada@gmail.com Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown License-
 File: LICENSE [![ci](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml/
 badge.svg)](https://github.com/sotetsuk/pgx/actions/workflows/ci.yml)
@@ -27,36 +27,37 @@
 support** including **Backgammon**, **Chess**, **Shogi**, and **Go** - ð¼ï¸
 **Beautiful visualization** in SVG format ## Installation ```sh pip install pgx
 ``` ## Usage Note that all `step` functions in Pgx environments are **JAX-
 native.**, i.e., they are all *JIT-able*. [Open_In_Colab] ```py import jax
 import pgx env = pgx.make("go_19x19") init = jax.jit(jax.vmap(env.init)) #
 vectorize and JIT-compile step = jax.jit(jax.vmap(env.step)) batch_size = 1024
 keys = jax.random.split(jax.random.PRNGKey(42), batch_size) state = init(keys)
-# vectorized states while not state.terminated.all(): action = model
-(state.current_player, state.observation, state.legal_action_mask) state = step
-(state, action) # state.reward (2,) ``` > â ï¸ Pgx is currently in the beta
-version. Therefore, API is subject to change without notice. We aim to release
-v1.0.0 in April 2023. Opinions and comments are more than welcome!  ##
-Supported games | Backgammon | Chess | Shogi | Go | |:---:|:---:|:---:|:---:| |
-[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
-backgammon_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/backgammon_light.gif#gh-light-mode-only]|[https:/
-/raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-
-dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/chess_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/shogi_dark.gif#gh-dark-mode-only][https://
-raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-
+# vectorized states while not (state.terminated | state.terminated).all():
+action = model(state.current_player, state.observation,
+state.legal_action_mask) state = step(state, action) # state.reward (2,) ``` >
+â ï¸ Pgx is currently in the beta version. Therefore, API is subject to
+change without notice. We aim to release v1.0.0 in April 2023. Opinions and
+comments are more than welcome!  ## Supported games | Backgammon | Chess |
+Shogi | Go | |:---:|:---:|:---:|:---:| |[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/backgammon_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
+backgammon_light.gif#gh-light-mode-only]|[https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/chess_dark.gif#gh-dark-mode-only][https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/chess_light.gif#gh-
 light-mode-only]|[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
-assets/go-19x19_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
-sotetsuk/pgx/main/docs/assets/go-19x19_light.gif#gh-light-mode-only]| Use
-`pgx.available_games() -> Tuple[EnvId]` to see the list of currently available
-games. Given an ``, you can create the environment via ```py >>> env = pgx.make
-() ``` You can check the current version of each environment by ```py >>>
-env.version ``` | Game/EnvId | Visualization | Version | Five-word description
-| |:---:|:---:|:---:|:---:| |2048
+assets/shogi_dark.gif#gh-dark-mode-only][https://raw.githubusercontent.com/
+sotetsuk/pgx/main/docs/assets/shogi_light.gif#gh-light-mode-only]|[https://
+raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/go-19x19_dark.gif#gh-
+dark-mode-only][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
+assets/go-19x19_light.gif#gh-light-mode-only]| Use `pgx.available_envs() -
+> Tuple[EnvId]` to see the list of currently available games. Given an ``, you
+can create the environment via ```py >>> env = pgx.make() ``` You can check the
+current version of each environment by ```py >>> env.version ``` | Game/EnvId |
+Visualization | Version | Five-word description | |:---:|:---:|:---:|:---:
+| |2048
 `"2048"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/assets/
 2048_light.gif]| `beta` | *Merge tiles to create 2048.* | |Animal_Shogi
 `"animal_shogi"` |[https://raw.githubusercontent.com/sotetsuk/pgx/main/docs/
 assets/animal_shogi_dark.gif][https://raw.githubusercontent.com/sotetsuk/pgx/
 main/docs/assets/animal_shogi_light.gif]| `beta` | *Animal-themed child-
 friendly shogi.* | |Backgammon
```

### Comparing `pgx-0.6.1/pgx.egg-info/SOURCES.txt` & `pgx-0.7.0/pgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/setup.py` & `pgx-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx",
-    version="0.6.1",
+    version="0.7.0",
     description="GPU/TPU-accelerated parallel game simulators for reinforcement learning (RL)",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/sotetsuk/pgx",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
```

### Comparing `pgx-0.6.1/tests/minatar_utils.py` & `pgx-0.7.0/tests/minatar_utils.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_animal_shogi.py` & `pgx-0.7.0/tests/test_animal_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_asterix.py` & `pgx-0.7.0/tests/test_asterix.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 minatar2pgx(s, asterix.State),
                 a,
                 lr,
                 is_gold,
                 slot,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-            assert r == s_next_pgx.reward[0]
+            assert r == s_next_pgx.rewards[0]
             assert done == s_next_pgx.terminated
 
 
 def test_observe():
     env = Environment("asterix", sticky_action_prob=0.0)
     num_actions = env.num_actions()
```

### Comparing `pgx-0.6.1/tests/test_backgammon.py` & `pgx-0.7.0/tests/test_backgammon.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_breakout.py` & `pgx-0.7.0/tests/test_breakout.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             a = random.randrange(num_actions)
             r, done = env.act(a)
             s_next = extract_state(env, state_keys)
             s_next_pgx = _step_det(
                 minatar2pgx(s, breakout.State), a
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-            assert r == s_next_pgx.reward[0]
+            assert r == s_next_pgx.rewards[0]
             assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("breakout", sticky_action_prob=0.0)
     N = 1
     for _ in range(N):
```

### Comparing `pgx-0.6.1/tests/test_bridge_bidding.py` & `pgx-0.7.0/tests/test_bridge_bidding.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,16 +85,16 @@
         )
 
 
 def test_illegal_action_penalty():
     key = jax.random.PRNGKey(0)
     state = init(key)
     state = step(state, 36)
-    print(state.reward)
-    assert jnp.all(state.reward == jnp.array([22800, -7600, 22800, 22800]))
+    print(state.rewards)
+    assert jnp.all(state.rewards == jnp.array([22800, -7600, 22800, 22800]))
 
 
 def test_step():
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
@@ -139,15 +139,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == np.zeros(4))
+    assert jnp.all(state.rewards == np.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
@@ -162,15 +162,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -185,15 +185,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 3
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 0)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -213,15 +213,15 @@
     assert state._last_bid == 0
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 8)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -243,15 +243,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -274,15 +274,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -306,15 +306,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -339,15 +339,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -372,15 +372,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -405,15 +405,15 @@
     assert state._last_bid == 8
     assert _player_position(state._last_bidder, state) == 1
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 22)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -438,15 +438,15 @@
     assert state._last_bid == 22
     assert _player_position(state._last_bidder, state) == 3
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 23)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -472,15 +472,15 @@
     assert state._last_bid == 23
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -506,15 +506,15 @@
     assert state._last_bid == 23
     assert _player_position(state._last_bidder, state) == 0
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 25)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -540,15 +540,15 @@
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 36)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -574,15 +574,15 @@
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert not state._call_xx
     assert np.all(state._first_denomination_NS == first_denomination_NS)
     assert np.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert np.all(state.reward == np.zeros(4))
+    assert np.all(state.rewards == np.zeros(4))
 
     state = step(state, 37)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -609,15 +609,15 @@
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -644,15 +644,15 @@
     assert state._last_bid == 25
     assert _player_position(state._last_bidder, state) == 2
     assert state._call_x
     assert state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 30)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -679,15 +679,15 @@
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 0
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -714,15 +714,15 @@
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -750,15 +750,15 @@
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -787,17 +787,17 @@
     assert state._last_bid == 30
     assert _player_position(state._last_bidder, state) == 2
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 3
-    assert state.reward.shape == (4,)
+    assert state.rewards.shape == (4,)
     assert jnp.all(
-        state.reward == jnp.array([-600, -600, 600, 600], dtype=jnp.int16)
+        state.rewards == jnp.array([-600, -600, 600, 600], dtype=jnp.int16)
     )
     declare_position, denomination, level, vul = _contract(state)
     assert declare_position == 0
     assert denomination == 0
     assert level == 7
     assert vul == 0
 
@@ -872,15 +872,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 1
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P
@@ -895,15 +895,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 2
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -918,15 +918,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 3
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
     state = step(state, 35)
     #  player_id: 0 = N, 1 = S, 2 = W, 3 = E
     #   0  3  1  2
     #   N  E  S  W
     #  -----------
     #      P  P  P
@@ -940,15 +940,15 @@
     assert state._last_bid == -1
     assert _player_position(state._last_bidder, state) == -1
     assert not state._call_x
     assert not state._call_xx
     assert jnp.all(state._first_denomination_NS == first_denomination_NS)
     assert jnp.all(state._first_denomination_EW == first_denomination_EW)
     assert state._pass_num == 4
-    assert jnp.all(state.reward == jnp.zeros(4))
+    assert jnp.all(state.rewards == jnp.zeros(4))
 
 
 def test_observe():
     # test init_obs
     # hand
     # hand: N:J92.J76.K72.9432 AKQ6.84.J863.T65 87543.KQ9532..K7 T.AT.AQT954.AQJ8
     player0_hand = (
```

### Comparing `pgx-0.6.1/tests/test_chess.py` & `pgx-0.7.0/tests/test_chess.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,154 +425,154 @@
 def test_terminal():
     # checkmate (white win)
     state = State._from_fen("7k/7R/5N2/8/8/8/8/K7 b - - 0 1")
     state.save_svg("tests/assets/chess/terminal_001.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert state.reward[state.current_player] == -1
-    assert state.reward[1 - state.current_player] == 1.
+    assert state.rewards[state.current_player] == -1
+    assert state.rewards[1 - state.current_player] == 1.
 
     # stalemate
     state = State._from_fen("k7/8/1Q6/K7/8/8/8/8 b - - 0 1")
     state.save_svg("tests/assets/chess/terminal_002.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # 50-move draw rule
     # FEN is from https://www.chess.com/terms/fen-chess#halfmove-clock
     state = State._from_fen("8/5k2/3p4/1p1Pp2p/pP2Pp1P/P4P1K/8/8 b - - 99 50")
     state.save_svg("tests/assets/chess/terminal_003.svg")
     state = step(state, jnp.nonzero(state.legal_action_mask, size=1)[0][0])
     state.save_svg("tests/assets/chess/terminal_004.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # insufficient pieces
     # K vs K
     state = State._from_fen("k7/8/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_005.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B vs K
     state = State._from_fen("k7/8/8/8/8/8/8/6BK w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_006.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K vs K+B
     state = State._from_fen("kb6/8/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_007.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+N vs K
     state = State._from_fen("k7/8/8/8/8/8/8/6NK w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_008.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K vs K+N
     state = State._from_fen("kn6/8/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_009.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B vs K+B (Bishop in Black tile)
     state = State._from_fen("kb6/8/8/8/8/8/8/6BK w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_010.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B vs K+B (Bishop in White tile)
     state = State._from_fen("k1b1B3/8/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_011.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # insufficient cases by underpromotion
     # K+B vs K
     state = State._from_fen("k7/7P/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_012.svg")
     state = step(state, jnp.int32(4529))
     state.save_svg("tests/assets/chess/terminal_013.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+N vs K
     state = State._from_fen("k7/7P/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_014.svg")
     state = step(state, jnp.int32(4532))
     state.save_svg("tests/assets/chess/terminal_015.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B vs K+B(Bishop in Black tile)
     state = State._from_fen("k1b5/4P3/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_016.svg")
     state = step(state, jnp.int32(2777))
     state.save_svg("tests/assets/chess/terminal_017.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B vs K+B (Bishop in White tile)
     state = State._from_fen("kb6/3P4/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_018.svg")
     state = step(state, jnp.int32(2193))
     state.save_svg("tests/assets/chess/terminal_019.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B*2 vs K(Bishop in Black tile)
     state = State._from_fen("k1B5/4P3/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_020.svg")
     state = step(state, jnp.int32(2777))
     state.save_svg("tests/assets/chess/terminal_021.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # K+B*2 vs K (Bishop in White tile)
     state = State._from_fen("kB6/3P4/8/8/8/8/8/7K w - - 0 1")
     state.save_svg("tests/assets/chess/terminal_022.svg")
     state = step(state, jnp.int32(2193))
     state.save_svg("tests/assets/chess/terminal_023.svg")
     print(state._to_fen())
     assert state.terminated
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
     # stalemate with pin
     state = State._from_fen("kbR5/pn6/P1B5/8/8/8/8/7K b - - 0 1")
     state.save_svg("tests/assets/chess/terminal_024.svg")
     print(state._to_fen())
     assert state.terminated
     assert state.current_player == 0
-    assert (state.reward == 0.0).all()
+    assert (state.rewards == 0.0).all()
 
 
 def test_buggy_samples():
     # Found buggy samples by random playing debug
 
     # Bishop by bishop
     state = State._from_fen("r1q1k1nr/2p2p1B/p3pb2/1p4pP/P1pBP3/5P1N/R2P2KP/1Nn2Q1R w kq - 4 23")
```

### Comparing `pgx-0.6.1/tests/test_connect_four.py` & `pgx-0.7.0/tests/test_connect_four.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,37 +62,37 @@
     assert state.current_player == 0
 
     for _ in range(3):
         state = step(state, 0)
         state = step(state, 1)
     state = step(state, 0)
     assert state.terminated
-    assert (state.reward == jnp.array([1.0, -1.0])).all()
+    assert (state.rewards == jnp.array([1.0, -1.0])).all()
 
     state = init(sub_key)
     for i in range(3):
         state = step(state, i)
         state = step(state, i)
     state = step(state, 3)
     assert state.terminated
-    assert (state.reward == jnp.array([1.0, -1.0])).all()
+    assert (state.rewards == jnp.array([1.0, -1.0])).all()
 
     state = init(sub_key)
     for i in [1, 2, 2, 3, 3, 4, 3, 4, 4, 6, 4]:
         state = step(state, i)
     """
     .......
     .......
     ....@..
     ...@@..
     ..@@O..
     .@OOO.O
     """
     assert state.terminated
-    assert (state.reward == jnp.array([1.0, -1.0])).all()
+    assert (state.rewards == jnp.array([1.0, -1.0])).all()
 
 
 def test_random_play():
     key = jax.random.PRNGKey(0)
     done = jnp.bool_(False)
     key, sub_key = jax.random.split(key)
     state = init(sub_key)
```

### Comparing `pgx-0.6.1/tests/test_freeway.py` & `pgx-0.7.0/tests/test_freeway.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             s_next_pgx = _step_det(
                 minatar2pgx(s, freeway.State),
                 a,
                 speeds,
                 directions,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-            assert r == s_next_pgx.reward[0]
+            assert r == s_next_pgx.rewards[0]
             assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("freeway", sticky_action_prob=0.0)
     N = 10
     for _ in range(N):
```

### Comparing `pgx-0.6.1/tests/test_go.py` & `pgx-0.7.0/tests/test_go.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     [3] O O @ + @
     [4] O O O @ +
     """
     assert (jnp.clip(state._chain_id_board, -1, 1) == expected_board.ravel()).all()
     assert state.terminated
 
     # 同点なのでコミの分 黒 == player_1 の負け
-    assert (state.reward == jnp.array([1, -1])).all()
+    assert (state.rewards == jnp.array([1, -1])).all()
 
 
 def test_ko():
     key = jax.random.PRNGKey(0)
 
     state: State = init(key=key)
     assert state.current_player == 1
@@ -123,16 +123,16 @@
 
     loser = state.current_player
     state1: State = step(
         state=state, action=12
     )  # BLACK
     # ルール違反により黒 = player_id=1 の負け
     assert state1.terminated
-    assert state1.reward[loser] == -1.
-    assert state1.reward.sum() == 0.
+    assert state1.rewards[loser] == -1.
+    assert state1.rewards.sum() == 0.
 
     state2: State = step(state=state, action=0)  # BLACK
     # 回避した場合
     assert not state2.terminated
     assert state2._ko == -1
 
     # see #468
@@ -1103,15 +1103,15 @@
     #  O O + @ O
     #  @ @ @ O O
     #  @ @ @ O +
     #  + @ O O O
     #  @ @ @ O +
     assert state.terminated
     assert state._black_player == 1
-    assert (state.reward == jnp.float32([-1, 1])).all()  # black wins
+    assert (state.rewards == jnp.float32([-1, 1])).all()  # black wins
 
 
 def test_random_play_5():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     while not state.terminated:
         actions = np.where(state.legal_action_mask)
```

### Comparing `pgx-0.6.1/tests/test_hex.py` & `pgx-0.7.0/tests/test_hex.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,29 +67,29 @@
     assert not state.terminated
 
 
 def test_reward():
     key = jax.random.PRNGKey(1)
     state = init(key=key)
     assert state.current_player == 1
-    assert (state.reward == jnp.float32([0.0, 0.0])).all()
+    assert (state.rewards == jnp.float32([0.0, 0.0])).all()
 
     for i in range(10):
         state = step(state, i * 11)
         state = step(state, i * 11 + 1)
     state = step(state, 110)
-    assert (state.reward == jnp.float32([-1.0, 1.0])).all()
+    assert (state.rewards == jnp.float32([-1.0, 1.0])).all()
 
     state = init(key=key)
     for i in range(10):
         state = step(state, i)
         state = step(state, i + 11)
     state = step(state, 120)
     state = step(state, 21)
-    assert (state.reward == jnp.float32([1.0, -1.0])).all()
+    assert (state.rewards == jnp.float32([1.0, -1.0])).all()
 
 
 def test_observe():
     """
     @ O . . .
      . . . . .
       . . . . .
@@ -118,14 +118,14 @@
     rewards = jnp.int16([0.0, 0.0])
     while not done:
         legal_actions = jnp.where(state.legal_action_mask)[0]
         key, sub_key = jax.random.split(key)
         action = jax.random.choice(sub_key, legal_actions)
         state = step(state, jnp.int16(action))
         done = state.terminated
-        rewards += state.reward
+        rewards += state.rewards
 
 
 def test_api():
     import pgx
     env = pgx.make("hex")
     pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.6.1/tests/test_kuhn_poker.py` & `pgx-0.7.0/tests/test_kuhn_poker.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,47 +19,47 @@
     key = jax.random.PRNGKey(0)
     # cards = [2, 0]
     state = init(key)
     state = step(state, CHECK)
     assert not state.terminated
     state = step(state, CHECK)
     assert state.terminated
-    assert (state.reward == jnp.float32([1, -1])).all()
+    assert (state.rewards == jnp.float32([1, -1])).all()
 
     state = init(key)
     state = step(state, CHECK)
     assert not state.terminated
     state = step(state, BET)
     assert not state.terminated
     state = step(state, FOLD)
     assert state.terminated
-    assert (state.reward == jnp.float32([-1, 1])).all()
+    assert (state.rewards == jnp.float32([-1, 1])).all()
 
     state = init(key)
     state = step(state, CHECK)
     assert not state.terminated
     state = step(state, BET)
     assert not state.terminated
     state = step(state, CALL)
     assert state.terminated
-    assert (state.reward == jnp.float32([2, -2])).all()
+    assert (state.rewards == jnp.float32([2, -2])).all()
 
     state = init(key)
     state = step(state, BET)
     assert not state.terminated
     state = step(state, FOLD)
     assert state.terminated
-    assert (state.reward == jnp.float32([1, -1])).all()
+    assert (state.rewards == jnp.float32([1, -1])).all()
 
     state = init(key)
     state = step(state, BET)
     assert not state.terminated
     state = step(state, CALL)
     assert state.terminated
-    assert (state.reward == jnp.float32([2, -2])).all()
+    assert (state.rewards == jnp.float32([2, -2])).all()
 
 
 def test_legal_action():
     key = jax.random.PRNGKey(0)
     # cards = [2, 0]
     state = init(key)
     state = step(state, CHECK)
```

### Comparing `pgx-0.6.1/tests/test_leduc_holdem.py` & `pgx-0.7.0/tests/test_leduc_holdem.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     assert state.current_player == 1
     state = step(state, CALL)
     state = step(state, RAISE)  # +4(7)
     state = step(state, RAISE)  # +4(11)
     assert not state.terminated
     state = step(state, CALL)
     assert state.terminated
-    assert (state.reward == jnp.float32([11, -11])).all()
+    assert (state.rewards == jnp.float32([11, -11])).all()
 
     state = init(key)
     assert state.current_player == 1
     # cards = [1 0]
     # player 1 is the first
 
     # first round
@@ -51,15 +51,15 @@
     # second round
     state = step(state, CALL)
     state = step(state, RAISE)  # +4(7)
     state = step(state, RAISE)  # +4(11)
     assert not state.terminated
     state = step(state, FOLD)
     assert state.terminated
-    assert (state.reward == jnp.float32([-7, 7])).all()
+    assert (state.rewards == jnp.float32([-7, 7])).all()
 
 
 def test_legal_action():
     key = jax.random.PRNGKey(0)
     state = init(key=key)
     assert (state.legal_action_mask == jnp.bool_([1, 1, 0])).all()
 
@@ -93,15 +93,15 @@
     state = step(state, CALL)
 
     state = step(state, RAISE)
     state = step(state, RAISE)
     assert not state.terminated
     state = step(state, CALL)
     assert state.terminated
-    assert (state.reward == jnp.float32([0, 0])).all()
+    assert (state.rewards == jnp.float32([0, 0])).all()
 
 
 def test_observe():
     key = jax.random.PRNGKey(5)
     state = init(key)
     """
     player 1 is the First.
```

### Comparing `pgx-0.6.1/tests/test_mahjong.py` & `pgx-0.7.0/tests/test_mahjong.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_othello.py` & `pgx-0.7.0/tests/test_othello.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     key = jax.random.PRNGKey(0)
     state = init(key)
     for i in [37, 43, 34, 29, 52, 45, 38, 44]:
         state = step(state, i)
         assert not state.terminated
     state = step(state, 20)
     assert state.terminated
-    assert (state.reward == jnp.float32([1.0, -1.0])).all()
+    assert (state.rewards == jnp.float32([1.0, -1.0])).all()
 
 
 def test_legal_action():
     # cannot put
     key = jax.random.PRNGKey(0)
     state = init(key)
     assert state.current_player == 0
@@ -123,15 +123,15 @@
     rewards = jnp.int16([0.0, 0.0])
     while not done:
         legal_actions = jnp.where(state.legal_action_mask)[0]
         key, sub_key = jax.random.split(key)
         action = jax.random.choice(sub_key, legal_actions)
         state = step(state, jnp.int16(action))
         done = state.terminated
-        rewards += state.reward
+        rewards += state.rewards
 
 
 def test_api():
     import pgx
 
     env = pgx.make("othello")
     pgx.v1_api_test(env, 10)
```

### Comparing `pgx-0.6.1/tests/test_play2048.py` & `pgx-0.7.0/tests/test_play2048.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_seaquest.py` & `pgx-0.7.0/tests/test_seaquest.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 env.state(),
                 observe(s_next_pgx),
             )
             # if not jnp.allclose(env.state(), observe(s_next_pgx)):
             #     for field in fields(s_next_pgx):
             #         print(str(field.name) + "\n" + str(getattr(s_next_pgx, field.name)) + "\n"  + str(getattr(minatar2pgx(extract_state(env, state_keys), seaquest.MinAtarSeaquestState), field.name)))
             #     assert False
-            assert r == s_next_pgx.reward[0]
+            assert r == s_next_pgx.rewards[0]
             assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("seaquest", sticky_action_prob=0.0)
     N = 100
     for _ in range(N):
```

### Comparing `pgx-0.6.1/tests/test_shogi.py` & `pgx-0.7.0/tests/test_shogi.py`

 * *Files identical despite different names*

### Comparing `pgx-0.6.1/tests/test_space_invaders.py` & `pgx-0.7.0/tests/test_space_invaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             r, done = env.act(a)
             s_next = extract_state(env, state_keys)
             s_next_pgx = _step_det(
                 minatar2pgx(s, space_invaders.State),
                 a,
             )
             assert_states(s_next, pgx2minatar(s_next_pgx, state_keys))
-            assert r == s_next_pgx.reward[0]
+            assert r == s_next_pgx.rewards[0]
             assert done == s_next_pgx.terminated
 
 
 def test_init_det():
     env = Environment("space_invaders", sticky_action_prob=0.0)
     N = 10
     for _ in range(N):
```

### Comparing `pgx-0.6.1/tests/test_sparrow_mahjong.py` & `pgx-0.7.0/tests/test_sparrow_mahjong.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         while not state.terminated:
             legal_actions = jnp.where(state.legal_action_mask)[0]
             key, subkey = jax.random.split(key)
             action = jax.random.choice(subkey, legal_actions)
             state = step(state, action)
             # _validate(state)
         print(_to_str(state))
-        print(state.reward)
+        print(state.rewards)
         results += _to_str(state)
 
     expected = """[terminated] dora: 5
  [1] 1 4 6 8*g   : 7*_ _ _ _ _ _ _ _ _  
  [0] 5 8 9*9 g   : 5 _ _ _ _ _ _ _ _ _  
  [2] 2*3 4 6 7   : _ _ _ _ _ _ _ _ _ _  
 [terminated] dora: 4
```

### Comparing `pgx-0.6.1/tests/test_tic_tac_toe.py` & `pgx-0.7.0/tests/test_tic_tac_toe.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,75 +39,75 @@
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([1, 1, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(
         state._board == jnp.int8([-1, -1, -1, -1, 0, -1, -1, -1, -1])
     )
-    assert jnp.all(state.reward == 0)  # fmt: ignore
+    assert jnp.all(state.rewards == 0)  # fmt: ignore
     assert not state.terminated
     # -1 -1 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(0)
     state = step(state, action)
     assert state.current_player == 1
     assert state._turn == 0
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 1, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(state._board == jnp.int8([1, -1, -1, -1, 0, -1, -1, -1, -1]))
-    assert jnp.all(state.reward == 0)  # fmt: ignore
+    assert jnp.all(state.rewards == 0)  # fmt: ignore
     assert not state.terminated
     #  1 -1 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(1)
     state = step(state, action)
     assert state.current_player == 0
     assert state._turn == 1
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 0, 1, 1, 0, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, -1]))
-    assert jnp.all(state.reward == 0)  # fmt: ignore
+    assert jnp.all(state.rewards == 0)  # fmt: ignore
     assert not state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1 -1 -1
 
     action = jnp.int8(8)
     state = step(state, action)
     assert state.current_player == 1
     assert state._turn == 0
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([0, 0, 1, 1, 0, 1, 1, 1, 0], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, -1, 1]))
-    assert jnp.all(state.reward == 0)  # fmt: ignore
+    assert jnp.all(state.rewards == 0)  # fmt: ignore
     assert not state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1 -1  1
 
     action = jnp.int8(7)
     state = step(state, action)
     assert state.current_player == 0
     assert state._turn == 1
     assert jnp.all(
         state.legal_action_mask
         == jnp.array([1, 1, 1, 1, 1, 1, 1, 1, 1], jnp.bool_)
     )  # fmt: ignore
     assert jnp.all(state._board == jnp.int8([1, 0, -1, -1, 0, -1, -1, 0, 1]))
-    assert jnp.all(state.reward == jnp.int16([-1, 1]))  # fmt: ignore
+    assert jnp.all(state.rewards == jnp.int16([-1, 1]))  # fmt: ignore
     assert state.terminated
     #  1  0 -1
     # -1  0 -1
     # -1  0  1
 
 
 def test_random_play():
@@ -121,15 +121,15 @@
         while not done:
             assert jnp.all(rewards == 0), state._board
             legal_actions = jnp.where(state.legal_action_mask)[0]
             key, sub_key = jax.random.split(key)
             action = jax.random.choice(sub_key, legal_actions)
             state = step(state, action)
             done = state.terminated
-            rewards += state.reward
+            rewards += state.rewards
 
 
 def test_win_check():
     board = jnp.int8([-1, -1, -1, -1, -1, -1, -1, -1, -1])
     turn = jnp.int8(1)
     assert not _win_check(board, turn)
```

