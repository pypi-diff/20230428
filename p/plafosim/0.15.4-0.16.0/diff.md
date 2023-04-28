# Comparing `tmp/plafosim-0.15.4.tar.gz` & `tmp/plafosim-0.16.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plafosim-0.15.4.tar", max compression
+gzip compressed data, was "plafosim-0.16.0.tar", max compression
```

## Comparing `plafosim-0.15.4.tar` & `plafosim-0.16.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    35149 2021-02-01 21:06:08.184543 plafosim-0.15.4/LICENSE
--rw-r--r--   0        0        0     8986 2022-10-20 15:41:39.196054 plafosim-0.15.4/README.md
--rw-r--r--   0        0        0     1688 2022-10-20 15:41:39.196054 plafosim-0.15.4/pyproject.toml
--rw-r--r--   0        0        0      716 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/__init__.py
--rw-r--r--   0        0        0        0 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/algorithms/__init__.py
--rw-r--r--   0        0        0     2363 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/algorithms/dummy.py
--rw-r--r--   0        0        0    30530 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/algorithms/speed_position.py
--rw-r--r--   0        0        0        0 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/cli/__init__.py
--rwxr-xr-x   0        0        0    24842 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/cli/plafosim.py
--rwxr-xr-x   0        0        0     6875 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/cli/trace_replay.py
--rw-r--r--   0        0        0     1636 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/emissions.py
--rw-r--r--   0        0        0     2584 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/formation_algorithm.py
--rw-r--r--   0        0        0     9333 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/gui.py
--rw-r--r--   0        0        0     4314 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/infrastructure.py
--rw-r--r--   0        0        0     6376 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/message.py
--rw-r--r--   0        0        0    18962 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/mobility.py
--rw-r--r--   0        0        0     4974 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/neighbortable.py
--rw-r--r--   0        0        0     7286 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/platoon.py
--rw-r--r--   0        0        0     1124 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/platoon_role.py
--rw-r--r--   0        0        0    55792 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/platooning_vehicle.py
--rw-r--r--   0        0        0    75738 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/simulator.py
--rw-r--r--   0        0        0     4576 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/spawning.py
--rw-r--r--   0        0        0    19244 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/statistics.py
--rw-r--r--   0        0        0    41732 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/sumocfg/freeway.gui.xml
--rw-r--r--   0        0        0     1192 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/sumocfg/freeway.net.xml
--rw-r--r--   0        0        0      328 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/sumocfg/freeway.rou.xml
--rw-r--r--   0        0        0      618 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/sumocfg/freeway.sumo.cfg
--rw-r--r--   0        0        0     5704 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/util.py
--rw-r--r--   0        0        0    21160 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/vehicle.py
--rw-r--r--   0        0        0     3963 2022-10-20 15:41:39.196054 plafosim-0.15.4/src/plafosim/vehicle_type.py
--rw-r--r--   0        0        0    10279 2022-10-20 15:45:32.973359 plafosim-0.15.4/setup.py
--rw-r--r--   0        0        0    10184 2022-10-20 15:45:32.973988 plafosim-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-02-01 21:06:08.184543 plafosim-0.16.0/LICENSE
+-rw-r--r--   0        0        0     9934 2023-04-28 13:34:00.128362 plafosim-0.16.0/README.md
+-rw-r--r--   0        0        0     2427 2023-04-28 13:34:00.128362 plafosim-0.16.0/pyproject.toml
+-rw-r--r--   0        0        0     2527 2023-04-28 13:34:00.128362 plafosim-0.16.0/src/plafosim/__init__.py
+-rw-r--r--   0        0        0      738 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/__init__.py
+-rw-r--r--   0        0        0     2407 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/dummy.py
+-rw-r--r--   0        0        0    30567 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/algorithms/speed_position.py
+-rw-r--r--   0        0        0      738 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/__init__.py
+-rw-r--r--   0        0        0    23667 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/plafosim.py
+-rw-r--r--   0        0        0     5357 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/cli/trace_replay.py
+-rw-r--r--   0        0        0     1716 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/emissions.py
+-rw-r--r--   0        0        0     2664 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/formation_algorithm.py
+-rw-r--r--   0        0        0     9372 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/gui.py
+-rw-r--r--   0        0        0     4398 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/infrastructure.py
+-rw-r--r--   0        0        0     6646 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/message.py
+-rw-r--r--   0        0        0    19006 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/mobility.py
+-rw-r--r--   0        0        0     5190 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/neighbortable.py
+-rw-r--r--   0        0        0     7553 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platoon.py
+-rw-r--r--   0        0        0     1180 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platoon_role.py
+-rw-r--r--   0        0        0    56157 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/platooning_vehicle.py
+-rw-r--r--   0        0        0    76270 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/simulator.py
+-rw-r--r--   0        0        0     4661 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/spawning.py
+-rw-r--r--   0        0        0    19290 2023-04-28 13:23:07.974459 plafosim-0.16.0/src/plafosim/statistics.py
+-rw-r--r--   0        0        0    42487 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml
+-rw-r--r--   0        0        0     1907 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml
+-rw-r--r--   0        0        0     1083 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.rou.xml
+-rw-r--r--   0        0        0     1328 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/sumocfg/freeway.sumo.cfg
+-rw-r--r--   0        0        0     5756 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/util.py
+-rw-r--r--   0        0        0    21551 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/vehicle.py
+-rw-r--r--   0        0        0     4188 2023-04-28 13:23:07.978459 plafosim-0.16.0/src/plafosim/vehicle_type.py
+-rw-r--r--   0        0        0    11244 2023-04-28 13:38:46.620355 plafosim-0.16.0/setup.py
+-rw-r--r--   0        0        0    11132 2023-04-28 13:38:46.620857 plafosim-0.16.0/PKG-INFO
```

### Comparing `plafosim-0.15.4/LICENSE` & `plafosim-0.16.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plafosim-0.15.4/README.md` & `plafosim-0.16.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # Platoon Formation Simulator (PlaFoSim)
 
