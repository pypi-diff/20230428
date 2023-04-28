# Comparing `tmp/pomodoro_timer_cli-0.1.5.tar.gz` & `tmp/pomodoro_timer_cli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomodoro_timer_cli-0.1.5.tar", max compression
+gzip compressed data, was "pomodoro_timer_cli-0.1.6.tar", max compression
```

## Comparing `pomodoro_timer_cli-0.1.5.tar` & `pomodoro_timer_cli-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.5/LICENSE
--rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/__init__.py
--rw-r--r--   0        0        0       72 2023-04-28 13:24:37.422680 pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/__main__.py
--rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/complete.wav
--rw-r--r--   0        0        0     1464 2023-04-28 13:13:41.370367 pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/pomodoro.py
--rw-r--r--   0        0        0      418 2023-04-28 13:27:11.407974 pomodoro_timer_cli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.6/LICENSE
+-rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/__init__.py
+-rw-r--r--   0        0        0       62 2023-04-28 13:38:11.153925 pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/__main__.py
+-rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/complete.wav
+-rw-r--r--   0        0        0     1464 2023-04-28 13:13:41.370367 pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/pomodoro.py
+-rw-r--r--   0        0        0      418 2023-04-28 13:38:43.702000 pomodoro_timer_cli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.6/PKG-INFO
```

### Comparing `pomodoro_timer_cli-0.1.5/LICENSE` & `pomodoro_timer_cli-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/complete.wav` & `pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/complete.wav`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.5/pomodoro_timer_cli/pomodoro.py` & `pomodoro_timer_cli-0.1.6/pomodoro_timer_cli/pomodoro.py`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.5/PKG-INFO` & `pomodoro_timer_cli-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomodoro-timer-cli
-Version: 0.1.5
+Version: 0.1.6
 Summary: A simple CLI-based tomato timer.
 License: MIT
 Author: hungtsetse
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

