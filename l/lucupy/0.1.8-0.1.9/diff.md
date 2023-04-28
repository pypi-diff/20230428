# Comparing `tmp/lucupy-0.1.8.tar.gz` & `tmp/lucupy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lucupy-0.1.8.tar", max compression
+gzip compressed data, was "lucupy-0.1.9.tar", max compression
```

## Comparing `lucupy-0.1.8.tar` & `lucupy-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1528 2022-10-17 17:24:45.820558 lucupy-0.1.8/LICENSE
--rw-r--r--   0        0        0     1006 2022-10-17 17:24:45.820882 lucupy-0.1.8/README.rst
--rw-r--r--   0        0        0     1026 2022-10-17 17:24:45.821333 lucupy-0.1.8/lucupy/__init__.py
--rw-r--r--   0        0        0      734 2022-10-17 17:24:45.821567 lucupy-0.1.8/lucupy/decorators/__init__.py
--rw-r--r--   0        0        0     7408 2022-10-17 17:24:45.821843 lucupy-0.1.8/lucupy/helpers/__init__.py
--rw-r--r--   0        0        0      636 2022-10-17 17:24:45.822222 lucupy-0.1.8/lucupy/minimodel/__init__.py
--rw-r--r--   0        0        0     1309 2022-10-17 17:24:45.822493 lucupy-0.1.8/lucupy/minimodel/atom.py
--rw-r--r--   0        0        0     8328 2022-10-17 17:24:45.822840 lucupy-0.1.8/lucupy/minimodel/constraints.py
--rw-r--r--   0        0        0     9187 2022-10-31 09:30:18.363574 lucupy-0.1.8/lucupy/minimodel/group.py
--rw-r--r--   0        0        0     2766 2022-10-17 17:24:45.823700 lucupy-0.1.8/lucupy/minimodel/magnitude.py
--rw-r--r--   0        0        0    10031 2022-10-31 09:29:06.698972 lucupy-0.1.8/lucupy/minimodel/observation.py
--rw-r--r--   0        0        0      974 2022-10-17 17:24:45.824269 lucupy-0.1.8/lucupy/minimodel/observationmode.py
--rw-r--r--   0        0        0     4704 2022-10-31 09:14:49.262276 lucupy-0.1.8/lucupy/minimodel/program.py
--rw-r--r--   0        0        0      780 2022-10-17 17:24:45.824744 lucupy-0.1.8/lucupy/minimodel/qastate.py
--rw-r--r--   0        0        0     1055 2022-10-17 17:24:45.825010 lucupy-0.1.8/lucupy/minimodel/resource.py
--rw-r--r--   0        0        0      914 2022-10-17 17:24:45.825413 lucupy-0.1.8/lucupy/minimodel/semester.py
--rw-r--r--   0        0        0     1562 2022-10-17 17:24:45.825817 lucupy-0.1.8/lucupy/minimodel/site.py
--rw-r--r--   0        0        0     2878 2022-10-17 17:24:45.826095 lucupy-0.1.8/lucupy/minimodel/target.py
--rw-r--r--   0        0        0     2135 2022-10-17 17:24:45.826341 lucupy-0.1.8/lucupy/minimodel/timeallocation.py
--rw-r--r--   0        0        0     1364 2022-10-17 17:24:45.826580 lucupy-0.1.8/lucupy/minimodel/timingwindow.py
--rw-r--r--   0        0        0      844 2022-10-17 17:24:45.826826 lucupy-0.1.8/lucupy/minimodel/too.py
--rw-r--r--   0        0        0      244 2022-10-17 17:24:45.826986 lucupy-0.1.8/lucupy/observatory/__init__.py
--rw-r--r--   0        0        0     3262 2022-10-20 01:15:57.052740 lucupy-0.1.8/lucupy/observatory/abstract/__init__.py
--rw-r--r--   0        0        0      245 2022-10-06 01:52:10.238720 lucupy-0.1.8/lucupy/observatory/gemini/__init__.py
--rw-r--r--   0        0        0      971 2022-10-31 09:41:37.492052 lucupy-0.1.8/lucupy/observatory/gemini/geminiobservation.py
--rw-r--r--   0        0        0     3599 2022-10-31 08:20:40.160082 lucupy-0.1.8/lucupy/observatory/gemini/geminiproperties.py
--rw-r--r--   0        0        0      606 2022-10-17 17:17:40.108151 lucupy-0.1.8/lucupy/sky/__init__.py
--rw-r--r--   0        0        0     4426 2022-10-17 17:24:45.829186 lucupy-0.1.8/lucupy/sky/altitude.py
--rw-r--r--   0        0        0     9312 2022-10-17 17:24:45.830370 lucupy-0.1.8/lucupy/sky/brightness.py
--rw-r--r--   0        0        0     2039 2022-10-17 17:24:45.830966 lucupy-0.1.8/lucupy/sky/constants.py
--rw-r--r--   0        0        0     3136 2022-10-17 17:24:45.831527 lucupy-0.1.8/lucupy/sky/events.py
--rw-r--r--   0        0        0    21553 2022-10-17 17:24:45.832550 lucupy-0.1.8/lucupy/sky/moon.py
--rw-r--r--   0        0        0     8763 2022-10-17 17:24:45.833321 lucupy-0.1.8/lucupy/sky/sun.py
--rw-r--r--   0        0        0    14876 2022-10-17 17:24:45.833972 lucupy-0.1.8/lucupy/sky/utils.py
--rw-r--r--   0        0        0     4248 2022-10-17 17:24:45.834519 lucupy-0.1.8/lucupy/timeutils/__init__.py
--rw-r--r--   0        0        0      478 2022-10-06 01:52:10.245296 lucupy-0.1.8/lucupy/types/__init__.py
--rw-r--r--   0        0        0     1998 2022-10-31 09:43:40.157299 lucupy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 lucupy-0.1.8/setup.py
--rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 lucupy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1528 2022-10-17 17:24:45.820558 lucupy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1006 2022-10-17 17:24:45.820882 lucupy-0.1.9/README.rst
+-rw-r--r--   0        0        0     1026 2022-10-17 17:24:45.821333 lucupy-0.1.9/lucupy/__init__.py
+-rw-r--r--   0        0        0      734 2022-10-17 17:24:45.821567 lucupy-0.1.9/lucupy/decorators/__init__.py
+-rw-r--r--   0        0        0     7408 2022-10-17 17:24:45.821843 lucupy-0.1.9/lucupy/helpers/__init__.py
+-rw-r--r--   0        0        0      636 2022-10-17 17:24:45.822222 lucupy-0.1.9/lucupy/minimodel/__init__.py
+-rw-r--r--   0        0        0     1309 2022-10-17 17:24:45.822493 lucupy-0.1.9/lucupy/minimodel/atom.py
+-rw-r--r--   0        0        0     8328 2022-10-17 17:24:45.822840 lucupy-0.1.9/lucupy/minimodel/constraints.py
+-rw-r--r--   0        0        0     9204 2022-11-09 03:07:10.325056 lucupy-0.1.9/lucupy/minimodel/group.py
+-rw-r--r--   0        0        0     2766 2022-10-17 17:24:45.823700 lucupy-0.1.9/lucupy/minimodel/magnitude.py
+-rw-r--r--   0        0        0    10051 2022-11-09 03:07:10.325546 lucupy-0.1.9/lucupy/minimodel/observation.py
+-rw-r--r--   0        0        0      974 2022-10-17 17:24:45.824269 lucupy-0.1.9/lucupy/minimodel/observationmode.py
+-rw-r--r--   0        0        0     4715 2022-11-09 03:07:10.326105 lucupy-0.1.9/lucupy/minimodel/program.py
+-rw-r--r--   0        0        0      780 2022-10-17 17:24:45.824744 lucupy-0.1.9/lucupy/minimodel/qastate.py
+-rw-r--r--   0        0        0     1055 2022-10-17 17:24:45.825010 lucupy-0.1.9/lucupy/minimodel/resource.py
+-rw-r--r--   0        0        0      914 2022-10-17 17:24:45.825413 lucupy-0.1.9/lucupy/minimodel/semester.py
+-rw-r--r--   0        0        0     1562 2022-10-17 17:24:45.825817 lucupy-0.1.9/lucupy/minimodel/site.py
+-rw-r--r--   0        0        0     2878 2022-10-17 17:24:45.826095 lucupy-0.1.9/lucupy/minimodel/target.py
+-rw-r--r--   0        0        0     2135 2022-10-17 17:24:45.826341 lucupy-0.1.9/lucupy/minimodel/timeallocation.py
+-rw-r--r--   0        0        0     1364 2022-10-17 17:24:45.826580 lucupy-0.1.9/lucupy/minimodel/timingwindow.py
+-rw-r--r--   0        0        0      844 2022-10-17 17:24:45.826826 lucupy-0.1.9/lucupy/minimodel/too.py
+-rw-r--r--   0        0        0      424 2022-11-07 18:10:11.047500 lucupy-0.1.9/lucupy/observatory/__init__.py
+-rw-r--r--   0        0        0     3262 2022-10-20 01:15:57.052740 lucupy-0.1.9/lucupy/observatory/abstract/__init__.py
+-rw-r--r--   0        0        0      245 2022-10-06 01:52:10.238720 lucupy-0.1.9/lucupy/observatory/gemini/__init__.py
+-rw-r--r--   0        0        0     1119 2022-11-09 03:07:10.326550 lucupy-0.1.9/lucupy/observatory/gemini/geminiobservation.py
+-rw-r--r--   0        0        0     3599 2022-10-31 08:20:40.160082 lucupy-0.1.9/lucupy/observatory/gemini/geminiproperties.py
+-rw-r--r--   0        0        0      606 2022-10-17 17:17:40.108151 lucupy-0.1.9/lucupy/sky/__init__.py
+-rw-r--r--   0        0        0     4426 2022-10-17 17:24:45.829186 lucupy-0.1.9/lucupy/sky/altitude.py
+-rw-r--r--   0        0        0     9312 2022-10-17 17:24:45.830370 lucupy-0.1.9/lucupy/sky/brightness.py
+-rw-r--r--   0        0        0     2039 2022-10-17 17:24:45.830966 lucupy-0.1.9/lucupy/sky/constants.py
+-rw-r--r--   0        0        0     3136 2022-10-17 17:24:45.831527 lucupy-0.1.9/lucupy/sky/events.py
+-rw-r--r--   0        0        0    21553 2022-10-17 17:24:45.832550 lucupy-0.1.9/lucupy/sky/moon.py
+-rw-r--r--   0        0        0     8763 2022-10-17 17:24:45.833321 lucupy-0.1.9/lucupy/sky/sun.py
+-rw-r--r--   0        0        0    14876 2022-10-17 17:24:45.833972 lucupy-0.1.9/lucupy/sky/utils.py
+-rw-r--r--   0        0        0     4248 2022-10-17 17:24:45.834519 lucupy-0.1.9/lucupy/timeutils/__init__.py
+-rw-r--r--   0        0        0      558 2022-11-09 03:07:10.338478 lucupy-0.1.9/lucupy/types/__init__.py
+-rw-r--r--   0        0        0     1998 2022-11-09 03:07:10.327506 lucupy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1975 1970-01-01 00:00:00.000000 lucupy-0.1.9/setup.py
+-rw-r--r--   0        0        0     1916 1970-01-01 00:00:00.000000 lucupy-0.1.9/PKG-INFO
```

### Comparing `lucupy-0.1.8/LICENSE` & `lucupy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/README.rst` & `lucupy-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/__init__.py` & `lucupy-0.1.9/lucupy/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/decorators/__init__.py` & `lucupy-0.1.9/lucupy/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/helpers/__init__.py` & `lucupy-0.1.9/lucupy/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/__init__.py` & `lucupy-0.1.9/lucupy/minimodel/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/atom.py` & `lucupy-0.1.9/lucupy/minimodel/atom.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/constraints.py` & `lucupy-0.1.9/lucupy/minimodel/constraints.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/group.py` & `lucupy-0.1.9/lucupy/minimodel/group.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from lucupy.helpers import flatten
 
 from .constraints import Constraints
 from .observation import Observation
 from .resource import Resource
 from .site import Site
