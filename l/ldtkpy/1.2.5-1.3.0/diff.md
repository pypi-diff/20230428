# Comparing `tmp/ldtkpy-1.2.5.tar.gz` & `tmp/ldtkpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldtkpy-1.2.5.tar", max compression
+gzip compressed data, was "ldtkpy-1.3.0.tar", max compression
```

## Comparing `ldtkpy-1.2.5.tar` & `ldtkpy-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0      308 2022-02-03 10:22:47.991714 ldtkpy-1.2.5/README.md
--rw-r--r--   0        0        0        0 2022-02-03 10:11:07.206545 ldtkpy-1.2.5/ldtkpy/__init__.py
--rw-r--r--   0        0        0   132112 2023-02-18 10:16:12.297741 ldtkpy-1.2.5/ldtkpy/api.py
--rw-r--r--   0        0        0      428 2023-02-18 10:15:38.113548 ldtkpy-1.2.5/pyproject.toml
--rw-r--r--   0        0        0      841 2023-02-18 10:18:58.599782 ldtkpy-1.2.5/setup.py
--rw-r--r--   0        0        0     1098 2023-02-18 10:18:58.600062 ldtkpy-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      308 2022-02-03 10:22:47.991714 ldtkpy-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2022-02-03 10:11:07.206545 ldtkpy-1.3.0/ldtkpy/__init__.py
+-rw-r--r--   0        0        0   136101 2023-04-28 02:31:55.505545 ldtkpy-1.3.0/ldtkpy/api.py
+-rw-r--r--   0        0        0      428 2023-04-28 02:32:20.865398 ldtkpy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 ldtkpy-1.3.0/PKG-INFO
```

### Comparing `ldtkpy-1.2.5/ldtkpy/api.py` & `ldtkpy-1.3.0/ldtkpy/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,21 +31,21 @@
         try:
             return f(x)
         except:
             pass
     assert False
 
 
-def from_bool(x: Any) -> bool:
-    assert isinstance(x, bool)
+def from_int(x: Any) -> int:
+    assert isinstance(x, int) and not isinstance(x, bool)
     return x
 
 
-def from_int(x: Any) -> int:
-    assert isinstance(x, int) and not isinstance(x, bool)
+def from_bool(x: Any) -> bool:
+    assert isinstance(x, bool)
     return x
 
 
 def from_float(x: Any) -> float:
     assert isinstance(x, (float, int)) and not isinstance(x, bool)
     return float(x)
 
@@ -94,32 +94,34 @@
         result: dict = {}
         result["command"] = from_str(self.command)
         result["when"] = to_enum(When, self.when)
         return result
 
 
 class AllowedRefs(Enum):
-    """Possible values: `Any`, `OnlySame`, `OnlyTags`"""
+    """Possible values: `Any`, `OnlySame`, `OnlyTags`, `OnlySpecificEntity`"""
 
     ANY = "Any"
     ONLY_SAME = "OnlySame"
+    ONLY_SPECIFIC_ENTITY = "OnlySpecificEntity"
     ONLY_TAGS = "OnlyTags"
 
 
 class EditorDisplayMode(Enum):
-    """Possible values: `Hidden`, `ValueOnly`, `NameAndValue`, `EntityTile`, `Points`,
-    `PointStar`, `PointPath`, `PointPathLoop`, `RadiusPx`, `RadiusGrid`,
+    """Possible values: `Hidden`, `ValueOnly`, `NameAndValue`, `EntityTile`, `LevelTile`,
+    `Points`, `PointStar`, `PointPath`, `PointPathLoop`, `RadiusPx`, `RadiusGrid`,
     `ArrayCountWithLabel`, `ArrayCountNoLabel`, `RefLinkBetweenPivots`,
     `RefLinkBetweenCenters`
     """
 
     ARRAY_COUNT_NO_LABEL = "ArrayCountNoLabel"
     ARRAY_COUNT_WITH_LABEL = "ArrayCountWithLabel"
     ENTITY_TILE = "EntityTile"
     HIDDEN = "Hidden"
+    LEVEL_TILE = "LevelTile"
     NAME_AND_VALUE = "NameAndValue"
     POINTS = "Points"
     POINT_PATH = "PointPath"
     POINT_PATH_LOOP = "PointPathLoop"
     POINT_STAR = "PointStar"
     RADIUS_GRID = "RadiusGrid"
     RADIUS_PX = "RadiusPx"
@@ -171,16 +173,17 @@
     instead of "*String*" when relevant.
     """
     type: str
     """Optional list of accepted file extensions for FilePath value type. Includes the dot:
     `.ext`
     """
     accept_file_types: Optional[List[str]]
