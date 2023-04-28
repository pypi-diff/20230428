# Comparing `tmp/qpsolvers-3.3.1.tar.gz` & `tmp/qpsolvers-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpsolvers-3.3.1.tar", last modified: Wed Apr 12 09:43:49 2023, max compression
+gzip compressed data, was "qpsolvers-3.4.0.tar", last modified: Fri Apr 28 13:49:12 2023, max compression
```

## Comparing `qpsolvers-3.3.1.tar` & `qpsolvers-3.4.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0     1590 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/.github/workflows/docs.yml
--rw-r--r--   0        0        0     2529 2023-03-29 16:03:40.695119 qpsolvers-3.3.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      128 2023-03-03 11:09:52.358283 qpsolvers-3.3.1/.gitignore
--rw-r--r--   0        0        0    15890 2023-04-12 09:43:12.950561 qpsolvers-3.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      916 2023-02-28 14:28:36.811176 qpsolvers-3.3.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.3.1/LICENSE
--rw-r--r--   0        0        0     9754 2023-04-11 09:57:38.987082 qpsolvers-3.3.1/README.md
--rw-r--r--   0        0        0      832 2023-02-28 13:41:23.525818 qpsolvers-3.3.1/THANKS
--rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_dense_problem.py
--rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_model_predictive_control.py
--rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_random_problems.py
--rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.3.1/benchmark/benchmark_sparse_problem.py
--rw-r--r--   0        0        0     9656 2023-03-03 11:09:52.358283 qpsolvers-3.3.1/doc/conf.py
--rw-r--r--   0        0        0     2924 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/developer-notes.rst
--rw-r--r--   0        0        0      265 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/environment.yml
--rw-r--r--   0        0        0      931 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/index.rst
--rw-r--r--   0        0        0     3707 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/installation.rst
--rw-r--r--   0        0        0     1006 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/doc/least-squares.rst
--rw-r--r--   0        0        0     5559 2023-03-03 15:29:30.344114 qpsolvers-3.3.1/doc/quadratic-programming.rst
--rw-r--r--   0        0        0     2521 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/references.rst
--rw-r--r--   0        0        0      968 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/doc/supported-solvers.rst
--rw-r--r--   0        0        0      473 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/doc/unsupported-solvers.rst
--rw-r--r--   0        0        0      636 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/README.md
--rw-r--r--   0        0        0     2030 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/box_inequalities.py
--rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.3.1/examples/constrained_linear_regression.py
--rw-r--r--   0        0        0     2790 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/dual_multipliers.py
--rw-r--r--   0        0        0     1867 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/examples/least_squares.py
--rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.3.1/examples/model_predictive_control.py
--rw-r--r--   0        0        0     2045 2023-03-03 11:01:10.969238 qpsolvers-3.3.1/examples/quadratic_program.py
--rw-r--r--   0        0        0     2656 2023-03-28 08:42:54.624660 qpsolvers-3.3.1/examples/sparse_least_squares.py
--rw-r--r--   0        0        0     2100 2023-04-12 09:42:35.095945 qpsolvers-3.3.1/pyproject.toml
--rw-r--r--   0        0        0     2295 2023-04-12 09:43:22.815073 qpsolvers-3.3.1/qpsolvers/__init__.py
--rw-r--r--   0        0        0     1317 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/_internals.py
--rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.3.1/qpsolvers/conversions/__init__.py
--rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.3.1/qpsolvers/conversions/ensure_sparse_matrices.py
--rw-r--r--   0        0        0     3561 2023-02-28 14:10:40.413484 qpsolvers-3.3.1/qpsolvers/conversions/linear_from_box_inequalities.py
--rw-r--r--   0        0        0     3762 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/conversions/socp_from_qp.py
--rw-r--r--   0        0        0     2284 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/conversions/split_dual_linear_box.py
--rw-r--r--   0        0        0     1677 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/exceptions.py
--rw-r--r--   0        0        0     8531 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/qpsolvers/problem.py
--rw-r--r--   0        0        0     6610 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/problems.py
--rw-r--r--   0        0        0     7795 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solution.py
--rw-r--r--   0        0        0     7412 2023-03-28 08:42:54.624660 qpsolvers-3.3.1/qpsolvers/solve_ls.py
--rw-r--r--   0        0        0     3437 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/solve_problem.py
--rw-r--r--   0        0        0     4698 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solve_qp.py
--rw-r--r--   0        0        0     1743 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solve_unconstrained.py
--rw-r--r--   0        0        0    12032 2023-04-11 09:56:34.196100 qpsolvers-3.3.1/qpsolvers/solvers/__init__.py
--rw-r--r--   0        0        0     6665 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/clarabel_.py
--rw-r--r--   0        0        0     9089 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/cvxopt_.py
--rw-r--r--   0        0        0     6441 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/daqp_.py
--rw-r--r--   0        0        0     8434 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/ecos_.py
--rw-r--r--   0        0        0     7813 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/gurobi_.py
--rw-r--r--   0        0        0     9571 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/highs_.py
--rw-r--r--   0        0        0     9733 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/osqp_.py
--rw-r--r--   0        0        0     9807 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/proxqp_.py
--rw-r--r--   0        0        0    13544 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/qpoases_.py
--rw-r--r--   0        0        0    10619 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/qpswift_.py
--rw-r--r--   0        0        0     6046 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/quadprog_.py
--rw-r--r--   0        0        0     9904 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/solvers/scs_.py
--rw-r--r--   0        0        0     2808 2023-03-03 15:09:27.367215 qpsolvers-3.3.1/qpsolvers/unsupported/__init__.py
--rw-r--r--   0        0        0     4274 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/unsupported/mosek_.py
--rw-r--r--   0        0        0     6453 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/qpsolvers/unsupported/nppro_.py
--rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.3.1/qpsolvers/utils.py
--rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.3.1/tests/__init__.py
--rw-r--r--   0        0        0     2612 2023-03-28 08:42:54.628660 qpsolvers-3.3.1/tests/problems.py
--rw-r--r--   0        0        0     2214 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_clarabel.py
--rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_conversions.py
--rw-r--r--   0        0        0     3940 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_cvxopt.py
--rw-r--r--   0        0        0     1370 2023-03-31 12:30:36.615914 qpsolvers-3.3.1/tests/test_ecos.py
--rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_gurobi.py
--rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_highs.py
--rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_mosek.py
--rw-r--r--   0        0        0     1348 2023-03-03 11:09:52.362283 qpsolvers-3.3.1/tests/test_nppro.py
--rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_osqp.py
--rw-r--r--   0        0        0     3584 2023-02-28 14:10:40.417483 qpsolvers-3.3.1/tests/test_problem.py
--rw-r--r--   0        0        0     3570 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_proxqp.py
--rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_qpoases.py
--rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_qpswift.py
--rw-r--r--   0        0        0     2332 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_quadprog.py
--rw-r--r--   0        0        0     1695 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_scs.py
--rw-r--r--   0        0        0     2640 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_solution.py
--rw-r--r--   0        0        0     9194 2023-03-28 08:42:54.628660 qpsolvers-3.3.1/tests/test_solve_ls.py
--rw-r--r--   0        0        0    11123 2023-04-11 10:02:56.850101 qpsolvers-3.3.1/tests/test_solve_problem.py
--rw-r--r--   0        0        0    25373 2023-03-31 12:28:59.113529 qpsolvers-3.3.1/tests/test_solve_qp.py
--rw-r--r--   0        0        0     3012 2023-02-28 14:10:40.421483 qpsolvers-3.3.1/tests/test_unfeasible_problem.py
--rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     2426 2023-04-12 09:42:35.095945 qpsolvers-3.3.1/tox.ini
--rw-r--r--   0        0        0    11721 1970-01-01 00:00:00.000000 qpsolvers-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1590 2023-04-28 12:27:28.151337 qpsolvers-3.4.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     2749 2023-04-28 12:27:28.151337 qpsolvers-3.4.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      128 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/.gitignore
+-rw-r--r--   0        0        0    16351 2023-04-28 13:47:55.623443 qpsolvers-3.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1350 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/CITATION.cff
+-rw-r--r--   0        0        0      916 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     7652 2021-03-24 14:54:52.923152 qpsolvers-3.4.0/LICENSE
+-rw-r--r--   0        0        0    10120 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/README.md
+-rw-r--r--   0        0        0     2740 2023-02-23 09:14:02.675958 qpsolvers-3.4.0/benchmark/benchmark_dense_problem.py
+-rw-r--r--   0        0        0     2077 2023-02-23 09:14:02.675958 qpsolvers-3.4.0/benchmark/benchmark_model_predictive_control.py
+-rw-r--r--   0        0        0     3471 2023-02-23 09:14:02.675958 qpsolvers-3.4.0/benchmark/benchmark_random_problems.py
+-rw-r--r--   0        0        0     3017 2023-02-23 09:14:02.675958 qpsolvers-3.4.0/benchmark/benchmark_sparse_problem.py
+-rw-r--r--   0        0        0     9656 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/conf.py
+-rw-r--r--   0        0        0     2924 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/developer-notes.rst
+-rw-r--r--   0        0        0      265 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/environment.yml
+-rw-r--r--   0        0        0      931 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/index.rst
+-rw-r--r--   0        0        0     3707 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/installation.rst
+-rw-r--r--   0        0        0     1006 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/least-squares.rst
+-rw-r--r--   0        0        0     5559 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/quadratic-programming.rst
+-rw-r--r--   0        0        0     2521 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/references.rst
+-rw-r--r--   0        0        0     1037 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/supported-solvers.rst
+-rw-r--r--   0        0        0      400 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/doc/unsupported-solvers.rst
+-rw-r--r--   0        0        0      636 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/README.md
+-rw-r--r--   0        0        0     2030 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/box_inequalities.py
+-rw-r--r--   0        0        0     1601 2023-02-23 09:14:02.683958 qpsolvers-3.4.0/examples/constrained_linear_regression.py
+-rw-r--r--   0        0        0     2790 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/dual_multipliers.py
+-rw-r--r--   0        0        0     1867 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/least_squares.py
+-rw-r--r--   0        0        0     8297 2023-02-23 09:14:02.683958 qpsolvers-3.4.0/examples/model_predictive_control.py
+-rw-r--r--   0        0        0     2045 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/quadratic_program.py
+-rw-r--r--   0        0        0     2049 2023-04-28 12:27:28.155336 qpsolvers-3.4.0/examples/sparse_least_squares.py
+-rw-r--r--   0        0        0     2100 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2299 2023-04-28 13:48:04.315306 qpsolvers-3.4.0/qpsolvers/__init__.py
+-rw-r--r--   0        0        0     1317 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/_internals.py
+-rw-r--r--   0        0        0     1216 2023-02-23 09:14:02.687958 qpsolvers-3.4.0/qpsolvers/conversions/__init__.py
+-rw-r--r--   0        0        0     2317 2023-02-23 09:14:02.687958 qpsolvers-3.4.0/qpsolvers/conversions/ensure_sparse_matrices.py
+-rw-r--r--   0        0        0     3561 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/conversions/linear_from_box_inequalities.py
+-rw-r--r--   0        0        0     3762 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/conversions/socp_from_qp.py
+-rw-r--r--   0        0        0     2284 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/conversions/split_dual_linear_box.py
+-rw-r--r--   0        0        0     1677 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/exceptions.py
+-rw-r--r--   0        0        0     8908 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/problem.py
+-rw-r--r--   0        0        0     6610 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/problems.py
+-rw-r--r--   0        0        0     7849 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solution.py
+-rw-r--r--   0        0        0     7412 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solve_ls.py
+-rw-r--r--   0        0        0     3437 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solve_problem.py
+-rw-r--r--   0        0        0     4698 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solve_qp.py
+-rw-r--r--   0        0        0     1743 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solve_unconstrained.py
+-rw-r--r--   0        0        0    12918 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solvers/__init__.py
+-rw-r--r--   0        0        0     6665 2023-04-28 12:27:28.159336 qpsolvers-3.4.0/qpsolvers/solvers/clarabel_.py
+-rw-r--r--   0        0        0     9200 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/cvxopt_.py
+-rw-r--r--   0        0        0     6441 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/daqp_.py
+-rw-r--r--   0        0        0     8905 2023-04-28 13:47:20.455996 qpsolvers-3.4.0/qpsolvers/solvers/ecos_.py
+-rw-r--r--   0        0        0     7813 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/gurobi_.py
+-rw-r--r--   0        0        0     9571 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/highs_.py
+-rw-r--r--   0        0        0     4336 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/mosek_.py
+-rw-r--r--   0        0        0     9733 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/osqp_.py
+-rw-r--r--   0        0        0     9807 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/proxqp_.py
+-rw-r--r--   0        0        0    13544 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/qpoases_.py
+-rw-r--r--   0        0        0    10619 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/qpswift_.py
+-rw-r--r--   0        0        0     6046 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/quadprog_.py
+-rw-r--r--   0        0        0     9904 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/solvers/scs_.py
+-rw-r--r--   0        0        0     1957 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/unsupported/__init__.py
+-rw-r--r--   0        0        0     6453 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/qpsolvers/unsupported/nppro_.py
+-rw-r--r--   0        0        0     2390 2023-02-28 13:27:49.518364 qpsolvers-3.4.0/qpsolvers/utils.py
+-rw-r--r--   0        0        0       59 2021-04-09 11:14:24.912320 qpsolvers-3.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2612 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/tests/problems.py
+-rw-r--r--   0        0        0     2214 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/tests/test_clarabel.py
+-rw-r--r--   0        0        0     3681 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_conversions.py
+-rw-r--r--   0        0        0     3940 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/tests/test_cvxopt.py
+-rw-r--r--   0        0        0     1780 2023-04-28 13:47:20.455996 qpsolvers-3.4.0/tests/test_ecos.py
+-rw-r--r--   0        0        0     1527 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_gurobi.py
+-rw-r--r--   0        0        0     1773 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_highs.py
+-rw-r--r--   0        0        0     1377 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_mosek.py
+-rw-r--r--   0        0        0     1348 2023-04-28 12:27:28.163336 qpsolvers-3.4.0/tests/test_nppro.py
+-rw-r--r--   0        0        0     1370 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_osqp.py
+-rw-r--r--   0        0        0     3584 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_problem.py
+-rw-r--r--   0        0        0     3570 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_proxqp.py
+-rw-r--r--   0        0        0     3191 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_qpoases.py
+-rw-r--r--   0        0        0     1733 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_qpswift.py
+-rw-r--r--   0        0        0     2332 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_quadprog.py
+-rw-r--r--   0        0        0     1695 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_scs.py
+-rw-r--r--   0        0        0     2912 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_solution.py
+-rw-r--r--   0        0        0    10203 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_solve_ls.py
+-rw-r--r--   0        0        0    11212 2023-04-28 13:47:20.455996 qpsolvers-3.4.0/tests/test_solve_problem.py
+-rw-r--r--   0        0        0    25402 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_solve_qp.py
+-rw-r--r--   0        0        0     3012 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tests/test_unfeasible_problem.py
+-rw-r--r--   0        0        0     1865 2023-02-28 13:41:23.529818 qpsolvers-3.4.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2542 2023-04-28 12:27:28.167336 qpsolvers-3.4.0/tox.ini
+-rw-r--r--   0        0        0    12087 1970-01-01 00:00:00.000000 qpsolvers-3.4.0/PKG-INFO
```

### Comparing `qpsolvers-3.3.1/.github/workflows/docs.yml` & `qpsolvers-3.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/.github/workflows/test.yml` & `qpsolvers-3.4.0/.github/workflows/test.yml`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
                   python -m pip install --upgrade pip
                   python -m pip install tox
 
             - name: "Test with tox for ${{ matrix.os }}"
               run: |
                   tox -e lint
               env:
+                  MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
                   PLATFORM: ubuntu-latest
 
     coverage:
         name: "Coverage"
         runs-on: ubuntu-latest
 
         steps:
@@ -47,14 +48,16 @@
 
             - name: "Install dependencies"
               run: |
                   python -m pip install --upgrade pip
                   python -m pip install coveralls tox
 
             - name: "Check code coverage"
+              env:
+                  MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
               run: |
                   tox -e coverage
 
             - name: "Coveralls"
               env:
                   GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
               run: |
@@ -80,11 +83,12 @@
 
             - name: "Install dependencies"
               run: |
                   python -m pip install --upgrade pip
                   python -m pip install tox tox-gh-actions
 
             - name: "Test with tox for ${{ matrix.os }}"
-              run: |
-                  tox
               env:
+                  MOSEKLM_LICENSE_FILE: ${{ secrets.MSK_LICENSE }}
                   PLATFORM: ${{ matrix.os }}
+              run: |
+                  tox
```

