# Comparing `tmp/nbt_structure_utils-0.2.0.tar.gz` & `tmp/nbt_structure_utils-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbt_structure_utils-0.2.0.tar", max compression
+gzip compressed data, was "nbt_structure_utils-0.3.0.tar", max compression
```

## Comparing `nbt_structure_utils-0.2.0.tar` & `nbt_structure_utils-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/LICENSE
--rw-r--r--   0        0        0     2207 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/README.md
--rw-r--r--   0        0        0      323 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/__init__.py
--rw-r--r--   0        0        0     4954 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/blocks.py
--rw-r--r--   0        0        0       18 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/entities.py
--rw-r--r--   0        0        0     6686 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/items.py
--rw-r--r--   0        0        0    27332 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/nbt_structure.py
--rw-r--r--   0        0        0    14332 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/nbt_structure_utils/shapes.py
--rw-r--r--   0        0        0     2308 2023-04-24 03:34:12.284656 nbt_structure_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3431 1970-01-01 00:00:00.000000 nbt_structure_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2263 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/README.md
+-rw-r--r--   0        0        0      323 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/__init__.py
+-rw-r--r--   0        0        0     2226 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/block_state_transformations.py
+-rw-r--r--   0        0        0    10196 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/blocks.py
+-rw-r--r--   0        0        0       18 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/entities.py
+-rw-r--r--   0        0        0     6686 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/items.py
+-rw-r--r--   0        0        0    29916 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/nbt_structure.py
+-rw-r--r--   0        0        0    14332 2023-04-28 05:01:01.217349 nbt_structure_utils-0.3.0/nbt_structure_utils/shapes.py
+-rw-r--r--   0        0        0     2326 2023-04-28 05:01:01.221349 nbt_structure_utils-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3526 1970-01-01 00:00:00.000000 nbt_structure_utils-0.3.0/PKG-INFO
```

### Comparing `nbt_structure_utils-0.2.0/LICENSE` & `nbt_structure_utils-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nbt_structure_utils-0.2.0/README.md` & `nbt_structure_utils-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-# NBTStructureUtils
+# NBT Structure Utils
 
 > A python library to create and edit NBT structure files for Minecraft.
 
-This has been tested with Minecraft version 1.19.3.
+This has been tested with Minecraft Java, version 1.19.3.
 
 **Features**
 
 - Create, read, and edit NBT structure files.
 - Methods inspired by Minecraft's fill, setblock, and clone commands.
 - Edit the state, inventory, and NBT data of blocks.
 - Special classes to help fill Cuboids and draw straight lines.
 
 ## Basic Usage