-    """Possible values: `Any`, `OnlySame`, `OnlyTags`"""
+    """Possible values: `Any`, `OnlySame`, `OnlyTags`, `OnlySpecificEntity`"""
     allowed_refs: AllowedRefs
+    allowed_refs_entity_uid: Optional[int]
     allowed_ref_tags: List[str]
     allow_out_of_level_ref: bool
     """Array max length"""
     array_max_length: Optional[int]
     """Array min length"""
     array_min_length: Optional[int]
     auto_chain_ref: bool
@@ -192,22 +195,23 @@
     default_override: Any
     """User defined documentation for this field to provide help/tips to level designers about
     accepted values.
     """
     doc: Optional[str]
     editor_always_show: bool
     editor_cut_long_values: bool
-    """Possible values: `Hidden`, `ValueOnly`, `NameAndValue`, `EntityTile`, `Points`,
-    `PointStar`, `PointPath`, `PointPathLoop`, `RadiusPx`, `RadiusGrid`,
+    """Possible values: `Hidden`, `ValueOnly`, `NameAndValue`, `EntityTile`, `LevelTile`,
+    `Points`, `PointStar`, `PointPath`, `PointPathLoop`, `RadiusPx`, `RadiusGrid`,
     `ArrayCountWithLabel`, `ArrayCountNoLabel`, `RefLinkBetweenPivots`,
     `RefLinkBetweenCenters`
     """
     editor_display_mode: EditorDisplayMode
     """Possible values: `Above`, `Center`, `Beneath`"""
     editor_display_pos: EditorDisplayPos
+    editor_display_scale: float
     """Possible values: `ZigZag`, `StraightArrow`, `CurvedArrow`, `ArrowsLine`, `DashedLine`"""
     editor_link_style: EditorLinkStyle
     editor_show_in_world: bool
     editor_text_prefix: Optional[str]
     editor_text_suffix: Optional[str]
     """User defined unique identifier"""
     identifier: str
@@ -241,26 +245,28 @@
     use_for_smart_color: bool
 
     def __init__(
         self,
         type: str,
         accept_file_types: Optional[List[str]],
         allowed_refs: AllowedRefs,
+        allowed_refs_entity_uid: Optional[int],
         allowed_ref_tags: List[str],
         allow_out_of_level_ref: bool,
         array_max_length: Optional[int],
         array_min_length: Optional[int],
         auto_chain_ref: bool,
         can_be_null: bool,
         default_override: Any,
         doc: Optional[str],
         editor_always_show: bool,
         editor_cut_long_values: bool,
         editor_display_mode: EditorDisplayMode,
         editor_display_pos: EditorDisplayPos,
+        editor_display_scale: float,
         editor_link_style: EditorLinkStyle,
         editor_show_in_world: bool,
         editor_text_prefix: Optional[str],
         editor_text_suffix: Optional[str],
         identifier: str,
         is_array: bool,
         max: Optional[float],
@@ -272,26 +278,28 @@
         field_definition_type: str,
         uid: int,
         use_for_smart_color: bool,
     ) -> None:
         self.type = type
         self.accept_file_types = accept_file_types
         self.allowed_refs = allowed_refs
+        self.allowed_refs_entity_uid = allowed_refs_entity_uid
         self.allowed_ref_tags = allowed_ref_tags
         self.allow_out_of_level_ref = allow_out_of_level_ref
         self.array_max_length = array_max_length
         self.array_min_length = array_min_length
         self.auto_chain_ref = auto_chain_ref
         self.can_be_null = can_be_null
         self.default_override = default_override
         self.doc = doc
         self.editor_always_show = editor_always_show
         self.editor_cut_long_values = editor_cut_long_values
         self.editor_display_mode = editor_display_mode
         self.editor_display_pos = editor_display_pos
+        self.editor_display_scale = editor_display_scale
         self.editor_link_style = editor_link_style
         self.editor_show_in_world = editor_show_in_world
         self.editor_text_prefix = editor_text_prefix
         self.editor_text_suffix = editor_text_suffix
         self.identifier = identifier
         self.is_array = is_array
         self.max = max
@@ -308,26 +316,30 @@
     def from_dict(obj: Any) -> "FieldDefinition":
         assert isinstance(obj, dict)
         type = from_str(obj.get("__type"))
         accept_file_types = from_union(
             [from_none, lambda x: from_list(from_str, x)], obj.get("acceptFileTypes")
         )
         allowed_refs = AllowedRefs(obj.get("allowedRefs"))
+        allowed_refs_entity_uid = from_union(
+            [from_none, from_int], obj.get("allowedRefsEntityUid")
+        )
         allowed_ref_tags = from_list(from_str, obj.get("allowedRefTags"))
         allow_out_of_level_ref = from_bool(obj.get("allowOutOfLevelRef"))
         array_max_length = from_union([from_none, from_int], obj.get("arrayMaxLength"))
         array_min_length = from_union([from_none, from_int], obj.get("arrayMinLength"))
         auto_chain_ref = from_bool(obj.get("autoChainRef"))
         can_be_null = from_bool(obj.get("canBeNull"))
         default_override = obj.get("defaultOverride")
         doc = from_union([from_none, from_str], obj.get("doc"))
         editor_always_show = from_bool(obj.get("editorAlwaysShow"))
         editor_cut_long_values = from_bool(obj.get("editorCutLongValues"))
         editor_display_mode = EditorDisplayMode(obj.get("editorDisplayMode"))
         editor_display_pos = EditorDisplayPos(obj.get("editorDisplayPos"))
+        editor_display_scale = from_float(obj.get("editorDisplayScale"))
         editor_link_style = EditorLinkStyle(obj.get("editorLinkStyle"))
         editor_show_in_world = from_bool(obj.get("editorShowInWorld"))
         editor_text_prefix = from_union(
             [from_none, from_str], obj.get("editorTextPrefix")
         )
         editor_text_suffix = from_union(
             [from_none, from_str], obj.get("editorTextSuffix")
@@ -345,26 +357,28 @@
         field_definition_type = from_str(obj.get("type"))
         uid = from_int(obj.get("uid"))
         use_for_smart_color = from_bool(obj.get("useForSmartColor"))
         return FieldDefinition(
             type,
             accept_file_types,
             allowed_refs,
+            allowed_refs_entity_uid,
             allowed_ref_tags,
             allow_out_of_level_ref,
             array_max_length,
             array_min_length,
             auto_chain_ref,
             can_be_null,
             default_override,
             doc,
             editor_always_show,
             editor_cut_long_values,
             editor_display_mode,
             editor_display_pos,
+            editor_display_scale,
             editor_link_style,
             editor_show_in_world,
             editor_text_prefix,
             editor_text_suffix,
             identifier,
             is_array,
             max,
@@ -382,14 +396,18 @@
         result: dict = {}
         result["__type"] = from_str(self.type)
         if self.accept_file_types is not None:
             result["acceptFileTypes"] = from_union(
                 [from_none, lambda x: from_list(from_str, x)], self.accept_file_types
             )
         result["allowedRefs"] = to_enum(AllowedRefs, self.allowed_refs)
+        if self.allowed_refs_entity_uid is not None:
+            result["allowedRefsEntityUid"] = from_union(
+                [from_none, from_int], self.allowed_refs_entity_uid
+            )
         result["allowedRefTags"] = from_list(from_str, self.allowed_ref_tags)
         result["allowOutOfLevelRef"] = from_bool(self.allow_out_of_level_ref)
         if self.array_max_length is not None:
             result["arrayMaxLength"] = from_union(
                 [from_none, from_int], self.array_max_length
             )
         if self.array_min_length is not None:
@@ -404,14 +422,15 @@
             result["doc"] = from_union([from_none, from_str], self.doc)
         result["editorAlwaysShow"] = from_bool(self.editor_always_show)
         result["editorCutLongValues"] = from_bool(self.editor_cut_long_values)
         result["editorDisplayMode"] = to_enum(
             EditorDisplayMode, self.editor_display_mode
         )
         result["editorDisplayPos"] = to_enum(EditorDisplayPos, self.editor_display_pos)
+        result["editorDisplayScale"] = to_float(self.editor_display_scale)
         result["editorLinkStyle"] = to_enum(EditorLinkStyle, self.editor_link_style)
         result["editorShowInWorld"] = from_bool(self.editor_show_in_world)
         if self.editor_text_prefix is not None:
             result["editorTextPrefix"] = from_union(
                 [from_none, from_str], self.editor_text_prefix
             )
         if self.editor_text_suffix is not None:
@@ -754,59 +773,72 @@
             result["tilesetId"] = from_union([from_none, from_int], self.tileset_id)
         result["uid"] = from_int(self.uid)
         result["width"] = from_int(self.width)
         return result
 
 
 class EnumValueDefinition:
-    """An array of 4 Int values that refers to the tile in the tileset image: `[ x, y, width,
-    height ]`
+    """**WARNING**: this deprecated value will be *removed* completely on version 1.4.0+
+    Replaced by: `tileRect`
     """
 
     tile_src_rect: Optional[List[int]]
     """Optional color"""
     color: int
     """Enum value"""
     id: str