+from ..types import ZeroTime
 
 GroupID = str
 
 
 @dataclass
 class Group(ABC):
     """This is the base implementation of AND / OR Groups.
@@ -118,48 +119,48 @@
 
         Returns:
             exec_time (timedelta): Sum of all the execution times.
         """
         if issubclass(type(self.children), Observation):
             return self.children.exec_time()
         else:
-            sum((child.exec_time() for child in self.children), timedelta())
+            sum((child.exec_time() for child in self.children), ZeroTime)
 
     def program_used(self) -> timedelta:
         """Program time used across the group.
 
         Returns:
             program_used (timedelta): Sum of all program_used times across children of this group.
         """
         if issubclass(type(self.children), Observation):
             return self.children.program_used()
         else:
-            return sum((child.program_used() for child in self.children), timedelta())
+            return sum((child.program_used() for child in self.children), ZeroTime)
 
     def partner_used(self) -> timedelta:
         """Partner time used across the group.
 
         Returns:
             partner_time (timedelta): Sum of all `partner_used` across the children of this group.
         """
         if issubclass(type(self.children), Observation):
             return self.children.partner_used()
         else:
-            return sum((child.partner_used() for child in self.children), timedelta())
+            return sum((child.partner_used() for child in self.children), ZeroTime)
 
     def total_used(self) -> timedelta:
         """Total time used across the group: includes program time and partner time.
 
         Returns:
             total_used (timedelta): Sum of total_used times across all children.
         """
         if issubclass(type(self.children), Observation):
             return self.children.total_used()
         else:
-            return sum((child.total_used() for child in self.children), timedelta())
+            return sum((child.total_used() for child in self.children), ZeroTime)
 
     def show(self, depth: int = 1) -> NoReturn:
         """Print content of the Group.
 
         Args:
             depth (int, optional): depth of the separator. Defaults to 1.
         """
```

### Comparing `lucupy-0.1.8/lucupy/minimodel/magnitude.py` & `lucupy-0.1.9/lucupy/minimodel/magnitude.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/observation.py` & `lucupy-0.1.9/lucupy/minimodel/observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .atom import Atom
 from .constraints import Constraints
 from .qastate import QAState
 from .resource import Resource
 from .site import Site
 from .target import Target, TargetType
 from .too import TooType
+from ..types import ZeroTime
 
 ObservationID = str
 
 
 class ObservationStatus(IntEnum):
     """
     The status of an observation as indicated in the Observing Tool / ODB.
@@ -164,15 +165,15 @@
         return next(filter(lambda t: t.type == TargetType.BASE, self.targets), None)
 
     def exec_time(self) -> timedelta:
         """
         Returns:
             Total execution time for the program, which is the sum across atoms and the acquisition overhead.
         """
-        return sum((atom.exec_time for atom in self.sequence), timedelta()) + self.acq_overhead
+        return sum((atom.exec_time for atom in self.sequence), ZeroTime) + self.acq_overhead
 
     def total_used(self) -> timedelta:
         """
         Returns:
             Total program time used: includes program time and partner time.
         """
         return self.program_used() + self.partner_used()
@@ -212,25 +213,25 @@
     def program_used(self) -> timedelta:
         """We roll this information up from the atoms as it will be calculated
             during the Optimizer algorithm. Note that it is also available directly
             from the OCS, which is used to populate the time allocation.
         Returns:
             (timedelta): With the time program used.
         """
-        return sum((atom.prog_time for atom in self.sequence), start=timedelta())
+        return sum((atom.prog_time for atom in self.sequence), start=ZeroTime)
 
     def partner_used(self) -> timedelta:
         """We roll this information up from the atoms as it will be calculated
         during the Optimizer algorithm. Note that it is also available directly
         from the OCS, which is used to populate the time allocation.
 
         Returns:
             (timedelta): With the time program used.
         """
-        return sum((atom.part_time for atom in self.sequence), start=timedelta())
+        return sum((atom.part_time for atom in self.sequence), start=ZeroTime)
 
     @staticmethod
     def _select_obsclass(classes: List[ObservationClass]) -> Optional[ObservationClass]:
         """Given a list of non-empty ObservationClasses, determine which occurs with
         highest precedence in the ObservationClasses enum, i.e. has the lowest index.
 
         This will be used when examining the sequence for atoms.