-[![Code Version](https://img.shields.io/badge/code-v0.15.4-blue)](CHANGELOG.md)
+[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)
 [![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)
 [![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)
 [![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)
 
 [PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.
 
 PlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.
 While the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.
 
-Conceptual view on the process of Platoon Formation:
+Conceptual view on the process of Platoon Formation [1-2]:
 | Scenario | Advertisement | Assignment | Maneuver |
 | -------- | ------------- | ---------- | -------- |
 | ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |
 
-PlaFoSim is published here:
+PlaFoSim is published [here](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):
 
-> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.
+> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.
 
 Please note that PlaFoSim is still under heavy development.
 
 ---
 
 ## Installation
 
 - Install Python (>=3.7.0,<3.10)
 - Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
-- Install PlaFoSim via pypi:
+- Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):
 ```pip install plafosim```
 
 NOTE: The project is currently only tested under Linux.
 
 ## Running a Simulation
 
 You can use the simulator as module as well as from the command-line.
@@ -58,15 +58,15 @@
 - vehicle properties
 - trip properties
 - communication properties
 - platoon properties
 - formation properties
 - infrastructure properties
 - simulation properties
-- gui properties
+- GUI properties
 - result recording properties
 ```
 
 You can see the complete list of available parameters in the help:
 
 ```plafosim -h, --help```
 
@@ -121,31 +121,31 @@
 To see all options of this script, run:
 
 ```plafosim-replay -h, --help```
 
 ## Extending
 
 - Clone the repository
-- Install poetry
+- Install [poetry](https://python-poetry.org/):
 ```pip install poetry```
-- Install PlaFoSim from source in editable mode
+- Install PlaFoSim from source in editable mode:
 ```poetry install```
 - Run PlaFoSim in the virtual environment with
 ```poetry run plafosim```
 or activate the virtual enviroment first with
 ```poetry shell```
 and run the commands as usual (see above)
 
 NOTE: The project is currently only tested under Linux.
 
 In order to add a new formation algorithm, you need to follow these steps:
 - Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.
 - Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.
 - Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.
-- Import your algorithm and add parsing of its `__name__` to `__init__` within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
+- Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
 
 You should now be able to use your new algorithm with
 ```
 plafosim --formation-algorithm dummy_algorithm_name
 ```
 
 ## Contributing
@@ -164,28 +164,40 @@
 
 ### Validation
 
 To validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).
 The corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.
 You can have a look at `.drone.yml` for details regarding the execution.
 
+### Profiling
+
+You can profile the runtime of PlaFoSim's code by using [cProfile](https://docs.python.org/3/library/profile.html#module-cProfile):
+
+```poetry run python -m cProfile -o profile.out -m plafosim.cli.plafosim```
+
+You can visualize the results of the profiling run by using [SnakeViz](https://docs.python.org/3/library/profile.html#module-cProfile):
+
+```snakeviz profile.out```
+
 ## Contributors & Citing
 
-PlaFoSim was designed built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).
+PlaFoSim was designed and built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).
 It is currently maintained by [Julian Heinovski](https://github.com/heinovski/).
 The list of all authors can be found [here](AUTHORS.md).
 
-If you are working with `PlaFoSim`, please cite the [following paper](https://www2.tkn.tu-berlin.de/bib/heinovski2021scalable/):
+If you are working with `PlaFoSim`, please cite the [following paper](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):
 
-> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.
+> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.
 
 ```bibtex
 @inproceedings{heinovski2021scalable,
     author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},
+    doi = {10.1109/VNC52810.2021.9644678},
     title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},
+    pages = {137--138},
     publisher = {IEEE},
     issn = {2157-9865},
     isbn = {978-1-66544-450-7},
     address = {Virtual Conference},
     booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},
     month = {11},
     year = {2021},
@@ -195,14 +207,16 @@
 ## License
 
 PlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.
 
 ```
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -211,8 +225,10 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ```
 
 ## List of References
 
-[1] Julian Heinovski and Falko Dressler, "Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols," Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.
+[1] Julian Heinovski and Falko Dressler, ["Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols,"](https://www.tkn.tu-berlin.de/bib/heinovski2018platoon/) Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.
+
+[2] Julian Heinovski, ["Platoon Formation: Car-to-Platoon Assignments for Individual Cars,"](https://www.tkn.tu-berlin.de/bib/heinovski2019platoon/) Proceedings of International Conference on Networked Systems (NetSys 2019), PhD Forum, Munich, Germany, March 2019.
```

### Comparing `plafosim-0.15.4/src/plafosim/__init__.py` & `plafosim-0.16.0/src/plafosim/algorithms/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
-
-__version__ = "0.15.4"
```

### Comparing `plafosim-0.15.4/src/plafosim/algorithms/dummy.py` & `plafosim-0.16.0/src/plafosim/algorithms/dummy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -21,25 +23,25 @@
 from ..formation_algorithm import FormationAlgorithm
 
 LOG = logging.getLogger(__name__)
 
 
 class Dummy(FormationAlgorithm):
     """
-    Dummy Formation Algorithm
+    Dummy Formation Algorithm.
     """
 
     def __init__(
         self,
         owner: object,
         **kw_args,
     ):
 
         """
-        Initializes an instance of this formation algorithm to be used in a vehicle or an infrastructure.
+        Initialize an instance of this formation algorithm to be used in a vehicle or an infrastructure.
 
         Parameters
         ----------
         owner : object
             The owning object that is execution this algorithm.
             This can be either a PlatooningVehicle or an Infrastructure.
         """
@@ -54,25 +56,25 @@
             type=int,
             default=-1,
             help="A dummy parameter",
         )
 
     def do_formation(self):
         """
-        Runs platoon formation algorithm to search for a platooning opportunity
+        Run platoon formation algorithm to search for a platooning opportunity
         and performs the corresponding maneuvers.
         """
 
         from ..infrastructure import Infrastructure
         if isinstance(self._owner, Infrastructure):
             print(f'Running formation algorithm {self.name} on infrastructure! Unfortunately, this is just a dummy!')
         else:
             print(f'Running formation algorithm {self.name} on a vehicle! Unfortunately, this is just a dummy!')
 
     def finish(self):
         """
-        Cleans up the instance of the formation algorithm.
+        Clean up the instance of the formation algorithm.
 
         This includes mostly statistic recording.
         """
 
         pass
```

### Comparing `plafosim-0.15.4/src/plafosim/algorithms/speed_position.py` & `plafosim-0.16.0/src/plafosim/algorithms/speed_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -56,15 +58,15 @@
         position_deviation_threshold: int = DEFAULTS['position_deviation_threshold'],
         formation_centralized_kind: str = DEFAULTS['formation_centralized_kind'],
         solver_time_limit: int = DEFAULTS['solver_time_limit'],
         **kw_args,
     ):
 
         """
-        Initializes an instance of this formation algorithm to be used in a vehicle or an infrastructure.
+        Initialize an instance of this formation algorithm to be used in a vehicle or an infrastructure.
 
         Parameters
         ----------
         owner : object
             The owning object that is execution this algorithm.
             This can be either a PlatooningVehicle or an Infrastructure.
         alpha : float
@@ -141,15 +143,15 @@
             type=int,
             default=int(DEFAULTS['solver_time_limit'] / 1000),  # ms -> s
             help="The time limit for the optimal solver per assignment problem in s. Influences the quality of the solution.",
         )
 
     def ds(self, vehicle: 'PlatooningVehicle', platoon: 'Platoon'):
         """
-        Returns the deviation in speed from a given platoon.
+        Return the deviation in speed from a given platoon.
 
         NOTE: In the original version of the paper, the deviation calculated here was not normalized.
 
         Parameters
         ----------
         vehicle : PlatooningVehicle
             The vehicle for which the deviation is calculated
@@ -160,15 +162,15 @@
         diff = abs(vehicle._desired_speed - platoon.desired_speed)
 
         # normalize deviation by maximum allowed speed deviation
         return (diff / (self._speed_deviation_threshold * vehicle._desired_speed))
 
     def dp(self, vehicle: 'PlatooningVehicle', platoon: 'Platoon'):
         """
-        Returns the deviation in position from a given platoon.
+        Return the deviation in position from a given platoon.
 
         NOTE: In the original version of the paper, the deviation calculated here was not normalized.
 
         Parameters
         ----------
         vehicle : PlatooningVehicle
             The vehicle for which the deviation is calculated
@@ -184,29 +186,29 @@
             diff = abs(platoon.rear_position - vehicle.position)
 
         # normalize deviation by maximum allowed position deviation
         return (diff / self._position_deviation_threshold)
 
     def cost_speed_position(self, ds: float, dp: int):
         """
-        Returns the overall cost (i.e., the weighted deviation) for a candidate.
+        Return the overall cost (i.e., the weighted deviation) for a candidate.
 
         Parameters
         ----------
         ds : float
             The deviation in speed
         dp : int
             The deviation in position
         """
 
         return (self._alpha * ds) + ((1.0 - self._alpha) * dp)
 
     def do_formation(self):
         """
-        Runs platoon formation algorithms to search for a platooning opportunity
+        Run platoon formation algorithms to search for a platooning opportunity
         and performs the corresponding join maneuver.
         """
 
         from ..infrastructure import Infrastructure
         if isinstance(self._owner, Infrastructure):
             LOG.info(f"{self._owner.iid} is running formation algorithm {self.name} ({self._formation_centralized_kind}) at {self._owner._simulator.step}")
             if self._formation_centralized_kind == 'optimal':
@@ -217,15 +219,15 @@
                 self._do_formation_centralized()
         else:
             # greedy
             self._do_formation_distributed()
 
     def finish(self):
         """
-        Cleans up the instance of the formation algorithm.
+        Clean up the instance of the formation algorithm.
 
         This includes mostly statistic recording.
         """
 
         # write statistics
         if not self._owner._simulator._record_platoon_formation:
             return
@@ -240,15 +242,15 @@
                 basename=self._owner._simulator._result_base_filename,
                 iid=self._owner.iid,
                 algorithm=self,
             )
 
     def _do_formation_distributed(self):
         """
-        Runs distributed greedy formation approach.
+        Run distributed greedy formation approach.
 
         This selects a candidate and triggers a join maneuver.
         """
 
         # we can only run the algorithm if we are not yet in a platoon
         # because this algorithm does not support changing the platoon later on
         if self._owner.platoon_role != PlatoonRole.NONE:
@@ -310,15 +312,15 @@
         # perform a join maneuver with the candidate's platoon
         # do we really want the candidate to advertise its platoon
         # or do we just want the leader to advertise its platoon?
         self._owner._join(best['pid'], best['lid'])
 
     def _do_formation_centralized(self):
         """
-        Runs centralized greedy formation approach.
+        Run centralized greedy formation approach.
 
         This selects candidates and triggers join maneuvers.
         """
 
         all_found_candidates = []
 
         from ..platooning_vehicle import PlatooningVehicle  # noqa 811
@@ -432,15 +434,15 @@
             # do we really want the candidate to advertise its platoon
             # or do we just want the leader to advertise its platoon?
             vehicle._join(best['pid'], best['lid'])
 
             # remove all matches from the list of possible matches that would include the selected vehicle
             def is_available(x: dict) -> bool:
                 """
-                Returns whether an entry from the list of possible matches is (still) available.
+                Return whether an entry from the list of possible matches is (still) available.
 
                 Parameters
                 ----------
                 x : dict
                     The entry from the list of possible matches
                 """
```

### Comparing `plafosim-0.15.4/src/plafosim/cli/plafosim.py` & `plafosim-0.16.0/src/plafosim/cli/plafosim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,77 +17,40 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import argparse
 import logging
 import pickle
 import sys
-import textwrap
 from distutils.util import strtobool
 from signal import SIGINT, signal
 from timeit import default_timer as timer
 
-from plafosim import __version__
+from plafosim import CustomFormatter, __citation__, __description__, __version__
 from plafosim.algorithms.speed_position import SpeedPosition
 from plafosim.simulator import DEFAULTS, Simulator
 from plafosim.util import find_resource
 
 
-class CustomFormatter(
-    argparse.ArgumentDefaultsHelpFormatter,
-    argparse.RawDescriptionHelpFormatter,
-    argparse.MetavarTypeHelpFormatter,
-):
-    """Metaclass combining multiple formatter classes for argparse"""
-
-    pass
-
-
 # TODO duplicated code with trace replay
 def parse_args() -> (argparse.Namespace, argparse._ArgumentGroup):
 
     # parse some parameters
     parser = argparse.ArgumentParser(
         formatter_class=CustomFormatter,
         allow_abbrev=False,
-        description=textwrap.dedent(f"""\
-            Platoon Formation Simulator (PlaFoSim) -- Version {__version__}.
-            A simple and scalable simulator for platoon formation.
-
-            Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
-            This program comes with ABSOLUTELY NO WARRANTY.
-            This is free software, and you are welcome to redistribute it under certain conditions.
-
-            If you are working with PlaFoSim, please cite the following paper:
-
-            Julian Heinovski, Dominik S. Buse and Falko Dressler,
-            "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim,"
-            Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021),
-            Poster Session, Virtual Conference, November 2021.
-        """),
+        description=__description__,
     )
 
     # miscellaneous
     parser.add_argument(
         "-C", "--citation",
         action="version",
         help="show the citation information and exit",
-        version=textwrap.dedent("""
-            @inproceedings{heinovski2021scalable,
-                author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},
-                title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},
-                publisher = {IEEE},
-                issn = {2157-9865},
-                isbn = {978-1-66544-450-7},
-                address = {Virtual Conference},
-                booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},
-                month = {11},
-                year = {2021},
-            }
-        """),
+        version=__citation__,
     )
     parser.add_argument(
         "-V", "--version",
         action="version",
         version=f"%(prog)s {__version__}",
     )
     parser.add_argument(
@@ -95,14 +60,26 @@
     )
     parser.add_argument(
         "-n", "--dry-run",
         action="store_true",
         help="show the current configuration and exit",
     )
     parser.add_argument(
+        "-q", "--quiet",
+        action="count",
+        default=0,
+        help=f"The amount of verbosity levels to be removed for printing the logs to the CLI. The starting level is {logging.getLevelName(DEFAULTS['log_level'])}.",
+    )
+    parser.add_argument(
+        "-v", "--verbosity",
+        action="count",
+        default=0,
+        help=f"The amount of verbosity levels to be added for printing the logs to the CLI. The starting level is {logging.getLevelName(DEFAULTS['log_level'])}.",
+    )
+    parser.add_argument(
         "--save-snapshot",
         type=str,
         default=None,
         metavar="FILE",
         help="Save a snapshot of the scenario to FILE and exit",
     )
     parser.add_argument(
@@ -412,21 +389,14 @@
     simulation.add_argument(
         "--random-seed",
         type=int,
         default=DEFAULTS['random_seed'],
         help="The seed (>=0) for the random number generator instead of the current system time",
     )
     simulation.add_argument(
-        "--log-level",
-        type=str,
-        default=logging.getLevelName(DEFAULTS['log_level']).lower(),
-        choices=["error", "warn", "info", "debug", "trace"],
-        help="The minimum level of logs to be printed",
-    )
-    simulation.add_argument(
         "--progress",
         type=lambda x: bool(strtobool(x)),
         default=DEFAULTS['progress'],
         choices=(True, False),
         help="Whether to enable the (simulation) progress bar",
     )
 
@@ -666,15 +636,15 @@
 
 def create_simulator(**kwargs: dict) -> Simulator:
     assert kwargs
 
     # prepare keyword arguments for simulator
     kwargs.pop('load_snapshot')
     kwargs.pop('save_snapshot')
-    kwargs['log_level'] = getattr(logging, kwargs['log_level'].upper(), 5)
+    kwargs['log_level'] = logging.getLevelName(max(DEFAULTS['log_level'] - ((kwargs['verbosity'] - kwargs['quiet']) * 10), 5))
     kwargs['max_step'] = int(kwargs['max_step'])
 
     # create new simulator
     return Simulator(**kwargs)
 
 
 def main():
@@ -712,15 +682,15 @@
             sys.exit("ERROR: Saving a loaded snapshot does not make sense!")
         # save snapshot
         save_snapshot(simulator, snapshot_filename=args.save_snapshot)
         print(f"Saved a snapshot of the simulation to {args.save_snapshot}. Exiting...")
         return
 
     def handler(signal, frame):
-        simulator.stop("SIGINT or CTRL-C detected!")
+        simulator.stop("SIGINT or CTRL-C detected! Stopping simulation...")
 
     signal(SIGINT, handler)
 
     # execute simulation
     start_time = timer()
 
     steps = simulator.run()
```

### Comparing `plafosim-0.15.4/src/plafosim/cli/trace_replay.py` & `plafosim-0.16.0/src/plafosim/cli/trace_replay.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -14,21 +16,20 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import argparse
 import logging
 import sys
-import textwrap
 import time
 
 import pandas
 from tqdm import tqdm
 
-from plafosim import __version__
+from plafosim import CustomFormatter, __citation__, __description__, __version__
 from plafosim.gui import (
     add_gui_vehicle,
     change_gui_vehicle_color,
     check_and_prepare_gui,
     close_gui,
     gui_step,
     move_gui_vehicle,
@@ -37,65 +38,29 @@
 )
 from plafosim.simulator import DEFAULTS
 from plafosim.util import find_resource, hex2rgb
 
 LOG = logging.getLogger(__name__)
 
 
-class CustomFormatter(
-    argparse.ArgumentDefaultsHelpFormatter,
-    argparse.RawDescriptionHelpFormatter,
-    argparse.MetavarTypeHelpFormatter,
-):
-    """Metaclass combining multiple formatter classes for argparse"""
-
-    pass
-
-
 # TODO duplicated code with main script
 def parse_args() -> argparse.Namespace:
     # parse some parameters
     parser = argparse.ArgumentParser(
         formatter_class=CustomFormatter,
         allow_abbrev=False,
-        description=textwrap.dedent(f"""\
-            Platoon Formation Simulator (PlaFoSim) -- Version {__version__}.
-            A simple and scalable simulator for platoon formation.
-
-            Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
-            This program comes with ABSOLUTELY NO WARRANTY.
-            This is free software, and you are welcome to redistribute it under certain conditions.
-
-            If you are working with PlaFoSim, please cite the following paper:
-
-            Julian Heinovski, Dominik S. Buse and Falko Dressler,
-            "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim,"
-            Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021),
-            Poster Session, Virtual Conference, November 2021.
-        """),
+        description=__description__,
     )
 
     # miscellaneous
     parser.add_argument(
         "-C", "--citation",
         action="version",
         help="show the citation information and exit",
-        version=textwrap.dedent("""
-            @inproceedings{heinovski2021scalable,
-                author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},
-                title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},
-                publisher = {IEEE},
-                issn = {2157-9865},
-                isbn = {978-1-66544-450-7},
-                address = {Virtual Conference},
-                booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},
-                month = {11},
-                year = {2021},
-            }
-        """),
+        version=__citation__,
     )
     parser.add_argument(
         "-V", "--version",
         action="version",
         version=f"%(prog)s {__version__}",
     )
```

### Comparing `plafosim-0.15.4/src/plafosim/emissions.py` & `plafosim-0.16.0/src/plafosim/emissions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -35,18 +37,22 @@
     Emission class for the HBEFA3 model.
     """
 
     PC_G_EU4 = 0
 
     @property
     def emission_factors(self) -> dict:
-        """Returns the emission factors of an emission class."""
+        """
+        Return the emission factors of an emission class.
+        """
 
         return EMISSION_FACTORS[self.name]
 
     @property
     def is_diesel(self) -> bool:
-        """Returns whether an emission class is for a diesel engine."""
+        """
+        Return whether an emission class is for a diesel engine.
+        """
 
         split = self.name.split('_')
         assert len(split) == 3
         return split[1] == 'D'
```

### Comparing `plafosim-0.15.4/src/plafosim/formation_algorithm.py` & `plafosim-0.16.0/src/plafosim/formation_algorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -28,15 +30,15 @@
     Abstract base class for any type of platoon formation algorithm (i.e., assignment calculation).
 
     Implementing sub-classes need to override the do_formation() method.
     """
 
     def __init__(self, owner: object):
         """
-        Initializes an instance of a formation algorithm.
+        Initialize an instance of a formation algorithm.
 
         Parameters
         ----------
         owner : object
             The owning object that is execution this algorithm.
             This can be either a PlatooningVehicle or an Infrastructure.
         """
@@ -44,15 +46,17 @@
         from .infrastructure import Infrastructure
         from .platooning_vehicle import PlatooningVehicle  # noqa 811
         assert (isinstance(owner, PlatooningVehicle) or isinstance(owner, Infrastructure))
         self._owner = owner  # the owning vehicle or infrastructure
 
     @property
     def name(self):
-        """Prints the name of the formation algorithm."""
+        """
+        Print the name of the formation algorithm.
+        """
 
         return self.__class__.__name__
 
     @abstractmethod
     def add_parser_argument_group(cls, parser: argparse.ArgumentParser) -> argparse._ArgumentGroup:
         """
         Abstract method for performing any type of platoon formation (i.e., assignment calculation).
@@ -69,10 +73,12 @@
 
         This methods needs to be overridden in implementing sub-classes.
         """
 
         sys.exit("ERROR: There shouldn't be an instance of this abstract base class!")
 
     def finish(self):
-        """Reserved for future use."""
+        """
+        Reserved for future use.
+        """
 
         pass
```

### Comparing `plafosim-0.15.4/src/plafosim/gui.py` & `plafosim-0.16.0/src/plafosim/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -44,15 +46,15 @@
 
     if api_version != TRACI_SUPPORTED_VERSION:
         sys.exit(f"ERROR: You are using an unsupported TraCI version ({api_version})! Make sure to install a SUMO version with TraCI API version {TRACI_SUPPORTED_VERSION}.")
 
 
 def start_gui(config: str, play: bool = True):
     """
-    Starts the GUI.
+    Start the GUI.
 
     Parameters
     ----------
     config : str
         The name of the configuration file
     """
 
@@ -108,15 +110,15 @@
     )
     # TODO set zoom?
     # traci.gui.setZoom(traci.gui.DEFAULT_VIEW, 1000)
 
 
 def add_gui_vehicle(vid: int, position: float, lane: int, speed: float, color: tuple = (0, 255, 0), track: bool = False):
     """
-    Adds a vehicle to the GUI.
+    Add a vehicle to the GUI.
 
     Parameters
     ----------
     vid : int
         The vehicle's id
     position : float
         The vehicle's current position
@@ -148,15 +150,15 @@
         if track:
             traci.gui.trackVehicle(traci.gui.DEFAULT_VIEW, str(vid))
             traci.gui.setZoom(traci.gui.DEFAULT_VIEW, 700000)
 
 
 def move_gui_vehicle(vid: int, position: float, lane: int, speed: float):
     """
-    Moves a vehicle in the GUI.
+    Move a vehicle in the GUI.
 
     Parameters
     ----------
     vid : int
         The id of the vehicle to change
     position : float
         The vehicle's new position
@@ -185,15 +187,15 @@
     import traci
     traci.simulationStep(target_step)
     assert traci.simulation.getTime() == float(target_step)
 
 
 def change_gui_vehicle_color(vid: int, color: tuple):
     """
-    Changes the color of a vehicle in the GUI.
+    Change the color of a vehicle in the GUI.
 
     Parameters
     ----------
     vid : int
         The id of the vehicle to change
     color : tuple
         The color (R, G, B) to use for the vehicle
@@ -202,15 +204,15 @@
     import traci
     LOG.trace(f"Changing color of vehicle {vid} to {color}")
     traci.vehicle.setColor(str(vid), color)
 
 
 def remove_gui_vehicle(vid: int):
     """
-    Removes a vehicle from the GUI.
+    Remove a vehicle from the GUI.
 
     Parameters
     ----------
     vid : int
         The id of the vehicle to remove
     """
 
@@ -232,16 +234,15 @@
     import traci
     for vid in set(map(int, traci.vehicle.getIDList())) - set(keep_vids):
         remove_gui_vehicle(vid)
 
 
 def close_gui():
     """
-    Closes the GUI.
-
+    Close the GUI.
     """
 
     import traci
     traci.close(False)
 
 
 def draw_ramps(road_length: int, interval: int, labels: bool):
```

### Comparing `plafosim-0.15.4/src/plafosim/infrastructure.py` & `plafosim-0.16.0/src/plafosim/infrastructure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -14,15 +16,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 import logging
 import sys
 
-from .algorithms.speed_position import SpeedPosition
+from .algorithms.speed_position import SpeedPosition  # noqa 401
 from .platooning_vehicle import PlatooningVehicle
 
 #from .simulator import Simulator  # TODO fix circular import
 
 LOG = logging.getLogger(__name__)
 
 
@@ -54,41 +56,44 @@
 
         self._simulator = simulator  # the simulator
         self._iid = iid  # the id of the infrastructure
         self._position = position  # the x position of the infrastructure
 
         if formation_algorithm is not None:
             # initialize formation algorithm
