# Comparing `tmp/mathlib-0.4.0.tar.gz` & `tmp/mathlib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathlib-0.4.0.tar", max compression
+gzip compressed data, was "mathlib-0.5.0.tar", max compression
```

## Comparing `mathlib-0.4.0.tar` & `mathlib-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     7652 2021-04-14 15:32:01.444100 mathlib-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1535 2022-01-10 16:13:26.870159 mathlib-0.4.0/README.rst
--rw-r--r--   0        0        0     1553 2022-01-10 16:13:03.194050 mathlib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-04-14 15:32:01.444100 mathlib-0.4.0/src/mathlib/__init__.py
--rw-r--r--   0        0        0     1348 2021-10-21 16:46:32.855689 mathlib-0.4.0/src/mathlib/_seven.py
--rw-r--r--   0        0        0      188 2021-10-21 19:36:34.568402 mathlib-0.4.0/src/mathlib/_seven.pyi
--rw-r--r--   0        0        0     2517 2021-10-21 15:19:40.184281 mathlib-0.4.0/src/mathlib/numbers.py
--rw-r--r--   0        0        0     4104 2021-06-12 08:24:53.185451 mathlib-0.4.0/src/mathlib/primes.py
--rw-r--r--   0        0        0        0 2021-04-14 15:32:01.444100 mathlib-0.4.0/src/mathlib/py.typed
--rw-r--r--   0        0        0     2206 2022-01-10 16:15:14.521807 mathlib-0.4.0/setup.py
--rw-r--r--   0        0        0     2485 2022-01-10 16:15:14.522004 mathlib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:26.109182 mathlib-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1728 2023-04-28 15:36:49.070805 mathlib-0.5.0/README.rst
+-rw-r--r--   0        0        0     2763 2023-04-28 15:36:49.071511 mathlib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:26.109932 mathlib-0.5.0/src/mathlib/__init__.py
+-rw-r--r--   0        0        0      443 2023-03-07 22:01:49.666318 mathlib-0.5.0/src/mathlib/_seven.py
+-rw-r--r--   0        0        0       72 2023-04-28 15:05:39.227064 mathlib-0.5.0/src/mathlib/_seven.pyi
+-rw-r--r--   0        0        0      725 2023-04-28 15:36:48.805009 mathlib-0.5.0/src/mathlib/general.py
+-rw-r--r--   0        0        0     3473 2023-03-08 22:03:30.962095 mathlib-0.5.0/src/mathlib/numbers.py
+-rw-r--r--   0        0        0     4782 2023-03-08 10:49:53.745689 mathlib-0.5.0/src/mathlib/primes.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:26.110240 mathlib-0.5.0/src/mathlib/py.typed
+-rw-r--r--   0        0        0     2751 1970-01-01 00:00:00.000000 mathlib-0.5.0/PKG-INFO
```

### Comparing `mathlib-0.4.0/LICENSE.txt` & `mathlib-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mathlib-0.4.0/README.rst` & `mathlib-0.5.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 ====================================
 mathlib: a pure python maths library
 ====================================
 
-.. image:: https://github.com/spapanik/mathlib/actions/workflows/build.yml/badge.svg
-  :alt: Build
-  :target: https://github.com/spapanik/mathlib/actions/workflows/build.yml
-.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/mathlib.svg
-  :alt: Total alerts
-  :target: https://lgtm.com/projects/g/spapanik/mathlib/alerts/
+.. image:: https://github.com/spapanik/mathlib/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/mathlib/actions/workflows/tests.yml
 .. image:: https://img.shields.io/github/license/spapanik/mathlib
   :alt: License
   :target: https://github.com/spapanik/mathlib/blob/main/LICENSE.txt
 .. image:: https://img.shields.io/pypi/v/mathlib
   :alt: PyPI
   :target: https://pypi.org/project/mathlib
 .. image:: https://pepy.tech/badge/mathlib
   :alt: Downloads
   :target: https://pepy.tech/project/mathlib
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: Code style
+  :alt: code style: black
   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
 
 ``mathlib`` is a maths library written in pure python, so that it can be used
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `poetry`_ to manage your dependencies and add *mathlib* to them.
 
 .. code-block:: toml
 
     [tool.poetry.dependencies]
-    mathlib = "^0.4.0"
+    mathlib = "^0.5.0"
 
 Usage
 ^^^^^
 
 ``mathlib`` mainly offers some number theoretic functions.
```

### Comparing `mathlib-0.4.0/src/mathlib/primes.py` & `mathlib-0.5.0/src/mathlib/primes.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,67 @@
 import math
 from itertools import chain, count
-from typing import Iterable, Iterator
+from typing import Iterator
+
+SMALL_PRIMES = {
+    2,
+    3,
+    5,
+    7,
+    11,
+    13,
+    17,
+    19,
+    23,
+    29,
+    31,
+    37,
+    41,
+    43,
+    47,
+    53,
+    59,
+    61,
+    67,
+    71,
+    73,
+    79,
+    83,
+    89,
+    97,
+    101,
+    103,
+    107,
+    109,
+    113,
+    127,
+    131,
+    137,
+    139,
+    149,
+    151,
+    157,
+    163,
+    167,
+    173,
+    179,
+    181,
+    191,
+    193,
+    197,
+    199,
+    211,
+    223,
+    227,
+    229,
+    233,
+    239,
+    241,
+    251,
+}
 
 
 class UnreachableError(Exception):
     """
     Make mypy happy; this part of the code is unreachable
     """
 
@@ -42,72 +99,80 @@
             yield 2 * i + 3
 
 
 def _miller_rabin_loop(witness: int, mantissa: int, power: int, n: int) -> bool:
     if pow(witness, mantissa, n) == 1:
         return False
 
