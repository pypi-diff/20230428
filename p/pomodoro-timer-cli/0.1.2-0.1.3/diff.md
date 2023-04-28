# Comparing `tmp/pomodoro_timer_cli-0.1.2.tar.gz` & `tmp/pomodoro_timer_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomodoro_timer_cli-0.1.2.tar", max compression
+gzip compressed data, was "pomodoro_timer_cli-0.1.3.tar", max compression
```

## Comparing `pomodoro_timer_cli-0.1.2.tar` & `pomodoro_timer_cli-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/__init__.py
--rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/complete.wav
--rw-r--r--   0        0        0     1464 2023-04-28 13:08:53.445207 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/pomodoro.py
--rw-r--r--   0        0        0      465 2023-04-28 13:09:54.068159 pomodoro_timer_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.3/LICENSE
+-rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.3/pomodoro_timer_cli/__init__.py
+-rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.3/pomodoro_timer_cli/complete.wav
+-rw-r--r--   0        0        0     1464 2023-04-28 13:13:41.370367 pomodoro_timer_cli-0.1.3/pomodoro_timer_cli/pomodoro.py
+-rw-r--r--   0        0        0      418 2023-04-28 13:14:22.751885 pomodoro_timer_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.3/PKG-INFO
```

### Comparing `pomodoro_timer_cli-0.1.2/LICENSE` & `pomodoro_timer_cli-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/complete.wav` & `pomodoro_timer_cli-0.1.3/pomodoro_timer_cli/complete.wav`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/pomodoro.py` & `pomodoro_timer_cli-0.1.3/pomodoro_timer_cli/pomodoro.py`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.2/PKG-INFO` & `pomodoro_timer_cli-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomodoro-timer-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple CLI-based tomato timer.
 License: MIT
 Author: hungtsetse
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