-            # TODO make enum
-            if formation_algorithm == SpeedPosition.__name__:
-                self._formation_algorithm = SpeedPosition(self, **kw_args)
-            else:
-                sys.exit(f"ERROR: Unknown formation algorithm {formation_algorithm}!")
+            try:
+                self._formation_algorithm = globals()[formation_algorithm](self, **kw_args)
+            except KeyError:
+                sys.exit(f"ERROR: Unknown formation algorithm {formation_algorithm}! Did you import it?")
             self._execution_interval = execution_interval
 
             # initialize timer
             self._last_formation_step = 0  # initialize with vehicle start
         else:
             self._formation_algorithm = None
 
     @property
     def iid(self) -> int:
-        """Returns the id of an infrastructure."""
+        """
+        Return the id of an infrastructure.
+        """
 
         return self._iid
 
     @property
     def position(self) -> int:
-        """Returns the position of an infrastructure."""
+        """
+        Return the position of an infrastructure.
+        """
 
         return self._position
 
     def action(self, step: int):
         """
-        Triggers actions of an infrastructure
+        Triggers actions of an infrastructure.
 
         Parameters
         ----------
         step : int
             The current simulation step
         """
 
@@ -129,11 +134,13 @@
                 continue
 
             neighbors.append(vehicle)
 
         return neighbors
 
     def finish(self):
-        """Cleans up the instance of the infrastructure"""
+        """
+        Clean up the instance of the infrastructure.
+        """
 
         if self._formation_algorithm is not None:
             self._formation_algorithm.finish()
```

### Comparing `plafosim-0.15.4/src/plafosim/message.py` & `plafosim-0.16.0/src/plafosim/message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,74 +17,92 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 from enum import Enum
 
 
 class Message:
-    """"
-    A collection of general data for an arbitrary message.
+    """
+    " A collection of general data for an arbitrary message.
 
     Messages are in general not used at the moment.
     """
 
     def __init__(self, origin: int, destination: int, data=None):
         self._origin = origin  # id of the originator of this message
         self._destination = destination  # id of the destination of this message
         self._data = data  # generic data of this message
 
     @property
     def origin(self) -> int:
-        """Get the originator of the message"""
+        """
+        Get the originator of the message.
+        """
         return self._origin
 
     @property
     def destination(self) -> int:
-        """Get the destination of the message"""
+        """
+        Get the destination of the message.
+        """
         return self._destination
 
     @property
     def data(self):
-        """Get the data of the message"""
+        """
+        Get the data of the message.
+        """
         return self._data
 
     def __str__(self) -> str:
-        """Get a string representation of the message"""
+        """
+        Get a string representation of the message.
+        """
         return f"{self._origin} -> {self._destination} ({self.__class__.__name__}): {self._data}"
 
 
 class ManeuverType(Enum):
-    """A collection of available maneuver (message) types"""
+    """
+    A collection of available maneuver (message) types.
+    """
 
     JOIN = 1  # corresponds to a join maneuver
     LEAVE = 2  # corresponds to a leave maneuver
     MERGE = 3  # corresponds to a merge maneuver
     SPLIT = 4  # corresponds to a split maneuver
     LANE_CHANGE = 5  # corresponds to a lane change maneuver
 
 
 class ManeuverMessage(Message):
-    """A collection of general data for an arbitrary maneuver maessage"""
+    """
+    A collection of general data for an arbitrary maneuver maessage.
+    """
 
     def __init__(self, origin: int, destination: int, maneuver_type: ManeuverType, platoon_id: int, leader_id: int):
-        """Initialize a maneuver message instance"""
+        """
+        Initialize a maneuver message instance.
+        """
 
         super().__init__(origin, destination)
         self._maneuver_type = maneuver_type  # ManeuverType of this message
         self._platoon_id = platoon_id  # id of the platoon the message corresponds to
         self._leader_id = leader_id  # id of the leader of the corresponding platoon
 
     @property
     def platoon_id(self) -> int:
-        """Get the platoon id the message corresponds to"""
+        """
+        Get the platoon id the message corresponds to.
+        """
         return self._platoon_id
 
     @property
     def leader_id(self) -> int:
-        """Get the leader id of the platoon the message corresponds to"""
+        """
+        Get the leader id of the platoon the message corresponds to.
+        """
         return self._leader_id
 
     @property
     def maneuver_type(self) -> ManeuverType:
         return self._maneuver_type
 
     def __str__(self) -> str:
@@ -157,48 +177,56 @@
 
 # TODO
 class AbortManeuver(ManeuverMessage):
     pass
 
 
 class PlatoonAdvertisement(Message):
-    """A collection of general data for a platoon advertisement message"""
+    """
+    A collection of general data for a platoon advertisement message.
+    """
 
     def __init__(
             self,
             origin: int,
             destination: int,
             platoon_id: int,
             leader_id: int,
             platoon_speed: float,
             platoon_lane: int,
             platoon_formation: list,
             platoon_position_front: float,
             platoon_position_back: float):
-        """Initialize a platoon advertisement instance"""
+        """
+        Initialize a platoon advertisement instance.
+        """
 
         super().__init__(origin, destination)
         self._platoon_id = platoon_id  # id of the platoon the message corresponds to
         self._leader_id = leader_id  # id of the leader of the corresponding platoon
         self._platoon_speed = platoon_speed  # current speed of the advertised platoon
         self._platoon_lane = platoon_lane  # current lane of the advertised platoon
         self._platoon_formation = platoon_formation  # current formation of the advertised platoon
         # current position of the front of the advertised platoon (front of leader)
         self._platoon_position_front = platoon_position_front
         # current position of the back of the advertised platoon (back of last vehicle)
         self._platoon_position_back = platoon_position_back
 
     @property
     def platoon_id(self) -> int:
-        """Get the platoon id the message corresponds to"""
+        """
+        Get the platoon id the message corresponds to.
+        """
         return self._platoon_id
 
     @property
     def leader_id(self) -> int:
-        """Get the leader id of the platoon the message corresponds to"""
+        """
+        Get the leader id of the platoon the message corresponds to.
+        """
         return self._leader_id
 
     @property
     def platoon_speed(self) -> float:
         return self._platoon_speed
 
     @property
```

### Comparing `plafosim-0.15.4/src/plafosim/mobility.py` & `plafosim-0.16.0/src/plafosim/mobility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -518,15 +520,15 @@
 
 
 # position update components
 
 
 def clip_position(position: pd.Series, vdf: pd.DataFrame) -> pd.Series:
     """
-    Returns the clipped positions (i.e., by arrival position) of vehicles within a pandas DataFrame.
+    Return the clipped positions (i.e., by arrival position) of vehicles within a pandas DataFrame.
 
     Parameters
     ----------
     position : pandas.Series
         The series containing the positions to be clipped
         index: vid
         columns: [position, length, lane, ..]
@@ -549,15 +551,15 @@
     assert_index_equal(clipped_position, position)
 
     return clipped_position
 
 
 def update_position(vdf: pd.DataFrame, step_length: int) -> pd.DataFrame:
     """
-    Updates the position of vehicles within a pandas DataFrame.
+    Update the position of vehicles within a pandas DataFrame.
 
     This is based on Krauss' single lane traffic:
     adjust position (move)
     x(t + step_size) = x(t) + v(t)*step_size
 
     Parameters
     ----------
@@ -572,15 +574,15 @@
     position = vdf.position + (vdf.speed * step_length)
     vdf["position"] = clip_position(position, vdf)
     return vdf
 
 
 def get_crashed_vehicles(vdf: pd.DataFrame) -> list:
     """
-    Returns the list of crashed vehicles' ids
+    Return the list of crashed vehicles' ids.
 
     Parameters
     ----------
     vdf : pandas.DataFrame
         The dataframe containing the vehicles as rows
         index: vid
         columns: [position, length, lane, ..]
```

### Comparing `plafosim-0.15.4/src/plafosim/neighbortable.py` & `plafosim-0.16.0/src/plafosim/neighbortable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
-
 class NeighborData:
     """
     Collection of information from a single neighbor to be used within a NeighborTable.
 
     Neighbor tables are in general not used at the moment.
     """
 
@@ -31,15 +32,17 @@
                  platoon_speed: float,
                  platoon_lane: int,
                  platoon_formation: list,
                  platoon_position_front: float,
                  platoon_position_back: float,
                  timestamp: int,
                  valid: bool = True):
-        """Initialize a neighbor data instance"""
+        """
+        Initialize a neighbor data instance.
+        """
 
         self._vid = vid  # the id of the neighbor
         self._originator_id = originator_id  # the id the originator of this information
         self._platoon_id = platoon_id  # id of the platoon the message corresponds to
         self._leader_id = leader_id  # id of the leader of the corresponding platoon
         self._platoon_speed = platoon_speed  # current speed of the advertised platoon
         self._platoon_lane = platoon_lane  # current lane of the advertised platoon
@@ -100,45 +103,61 @@
     """
     Collection of information from neighbors, received via communication.
 
     Neighbor tables are in general not used at the moment.
     """
 
     def __init__(self, validity_time: int):
-        """Initialize a neighbor table instance"""
+        """
+        Initialize a neighbor table instance.
+        """
 
         self.neighbors = []  # the list of neighbors in the table
         self._validity_time = validity_time  # the time an entry in the table is valid
 
     def add_neighbor(self, neighbor: NeighborData):
-        """Add a neighbor to the neighbor table"""
+        """
+        Add a neighbor to the neighbor table.
+        """
         self._neighbors.append({neighbor.vid: neighbor})
 
     def remove_neighbor(self, neighbor_id: int) -> bool:
-        """Remove a neighbor from the neighbor table"""
+        """
+        Remove a neighbor from the neighbor table.
+        """
         self._vehicles.remove()
 
     def update_neighbor(self, neighbor: NeighborData):
-        """Update a neighbor in the neighbor table"""
+        """
+        Update a neighbor in the neighbor table.
+        """
         return self.add_neighbor(neighbor)  # TODO fix dict
 
     def get_neighbor(self, neighbor_id: int) -> NeighborData:
-        """Return a neighbor entry with the given id from the table"""
+        """
+        Return a neighbor entry with the given id from the table.
+        """
         pass
 
     def is_in_table(self, neighbor_id: int) -> bool:
-        """Return whether a neighbor with the given id is in the neighbor table"""
+        """
+        Return whether a neighbor with the given id is in the neighbor table.
+        """
         pass
 
     def size(self) -> int:
-        """Return the size of the neighbor table"""
+        """
+        Return the size of the neighbor table.
+        """
         return len(self._neighbors)
 
     def invalidate_entries(self, current_step: int):
-        """Invalidate entries in the neighbor table that exceeded the validity time"""
+        """
+        Invalidate entries in the neighbor table that exceeded the validity time.
+        """
         pass
 
     def number_of_valid_entries(self) -> int:
         pass
 
     @property
     def valid_entries(self) -> list:
```

### Comparing `plafosim-0.15.4/src/plafosim/platoon.py` & `plafosim-0.16.0/src/plafosim/platoon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -22,15 +24,17 @@
 if TYPE_CHECKING:
     from .platooning_vehicle import PlatooningVehicle  # noqa 401
 
 LOG = logging.getLogger(__name__)
 
 
 class Platoon:
-    """A collection of parameters for a specific platoon."""
+    """
+    A collection of parameters for a specific platoon.
+    """
 
     def __init__(
             self,
             platoon_id: int,
             formation: list,
             desired_speed: float):
         """
@@ -53,200 +57,226 @@
         self._max_acceleration = None
         self.update_max_acceleration()
         self._max_deceleration = None
         self.update_max_deceleration()
 
     @property
     def platoon_id(self) -> int:
-        """Returns the id of the platoon."""
+        """
+        Return the id of the platoon.
+        """
 
         return self._platoon_id
 
     @property
     def leader(self) -> 'PlatooningVehicle':
-        """Returns the leading PlatoonVehicle of the platoon."""
+        """
+        Return the leading PlatoonVehicle of the platoon.
+        """
 
         return self._formation[0]
 
     @property
     def last(self) -> 'PlatooningVehicle':
-        """Returns the last PlatooningVehicle of the platoon."""
+        """
+        Return the last PlatooningVehicle of the platoon.
+        """
 
         return self._formation[-1]
 
     @property
     def formation(self) -> list:
-        """Returns the complete formation of the platoon."""
+        """
+        Return the complete formation of the platoon.
+        """
 
         return self._formation
 
     @property
     def member_ids(self) -> list:
-        """Returns the ids of all platoon members."""
+        """
+        Return the ids of all platoon members.
+        """
 
         return [x._vid for x in self._formation]
 
     @property
     def desired_speed(self) -> float:
-        """Returns the desired driving speed of the platoon."""
+        """
+        Return the desired driving speed of the platoon.
+        """
 
         return self._desired_speed
 
     @property
     def speed(self) -> float:
-        """Returns the current driving speed of the platoon."""
+        """
+        Return the current driving speed of the platoon.
+        """
 
         # HACK for keeping the speed up to date
         return self.leader.speed
 
     @property
     def lane(self) -> int:
-        """Returns the current lane of the platoon."""
+        """
+        Return the current lane of the platoon.
+        """
 
         # HACK for keeping the lane up to date
         return self.leader.lane
 
     @property
     def max_speed(self) -> float:
         """
-        Returns the maximum speed of the platoon.
+        Return the maximum speed of the platoon.
 
         The maximum speed is based on the slowest vehicle within the platoon.
         """
 
         return self._max_speed
 
     def update_max_speed(self):
         """
-        Updates the maximum speed of the platoon.
+        Update the maximum speed of the platoon.
 
         The maximum speed is based on the slowest vehicle within the platoon.
         """
 
         self._max_speed = min(v.max_speed for v in self._formation)
 
     @property
     def max_acceleration(self) -> float:
         """
-        Returns the maximum acceleration of the platoon.
+        Return the maximum acceleration of the platoon.
 
         The maximum acceleration is based on the slowest vehicle within the platoon.
         """
 
         return self._max_acceleration
 
     def update_max_acceleration(self):
         """
-        Updates the maximum acceleration of the platoon.
+        Update the maximum acceleration of the platoon.
 
         The maximum acceleration is based on the slowest vehicle within the platoon.
         """
 
         self._max_acceleration = min(v.max_acceleration for v in self._formation)
 
     @property
     def max_deceleration(self) -> float:
         """
-        Returns the maximum deceleration of the platoon.
+        Return the maximum deceleration of the platoon.
 
         The maximum deceleration is based on the slowest vehicle within the platoon.
         """
 
         return self._max_deceleration
 
     def update_max_deceleration(self):
         """
-        Updates the maximum deceleration of the platoon.
+        Update the maximum deceleration of the platoon.
 
         The maximum deceleration is based on the slowest vehicle within the platoon.
         """
 
         self._max_deceleration = min(v.max_deceleration for v in self._formation)
 
     @property
     def size(self) -> int:
-        """Returns the size of the platoon."""
+        """
+        Return the size of the platoon.
+        """
 
         return len(self._formation)
 
     @property
     def position(self) -> int:
-        """Returns the current position of the platoon."""
+        """
+        Return the current position of the platoon.
+        """
 
         # HACK for keeping the position up to date
         return self.leader.position
 
     @property
     def rear_position(self) -> int:
-        """Returns the current rear position of the platoon."""
+        """
+        Return the current rear position of the platoon.
+        """
 
         # HACK for keeping the rear position up to date
         return self.last.rear_position
 
     @property
     def length(self) -> float:
-        """Returns the length of the platoon."""
+        """
+        Return the length of the platoon.
+        """
 
         return self.position - self.rear_position
 
     def get_member_index(self, vehicle: 'PlatooningVehicle') -> int:
         """