-    for r in range(power):
-        if pow(witness, mantissa * (1 << r), n) + 1 == n:
-            return False
+    return all(pow(witness, mantissa * (1 << r), n) + 1 != n for r in range(power))
 
-    return True
 
-
-def _miller_rabin_witnesses(n: int) -> Iterable[int]:
+def _miller_rabin_witnesses(n: int) -> Iterator[int]:
     if n < 2047:
-        return (2,)
+        yield from [2]
+        return
 
     if n < 1373653:
-        return 2, 3
+        yield from [2, 3]
+        return
 
     if n < 9080191:
-        return 31, 73
+        yield from [31, 73]
+        return
 
     if n < 25326001:
-        return 2, 3, 5
+        yield from [2, 3, 5]
+        return
 
     if n < 4759123141:
-        return 2, 7, 61
+        yield from [2, 7, 61]
+        return
 
     if n < 1122004669633:
-        return 2, 13, 23, 1662803
+        yield from [2, 13, 23, 1662803]
+        return
 
     if n < 2152302898747:
-        return 2, 3, 5, 7, 11
+        yield from [2, 3, 5, 7, 11]
+        return
 
     if n < 3474749660383:
-        return 2, 3, 5, 7, 11, 13
+        yield from [2, 3, 5, 7, 11, 13]
+        return
 
     if n < 341550071728321:
-        return 2, 3, 5, 7, 11, 13, 17
+        yield from [2, 3, 5, 7, 11, 13, 17]
+        return
 
     if n < 3825123056546413051:
-        return 2, 3, 5, 7, 11, 13, 17, 19, 23
+        yield from [2, 3, 5, 7, 11, 13, 17, 19, 23]
+        return
 
     if n < 318665857834031151167461:
-        return 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37
+        yield from [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37]
+        return
 
     if n < 3317044064679887385961981:
-        return 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41
+        yield from [2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41]
+        return
 
-    return range(2, math.floor(2 * (math.log(n) ** 2)) + 1)
+    yield from sieve(math.floor(2 * (math.log(n) ** 2)) + 1)
 
 
 def is_prime(n: int) -> bool:
     """
     Check if n is a prime number.
 
     This is a deterministic primality test, but it relies on GHR. This
     seems a good enough compromise. It is very fast for up to 81-bit
     integers, after which it is starts slowing down, due to the fact
     that we need to check for all possible Miller-Rabin witnesses.
     """
-    if n < 5:
-        return n in (2, 3)
+    if n < 256:
+        return n in SMALL_PRIMES
 
     if n % 2 == 0:
         return False
 
     mantissa, power = n - 1, 0
     while mantissa & 1 == 0:
         mantissa >>= 1
@@ -131,17 +196,17 @@
         return 3
 
     if n & 1 == 1:
         n += 2
     else:
         n += 1
 
-    for n in count(n, 2):
-        if is_prime(n):
-            return n
+    for p in count(n, 2):
+        if is_prime(p):
+            return p
 
     raise UnreachableError("A prime will be reached")
 
 
 def primes() -> Iterator[int]:
     """
     Make an iterator that returns the prime numbers in ascending order.
@@ -163,14 +228,14 @@
         while n % prime_div == 0:
             power += 1
             n //= prime_div
         if power != 1:
             if x == 0:
                 out *= power
             elif x == 1:
-                out *= (prime_div ** power - 1) // (prime_div - 1)
+                out *= (prime_div**power - 1) // (prime_div - 1)
             else:
-                out *= (prime_div ** (x * power) - 1) // (prime_div ** x - 1)
+                out *= (prime_div ** (x * power) - 1) // (prime_div**x - 1)
             if n == 1:
                 return out
 
     raise UnreachableError("At some point divisors will be exhausted")
```

### Comparing `mathlib-0.4.0/PKG-INFO` & `mathlib-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 Metadata-Version: 2.1
 Name: mathlib
-Version: 0.4.0
+Version: 0.5.0
 Summary: A pure-python maths library
-Home-page: https://github.com/spapanik/mathlib
+Home-page: https://mathlib.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: mathematics
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Project-URL: Documentation, https://mathlib.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/mathlib
 Description-Content-Type: text/x-rst
 
 ====================================
 mathlib: a pure python maths library
 ====================================
 
-.. image:: https://github.com/spapanik/mathlib/actions/workflows/build.yml/badge.svg
-  :alt: Build
-  :target: https://github.com/spapanik/mathlib/actions/workflows/build.yml
-.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/mathlib.svg
-  :alt: Total alerts
-  :target: https://lgtm.com/projects/g/spapanik/mathlib/alerts/
+.. image:: https://github.com/spapanik/mathlib/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/mathlib/actions/workflows/tests.yml
 .. image:: https://img.shields.io/github/license/spapanik/mathlib
   :alt: License
   :target: https://github.com/spapanik/mathlib/blob/main/LICENSE.txt
 .. image:: https://img.shields.io/pypi/v/mathlib
   :alt: PyPI
   :target: https://pypi.org/project/mathlib
 .. image:: https://pepy.tech/badge/mathlib
   :alt: Downloads
   :target: https://pepy.tech/project/mathlib
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: Code style
+  :alt: code style: black
   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
 
 ``mathlib`` is a maths library written in pure python, so that it can be used
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `poetry`_ to manage your dependencies and add *mathlib* to them.
 
 .. code-block:: toml
 
     [tool.poetry.dependencies]
-    mathlib = "^0.4.0"
+    mathlib = "^0.5.0"
 
 Usage
 ^^^^^
 
 ``mathlib`` mainly offers some number theoretic functions.
```