-    """The optional ID of the tile"""
+    """**WARNING**: this deprecated value will be *removed* completely on version 1.4.0+
+    Replaced by: `tileRect`
+    """
     tile_id: Optional[int]
+    """Optional tileset rectangle to represents this value"""
+    tile_rect: Optional[TilesetRectangle]
 
     def __init__(
         self,
         tile_src_rect: Optional[List[int]],
         color: int,
         id: str,
         tile_id: Optional[int],
+        tile_rect: Optional[TilesetRectangle],
     ) -> None:
         self.tile_src_rect = tile_src_rect
         self.color = color
         self.id = id
         self.tile_id = tile_id
+        self.tile_rect = tile_rect
 
     @staticmethod
     def from_dict(obj: Any) -> "EnumValueDefinition":
         assert isinstance(obj, dict)
         tile_src_rect = from_union(
             [from_none, lambda x: from_list(from_int, x)], obj.get("__tileSrcRect")
         )
         color = from_int(obj.get("color"))
         id = from_str(obj.get("id"))
         tile_id = from_union([from_none, from_int], obj.get("tileId"))
-        return EnumValueDefinition(tile_src_rect, color, id, tile_id)
+        tile_rect = from_union(
+            [from_none, TilesetRectangle.from_dict], obj.get("tileRect")
+        )
+        return EnumValueDefinition(tile_src_rect, color, id, tile_id, tile_rect)
 
     def to_dict(self) -> dict:
         result: dict = {}
         if self.tile_src_rect is not None:
             result["__tileSrcRect"] = from_union(
                 [from_none, lambda x: from_list(from_int, x)], self.tile_src_rect
             )
         result["color"] = from_int(self.color)
         result["id"] = from_str(self.id)
         if self.tile_id is not None:
             result["tileId"] = from_union([from_none, from_int], self.tile_id)