+See class docstrings for finer details and lists of methods.
+
 ### Minecraft NBT Structure
 This library creates .nbt files that can be placed in minecraft worlds. with a Structure Block or structure command. 
 
 See the minecraft wiki for details on each:
 - [Structure Block](https://minecraft.fandom.com/wiki/Structure_Block)
 - [structure Command](https://minecraft.fandom.com/wiki/Commands/structure)
 
 
 ### Edit blocks
-Basic Example: create a 5x5x5 hollow cube of stone and save to file:
+Basic Example: create a 5x5x5 cube of stone and save to file:
 ```python
 from nbt_structure_utils import NBTStructure, Vector, Cuboid, BlockData
 nbtstructure = NBTStructure()
 c1, c2 = Vector(0, 0, 0), Vector(4, 4, 4)
-nbtstructure.fill_hollow(Cuboid(c1, c2), BlockData("stone"))
+nbtstructure.fill(Cuboid(c1, c2), BlockData("stone"))
 nbtstructure.get_nbt().write_file(filename="path/to/output/hollow_box.nbt")
 ```
 
 ### Read and Edit 
 You can load and edit NBT structures created by this library or by Minecraft. All or part of a structure can also be cloned into other structures.
 
 Example: Load from disk and mirror the structure to be upside down:
```

### Comparing `nbt_structure_utils-0.2.0/nbt_structure_utils/items.py` & `nbt_structure_utils-0.3.0/nbt_structure_utils/items.py`

 * *Files identical despite different names*

### Comparing `nbt_structure_utils-0.2.0/nbt_structure_utils/nbt_structure.py` & `nbt_structure_utils-0.3.0/nbt_structure_utils/nbt_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 from collections.abc import Iterable
 from contextlib import suppress
 
+import numpy as np
 from nbt.nbt import NBTFile, TAG_Compound, TAG_Int, TAG_List, TAG_String
 
-from .blocks import BlockData
+from .blocks import X_AXIS, Y_AXIS, Z_AXIS, BlockData
 from .items import Inventory
 from .shapes import Cuboid, IVolume, Vector
 
 AIR_BLOCK = BlockData("minecraft:air")
 EMPTY_SPACE = None
 DATAVERSION = 3218
 
@@ -19,14 +20,15 @@
     Methods:
         get_state(block): Get index of state that matches block.
         try_get_state(block): Get index of state that matches block, else None.
         try_append(block): Add block if not in palette.
         extend(blocks): Adds any blocks not in palette.
         copy(): Return a copy of this palette.
         reflect(reflector): Reflect block states across different planes.
+        rotate(axis, angle): Rotate all states by angle around specified axis.
         get_nbt(): Get TAG_List representation of palette.
     """
 
     __blocks: "list[BlockData]"
 
     def __init__(self, block_data: "Iterable[BlockData]" = []) -> None:
         self.__blocks = [b.copy() for b in block_data]
@@ -109,14 +111,24 @@
         for block in self.__blocks:
             block.reflect(
                 reflector.x is not None,
                 reflector.y is not None,
                 reflector.z is not None,
             )
 
+    def rotate(self, axis: str, angle: int) -> None:
+        """Rotate all states by angle around specified axis.
+
+        Args:
+            axis (str): The axis to rotate around
+            angle (int): The angle in degrees.
+        """
+        for block in self.__blocks:
+            block.rotate(axis, angle)
+
 
 class BlockPosition:
     """For use in NBTStructure. Stores block position, state from Palette, and inventory.
 
     Attributes:
         pos (Vector): x,y,z location of block.
         state (int): state id from the palette.
@@ -238,14 +250,16 @@
     Bulk Update Methods:
         crop(volume):
             Remove blocks outside of volume.
         translate(delta):
             Move entire structure by some distance.
         reflect(reflector):
             Mirror the structure over specific planes.
+        rotate(axis, angle):
+            Rotate all positions and states by angle around specified axis
         pressurize(volume):
             Replace all empty spaces with air blocks.
         depressurize(volume):
             Replace all air blocks with empty spaces.
 
     Static Methods:
         load_from_nbt(nbt): Loads an NBT file from disk into self.
@@ -318,36 +332,41 @@
                 if not other_nbt.tags:
                     other_nbt = None
             block = BlockPosition(pos, b["state"].value, inv, other_nbt)
             structure.__set_block(block)
         return structure
 
     def get_nbt(
-        self, pressurize: bool = True, trim_excess_air: bool = False
+        self,
+        pressurize: bool = True,
+        trim_excess_air: bool = False,
+        align_to_origin: bool = True,
     ) -> NBTFile:
         """Create NBTFile representation of self.
 
         Can be saved to disk then loaded into Minecraft via a structure block. Default args will save like a structure block would.
 
         Args:
             pressurize (bool, optional): Replace empty space with air blocks. Defaults to True.
             trim_excess_air (bool, optional): Minimize size by removing air outside of smallest cuboid. Defaults to False.
+            align_to_origin (bool, optional): Move all blocks so that the minimum corner is at 0,0,0
 
         Returns:
             NBTFile: the complete NBT representation of the structure.
         """
         # prepare and clean up copy
         working_copy = self.copy()
         min_coords = working_copy.get_min_coords(include_air=not trim_excess_air)
         max_coords = working_copy.get_max_coords(include_air=not trim_excess_air)
         if trim_excess_air:
             working_copy.crop(Cuboid(min_coords, max_coords))
         if pressurize:
             working_copy.pressurize(Cuboid(min_coords, max_coords))
-        working_copy.translate(min_coords * -1)
+        if align_to_origin:
+            working_copy.translate(min_coords * -1)
         working_copy.cleanse_palette()
 
         # generate file from copy
         structure_file = NBTFile()
         size = max_coords - min_coords + Vector(1, 1, 1)
         structure_file.tags.append(size.get_nbt("size"))
         structure_file.tags.append(TAG_List(name="entities", type=TAG_Compound))
@@ -538,14 +557,54 @@
             new_pos.x = 2 * reflector.x - pos.x
         if reflector.y is not None:
             new_pos.y = 2 * reflector.y - pos.y
         if reflector.z is not None:
             new_pos.z = 2 * reflector.z - pos.z
         return new_pos
 
+    def rotate(self, axis: str, angle: int) -> None:
+        """Rotate the blocks and states around an axis by an angle.
+
+        The positive angle direction is determined by the right-hand rule, unlike Minecraft.
+        This means 90 degrees here is 270 in the structure block UI and vice versa.
+        Facing directly east (+x), up (+y), or south (+z), positive rotation is clockwise.
+
+        Parameters:
+            axis(str): Choose to rotate around the x,y or z azis.
+            angle(int): Rotation angle, in degrees. Must be multiple of 90.
+        """
+        if axis not in [X_AXIS, Y_AXIS, Z_AXIS]:
+            raise ValueError("Must choose valid axis")
+        if not angle % 90 == 0:
+            raise ValueError("Must choose multiple of 90 degrees.")
+        angle = angle % 360
+        if angle == 0:
+            return
+        rotation: "dict(int,BlockPosition)" = {}
+        for block in self.blocks.values():
+            new_pos = self.__get_rotated_pos(block.pos, axis, angle)
+            block.pos = new_pos
+            rotation[new_pos] = block
+        self.blocks = rotation
+        self.palette.rotate(axis, angle)
+
+    def __get_rotated_pos(self, pos: Vector, axis: str, angle: int) -> Vector:
+        """Hit it with a rotation matrix."""
+        original_pos = np.array((pos.x, pos.y, pos.z))
+        theta = np.radians(angle)
+        c, s = np.cos(theta), np.sin(theta)
+        if axis == X_AXIS:
+            rotation_matrix = np.array([(1, 0, 0), (0, c, -s), (0, s, c)], dtype=int)
+        if axis == Y_AXIS:
+            rotation_matrix = np.array([(c, 0, s), (0, 1, 0), (-s, 0, c)], dtype=int)
+        if axis == Z_AXIS:
+            rotation_matrix = np.array([(c, -s, 0), (s, c, 0), (0, 0, 1)], dtype=int)
+        new_pos = np.matmul(rotation_matrix, original_pos)
+        return Vector(new_pos[0], new_pos[1], new_pos[2])
+
     def clone_structure(
         self,
         other: "NBTStructure",
         dest: Vector,
         source_volume: "Iterable[Vector]" = None,
     ) -> None:
         """Clone blocks from another structure to this one.
```

### Comparing `nbt_structure_utils-0.2.0/nbt_structure_utils/shapes.py` & `nbt_structure_utils-0.3.0/nbt_structure_utils/shapes.py`

 * *Files identical despite different names*

### Comparing `nbt_structure_utils-0.2.0/pyproject.toml` & `nbt_structure_utils-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nbt-structure-utils"
-version = "0.2.0"
+version = "0.3.0"
 description = "Create, read, and edit Minecraft NBT structure files."
 authors = ["Ben Burton <benjaminburtondev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nbt_structure_utils"}]
 homepage = "https://github.com/BenBenBenB/nbt-structure-utils"
 repository = "https://github.com/BenBenBenB/nbt-structure-utils"
@@ -24,14 +24,15 @@
     "Topic :: Games/Entertainment",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 nbt ="^1.5.1"
+numpy = "^1.24.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 black = "^23.3.0"
 isort = "^5.12.0"
 bandit = "^1.7.5"
```

### Comparing `nbt_structure_utils-0.2.0/PKG-INFO` & `nbt_structure_utils-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbt-structure-utils
-Version: 0.2.0
+Version: 0.3.0
 Summary: Create, read, and edit Minecraft NBT structure files.
 Home-page: https://github.com/BenBenBenB/nbt-structure-utils
 License: MIT
 Keywords: minecraft,nbt-structure,nbt
 Author: Ben Burton
 Author-email: benjaminburtondev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -20,46 +20,49 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: nbt (>=1.5.1,<2.0.0)
+Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Project-URL: Repository, https://github.com/BenBenBenB/nbt-structure-utils
 Description-Content-Type: text/markdown
 
-# NBTStructureUtils
+# NBT Structure Utils
 
 > A python library to create and edit NBT structure files for Minecraft.
 
-This has been tested with Minecraft version 1.19.3.
+This has been tested with Minecraft Java, version 1.19.3.
 
 **Features**
 
 - Create, read, and edit NBT structure files.
 - Methods inspired by Minecraft's fill, setblock, and clone commands.
 - Edit the state, inventory, and NBT data of blocks.
 - Special classes to help fill Cuboids and draw straight lines.
 
 ## Basic Usage
+See class docstrings for finer details and lists of methods.
+
 ### Minecraft NBT Structure
 This library creates .nbt files that can be placed in minecraft worlds. with a Structure Block or structure command. 
 
 See the minecraft wiki for details on each:
 - [Structure Block](https://minecraft.fandom.com/wiki/Structure_Block)
 - [structure Command](https://minecraft.fandom.com/wiki/Commands/structure)
 
 
 ### Edit blocks
-Basic Example: create a 5x5x5 hollow cube of stone and save to file:
+Basic Example: create a 5x5x5 cube of stone and save to file:
 ```python
 from nbt_structure_utils import NBTStructure, Vector, Cuboid, BlockData
 nbtstructure = NBTStructure()
 c1, c2 = Vector(0, 0, 0), Vector(4, 4, 4)
-nbtstructure.fill_hollow(Cuboid(c1, c2), BlockData("stone"))
+nbtstructure.fill(Cuboid(c1, c2), BlockData("stone"))
 nbtstructure.get_nbt().write_file(filename="path/to/output/hollow_box.nbt")
 ```
 
 ### Read and Edit 
 You can load and edit NBT structures created by this library or by Minecraft. All or part of a structure can also be cloned into other structures.
 
 Example: Load from disk and mirror the structure to be upside down:
```