```

### Comparing `lucupy-0.1.8/lucupy/minimodel/observationmode.py` & `lucupy-0.1.9/lucupy/minimodel/observationmode.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/program.py` & `lucupy-0.1.9/lucupy/minimodel/program.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import ClassVar, FrozenSet, List, Optional
 
 from .group import AndGroup, Group, GroupID
 from .observation import Observation
 from .semester import Semester
 from .timeallocation import TimeAllocation
 from .too import TooType
+from ..types import ZeroTime
 
 ProgramID = str
 
 
 class Band(IntEnum):
     """
     Program band.
@@ -93,30 +94,30 @@
     allocated_time: FrozenSet[TimeAllocation]
     root_group: AndGroup
     too_type: Optional[TooType] = None
 
     FUZZY_BOUNDARY: ClassVar[timedelta] = timedelta(days=14)
 
     def program_awarded(self) -> timedelta:
-        return sum((t.program_awarded for t in self.allocated_time), timedelta())
+        return sum((t.program_awarded for t in self.allocated_time), ZeroTime)
 
     def program_awarded_used(self) -> timedelta:
-        return sum((t.program_used for t in self.allocated_time), timedelta())
+        return sum((t.program_used for t in self.allocated_time), ZeroTime)
 
     def partner_awarded(self) -> timedelta:
-        return sum((t.partner_awarded for t in self.allocated_time), timedelta())
+        return sum((t.partner_awarded for t in self.allocated_time), ZeroTime)
 
     def partner_awarded_used(self) -> timedelta:
-        return sum((t.partner_used for t in self.allocated_time), timedelta())
+        return sum((t.partner_used for t in self.allocated_time), ZeroTime)
 
     def total_awarded(self) -> timedelta:
-        return sum((t.total_awarded() for t in self.allocated_time), timedelta())
+        return sum((t.total_awarded() for t in self.allocated_time), ZeroTime)
 
     def total_awarded_used(self) -> timedelta:
-        return sum((t.total_used() for t in self.allocated_time), timedelta())
+        return sum((t.total_used() for t in self.allocated_time), ZeroTime)
 
     def program_used(self) -> timedelta:
         return self.root_group.program_used()
 
     def partner_used(self) -> timedelta:
         return self.root_group.partner_used()
```

### Comparing `lucupy-0.1.8/lucupy/minimodel/qastate.py` & `lucupy-0.1.9/lucupy/minimodel/qastate.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/resource.py` & `lucupy-0.1.9/lucupy/minimodel/resource.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/semester.py` & `lucupy-0.1.9/lucupy/minimodel/semester.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/site.py` & `lucupy-0.1.9/lucupy/minimodel/site.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/target.py` & `lucupy-0.1.9/lucupy/minimodel/target.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/timeallocation.py` & `lucupy-0.1.9/lucupy/minimodel/timeallocation.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/timingwindow.py` & `lucupy-0.1.9/lucupy/minimodel/timingwindow.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/minimodel/too.py` & `lucupy-0.1.9/lucupy/minimodel/too.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/observatory/abstract/__init__.py` & `lucupy-0.1.9/lucupy/observatory/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/observatory/gemini/geminiobservation.py` & `lucupy-0.1.9/lucupy/observatory/gemini/geminiobservation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Copyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
 # For license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause
 
 from datetime import timedelta
+from typing import Final
 
 from lucupy.minimodel import Observation
 
 from .geminiproperties import GeminiProperties
+from ...types import ZeroTime
+
+_IGRINS_CAL_TIME: Final[timedelta] = timedelta(minutes=10)
 
 
 def with_igrins_cal(func):
     def add_calibration(self):
-        if GeminiProperties.Instruments.IGRINS in self.required_resources() and self.partner_used() > 0:
-            return func(self) + timedelta(seconds=(1 / 6))
+        if (GeminiProperties.Instruments.IGRINS in self.required_resources()
+                and self.total_used - self.program_time() > ZeroTime):
+            return func(self) + _IGRINS_CAL_TIME
         return func(self)
 
     return add_calibration
 
 
 class GeminiObservation(Observation):
     """A Gemini-specific extension of the Observation class.