+        if self.tile_rect is not None:
+            result["tileRect"] = from_union(
+                [from_none, lambda x: to_class(TilesetRectangle, x)], self.tile_rect
+            )
         return result
 
 
 class EnumDefinition:
     external_file_checksum: Optional[str]
     """Relative path to the external file providing this Enum"""
     external_rel_path: Optional[str]
@@ -936,14 +968,26 @@
     pivot_y: float
     """Pattern width & height. Should only be 1,3,5 or 7."""
     size: int
     """Array of all the tile IDs. They are used randomly or as stamps, based on `tileMode` value."""
     tile_ids: List[int]
     """Defines how tileIds array is used Possible values: `Single`, `Stamp`"""
     tile_mode: TileMode
+    """Max random offset for X tile pos"""
+    tile_random_x_max: int
+    """Min random offset for X tile pos"""
+    tile_random_x_min: int
+    """Max random offset for Y tile pos"""
+    tile_random_y_max: int
+    """Min random offset for Y tile pos"""
+    tile_random_y_min: int
+    """Tile X offset"""
+    tile_x_offset: int
+    """Tile Y offset"""
+    tile_y_offset: int
     """Unique Int identifier"""
     uid: int
     """X cell coord modulo"""
     x_modulo: int
     """X cell start offset"""
     x_offset: int
     """Y cell coord modulo"""
