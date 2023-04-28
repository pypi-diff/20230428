# Comparing `tmp/pomodoro_timer_cli-0.1.9.tar.gz` & `tmp/pomodoro_timer_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomodoro_timer_cli-0.1.9.tar", max compression
+gzip compressed data, was "pomodoro_timer_cli-0.2.0.tar", max compression
```

## Comparing `pomodoro_timer_cli-0.1.9.tar` & `pomodoro_timer_cli-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.9/LICENSE
--rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/__init__.py
--rw-r--r--   0        0        0       63 2023-04-28 13:41:11.231621 pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/__main__.py
--rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/complete.wav
--rw-r--r--   0        0        0     1464 2023-04-28 14:07:05.409344 pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/pomodoro.py
--rw-r--r--   0        0        0      422 2023-04-28 14:17:16.861497 pomodoro_timer_cli-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      175 2023-04-28 14:24:50.658301 pomodoro_timer_cli-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-28 13:41:11.231621 pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/__main__.py
+-rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/complete.wav
+-rw-r--r--   0        0        0     1464 2023-04-28 14:07:05.409344 pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/pomodoro.py
+-rw-r--r--   0        0        0      422 2023-04-28 14:25:01.096166 pomodoro_timer_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      648 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.2.0/PKG-INFO
```

### Comparing `pomodoro_timer_cli-0.1.9/LICENSE` & `pomodoro_timer_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/complete.wav` & `pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/complete.wav`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.9/pomodoro_timer_cli/pomodoro.py` & `pomodoro_timer_cli-0.2.0/pomodoro_timer_cli/pomodoro.py`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.9/PKG-INFO` & `pomodoro_timer_cli-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomodoro-timer-cli
-Version: 0.1.9
+Version: 0.2.0
 Summary: A simple CLI-based tomato timer.
 License: MIT
 Author: hungtsetse
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 
 # pomodoro-timer-cli
 A simple CLI-based tomato timer.
 
 ## Installation
 ```bash
-pipx install pomodoro-timer-cli
+pip install pomodoro-timer-cli
 ```
 
 ## Example
 ```bash
 pomodoro
 ```
 ```bash
```