```

### Comparing `lucupy-0.1.8/lucupy/observatory/gemini/geminiproperties.py` & `lucupy-0.1.9/lucupy/observatory/gemini/geminiproperties.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/__init__.py` & `lucupy-0.1.9/lucupy/sky/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/altitude.py` & `lucupy-0.1.9/lucupy/sky/altitude.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/brightness.py` & `lucupy-0.1.9/lucupy/sky/brightness.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/constants.py` & `lucupy-0.1.9/lucupy/sky/constants.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/events.py` & `lucupy-0.1.9/lucupy/sky/events.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/moon.py` & `lucupy-0.1.9/lucupy/sky/moon.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/sun.py` & `lucupy-0.1.9/lucupy/sky/sun.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/sky/utils.py` & `lucupy-0.1.9/lucupy/sky/utils.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/lucupy/timeutils/__init__.py` & `lucupy-0.1.9/lucupy/timeutils/__init__.py`

 * *Files identical despite different names*

### Comparing `lucupy-0.1.8/pyproject.toml` & `lucupy-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lucupy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Lucuma core package for the Gemini Automated Scheduler at: https://github.com/gemini-hlsw/scheduler"
 authors = ["Sergio Troncoso <sergio.troncoso@noirlab.edu>",
            "Sebastian Raaphorst <sebastian.raaphorst@noirlab.edu>",
            "Bryan Miller <bryan.miller@noirlab.edu"]
 readme = "README.rst"
 homepage = "https://github.com/gemini-hlsw/lucupy"
 repository = "https://github.com/gemini-hlsw/lucupy"