-        Returns the index of a member within the platoon.
+        Return the index of a member within the platoon.
 
         Parameters
         ----------
         vehicle : PlatooningVehicle
             The considered vehicle within the platoon.
         """
 
         return self._formation.index(vehicle)
 
     def get_front(self, vehicle: 'PlatooningVehicle'):
         """
-        Returns the PlatooningVehicle in the front.
+        Return the PlatooningVehicle in the front.
 
         Parameters
         ----------
         vehicle : PlatooningVehicle
             The considered vehicle within the platoon.
         """
 
         if vehicle is not self.leader:
             return self._formation[self.get_member_index(vehicle) - 1]
         else:
             return None
 
     def get_back(self, vehicle: 'PlatooningVehicle'):
         """
-        Returns the PlatooningVehicle in the back.
+        Return the PlatooningVehicle in the back.
 
         Parameters
         ----------
         vehicle : PlatooningVehicle
             The considered vehicle within the platoon.
         """
 
         if vehicle is not self.last:
             return self._formation[self.get_member_index(vehicle) + 1]
         else:
             return None
 
     def update_desired_speed(self):
         """
-        Updates the desired driving speed of the platoon.
+        Update the desired driving speed of the platoon.
 
         This is based on the desired driving speed of all members.
         """
 
         old_desired_speed = self._desired_speed
         self._desired_speed = min(mean([v._desired_speed for v in self._formation]), self.max_speed)
         LOG.debug(f"Updated platoon {self.platoon_id}'s desired speed to {self.desired_speed} (from {old_desired_speed})")
 
     def update_limits(self):
         self.update_max_speed()
         self.update_max_acceleration()
         self.update_max_deceleration()
 
     def __str__(self) -> str:
-        """Returns the str representation of the platoon."""
+        """
+        Return the str representation of the platoon.
+        """
 
         return f"{self._platoon_id}: {self.member_ids}"
```

### Comparing `plafosim-0.15.4/src/plafosim/platoon_role.py` & `plafosim-0.16.0/src/plafosim/platoon_role.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -15,14 +17,16 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
 from enum import Enum
 
 
 class PlatoonRole(Enum):
-    """A collection of available platoon roles."""
+    """
+    A collection of available platoon roles.
+    """
 
     NONE = 0  # corresponds to driving individually
     LEADER = 1  # corresponds to being the leader of a platoon
     FOLLOWER = 2  # corresponds to being a follower in a platoon
     JOINER = 3  # corresponds to being in the process of joining a platoon
     LEAVER = 4  # corresponds to being in the process of leaving a platoon
```

### Comparing `plafosim-0.15.4/src/plafosim/platooning_vehicle.py` & `plafosim-0.16.0/src/plafosim/platooning_vehicle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -16,15 +18,15 @@
 #
 
 import logging
 import math
 import sys
 from typing import TYPE_CHECKING
 
-from .algorithms.speed_position import SpeedPosition
+from .algorithms.speed_position import SpeedPosition  # noqa 401
 from .gui import change_gui_vehicle_color
 from .message import Message, PlatoonAdvertisement
 from .mobility import CF_Model
 from .platoon import Platoon
 from .platoon_role import PlatoonRole
 from .statistics import (
     record_platoon_formation,
@@ -40,15 +42,17 @@
 if TYPE_CHECKING:
     from .simulator import Simulator  # noqa 401
 
 LOG = logging.getLogger(__name__)
 
 
 class PlatooningVehicle(Vehicle):
-    """A vehicle that has platooning functionality."""
+    """
+    A vehicle that has platooning functionality.
+    """
 
     def __init__(
             self,
             simulator: 'Simulator',
             vid: int,
             vehicle_type: VehicleType,
             depart_position: int,
@@ -64,15 +68,15 @@
             formation_algorithm: str = None,
             execution_interval: int = 1,  # TODO use defaults
             pre_filled: bool = False,
             **kw_args,
     ):
         # TODO use global default values
         """
-        Initializes a platooning vehicle instance.
+        Initialize a platooning vehicle instance.
 
         Parameters
         ----------
         simulator : Simulator
             The global simulator object
         vid : int
             The id of the vehicle
@@ -134,19 +138,18 @@
         self._join_data_last = None
         self._join_data_new_position = None
         # for a LEADER
         self._joiner = None
 
         if formation_algorithm:
             # initialize formation algorithm
-            # TODO make enum
-            if formation_algorithm == SpeedPosition.__name__:
-                self._formation_algorithm = SpeedPosition(self, **kw_args)
-            else:
-                sys.exit(f"ERROR: Unknown formation algorithm {formation_algorithm}!")
+            try:
+                self._formation_algorithm = globals()[formation_algorithm](self, **kw_args)
+            except KeyError:
+                sys.exit(f"ERROR: Unknown formation algorithm {formation_algorithm}! Did you import it?")
             self._execution_interval = execution_interval
 
             # initialize timers
             if pre_filled:
                 self._last_formation_step = simulator._rng.randint(0, self._execution_interval - 1)
             else:
                 self._last_formation_step = self._depart_time  # initialize with vehicle start
@@ -202,134 +205,146 @@
         self._candidates_found = 0
         self._candidates_filtered = 0
         self._candidates_filtered_follower = 0
         self._candidates_filtered_maneuver = 0
 
     @property
     def acc_headway_time(self) -> float:
-        """Returns the ACC headway time of the vehicle."""
+        """
+        Return the ACC headway time of the vehicle.
+        """
 
         return self._acc_headway_time
 
     @property
     def desired_headway_time(self) -> float:
         """
-        Returns the desired headway time of the vehicle.
+        Return the desired headway time of the vehicle.
 
         This is based on the currently active car following model.
         """
 
         if self._cf_model == CF_Model.ACC:
             return self._acc_headway_time
         elif self._cf_model == CF_Model.CACC:
             return -1
         return super().desired_headway_time
 
     @property
     def desired_speed(self) -> float:
         """
-        Returns the desired driving speed of the vehicle.
+        Return the desired driving speed of the vehicle.
 
         If the vehicle is in a platoon, it returns the desired driving speed of the entire platoon.
         """
 
         return self._platoon.desired_speed if self.is_in_platoon() else self._desired_speed
 
     @property
     def desired_gap(self) -> float:
         """
-        Returns the desired gap of the vehicle.
+        Return the desired gap of the vehicle.
 
         This is based on the currently active car following model.
         """
         if self._cf_model == CF_Model.CACC:
             return self._cacc_spacing
         return super().desired_gap
 
     @property
     def platoon_role(self) -> PlatoonRole:
-        """Returns the current platoon role of the vehicle."""
+        """
+        Return the current platoon role of the vehicle.
+        """
 
         return self._platoon_role
 
     @property
     def platoon(self) -> Platoon:
-        """Returns the platoon of the vehicle."""
+        """
+        Return the platoon of the vehicle.
+        """
 
         return self._platoon
 
     def is_in_platoon(self) -> bool:
         """
-        Returns whether the vehicle currently is in a platoon.
+        Return whether the vehicle currently is in a platoon.
 
         This is based on the current PlatoonRole.
         A joining or leaving vehicle is either not yet or still part of a platoon, thus the returned value should be true.
         """
 
         return self._platoon_role is not PlatoonRole.NONE
 
     def get_front_gap(self) -> float:
         """
-        Returns the gap to the vehicle in the front.
+        Return the gap to the vehicle in the front.
 
         This imitates a measurement of the front radar sensor.
         """
 
         return self._simulator._get_predecessor_rear_position(self) - self._position
 
     def get_front_speed(self) -> float:
         """
-        Returns the speed to the vehicle in the front.
+        Return the speed to the vehicle in the front.
 
         This imitates a measurement of the front radar sensor.
         """
 
         return self._simulator._get_predecessor_speed(self)
 
     @property
     def in_maneuver(self) -> bool:
-        """Returns whether the vehicle is currently in a maneuver."""
+        """
+        Return whether the vehicle is currently in a maneuver.
+        """
 
         return self._in_maneuver
 
     @in_maneuver.setter
     def in_maneuver(self, var: bool):
         """
-        Sets the maneuver status of the vehicle.
+        Set the maneuver status of the vehicle.
 
         Parameters
         ----------
         var : bool
             The maneuver status
         """
 
         assert var != self._in_maneuver, f"Maneuver request {var} does not match maneuver status {self._in_maneuver} of {self._vid}!"
         self._in_maneuver = var
 
     @property
     def time_in_platoon(self) -> int:
-        """Returns the travelled time within platoons."""
+        """
+        Return the travelled time within platoons.
+        """
 
         return self._time_in_platoon
 
     @property
     def distance_in_platoon(self) -> float:
-        """Returns the travelled distance within platoons."""
+        """
+        Return the travelled distance within platoons.
+        """
 
         return self._distance_in_platoon
 
     @property
     def color(self) -> tuple:
         """Return the current color of the vehicle."""
 
         return self._platoon.leader._color if self.is_in_platoon() else self._color
 
     def _calculate_emission(self, a: float, v: float, f: list, scale: float) -> float:
         """
-        Calculates the emitted pollutant amount using the given speed and acceleration.
+        Calculate the emitted pollutant amount using the given speed and acceleration.
 
         Parameters
         ----------
         a : float
             The current acceleration
         v : float
             The current speed
@@ -367,15 +382,15 @@
         else:
             emission_change = 0.0
 
         return super()._calculate_emission(a, v, f, scale) * (1.0 - emission_change)
 
     def finish(self):
         """
-        Cleans up the instance of the PlatooningVehicle.
+        Clean up the instance of the PlatooningVehicle.
 
         This includes leaving the platoon and mostly statistics recording.
         """
 
         if (self._position < self._arrival_position):
             LOG.warning(f"{self._vid}'s finish method was called even though vehicle did not arrive yet!")
             return
@@ -484,28 +499,34 @@
             # execute formation algorithm at every execution interval
             if step >= self._last_formation_step + self._execution_interval:
                 # search for a platoon (depending on the algorithm)
                 self._formation_algorithm.do_formation()
                 self._last_formation_step = step
 
     def info(self) -> str:
-        """Returns information about the PlatooningVehicle."""
+        """
+        Return information about the PlatooningVehicle.
+        """
 
         return f"{super().info()}, platoon {self._platoon}"
 
     def __str__(self) -> str:
-        """Returns the str representation of the platooning vehicle."""
+        """
+        Return the str representation of the platooning vehicle.
+        """
 
         self_dict = self.__dict__.copy()
         self_dict.update({'_vehicle_type': str(self._vehicle_type)})  # use str representation of vehicle type
         self_dict.update({'_platoon': str(self._platoon)})  # use str representation of platoon
         return str(self_dict)
 
     def _statistics(self):
-        """Writes continuous statistics."""
+        """
+        Write continuous statistics.
+        """
 
         super()._statistics()
 
         if not self._simulator._record_prefilled and self._depart_time == -1:
             # we do not record statistics for pre-filled vehicles
             return
 
@@ -524,15 +545,15 @@
                     step=self._simulator.step,
                     vehicle=self
                 )
 
     # TODO rework to only include "neighbors" and move platoon extraction to formation algorithm
     def _get_available_platoons(self):
         """
-        Returns the available platoon candidates of the vehicle.
+        Return the available platoon candidates of the vehicle.
 
         This imitates neighbor maintenance by using a neighbor table.
         """
 
         # HACK FOR AVOIDING MAINTAINING A NEIGHBOR TABLE (for now)
         platoons = []
         for vehicle in self._simulator._vehicles.values():
@@ -952,15 +973,15 @@
         LOG.debug(f"{self._vid} joined platoon {leader.platoon.platoon_id} (leader: {leader.vid})")
 
         self.in_maneuver = False
         leader.in_maneuver = False
 
     def calculate_approaching_time(self, target_position: float, target_speed: float) -> float:
         """
-        Calculate approximate time to approach the target position at target speed
+        Calculate approximate time to approach the target position at target speed.
 
         Parameters
         ----------
 
         target_position : float
             The target position to approach
         target_speed : float
@@ -1143,14 +1164,16 @@
 
             # we do not need to switch lanes if we arrived
             if self._position < self._arrival_position:
                 # leave the formation by changing the lane
                 # TODO this looks strange in the GUI, since we do this before actually leaving the formation
                 self._platoon_role = PlatoonRole.LEAVER
                 self._cf_model = CF_Model.ACC
+                # FIXME Missing method. TODO Implement with new function!
+                sys.exit(f"ERROR: This is not implemented (anymore)! {__file__}:{sys._getframe().f_lineno}")
                 if not self._simulator._change_lane(self, self._lane + 1, "maneuver"):
                     # could not leave the platoon
                     # TODO this could be just a return in future to let the leaver try again
                     sys.exit(f"ERROR: Could not move vehicle {self._vid} to the adjacent lane to leave the platoon {self._platoon.platoon_id}!")
 
             # move all remaining platoon members further to the front
             front = self._platoon.get_front(self)
@@ -1247,15 +1270,15 @@
                 self._vid,
                 self._position,
                 self.rear_position,
             ))
 
     def _handle_message(self, message: Message):
         """
-        Handles a message of arbitrary type Message.
+        Handle a message of arbitrary type Message.
 
         Messages are in general not used at the moment.
 
         Parameters
         ----------
         message : Message
             The message to be handled
@@ -1266,15 +1289,15 @@
         func = self.__class__.__dict__.get(
             '_receive_' + message.__class__.__name__,
             super().__dict__.get('_handle_message'))
         return func(self, message)
 
     def _receive_PlatoonAdvertisement(self, advertisement: PlatoonAdvertisement):
         """
-        Handles a message of the specific type PlatoonAdvertisement.
+        Handle a message of the specific type PlatoonAdvertisement.
 
         Messages are in general not used at the moment.
 
         Parameters
         ----------
         advertisement : PlatoonAdvertisement
             The advertisement to be received
```

### Comparing `plafosim-0.15.4/src/plafosim/simulator.py` & `plafosim-0.16.0/src/plafosim/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -74,19 +76,17 @@
     record_general_data_begin,
     record_general_data_end,
     record_platoon_change,
     record_simulation_trace,
     record_vehicle_change,
     record_vehicle_platoon_change,
 )
-from .util import addLoggingLevel
 from .vehicle import Vehicle
 from .vehicle_type import VehicleType
 
-addLoggingLevel('TRACE', 5)
 LOG = logging.getLogger(__name__)
 
 # assumptions
 # you just reach your arrival_position
 # position is in the middle of the front bumper
 # a vehicle ends at position + length
 # crash detection does not work with step length greater than 1
@@ -219,15 +219,17 @@
     LOG.warning(
         "The following vehicles performed rough braking:\n%s",
         brake_df
     )
 
 
 class Simulator:
-    """A collection of parameters and information of the simulator."""
+    """
+    A collection of parameters and information of the simulator.
+    """
 
     def __init__(
             self,
             *,
             road_length: int = DEFAULTS['road_length'],
             number_of_lanes: int = DEFAULTS['lanes'],
             ramp_interval: int = DEFAULTS['ramp_interval'],
@@ -297,15 +299,17 @@
             record_platoon_formation: bool = DEFAULTS['record_platoon_formation'],
             record_platoon_traces: bool = DEFAULTS['record_platoon_traces'],
             record_platoon_changes: bool = DEFAULTS['record_platoon_changes'],
             record_infrastructure_assignments: bool = DEFAULTS['record_infrastructure_assignments'],
             record_prefilled: bool = DEFAULTS['record_prefilled'],
             **kwargs: dict,
     ):
