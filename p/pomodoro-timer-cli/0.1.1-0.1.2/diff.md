# Comparing `tmp/pomodoro_timer_cli-0.1.1.tar.gz` & `tmp/pomodoro_timer_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomodoro_timer_cli-0.1.1.tar", max compression
+gzip compressed data, was "pomodoro_timer_cli-0.1.2.tar", max compression
```

## Comparing `pomodoro_timer_cli-0.1.1.tar` & `pomodoro_timer_cli-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.1/pomodoro_timer_cli/__init__.py
--rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.1/pomodoro_timer_cli/complete.wav
--rw-r--r--   0        0        0     1435 2023-04-28 12:03:10.210505 pomodoro_timer_cli-0.1.1/pomodoro_timer_cli/pomodoro.py
--rw-r--r--   0        0        0      449 2023-04-28 12:52:47.700738 pomodoro_timer_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      738 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-27 08:54:49.988536 pomodoro_timer_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0      176 2023-04-28 12:22:16.971706 pomodoro_timer_cli-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-28 12:22:04.751249 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/__init__.py
+-rw-r--r--   0        0        0   434512 2023-04-24 05:10:50.831129 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/complete.wav
+-rw-r--r--   0        0        0     1464 2023-04-28 13:08:53.445207 pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/pomodoro.py
+-rw-r--r--   0        0        0      465 2023-04-28 13:09:54.068159 pomodoro_timer_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 pomodoro_timer_cli-0.1.2/PKG-INFO
```

### Comparing `pomodoro_timer_cli-0.1.1/LICENSE` & `pomodoro_timer_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.1/pomodoro_timer_cli/complete.wav` & `pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/complete.wav`

 * *Files identical despite different names*

### Comparing `pomodoro_timer_cli-0.1.1/pomodoro_timer_cli/pomodoro.py` & `pomodoro_timer_cli-0.1.2/pomodoro_timer_cli/pomodoro.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def play_sound_effect():
     duration = miniaudio.wav_get_file_info("complete.wav").duration
     stream = miniaudio.stream_file("complete.wav")
     with miniaudio.PlaybackDevice() as device:
         device.start(stream)
         time.sleep(duration)
 
-def main(
+def pomodoro(
     pomodoro: int = typer.Option(4, "--pomodoro", "-p", help="Numbers of pomodoros"),
     focus_min: int = typer.Option(25, "--focus", "-f", help="Numbers of minutes for focus"),
     break_min: int = typer.Option(5, "--break", "-b", help="Numbers of minutes for break"),
 ):
     with Progress(SpinnerColumn(),TextColumn("[progress.description]{task.description}"),BarColumn(),TimeElapsedColumn()) as progress:
         for ith in range(1, pomodoro+1):
             focus = progress.add_task(f"{ith}. Focus", total=60*focus_min)
@@ -27,10 +27,12 @@
             _break = progress.add_task(f"{ith}. Break", total=60*break_min)
             while not progress.finished:
                 time.sleep(1)
                 progress.update(_break, advance=1)
             play_sound_effect()
     print("WELL DONE! Take a long break. :party_popper:")
 
+def cli():
+    typer.run(pomodoro)
 
 if __name__ == "__main__":
-    typer.run(main)
+    cli()
```

### Comparing `pomodoro_timer_cli-0.1.1/PKG-INFO` & `pomodoro_timer_cli-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: pomodoro-timer-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple CLI-based tomato timer.
 License: MIT
 Author: hungtsetse
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: markdown-it-py (>=2.2.0,<3.0.0)
 Requires-Dist: miniaudio (>=1.56,<2.0)
-Requires-Dist: pygments (>=2.15.1,<3.0.0)
 Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # pomodoro-timer-cli
 A simple CLI-based tomato timer.
```