### Comparing `qpsolvers-3.3.1/CHANGELOG.md` & `qpsolvers-3.4.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [3.4.0] - 2023/04/28
+
+### Changed
+
+- Converted THANKS file to [CFF](https://citation-file-format.github.io/)
+- ECOS: raise a ProblemError if inequality vectors contain infinite values
+- ECOS: raise a ProblemError if the cost matrix is not positive definite
+- MOSEK is now a supported solver (thanks to @uricohen and @aszekMosek)
+
+### Fixed
+
+- Residual and duality gap computations when solution is not found
+- Update OSQP version to 0.6.2.post9 for testing
+
 ## [3.3.1] - 2023/04/12
 
 ### Fixed
 
 - DAQP: Update to 0.5.1 to fix installation of arm64 wheels
 
 ## [3.3.0] - 2023/04/11
```

### Comparing `qpsolvers-3.3.1/CONTRIBUTING.md` & `qpsolvers-3.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/LICENSE` & `qpsolvers-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/README.md` & `qpsolvers-3.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# QP Solvers for Python
+# Quadratic Programming Solvers in Python
 
 [![Build](https://img.shields.io/github/actions/workflow/status/qpsolvers/qpsolvers/test.yml?branch=master)](https://github.com/qpsolvers/qpsolvers/actions)
 [![Coverage](https://coveralls.io/repos/github/qpsolvers/qpsolvers/badge.svg?branch=master)](https://coveralls.io/github/qpsolvers/qpsolvers?branch=master)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/qpsolvers/qpsolvers/docs.yml?branch=master&label=docs)](https://qpsolvers.github.io/qpsolvers/)
 [![Downloads/month](https://pepy.tech/badge/qpsolvers/month)](https://pepy.tech/project/qpsolvers)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/qpsolvers.svg)](https://anaconda.org/conda-forge/qpsolvers)
 [![PyPI version](https://img.shields.io/pypi/v/qpsolvers)](https://pypi.org/project/qpsolvers/)
@@ -156,7 +156,13 @@
 <img src="https://scaron.info/images/qp-benchmark-2022.png">
 
 Note that performances of QP solvers largely depend on the problem solved. For instance, MOSEK performs an [automatic conversion to Second-Order Cone Programming (SOCP)](https://docs.mosek.com/8.1/pythonapi/prob-def-quadratic.html) which the documentation advises bypassing for better performance. Similarly, ECOS reformulates [from QP to SOCP](qpsolvers/solvers/conversions/socp_from_qp.py) and [works best on small problems](https://web.stanford.edu/%7Eboyd/papers/ecos.html).
 
 # Contributing
 
 We welcome contributions, see [Contributing](https://github.com/qpsolvers/qpsolvers/blob/master/CONTRIBUTING.md) for details.
+
+We are also looking forward to hearing about your use cases! Please share them in [Show and tell](https://github.com/qpsolvers/qpsolvers/discussions/categories/show-and-tell).
+
+# Citing qpsolvers
+
+If you find this project useful, please consider giving it a :star: and a citation :books: (check out the ``Cite this repository`` button on GitHub).
```

### Comparing `qpsolvers-3.3.1/benchmark/benchmark_dense_problem.py` & `qpsolvers-3.4.0/benchmark/benchmark_dense_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/benchmark/benchmark_model_predictive_control.py` & `qpsolvers-3.4.0/benchmark/benchmark_model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/benchmark/benchmark_random_problems.py` & `qpsolvers-3.4.0/benchmark/benchmark_random_problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/benchmark/benchmark_sparse_problem.py` & `qpsolvers-3.4.0/benchmark/benchmark_sparse_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/conf.py` & `qpsolvers-3.4.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/developer-notes.rst` & `qpsolvers-3.4.0/doc/developer-notes.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/index.rst` & `qpsolvers-3.4.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/installation.rst` & `qpsolvers-3.4.0/doc/installation.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/least-squares.rst` & `qpsolvers-3.4.0/doc/least-squares.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/quadratic-programming.rst` & `qpsolvers-3.4.0/doc/quadratic-programming.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/references.rst` & `qpsolvers-3.4.0/doc/references.rst`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/doc/supported-solvers.rst` & `qpsolvers-3.4.0/doc/supported-solvers.rst`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 
 HiGHS
 =====
 
 .. automodule:: qpsolvers.solvers.highs_
     :members:
 
+MOSEK
+=====
+
+.. automodule:: qpsolvers.solvers.mosek_
+    :members:
+
 OSQP
 ====
 
 .. automodule:: qpsolvers.solvers.osqp_
     :members:
 
 ProxQP
```

### Comparing `qpsolvers-3.3.1/examples/README.md` & `qpsolvers-3.4.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/box_inequalities.py` & `qpsolvers-3.4.0/examples/box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/constrained_linear_regression.py` & `qpsolvers-3.4.0/examples/constrained_linear_regression.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/dual_multipliers.py` & `qpsolvers-3.4.0/examples/dual_multipliers.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/least_squares.py` & `qpsolvers-3.4.0/examples/least_squares.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/model_predictive_control.py` & `qpsolvers-3.4.0/examples/model_predictive_control.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/quadratic_program.py` & `qpsolvers-3.4.0/examples/quadratic_program.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/examples/sparse_least_squares.py` & `qpsolvers-3.4.0/examples/sparse_least_squares.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,64 +22,32 @@
 
 See also: https://stackoverflow.com/a/74415546/3721564
 """
 
 import random
 from time import perf_counter
 
-import numpy as np
-import scipy.sparse as spa
-
 import qpsolvers
 from qpsolvers import solve_ls
-
-n = 150_000
-
-# minimize 1/2 || x - s ||^2
-R = spa.eye(n, format="csc")
-s = np.array(range(n), dtype=float)
-
-# such that G * x <= h
-G = spa.diags(
-    diagonals=[
-        [1.0 if i % 2 == 0 else 0.0 for i in range(n)],
-        [1.0 if i % 3 == 0 else 0.0 for i in range(n - 1)],
-        [1.0 if i % 5 == 0 else 0.0 for i in range(n - 1)],
-    ],
-    offsets=[0, 1, -1],
-    format="csc",
-)
-a_dozen_rows = np.linspace(0, n - 1, 12, dtype=int)
-G = G[a_dozen_rows]
-h = np.ones(12)
-
-# such that sum(x) == 42
-A = spa.csc_matrix(np.ones((1, n)))
-b = np.array([42.0]).reshape((1,))
-
-# such that x >= 0
-lb = np.zeros(n)
-
+from qpsolvers.problems import get_sparse_least_squares
 
 if __name__ == "__main__":
-    solver = (
-        "osqp"
-        if "osqp" in qpsolvers.sparse_solvers
-        else random.choice(qpsolvers.sparse_solvers)
-    )
+    solver = random.choice(qpsolvers.sparse_solvers)
 
+    R, s, G, h, A, b, lb, ub = get_sparse_least_squares(n=150_000)
     start_time = perf_counter()
     x = solve_ls(
         R,
         s,
         G,
         h,
         A,
         b,
         lb,
+        ub,
         solver=solver,
         verbose=False,
         sparse_conversion=True,
     )
     end_time = perf_counter()
     duration_ms = 1e3 * (end_time - start_time)
     tol = 1e-6  # tolerance for checks
```

### Comparing `qpsolvers-3.3.1/pyproject.toml` & `qpsolvers-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/__init__.py` & `qpsolvers-3.4.0/qpsolvers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,26 +37,27 @@
 from .solvers import (
     cvxopt_solve_qp,
     daqp_solve_qp,
     dense_solvers,
     ecos_solve_qp,
     gurobi_solve_qp,
     highs_solve_qp,
+    mosek_solve_qp,
     osqp_solve_qp,
     proxqp_solve_qp,
     qpoases_solve_qp,
     qpswift_solve_qp,
     quadprog_solve_qp,
     scs_solve_qp,
     sparse_solvers,
 )
-from .unsupported import mosek_solve_qp, nppro_solve_qp
+from .unsupported import nppro_solve_qp
 from .utils import print_matrix_vector
 
-__version__ = "3.3.1"
+__version__ = "3.4.0"
 
 __all__ = [
     "NoSolverSelected",
     "ParamError",
     "Problem",
     "ProblemError",
     "QPError",
```

### Comparing `qpsolvers-3.3.1/qpsolvers/_internals.py` & `qpsolvers-3.4.0/qpsolvers/_internals.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/conversions/__init__.py` & `qpsolvers-3.4.0/qpsolvers/conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/conversions/ensure_sparse_matrices.py` & `qpsolvers-3.4.0/qpsolvers/conversions/ensure_sparse_matrices.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/conversions/linear_from_box_inequalities.py` & `qpsolvers-3.4.0/qpsolvers/conversions/linear_from_box_inequalities.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/conversions/socp_from_qp.py` & `qpsolvers-3.4.0/qpsolvers/conversions/socp_from_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/conversions/split_dual_linear_box.py` & `qpsolvers-3.4.0/qpsolvers/conversions/split_dual_linear_box.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/exceptions.py` & `qpsolvers-3.4.0/qpsolvers/exceptions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/problem.py` & `qpsolvers-3.4.0/qpsolvers/problem.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,14 +170,30 @@
         sparse_types = (spa.csc_matrix, spa.dia_matrix)
         return (
             isinstance(self.P, sparse_types)
             or isinstance(self.G, sparse_types)
             or isinstance(self.A, sparse_types)
         )
 
+    @property
+    def is_unconstrained(self) -> bool:
+        """Check whether the problem has any constraint.
+
+        Returns
+        -------
+        :
+            True if the problem has at least one constraint.
+        """
+        return (
+            self.G is None
+            and self.A is None
+            and self.lb is None
+            and self.ub is None
+        )
+
     def unpack(
         self,
     ) -> Tuple[
         Union[np.ndarray, spa.csc_matrix],
         np.ndarray,
         Optional[Union[np.ndarray, spa.csc_matrix]],
         Optional[np.ndarray],
```

### Comparing `qpsolvers-3.3.1/qpsolvers/problems.py` & `qpsolvers-3.4.0/qpsolvers/problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solution.py` & `qpsolvers-3.4.0/qpsolvers/solution.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         Notes
         -----
         See for instance [tolerances]_ for an overview of optimality conditions
         and why this residual will be zero at the optimum.
         """
         _, _, G, h, A, b, lb, ub = self.problem.unpack()
-        if self.x is None:
+        if not self.found or self.x is None:
             return np.inf
         x = self.x
         return max(
             [
                 0.0,
                 np.max(G.dot(x) - h) if G is not None else 0.0,
                 np.linalg.norm(A.dot(x) - b, np.inf) if A is not None else 0.0,
@@ -164,15 +164,15 @@
 
         Notes
         -----
         See for instance [tolerances]_ for an overview of optimality conditions
         and why this residual will be zero at the optimum.
         """
         P, q, G, _, A, _, lb, ub = self.problem.unpack()
-        if self.x is None:
+        if not self.found or self.x is None:
             return np.inf
         zeros = np.zeros(self.x.shape)
         Px = P.dot(self.x)
 
         ATy = zeros
         if A is not None:
             if self.y is None:
@@ -213,15 +213,15 @@
 
         Notes
         -----
         See for instance [tolerances]_ for an overview of optimality conditions
         and why this gap will be zero at the optimum.
         """
         P, q, _, h, _, b, lb, ub = self.problem.unpack()
-        if self.x is None:
+        if not self.found or self.x is None:
             return np.inf
         xPx = self.x.T.dot(P.dot(self.x))
         qx = q.dot(self.x)
 
         hz = 0.0
         if h is not None:
             if self.z is None:
```

### Comparing `qpsolvers-3.3.1/qpsolvers/solve_ls.py` & `qpsolvers-3.4.0/qpsolvers/solve_ls.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solve_problem.py` & `qpsolvers-3.4.0/qpsolvers/solve_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solve_qp.py` & `qpsolvers-3.4.0/qpsolvers/solve_qp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solve_unconstrained.py` & `qpsolvers-3.4.0/qpsolvers/solve_unconstrained.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/__init__.py` & `qpsolvers-3.4.0/qpsolvers/solvers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,26 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
 """Import available QP solvers."""
 
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from numpy import ndarray
 from scipy.sparse import csc_matrix
 
 from ..problem import Problem
 from ..solution import Solution
 
-available_solvers = []
-dense_solvers = []
+available_solvers: List[str] = []
+dense_solvers: List[str] = []
 solve_function: Dict[str, Any] = {}
-sparse_solvers = []
+sparse_solvers: List[str] = []
 
 # Clarabel.rs
 # ===========
 
 clarabel_solve_problem: Optional[
     Callable[
         [
@@ -284,14 +284,56 @@
     solve_function["highs"] = highs_solve_problem
     available_solvers.append("highs")
     sparse_solvers.append("highs")
 except ImportError:
     pass
 
 
+# MOSEK
+# =====
+
+mosek_solve_problem: Optional[
+    Callable[
+        [
+            Problem,
+            Optional[ndarray],
+            bool,
+        ],
+        Solution,
+    ]
+] = None
+
+mosek_solve_qp: Optional[
+    Callable[
+        [
+            Union[ndarray, csc_matrix],
+            ndarray,
+            Union[ndarray, csc_matrix],
+            ndarray,
+            Optional[Union[ndarray, csc_matrix]],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            Optional[ndarray],
+            bool,
+        ],
+        Optional[ndarray],
+    ]
+] = None
+
+try:
+    from .mosek_ import mosek_solve_problem, mosek_solve_qp
+
+    solve_function["mosek"] = mosek_solve_problem
+    available_solvers.append("mosek")
+    sparse_solvers.append("mosek")
+except ImportError:
+    pass
+
+
 # OSQP
 # ====
 
 osqp_solve_problem: Optional[
     Callable[
         [
             Problem,
@@ -559,14 +601,15 @@
     "clarabel_solve_qp",
     "cvxopt_solve_qp",
     "daqp_solve_qp",
     "dense_solvers",
     "ecos_solve_qp",
     "gurobi_solve_qp",
     "highs_solve_qp",
+    "mosek_solve_qp",
     "osqp_solve_qp",
     "proxqp_solve_qp",
     "qpoases_solve_qp",
     "qpswift_solve_qp",
     "quadprog_solve_qp",
     "scs_solve_qp",
     "solve_function",
```

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/clarabel_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/clarabel_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/cvxopt_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/cvxopt_.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 purpose is to make the development of software for convex optimization
 applications straightforward by building on Python’s extensive standard library
 and on the strengths of Python as a high-level programming language. If you are
 using CVXOPT in some academic work, consider citing the corresponding report
 [Vandenberghe2010]_.
 """
 
+import warnings
 from typing import Dict, Optional, Union
 
 import cvxopt
 import numpy as np
 import scipy.sparse as spa
 from cvxopt.solvers import qp
 
@@ -165,14 +166,16 @@
         constraints["G"] = __to_cvxopt(G)
         constraints["h"] = __to_cvxopt(h)
     if A is not None and b is not None:
         constraints["A"] = __to_cvxopt(A)
         constraints["b"] = __to_cvxopt(b)
     initvals_dict: Optional[Dict[str, cvxopt.matrix]] = None
     if initvals is not None:
+        if "mosek" in kwargs:
+            warnings.warn("MOSEK: warm-start values are ignored")
         initvals_dict = {"x": __to_cvxopt(initvals)}
     kwargs["show_progress"] = verbose
 
     try:
         res = qp(
             *args,
             solver=solver,
@@ -185,25 +188,24 @@
         if "Rank(A)" in error:
             raise ProblemError(error) from exception
         raise SolverError(error) from exception
 
     solution = Solution(problem)
     solution.extras = res
     solution.found = "optimal" in res["status"]
-    solution.x = np.array(res["x"]).reshape((q.shape[0],))
+    solution.x = np.array(res["x"]).flatten()
     solution.y = (
-        np.array(res["y"]).reshape((b.shape[0],))
-        if b is not None
-        else np.empty((0,))
+        np.array(res["y"]).flatten() if b is not None else np.empty((0,))
     )
     if h is not None:
-        z_cvx = np.array(res["z"]).reshape((h.shape[0],))
-        z, z_box = split_dual_linear_box(z_cvx, lb, ub)
-        solution.z = z
-        solution.z_box = z_box
+        z_cvxopt = np.array(res["z"]).flatten()
+        if z_cvxopt.size == h.size:
+            z, z_box = split_dual_linear_box(z_cvxopt, lb, ub)
+            solution.z = z
+            solution.z_box = z_box
     else:  # h is None
         solution.z = np.empty((0,))
         solution.z_box = np.empty((0,))
     solution.obj = res["primal objective"]
     return solution
```

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/daqp_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/daqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/ecos_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/ecos_.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 from scipy import sparse as spa
 
 from ..conversions import (
     linear_from_box_inequalities,
     socp_from_qp,
     split_dual_linear_box,
 )
+from ..exceptions import ProblemError
 from ..problem import Problem
 from ..solution import Solution
 
 __exit_flag_meaning__ = {
     0: "OPTIMAL",
     1: "PINF: found certificate of primal infeasibility",
     2: "DING: found certificate of dual infeasibility",
@@ -87,14 +88,23 @@
         Set to `True` to print out extra information.
 
     Returns
     -------
     :
         Solution to the QP, if found, otherwise ``None``.
 
+    Raises
+    ------
+    ProblemError :
+        If inequality constraints contain infinite values that the solver
+        doesn't handle.
+
+    ValueError :
+        If the cost matrix is not positive definite.
+
     Notes
     -----
     All other keyword arguments are forwarded as options to the ECOS solver.
     For instance, you can call ``qpswift_solve_qp(P, q, G, h, abstol=1e-5)``.
 
     For a quick overview, the solver accepts the following settings:
 
@@ -129,30 +139,31 @@
     if initvals is not None:
         warnings.warn("warm-start values are ignored by this wrapper")
     P, q, G, h, A, b, lb, ub = problem.unpack()
     if lb is not None or ub is not None:
         G, h = linear_from_box_inequalities(
             G, h, lb, ub, use_sparse=problem.has_sparse
         )
-    kwargs.update(
-        {
-            "verbose": verbose,
-        }
-    )
+    kwargs.update({"verbose": verbose})
     c_socp, G_socp, h_socp, dims = socp_from_qp(P, q, G, h)
     if A is not None:
         A_socp = spa.hstack([A, spa.csc_matrix((A.shape[0], 1))], format="csc")
         result = solve(c_socp, G_socp, h_socp, dims, A_socp, b, **kwargs)
     else:
         result = solve(c_socp, G_socp, h_socp, dims, **kwargs)
     flag = result["info"]["exitFlag"]
     solution = Solution(problem)
     solution.extras = result["info"]
     solution.found = flag == 0
     if not solution.found:
+        if h is not None and not np.isfinite(h).all():
+            raise ProblemError(
+                "ECOS does not handle infinite values in inequality vectors, "
+                "try clipping them to a finite value suitable to your problem"
+            )
         meaning = __exit_flag_meaning__.get(flag, "unknown exit flag")
         warnings.warn(f"ECOS returned exit flag {flag} ({meaning})")
     solution.x = result["x"][:-1]
     if A is not None:
         solution.y = result["y"]
     if G is not None:
         z_ecos = result["z"][: G.shape[0]]
```

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/gurobi_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/gurobi_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/highs_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/highs_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/osqp_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/osqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/proxqp_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/proxqp_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/qpoases_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/qpoases_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/qpswift_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/qpswift_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/quadprog_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/quadprog_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/solvers/scs_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/scs_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/unsupported/mosek_.py` & `qpsolvers-3.4.0/qpsolvers/solvers/mosek_.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 quadratic, quadratically constraint, conic and convex nonlinear mathematical
 optimization problems. Its interior-point method is geared towards large scale
 sparse problems, in particular for linear or conic quadratic programs.
 """
 
 from typing import Optional, Union
 
-import cvxopt.msk
 import mosek
 import numpy as np
 import scipy.sparse as spa
 
 from ..problem import Problem
 from ..solution import Solution
+from ..solve_unconstrained import solve_unconstrained
 from ..solvers.cvxopt_ import cvxopt_solve_problem
 
 
 def mosek_solve_problem(
     problem: Problem,
     initvals: Optional[np.ndarray] = None,
     verbose: bool = False,
@@ -70,18 +70,20 @@
         Set to `True` to print out extra information.
 
     Returns
     -------
     :
         Solution to the QP, if found, otherwise ``None``.
     """
-    original_options = cvxopt.solvers.options
-    cvxopt.solvers.options["mosek"] = {mosek.iparam.log: 1 if verbose else 0}
+    if problem.is_unconstrained:
+        return solve_unconstrained(problem)
+    if "mosek" not in kwargs:
+        kwargs["mosek"] = {}
+    kwargs["mosek"][mosek.iparam.log] = 1 if verbose else 0
     solution = cvxopt_solve_problem(problem, "mosek", initvals, **kwargs)
-    cvxopt.solvers.options = original_options
     return solution
 
 
 def mosek_solve_qp(
     P: Union[np.ndarray, spa.csc_matrix],
     q: np.ndarray,
     G: Optional[Union[np.ndarray, spa.csc_matrix]] = None,
```

### Comparing `qpsolvers-3.3.1/qpsolvers/unsupported/nppro_.py` & `qpsolvers-3.4.0/qpsolvers/unsupported/nppro_.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/qpsolvers/utils.py` & `qpsolvers-3.4.0/qpsolvers/utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/problems.py` & `qpsolvers-3.4.0/tests/problems.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_clarabel.py` & `qpsolvers-3.4.0/tests/test_clarabel.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_conversions.py` & `qpsolvers-3.4.0/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_cvxopt.py` & `qpsolvers-3.4.0/tests/test_cvxopt.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_ecos.py` & `qpsolvers-3.4.0/tests/test_osqp.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for ECOS."""
+"""Unit tests for OSQP."""
 
 import unittest
 import warnings
 
 from .problems import get_sd3310_problem
 
 try:
-    from qpsolvers.solvers.ecos_ import ecos_solve_qp
+    from qpsolvers.solvers.osqp_ import osqp_solve_qp
 
-    class TestECOS(unittest.TestCase):
-        """Tests specific to ECOS."""
+    class TestOSQP(unittest.TestCase):
+        """Tests specific to OSQP."""
 
         def test_problem(self):
             problem = get_sd3310_problem()
             P, q, G, h, A, b, lb, ub = problem.unpack()
-            self.assertIsNotNone(ecos_solve_qp(P, q, G, h, A, b, lb, ub))
+            self.assertIsNotNone(osqp_solve_qp(P, q, G, h, A, b, lb, ub))
 
 
 except ImportError:  # solver not installed
-    warnings.warn("Skipping ECOS tests as the solver is not installed")
+    warnings.warn("Skipping OSQP tests as the solver is not installed")
```

### Comparing `qpsolvers-3.3.1/tests/test_gurobi.py` & `qpsolvers-3.4.0/tests/test_gurobi.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_highs.py` & `qpsolvers-3.4.0/tests/test_highs.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_mosek.py` & `qpsolvers-3.4.0/tests/test_mosek.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_nppro.py` & `qpsolvers-3.4.0/tests/test_nppro.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_osqp.py` & `qpsolvers-3.4.0/tests/test_ecos.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,28 +14,40 @@
 # WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR
 # A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for OSQP."""
+"""Unit tests for ECOS."""
 
 import unittest
 import warnings
 
+import numpy as np
+
+from qpsolvers.exceptions import ProblemError
+
 from .problems import get_sd3310_problem
 
 try:
-    from qpsolvers.solvers.osqp_ import osqp_solve_qp
+    from qpsolvers.solvers.ecos_ import ecos_solve_qp
 
-    class TestOSQP(unittest.TestCase):
-        """Tests specific to OSQP."""
+    class TestECOS(unittest.TestCase):
+        """Tests specific to ECOS."""
 
         def test_problem(self):
             problem = get_sd3310_problem()
             P, q, G, h, A, b, lb, ub = problem.unpack()
-            self.assertIsNotNone(osqp_solve_qp(P, q, G, h, A, b, lb, ub))
+            self.assertIsNotNone(ecos_solve_qp(P, q, G, h, A, b, lb, ub))
+
+        def test_infinite_inequality(self):
+            problem = get_sd3310_problem()
+            P, q, G, h, A, b, _, _ = problem.unpack()
+            lb = np.array([-1.0, -np.inf, -1.0])
+            ub = np.array([np.inf, 1.0, 1.0])
+            with self.assertRaises(ProblemError):
+                ecos_solve_qp(P, q, G, h, lb=lb, ub=ub)
 
 
 except ImportError:  # solver not installed
-    warnings.warn("Skipping OSQP tests as the solver is not installed")
+    warnings.warn("Skipping ECOS tests as the solver is not installed")
```

### Comparing `qpsolvers-3.3.1/tests/test_problem.py` & `qpsolvers-3.4.0/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_proxqp.py` & `qpsolvers-3.4.0/tests/test_proxqp.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_qpoases.py` & `qpsolvers-3.4.0/tests/test_qpoases.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_qpswift.py` & `qpsolvers-3.4.0/tests/test_qpswift.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_quadprog.py` & `qpsolvers-3.4.0/tests/test_quadprog.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_scs.py` & `qpsolvers-3.4.0/tests/test_scs.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_solution.py` & `qpsolvers-3.4.0/tests/test_solution.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,21 @@
         solution = Solution(get_sd3310_problem())
 
         # solution is fully undefined
         self.assertEqual(solution.primal_residual(), np.inf)
         self.assertEqual(solution.dual_residual(), np.inf)
         self.assertEqual(solution.duality_gap(), np.inf)
 
+        # solution was not found
+        solution.found = False
+        self.assertEqual(solution.primal_residual(), np.inf)
+        self.assertEqual(solution.dual_residual(), np.inf)
+        self.assertEqual(solution.duality_gap(), np.inf)
+
+        solution.found = True
         solution.x = np.array([1.0, 2.0, 3.0])
         self.assertNotEqual(solution.primal_residual(), np.inf)
         self.assertEqual(solution.dual_residual(), np.inf)
         self.assertEqual(solution.duality_gap(), np.inf)
 
         solution.z = np.array([-1.0, -2.0, -3.0])
         self.assertEqual(solution.dual_residual(), np.inf)
```

### Comparing `qpsolvers-3.3.1/tests/test_solve_ls.py` & `qpsolvers-3.4.0/tests/test_solve_ls.py`

 * *Files 11% similar despite different names*

```diff
@@ -178,15 +178,15 @@
             sol_tolerance = 1e-8
             self.assertLess(norm(x_csc - x_dia), sol_tolerance)
             self.assertLess(norm(x_csc - x_np_dia), sol_tolerance)
 
         return test
 
     @staticmethod
-    def get_test_medium_sparse(solver: str, sparse_conversion: bool):
+    def get_test_medium_sparse(solver: str, sparse_conversion: bool, **kwargs):
         """Get test function for a large sparse problem with a given solver.
 
         Parameters
         ----------
         solver :
             Name of the solver to test.
         sparse_conversion :
@@ -195,55 +195,67 @@
         Returns
         -------
         :
             Test function for that solver.
         """
 
         def test(self):
-            R, s, G, h, A, b, lb, ub = get_sparse_least_squares(n=1500)
+            R, s, G, h, A, b, _, _ = get_sparse_least_squares(n=1500)
             x = solve_ls(
                 R,
                 s,
                 G,
                 h,
                 A,
                 b,
                 solver=solver,
                 sparse_conversion=sparse_conversion,
+                **kwargs,
             )
             self.assertIsNotNone(x)
 
         return test
 
     @staticmethod
-    def get_test_large_sparse(solver: str, sparse_conversion: bool):
+    def get_test_large_sparse(
+        solver: str,
+        sparse_conversion: bool,
+        obj_scaling: float = 1.0,
+        **kwargs,
+    ):
         """Get test function for a large sparse problem with a given solver.
 
         Parameters
         ----------
         solver :
             Name of the solver to test.
+        sparse_conversion :
+            Whether to perform sparse or dense LS-to-QP conversion.
+        obj_scaling:
+            Scale objective matrices by this factor. Suitable values can help
+            solvers that don't compute a preconditioner internally.
 
         Returns
         -------
         :
             Test function for that solver.
         """
 
         def test(self):
-            R, s, G, h, A, b, lb, ub = get_sparse_least_squares(n=15_000)
+            R, s, G, h, A, b, _, _ = get_sparse_least_squares(n=15_000)
             x = solve_ls(
-                R,
-                s,
+                obj_scaling * R,
+                obj_scaling * s,
                 G,
                 h,
                 A,
                 b,
                 solver=solver,
                 sparse_conversion=sparse_conversion,
+                **kwargs,
             )
             self.assertIsNotNone(x)
 
         return test
 
 
 # Generate test fixtures for each solver
@@ -255,43 +267,62 @@
     setattr(
         TestSolveLS,
         "test_mixed_sparse_args_{}".format(solver),
         TestSolveLS.get_test_mixed_sparse_args(solver),
     )
     if solver != "gurobi":
         # Gurobi: model too large for size-limited license
+        kwargs = {}
+        if solver == "mosek":
+            try:
+                import mosek
+
+                kwargs["mosek"] = {mosek.dparam.intpnt_qo_tol_rel_gap: 1e-6}
+            except ImportError:
+                pass
         setattr(
             TestSolveLS,
             "test_medium_sparse_dense_conversion_{}".format(solver),
             TestSolveLS.get_test_medium_sparse(
-                solver, sparse_conversion=False
+                solver, sparse_conversion=False, **kwargs
             ),
         )
-        if solver != "cvxopt":
-            # CVXOPT: sparse conversion breaks rank assumption
-            setattr(
-                TestSolveLS,
-                "test_medium_sparse_sparse_conversion_{}".format(solver),
-                TestSolveLS.get_test_medium_sparse(
-                    solver, sparse_conversion=True
-                ),
-            )
-    if solver not in ["gurobi", "highs", "scs"]:
+    if solver not in ["cvxopt", "gurobi"]:
+        # CVXOPT: sparse conversion breaks rank assumption
+        # Gurobi: model too large for size-limited license
+        setattr(
+            TestSolveLS,
+            "test_medium_sparse_sparse_conversion_{}".format(solver),
+            TestSolveLS.get_test_medium_sparse(solver, sparse_conversion=True),
+        )
+    if solver not in ["gurobi", "highs"]:
         # Gurobi: model too large for size-limited license
         # HiGHS: model too large https://github.com/ERGO-Code/HiGHS/issues/992
-        # SCS: issue reported in https://github.com/cvxgrp/scs/issues/234
+        kwargs = {"eps_infeas": 1e-12} if solver == "scs" else {}
+        if solver == "mosek":
+            try:
+                import mosek
+
+                kwargs["mosek"] = {mosek.dparam.intpnt_qo_tol_rel_gap: 1e-7}
+            except ImportError:
+                pass
         setattr(
             TestSolveLS,
             "test_large_sparse_problem_dense_conversion_{}".format(solver),
-            TestSolveLS.get_test_large_sparse(solver, sparse_conversion=False),
+            TestSolveLS.get_test_large_sparse(
+                solver,
+                sparse_conversion=False,
+                obj_scaling=1e-3 if solver == "mosek" else 1.0,
+                **kwargs,
+            ),
         )
         if solver != "cvxopt":
             # CVXOPT: sparse conversion breaks rank assumption
             setattr(
                 TestSolveLS,
                 "test_large_sparse_problem_sparse_conversion_{}".format(
                     solver
                 ),
                 TestSolveLS.get_test_large_sparse(
-                    solver, sparse_conversion=True
+                    solver, sparse_conversion=True, **kwargs
                 ),
             )
```

### Comparing `qpsolvers-3.3.1/tests/test_solve_problem.py` & `qpsolvers-3.4.0/tests/test_solve_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with qpsolvers. If not, see <http://www.gnu.org/licenses/>.
 
 """Unit tests for the `solve_problem` function."""
 
-import math
 import unittest
 
 import numpy as np
 from numpy.linalg import norm
 
 from qpsolvers import available_solvers, solve_problem
 from qpsolvers.problems import (
@@ -111,15 +110,15 @@
                 else 5e-4
                 if solver in ["proxqp", "scs"]
                 else 1e-4
                 if solver == "cvxopt"
                 else 1e-5
                 if solver in ["highs", "osqp"]
                 else 5e-7
-                if solver in ["clarabel", "qpswift"]
+                if solver in ["clarabel", "mosek", "qpswift"]
                 else 1e-7
                 if solver == "gurobi"
                 else 1e-8
             )
             self.assertLess(norm(solution.x - ref_solution.x), eps_abs)
             self.assertLess(solution.primal_residual(), eps_abs)
             self.assertLess(solution.dual_residual(), eps_abs)
@@ -146,17 +145,21 @@
             problem, ref_solution = get_qpsut03()
             solution = solve_problem(problem, solver=solver)
             self.assertEqual(solution.y.shape, (0,))
             self.assertEqual(solution.z.shape, (0,))
             self.assertAlmostEqual(
                 np.linalg.norm(solution.z_box),
                 0.0,
-                places=3 if solver == "cvxopt" else 7,
+                places=3
+                if solver == "cvxopt"
+                else 5
+                if solver == "mosek"
+                else 7,
             )
-            self.assertFalse(math.isnan(solution.duality_gap()))
+            self.assertTrue(np.isfinite(solution.duality_gap()))
 
         return test
 
     @staticmethod
     def get_test_qpsut04(solver: str):
         """
         Get test function for the QPSUT04 problem.
@@ -316,15 +319,15 @@
     )
     setattr(
         TestSolveProblem,
         f"test_qpsut02_{solver}",
         TestSolveProblem.get_test_qpsut02(solver),
     )
     if solver not in ["ecos", "qpswift"]:
-        # ECOS: https://github.com/qpsolvers/qpsolvers/issues/160
+        # ECOS: https://github.com/embotech/ecos-python/issues/49
         # qpSWIFT: https://github.com/qpsolvers/qpsolvers/issues/159
         setattr(
             TestSolveProblem,
             f"test_qpsut03_{solver}",
             TestSolveProblem.get_test_qpsut03(solver),
         )
     setattr(
```

### Comparing `qpsolvers-3.3.1/tests/test_solve_qp.py` & `qpsolvers-3.4.0/tests/test_solve_qp.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                     "ub": ub_case,
                 }
                 for (G_case, h_case) in ineq_variants
                 for (A_case, b_case) in eq_variants
                 for (lb_case, ub_case) in box_variants
             ]
 
-            for (i, test_case) in enumerate(cases):
+            for i, test_case in enumerate(cases):
                 no_inequality = "G" not in test_case or test_case["G"] is None
                 if no_inequality and solver == "qpswift":
                     # QPs without inequality constraints not handled by qpSWIFT
                     continue
                 test_comp = {
                     k: v.shape if v is not None else "None"
                     for k, v in test_case.items()
@@ -499,15 +499,15 @@
                 5e-3
                 if solver == "cvxopt"
                 else 2e-3
                 if solver == "osqp"
                 else 1e-3
                 if solver == "gurobi"
                 else 5e-4
-                if solver == "clarabel"
+                if solver in ["clarabel", "mosek"]
                 else 1e-4
                 if solver == "scs"
                 else 2e-5
                 if solver == "proxqp"
                 else 1e-6
                 if solver == "highs"
                 else 1e-7
@@ -553,15 +553,15 @@
             known_solution = array([2.2] * 149 + [2.4])
             sol_tolerance = (
                 1e-3
                 if solver == "gurobi"
                 else 1e-3
                 if solver == "osqp"
                 else 5e-6
-                if solver == "proxqp"
+                if solver in ["mosek", "proxqp"]
                 else 1e-7
                 if solver in ["cvxopt", "scs"]
                 else 1e-8
             )
             ineq_tolerance = 1e-10
             self.assertLess(norm(x - known_solution), sol_tolerance)
             self.assertLess(max(G * x - h), ineq_tolerance)
@@ -738,15 +738,15 @@
                 2e-3
                 if solver == "osqp"
                 else 5e-4
                 if solver == "scs"
                 else 2e-5
                 if solver == "proxqp"
                 else 1e-6
-                if solver in ["cvxopt", "qpswift"]
+                if solver in ["cvxopt", "mosek", "qpswift"]
                 else 1e-8
             )
             self.assertIsNotNone(x)
             self.assertLess(np.linalg.norm(x - known_solution), sol_tolerance)
 
         return test
```

### Comparing `qpsolvers-3.3.1/tests/test_unfeasible_problem.py` & `qpsolvers-3.4.0/tests/test_unfeasible_problem.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tests/test_utils.py` & `qpsolvers-3.4.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `qpsolvers-3.3.1/tox.ini` & `qpsolvers-3.4.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -12,43 +12,47 @@
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
     macos-latest: macos
     windows-latest: windows
 
 [testenv]
+passenv = MOSEKLM_LICENSE_FILE
 deps =
     clarabel >=0.4.1
     cvxopt >=1.2.6
     daqp >=0.5.1
     ecos >=2.0.8
     gurobipy >=9.5.2
-    numpy <1.24.0
-    osqp >=0.6.2
+    mosek >=10.0.40
+    numpy >=1.15.4
+    osqp >=0.6.2.post9
     quadprog >=0.1.11
     scipy >=1.2.0
     scs >=3.2.0
 
     !windows: highspy >=1.1.2.dev3
     py38-{linux,macos}: proxsuite >=0.2.9
     py{39,310}-linux: proxsuite >=0.2.9
 commands =
     python -m unittest discover
 
 [testenv:coverage]
+passenv = MOSEKLM_LICENSE_FILE
 deps =
     clarabel >=0.4.1
     coverage >=5.5
     cvxopt >=1.2.6
     daqp >=0.5.1
     ecos >=2.0.8
     gurobipy >=9.5.2
+    mosek >=10.0.40
     highspy >=1.1.2.dev3
-    numpy <1.24.0
-    osqp >=0.6.2
+    numpy >=1.15.4
+    osqp >=0.6.2.post9
     proxsuite >=0.3.1
     quadprog >=0.1.11
     scipy >=1.2.0
     scs >=3.2.0
 commands =
     coverage erase
     coverage run -m unittest discover
```

### Comparing `qpsolvers-3.3.1/PKG-INFO` & `qpsolvers-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpsolvers
-Version: 3.3.1
+Version: 3.4.0
 Summary: Quadratic programming solvers in Python with a unified API.
 Keywords: quadratic programming,solver,numerical optimization
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 Requires-Dist: scs >=3.2.0 ; extra == "open_source_solvers"
 Project-URL: Changelog, https://github.com/qpsolvers/qpsolvers/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://qpsolvers.github.io/qpsolvers/
 Project-URL: Source, https://github.com/qpsolvers/qpsolvers
 Project-URL: Tracker, https://github.com/qpsolvers/qpsolvers/issues
 Provides-Extra: open_source_solvers
 
-# QP Solvers for Python
+# Quadratic Programming Solvers in Python
 
 [![Build](https://img.shields.io/github/actions/workflow/status/qpsolvers/qpsolvers/test.yml?branch=master)](https://github.com/qpsolvers/qpsolvers/actions)
 [![Coverage](https://coveralls.io/repos/github/qpsolvers/qpsolvers/badge.svg?branch=master)](https://coveralls.io/github/qpsolvers/qpsolvers?branch=master)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/qpsolvers/qpsolvers/docs.yml?branch=master&label=docs)](https://qpsolvers.github.io/qpsolvers/)
 [![Downloads/month](https://pepy.tech/badge/qpsolvers/month)](https://pepy.tech/project/qpsolvers)
 [![Conda version](https://img.shields.io/conda/vn/conda-forge/qpsolvers.svg)](https://anaconda.org/conda-forge/qpsolvers)
 [![PyPI version](https://img.shields.io/pypi/v/qpsolvers)](https://pypi.org/project/qpsolvers/)
@@ -197,7 +197,13 @@
 
 Note that performances of QP solvers largely depend on the problem solved. For instance, MOSEK performs an [automatic conversion to Second-Order Cone Programming (SOCP)](https://docs.mosek.com/8.1/pythonapi/prob-def-quadratic.html) which the documentation advises bypassing for better performance. Similarly, ECOS reformulates [from QP to SOCP](qpsolvers/solvers/conversions/socp_from_qp.py) and [works best on small problems](https://web.stanford.edu/%7Eboyd/papers/ecos.html).
 
 # Contributing
 
 We welcome contributions, see [Contributing](https://github.com/qpsolvers/qpsolvers/blob/master/CONTRIBUTING.md) for details.
 
+We are also looking forward to hearing about your use cases! Please share them in [Show and tell](https://github.com/qpsolvers/qpsolvers/discussions/categories/show-and-tell).
+
+# Citing qpsolvers
+
+If you find this project useful, please consider giving it a :star: and a citation :books: (check out the ``Cite this repository`` button on GitHub).
+
```

