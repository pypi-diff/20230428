# Comparing `tmp/concordia-harmony-0.1.3.tar.gz` & `tmp/concordia-harmony-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "concordia-harmony-0.1.3.tar", last modified: Wed Apr 26 04:46:25 2023, max compression
+gzip compressed data, was "concordia-harmony-0.1.4.tar", last modified: Fri Apr 28 01:51:32 2023, max compression
```

## Comparing `concordia-harmony-0.1.3.tar` & `concordia-harmony-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/src/concordia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/src/concordia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/src/concordia/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/src/concordia/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 04:46:16.000000 concordia-harmony-0.1.3/src/concordia/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 04:46:25.389396 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-26 04:46:25.000000 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-26 04:46:25.000000 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 04:46:25.000000 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-26 04:46:25.000000 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 04:46:25.000000 concordia-harmony-0.1.3/src/concordia_harmony.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:51:32.259542 concordia-harmony-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 01:51:32.259542 concordia-harmony-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 01:51:32.263542 concordia-harmony-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:51:32.259542 concordia-harmony-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:51:32.259542 concordia-harmony-0.1.4/src/concordia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/src/concordia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/src/concordia/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/src/concordia/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 01:51:17.000000 concordia-harmony-0.1.4/src/concordia/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 01:51:32.259542 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-04-28 01:51:32.000000 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-28 01:51:32.000000 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 01:51:32.000000 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 01:51:32.000000 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 01:51:32.000000 concordia-harmony-0.1.4/src/concordia_harmony.egg-info/top_level.txt
```

### Comparing `concordia-harmony-0.1.3/LICENSE` & `concordia-harmony-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `concordia-harmony-0.1.3/src/concordia/library.py` & `concordia-harmony-0.1.4/src/concordia/library.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,51 +7,72 @@
 # 0-11?
 PitchClassVarRef = z3.ArithRef
 PitchClassValue = int
 
 
 @dataclass
 class PitchVarRef:
+    """
+    A class representing a pitch variable.
+    """
+
     midi: PitchMidiVarRef
     pitchClass: PitchClassVarRef
 
 
 @dataclass
 class ChordVarRef:
+    """
+    A class representing a chord variable.
+    """
+
     pitches: list[PitchVarRef]
 
     def soprano(self):
+        """Gets the soprano pitch variable."""
         return self.pitches[0]
 
     def alto(self):
+        """Gets the alto pitch variable."""
         return self.pitches[1]
 
     def tenor(self):
+        """Gets the tenor pitch variable."""
         return self.pitches[2]
 
     def bass(self):
+        """Gets the bass pitch variable."""
         return self.pitches[3]
 
 
 @dataclass
 class StreamVarRef:
+    """
+    A class representing a note stream (voice/part) variable.
+    """
+
     pitches: list[PitchVarRef]
 
 
 def PitchVar(name: str) -> PitchVarRef:
+    """Creates a pitch variable."""
     return PitchVarRef(z3.Int(f"{name}.pitchMidi"), z3.Int(f"{name}.pitchClass"))
 
 
 def PitchMidiVar(name: str) -> PitchMidiVarRef:
+    """Creates a pitch midi variable."""
     return z3.Int(f"{name}.pitchMidi")
 
 
 def PitchClassVar(name: str) -> PitchClassVarRef:
+    """Creates a pitch class variable."""
     return z3.Int(f"{name}.pitchClass")
 
 
 def StreamVar(var_names: list[str]) -> StreamVarRef:
+    """Creates a note stream (part/voice) variable."""
     return StreamVarRef([PitchVar(name) for name in var_names])
 
 
 def ChordVar(var_names: list[str]) -> ChordVarRef:
+    """Creates a chord variable."""
     return ChordVarRef([PitchVar(name) for name in var_names])
```

### Comparing `concordia-harmony-0.1.3/src/concordia/solver.py` & `concordia-harmony-0.1.4/src/concordia/solver.py`

 * *Files identical despite different names*