@@ -966,14 +1010,20 @@
         perlin_scale: float,
         perlin_seed: float,
         pivot_x: float,
         pivot_y: float,
         size: int,
         tile_ids: List[int],
         tile_mode: TileMode,
+        tile_random_x_max: int,
+        tile_random_x_min: int,
+        tile_random_y_max: int,
+        tile_random_y_min: int,
+        tile_x_offset: int,
+        tile_y_offset: int,
         uid: int,
         x_modulo: int,
         x_offset: int,
         y_modulo: int,
         y_offset: int,
     ) -> None:
         self.active = active
@@ -989,14 +1039,20 @@
         self.perlin_scale = perlin_scale
         self.perlin_seed = perlin_seed
         self.pivot_x = pivot_x
         self.pivot_y = pivot_y
         self.size = size
         self.tile_ids = tile_ids
         self.tile_mode = tile_mode
+        self.tile_random_x_max = tile_random_x_max
+        self.tile_random_x_min = tile_random_x_min
+        self.tile_random_y_max = tile_random_y_max
+        self.tile_random_y_min = tile_random_y_min
+        self.tile_x_offset = tile_x_offset
+        self.tile_y_offset = tile_y_offset
         self.uid = uid
         self.x_modulo = x_modulo
         self.x_offset = x_offset
         self.y_modulo = y_modulo
         self.y_offset = y_offset
 
     @staticmethod
@@ -1017,14 +1073,20 @@
         perlin_scale = from_float(obj.get("perlinScale"))
         perlin_seed = from_float(obj.get("perlinSeed"))
         pivot_x = from_float(obj.get("pivotX"))
         pivot_y = from_float(obj.get("pivotY"))
         size = from_int(obj.get("size"))
         tile_ids = from_list(from_int, obj.get("tileIds"))
         tile_mode = TileMode(obj.get("tileMode"))
+        tile_random_x_max = from_int(obj.get("tileRandomXMax"))
+        tile_random_x_min = from_int(obj.get("tileRandomXMin"))
+        tile_random_y_max = from_int(obj.get("tileRandomYMax"))
+        tile_random_y_min = from_int(obj.get("tileRandomYMin"))
+        tile_x_offset = from_int(obj.get("tileXOffset"))
+        tile_y_offset = from_int(obj.get("tileYOffset"))
         uid = from_int(obj.get("uid"))
         x_modulo = from_int(obj.get("xModulo"))
         x_offset = from_int(obj.get("xOffset"))
         y_modulo = from_int(obj.get("yModulo"))
         y_offset = from_int(obj.get("yOffset"))
         return AutoLayerRuleDefinition(
             active,
@@ -1040,14 +1102,20 @@
             perlin_scale,
             perlin_seed,
             pivot_x,
             pivot_y,
             size,
             tile_ids,
             tile_mode,
+            tile_random_x_max,
+            tile_random_x_min,
+            tile_random_y_max,
+            tile_random_y_min,
+            tile_x_offset,
+            tile_y_offset,
             uid,
             x_modulo,
             x_offset,
             y_modulo,
             y_offset,
         )
 
@@ -1069,14 +1137,20 @@
         result["perlinScale"] = to_float(self.perlin_scale)
         result["perlinSeed"] = to_float(self.perlin_seed)
         result["pivotX"] = to_float(self.pivot_x)
         result["pivotY"] = to_float(self.pivot_y)
         result["size"] = from_int(self.size)
         result["tileIds"] = from_list(from_int, self.tile_ids)
         result["tileMode"] = to_enum(TileMode, self.tile_mode)