```

### Comparing `lucupy-0.1.8/setup.py` & `lucupy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'': ['*']}
 
 install_requires = \
 ['astropy>=5.1,<6.0', 'pytz>=2022.2,<2023.0']
 
 setup_kwargs = {
     'name': 'lucupy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Lucuma core package for the Gemini Automated Scheduler at: https://github.com/gemini-hlsw/scheduler',
     'long_description': "Lucupy\n#########\n\nThis package contains data structures and functions to support all the microservices that make up the Schedule app\nfor the Gemini Program Plataform (and other auxiliary services such as Env and Resource)\n\nContent\n-------\n\n- Minimodel: A small version of GPP's data model. This allows for any services to use common data structures to model programs, observations, etc.\n- Helpers: A collection of functions that helps with the handling of data.\n- Observatory: An API that allows Observatory-specific behaviour to be added to a service (or sub-service: e.g Collector)\n- Sky: A library that calculates night events for the use of visibility in Observations\n- Time Utils: Time handling functions\n- Types: A collection of variables to use with Python typing\n- Decorators: A collection of decorators (Currently empty)\n\nCopyright (c) 2016-2022 Association of Universities for Research in Astronomy, Inc. (AURA)\nFor license information see LICENSE or https://opensource.org/licenses/BSD-3-Clause\n",
     'author': 'Sergio Troncoso',
     'author_email': 'sergio.troncoso@noirlab.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/gemini-hlsw/lucupy',
```

### Comparing `lucupy-0.1.8/PKG-INFO` & `lucupy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lucupy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Lucuma core package for the Gemini Automated Scheduler at: https://github.com/gemini-hlsw/scheduler
 Home-page: https://github.com/gemini-hlsw/lucupy
 Keywords: lucuma,scheudule,gpp
 Author: Sergio Troncoso
 Author-email: sergio.troncoso@noirlab.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Web Environment
```