-        """Initializes a simulator instance."""
+        """
+        Initialize a simulator instance.
+        """
 
         # TODO add custom filter that prepends the log entry with the step time
         logging.basicConfig(level=log_level, stream=sys.stdout, format="%(levelname)s [%(name)s]: %(message)s")
 
         # road network properties
         self._road_length = road_length  # the length of the road
         self._number_of_lanes = number_of_lanes  # the number of lanes
@@ -395,14 +399,18 @@
         else:
             if maximum_trip_length < minimum_trip_length:
                 sys.exit("ERROR: Maximum trip length cannot be smaller than the minimum trip length!")
             if maximum_trip_length < ramp_interval:
                 sys.exit("ERROR: Maximum trip length cannot be smaller than the ramp interval!")
             if not maximum_trip_length % ramp_interval == 0:
                 sys.exit("ERROR: Maximum trip length has to be a multiple of the ramp interval!")
+            if maximum_trip_length == minimum_trip_length:
+                LOG.debug(f"Using static trip length of {maximum_trip_length}m for all vehicles")
+                if not random_arrival_position:
+                    sys.exit("ERROR: Static trip length is only possible in conjuction with random-arrival-position!")
             self._maximum_trip_length = maximum_trip_length  # the maximum trip length
 
         # communication properties
         self._communication_range = communication_range  # the maximum communication range between two vehicles
         if communication_range == -1:
             self._communication_range = road_length
         if self._communication_range <= 0:
@@ -530,51 +538,63 @@
         else:
             self._number_of_prefilled_vehicles = 0
 
         self._generate_infrastructures(number_of_infrastructures)
 
     @property
     def road_length(self) -> int:
-        """Returns the road length."""
+        """
+        Return the road length.
+        """
 
         return self._road_length
 
     @property
     def number_of_lanes(self) -> int:
-        """Returns the number of lanes."""
+        """
+        Return the number of lanes.
+        """
 
         return self._number_of_lanes
 
     @property
     def step_length(self) -> int:
-        """Returns the length of a simulation step."""
+        """
+        Return the length of a simulation step.
+        """
 
         return self._step_length
 
     @property
     def step(self) -> int:
-        """Returns the current simulation step."""
+        """
+        Return the current simulation step.
+        """
 
         return self._step
 
     def _call_vehicle_actions(self):
-        """Triggers actions on all vehicles in the simulation."""
+        """
+        Triggers actions on all vehicles in the simulation.
+        """
 
         for vehicle in self._vehicles.values():
             vehicle.action(self._step)
 
     def _call_infrastructure_actions(self):
-        """Triggers actions on all infrastructures in the simulation."""
+        """
+        Triggers actions on all infrastructures in the simulation.
+        """
 
         for infrastructure in self._infrastructures.values():
             infrastructure.action(self._step)
 
     def _get_predecessor(self, vehicle: Vehicle, lane: int = -1) -> Vehicle:
         """
-        Returns the preceding (i.e., front) vehicle for a given vehicle on a given lane.
+        Return the preceding (i.e., front) vehicle for a given vehicle on a given lane.
 
         Parameters
         ----------
         vehicle : Vehicle
             The vehicle to consider
         lane : int, optional
             The lane to consider.
@@ -596,15 +616,15 @@
         # we do not check for collisions here because this method is also called within an update step
         if candidates:
             predecessor = self._vehicles[min(candidates, key=candidates.get)]
         return predecessor
 
     def _get_successor(self, vehicle: Vehicle, lane: int = -1) -> Vehicle:
         """
-        Returns the succeeding (i.e., back) vehicle for a given vehicle on a given lane.
+        Return the succeeding (i.e., back) vehicle for a given vehicle on a given lane.
 
         Parameters
         ----------
         vehicle : Vehicle
             The vehicle to consider
         lane : int, optional
             The lane to consider.
@@ -626,15 +646,15 @@
         # we do not check for collisions here because this method is also called within an update step
         if candidates:
             successor = self._vehicles[max(candidates, key=candidates.get)]
         return successor
 
     def _get_predecessor_rear_position(self, vehicle: Vehicle, lane: int = -1) -> float:
         """
-        Returns the rear position of the preceding (i.e., front) vehicle for a given vehicle on a given lane.
+        Return the rear position of the preceding (i.e., front) vehicle for a given vehicle on a given lane.
 
         Parameters
         ----------
         vehicle : Vehicle
             The vehicle to consider
         lane : int, optional
             The lane to consider.
@@ -645,15 +665,15 @@
         if not p:
             return -1
         else:
             return p.rear_position
 
     def _get_predecessor_speed(self, vehicle: Vehicle, lane: int = -1) -> float:
         """
-        Returns the speed of the preceding (i.e., front) vehicle for a given vehicle on a given lane.
+        Return the speed of the preceding (i.e., front) vehicle for a given vehicle on a given lane.
 
         Parameters
         ----------
         vehicle : Vehicle
             The vehicle to consider
         lane : int, optional
             The lane to consider.
@@ -664,15 +684,15 @@
         if not p:
             return -1
         else:
             return p._speed
 
     def _remove_arrived_vehicles(self, arrived_vehicles: list):
         """
-        Removes arrived vehicles from the simulation.
+        Remove arrived vehicles from the simulation.
 
         Parameters
         ----------
         arrived_vehicles : list
             The ids of arrived vehicles
         """
 
@@ -684,15 +704,15 @@
                 remove_gui_vehicle(vid)
             # remove from vehicles
             del self._vehicles[vid]
 
     @staticmethod
     def _check_collisions(vdf: pd.DataFrame):
         """
-        Does collision checks for all vehicles in the simulation.
+        Do collision checks for all vehicles in the simulation.
 
         Parameters
         ----------
         vdf : pandas.DataFrame
             The dataframe containing the vehicles as rows
             index: vid
             columns: [position, length, lane, ..]
@@ -706,27 +726,29 @@
             for v in crashed_vehicles:
                 print(f"{v}: {vdf.at[v, 'position']}-{vdf.at[v, 'position']-vdf.at[v, 'length']},{vdf.at[v, 'lane']}")
             sys.exit(f"ERROR: There were collisions with the following vehicles {crashed_vehicles}!")
 
     @staticmethod
     def has_collision(vehicle1: TV, vehicle2: TV) -> bool:
         """
-        Checks for a collision between two vehicles.
+        Check for a collision between two vehicles.
 
         Parameters
         ----------
         vehicle1 : TV(position, rear_position, lane)
         vehicle2 : TV(position, rear_position, lane)
         """
         assert vehicle1 is not vehicle2
         assert vehicle1.lane == vehicle2.lane
         return min(vehicle1.position, vehicle2.position) - max(vehicle1.rear_position, vehicle2.rear_position) >= 0
 
     def _generate_vehicles(self):
-        """Adds pre-filled vehicles to the simulation."""
+        """
+        Add pre-filled vehicles to the simulation.
+        """
 
         LOG.debug(f"Pre-filling the road network with {self._number_of_vehicles} vehicles")
 
         assert not self._vehicles
         assert self._last_vehicle_id == -1
 
         for vid in tqdm(range(0, self._number_of_vehicles), desc="Generated vehicles", disable=not self._progress):
@@ -836,15 +858,15 @@
             LOG.trace(f"Generated vehicle {vid} at {depart_position}-{depart_position - vtype._length},{depart_lane} with {depart_speed}")
 
         if self._start_as_platoon:
             self._initialize_prefilled_platoon()
 
     def _vehicles_to_be_scheduled(self):
         """
-        1) Calculate how many vehicles should be spawned according to the depart method
+        1) Calculate how many vehicles should be spawned according to the depart method.
         """
 
         vehicles_to_be_scheduled = -1
         if not self._depart_flow and self._last_vehicle_id >= self._number_of_vehicles - 1:
             # limit the spawn by a maximum number of total vehicles
             LOG.debug(f"All {self._number_of_vehicles} vehicles have been spawned already")
             # clear scheduled vehicles
@@ -1016,15 +1038,15 @@
         depart_speed: float,
         depart_time: int,
         depart_delay: int = 0,
         communication_range: int = DEFAULTS['communication_range'],
         pre_filled: bool = False,
     ):
         """
-        Adds a vehicle to the simulation based on the given parameters.
+        Add a vehicle to the simulation based on the given parameters.
 
         NOTE: Make sure that you set last_vehicle_id correctly.
 
         Parameters
         ----------
         vid : int
             The id of the vehicle
@@ -1090,15 +1112,15 @@
         # add instance
         self._vehicles[vid] = vehicle
 
         return vehicle
 
     def _generate_infrastructures(self, number_of_infrastructures: int):
         """
-        Generates infrastructures for the simulation.
+        Generate infrastructures for the simulation.
 
         Parameters
         ----------
         number_of_infrastructures : int
             The number of infrastructures to generate
         """
 
@@ -1119,15 +1141,17 @@
                 **self._kwargs,
             )
             self._infrastructures[iid] = infrastructure
 
             LOG.info(f"Generated infrastructure {infrastructure.iid} at {position}")
 
     def _initialize_result_recording(self):
-        """Creates output files for all (enabled) statistics and writes the headers."""
+        """
+        Create output files for all (enabled) statistics and writes the headers.
+        """
 
         # write some general information about the simulation
         record_general_data_begin(basename=self._result_base_filename, simulator=self)
 
         if self._record_vehicle_trips:
             # create output file for vehicle trips
             initialize_vehicle_trips(basename=self._result_base_filename)
@@ -1182,15 +1206,15 @@
 
         if self._record_simulation_trace:
             # create output file for continuous simulation trace
             initialize_simulation_trace(basename=self._result_base_filename)
 
     def _initialize_prefilled_platoon(self):
         """
-        Initializes all pre-filled vehicles as one platoon.
+        Initialize all pre-filled vehicles as one platoon.
         """
 
         # we avoid the complicated join procedure and simply set all parameters
         leader = self._vehicles[0]
         leader._platoon_role = PlatoonRole.LEADER
         leader._platoon._formation = list(self._vehicles.values())
         if self._update_desired_speed:
@@ -1209,15 +1233,17 @@
             vehicle._cf_target_speed = vehicle._platoon.desired_speed
             vehicle._first_platoon_join_time = 0
             vehicle._last_platoon_join_time = 0
             vehicle._first_platoon_join_position = vehicle._position
             vehicle._last_platoon_join_position = vehicle._position
 
     def _initialize_gui(self):
-        """Initializes the GUI."""
+        """
+        Initialize the GUI.
+        """
 
         # start gui
         start_gui(self._sumo_config, self._gui_play)
 
         # set correct boundary and zoom
         set_gui_window(road_length=self._road_length)
 
@@ -1255,30 +1281,32 @@
                     if (isinstance(vehicle, PlatooningVehicle) and vehicle.is_in_platoon)
                     else vehicle._color
                 ),
                 track=vehicle.vid == self._gui_track_vehicle,
             )
 
     def _update_gui(self):
-        """Updates the GUI."""
+        """
+        Update the GUI.
+        """
 
         for vehicle in self._vehicles.values():
             # update vehicles
             move_gui_vehicle(vehicle.vid, vehicle.position, vehicle.lane, vehicle.speed)
 
         # remove vehicles not in simulator
         prune_vehicles(keep_vids=self._vehicles.keys())
 
         # sleep for visualization
         time.sleep(self._gui_delay)
 
     def run(self):
         """
+        Run the simulation with the specified parameters until it is stopped.
         Main simulation method.
-        Runs the simulation with the specified parameters until it is stopped.
 
         This is based on Krauss' multi lane traffic:
         laneChange();
         adjust();
         move();
         """
 
@@ -1422,15 +1450,17 @@
             self,
             vehicles_in_simulator: int,
             vehicles_in_queue: int,
             vehicles_spawned: int,
             vehicles_arrived: int,
             runtime: float
     ):
-        """Record some period statistics."""
+        """
+        Record some period statistics.
+        """
 
         self._avg_number_vehicles = int(
             (self._values_in_avg_number_vehicles * self._avg_number_vehicles + vehicles_in_simulator) /
             (self._values_in_avg_number_vehicles + 1)
         )
 
         if self._record_simulation_trace:
@@ -1442,15 +1472,15 @@
                 vehicles_in_queue=vehicles_in_queue,
                 vehicles_spawned=vehicles_spawned,
                 vehicles_arrived=vehicles_arrived,
                 runtime=runtime,
             )
 
     def _record_lane_changes(self, vdf: pd.DataFrame):
-        for row in vdf.query('lane != old_lane').itertuples():
+        for row in vdf[vdf.lane != vdf.old_lane].itertuples():
             if row.cf_model != CF_Model.CACC:
                 if self._record_vehicle_changes:
                     record_vehicle_change(
                         basename=self._result_base_filename,
                         step=self._step,
                         vid=row.Index,
                         position=row.position,
@@ -1476,15 +1506,17 @@
                         member=self._vehicles[row.Index],
                         source_lane=row.old_lane,
                         target_lane=row.lane,
                         reason=row.lc_reason,
                     )
 
     def _get_vehicles_df(self) -> pd.DataFrame:
-        """Returns a pandas dataframe from the internal data structure."""
+        """
+        Return a pandas dataframe from the internal data structure.
+        """
         platoon_fields = [
             "leader_id",
             "platoon_id",
             "platoon_desired_speed",
             "platoon_max_speed",
             "platoon_max_acceleration",
             "platoon_max_deceleration",
@@ -1557,15 +1589,15 @@
                 rear_position=lambda df: df[["rear_position", "platoon_rear_position"]].min(axis="columns"),
             )
             .drop(["cf_target_speed"], axis="columns")
         )
 
     def _write_back_vehicles_df(self, vdf: pd.DataFrame):
         """
-        Writes back the vehicle updates from a given pandas dataframe to the internal data structure.
+        Write back the vehicle updates from a given pandas dataframe to the internal data structure.
 
         Parameters
         ----------
         vdf : pandas.DataFrame
             The dataframe containing the vehicles as rows
             index: vid
             columns: [position, length, lane, ..]
@@ -1581,38 +1613,42 @@
             vehicle._speed = row.speed
             vehicle._acceleration = row.speed - row.old_speed
             vehicle._blocked_front = row.blocked_front
             vehicle._lane = row.lane
 
     def stop(self, msg: str):
         """
-        Stops the simulation with the given message.
+        Stop the simulation with the given message.
 
         Parameters
         ----------
         msg : str
             The message to show after stopping the simulation
         """
 
         self._running = False
         if self._progress:
             print(f"\n{msg}")
 
     def __str__(self) -> str:
-        """Returns a str representation of a simulator instance."""
+        """
+        Return a str representation of a simulator instance.
+        """
 
         sim_dict = vars(self).copy()
         sim_dict.pop('_vehicles')
         sim_dict.pop('_infrastructures')
         sim_dict.update({'current_number_of_vehicles': len(self._vehicles)})
         sim_dict.update({'current_number_of_infrastructures': len(self._infrastructures)})
         return str(dict(sorted(sim_dict.items())))
 
     def _finish(self):
-        """Cleans up the simulation."""
+        """
+        Clean up the simulation.
+        """
 
         if self._running:
             LOG.warning("Finish called during simulation!")
             return
 
         # write some general information about the simulation
         record_general_data_end(basename=self._result_base_filename, simulator=self)
@@ -1646,15 +1682,15 @@
     ramp_positions: list,
     current_step: int,
     rng: random.Random,
     random_depart_position: bool,
     random_arrival_position: bool,
 ):
     """