+        result["tileRandomXMax"] = from_int(self.tile_random_x_max)
+        result["tileRandomXMin"] = from_int(self.tile_random_x_min)
+        result["tileRandomYMax"] = from_int(self.tile_random_y_max)
+        result["tileRandomYMin"] = from_int(self.tile_random_y_min)
+        result["tileXOffset"] = from_int(self.tile_x_offset)
+        result["tileYOffset"] = from_int(self.tile_y_offset)
         result["uid"] = from_int(self.uid)
         result["xModulo"] = from_int(self.x_modulo)
         result["xOffset"] = from_int(self.x_offset)
         result["yModulo"] = from_int(self.y_modulo)
         result["yOffset"] = from_int(self.y_offset)
         return result
 
@@ -2337,14 +2411,15 @@
         return result
 
 
 class BgPos(Enum):
     CONTAIN = "Contain"
     COVER = "Cover"
     COVER_DIRTY = "CoverDirty"
+    REPEAT = "Repeat"
     UNSCALED = "Unscaled"
 
 
 class NeighbourLevel:
     """Nearby level info"""
 
     """A single lowercase character tipping on the level location (`n`orth, `s`outh, `w`est,
@@ -2412,15 +2487,15 @@
     level_bg_color: Optional[str]
     """Background image X pivot (0-1)"""
     bg_pivot_x: float
     """Background image Y pivot (0-1)"""
     bg_pivot_y: float
     """An enum defining the way the background image (if any) is positioned on the level. See
     `__bgPos` for resulting position info. Possible values: &lt;`null`&gt;, `Unscaled`,
-    `Contain`, `Cover`, `CoverDirty`
+    `Contain`, `Cover`, `CoverDirty`, `Repeat`
     """
     level_bg_pos: Optional[BgPos]
     """The *optional* relative path to the level background image."""
     bg_rel_path: Optional[str]
     """This value is not null if the project option "*Save levels separately*" is enabled. In
     this case, this **relative** path points to the level Json file.
     """
@@ -2644,17 +2719,17 @@
     FREE = "Free"
     GRID_VANIA = "GridVania"
     LINEAR_HORIZONTAL = "LinearHorizontal"
     LINEAR_VERTICAL = "LinearVertical"
 
 
 class World:
-    """**IMPORTANT**: this type is not used *yet* in current LDtk version. It's only presented
-    here as a preview of a planned feature.  A World contains multiple levels, and it has its
-    own layout settings.
+    """**IMPORTANT**: this type is available as a preview. You can rely on it to update your
+    importers, for when it will be officially available.  A World contains multiple levels,
+    and it has its own layout settings.
     """
 
     """Default new level height"""
     default_level_height: int
     """Default new level width"""
     default_level_width: int
     """User defined unique identifier"""
@@ -3084,14 +3159,16 @@
     anonymous.
     """
     app_build_id: float
     """Number of backup files to keep, if the `backupOnSave` is TRUE"""
     backup_limit: int
     """If TRUE, an extra copy of the project will be created in a sub folder, when saving."""
     backup_on_save: bool
+    """Target relative path to store backup files"""
+    backup_rel_path: Optional[str]
     """Project background color"""
     bg_color: str
     """An array of command lines that can be ran manually by the user"""
     custom_commands: List[LdtkCustomCommand]
     """Default grid size for new layers"""
     default_grid_size: int
     """Default background color of levels"""
@@ -3108,14 +3185,16 @@
     default_level_width: Optional[int]
     """Default X pivot (0 to 1) for new entities"""
     default_pivot_x: float
     """Default Y pivot (0 to 1) for new entities"""
     default_pivot_y: float
     """A structure containing all the definitions of this project"""
     defs: Definitions
+    """If the project isn't in MultiWorlds mode, this is the IID of the internal "dummy" World."""
+    dummy_world_iid: str
     """If TRUE, the exported PNGs will include the level background (color or image)."""
     export_level_bg: bool
     """**WARNING**: this deprecated value is no longer exported since version 0.9.3  Replaced
     by: `imageExportMode`
     """
     export_png: Optional[bool]
     """If TRUE, a Tiled compatible file will also be generated along with the LDtk JSON file
@@ -3183,43 +3262,43 @@
     """**WARNING**: this field will move to the `worlds` array after the "multi-worlds" update.
     It will then be `null`. You can enable the Multi-worlds advanced project option to enable
     the change immediately.<br/><br/>  An enum that describes how levels are organized in
     this project (ie. linearly or in a 2D space). Possible values: &lt;`null`&gt;, `Free`,
     `GridVania`, `LinearHorizontal`, `LinearVertical`
     """
     world_layout: Optional[WorldLayout]
-    """This array is not used yet in current LDtk version (so, for now, it's always
-    empty).<br/><br/>In a later update, it will be possible to have multiple Worlds in a
-    single project, each containing multiple Levels.<br/><br/>What will change when "Multiple
-    worlds" support will be added to LDtk:<br/><br/> - in current version, a LDtk project
-    file can only contain a single world with multiple levels in it. In this case, levels and
-    world layout related settings are stored in the root of the JSON.<br/> - after the
-    "Multiple worlds" update, there will be a `worlds` array in root, each world containing
-    levels and layout settings. Basically, it's pretty much only about moving the `levels`
-    array to the `worlds` array, along with world layout related values (eg. `worldGridWidth`
-    etc).<br/><br/>If you want to start supporting this future update easily, please refer to
-    this documentation: https://github.com/deepnight/ldtk/issues/231
+    """This array will be empty, unless you enable the Multi-Worlds in the project advanced
+    settings.<br/><br/> - in current version, a LDtk project file can only contain a single
+    world with multiple levels in it. In this case, levels and world layout related settings
+    are stored in the root of the JSON.<br/> - with "Multi-worlds" enabled, there will be a
+    `worlds` array in root, each world containing levels and layout settings. Basically, it's
+    pretty much only about moving the `levels` array to the `worlds` array, along with world
+    layout related values (eg. `worldGridWidth` etc).<br/><br/>If you want to start
+    supporting this future update easily, please refer to this documentation:
+    https://github.com/deepnight/ldtk/issues/231
     """
     worlds: List[World]
 
     def __init__(
         self,
         forced_refs: Optional[ForcedRefs],
         app_build_id: float,
         backup_limit: int,
         backup_on_save: bool,
+        backup_rel_path: Optional[str],
         bg_color: str,
         custom_commands: List[LdtkCustomCommand],
         default_grid_size: int,
         default_level_bg_color: str,
         default_level_height: Optional[int],
         default_level_width: Optional[int],
         default_pivot_x: float,
         default_pivot_y: float,
         defs: Definitions,
+        dummy_world_iid: str,
         export_level_bg: bool,
         export_png: Optional[bool],
         export_tiled: bool,
         external_levels: bool,
         flags: List[Flag],
         identifier_style: IdentifierStyle,
         iid: str,
@@ -3238,23 +3317,25 @@
         world_layout: Optional[WorldLayout],
         worlds: List[World],
     ) -> None:
         self.forced_refs = forced_refs
         self.app_build_id = app_build_id
         self.backup_limit = backup_limit
         self.backup_on_save = backup_on_save
+        self.backup_rel_path = backup_rel_path
         self.bg_color = bg_color
         self.custom_commands = custom_commands
         self.default_grid_size = default_grid_size
         self.default_level_bg_color = default_level_bg_color
         self.default_level_height = default_level_height
         self.default_level_width = default_level_width
         self.default_pivot_x = default_pivot_x
         self.default_pivot_y = default_pivot_y
         self.defs = defs
+        self.dummy_world_iid = dummy_world_iid
         self.export_level_bg = export_level_bg
         self.export_png = export_png
         self.export_tiled = export_tiled
         self.external_levels = external_levels
         self.flags = flags
         self.identifier_style = identifier_style
         self.iid = iid
@@ -3278,14 +3359,15 @@
         assert isinstance(obj, dict)
         forced_refs = from_union(
             [ForcedRefs.from_dict, from_none], obj.get("__FORCED_REFS")
         )
         app_build_id = from_float(obj.get("appBuildId"))
         backup_limit = from_int(obj.get("backupLimit"))
         backup_on_save = from_bool(obj.get("backupOnSave"))