-    Schritt 4, siehe oben
+    Schritt 4, siehe oben.
 
     Assumption: list of vehicles is already sorted ascending by depart priority (e.g., waiting time)
     Assumption: ramp positions is sorted in ascending manner
     """
 
     if not vehicles:
         return pd.DataFrame(), []
@@ -1674,27 +1710,25 @@
 
         spawn_position = position + vtype.length
 
         # select predecessor at spawn position
         # since we have the dummy, we can assume there is always at least one vehicle
         vehicle_after_spawn_position = (
             vdf
-            .loc[vdf.position >= spawn_position]
-            .query('lane == 0')
+            [(vdf.position >= spawn_position) & (vdf.lane == 0)]
             .sort_values("position", ascending=True)
             .iloc[0]
         )
         gap_to_next_vehicle = vehicle_after_spawn_position.position - vtype.length - spawn_position
 
         # select successor of spawn position
         # since we have the dummy, we can assume there is always at least one vehicle
         vehicle_before_spawn_position = (
             vdf
-            .loc[vdf.position < spawn_position]
-            .query('lane == 0')
+            [(vdf.position < spawn_position) & (vdf.lane == 0)]
             .sort_values("position", ascending=True)
             .iloc[-1]
         )
         gap_to_previous_vehicle = spawn_position - vtype.length - vehicle_before_spawn_position.position
 
         max_remanining_trip_length = ramp_positions[-1] - position
```

### Comparing `plafosim-0.15.4/src/plafosim/spawning.py` & `plafosim-0.16.0/src/plafosim/spawning.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -22,15 +24,17 @@
     desired_speed: float,
     rng: random.Random,
     speed_variation: float,
     min_desired_speed: float,
     max_desired_speed: float,
     random_desired_speed: bool = False,
 ) -> float:
-    """Returns a (random) depart speed."""
+    """
+    Return a (random) depart speed.
+    """
 
     if random_desired_speed:
         # normal distribution
         speed = desired_speed * rng.normalvariate(1.0, speed_variation)
         speed = max(speed, min_desired_speed)
         speed = min(speed, max_desired_speed)
     else:
@@ -42,15 +46,15 @@
 def get_depart_speed(
     desired_speed: float,
     rng: random.Random,
     depart_desired: bool = False,
     random_depart_speed: bool = False,
 ) -> float:
     """
-    Returns a (random) depart speed.
+    Return a (random) depart speed.
 
     Parameters
     ----------
     desired_speed : float
         The desired speed to consider
     """
 
@@ -73,15 +77,15 @@
     min_trip_length: int,
     max_trip_length: int,
     rng: random.Random,
     random_arrival_position: bool = False,
     pre_fill: bool = False,
 ) -> int:
     """
-    Returns a (random) arrival position for a given depart position.
+    Return a (random) arrival position for a given depart position.
 
     This considers the ramp interval, road length, and minimum trip length.
 
     Parameters
     ----------
     depart_position : int
         The depart position to consider
@@ -119,18 +123,19 @@
     assert min_arrival_ramp >= 0
     assert min_arrival_ramp <= road_length
     assert min_arrival_ramp <= max_arrival_ramp
     assert max_arrival_ramp <= road_length
     if min_arrival % ramp_interval == 0:
         assert min_arrival == min_arrival_ramp
 
-    if random_arrival_position and max_arrival_ramp < road_length:
+    if random_arrival_position:
         # make sure to also include the end of the road itself
         arrival_position = rng.randrange(min_arrival_ramp, max_arrival_ramp + 1, ramp_interval)
-        assert arrival_position >= min_arrival_ramp
+        assert min_arrival_ramp <= arrival_position <= max_arrival_ramp
+        assert arrival_position <= road_length
     else:
         # simply drive until the end of the trip or the road
         arrival_position = min(max_arrival_ramp, road_length)
 
     assert arrival_position <= road_length
     assert arrival_position > depart_position
     assert arrival_position - depart_position <= max_trip_length
```

### Comparing `plafosim-0.15.4/src/plafosim/statistics.py` & `plafosim-0.16.0/src/plafosim/statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
```

### Comparing `plafosim-0.15.4/src/plafosim/sumocfg/freeway.gui.xml` & `plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml`

 * *Files 0% similar despite different names*

#### Comparing `plafosim-0.15.4/src/plafosim/sumocfg/freeway.gui.xml` & `plafosim-0.16.0/src/plafosim/sumocfg/freeway.gui.xml`

```diff
@@ -1,8 +1,26 @@
 <?xml version="1.0" encoding="utf-8"?>
+<!--
+Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+
+SPDX-License-Identifier: GPL-3.0-or-later
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+-->
 <viewsettings>
   <scheme name="custom_1">
     <opengl dither="0" fps="0"/>
     <background backgroundColor="51,128,51" showGrid="0" gridXSize="100.00" gridYSize="100.00"/>
     <edges laneEdgeMode="0" scaleMode="0" laneShowBorders="1" showBikeMarkings="1" showLinkDecals="1" showLinkRules="1" showRails="1" hideConnectors="1" widthExaggeration="1.00" minSize="0.00" showDirection="0" showSublanes="1" spreadSuperposed="0" edgeParam="EDGE_KEY" laneParam="LANE_KEY" edgeData="speed" edgeName_show="0" edgeName_size="50.00" edgeName_color="orange" edgeName_bgColor="128,0,0,0" edgeName_constantSize="1" internalEdgeName_show="0" internalEdgeName_size="40.00" internalEdgeName_color="128,64,0" internalEdgeName_bgColor="128,0,0,0" internalEdgeName_constantSize="1" cwaEdgeName_show="0" cwaEdgeName_size="50.00" cwaEdgeName_color="magenta" cwaEdgeName_bgColor="128,0,0,0" cwaEdgeName_constantSize="1" streetName_show="0" streetName_size="55.00" streetName_color="yellow" streetName_bgColor="128,0,0,0" streetName_constantSize="1" edgeValue_show="0" edgeValue_size="100.00" edgeValue_color="cyan" edgeValue_bgColor="128,0,0,0" edgeValue_constantSize="1">
       <colorScheme name="uniform">
         <entry color="black" name="road"/>
```

### Comparing `plafosim-0.15.4/src/plafosim/sumocfg/freeway.net.xml` & `plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml`

 * *Files 21% similar despite different names*

#### Comparing `plafosim-0.15.4/src/plafosim/sumocfg/freeway.net.xml` & `plafosim-0.16.0/src/plafosim/sumocfg/freeway.net.xml`

```diff
@@ -1,8 +1,26 @@
 <?xml version="1.0" encoding="utf-8"?>
+<!--
+Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
+
+SPDX-License-Identifier: GPL-3.0-or-later
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+-->
 <net xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" version="1.1" xsi:noNamespaceSchemaLocation="http://sumo.dlr.de/xsd/net_file.xsd">
   <location netOffset="0.00,254.00" convBoundary="0.00,254.00,9400.00,254.00" origBoundary="0.00,-254.00,50000.00,0.00" projParameter="!"/>
   <edge id="edge_0_0" from="node_0_0" to="node_0_1" priority="7" length="1000000.00">
     <lane id="edge_0_0_0" index="0" speed="36.0" length="1000000.00" shape="0.00,242.80 1000000.00,242.80"/>
     <lane id="edge_0_0_1" index="1" speed="36.0" length="1000000.00" shape="0.00,246.00 1000000.00,246.00"/>
     <lane id="edge_0_0_2" index="2" speed="36.0" length="1000000.00" shape="0.00,249.20 1000000.00,249.20"/>
     <lane id="edge_0_0_3" index="3" speed="36.0" length="1000000.00" shape="0.00,252.40 1000000.00,252.40"/>
```

### Comparing `plafosim-0.15.4/src/plafosim/util.py` & `plafosim-0.16.0/src/plafosim/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -55,73 +57,73 @@
     assert len(hex[1:]) == 6
 
     return tuple(int(i, 16) for i in textwrap.wrap(hex[1:], 2))
 
 
 def assert_index_equal(a, b):
     """
-    Ensures the indeces of two Sequences/DataFrames are equal.
+    Ensure the indeces of two Sequences/DataFrames are equal.
 
     Parameters
     ----------
     a : pandas.Sequence / pandas.DataFrame
     b : pandas.Sequence / pandas.DataFrame
     """
 
     assert list(a.index) == list(b.index)
 
 
 def speed2distance(speed: float, time_interval: float = 1.0) -> float:
     """
-    Converts a driving speed to a distance driven within a given time interval.
+    Convert a driving speed to a distance driven within a given time interval.
 
     Parameters
     ----------
     speed : float
         The speed to be converted
     time_interval : float, optional
         The time to consider
     """
 
     return speed * time_interval
 
 
 def distance2speed(distance: float, time_interval: float = 1.0) -> float:
     """
-    Converts a driven distance to a driving speed for a given time interval.
+    Convert a driven distance to a driving speed for a given time interval.
 
     Parameters
     ----------
     distance : float
         The distance to be converted
     time_interval : float, optional
         The time to consider
     """
 
     return distance / time_interval
 
 
 def acceleration2speed(acceleration: float, time_interval: float = 1.0) -> float:
     """
-    Converts an acceleration to a driving speed for a given time interval.
+    Convert an acceleration to a driving speed for a given time interval.
 
     Parameters
     ----------
     acceleration : float
         The acceleration to be converted
     time_interval : float, optional
         The time to consider
     """
 
     return acceleration * time_interval
 
 
 def speed2acceleration(speed_from: float, speed_to: float, time_interval: float = 1.0) -> float:
     """
-    Converts a speed range to an acceleration within a given time interval.
+    Convert a speed range to an acceleration within a given time interval.
 
     Parameters
     ----------
     speed_from : float
         The initial speed
     speed_to : float
         The target speed
@@ -130,15 +132,15 @@
     """
 
     return (speed_to - speed_from) / time_interval
 
 
 def addLoggingLevel(levelName, levelNum, methodName=None):
     """
-    https://stackoverflow.com/a/35804945
+    https://stackoverflow.com/a/35804945.
 
     Comprehensively adds a new logging level to the `logging` module and the currently configured logging class.
 
     `levelName` becomes an attribute of the `logging` module with the value `levelNum`. `methodName` becomes a convenience method for both `logging` itself and the class returned by `logging.getLoggerClass()` (usually just `logging.Logger`). If `methodName` is not specified, `levelName.lower()` is used.
 
     To avoid accidental clobberings of existing attributes, this method will raise an `AttributeError` if the level name is already an attribute of the `logging` module or if the method name is already present
     """
@@ -166,15 +168,17 @@
     logging.addLevelName(levelNum, levelName)
     setattr(logging, levelName, levelNum)
     setattr(logging.getLoggerClass(), methodName, logForLevel)
     setattr(logging, methodName, logToRoot)
 
 
 class FakeLog:
-    """A fake logger, hide LOG behind this and be happy."""
+    """
+    A fake logger, hide LOG behind this and be happy.
+    """
     def trace(self, *arg, **kwd):
         pass
 
     def debug(self, *arg, **kwd):
         pass
 
     def info(self, *arg, **kwd):
```

### Comparing `plafosim-0.15.4/src/plafosim/vehicle.py` & `plafosim-0.16.0/src/plafosim/vehicle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -65,15 +67,15 @@
             depart_speed: float,
             depart_time: int,
             depart_delay: int,
             communication_range: int,
             pre_filled: bool = False,
     ):
         """
-        Initializes a vehicle instance.
+        Initialize a vehicle instance.
 
         Parameters
         ----------
         simulator : Simulator
             The global simulator object
         vid : int
             The id of the vehicle
@@ -142,185 +144,219 @@
             self._simulator._rng.randrange(0, 255, 1),
             self._simulator._rng.randrange(0, 255, 1),
             self._simulator._rng.randrange(0, 255, 1),
         )
 
     @property
     def vid(self) -> int:
-        """Return the id of the vehicle."""
+        """
+        Return the id of the vehicle.
+        """
 
         return self._vid
 
     @property
     def vehicle_type(self) -> VehicleType:
-        """Returns the VehicleType of the vehicle."""
+        """
+        Return the VehicleType of the vehicle.
+        """
 
         return self._vehicle_type
 
     @property
     def length(self) -> int:
         """
-        Returns the length of the vehicle.
+        Return the length of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._length
 
     @property
     def max_speed(self) -> float:
         """
-        Returns the maximum speed of the vehicle.
+        Return the maximum speed of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._max_speed
 
     @property
     def max_acceleration(self) -> float:
         """
-        Returns the maximum acceleration of the vehicle.
+        Return the maximum acceleration of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._max_acceleration
 
     @property
     def max_deceleration(self) -> float:
         """
-        Returns the maximum deceleration of the vehicle.
+        Return the maximum deceleration of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._max_deceleration
 
     @property
     def min_gap(self) -> float:
         """
-        Returns the minimum safety gap to the vehicle in front of the vehicle.
+        Return the minimum safety gap to the vehicle in front of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._min_gap
 
     @property
     def headway_time(self) -> float:
         """
-        Returns the human headway time of the vehicle.
+        Return the human headway time of the vehicle.
 
         This is based on the vehicle type.
         """
 
         return self._vehicle_type._headway_time
 
     @property
     def desired_headway_time(self) -> float:
-        """Returns the desired headway time of the vehicle."""
+        """
+        Return the desired headway time of the vehicle.
+        """
 
         return self._vehicle_type._headway_time
 
     @property
     def depart_position(self) -> int:
-        """Returns the depart position of the vehicle."""
+        """
+        Return the depart position of the vehicle.
+        """
 
         return self._depart_position
 
     @property
     def arrival_position(self) -> int:
-        """Returns the arrival position of the vehicle."""
+        """
+        Return the arrival position of the vehicle.
+        """
 
         return self._arrival_position
 
     @property
     def desired_speed(self) -> float:
-        """Returns the desired driving speed of the vehicle."""
+        """
+        Return the desired driving speed of the vehicle.
+        """
 
         return self._desired_speed
 
     @property
     def desired_gap(self) -> float:
         """
-        Returns the desired gap to the vehicle in front of the vehicle.
+        Return the desired gap to the vehicle in front of the vehicle.
 
         This is based on the desired headway time and the current driving speed.
         """
 
         # use potential other desired headway time
         # TODO should this be target speed?
         return speed2distance(self.desired_headway_time * self._speed, self._simulator._step_length)
 
     @property
     def depart_lane(self) -> int:
-        """Returns the depart lane of the vehicle."""
+        """
+        Return the depart lane of the vehicle.
+        """
 
         return self._depart_lane
 
     @property
     def depart_speed(self) -> float:
-        """Returns the depart speed of the vehicle."""
+        """
+        Return the depart speed of the vehicle.
+        """
 
         return self._depart_speed
 
     @property
     def depart_time(self) -> int:
-        """Returns the depart time of the vehicle."""
+        """
+        Return the depart time of the vehicle.
+        """
 
         return self._depart_time
 
     @property
     def position(self) -> float:
-        """Returns the current position of the vehicle."""
+        """
+        Return the current position of the vehicle.
+        """
 
         return self._position
 
     @property
     def rear_position(self) -> int:
-        """Returns the current rear position of the vehicle."""
+        """
+        Return the current rear position of the vehicle.
+        """
 
         position = self._position - self._vehicle_type._length
         assert position >= 0
         return position
 
     @property
     def lane(self) -> int:
-        """Returns the current lane of the vehicle."""
+        """
+        Return the current lane of the vehicle.
+        """
 
         return self._lane
 
     @property
     def speed(self) -> float:
-        """Returns the current driving speed of the vehicle."""
+        """
+        Return the current driving speed of the vehicle.
+        """
 
         return self._speed
 
     @property
     def cf_model(self) -> CF_Model:
-        """Returns the currently activated car following model of the vehicle."""
+        """
+        Return the currently activated car following model of the vehicle.
+        """
 
         return self._cf_model
 
     @property
     def travel_distance(self) -> float:
-        """Returns the current traveled distance of the vehicle."""
+        """
+        Return the current traveled distance of the vehicle.
+        """
 
         return self._position - self._depart_position
 
     @property
     def travel_time(self) -> float:
-        """Returns the current traveled time of the vehicle."""
+        """
+        Return the current traveled time of the vehicle.
+        """
 
         return self._simulator.step - self._depart_time
 
     @property
     def blocked_front(self) -> bool:
-        """Returns whether the vehicle is currently blocked by a slow vehicle in the front."""
+        """
+        Return whether the vehicle is currently blocked by a slow vehicle in the front.
+        """
 
         return self._blocked_front
 
     @property
     def color(self) -> tuple:
         """Return the current color of the vehicle."""
         return self._color
@@ -359,33 +395,39 @@
             The current simulation step
         """
 
         pass  # this vehicle has no application running
 
     # TODO: obsolete?
     def _start(self):
-        """Starts this Vehicle"""
+        """
+        Start this Vehicle.
+        """
 
         if self._started:
             return
 
         self._started = True
 
     def info(self) -> str:
-        """Returns information about the vehicle."""
+        """
+        Return information about the vehicle.
+        """
 
         estimated_remaining_travel_time = (
             (self._arrival_position - self._position) / self._speed
             if self._speed > 0
             else self.desired_speed  # use potential other desired driving speed
         )
         return f"{self._vid} at {self._position}-{self.rear_position}, {self._lane} with {self._speed}, takes {estimated_remaining_travel_time}s to reach {self._arrival_position}"
 
     def _statistics(self):
-        """Writes continuous statistics for the vehicle."""
+        """
+        Write continuous statistics for the vehicle.
+        """
 
         if not self._simulator._record_prefilled and self._depart_time == -1:
             # we do not record statistics for pre-filled vehicles
             return
 
         # calculate time loss
         # SUMO: "The time lost due to driving below the ideal speed."
@@ -400,15 +442,15 @@
 
         self._calculate_emissions()
 
         # TODO current gap to front
 
     def _calculate_emissions(self):
         """
-        Calculates the emitted pollutant amount using the given speed and acceleration based on the HBEFA3 model.
+        Calculate the emitted pollutant amount using the given speed and acceleration based on the HBEFA3 model.
 
         As the functions are defining emissions in g/hour, the function's result is normed
         by 3.6 (seconds in an hour/1000) yielding mg/s. For fuel ml/s is returned.
         Negative acceleration results directly in zero emission.
 
         The amount emitted by the given emission class when moving with the given velocity and acceleration [mg/s or ml/s]
         """
@@ -444,15 +486,15 @@
                 record_emission_trace_value(basename=self._simulator._result_base_filename, value=value)
 
         if self._simulator._record_emission_traces:
             record_emission_trace_suffix(basename=self._simulator._result_base_filename)
 
     def _calculate_emission(self, a: float, v: float, f: list, scale: float) -> float:
         """
-        Calculates the actual emission of the vehicle.
+        Calculate the actual emission of the vehicle.
 
         Parameters
         ----------
         a : float
             The current acceleration
         v : float
             The current speed
@@ -464,15 +506,15 @@
 
         if a < 0:
             return 0
         return max((f[0] + f[1] * a * v + f[2] * a * a * v + f[3] * v + f[4] * v * v + f[5] * v * v * v) / scale, 0.0)
 
     def finish(self):
         """
-        Cleans up the instance of the vehicle.
+        Clean up the instance of the vehicle.
 
         This includes mostly statistic recording.
         """
 
         if (self._position < self._arrival_position):
             LOG.warning(f"{self._vid}'s finish method was called even though vehicle did not arrive yet!")
             return
@@ -526,23 +568,25 @@
                 average_deviation_desired_speed=average_deviation_desired_speed,
             )
 
         if self._simulator._record_vehicle_emissions:
             record_vehicle_emission(basename=self._simulator._result_base_filename, vehicle=self)
 
     def __str__(self) -> str:
-        """Returns the str representation of the vehicle."""
+        """
+        Return the str representation of the vehicle.
+        """
 
         self_dict = self.__dict__.copy()
         self_dict.update({'_vehicle_type': str(self._vehicle_type)})  # use str representation of vehicle type
         return str(self_dict)
 
     def _transmit(self, destination_vid: int, message: Message) -> bool:
         """
-        Transmits a message of type Message.
+        Transmit a message of type Message.
 
         Messages are in general not used at the moment.
 
         Parameters
         ----------
         destination_vid : int
             The id of the destination vehicle
@@ -591,15 +635,15 @@
                 self._handle_message(message)
             # we cannot receive this message since it was not for us
             return False
         raise RuntimeError("Message is not an instance of type Message")
 
     def _handle_message(self, message: Message):
         """
-        Handles a message of arbitrary type Message.
+        Handle a message of arbitrary type Message.
 
         Messages are in general not used at the moment.
 
         Parameters
         ----------
         message : Message
             The message to be handled
@@ -609,15 +653,15 @@
 
         func = self.__class__.__dict__.get('_receive_' + message.__class__.__name__,
                                            lambda v, m: print("cannot handle message", m))
         return func(self, message)
 
     def _receive_Message(self, message: Message):
         """
-        Handles a message of the specific type Message.
+        Handle a message of the specific type Message.
 
         Messages are in general not used at the moment.
 
         Parameters
         ----------
         message : Message
             The message to be received
```

### Comparing `plafosim-0.15.4/src/plafosim/vehicle_type.py` & `plafosim-0.16.0/src/plafosim/vehicle_type.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 
-
 from .emissions import EmissionClass
 
 
 class VehicleType:
-    """A collection of parameters for a concrete vehicle type"""
+    """
+    A collection of parameters for a concrete vehicle type.
+    """
 
     def __init__(
             self, name: str,
             length: int,
             max_speed: float,
             max_acceleration: float,
             max_deceleration: float,
             min_gap: float,
             headway_time: float,
             emission_class: str,
     ):
         """
-        Initializes a specific vehicle type.
+        Initialize a specific vehicle type.
 
         Parameters
         ----------
         name : str
             The name of the vehicle type
         length : int
             The length of the vehicle type
@@ -62,63 +65,83 @@
         self._max_deceleration = max_deceleration  # the maximum deceleration of the vehicle type
         self._min_gap = min_gap  # the minimum gap to the vehicle in front
         self._headway_time = headway_time  # the desired human headway time
         self._emission_class = EmissionClass[emission_class]  # the emission class of the vehicle type
 
     @property
     def name(self) -> str:
-        """Returns the name of a vehicle type."""
+        """
+        Return the name of a vehicle type.
+        """
 
         return self._name
 
     @property
     def length(self) -> int:
-        """Returns the length of a vehicle type."""
+        """
+        Return the length of a vehicle type.
+        """
 
         return self._length
 
     @property
     def max_speed(self) -> float:
-        """Returns the maximum speed of a vehicle type."""
+        """
+        Return the maximum speed of a vehicle type.
+        """
 
         return self._max_speed
 
     @property
     def max_acceleration(self) -> float:
-        """Returns the maximum acceleration of a vehicle type."""
+        """
+        Return the maximum acceleration of a vehicle type.
+        """
 
         return self._max_acceleration
 
     @property
     def max_deceleration(self) -> float:
-        """Returns the maximum deceleration of a vehicle type."""
+        """
+        Return the maximum deceleration of a vehicle type.
+        """
 
         return self._max_deceleration
 
     @property
     def min_gap(self) -> float:
-        """Returns the minimum gap of a vehicle type."""
+        """
+        Return the minimum gap of a vehicle type.
+        """
 
         return self._min_gap
 
     @property
     def headway_time(self) -> float:
-        """Returns the desired human headway time of a vehicle type."""
+        """
+        Return the desired human headway time of a vehicle type.
+        """
 
         return self._headway_time
 
     @property
     def emission_class(self) -> EmissionClass:
-        """Returns the emission class of a vehicle type."""
+        """
+        Return the emission class of a vehicle type.
+        """
 
         return self._emission_class
 
     @property
     def emission_factors(self) -> dict:
-        """Returns the emission factors of a vehicle type."""
+        """
+        Return the emission factors of a vehicle type.
+        """
 
         return self._emission_class.emission_factors
 
     def __str__(self) -> str:
-        """Returns the str representation of a vehicle type."""
+        """
+        Return the str representation of a vehicle type.
+        """
 
         return str(self.__dict__)