+        backup_rel_path = from_union([from_none, from_str], obj.get("backupRelPath"))
         bg_color = from_str(obj.get("bgColor"))
         custom_commands = from_list(
             LdtkCustomCommand.from_dict, obj.get("customCommands")
         )
         default_grid_size = from_int(obj.get("defaultGridSize"))
         default_level_bg_color = from_str(obj.get("defaultLevelBgColor"))
         default_level_height = from_union(
@@ -3293,14 +3375,15 @@
         )
         default_level_width = from_union(
             [from_none, from_int], obj.get("defaultLevelWidth")
         )
         default_pivot_x = from_float(obj.get("defaultPivotX"))
         default_pivot_y = from_float(obj.get("defaultPivotY"))
         defs = Definitions.from_dict(obj.get("defs"))
+        dummy_world_iid = from_str(obj.get("dummyWorldIid"))
         export_level_bg = from_bool(obj.get("exportLevelBg"))
         export_png = from_union([from_none, from_bool], obj.get("exportPng"))
         export_tiled = from_bool(obj.get("exportTiled"))
         external_levels = from_bool(obj.get("externalLevels"))
         flags = from_list(Flag, obj.get("flags"))
         identifier_style = IdentifierStyle(obj.get("identifierStyle"))
         iid = from_str(obj.get("iid"))
@@ -3321,23 +3404,25 @@
         world_layout = from_union([from_none, WorldLayout], obj.get("worldLayout"))
         worlds = from_list(World.from_dict, obj.get("worlds"))
         return LdtkJSON(
             forced_refs,
             app_build_id,
             backup_limit,
             backup_on_save,
+            backup_rel_path,
             bg_color,
             custom_commands,
             default_grid_size,
             default_level_bg_color,
             default_level_height,
             default_level_width,
             default_pivot_x,
             default_pivot_y,
             defs,
+            dummy_world_iid,
             export_level_bg,
             export_png,
             export_tiled,
             external_levels,
             flags,
             identifier_style,
             iid,
@@ -3362,14 +3447,18 @@
         if self.forced_refs is not None:
             result["__FORCED_REFS"] = from_union(
                 [lambda x: to_class(ForcedRefs, x), from_none], self.forced_refs
             )
         result["appBuildId"] = to_float(self.app_build_id)
         result["backupLimit"] = from_int(self.backup_limit)
         result["backupOnSave"] = from_bool(self.backup_on_save)
+        if self.backup_rel_path is not None:
+            result["backupRelPath"] = from_union(
+                [from_none, from_str], self.backup_rel_path
+            )
         result["bgColor"] = from_str(self.bg_color)
         result["customCommands"] = from_list(
             lambda x: to_class(LdtkCustomCommand, x), self.custom_commands
         )
         result["defaultGridSize"] = from_int(self.default_grid_size)
         result["defaultLevelBgColor"] = from_str(self.default_level_bg_color)
         if self.default_level_height is not None:
@@ -3379,14 +3468,15 @@
         if self.default_level_width is not None:
             result["defaultLevelWidth"] = from_union(
                 [from_none, from_int], self.default_level_width
             )
         result["defaultPivotX"] = to_float(self.default_pivot_x)
         result["defaultPivotY"] = to_float(self.default_pivot_y)
         result["defs"] = to_class(Definitions, self.defs)
+        result["dummyWorldIid"] = from_str(self.dummy_world_iid)
         result["exportLevelBg"] = from_bool(self.export_level_bg)
         if self.export_png is not None:
             result["exportPng"] = from_union([from_none, from_bool], self.export_png)
         result["exportTiled"] = from_bool(self.export_tiled)
         result["externalLevels"] = from_bool(self.external_levels)
         result["flags"] = from_list(lambda x: to_enum(Flag, x), self.flags)
         result["identifierStyle"] = to_enum(IdentifierStyle, self.identifier_style)
```

### Comparing `ldtkpy-1.2.5/PKG-INFO` & `ldtkpy-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ldtkpy
-Version: 1.2.5
+Version: 1.3.0
 Summary: Load and parse LDtk files, with full types definitions.
 Home-page: https://ldtk.io/api/
 Author: Yann Vaillant
 Author-email: va@yan.pm
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/vayan/ldtk-py
 Description-Content-Type: text/markdown
 
 # LDtk Python 
 
 Load and parse LDtk files, with full types definitions.
```