```

### Comparing `plafosim-0.15.4/setup.py` & `plafosim-0.16.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 entry_points = \
 {'console_scripts': ['plafosim = plafosim.cli.plafosim:main',
                      'plafosim-replay = plafosim.cli.trace_replay:main']}
 
 setup_kwargs = {
     'name': 'plafosim',
-    'version': '0.15.4',
+    'version': '0.16.0',
     'description': 'A simple and scalable simulator for platoon formation.',
-    'long_description': '# Platoon Formation Simulator (PlaFoSim)\n\n[![Code Version](https://img.shields.io/badge/code-v0.15.4-blue)](CHANGELOG.md)\n[![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)\n[![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)\n[![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)\n\n[PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.\n\nPlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.\nWhile the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.\n\nConceptual view on the process of Platoon Formation:\n| Scenario | Advertisement | Assignment | Maneuver |\n| -------- | ------------- | ---------- | -------- |\n| ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |\n\nPlaFoSim is published here:\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.\n\nPlease note that PlaFoSim is still under heavy development.\n\n---\n\n## Installation\n\n- Install Python (>=3.7.0,<3.10)\n- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)\n- Install PlaFoSim via pypi:\n```pip install plafosim```\n\nNOTE: The project is currently only tested under Linux.\n\n## Running a Simulation\n\nYou can use the simulator as module as well as from the command-line.\nCurrently, only command-line is thoroughly tested and thus completely available though.\n\n### Quickstart\n\nUse PlaFoSim\'s binary to run a simulation with the default configuration:\n\n```plafosim -d```\n\n### Advanced Simulation Control\n\nYou can use a variety of different parameters to customize the scenario and the simulation itself.\nE.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:\n\n```plafosim --vehicles 1000```\n\nThe available parameters are grouped into different categories:\n\n```\n- road network properties\n- vehicle properties\n- trip properties\n- communication properties\n- platoon properties\n- formation properties\n- infrastructure properties\n- simulation properties\n- gui properties\n- result recording properties\n```\n\nYou can see the complete list of available parameters in the help:\n\n```plafosim -h, --help```\n\n### Examples\n\n```\n# Configure a 100km freeway with ramps at every 10km\nplafosim --road-length 100 --ramp-interval 10\n\n# Configure random (normally distributed) desired driving speed of 130km/h\nplafosim --random-desired-speed true --desired-speed 36\n\n# Configure random trips for 500 vehicles\nplafosim --vehicles 500 --random-depart-position true --random-arrival-position true --depart-desired true\n\n# Pre fill the freeway with 1000 vehicles\nplafosim --vehicles 1000 --pre-fill true\n\n# Configure 50% of the vehicles with Advanced Cruise Control (ACC) and a headway time of 1.5s\nplafosim --penetration 0.5 --acc-headway-time 1.5\n\n# Enable a simple, distributed platoon formation algorithm [1] in order to form platoons every 30s\nplafosim --formation-algorithm SpeedPosition --formation-strategy distributed --execution-interval 30\n```\n\n### Live GUI\n\nYou can get a very simple live GUI based on SUMO by using the parameter `gui` (requires installation of SUMO and decleration of `SUMO_HOME` variable):\n\n```plafosim --gui```\n\n![](docs/gui.png)\n*A screenshot of PlaFoSim\'s live GUI showing 2 platoons and various individual vehicles. Copyright © 2021 IEEE.*\n\nMore options for the live GUI can be found within the ``gui properties`` section of the help.\n\n### Faster Simulation\n\nYou can speed up the simulation performance by enabling Python\'s optimization ```PYTHONOPTIMIZE```, e.g., in order to disable assertions:\n\n```PYTHONOPTIMIZE=1 plafosim```\n\nSee the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.\n\n## Re-Playing a Simulation\n\nThe simulation can write a trace file for every simulated vehicle (default `results_vehicle_traces.csv`).\nYou can replay the simulation based on the trace file by using a corresponding binary:\n\n```plafosim-replay results_vehicle_traces.csv```\n\nTo see all options of this script, run:\n\n```plafosim-replay -h, --help```\n\n## Extending\n\n- Clone the repository\n- Install poetry\n```pip install poetry```\n- Install PlaFoSim from source in editable mode\n```poetry install```\n- Run PlaFoSim in the virtual environment with\n```poetry run plafosim```\nor activate the virtual enviroment first with\n```poetry shell```\nand run the commands as usual (see above)\n\nNOTE: The project is currently only tested under Linux.\n\nIn order to add a new formation algorithm, you need to follow these steps:\n- Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.\n- Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.\n- Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.\n- Import your algorithm and add parsing of its `__name__` to `__init__` within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).\n\nYou should now be able to use your new algorithm with\n```\nplafosim --formation-algorithm dummy_algorithm_name\n```\n\n## Contributing\n\nIn order to contribute, please follow these steps:\n- Install PlaFoSim from source (see above)\n- Make desired changes\n- Run the tests located in `scripts` (see `.drone.yml`)\n- Submit a Pull Request (PR)\n\n### Testing\n\nWhen adding methods and functions, make sure to add corresponding unit tests for `py.test`.\nThe tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.\nThis will also generate a test coverage report.\n\n### Validation\n\nTo validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).\nThe corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.\nYou can have a look at `.drone.yml` for details regarding the execution.\n\n## Contributors & Citing\n\nPlaFoSim was designed built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).\nIt is currently maintained by [Julian Heinovski](https://github.com/heinovski/).\nThe list of all authors can be found [here](AUTHORS.md).\n\nIf you are working with `PlaFoSim`, please cite the [following paper](https://www2.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.\n\n```bibtex\n@inproceedings{heinovski2021scalable,\n    author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},\n    title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},\n    publisher = {IEEE},\n    issn = {2157-9865},\n    isbn = {978-1-66544-450-7},\n    address = {Virtual Conference},\n    booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},\n    month = {11},\n    year = {2021},\n}\n```\n\n## License\n\nPlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.\n\n```\n# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>\n#\n# This program is free software: you can redistribute it and/or modify\n# it under the terms of the GNU General Public License as published by\n# the Free Software Foundation, either version 3 of the License, or\n# any later version.\n#\n# This program is distributed in the hope that it will be useful,\n# but WITHOUT ANY WARRANTY; without even the implied warranty of\n# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n# GNU General Public License for more details.\n#\n# You should have received a copy of the GNU General Public License\n# along with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\n## List of References\n\n[1] Julian Heinovski and Falko Dressler, "Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols," Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.\n',
+    'long_description': '# Platoon Formation Simulator (PlaFoSim)\n\n[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)\n[![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)\n[![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)\n[![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)\n\n[PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.\n\nPlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.\nWhile the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.\n\nConceptual view on the process of Platoon Formation [1-2]:\n| Scenario | Advertisement | Assignment | Maneuver |\n| -------- | ------------- | ---------- | -------- |\n| ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |\n\nPlaFoSim is published [here](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\nPlease note that PlaFoSim is still under heavy development.\n\n---\n\n## Installation\n\n- Install Python (>=3.7.0,<3.10)\n- Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)\n- Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):\n```pip install plafosim```\n\nNOTE: The project is currently only tested under Linux.\n\n## Running a Simulation\n\nYou can use the simulator as module as well as from the command-line.\nCurrently, only command-line is thoroughly tested and thus completely available though.\n\n### Quickstart\n\nUse PlaFoSim\'s binary to run a simulation with the default configuration:\n\n```plafosim -d```\n\n### Advanced Simulation Control\n\nYou can use a variety of different parameters to customize the scenario and the simulation itself.\nE.g., use the parameter `vehicles` to configure the number of vehicles in the simulation:\n\n```plafosim --vehicles 1000```\n\nThe available parameters are grouped into different categories:\n\n```\n- road network properties\n- vehicle properties\n- trip properties\n- communication properties\n- platoon properties\n- formation properties\n- infrastructure properties\n- simulation properties\n- GUI properties\n- result recording properties\n```\n\nYou can see the complete list of available parameters in the help:\n\n```plafosim -h, --help```\n\n### Examples\n\n```\n# Configure a 100km freeway with ramps at every 10km\nplafosim --road-length 100 --ramp-interval 10\n\n# Configure random (normally distributed) desired driving speed of 130km/h\nplafosim --random-desired-speed true --desired-speed 36\n\n# Configure random trips for 500 vehicles\nplafosim --vehicles 500 --random-depart-position true --random-arrival-position true --depart-desired true\n\n# Pre fill the freeway with 1000 vehicles\nplafosim --vehicles 1000 --pre-fill true\n\n# Configure 50% of the vehicles with Advanced Cruise Control (ACC) and a headway time of 1.5s\nplafosim --penetration 0.5 --acc-headway-time 1.5\n\n# Enable a simple, distributed platoon formation algorithm [1] in order to form platoons every 30s\nplafosim --formation-algorithm SpeedPosition --formation-strategy distributed --execution-interval 30\n```\n\n### Live GUI\n\nYou can get a very simple live GUI based on SUMO by using the parameter `gui` (requires installation of SUMO and decleration of `SUMO_HOME` variable):\n\n```plafosim --gui```\n\n![](docs/gui.png)\n*A screenshot of PlaFoSim\'s live GUI showing 2 platoons and various individual vehicles. Copyright © 2021 IEEE.*\n\nMore options for the live GUI can be found within the ``gui properties`` section of the help.\n\n### Faster Simulation\n\nYou can speed up the simulation performance by enabling Python\'s optimization ```PYTHONOPTIMIZE```, e.g., in order to disable assertions:\n\n```PYTHONOPTIMIZE=1 plafosim```\n\nSee the Python [documention](https://docs.python.org/3/using/cmdline.html#envvar-PYTHONOPTIMIZE) for more details.\n\n## Re-Playing a Simulation\n\nThe simulation can write a trace file for every simulated vehicle (default `results_vehicle_traces.csv`).\nYou can replay the simulation based on the trace file by using a corresponding binary:\n\n```plafosim-replay results_vehicle_traces.csv```\n\nTo see all options of this script, run:\n\n```plafosim-replay -h, --help```\n\n## Extending\n\n- Clone the repository\n- Install [poetry](https://python-poetry.org/):\n```pip install poetry```\n- Install PlaFoSim from source in editable mode:\n```poetry install```\n- Run PlaFoSim in the virtual environment with\n```poetry run plafosim```\nor activate the virtual enviroment first with\n```poetry shell```\nand run the commands as usual (see above)\n\nNOTE: The project is currently only tested under Linux.\n\nIn order to add a new formation algorithm, you need to follow these steps:\n- Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.\n- Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.\n- Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.\n- Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).\n\nYou should now be able to use your new algorithm with\n```\nplafosim --formation-algorithm dummy_algorithm_name\n```\n\n## Contributing\n\nIn order to contribute, please follow these steps:\n- Install PlaFoSim from source (see above)\n- Make desired changes\n- Run the tests located in `scripts` (see `.drone.yml`)\n- Submit a Pull Request (PR)\n\n### Testing\n\nWhen adding methods and functions, make sure to add corresponding unit tests for `py.test`.\nThe tests are located under `tests` and can be executed with `./scripts/run-pytest.sh`.\nThis will also generate a test coverage report.\n\n### Validation\n\nTo validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).\nThe corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.\nYou can have a look at `.drone.yml` for details regarding the execution.\n\n### Profiling\n\nYou can profile the runtime of PlaFoSim\'s code by using [cProfile](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```poetry run python -m cProfile -o profile.out -m plafosim.cli.plafosim```\n\nYou can visualize the results of the profiling run by using [SnakeViz](https://docs.python.org/3/library/profile.html#module-cProfile):\n\n```snakeviz profile.out```\n\n## Contributors & Citing\n\nPlaFoSim was designed and built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).\nIt is currently maintained by [Julian Heinovski](https://github.com/heinovski/).\nThe list of all authors can be found [here](AUTHORS.md).\n\nIf you are working with `PlaFoSim`, please cite the [following paper](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):\n\n> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.\n\n```bibtex\n@inproceedings{heinovski2021scalable,\n    author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},\n    doi = {10.1109/VNC52810.2021.9644678},\n    title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},\n    pages = {137--138},\n    publisher = {IEEE},\n    issn = {2157-9865},\n    isbn = {978-1-66544-450-7},\n    address = {Virtual Conference},\n    booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},\n    month = {11},\n    year = {2021},\n}\n```\n\n## License\n\nPlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.\n\n```\n# Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>\n#\n# SPDX-License-Identifier: GPL-3.0-or-later\n#\n# This program is free software: you can redistribute it and/or modify\n# it under the terms of the GNU General Public License as published by\n# the Free Software Foundation, either version 3 of the License, or\n# any later version.\n#\n# This program is distributed in the hope that it will be useful,\n# but WITHOUT ANY WARRANTY; without even the implied warranty of\n# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\n# GNU General Public License for more details.\n#\n# You should have received a copy of the GNU General Public License\n# along with this program.  If not, see <https://www.gnu.org/licenses/>.\n```\n\n## List of References\n\n[1] Julian Heinovski and Falko Dressler, ["Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols,"](https://www.tkn.tu-berlin.de/bib/heinovski2018platoon/) Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.\n\n[2] Julian Heinovski, ["Platoon Formation: Car-to-Platoon Assignments for Individual Cars,"](https://www.tkn.tu-berlin.de/bib/heinovski2019platoon/) Proceedings of International Conference on Networked Systems (NetSys 2019), PhD Forum, Munich, Germany, March 2019.\n',
     'author': 'Julian Heinovski',
     'author_email': 'heinovski@ccs-labs.org',
     'maintainer': 'Julian Heinovski',
     'maintainer_email': 'heinovski@ccs-labs.org',
     'url': 'https://www.plafosim.de',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `plafosim-0.15.4/PKG-INFO` & `plafosim-0.16.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plafosim
-Version: 0.15.4
+Version: 0.16.0
 Summary: A simple and scalable simulator for platoon formation.
 Home-page: https://www.plafosim.de
 License: GPL-3.0-or-later
 Author: Julian Heinovski
 Author-email: heinovski@ccs-labs.org
 Maintainer: Julian Heinovski
 Maintainer-email: heinovski@ccs-labs.org
@@ -25,43 +25,43 @@
 Project-URL: Changelog, https://github.com/heinovski/plafosim/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://plafosim.readthedocs.io/
 Project-URL: Repository, https://github.com/heinovski/plafosim
 Description-Content-Type: text/markdown
 
 # Platoon Formation Simulator (PlaFoSim)
 
-[![Code Version](https://img.shields.io/badge/code-v0.15.4-blue)](CHANGELOG.md)
+[![Code Version](https://img.shields.io/badge/code-v0.16.0-blue)](CHANGELOG.md)
 [![PyPI Version](https://img.shields.io/pypi/v/plafosim)](https://pypi.org/project/plafosim/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plafosim)](https://pypi.org/project/plafosim/)
 [![License](https://img.shields.io/github/license/heinovski/plafosim?color=green)](https://github.com/heinovski/plafosim)
 [![DOI](https://img.shields.io/badge/DOI-10.1109/VNC52810.2021.9644678-blue)](http://dx.doi.org/10.1109/VNC52810.2021.9644678)
 
 [PlaFoSim](https://www.plafosim.de) - A simple and scalable simulator for platoon formation.
 
 PlaFoSim aims to facilitate and accelerate the research of platoon maneuvers and formation for individually driven vehicles.
 While the main focus of the simulator is on the assignment process, simulation of advertisements and maneuvers is implemented in a more abstract way.
 
-Conceptual view on the process of Platoon Formation:
+Conceptual view on the process of Platoon Formation [1-2]:
 | Scenario | Advertisement | Assignment | Maneuver |
 | -------- | ------------- | ---------- | -------- |
 | ![Scenario](docs/scenario.png)*A new vehicle enters the highway.* | ![Advertisement](docs/advertisement.png)*The vehicle advertises itself as interested in Platooning.* | ![Assignment](docs/assignment.png)*A Vehicle-to-Platoon assignment is calculated.* | ![Maneuver](docs/maneuver.png)*The new vehicle performs a join maneuver.* |
 
-PlaFoSim is published here:
+PlaFoSim is published [here](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):
 
-> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.
+> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.
 
 Please note that PlaFoSim is still under heavy development.
 
 ---
 
 ## Installation
 
 - Install Python (>=3.7.0,<3.10)
 - Optionally, install [SUMO](https://github.com/eclipse/sumo/) (>=1.6.0)
-- Install PlaFoSim via pypi:
+- Install PlaFoSim from [pypi](https://pypi.org/project/plafosim/):
 ```pip install plafosim```
 
 NOTE: The project is currently only tested under Linux.
 
 ## Running a Simulation
 
 You can use the simulator as module as well as from the command-line.
@@ -87,15 +87,15 @@
 - vehicle properties
 - trip properties
 - communication properties
 - platoon properties
 - formation properties
 - infrastructure properties
 - simulation properties
-- gui properties
+- GUI properties
 - result recording properties
 ```
 
 You can see the complete list of available parameters in the help:
 
 ```plafosim -h, --help```
 
@@ -150,31 +150,31 @@
 To see all options of this script, run:
 
 ```plafosim-replay -h, --help```
 
 ## Extending
 
 - Clone the repository
-- Install poetry
+- Install [poetry](https://python-poetry.org/):
 ```pip install poetry```
-- Install PlaFoSim from source in editable mode
+- Install PlaFoSim from source in editable mode:
 ```poetry install```
 - Run PlaFoSim in the virtual environment with
 ```poetry run plafosim```
 or activate the virtual enviroment first with
 ```poetry shell```
 and run the commands as usual (see above)
 
 NOTE: The project is currently only tested under Linux.
 
 In order to add a new formation algorithm, you need to follow these steps:
 - Create a new sub-class of `FormationAlgorithm` (see `formation_algorithm.py`). You can use the `Dummy` algorithm (see `algorithms/dummy.py`) as an example.
 - Import your algorithm and add its `__name__` to the list of available algorithms (see `--formation-algorithm`) within `cli/plafosim.py`.
 - Add specific properties of your algorithm via an argument parser group to `cli/plafosim.py` if necessary.
-- Import your algorithm and add parsing of its `__name__` to `__init__` within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
+- Import your algorithm within `PlatooningVehicle` (see `platooning_vehicle.py`) and/or `Infrastructure` (see `infrastructure.py`).
 
 You should now be able to use your new algorithm with
 ```
 plafosim --formation-algorithm dummy_algorithm_name
 ```
 
 ## Contributing
@@ -193,28 +193,40 @@
 
 ### Validation
 
 To validate the behavior of PlaFoSim, it is compared to SUMO 1.6.0 by means of simulation results (e.g., vehicle traces).
 The corresponding scripts are located under `scripts` and executed withn CI/CD pipelines.
 You can have a look at `.drone.yml` for details regarding the execution.
 
+### Profiling
+
+You can profile the runtime of PlaFoSim's code by using [cProfile](https://docs.python.org/3/library/profile.html#module-cProfile):
+
+```poetry run python -m cProfile -o profile.out -m plafosim.cli.plafosim```
+
+You can visualize the results of the profiling run by using [SnakeViz](https://docs.python.org/3/library/profile.html#module-cProfile):
+
+```snakeviz profile.out```
+
 ## Contributors & Citing
 
-PlaFoSim was designed built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).
+PlaFoSim was designed and built by [Julian Heinovski](https://github.com/heinovski/) with the help of [Dominik S. Buse](https://github.com/dbuse/).
 It is currently maintained by [Julian Heinovski](https://github.com/heinovski/).
 The list of all authors can be found [here](AUTHORS.md).
 
-If you are working with `PlaFoSim`, please cite the [following paper](https://www2.tkn.tu-berlin.de/bib/heinovski2021scalable/):
+If you are working with `PlaFoSim`, please cite the [following paper](https://www.tkn.tu-berlin.de/bib/heinovski2021scalable/):
 
-> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021.
+> Julian Heinovski, Dominik S. Buse and Falko Dressler, "Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim," Proceedings of 13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session, Virtual Conference, November 2021, pp. 137–138.
 
 ```bibtex
 @inproceedings{heinovski2021scalable,
     author = {Heinovski, Julian and Buse, Dominik S. and Dressler, Falko},
+    doi = {10.1109/VNC52810.2021.9644678},
     title = {{Scalable Simulation of Platoon Formation Maneuvers with PlaFoSim}},
+    pages = {137--138},
     publisher = {IEEE},
     issn = {2157-9865},
     isbn = {978-1-66544-450-7},
     address = {Virtual Conference},
     booktitle = {13th IEEE Vehicular Networking Conference (VNC 2021), Poster Session},
     month = {11},
     year = {2021},
@@ -224,14 +236,16 @@
 ## License
 
 PlaFoSim is licensed under the terms of the GNU General Public License 3.0 or later.
 
 ```
 # Copyright (c) 2020-2022 Julian Heinovski <heinovski@ccs-labs.org>
 #
+# SPDX-License-Identifier: GPL-3.0-or-later
+#
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # any later version.
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
@@ -240,9 +254,11 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ```
 
 ## List of References
 
-[1] Julian Heinovski and Falko Dressler, "Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols," Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.
+[1] Julian Heinovski and Falko Dressler, ["Platoon Formation: Optimized Car to Platoon Assignment Strategies and Protocols,"](https://www.tkn.tu-berlin.de/bib/heinovski2018platoon/) Proceedings of 10th IEEE Vehicular Networking Conference (VNC 2018), Taipei, Taiwan, December 2018.
+
+[2] Julian Heinovski, ["Platoon Formation: Car-to-Platoon Assignments for Individual Cars,"](https://www.tkn.tu-berlin.de/bib/heinovski2019platoon/) Proceedings of International Conference on Networked Systems (NetSys 2019), PhD Forum, Munich, Germany, March 2019.
```

