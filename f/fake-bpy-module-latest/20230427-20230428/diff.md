# Comparing `tmp/fake-bpy-module-latest-20230427.tar.gz` & `tmp/fake-bpy-module-latest-20230428.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fake-bpy-module-latest-20230427.tar", last modified: Thu Apr 27 06:26:23 2023, max compression
+gzip compressed data, was "dist/fake-bpy-module-latest-20230428.tar", last modified: Fri Apr 28 06:24:13 2023, max compression
```

## Comparing `fake-bpy-module-latest-20230427.tar` & `fake-bpy-module-latest-20230428.tar`

### file list

```diff
@@ -1,352 +1,352 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-27 06:26:22.000000 fake-bpy-module-latest-20230427/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/addon_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/animsys_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/aud.py
--rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-27 06:23:39.000000 fake-bpy-module-latest-20230427/bgl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_app_override/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_app_override/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_app_override/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_app_override/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_app_template_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_console_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/complete_calltip.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/complete_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/complete_namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/intellisense.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_console_utils/autocomplete/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_console_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/bl_extract_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/merge_po.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/utils_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/utils_languages_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_i18n_utils/utils_rtl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/keymap_from_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/keymap_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/platform_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_keymap_utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bl_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_operators/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/add_mesh_torus.py
--rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-27 06:23:54.000000 fake-bpy-module-latest-20230427/bl_operators/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_operators/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/bmesh/find_adjacent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_operators/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-27 06:23:52.000000 fake-bpy-module-latest-20230427/bl_operators/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-27 06:23:53.000000 fake-bpy-module-latest-20230427/bl_operators/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/bl_operators/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/bl_operators/freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/geometry_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-27 06:23:53.000000 fake-bpy-module-latest-20230427/bl_operators/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-27 06:23:50.000000 fake-bpy-module-latest-20230427/bl_operators/object_align.py
--rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-27 06:23:50.000000 fake-bpy-module-latest-20230427/bl_operators/object_quick_effects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/object_randomize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/bl_operators/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_operators/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-27 06:23:50.000000 fake-bpy-module-latest-20230427/bl_operators/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/screen_play_rendered_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/uvcalc_follow_active.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-27 06:23:53.000000 fake-bpy-module-latest-20230427/bl_operators/uvcalc_lightmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-27 06:23:55.000000 fake-bpy-module-latest-20230427/bl_operators/uvcalc_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_operators/vertexpaint_dirt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-27 06:23:50.000000 fake-bpy-module-latest-20230427/bl_operators/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-27 06:23:52.000000 fake-bpy-module-latest-20230427/bl_operators/wm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_previews_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_previews_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/bl_previews_utils/bl_previews_render.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_previews_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_rna_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/bl_rna_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/bl_rna_utils/data_path.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_rna_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_ui/
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-27 06:23:58.000000 fake-bpy-module-latest-20230427/bl_ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-27 06:24:22.000000 fake-bpy-module-latest-20230427/bl_ui/generic_ui_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 06:24:50.000000 fake-bpy-module-latest-20230427/bl_ui/node_add_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-27 06:24:07.000000 fake-bpy-module-latest-20230427/bl_ui/node_add_menu_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-27 06:24:22.000000 fake-bpy-module-latest-20230427/bl_ui/properties_animviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-27 06:24:16.000000 fake-bpy-module-latest-20230427/bl_ui/properties_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-27 06:24:41.000000 fake-bpy-module-latest-20230427/bl_ui/properties_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-27 06:25:59.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-27 06:24:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_bone.py
--rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-27 06:26:20.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-27 06:25:59.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-27 06:25:59.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-27 06:24:08.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-27 06:25:56.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-27 06:24:16.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_light.py
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-27 06:24:22.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_lightprobe.py
--rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-27 06:26:19.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-27 06:24:50.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_metaball.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-27 06:23:58.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_modifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-27 06:25:56.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_pointcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_shaderfx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-27 06:24:23.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_speaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-27 06:24:16.000000 fake-bpy-module-latest-20230427/bl_ui/properties_data_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_freestyle.py
--rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-27 06:23:59.000000 fake-bpy-module-latest-20230427/bl_ui/properties_grease_pencil_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-27 06:24:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_mask_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-27 06:25:56.000000 fake-bpy-module-latest-20230427/bl_ui/properties_material.py
--rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-27 06:23:59.000000 fake-bpy-module-latest-20230427/bl_ui/properties_material_gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-27 06:24:26.000000 fake-bpy-module-latest-20230427/bl_ui/properties_object.py
--rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-27 06:24:00.000000 fake-bpy-module-latest-20230427/bl_ui/properties_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-27 06:24:21.000000 fake-bpy-module-latest-20230427/bl_ui/properties_paint_common.py
--rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-27 06:24:54.000000 fake-bpy-module-latest-20230427/bl_ui/properties_particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-27 06:23:58.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-27 06:23:58.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-27 06:24:09.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_dynamicpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-27 06:25:57.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-27 06:26:01.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-27 06:26:18.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-27 06:24:42.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_rigidbody_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-27 06:26:02.000000 fake-bpy-module-latest-20230427/bl_ui/properties_physics_softbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-27 06:24:25.000000 fake-bpy-module-latest-20230427/bl_ui/properties_render.py
--rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-27 06:24:16.000000 fake-bpy-module-latest-20230427/bl_ui/properties_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-27 06:24:44.000000 fake-bpy-module-latest-20230427/bl_ui/properties_texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-27 06:25:55.000000 fake-bpy-module-latest-20230427/bl_ui/properties_view_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-27 06:24:44.000000 fake-bpy-module-latest-20230427/bl_ui/properties_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-27 06:26:02.000000 fake-bpy-module-latest-20230427/bl_ui/properties_world.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_ui/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-27 06:24:48.000000 fake-bpy-module-latest-20230427/bl_ui/space_clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-27 06:24:26.000000 fake-bpy-module-latest-20230427/bl_ui/space_console.py
--rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-27 06:24:23.000000 fake-bpy-module-latest-20230427/bl_ui/space_dopesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-27 06:24:18.000000 fake-bpy-module-latest-20230427/bl_ui/space_filebrowser.py
--rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-27 06:24:21.000000 fake-bpy-module-latest-20230427/bl_ui/space_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-27 06:24:15.000000 fake-bpy-module-latest-20230427/bl_ui/space_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-27 06:24:24.000000 fake-bpy-module-latest-20230427/bl_ui/space_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-27 06:25:55.000000 fake-bpy-module-latest-20230427/bl_ui/space_nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-27 06:24:19.000000 fake-bpy-module-latest-20230427/bl_ui/space_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-27 06:24:20.000000 fake-bpy-module-latest-20230427/bl_ui/space_outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-27 06:24:41.000000 fake-bpy-module-latest-20230427/bl_ui/space_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-27 06:24:05.000000 fake-bpy-module-latest-20230427/bl_ui/space_sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-27 06:25:56.000000 fake-bpy-module-latest-20230427/bl_ui/space_spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-27 06:24:19.000000 fake-bpy-module-latest-20230427/bl_ui/space_statusbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-27 06:25:58.000000 fake-bpy-module-latest-20230427/bl_ui/space_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-27 06:24:49.000000 fake-bpy-module-latest-20230427/bl_ui/space_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-27 06:24:20.000000 fake-bpy-module-latest-20230427/bl_ui/space_toolsystem_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-04-27 06:24:49.000000 fake-bpy-module-latest-20230427/bl_ui/space_toolsystem_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-27 06:24:50.000000 fake-bpy-module-latest-20230427/bl_ui/space_topbar.py
--rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-27 06:26:08.000000 fake-bpy-module-latest-20230427/bl_ui/space_userpref.py
--rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-27 06:25:54.000000 fake-bpy-module-latest-20230427/bl_ui/space_view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-27 06:26:18.000000 fake-bpy-module-latest-20230427/bl_ui/space_view3d_toolbar.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-27 06:24:20.000000 fake-bpy-module-latest-20230427/bl_ui/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bl_ui_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui_utils/bug_report_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bl_ui_utils/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bl_ui_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/blend_render_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-27 06:23:39.000000 fake-bpy-module-latest-20230427/blf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bmesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/bmesh/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bmesh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bmesh/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy/app/
--rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/app/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/app/icons.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/app/timers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/app/translations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/msgbus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-27 06:15:00.000000 fake-bpy-module-latest-20230427/bpy/ops/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-27 06:14:37.000000 fake-bpy-module-latest-20230427/bpy/ops/anim.py
--rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-27 06:14:38.000000 fake-bpy-module-latest-20230427/bpy/ops/armature.py
--rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-27 06:14:16.000000 fake-bpy-module-latest-20230427/bpy/ops/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-27 06:14:17.000000 fake-bpy-module-latest-20230427/bpy/ops/boid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-27 06:14:17.000000 fake-bpy-module-latest-20230427/bpy/ops/brush.py
--rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-27 06:14:38.000000 fake-bpy-module-latest-20230427/bpy/ops/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-27 06:14:54.000000 fake-bpy-module-latest-20230427/bpy/ops/cachefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-27 06:14:49.000000 fake-bpy-module-latest-20230427/bpy/ops/camera.py
--rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-27 06:14:53.000000 fake-bpy-module-latest-20230427/bpy/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-27 06:14:23.000000 fake-bpy-module-latest-20230427/bpy/ops/cloth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-27 06:15:00.000000 fake-bpy-module-latest-20230427/bpy/ops/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-27 06:14:52.000000 fake-bpy-module-latest-20230427/bpy/ops/console.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-27 06:14:48.000000 fake-bpy-module-latest-20230427/bpy/ops/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-27 06:14:28.000000 fake-bpy-module-latest-20230427/bpy/ops/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/ops/curves.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-27 06:14:43.000000 fake-bpy-module-latest-20230427/bpy/ops/cycles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-27 06:14:38.000000 fake-bpy-module-latest-20230427/bpy/ops/dpaint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-27 06:14:53.000000 fake-bpy-module-latest-20230427/bpy/ops/ed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-27 06:14:59.000000 fake-bpy-module-latest-20230427/bpy/ops/export_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-27 06:14:23.000000 fake-bpy-module-latest-20230427/bpy/ops/export_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-27 06:14:46.000000 fake-bpy-module-latest-20230427/bpy/ops/export_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-27 06:14:43.000000 fake-bpy-module-latest-20230427/bpy/ops/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-27 06:14:46.000000 fake-bpy-module-latest-20230427/bpy/ops/fluid.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-27 06:14:15.000000 fake-bpy-module-latest-20230427/bpy/ops/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-27 06:14:15.000000 fake-bpy-module-latest-20230427/bpy/ops/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-27 06:14:49.000000 fake-bpy-module-latest-20230427/bpy/ops/gizmogroup.py
--rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-27 06:14:26.000000 fake-bpy-module-latest-20230427/bpy/ops/gpencil.py
--rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-27 06:14:48.000000 fake-bpy-module-latest-20230427/bpy/ops/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-27 06:15:01.000000 fake-bpy-module-latest-20230427/bpy/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-27 06:14:48.000000 fake-bpy-module-latest-20230427/bpy/ops/import_anim.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-27 06:14:57.000000 fake-bpy-module-latest-20230427/bpy/ops/import_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-27 06:14:26.000000 fake-bpy-module-latest-20230427/bpy/ops/import_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-27 06:15:03.000000 fake-bpy-module-latest-20230427/bpy/ops/import_scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-27 06:14:23.000000 fake-bpy-module-latest-20230427/bpy/ops/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/lattice.py
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-27 06:14:42.000000 fake-bpy-module-latest-20230427/bpy/ops/marker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-27 06:14:49.000000 fake-bpy-module-latest-20230427/bpy/ops/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 06:14:53.000000 fake-bpy-module-latest-20230427/bpy/ops/material.py
--rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-27 06:14:15.000000 fake-bpy-module-latest-20230427/bpy/ops/mball.py
--rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-27 06:14:57.000000 fake-bpy-module-latest-20230427/bpy/ops/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-27 06:14:41.000000 fake-bpy-module-latest-20230427/bpy/ops/nla.py
--rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-27 06:14:18.000000 fake-bpy-module-latest-20230427/bpy/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-27 06:14:22.000000 fake-bpy-module-latest-20230427/bpy/ops/object.py
--rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-27 06:14:15.000000 fake-bpy-module-latest-20230427/bpy/ops/outliner.py
--rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-27 06:14:27.000000 fake-bpy-module-latest-20230427/bpy/ops/paint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/paintcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-27 06:14:48.000000 fake-bpy-module-latest-20230427/bpy/ops/palette.py
--rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-27 06:14:36.000000 fake-bpy-module-latest-20230427/bpy/ops/particle.py
--rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-27 06:15:02.000000 fake-bpy-module-latest-20230427/bpy/ops/pose.py
--rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-27 06:14:23.000000 fake-bpy-module-latest-20230427/bpy/ops/poselib.py
--rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-27 06:14:35.000000 fake-bpy-module-latest-20230427/bpy/ops/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/ptcache.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/ops/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-27 06:14:18.000000 fake-bpy-module-latest-20230427/bpy/ops/render.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-27 06:15:00.000000 fake-bpy-module-latest-20230427/bpy/ops/rigidbody.py
--rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-27 06:14:16.000000 fake-bpy-module-latest-20230427/bpy/ops/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-27 06:14:41.000000 fake-bpy-module-latest-20230427/bpy/ops/screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/script.py
--rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-27 06:14:51.000000 fake-bpy-module-latest-20230427/bpy/ops/sculpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-27 06:14:22.000000 fake-bpy-module-latest-20230427/bpy/ops/sculpt_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-27 06:14:59.000000 fake-bpy-module-latest-20230427/bpy/ops/sequencer.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-27 06:14:16.000000 fake-bpy-module-latest-20230427/bpy/ops/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-27 06:14:43.000000 fake-bpy-module-latest-20230427/bpy/ops/spreadsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-27 06:14:42.000000 fake-bpy-module-latest-20230427/bpy/ops/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-27 06:14:40.000000 fake-bpy-module-latest-20230427/bpy/ops/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-27 06:14:43.000000 fake-bpy-module-latest-20230427/bpy/ops/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-27 06:14:37.000000 fake-bpy-module-latest-20230427/bpy/ops/uilist.py
--rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-27 06:14:50.000000 fake-bpy-module-latest-20230427/bpy/ops/uv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-27 06:14:43.000000 fake-bpy-module-latest-20230427/bpy/ops/view2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-27 06:14:47.000000 fake-bpy-module-latest-20230427/bpy/ops/view3d.py
--rw-r--r--   0 runner    (1001) docker     (123)   246049 2023-04-27 06:14:35.000000 fake-bpy-module-latest-20230427/bpy/ops/wm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-27 06:14:37.000000 fake-bpy-module-latest-20230427/bpy/ops/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-27 06:14:53.000000 fake-bpy-module-latest-20230427/bpy/ops/world.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/props.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-04-27 06:23:36.000000 fake-bpy-module-latest-20230427/bpy/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/utils/previews.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy/utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-27 06:23:37.000000 fake-bpy-module-latest-20230427/bpy/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/anim_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/asset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/bmesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/id_map_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/keyconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/mesh_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/node_shader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/object_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/view3d_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/bpy_extras/wm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/wm_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/bpy_extras/wm_utils/progress_report.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/bpy_extras/wm_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/bpy_restrict_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-27 06:23:58.000000 fake-bpy-module-latest-20230427/bpy_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/console_python.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/console_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/freestyle/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/freestyle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-27 06:23:45.000000 fake-bpy-module-latest-20230427/freestyle/chainingiterators.py
--rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/freestyle/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-27 06:23:42.000000 fake-bpy-module-latest-20230427/freestyle/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/freestyle/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-27 06:23:42.000000 fake-bpy-module-latest-20230427/freestyle/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/freestyle/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/freestyle/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/freestyle/utils/ContextFunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/freestyle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/freestyle/utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/gpu/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/gpu/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/shader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/texture.py
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/gpu_extras/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu_extras/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/gpu_extras/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/gpu_extras/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/graphviz_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/idprop/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/idprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/idprop/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/idprop/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/imbuf/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/imbuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/imbuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/imbuf/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/keyingsets_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/keyingsets_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/mathutils/
--rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-27 06:23:40.000000 fake-bpy-module-latest-20230427/mathutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-27 06:23:40.000000 fake-bpy-module-latest-20230427/mathutils/bvhtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-27 06:23:40.000000 fake-bpy-module-latest-20230427/mathutils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-27 06:23:40.000000 fake-bpy-module-latest-20230427/mathutils/interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-27 06:23:40.000000 fake-bpy-module-latest-20230427/mathutils/kdtree.py
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-27 06:23:41.000000 fake-bpy-module-latest-20230427/mathutils/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 06:14:14.000000 fake-bpy-module-latest-20230427/mathutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/nodeitems_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/nodeitems_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/rna_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-27 06:23:49.000000 fake-bpy-module-latest-20230427/rna_keymap_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-27 06:23:48.000000 fake-bpy-module-latest-20230427/rna_prop_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-27 06:26:21.000000 fake-bpy-module-latest-20230427/rna_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 06:26:23.000000 fake-bpy-module-latest-20230427/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-27 06:26:22.000000 fake-bpy-module-latest-20230427/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-27 06:23:56.000000 fake-bpy-module-latest-20230427/sys_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/addon_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/animsys_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31249 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/aud.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116266 2023-04-28 06:21:56.000000 fake-bpy-module-latest-20230428/bgl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_app_override/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_app_override/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_app_override/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_app_override/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_app_template_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_console_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/complete_calltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/complete_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/complete_namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/intellisense.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_console_utils/autocomplete/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_console_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/bl_extract_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/merge_po.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/utils_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/utils_languages_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_i18n_utils/utils_rtl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/keymap_from_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/keymap_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/platform_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_keymap_utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/add_mesh_torus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8777 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_operators/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_operators/assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_operators/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/bmesh/find_adjacent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_operators/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22556 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-04-28 06:24:07.000000 fake-bpy-module-latest-20230428/bl_operators/freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/geometry_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-04-28 06:24:09.000000 fake-bpy-module-latest-20230428/bl_operators/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38053 2023-04-28 06:24:07.000000 fake-bpy-module-latest-20230428/bl_operators/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/object_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9176 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/object_quick_effects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/object_randomize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42973 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_operators/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/screen_play_rendered_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12099 2023-04-28 06:24:07.000000 fake-bpy-module-latest-20230428/bl_operators/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56119 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/uvcalc_follow_active.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/uvcalc_lightmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_operators/uvcalc_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-28 06:24:06.000000 fake-bpy-module-latest-20230428/bl_operators/vertexpaint_dirt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11529 2023-04-28 06:24:07.000000 fake-bpy-module-latest-20230428/bl_operators/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97820 2023-04-28 06:24:09.000000 fake-bpy-module-latest-20230428/bl_operators/wm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_previews_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_previews_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/bl_previews_utils/bl_previews_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_previews_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_rna_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_rna_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/bl_rna_utils/data_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_rna_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bl_ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-28 06:23:44.000000 fake-bpy-module-latest-20230428/bl_ui/generic_ui_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 06:23:47.000000 fake-bpy-module-latest-20230428/bl_ui/node_add_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108259 2023-04-28 06:22:05.000000 fake-bpy-module-latest-20230428/bl_ui/node_add_menu_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-04-28 06:23:41.000000 fake-bpy-module-latest-20230428/bl_ui/properties_animviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13049 2023-04-28 06:23:45.000000 fake-bpy-module-latest-20230428/bl_ui/properties_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   385296 2023-04-28 06:23:20.000000 fake-bpy-module-latest-20230428/bl_ui/properties_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25330 2023-04-28 06:23:06.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22602 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_bone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36945 2023-04-28 06:24:03.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38857 2023-04-28 06:23:31.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15423 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-28 06:23:29.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46403 2023-04-28 06:23:59.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-04-28 06:24:01.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28154 2023-04-28 06:22:05.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_light.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-04-28 06:22:05.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_lightprobe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57510 2023-04-28 06:24:00.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-04-28 06:22:58.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_metaball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-04-28 06:22:05.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_pointcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-28 06:24:00.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_shaderfx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12829 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_speaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20178 2023-04-28 06:22:06.000000 fake-bpy-module-latest-20230428/bl_ui/properties_data_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66640 2023-04-28 06:23:31.000000 fake-bpy-module-latest-20230428/bl_ui/properties_freestyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32219 2023-04-28 06:23:28.000000 fake-bpy-module-latest-20230428/bl_ui/properties_grease_pencil_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-04-28 06:23:45.000000 fake-bpy-module-latest-20230428/bl_ui/properties_mask_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30514 2023-04-28 06:23:41.000000 fake-bpy-module-latest-20230428/bl_ui/properties_material.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25892 2023-04-28 06:23:01.000000 fake-bpy-module-latest-20230428/bl_ui/properties_material_gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35174 2023-04-28 06:23:28.000000 fake-bpy-module-latest-20230428/bl_ui/properties_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46745 2023-04-28 06:23:32.000000 fake-bpy-module-latest-20230428/bl_ui/properties_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-04-28 06:23:27.000000 fake-bpy-module-latest-20230428/bl_ui/properties_paint_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133597 2023-04-28 06:23:40.000000 fake-bpy-module-latest-20230428/bl_ui/properties_particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-04-28 06:23:46.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-28 06:22:58.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67584 2023-04-28 06:23:44.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_dynamicpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27217 2023-04-28 06:23:28.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91307 2023-04-28 06:23:01.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-28 06:23:37.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33547 2023-04-28 06:22:59.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_rigidbody_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39030 2023-04-28 06:23:02.000000 fake-bpy-module-latest-20230428/bl_ui/properties_physics_softbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89468 2023-04-28 06:23:08.000000 fake-bpy-module-latest-20230428/bl_ui/properties_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32886 2023-04-28 06:23:43.000000 fake-bpy-module-latest-20230428/bl_ui/properties_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66952 2023-04-28 06:24:03.000000 fake-bpy-module-latest-20230428/bl_ui/properties_texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37695 2023-04-28 06:23:08.000000 fake-bpy-module-latest-20230428/bl_ui/properties_view_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-28 06:23:40.000000 fake-bpy-module-latest-20230428/bl_ui/properties_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15459 2023-04-28 06:23:22.000000 fake-bpy-module-latest-20230428/bl_ui/properties_world.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_ui/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   174521 2023-04-28 06:23:06.000000 fake-bpy-module-latest-20230428/bl_ui/space_clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-04-28 06:23:51.000000 fake-bpy-module-latest-20230428/bl_ui/space_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62595 2023-04-28 06:23:41.000000 fake-bpy-module-latest-20230428/bl_ui/space_dopesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71853 2023-04-28 06:24:01.000000 fake-bpy-module-latest-20230428/bl_ui/space_filebrowser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43433 2023-04-28 06:23:42.000000 fake-bpy-module-latest-20230428/bl_ui/space_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187053 2023-04-28 06:23:51.000000 fake-bpy-module-latest-20230428/bl_ui/space_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-04-28 06:23:02.000000 fake-bpy-module-latest-20230428/bl_ui/space_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38361 2023-04-28 06:24:00.000000 fake-bpy-module-latest-20230428/bl_ui/space_nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65582 2023-04-28 06:23:22.000000 fake-bpy-module-latest-20230428/bl_ui/space_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35830 2023-04-28 06:23:29.000000 fake-bpy-module-latest-20230428/bl_ui/space_outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-28 06:24:03.000000 fake-bpy-module-latest-20230428/bl_ui/space_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182398 2023-04-28 06:23:36.000000 fake-bpy-module-latest-20230428/bl_ui/space_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-28 06:23:29.000000 fake-bpy-module-latest-20230428/bl_ui/space_spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-28 06:23:28.000000 fake-bpy-module-latest-20230428/bl_ui/space_statusbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40008 2023-04-28 06:23:43.000000 fake-bpy-module-latest-20230428/bl_ui/space_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-04-28 06:23:27.000000 fake-bpy-module-latest-20230428/bl_ui/space_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-28 06:23:02.000000 fake-bpy-module-latest-20230428/bl_ui/space_toolsystem_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21583 2023-04-28 06:23:30.000000 fake-bpy-module-latest-20230428/bl_ui/space_toolsystem_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65863 2023-04-28 06:23:47.000000 fake-bpy-module-latest-20230428/bl_ui/space_topbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   209844 2023-04-28 06:23:27.000000 fake-bpy-module-latest-20230428/bl_ui/space_userpref.py
+-rw-r--r--   0 runner    (1001) docker     (123)   611242 2023-04-28 06:22:58.000000 fake-bpy-module-latest-20230428/bl_ui/space_view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237261 2023-04-28 06:23:58.000000 fake-bpy-module-latest-20230428/bl_ui/space_view3d_toolbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bl_ui_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui_utils/bug_report_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bl_ui_utils/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bl_ui_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/blend_render_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-04-28 06:21:56.000000 fake-bpy-module-latest-20230428/blf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bmesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77491 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/bmesh/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    37270 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bmesh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bmesh/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy/app/
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/app/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/app/icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy/app/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/app/timers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/app/translations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-04-28 06:21:53.000000 fake-bpy-module-latest-20230428/bpy/msgbus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27608 2023-04-28 06:21:22.000000 fake-bpy-module-latest-20230428/bpy/ops/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35270 2023-04-28 06:21:13.000000 fake-bpy-module-latest-20230428/bpy/ops/anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25130 2023-04-28 06:21:53.000000 fake-bpy-module-latest-20230428/bpy/ops/armature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-28 06:21:51.000000 fake-bpy-module-latest-20230428/bpy/ops/boid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/brush.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12217 2023-04-28 06:21:52.000000 fake-bpy-module-latest-20230428/bpy/ops/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/cachefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70010 2023-04-28 06:21:52.000000 fake-bpy-module-latest-20230428/bpy/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/cloth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-28 06:21:46.000000 fake-bpy-module-latest-20230428/bpy/ops/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-28 06:21:29.000000 fake-bpy-module-latest-20230428/bpy/ops/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-04-28 06:21:35.000000 fake-bpy-module-latest-20230428/bpy/ops/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40490 2023-04-28 06:21:21.000000 fake-bpy-module-latest-20230428/bpy/ops/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8223 2023-04-28 06:21:26.000000 fake-bpy-module-latest-20230428/bpy/ops/curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-28 06:21:40.000000 fake-bpy-module-latest-20230428/bpy/ops/cycles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-28 06:21:25.000000 fake-bpy-module-latest-20230428/bpy/ops/dpaint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-04-28 06:21:38.000000 fake-bpy-module-latest-20230428/bpy/ops/ed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-28 06:21:26.000000 fake-bpy-module-latest-20230428/bpy/ops/export_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/export_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40642 2023-04-28 06:21:18.000000 fake-bpy-module-latest-20230428/bpy/ops/export_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30339 2023-04-28 06:21:25.000000 fake-bpy-module-latest-20230428/bpy/ops/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7036 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/fluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-04-28 06:21:48.000000 fake-bpy-module-latest-20230428/bpy/ops/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/gizmogroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132520 2023-04-28 06:21:31.000000 fake-bpy-module-latest-20230428/bpy/ops/gpencil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49736 2023-04-28 06:21:48.000000 fake-bpy-module-latest-20230428/bpy/ops/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53280 2023-04-28 06:21:24.000000 fake-bpy-module-latest-20230428/bpy/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/import_anim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-28 06:21:12.000000 fake-bpy-module-latest-20230428/bpy/ops/import_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-28 06:21:36.000000 fake-bpy-module-latest-20230428/bpy/ops/import_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-28 06:21:35.000000 fake-bpy-module-latest-20230428/bpy/ops/import_scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-04-28 06:21:32.000000 fake-bpy-module-latest-20230428/bpy/ops/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-28 06:21:24.000000 fake-bpy-module-latest-20230428/bpy/ops/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-04-28 06:21:51.000000 fake-bpy-module-latest-20230428/bpy/ops/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26986 2023-04-28 06:21:21.000000 fake-bpy-module-latest-20230428/bpy/ops/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 06:21:29.000000 fake-bpy-module-latest-20230428/bpy/ops/material.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-28 06:21:35.000000 fake-bpy-module-latest-20230428/bpy/ops/mball.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182898 2023-04-28 06:21:51.000000 fake-bpy-module-latest-20230428/bpy/ops/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28495 2023-04-28 06:21:34.000000 fake-bpy-module-latest-20230428/bpy/ops/nla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67349 2023-04-28 06:21:23.000000 fake-bpy-module-latest-20230428/bpy/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220624 2023-04-28 06:21:12.000000 fake-bpy-module-latest-20230428/bpy/ops/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44201 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/outliner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43251 2023-04-28 06:21:36.000000 fake-bpy-module-latest-20230428/bpy/ops/paint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-04-28 06:21:46.000000 fake-bpy-module-latest-20230428/bpy/ops/paintcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-28 06:21:20.000000 fake-bpy-module-latest-20230428/bpy/ops/palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22863 2023-04-28 06:21:12.000000 fake-bpy-module-latest-20230428/bpy/ops/particle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39857 2023-04-28 06:21:37.000000 fake-bpy-module-latest-20230428/bpy/ops/pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/poselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32388 2023-04-28 06:21:39.000000 fake-bpy-module-latest-20230428/bpy/ops/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 06:21:36.000000 fake-bpy-module-latest-20230428/bpy/ops/ptcache.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy/ops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-04-28 06:21:26.000000 fake-bpy-module-latest-20230428/bpy/ops/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-04-28 06:21:29.000000 fake-bpy-module-latest-20230428/bpy/ops/rigidbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25220 2023-04-28 06:21:36.000000 fake-bpy-module-latest-20230428/bpy/ops/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31884 2023-04-28 06:21:13.000000 fake-bpy-module-latest-20230428/bpy/ops/screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46533 2023-04-28 06:21:39.000000 fake-bpy-module-latest-20230428/bpy/ops/sculpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-04-28 06:21:40.000000 fake-bpy-module-latest-20230428/bpy/ops/sculpt_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93839 2023-04-28 06:21:20.000000 fake-bpy-module-latest-20230428/bpy/ops/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-28 06:21:32.000000 fake-bpy-module-latest-20230428/bpy/ops/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/spreadsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-04-28 06:21:32.000000 fake-bpy-module-latest-20230428/bpy/ops/surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30944 2023-04-28 06:21:40.000000 fake-bpy-module-latest-20230428/bpy/ops/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-28 06:21:40.000000 fake-bpy-module-latest-20230428/bpy/ops/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70511 2023-04-28 06:21:28.000000 fake-bpy-module-latest-20230428/bpy/ops/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19257 2023-04-28 06:21:33.000000 fake-bpy-module-latest-20230428/bpy/ops/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-28 06:21:36.000000 fake-bpy-module-latest-20230428/bpy/ops/uilist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56151 2023-04-28 06:21:26.000000 fake-bpy-module-latest-20230428/bpy/ops/uv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-04-28 06:21:48.000000 fake-bpy-module-latest-20230428/bpy/ops/view2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56515 2023-04-28 06:21:32.000000 fake-bpy-module-latest-20230428/bpy/ops/view3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)   246049 2023-04-28 06:21:46.000000 fake-bpy-module-latest-20230428/bpy/ops/wm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-04-28 06:21:14.000000 fake-bpy-module-latest-20230428/bpy/ops/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-28 06:21:52.000000 fake-bpy-module-latest-20230428/bpy/ops/world.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-04-28 06:21:53.000000 fake-bpy-module-latest-20230428/bpy/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27445 2023-04-28 06:21:54.000000 fake-bpy-module-latest-20230428/bpy/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)  3488183 2023-04-28 06:21:09.000000 fake-bpy-module-latest-20230428/bpy/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10832 2023-04-28 06:21:54.000000 fake-bpy-module-latest-20230428/bpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-04-28 06:21:54.000000 fake-bpy-module-latest-20230428/bpy/utils/previews.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy/utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-28 06:21:54.000000 fake-bpy-module-latest-20230428/bpy/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/anim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/asset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/bmesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/id_map_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/keyconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/mesh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/node_shader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/object_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/view3d_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/bpy_extras/wm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/wm_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/bpy_extras/wm_utils/progress_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/bpy_extras/wm_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/bpy_restrict_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54167 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/bpy_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/console_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/console_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/freestyle/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/freestyle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/freestyle/chainingiterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47908 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/freestyle/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/freestyle/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/freestyle/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23737 2023-04-28 06:21:59.000000 fake-bpy-module-latest-20230428/freestyle/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86403 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/freestyle/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/freestyle/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/freestyle/utils/ContextFunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/freestyle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/freestyle/utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/platform.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/gpu/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/shader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/texture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/gpu_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu_extras/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/gpu_extras/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/gpu_extras/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/graphviz_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/idprop/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/idprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/idprop/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/idprop/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/imbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/imbuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/imbuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-28 06:22:03.000000 fake-bpy-module-latest-20230428/imbuf/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48637 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/keyingsets_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/keyingsets_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/mathutils/
+-rw-r--r--   0 runner    (1001) docker     (123)    86215 2023-04-28 06:21:57.000000 fake-bpy-module-latest-20230428/mathutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-04-28 06:21:57.000000 fake-bpy-module-latest-20230428/mathutils/bvhtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22187 2023-04-28 06:21:57.000000 fake-bpy-module-latest-20230428/mathutils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-28 06:21:57.000000 fake-bpy-module-latest-20230428/mathutils/interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-28 06:21:57.000000 fake-bpy-module-latest-20230428/mathutils/kdtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-04-28 06:21:58.000000 fake-bpy-module-latest-20230428/mathutils/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:41.000000 fake-bpy-module-latest-20230428/mathutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/nodeitems_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/nodeitems_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/rna_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 06:24:10.000000 fake-bpy-module-latest-20230428/rna_keymap_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-28 06:24:04.000000 fake-bpy-module-latest-20230428/rna_prop_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-28 06:24:05.000000 fake-bpy-module-latest-20230428/rna_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 06:24:13.000000 fake-bpy-module-latest-20230428/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-04-28 06:24:12.000000 fake-bpy-module-latest-20230428/sys_info.py
```

### Comparing `fake-bpy-module-latest-20230427/PKG-INFO` & `fake-bpy-module-latest-20230428/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230427
+Version: 20230428
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230427/README.rst` & `fake-bpy-module-latest-20230428/README.rst`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/addon_utils.py` & `fake-bpy-module-latest-20230428/addon_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/animsys_refactor.py` & `fake-bpy-module-latest-20230428/animsys_refactor.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/aud.py` & `fake-bpy-module-latest-20230428/aud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bgl.py` & `fake-bpy-module-latest-20230428/bgl.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_app_override/helpers.py` & `fake-bpy-module-latest-20230428/bl_app_override/helpers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_i18n_utils/bl_extract_messages.py` & `fake-bpy-module-latest-20230428/bl_i18n_utils/bl_extract_messages.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_i18n_utils/settings.py` & `fake-bpy-module-latest-20230428/bl_i18n_utils/settings.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_i18n_utils/utils.py` & `fake-bpy-module-latest-20230428/bl_i18n_utils/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_keymap_utils/io.py` & `fake-bpy-module-latest-20230428/bl_keymap_utils/io.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_math.py` & `fake-bpy-module-latest-20230428/bl_math.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/__init__.py` & `fake-bpy-module-latest-20230428/bl_operators/__init__.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import sys
 import typing
-from . import add_mesh_torus
-from . import object_randomize_transform
+from . import assets
+from . import anim
+from . import screen_play_rendered_anim
+from . import console
+from . import uvcalc_lightmap
+from . import presets
+from . import geometry_nodes
+from . import constraint
+from . import mesh
 from . import spreadsheet
+from . import object_randomize_transform
 from . import vertexpaint_dirt
-from . import bmesh
-from . import screen_play_rendered_anim
-from . import sequencer
 from . import object_align
-from . import object_quick_effects
-from . import rigidbody
+from . import freestyle
+from . import object
 from . import view3d
+from . import sequencer
 from . import wm
-from . import clip
-from . import console
-from . import object
-from . import uvcalc_lightmap
-from . import anim
-from . import userpref
-from . import constraint
-from . import geometry_nodes
 from . import image
-from . import mesh
-from . import assets
-from . import node
+from . import userpref
 from . import uvcalc_transform
-from . import uvcalc_follow_active
-from . import presets
-from . import freestyle
 from . import file
+from . import clip
+from . import node
+from . import rigidbody
+from . import bmesh
+from . import object_quick_effects
+from . import uvcalc_follow_active
+from . import add_mesh_torus
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def register():
     '''
```

### Comparing `fake-bpy-module-latest-20230427/bl_operators/add_mesh_torus.py` & `fake-bpy-module-latest-20230428/bl_operators/add_mesh_torus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/anim.py` & `fake-bpy-module-latest-20230428/bl_operators/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/assets.py` & `fake-bpy-module-latest-20230428/bl_operators/assets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/bmesh/find_adjacent.py` & `fake-bpy-module-latest-20230428/bl_operators/bmesh/find_adjacent.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/clip.py` & `fake-bpy-module-latest-20230428/bl_operators/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/console.py` & `fake-bpy-module-latest-20230428/bl_operators/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/constraint.py` & `fake-bpy-module-latest-20230428/bl_operators/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/file.py` & `fake-bpy-module-latest-20230428/bl_operators/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/freestyle.py` & `fake-bpy-module-latest-20230428/bl_operators/freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/geometry_nodes.py` & `fake-bpy-module-latest-20230428/bl_operators/geometry_nodes.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/image.py` & `fake-bpy-module-latest-20230428/bl_operators/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/mesh.py` & `fake-bpy-module-latest-20230428/bl_operators/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/node.py` & `fake-bpy-module-latest-20230428/bl_operators/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/object.py` & `fake-bpy-module-latest-20230428/bl_operators/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/object_align.py` & `fake-bpy-module-latest-20230428/bl_operators/object_align.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/object_quick_effects.py` & `fake-bpy-module-latest-20230428/bl_operators/object_quick_effects.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/object_randomize_transform.py` & `fake-bpy-module-latest-20230428/bl_operators/object_randomize_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/presets.py` & `fake-bpy-module-latest-20230428/bl_operators/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/rigidbody.py` & `fake-bpy-module-latest-20230428/bl_operators/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/screen_play_rendered_anim.py` & `fake-bpy-module-latest-20230428/bl_operators/screen_play_rendered_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/sequencer.py` & `fake-bpy-module-latest-20230428/bl_operators/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/spreadsheet.py` & `fake-bpy-module-latest-20230428/bl_operators/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/userpref.py` & `fake-bpy-module-latest-20230428/bl_operators/userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/uvcalc_follow_active.py` & `fake-bpy-module-latest-20230428/bl_operators/uvcalc_follow_active.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/uvcalc_lightmap.py` & `fake-bpy-module-latest-20230428/bl_operators/uvcalc_lightmap.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/uvcalc_transform.py` & `fake-bpy-module-latest-20230428/bl_operators/uvcalc_transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/vertexpaint_dirt.py` & `fake-bpy-module-latest-20230428/bl_operators/vertexpaint_dirt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/view3d.py` & `fake-bpy-module-latest-20230428/bl_operators/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_operators/wm.py` & `fake-bpy-module-latest-20230428/bl_operators/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_previews_utils/bl_previews_render.py` & `fake-bpy-module-latest-20230428/bl_previews_utils/bl_previews_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/__init__.py` & `fake-bpy-module-latest-20230428/bl_ui/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,80 +1,80 @@
 import sys
 import typing
 import bpy_types
 
-from . import properties_physics_cloth
-from . import properties_physics_common
-from . import properties_data_modifier
-from . import properties_grease_pencil_common
-from . import properties_material_gpencil
-from . import properties_output
-from . import space_sequencer
 from . import node_add_menu_geometry
-from . import properties_data_gpencil
-from . import properties_physics_dynamicpaint
-from . import space_image
-from . import properties_scene
+from . import properties_data_pointcloud
+from . import properties_data_lightprobe
 from . import properties_data_light
-from . import properties_collection
 from . import properties_data_volume
-from . import space_filebrowser
-from . import space_node
-from . import space_statusbar
-from . import space_outliner
-from . import space_toolsystem_common
-from . import utils
-from . import space_graph
-from . import properties_mask_common
-from . import properties_paint_common
-from . import properties_data_bone
-from . import properties_data_lightprobe
-from . import properties_animviz
-from . import generic_ui_list
-from . import space_dopesheet
-from . import properties_data_speaker
+from . import space_view3d
+from . import properties_physics_common
+from . import properties_data_metaball
+from . import properties_physics_rigidbody_constraint
+from . import properties_physics_fluid
+from . import properties_material_gpencil
+from . import properties_physics_softbody
 from . import space_info
+from . import space_toolsystem_common
+from . import space_clip
+from . import properties_data_armature
 from . import properties_render
-from . import space_console
-from . import properties_object
+from . import properties_view_layer
 from . import properties_constraint
-from . import space_properties
-from . import properties_physics_rigidbody_constraint
-from . import properties_texture
-from . import properties_workspace
-from . import space_clip
-from . import space_toolsystem_toolbar
+from . import space_node
+from . import properties_world
+from . import space_userpref
 from . import space_time
-from . import space_topbar
-from . import properties_data_metaball
-from . import node_add_menu
+from . import properties_paint_common
+from . import properties_grease_pencil_common
+from . import properties_physics_field
+from . import space_statusbar
+from . import properties_object
+from . import properties_data_empty
+from . import space_spreadsheet
+from . import space_outliner
+from . import space_toolsystem_toolbar
+from . import properties_freestyle
+from . import properties_data_curve
+from . import properties_output
+from . import space_sequencer
+from . import properties_physics_rigidbody
 from . import properties_particle
-from . import space_view3d
-from . import properties_view_layer
-from . import space_nla
+from . import properties_workspace
+from . import space_dopesheet
 from . import properties_material
-from . import properties_data_pointcloud
-from . import space_spreadsheet
-from . import properties_data_lattice
-from . import properties_physics_field
+from . import properties_animviz
+from . import space_graph
 from . import space_text
-from . import properties_data_curve
-from . import properties_data_armature
-from . import properties_data_empty
-from . import properties_physics_fluid
-from . import properties_physics_softbody
-from . import properties_world
-from . import space_userpref
+from . import properties_scene
+from . import properties_physics_dynamicpaint
+from . import generic_ui_list
+from . import properties_mask_common
+from . import properties_collection
+from . import properties_physics_cloth
+from . import space_topbar
+from . import node_add_menu
+from . import space_image
+from . import space_console
 from . import space_view3d_toolbar
-from . import properties_physics_rigidbody
+from . import properties_data_gpencil
+from . import space_nla
 from . import properties_data_mesh
+from . import properties_data_shaderfx
+from . import space_filebrowser
+from . import properties_data_lattice
+from . import properties_texture
 from . import properties_data_camera
-from . import properties_freestyle
+from . import space_properties
+from . import properties_data_bone
 from . import properties_data_curves
-from . import properties_data_shaderfx
+from . import properties_data_speaker
+from . import utils
+from . import properties_data_modifier
 
 GenericType = typing.TypeVar("GenericType")
 
 
 class UI_MT_button_context_menu(bpy_types.Menu, bpy_types._GenericUI):
     bl_idname = None
     ''' '''
```

### Comparing `fake-bpy-module-latest-20230427/bl_ui/generic_ui_list.py` & `fake-bpy-module-latest-20230428/bl_ui/generic_ui_list.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/node_add_menu_geometry.py` & `fake-bpy-module-latest-20230428/bl_ui/node_add_menu_geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_animviz.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_animviz.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_collection.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_constraint.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_armature.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_bone.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_bone.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_camera.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_curve.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_curves.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_empty.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_empty.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_gpencil.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_lattice.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_light.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_light.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_lightprobe.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_lightprobe.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_mesh.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_metaball.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_metaball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_modifier.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_modifier.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_pointcloud.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_pointcloud.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_shaderfx.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_shaderfx.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_speaker.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_speaker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_data_volume.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_data_volume.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_freestyle.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_freestyle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_grease_pencil_common.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_grease_pencil_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_mask_common.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_mask_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_material.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_material_gpencil.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_material_gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_object.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_output.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_output.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_paint_common.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_paint_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_particle.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_cloth.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_common.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_dynamicpaint.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_dynamicpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_field.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_field.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_fluid.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_rigidbody.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_rigidbody_constraint.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_rigidbody_constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_physics_softbody.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_physics_softbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_render.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_scene.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_texture.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_view_layer.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_view_layer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_workspace.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/properties_world.py` & `fake-bpy-module-latest-20230428/bl_ui/properties_world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_clip.py` & `fake-bpy-module-latest-20230428/bl_ui/space_clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_console.py` & `fake-bpy-module-latest-20230428/bl_ui/space_console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_dopesheet.py` & `fake-bpy-module-latest-20230428/bl_ui/space_dopesheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_filebrowser.py` & `fake-bpy-module-latest-20230428/bl_ui/space_filebrowser.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_graph.py` & `fake-bpy-module-latest-20230428/bl_ui/space_graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_image.py` & `fake-bpy-module-latest-20230428/bl_ui/space_image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_info.py` & `fake-bpy-module-latest-20230428/bl_ui/space_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_nla.py` & `fake-bpy-module-latest-20230428/bl_ui/space_nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_node.py` & `fake-bpy-module-latest-20230428/bl_ui/space_node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_outliner.py` & `fake-bpy-module-latest-20230428/bl_ui/space_outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_properties.py` & `fake-bpy-module-latest-20230428/bl_ui/space_properties.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_sequencer.py` & `fake-bpy-module-latest-20230428/bl_ui/space_sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_spreadsheet.py` & `fake-bpy-module-latest-20230428/bl_ui/space_spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_statusbar.py` & `fake-bpy-module-latest-20230428/bl_ui/space_statusbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_text.py` & `fake-bpy-module-latest-20230428/bl_ui/space_text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_time.py` & `fake-bpy-module-latest-20230428/bl_ui/space_time.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_toolsystem_common.py` & `fake-bpy-module-latest-20230428/bl_ui/space_toolsystem_common.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_toolsystem_toolbar.py` & `fake-bpy-module-latest-20230428/bl_ui/space_toolsystem_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_topbar.py` & `fake-bpy-module-latest-20230428/bl_ui/space_topbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_userpref.py` & `fake-bpy-module-latest-20230428/bl_ui/space_userpref.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_view3d.py` & `fake-bpy-module-latest-20230428/bl_ui/space_view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/space_view3d_toolbar.py` & `fake-bpy-module-latest-20230428/bl_ui/space_view3d_toolbar.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bl_ui/utils.py` & `fake-bpy-module-latest-20230428/bl_ui/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/blf.py` & `fake-bpy-module-latest-20230428/blf.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bmesh/__init__.py` & `fake-bpy-module-latest-20230428/bmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bmesh/geometry.py` & `fake-bpy-module-latest-20230428/bmesh/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bmesh/ops.py` & `fake-bpy-module-latest-20230428/bmesh/ops.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bmesh/types.py` & `fake-bpy-module-latest-20230428/bmesh/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bmesh/utils.py` & `fake-bpy-module-latest-20230428/bmesh/utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/app/__init__.py` & `fake-bpy-module-latest-20230428/bpy/app/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
+from . import handlers
 from . import timers
-from . import icons
 from . import translations
-from . import handlers
+from . import icons
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def is_job_running(job_type: typing.Optional[str]) -> typing.Any:
     ''' Check whether a job of the given type is running.
```

### Comparing `fake-bpy-module-latest-20230427/bpy/app/handlers.py` & `fake-bpy-module-latest-20230428/bpy/app/handlers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/app/icons.py` & `fake-bpy-module-latest-20230428/bpy/app/icons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/app/timers.py` & `fake-bpy-module-latest-20230428/bpy/app/timers.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/app/translations.py` & `fake-bpy-module-latest-20230428/bpy/app/translations.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/msgbus.py` & `fake-bpy-module-latest-20230428/bpy/msgbus.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/__init__.py` & `fake-bpy-module-latest-20230428/bpy/ops/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 import sys
 import typing
-from . import curves
+from . import object
+from . import import_curve
+from . import particle
+from . import screen
+from . import anim
 from . import outliner
-from . import geometry
-from . import font
-from . import mball
-from . import scene
+from . import workspace
+from . import spreadsheet
 from . import asset
-from . import sound
-from . import boid
-from . import brush
-from . import node
-from . import render
-from . import object
-from . import sculpt_curves
-from . import info
+from . import camera
 from . import poselib
-from . import export_mesh
 from . import cloth
-from . import gpencil
-from . import import_mesh
-from . import paint
+from . import export_scene
+from . import sequencer
+from . import palette
+from . import mask
 from . import curve
-from . import wm
-from . import preferences
-from . import particle
-from . import anim
-from . import uilist
-from . import workspace
-from . import armature
+from . import action
+from . import node
+from . import image
+from . import lattice
+from . import file
 from . import dpaint
-from . import buttons
+from . import uv
+from . import render
+from . import curves
+from . import export_anim
 from . import transform
-from . import nla
-from . import screen
-from . import text
-from . import marker
-from . import file
-from . import spreadsheet
-from . import cycles
-from . import ui
-from . import view2d
-from . import export_scene
-from . import fluid
+from . import console
+from . import material
+from . import rigidbody
+from . import gpencil
 from . import view3d
-from . import paintcurve
 from . import surface
-from . import lattice
+from . import info
+from . import sound
+from . import ui
+from . import import_anim
 from . import script
+from . import brush
+from . import cachefile
+from . import font
+from . import export_mesh
+from . import fluid
+from . import gizmogroup
+from . import nla
+from . import import_scene
+from . import constraint
+from . import mball
+from . import paint
+from . import uilist
+from . import import_mesh
+from . import scene
 from . import ptcache
+from . import pose
+from . import ed
+from . import sculpt
+from . import preferences
+from . import text
 from . import texture
+from . import cycles
+from . import sculpt_curves
+from . import wm
+from . import paintcurve
+from . import collection
 from . import graph
-from . import palette
-from . import import_anim
-from . import constraint
-from . import mask
-from . import camera
-from . import gizmogroup
-from . import uv
-from . import sculpt
-from . import console
+from . import view2d
+from . import geometry
+from . import mesh
+from . import boid
+from . import marker
 from . import clip
-from . import material
+from . import buttons
 from . import world
-from . import ed
-from . import cachefile
-from . import mesh
-from . import import_curve
-from . import sequencer
-from . import export_anim
-from . import collection
-from . import rigidbody
-from . import action
-from . import image
-from . import pose
-from . import import_scene
+from . import armature
 
 GenericType = typing.TypeVar("GenericType")
```

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/action.py` & `fake-bpy-module-latest-20230428/bpy/ops/action.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/anim.py` & `fake-bpy-module-latest-20230428/bpy/ops/anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/armature.py` & `fake-bpy-module-latest-20230428/bpy/ops/armature.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/asset.py` & `fake-bpy-module-latest-20230428/bpy/ops/asset.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/boid.py` & `fake-bpy-module-latest-20230428/bpy/ops/boid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/brush.py` & `fake-bpy-module-latest-20230428/bpy/ops/brush.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/buttons.py` & `fake-bpy-module-latest-20230428/bpy/ops/buttons.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/cachefile.py` & `fake-bpy-module-latest-20230428/bpy/ops/cachefile.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/camera.py` & `fake-bpy-module-latest-20230428/bpy/ops/camera.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/clip.py` & `fake-bpy-module-latest-20230428/bpy/ops/clip.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/cloth.py` & `fake-bpy-module-latest-20230428/bpy/ops/cloth.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/collection.py` & `fake-bpy-module-latest-20230428/bpy/ops/collection.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/console.py` & `fake-bpy-module-latest-20230428/bpy/ops/console.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/constraint.py` & `fake-bpy-module-latest-20230428/bpy/ops/constraint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/curve.py` & `fake-bpy-module-latest-20230428/bpy/ops/curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/curves.py` & `fake-bpy-module-latest-20230428/bpy/ops/curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/cycles.py` & `fake-bpy-module-latest-20230428/bpy/ops/cycles.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/dpaint.py` & `fake-bpy-module-latest-20230428/bpy/ops/dpaint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/ed.py` & `fake-bpy-module-latest-20230428/bpy/ops/ed.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/export_anim.py` & `fake-bpy-module-latest-20230428/bpy/ops/export_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/export_mesh.py` & `fake-bpy-module-latest-20230428/bpy/ops/export_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/export_scene.py` & `fake-bpy-module-latest-20230428/bpy/ops/export_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/file.py` & `fake-bpy-module-latest-20230428/bpy/ops/file.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/fluid.py` & `fake-bpy-module-latest-20230428/bpy/ops/fluid.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/font.py` & `fake-bpy-module-latest-20230428/bpy/ops/font.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/geometry.py` & `fake-bpy-module-latest-20230428/bpy/ops/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/gizmogroup.py` & `fake-bpy-module-latest-20230428/bpy/ops/gizmogroup.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/gpencil.py` & `fake-bpy-module-latest-20230428/bpy/ops/gpencil.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/graph.py` & `fake-bpy-module-latest-20230428/bpy/ops/graph.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/image.py` & `fake-bpy-module-latest-20230428/bpy/ops/image.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/import_anim.py` & `fake-bpy-module-latest-20230428/bpy/ops/import_anim.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/import_curve.py` & `fake-bpy-module-latest-20230428/bpy/ops/import_curve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/import_mesh.py` & `fake-bpy-module-latest-20230428/bpy/ops/import_mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/import_scene.py` & `fake-bpy-module-latest-20230428/bpy/ops/import_scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/info.py` & `fake-bpy-module-latest-20230428/bpy/ops/info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/lattice.py` & `fake-bpy-module-latest-20230428/bpy/ops/lattice.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/marker.py` & `fake-bpy-module-latest-20230428/bpy/ops/marker.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/mask.py` & `fake-bpy-module-latest-20230428/bpy/ops/mask.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/material.py` & `fake-bpy-module-latest-20230428/bpy/ops/material.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/mball.py` & `fake-bpy-module-latest-20230428/bpy/ops/mball.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/mesh.py` & `fake-bpy-module-latest-20230428/bpy/ops/mesh.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/nla.py` & `fake-bpy-module-latest-20230428/bpy/ops/nla.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/node.py` & `fake-bpy-module-latest-20230428/bpy/ops/node.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/object.py` & `fake-bpy-module-latest-20230428/bpy/ops/object.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/outliner.py` & `fake-bpy-module-latest-20230428/bpy/ops/outliner.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/paint.py` & `fake-bpy-module-latest-20230428/bpy/ops/paint.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/paintcurve.py` & `fake-bpy-module-latest-20230428/bpy/ops/paintcurve.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/palette.py` & `fake-bpy-module-latest-20230428/bpy/ops/palette.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/particle.py` & `fake-bpy-module-latest-20230428/bpy/ops/particle.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/pose.py` & `fake-bpy-module-latest-20230428/bpy/ops/pose.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/poselib.py` & `fake-bpy-module-latest-20230428/bpy/ops/poselib.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/preferences.py` & `fake-bpy-module-latest-20230428/bpy/ops/preferences.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/ptcache.py` & `fake-bpy-module-latest-20230428/bpy/ops/ptcache.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/render.py` & `fake-bpy-module-latest-20230428/bpy/ops/render.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/rigidbody.py` & `fake-bpy-module-latest-20230428/bpy/ops/rigidbody.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/scene.py` & `fake-bpy-module-latest-20230428/bpy/ops/scene.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/screen.py` & `fake-bpy-module-latest-20230428/bpy/ops/screen.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/script.py` & `fake-bpy-module-latest-20230428/bpy/ops/script.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/sculpt.py` & `fake-bpy-module-latest-20230428/bpy/ops/sculpt.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/sculpt_curves.py` & `fake-bpy-module-latest-20230428/bpy/ops/sculpt_curves.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/sequencer.py` & `fake-bpy-module-latest-20230428/bpy/ops/sequencer.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/sound.py` & `fake-bpy-module-latest-20230428/bpy/ops/sound.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/spreadsheet.py` & `fake-bpy-module-latest-20230428/bpy/ops/spreadsheet.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/surface.py` & `fake-bpy-module-latest-20230428/bpy/ops/surface.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/text.py` & `fake-bpy-module-latest-20230428/bpy/ops/text.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/texture.py` & `fake-bpy-module-latest-20230428/bpy/ops/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/transform.py` & `fake-bpy-module-latest-20230428/bpy/ops/transform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/ui.py` & `fake-bpy-module-latest-20230428/bpy/ops/ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/uilist.py` & `fake-bpy-module-latest-20230428/bpy/ops/uilist.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/uv.py` & `fake-bpy-module-latest-20230428/bpy/ops/uv.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/view2d.py` & `fake-bpy-module-latest-20230428/bpy/ops/view2d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/view3d.py` & `fake-bpy-module-latest-20230428/bpy/ops/view3d.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/wm.py` & `fake-bpy-module-latest-20230428/bpy/ops/wm.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/workspace.py` & `fake-bpy-module-latest-20230428/bpy/ops/workspace.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/ops/world.py` & `fake-bpy-module-latest-20230428/bpy/ops/world.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/path.py` & `fake-bpy-module-latest-20230428/bpy/path.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/props.py` & `fake-bpy-module-latest-20230428/bpy/props.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/types.py` & `fake-bpy-module-latest-20230428/bpy/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,1050 +1,1050 @@
 00000000: 696d 706f 7274 2073 7973 0a69 6d70 6f72  import sys.impor
 00000010: 7420 7479 7069 6e67 0a69 6d70 6f72 7420  t typing.import 
 00000020: 6d61 7468 7574 696c 730a 696d 706f 7274  mathutils.import
 00000030: 2062 7079 0a69 6d70 6f72 7420 626c 5f75   bpy.import bl_u
-00000040: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
-00000050: 7369 6373 5f63 6c6f 7468 0a69 6d70 6f72  sics_cloth.impor
-00000060: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000070: 6573 5f70 6879 7369 6373 5f63 6f6d 6d6f  es_physics_commo
-00000080: 6e0a 696d 706f 7274 2062 6c5f 7569 2e70  n.import bl_ui.p
-00000090: 726f 7065 7274 6965 735f 6461 7461 5f6d  roperties_data_m
-000000a0: 6f64 6966 6965 720a 696d 706f 7274 2062  odifier.import b
-000000b0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000000c0: 6772 6561 7365 5f70 656e 6369 6c5f 636f  grease_pencil_co
-000000d0: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f6f  mmon.import bl_o
-000000e0: 7065 7261 746f 7273 2e73 7072 6561 6473  perators.spreads
-000000f0: 6865 6574 0a69 6d70 6f72 7420 626c 5f75  heet.import bl_u
-00000100: 692e 7072 6f70 6572 7469 6573 5f6d 6174  i.properties_mat
-00000110: 6572 6961 6c5f 6770 656e 6369 6c0a 696d  erial_gpencil.im
-00000120: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000130: 7274 6965 735f 6f75 7470 7574 0a69 6d70  rties_output.imp
-00000140: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000150: 7365 7175 656e 6365 720a 696d 706f 7274  sequencer.import
-00000160: 2062 6c5f 7569 2e6e 6f64 655f 6164 645f   bl_ui.node_add_
-00000170: 6d65 6e75 5f67 656f 6d65 7472 790a 696d  menu_geometry.im
-00000180: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000190: 7274 6965 735f 6461 7461 5f67 7065 6e63  rties_data_gpenc
-000001a0: 696c 0a69 6d70 6f72 7420 626c 5f75 692e  il.import bl_ui.
-000001b0: 7072 6f70 6572 7469 6573 5f70 6879 7369  properties_physi
-000001c0: 6373 5f64 796e 616d 6963 7061 696e 740a  cs_dynamicpaint.
-000001d0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-000001e0: 6365 5f69 6d61 6765 0a69 6d70 6f72 7420  ce_image.import 
-000001f0: 626c 5f6f 7065 7261 746f 7273 2e76 6965  bl_operators.vie
-00000200: 7733 640a 696d 706f 7274 2062 6c5f 7569  w3d.import bl_ui
-00000210: 2e70 726f 7065 7274 6965 735f 7363 656e  .properties_scen
-00000220: 650a 696d 706f 7274 2062 6c5f 6f70 6572  e.import bl_oper
-00000230: 6174 6f72 732e 776d 0a69 6d70 6f72 7420  ators.wm.import 
-00000240: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000250: 5f64 6174 615f 6c69 6768 740a 696d 706f  _data_light.impo
-00000260: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000270: 6965 735f 636f 6c6c 6563 7469 6f6e 0a69  ies_collection.i
-00000280: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000290: 6572 7469 6573 5f64 6174 615f 766f 6c75  erties_data_volu
-000002a0: 6d65 0a69 6d70 6f72 7420 626c 5f75 692e  me.import bl_ui.
-000002b0: 7370 6163 655f 6669 6c65 6272 6f77 7365  space_filebrowse
-000002c0: 720a 696d 706f 7274 2062 6c5f 7569 2e73  r.import bl_ui.s
-000002d0: 7061 6365 5f6e 6f64 650a 696d 706f 7274  pace_node.import
-000002e0: 2062 6c5f 7569 2e73 7061 6365 5f73 7461   bl_ui.space_sta
-000002f0: 7475 7362 6172 0a69 6d70 6f72 7420 626c  tusbar.import bl
-00000300: 5f75 692e 7370 6163 655f 6f75 746c 696e  _ui.space_outlin
-00000310: 6572 0a69 6d70 6f72 7420 626c 5f75 692e  er.import bl_ui.
-00000320: 7370 6163 655f 746f 6f6c 7379 7374 656d  space_toolsystem
-00000330: 5f63 6f6d 6d6f 6e0a 696d 706f 7274 2062  _common.import b
-00000340: 6c5f 6f70 6572 6174 6f72 732e 636c 6970  l_operators.clip
-00000350: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000360: 6163 655f 6772 6170 680a 696d 706f 7274  ace_graph.import
-00000370: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-00000380: 735f 6d61 736b 5f63 6f6d 6d6f 6e0a 696d  s_mask_common.im
-00000390: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-000003a0: 7274 6965 735f 7061 696e 745f 636f 6d6d  rties_paint_comm
-000003b0: 6f6e 0a69 6d70 6f72 7420 626c 5f75 692e  on.import bl_ui.
-000003c0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
-000003d0: 626f 6e65 0a69 6d70 6f72 7420 626c 5f6f  bone.import bl_o
-000003e0: 7065 7261 746f 7273 2e6f 626a 6563 740a  perators.object.
-000003f0: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
-00000400: 7065 7274 6965 735f 6461 7461 5f6c 6967  perties_data_lig
-00000410: 6874 7072 6f62 650a 696d 706f 7274 2062  htprobe.import b
-00000420: 6c5f 6f70 6572 6174 6f72 732e 616e 696d  l_operators.anim
-00000430: 0a69 6d70 6f72 7420 626c 5f75 692e 6765  .import bl_ui.ge
-00000440: 6e65 7269 635f 7569 5f6c 6973 740a 696d  neric_ui_list.im
-00000450: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
-00000460: 5f64 6f70 6573 6865 6574 0a69 6d70 6f72  _dopesheet.impor
-00000470: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000480: 6573 5f64 6174 615f 7370 6561 6b65 720a  es_data_speaker.
-00000490: 696d 706f 7274 2062 6c5f 6f70 6572 6174  import bl_operat
-000004a0: 6f72 732e 7573 6572 7072 6566 0a69 6d70  ors.userpref.imp
-000004b0: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-000004c0: 696e 666f 0a69 6d70 6f72 7420 626c 5f75  info.import bl_u
-000004d0: 692e 7072 6f70 6572 7469 6573 5f72 656e  i.properties_ren
-000004e0: 6465 720a 696d 706f 7274 2062 6c5f 7569  der.import bl_ui
-000004f0: 2e73 7061 6365 5f63 6f6e 736f 6c65 0a69  .space_console.i
-00000500: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000510: 6572 7469 6573 5f6f 626a 6563 740a 696d  erties_object.im
-00000520: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000530: 7274 6965 735f 636f 6e73 7472 6169 6e74  rties_constraint
-00000540: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-00000550: 746f 7273 2e63 6f6e 7374 7261 696e 740a  tors.constraint.
-00000560: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
-00000570: 6365 5f70 726f 7065 7274 6965 730a 696d  ce_properties.im
-00000580: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-00000590: 7274 6965 735f 7068 7973 6963 735f 7269  rties_physics_ri
-000005a0: 6769 6462 6f64 795f 636f 6e73 7472 6169  gidbody_constrai
-000005b0: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
-000005c0: 7072 6f70 6572 7469 6573 5f74 6578 7475  properties_textu
-000005d0: 7265 0a69 6d70 6f72 7420 626c 5f75 692e  re.import bl_ui.
-000005e0: 7072 6f70 6572 7469 6573 5f77 6f72 6b73  properties_works
-000005f0: 7061 6365 0a69 6d70 6f72 7420 626c 5f75  pace.import bl_u
-00000600: 692e 7370 6163 655f 636c 6970 0a69 6d70  i.space_clip.imp
-00000610: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000620: 746f 6f6c 7379 7374 656d 5f74 6f6f 6c62  toolsystem_toolb
-00000630: 6172 0a69 6d70 6f72 7420 626c 5f75 692e  ar.import bl_ui.
-00000640: 7370 6163 655f 7469 6d65 0a69 6d70 6f72  space_time.impor
-00000650: 7420 626c 5f75 692e 7370 6163 655f 746f  t bl_ui.space_to
-00000660: 7062 6172 0a69 6d70 6f72 7420 626c 5f75  pbar.import bl_u
-00000670: 690a 696d 706f 7274 2062 6c5f 7569 2e70  i.import bl_ui.p
-00000680: 726f 7065 7274 6965 735f 6461 7461 5f6d  roperties_data_m
-00000690: 6574 6162 616c 6c0a 696d 706f 7274 2062  etaball.import b
-000006a0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-000006b0: 7061 7274 6963 6c65 0a69 6d70 6f72 7420  particle.import 
-000006c0: 626c 5f75 692e 7370 6163 655f 7669 6577  bl_ui.space_view
-000006d0: 3364 0a69 6d70 6f72 7420 626c 5f75 692e  3d.import bl_ui.
-000006e0: 7072 6f70 6572 7469 6573 5f76 6965 775f  properties_view_
-000006f0: 6c61 7965 720a 696d 706f 7274 2062 6c5f  layer.import bl_
-00000700: 7569 2e73 7061 6365 5f6e 6c61 0a69 6d70  ui.space_nla.imp
-00000710: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
-00000720: 2e61 7373 6574 730a 696d 706f 7274 2062  .assets.import b
-00000730: 6c5f 6f70 6572 6174 6f72 732e 6e6f 6465  l_operators.node
-00000740: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000750: 6f70 6572 7469 6573 5f6d 6174 6572 6961  operties_materia
-00000760: 6c0a 696d 706f 7274 2062 6c5f 7569 2e70  l.import bl_ui.p
-00000770: 726f 7065 7274 6965 735f 6461 7461 5f70  roperties_data_p
-00000780: 6f69 6e74 636c 6f75 640a 696d 706f 7274  ointcloud.import
-00000790: 2062 6c5f 7569 2e73 7061 6365 5f73 7072   bl_ui.space_spr
-000007a0: 6561 6473 6865 6574 0a69 6d70 6f72 7420  eadsheet.import 
-000007b0: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-000007c0: 5f64 6174 615f 6c61 7474 6963 650a 696d  _data_lattice.im
-000007d0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
-000007e0: 7274 6965 735f 7068 7973 6963 735f 6669  rties_physics_fi
-000007f0: 656c 640a 696d 706f 7274 2062 6c5f 7569  eld.import bl_ui
-00000800: 2e73 7061 6365 5f74 6578 740a 696d 706f  .space_text.impo
-00000810: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
-00000820: 7072 6573 6574 730a 696d 706f 7274 2062  presets.import b
-00000830: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000840: 6461 7461 5f63 7572 7665 0a69 6d70 6f72  data_curve.impor
-00000850: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-00000860: 6573 5f64 6174 615f 6172 6d61 7475 7265  es_data_armature
-00000870: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
-00000880: 6f70 6572 7469 6573 5f64 6174 615f 656d  operties_data_em
-00000890: 7074 790a 696d 706f 7274 2062 6c5f 7569  pty.import bl_ui
-000008a0: 2e70 726f 7065 7274 6965 735f 7068 7973  .properties_phys
-000008b0: 6963 735f 666c 7569 640a 696d 706f 7274  ics_fluid.import
-000008c0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
-000008d0: 735f 7068 7973 6963 735f 736f 6674 626f  s_physics_softbo
-000008e0: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
-000008f0: 7072 6f70 6572 7469 6573 5f77 6f72 6c64  properties_world
-00000900: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
-00000910: 6163 655f 7573 6572 7072 6566 0a69 6d70  ace_userpref.imp
-00000920: 6f72 7420 626c 5f75 692e 7370 6163 655f  ort bl_ui.space_
-00000930: 7669 6577 3364 5f74 6f6f 6c62 6172 0a69  view3d_toolbar.i
-00000940: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-00000950: 6572 7469 6573 5f70 6879 7369 6373 5f72  erties_physics_r
-00000960: 6967 6964 626f 6479 0a69 6d70 6f72 7420  igidbody.import 
-00000970: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
-00000980: 5f64 6174 615f 6d65 7368 0a69 6d70 6f72  _data_mesh.impor
-00000990: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
-000009a0: 6573 5f64 6174 615f 6361 6d65 7261 0a69  es_data_camera.i
-000009b0: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
-000009c0: 6572 7469 6573 5f66 7265 6573 7479 6c65  erties_freestyle
-000009d0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
-000009e0: 746f 7273 2e66 7265 6573 7479 6c65 0a69  tors.freestyle.i
-000009f0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
-00000a00: 7273 2e66 696c 650a 696d 706f 7274 2062  rs.file.import b
-00000a10: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
-00000a20: 6461 7461 5f63 7572 7665 730a 696d 706f  data_curves.impo
+00000040: 692e 6e6f 6465 5f61 6464 5f6d 656e 755f  i.node_add_menu_
+00000050: 6765 6f6d 6574 7279 0a69 6d70 6f72 7420  geometry.import 
+00000060: 626c 5f75 692e 7072 6f70 6572 7469 6573  bl_ui.properties
+00000070: 5f64 6174 615f 706f 696e 7463 6c6f 7564  _data_pointcloud
+00000080: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
+00000090: 746f 7273 2e61 7373 6574 730a 696d 706f  tors.assets.impo
+000000a0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000000b0: 6965 735f 6461 7461 5f6c 6967 6874 7072  ies_data_lightpr
+000000c0: 6f62 650a 696d 706f 7274 2062 6c5f 7569  obe.import bl_ui
+000000d0: 2e70 726f 7065 7274 6965 735f 6461 7461  .properties_data
+000000e0: 5f6c 6967 6874 0a69 6d70 6f72 7420 626c  _light.import bl
+000000f0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000100: 6174 615f 766f 6c75 6d65 0a69 6d70 6f72  ata_volume.impor
+00000110: 7420 626c 5f6f 7065 7261 746f 7273 2e61  t bl_operators.a
+00000120: 6e69 6d0a 696d 706f 7274 2062 6c5f 7569  nim.import bl_ui
+00000130: 2e73 7061 6365 5f76 6965 7733 640a 696d  .space_view3d.im
+00000140: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000150: 7274 6965 735f 7068 7973 6963 735f 636f  rties_physics_co
+00000160: 6d6d 6f6e 0a69 6d70 6f72 7420 626c 5f75  mmon.import bl_u
+00000170: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000180: 615f 6d65 7461 6261 6c6c 0a69 6d70 6f72  a_metaball.impor
+00000190: 7420 626c 5f6f 7065 7261 746f 7273 2e70  t bl_operators.p
+000001a0: 7265 7365 7473 0a69 6d70 6f72 7420 626c  resets.import bl
+000001b0: 5f75 692e 7072 6f70 6572 7469 6573 5f70  _ui.properties_p
+000001c0: 6879 7369 6373 5f72 6967 6964 626f 6479  hysics_rigidbody
+000001d0: 5f63 6f6e 7374 7261 696e 740a 696d 706f  _constraint.impo
+000001e0: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+000001f0: 6965 735f 7068 7973 6963 735f 666c 7569  ies_physics_flui
+00000200: 640a 696d 706f 7274 2062 6c5f 7569 2e70  d.import bl_ui.p
+00000210: 726f 7065 7274 6965 735f 6d61 7465 7269  roperties_materi
+00000220: 616c 5f67 7065 6e63 696c 0a69 6d70 6f72  al_gpencil.impor
+00000230: 7420 626c 5f6f 7065 7261 746f 7273 2e63  t bl_operators.c
+00000240: 6f6e 7374 7261 696e 740a 696d 706f 7274  onstraint.import
+00000250: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000260: 735f 7068 7973 6963 735f 736f 6674 626f  s_physics_softbo
+00000270: 6479 0a69 6d70 6f72 7420 626c 5f75 692e  dy.import bl_ui.
+00000280: 7370 6163 655f 696e 666f 0a69 6d70 6f72  space_info.impor
+00000290: 7420 626c 5f75 692e 7370 6163 655f 746f  t bl_ui.space_to
+000002a0: 6f6c 7379 7374 656d 5f63 6f6d 6d6f 6e0a  olsystem_common.
+000002b0: 696d 706f 7274 2062 6c5f 7569 2e73 7061  import bl_ui.spa
+000002c0: 6365 5f63 6c69 700a 696d 706f 7274 2062  ce_clip.import b
+000002d0: 6c5f 7569 2e70 726f 7065 7274 6965 735f  l_ui.properties_
+000002e0: 6461 7461 5f61 726d 6174 7572 650a 696d  data_armature.im
+000002f0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000300: 7274 6965 735f 7265 6e64 6572 0a69 6d70  rties_render.imp
+00000310: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000320: 2e73 7072 6561 6473 6865 6574 0a69 6d70  .spreadsheet.imp
+00000330: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+00000340: 7469 6573 5f76 6965 775f 6c61 7965 720a  ties_view_layer.
+00000350: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000360: 7065 7274 6965 735f 636f 6e73 7472 6169  perties_constrai
+00000370: 6e74 0a69 6d70 6f72 7420 626c 5f75 692e  nt.import bl_ui.
+00000380: 7370 6163 655f 6e6f 6465 0a69 6d70 6f72  space_node.impor
+00000390: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000003a0: 6573 5f77 6f72 6c64 0a69 6d70 6f72 7420  es_world.import 
+000003b0: 626c 5f75 692e 7370 6163 655f 7573 6572  bl_ui.space_user
+000003c0: 7072 6566 0a69 6d70 6f72 7420 626c 5f75  pref.import bl_u
+000003d0: 692e 7370 6163 655f 7469 6d65 0a69 6d70  i.space_time.imp
+000003e0: 6f72 7420 626c 5f75 692e 7072 6f70 6572  ort bl_ui.proper
+000003f0: 7469 6573 5f70 6169 6e74 5f63 6f6d 6d6f  ties_paint_commo
+00000400: 6e0a 696d 706f 7274 2062 6c5f 7569 2e70  n.import bl_ui.p
+00000410: 726f 7065 7274 6965 735f 6772 6561 7365  roperties_grease
+00000420: 5f70 656e 6369 6c5f 636f 6d6d 6f6e 0a69  _pencil_common.i
+00000430: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000440: 6572 7469 6573 5f70 6879 7369 6373 5f66  erties_physics_f
+00000450: 6965 6c64 0a69 6d70 6f72 7420 626c 5f75  ield.import bl_u
+00000460: 692e 7370 6163 655f 7374 6174 7573 6261  i.space_statusba
+00000470: 720a 696d 706f 7274 2062 6c5f 7569 2e70  r.import bl_ui.p
+00000480: 726f 7065 7274 6965 735f 6f62 6a65 6374  roperties_object
+00000490: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000004a0: 6f70 6572 7469 6573 5f64 6174 615f 656d  operties_data_em
+000004b0: 7074 790a 696d 706f 7274 2062 6c5f 7569  pty.import bl_ui
+000004c0: 2e73 7061 6365 5f73 7072 6561 6473 6865  .space_spreadshe
+000004d0: 6574 0a69 6d70 6f72 7420 626c 5f6f 7065  et.import bl_ope
+000004e0: 7261 746f 7273 2e66 7265 6573 7479 6c65  rators.freestyle
+000004f0: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000500: 6163 655f 6f75 746c 696e 6572 0a69 6d70  ace_outliner.imp
+00000510: 6f72 7420 626c 5f6f 7065 7261 746f 7273  ort bl_operators
+00000520: 2e6f 626a 6563 740a 696d 706f 7274 2062  .object.import b
+00000530: 6c5f 7569 2e73 7061 6365 5f74 6f6f 6c73  l_ui.space_tools
+00000540: 7973 7465 6d5f 746f 6f6c 6261 720a 696d  ystem_toolbar.im
+00000550: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+00000560: 7274 6965 735f 6672 6565 7374 796c 650a  rties_freestyle.
+00000570: 696d 706f 7274 2062 6c5f 7569 2e70 726f  import bl_ui.pro
+00000580: 7065 7274 6965 735f 6461 7461 5f63 7572  perties_data_cur
+00000590: 7665 0a69 6d70 6f72 7420 626c 5f75 692e  ve.import bl_ui.
+000005a0: 7072 6f70 6572 7469 6573 5f6f 7574 7075  properties_outpu
+000005b0: 740a 696d 706f 7274 2062 6c5f 7569 2e73  t.import bl_ui.s
+000005c0: 7061 6365 5f73 6571 7565 6e63 6572 0a69  pace_sequencer.i
+000005d0: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+000005e0: 7273 2e76 6965 7733 640a 696d 706f 7274  rs.view3d.import
+000005f0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000600: 735f 7068 7973 6963 735f 7269 6769 6462  s_physics_rigidb
+00000610: 6f64 790a 696d 706f 7274 2062 6c5f 7569  ody.import bl_ui
+00000620: 2e70 726f 7065 7274 6965 735f 7061 7274  .properties_part
+00000630: 6963 6c65 0a69 6d70 6f72 7420 626c 5f6f  icle.import bl_o
+00000640: 7065 7261 746f 7273 2e77 6d0a 696d 706f  perators.wm.impo
+00000650: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
+00000660: 6965 735f 776f 726b 7370 6163 650a 696d  ies_workspace.im
+00000670: 706f 7274 2062 6c5f 7569 2e73 7061 6365  port bl_ui.space
+00000680: 5f64 6f70 6573 6865 6574 0a69 6d70 6f72  _dopesheet.impor
+00000690: 7420 626c 5f75 692e 7072 6f70 6572 7469  t bl_ui.properti
+000006a0: 6573 5f6d 6174 6572 6961 6c0a 696d 706f  es_material.impo
+000006b0: 7274 2062 6c5f 6f70 6572 6174 6f72 732e  rt bl_operators.
+000006c0: 7573 6572 7072 6566 0a69 6d70 6f72 7420  userpref.import 
+000006d0: 626c 5f75 692e 7370 6163 655f 6772 6170  bl_ui.space_grap
+000006e0: 680a 696d 706f 7274 2062 6c5f 7569 2e73  h.import bl_ui.s
+000006f0: 7061 6365 5f74 6578 740a 696d 706f 7274  pace_text.import
+00000700: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000710: 735f 7363 656e 650a 696d 706f 7274 2062  s_scene.import b
+00000720: 6c5f 7569 0a69 6d70 6f72 7420 626c 5f75  l_ui.import bl_u
+00000730: 692e 7072 6f70 6572 7469 6573 5f70 6879  i.properties_phy
+00000740: 7369 6373 5f64 796e 616d 6963 7061 696e  sics_dynamicpain
+00000750: 740a 696d 706f 7274 2062 6c5f 7569 2e67  t.import bl_ui.g
+00000760: 656e 6572 6963 5f75 695f 6c69 7374 0a69  eneric_ui_list.i
+00000770: 6d70 6f72 7420 626c 5f6f 7065 7261 746f  mport bl_operato
+00000780: 7273 2e66 696c 650a 696d 706f 7274 2062  rs.file.import b
+00000790: 6c5f 6f70 6572 6174 6f72 732e 636c 6970  l_operators.clip
+000007a0: 0a69 6d70 6f72 7420 626c 5f6f 7065 7261  .import bl_opera
+000007b0: 746f 7273 2e6e 6f64 650a 696d 706f 7274  tors.node.import
+000007c0: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+000007d0: 735f 6d61 736b 5f63 6f6d 6d6f 6e0a 696d  s_mask_common.im
+000007e0: 706f 7274 2062 6c5f 7569 2e70 726f 7065  port bl_ui.prope
+000007f0: 7274 6965 735f 636f 6c6c 6563 7469 6f6e  rties_collection
+00000800: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+00000810: 6f70 6572 7469 6573 5f70 6879 7369 6373  operties_physics
+00000820: 5f63 6c6f 7468 0a69 6d70 6f72 7420 626c  _cloth.import bl
+00000830: 5f75 692e 7370 6163 655f 746f 7062 6172  _ui.space_topbar
+00000840: 0a69 6d70 6f72 7420 626c 5f75 692e 7370  .import bl_ui.sp
+00000850: 6163 655f 696d 6167 650a 696d 706f 7274  ace_image.import
+00000860: 2062 6c5f 7569 2e73 7061 6365 5f63 6f6e   bl_ui.space_con
+00000870: 736f 6c65 0a69 6d70 6f72 7420 626c 5f75  sole.import bl_u
+00000880: 692e 7370 6163 655f 7669 6577 3364 5f74  i.space_view3d_t
+00000890: 6f6f 6c62 6172 0a69 6d70 6f72 7420 626c  oolbar.import bl
+000008a0: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+000008b0: 6174 615f 6770 656e 6369 6c0a 696d 706f  ata_gpencil.impo
+000008c0: 7274 2062 6c5f 7569 2e73 7061 6365 5f6e  rt bl_ui.space_n
+000008d0: 6c61 0a69 6d70 6f72 7420 626c 5f75 692e  la.import bl_ui.
+000008e0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+000008f0: 6d65 7368 0a69 6d70 6f72 7420 626c 5f75  mesh.import bl_u
+00000900: 692e 7072 6f70 6572 7469 6573 5f64 6174  i.properties_dat
+00000910: 615f 7368 6164 6572 6678 0a69 6d70 6f72  a_shaderfx.impor
+00000920: 7420 626c 5f75 692e 7370 6163 655f 6669  t bl_ui.space_fi
+00000930: 6c65 6272 6f77 7365 720a 696d 706f 7274  lebrowser.import
+00000940: 2062 6c5f 7569 2e70 726f 7065 7274 6965   bl_ui.propertie
+00000950: 735f 6461 7461 5f6c 6174 7469 6365 0a69  s_data_lattice.i
+00000960: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000970: 6572 7469 6573 5f74 6578 7475 7265 0a69  erties_texture.i
+00000980: 6d70 6f72 7420 626c 5f75 692e 7072 6f70  mport bl_ui.prop
+00000990: 6572 7469 6573 5f64 6174 615f 6361 6d65  erties_data_came
+000009a0: 7261 0a69 6d70 6f72 7420 626c 5f75 692e  ra.import bl_ui.
+000009b0: 7370 6163 655f 7072 6f70 6572 7469 6573  space_properties
+000009c0: 0a69 6d70 6f72 7420 626c 5f75 692e 7072  .import bl_ui.pr
+000009d0: 6f70 6572 7469 6573 5f64 6174 615f 626f  operties_data_bo
+000009e0: 6e65 0a69 6d70 6f72 7420 626c 5f75 692e  ne.import bl_ui.
+000009f0: 7072 6f70 6572 7469 6573 5f64 6174 615f  properties_data_
+00000a00: 6375 7276 6573 0a69 6d70 6f72 7420 626c  curves.import bl
+00000a10: 5f75 692e 7072 6f70 6572 7469 6573 5f64  _ui.properties_d
+00000a20: 6174 615f 7370 6561 6b65 720a 696d 706f  ata_speaker.impo
 00000a30: 7274 2062 6c5f 7569 2e70 726f 7065 7274  rt bl_ui.propert
-00000a40: 6965 735f 6461 7461 5f73 6861 6465 7266  ies_data_shaderf
-00000a50: 780a 0a47 656e 6572 6963 5479 7065 203d  x..GenericType =
+00000a40: 6965 735f 6461 7461 5f6d 6f64 6966 6965  ies_data_modifie
+00000a50: 720a 0a47 656e 6572 6963 5479 7065 203d  r..GenericType =
 00000a60: 2074 7970 696e 672e 5479 7065 5661 7228   typing.TypeVar(
 00000a70: 2247 656e 6572 6963 5479 7065 2229 0a0a  "GenericType")..
-00000a80: 0a63 6c61 7373 2062 7079 5f73 7472 7563  .class bpy_struc
-00000a90: 743a 0a20 2020 2027 2727 2062 7569 6c74  t:.    ''' built
-00000aa0: 2d69 6e20 6261 7365 2063 6c61 7373 2066  -in base class f
-00000ab0: 6f72 2061 6c6c 2063 6c61 7373 6573 2069  or all classes i
-00000ac0: 6e20 6270 792e 7479 7065 732e 0a20 2020  n bpy.types..   
-00000ad0: 2027 2727 0a0a 2020 2020 6964 5f64 6174   '''..    id_dat
-00000ae0: 6120 3d20 4e6f 6e65 0a20 2020 2027 2727  a = None.    '''
-00000af0: 2054 6865 2060 6270 792e 7479 7065 732e   The `bpy.types.
-00000b00: 4944 6020 6f62 6a65 6374 2074 6869 7320  ID` object this 
-00000b10: 6461 7461 626c 6f63 6b20 6973 2066 726f  datablock is fro
-00000b20: 6d20 6f72 204e 6f6e 652c 2028 6e6f 7420  m or None, (not 
-00000b30: 6176 6169 6c61 626c 6520 666f 7220 616c  available for al
-00000b40: 6c20 6461 7461 2074 7970 6573 2927 2727  l data types)'''
-00000b50: 0a0a 2020 2020 6465 6620 6173 5f70 6f69  ..    def as_poi
-00000b60: 6e74 6572 2873 656c 6629 202d 3e20 696e  nter(self) -> in
-00000b70: 743a 0a20 2020 2020 2020 2027 2727 2052  t:.        ''' R
-00000b80: 6574 7572 6e73 2074 6865 206d 656d 6f72  eturns the memor
-00000b90: 7920 6164 6472 6573 7320 7768 6963 6820  y address which 
-00000ba0: 686f 6c64 7320 6120 706f 696e 7465 7220  holds a pointer 
-00000bb0: 746f 2042 6c65 6e64 6572 2773 2069 6e74  to Blender's int
-00000bc0: 6572 6e61 6c20 6461 7461 0a0a 2020 2020  ernal data..    
-00000bd0: 2020 2020 3a72 7479 7065 3a20 696e 740a      :rtype: int.
-00000be0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000bf0: 2069 6e74 2028 6d65 6d6f 7279 2061 6464   int (memory add
-00000c00: 7265 7373 292e 0a20 2020 2020 2020 2027  ress)..        '
-00000c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00000c20: 0a20 2020 2064 6566 2064 7269 7665 725f  .    def driver_
-00000c30: 6164 6428 7365 6c66 2c0a 2020 2020 2020  add(self,.      
-00000c40: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00000c50: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
-00000c60: 616c 5b73 7472 5d2c 0a20 2020 2020 2020  al[str],.       
-00000c70: 2020 2020 2020 2020 2020 2020 696e 6465              inde
-00000c80: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00000c90: 616c 5b69 6e74 5d20 3d20 2d31 2920 2d3e  al[int] = -1) ->
-00000ca0: 2027 4643 7572 7665 273a 0a20 2020 2020   'FCurve':.     
-00000cb0: 2020 2027 2727 2041 6464 7320 6472 6976     ''' Adds driv
-00000cc0: 6572 2873 2920 746f 2074 6865 2067 6976  er(s) to the giv
-00000cd0: 656e 2070 726f 7065 7274 790a 0a20 2020  en property..   
-00000ce0: 2020 2020 203a 7061 7261 6d20 7061 7468       :param path
-00000cf0: 3a20 7061 7468 2074 6f20 7468 6520 7072  : path to the pr
-00000d00: 6f70 6572 7479 2074 6f20 6472 6976 652c  operty to drive,
-00000d10: 2061 6e61 6c6f 676f 7573 2074 6f20 7468   analogous to th
-00000d20: 6520 6663 7572 7665 2773 2064 6174 6120  e fcurve's data 
-00000d30: 7061 7468 2e0a 2020 2020 2020 2020 3a74  path..        :t
-00000d40: 7970 6520 7061 7468 3a20 7479 7069 6e67  ype path: typing
-00000d50: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00000d60: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00000d70: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
-00000d80: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00000d90: 2064 7269 7665 2e20 4465 6661 756c 7473   drive. Defaults
-00000da0: 2074 6f20 2d31 2066 6f72 2061 6c6c 2069   to -1 for all i
-00000db0: 6e64 6963 6573 206f 7220 6120 7369 6e67  ndices or a sing
-00000dc0: 6c65 2063 6861 6e6e 656c 2069 6620 7468  le channel if th
-00000dd0: 6520 7072 6f70 6572 7479 2069 7320 6e6f  e property is no
-00000de0: 7420 616e 2061 7272 6179 2e0a 2020 2020  t an array..    
-00000df0: 2020 2020 3a74 7970 6520 696e 6465 783a      :type index:
-00000e00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00000e10: 5b69 6e74 5d0a 2020 2020 2020 2020 3a72  [int].        :r
-00000e20: 7479 7065 3a20 2746 4375 7276 6527 0a20  type: 'FCurve'. 
-00000e30: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00000e40: 5468 6520 6472 6976 6572 2873 2920 6164  The driver(s) ad
-00000e50: 6465 642e 0a20 2020 2020 2020 2027 2727  ded..        '''
-00000e60: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00000e70: 2020 2064 6566 2064 7269 7665 725f 7265     def driver_re
-00000e80: 6d6f 7665 2873 656c 662c 0a20 2020 2020  move(self,.     
-00000e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ea0: 2070 6174 683a 2074 7970 696e 672e 4f70   path: typing.Op
-00000eb0: 7469 6f6e 616c 5b73 7472 5d2c 0a20 2020  tional[str],.   
-00000ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ed0: 2020 2069 6e64 6578 3a20 7479 7069 6e67     index: typing
-00000ee0: 2e4f 7074 696f 6e61 6c5b 696e 745d 203d  .Optional[int] =
-00000ef0: 202d 3129 202d 3e20 626f 6f6c 3a0a 2020   -1) -> bool:.  
-00000f00: 2020 2020 2020 2727 2720 5265 6d6f 7665        ''' Remove
-00000f10: 2064 7269 7665 7228 7329 2066 726f 6d20   driver(s) from 
-00000f20: 7468 6520 6769 7665 6e20 7072 6f70 6572  the given proper
-00000f30: 7479 0a0a 2020 2020 2020 2020 3a70 6172  ty..        :par
-00000f40: 616d 2070 6174 683a 2070 6174 6820 746f  am path: path to
-00000f50: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
-00000f60: 2064 7269 7665 2c20 616e 616c 6f67 6f75   drive, analogou
-00000f70: 7320 746f 2074 6865 2066 6375 7276 6527  s to the fcurve'
-00000f80: 7320 6461 7461 2070 6174 682e 0a20 2020  s data path..   
-00000f90: 2020 2020 203a 7479 7065 2070 6174 683a       :type path:
-00000fa0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00000fb0: 5b73 7472 5d0a 2020 2020 2020 2020 3a70  [str].        :p
-00000fc0: 6172 616d 2069 6e64 6578 3a20 6172 7261  aram index: arra
-00000fd0: 7920 696e 6465 7820 6f66 2074 6865 2070  y index of the p
-00000fe0: 726f 7065 7274 7920 6472 6976 652e 2044  roperty drive. D
-00000ff0: 6566 6175 6c74 7320 746f 202d 3120 666f  efaults to -1 fo
-00001000: 7220 616c 6c20 696e 6469 6365 7320 6f72  r all indices or
-00001010: 2061 2073 696e 676c 6520 6368 616e 6e65   a single channe
-00001020: 6c20 6966 2074 6865 2070 726f 7065 7274  l if the propert
-00001030: 7920 6973 206e 6f74 2061 6e20 6172 7261  y is not an arra
-00001040: 792e 0a20 2020 2020 2020 203a 7479 7065  y..        :type
-00001050: 2069 6e64 6578 3a20 7479 7069 6e67 2e4f   index: typing.O
-00001060: 7074 696f 6e61 6c5b 696e 745d 0a20 2020  ptional[int].   
-00001070: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00001080: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00001090: 6e3a 2053 7563 6365 7373 206f 6620 6472  n: Success of dr
-000010a0: 6976 6572 2072 656d 6f76 616c 2e0a 2020  iver removal..  
-000010b0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000010c0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-000010d0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
-000010e0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
-000010f0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
-00001100: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-00001110: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
-00001120: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
-00001130: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
-00001140: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
-00001150: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
-00001160: 6375 7374 6f6d 2070 726f 7065 7274 7920  custom property 
-00001170: 6173 7369 676e 6564 2074 6f20 6b65 7920  assigned to key 
-00001180: 6f72 2064 6566 6175 6c74 2077 6865 6e20  or default when 
-00001190: 6e6f 7420 666f 756e 6420 286d 6174 6368  not found (match
-000011a0: 6573 2050 7974 686f 6e27 7320 6469 6374  es Python's dict
-000011b0: 696f 6e61 7279 2066 756e 6374 696f 6e20  ionary function 
-000011c0: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-000011d0: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
-000011e0: 616d 206b 6579 3a20 5468 6520 6b65 7920  am key: The key 
-000011f0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00001200: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
-00001210: 7274 792e 0a20 2020 2020 2020 203a 7479  rty..        :ty
-00001220: 7065 206b 6579 3a20 7479 7069 6e67 2e4f  pe key: typing.O
-00001230: 7074 696f 6e61 6c5b 7374 725d 0a20 2020  ptional[str].   
-00001240: 2020 2020 203a 7061 7261 6d20 6465 6661       :param defa
-00001250: 756c 743a 204f 7074 696f 6e61 6c20 6172  ult: Optional ar
-00001260: 6775 6d65 6e74 2066 6f72 2074 6865 2076  gument for the v
-00001270: 616c 7565 2074 6f20 7265 7475 726e 2069  alue to return i
-00001280: 6620 2a6b 6579 2a20 6973 206e 6f74 2066  f *key* is not f
-00001290: 6f75 6e64 2e0a 2020 2020 2020 2020 3a74  ound..        :t
-000012a0: 7970 6520 6465 6661 756c 743a 2074 7970  ype default: typ
-000012b0: 696e 672e 4f70 7469 6f6e 616c 5b74 7970  ing.Optional[typ
-000012c0: 696e 672e 416e 795d 0a20 2020 2020 2020  ing.Any].       
-000012d0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-000012e0: 730a 0a20 2020 2064 6566 2069 645f 7072  s..    def id_pr
-000012f0: 6f70 6572 7469 6573 5f63 6c65 6172 2873  operties_clear(s
-00001300: 656c 6629 3a0a 2020 2020 2020 2020 2727  elf):.        ''
-00001310: 2720 0a0a 2020 2020 2020 2020 2727 270a  ' ..        '''.
-00001320: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00001330: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
-00001340: 6965 735f 656e 7375 7265 2873 656c 6629  ies_ensure(self)
-00001350: 202d 3e20 7479 7069 6e67 2e41 6e79 3a0a   -> typing.Any:.
-00001360: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00001370: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
-00001380: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
-00001390: 203a 7265 7475 726e 3a20 7468 6520 7061   :return: the pa
-000013a0: 7265 6e74 2067 726f 7570 2066 6f72 2061  rent group for a
-000013b0: 6e20 524e 4120 7374 7275 6374 2773 2063  n RNA struct's c
-000013c0: 7573 746f 6d20 4944 5072 6f70 6572 7469  ustom IDProperti
-000013d0: 6573 2e0a 2020 2020 2020 2020 2727 270a  es..        '''.
-000013e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000013f0: 2020 6465 6620 6964 5f70 726f 7065 7274    def id_propert
-00001400: 6965 735f 7569 2873 656c 662c 206b 6579  ies_ui(self, key
-00001410: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001420: 6c5b 7479 7069 6e67 2e41 6e79 5d29 202d  l[typing.Any]) -
-00001430: 3e20 7479 7069 6e67 2e41 6e79 3a0a 2020  > typing.Any:.  
-00001440: 2020 2020 2020 2727 2720 0a0a 2020 2020        ''' ..    
-00001450: 2020 2020 3a70 6172 616d 206b 6579 3a20      :param key: 
-00001460: 2053 7472 696e 6720 6e61 6d65 206f 6620   String name of 
-00001470: 7468 6520 7072 6f70 6572 7479 2e0a 2020  the property..  
-00001480: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
-00001490: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-000014a0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
-000014b0: 2020 2020 203a 7274 7970 653a 2074 7970       :rtype: typ
-000014c0: 696e 672e 416e 790a 2020 2020 2020 2020  ing.Any.        
-000014d0: 3a72 6574 7572 6e3a 2052 6574 7572 6e20  :return: Return 
-000014e0: 616e 206f 626a 6563 7420 7573 6564 2074  an object used t
-000014f0: 6f20 6d61 6e61 6765 2061 6e20 4944 5072  o manage an IDPr
-00001500: 6f70 6572 7479 2773 2055 4920 6461 7461  operty's UI data
-00001510: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00001520: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00001530: 6465 6620 6973 5f70 726f 7065 7274 795f  def is_property_
-00001540: 6869 6464 656e 2873 656c 662c 2070 726f  hidden(self, pro
-00001550: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
-00001560: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
-00001570: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
-00001580: 6973 2068 6964 6465 6e2e 0a0a 2020 2020  is hidden...    
-00001590: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-000015a0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000015b0: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
-000015c0: 7072 6f70 6572 7479 2069 7320 6869 6464  property is hidd
-000015d0: 656e 2e0a 2020 2020 2020 2020 2727 270a  en..        '''.
-000015e0: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000015f0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
-00001600: 795f 6f76 6572 7269 6461 626c 655f 6c69  y_overridable_li
-00001610: 6272 6172 7928 7365 6c66 2c20 7072 6f70  brary(self, prop
-00001620: 6572 7479 2920 2d3e 2062 6f6f 6c3a 0a20  erty) -> bool:. 
-00001630: 2020 2020 2020 2027 2727 2043 6865 636b         ''' Check
-00001640: 2069 6620 6120 7072 6f70 6572 7479 2069   if a property i
-00001650: 7320 6f76 6572 7269 6461 626c 652e 0a0a  s overridable...
-00001660: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00001670: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
-00001680: 7475 726e 3a20 5472 7565 2077 6865 6e20  turn: True when 
-00001690: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
-000016a0: 6f76 6572 7269 6461 626c 652e 0a20 2020  overridable..   
-000016b0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-000016c0: 2070 6173 730a 0a20 2020 2064 6566 2069   pass..    def i
-000016d0: 735f 7072 6f70 6572 7479 5f72 6561 646f  s_property_reado
-000016e0: 6e6c 7928 7365 6c66 2c20 7072 6f70 6572  nly(self, proper
-000016f0: 7479 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ty) -> bool:.   
-00001700: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
-00001710: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
-00001720: 7265 6164 6f6e 6c79 2e0a 0a20 2020 2020  readonly...     
-00001730: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00001740: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00001750: 2054 7275 6520 7768 656e 2074 6865 2070   True when the p
-00001760: 726f 7065 7274 7920 6973 2072 6561 646f  roperty is reado
-00001770: 6e6c 7920 286e 6f74 2077 7269 7461 626c  nly (not writabl
-00001780: 6529 2e0a 2020 2020 2020 2020 2727 270a  e)..        '''.
-00001790: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-000017a0: 2020 6465 6620 6973 5f70 726f 7065 7274    def is_propert
-000017b0: 795f 7365 7428 7365 6c66 2c20 7072 6f70  y_set(self, prop
-000017c0: 6572 7479 2c0a 2020 2020 2020 2020 2020  erty,.          
-000017d0: 2020 2020 2020 2020 2020 2020 2020 6768                gh
-000017e0: 6f73 743a 2074 7970 696e 672e 4f70 7469  ost: typing.Opti
-000017f0: 6f6e 616c 5b62 6f6f 6c5d 203d 2054 7275  onal[bool] = Tru
-00001800: 6529 202d 3e20 626f 6f6c 3a0a 2020 2020  e) -> bool:.    
-00001810: 2020 2020 2727 2720 4368 6563 6b20 6966      ''' Check if
-00001820: 2061 2070 726f 7065 7274 7920 6973 2073   a property is s
-00001830: 6574 2c20 7573 6520 666f 7220 7465 7374  et, use for test
-00001840: 696e 6720 6f70 6572 6174 6f72 2070 726f  ing operator pro
-00001850: 7065 7274 6965 732e 0a0a 2020 2020 2020  perties...      
-00001860: 2020 3a70 6172 616d 2067 686f 7374 3a20    :param ghost: 
-00001870: 5573 6564 2066 6f72 206f 7065 7261 746f  Used for operato
-00001880: 7273 2074 6861 7420 7265 2d72 756e 2077  rs that re-run w
-00001890: 6974 6820 7072 6576 696f 7573 2073 6574  ith previous set
-000018a0: 7469 6e67 732e 2049 6e20 7468 6973 2063  tings. In this c
-000018b0: 6173 6520 7468 6520 7072 6f70 6572 7479  ase the property
-000018c0: 2069 7320 6e6f 7420 6d61 726b 6564 2061   is not marked a
-000018d0: 7320 7365 742c 2079 6574 2074 6865 2076  s set, yet the v
-000018e0: 616c 7565 2066 726f 6d20 7468 6520 7072  alue from the pr
-000018f0: 6576 696f 7573 2065 7865 6375 7469 6f6e  evious execution
-00001900: 2069 7320 7573 6564 2e20 496e 2072 6172   is used. In rar
-00001910: 6520 6361 7365 7320 796f 7520 6d61 7920  e cases you may 
-00001920: 7761 6e74 2074 6f20 7365 7420 7468 6973  want to set this
-00001930: 206f 7074 696f 6e20 746f 2066 616c 7365   option to false
-00001940: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00001950: 6768 6f73 743a 2074 7970 696e 672e 4f70  ghost: typing.Op
-00001960: 7469 6f6e 616c 5b62 6f6f 6c5d 0a20 2020  tional[bool].   
-00001970: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00001980: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
-00001990: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
-000019a0: 2070 726f 7065 7274 7920 6861 7320 6265   property has be
-000019b0: 656e 2073 6574 2e0a 2020 2020 2020 2020  en set..        
-000019c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-000019d0: 0a0a 2020 2020 6465 6620 6974 656d 7328  ..    def items(
-000019e0: 7365 6c66 2920 2d3e 2074 7970 696e 672e  self) -> typing.
-000019f0: 416e 793a 0a20 2020 2020 2020 2027 2727  Any:.        '''
-00001a00: 2052 6574 7572 6e73 2074 6865 2069 7465   Returns the ite
-00001a10: 6d73 206f 6620 7468 6973 206f 626a 6563  ms of this objec
-00001a20: 7473 2063 7573 746f 6d20 7072 6f70 6572  ts custom proper
-00001a30: 7469 6573 2028 6d61 7463 6865 7320 5079  ties (matches Py
-00001a40: 7468 6f6e 2773 2064 6963 7469 6f6e 6172  thon's dictionar
-00001a50: 7920 6675 6e63 7469 6f6e 206f 6620 7468  y function of th
-00001a60: 6520 7361 6d65 206e 616d 6529 2e0a 0a20  e same name)... 
-00001a70: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-00001a80: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
-00001a90: 2020 3a72 6574 7572 6e3a 2063 7573 746f    :return: custo
-00001aa0: 6d20 7072 6f70 6572 7479 206b 6579 2c20  m property key, 
-00001ab0: 7661 6c75 6520 7061 6972 732e 0a20 2020  value pairs..   
-00001ac0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
-00001ad0: 2070 6173 730a 0a20 2020 2064 6566 206b   pass..    def k
-00001ae0: 6579 6672 616d 655f 6465 6c65 7465 280a  eyframe_delete(.
-00001af0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001b00: 2c0a 2020 2020 2020 2020 2020 2020 6461  ,.            da
-00001b10: 7461 5f70 6174 683a 2074 7970 696e 672e  ta_path: typing.
-00001b20: 4f70 7469 6f6e 616c 5b73 7472 5d2c 0a20  Optional[str],. 
-00001b30: 2020 2020 2020 2020 2020 2069 6e64 6578             index
+00000a80: 0a63 6c61 7373 2062 7079 5f70 726f 705f  .class bpy_prop_
+00000a90: 636f 6c6c 6563 7469 6f6e 2874 7970 696e  collection(typin
+00000aa0: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
+00000ab0: 6354 7970 655d 293a 0a20 2020 2027 2727  cType]):.    '''
+00000ac0: 2062 7569 6c74 2d69 6e20 636c 6173 7320   built-in class 
+00000ad0: 7573 6564 2066 6f72 2061 6c6c 2063 6f6c  used for all col
+00000ae0: 6c65 6374 696f 6e73 2e0a 2020 2020 2727  lections..    ''
+00000af0: 270a 0a20 2020 2064 6566 2066 696e 6428  '..    def find(
+00000b00: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00000b10: 672e 4f70 7469 6f6e 616c 5b73 7472 5d29  g.Optional[str])
+00000b20: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00000b30: 2027 2727 2052 6574 7572 6e73 2074 6865   ''' Returns the
+00000b40: 2069 6e64 6578 206f 6620 6120 6b65 7920   index of a key 
+00000b50: 696e 2061 2063 6f6c 6c65 6374 696f 6e20  in a collection 
+00000b60: 6f72 202d 3120 7768 656e 206e 6f74 2066  or -1 when not f
+00000b70: 6f75 6e64 2028 6d61 7463 6865 7320 5079  ound (matches Py
+00000b80: 7468 6f6e 2773 2073 7472 696e 6720 6669  thon's string fi
+00000b90: 6e64 2066 756e 6374 696f 6e20 6f66 2074  nd function of t
+00000ba0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+00000bb0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00000bc0: 6579 3a20 5468 6520 6964 656e 7469 6669  ey: The identifi
+00000bd0: 6572 2066 6f72 2074 6865 2063 6f6c 6c65  er for the colle
+00000be0: 6374 696f 6e20 6d65 6d62 6572 2e0a 2020  ction member..  
+00000bf0: 2020 2020 2020 3a74 7970 6520 6b65 793a        :type key:
+00000c00: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00000c10: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
+00000c20: 7479 7065 3a20 696e 740a 2020 2020 2020  type: int.      
+00000c30: 2020 3a72 6574 7572 6e3a 2069 6e64 6578    :return: index
+00000c40: 206f 6620 7468 6520 6b65 792e 0a20 2020   of the key..   
+00000c50: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00000c60: 2070 6173 730a 0a20 2020 2064 6566 2066   pass..    def f
+00000c70: 6f72 6561 6368 5f67 6574 2873 656c 662c  oreach_get(self,
+00000c80: 2061 7474 722c 2073 6571 293a 0a20 2020   attr, seq):.   
+00000c90: 2020 2020 2027 2727 2054 6869 7320 6973       ''' This is
+00000ca0: 2061 2066 756e 6374 696f 6e20 746f 2067   a function to g
+00000cb0: 6976 6520 6661 7374 2061 6363 6573 7320  ive fast access 
+00000cc0: 746f 2061 7474 7269 6275 7465 7320 7769  to attributes wi
+00000cd0: 7468 696e 2061 2063 6f6c 6c65 6374 696f  thin a collectio
+00000ce0: 6e2e 204f 6e6c 7920 776f 726b 7320 666f  n. Only works fo
+00000cf0: 7220 2762 6173 6963 2074 7970 6527 2070  r 'basic type' p
+00000d00: 726f 7065 7274 6965 7320 2862 6f6f 6c2c  roperties (bool,
+00000d10: 2069 6e74 2061 6e64 2066 6c6f 6174 2921   int and float)!
+00000d20: 204d 756c 7469 2d64 696d 656e 7369 6f6e   Multi-dimension
+00000d30: 616c 2061 7272 6179 7320 286c 696b 6520  al arrays (like 
+00000d40: 6172 7261 7920 6f66 2076 6563 746f 7273  array of vectors
+00000d50: 2920 7769 6c6c 2062 6520 666c 6174 7465  ) will be flatte
+00000d60: 6e65 6420 696e 746f 2073 6571 2e0a 0a20  ned into seq... 
+00000d70: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00000d80: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00000d90: 2066 6f72 6561 6368 5f73 6574 2873 656c   foreach_set(sel
+00000da0: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):. 
+00000db0: 2020 2020 2020 2027 2727 2054 6869 7320         ''' This 
+00000dc0: 6973 2061 2066 756e 6374 696f 6e20 746f  is a function to
+00000dd0: 2067 6976 6520 6661 7374 2061 6363 6573   give fast acces
+00000de0: 7320 746f 2061 7474 7269 6275 7465 7320  s to attributes 
+00000df0: 7769 7468 696e 2061 2063 6f6c 6c65 6374  within a collect
+00000e00: 696f 6e2e 204f 6e6c 7920 776f 726b 7320  ion. Only works 
+00000e10: 666f 7220 2762 6173 6963 2074 7970 6527  for 'basic type'
+00000e20: 2070 726f 7065 7274 6965 7320 2862 6f6f   properties (boo
+00000e30: 6c2c 2069 6e74 2061 6e64 2066 6c6f 6174  l, int and float
+00000e40: 2921 2073 6571 206d 7573 7420 6265 2075  )! seq must be u
+00000e50: 6e69 2d64 696d 656e 7369 6f6e 616c 2c20  ni-dimensional, 
+00000e60: 6d75 6c74 692d 6469 6d65 6e73 696f 6e61  multi-dimensiona
+00000e70: 6c20 6172 7261 7973 2028 6c69 6b65 2061  l arrays (like a
+00000e80: 7272 6179 206f 6620 7665 6374 6f72 7329  rray of vectors)
+00000e90: 2077 696c 6c20 6265 2072 652d 6372 6561   will be re-crea
+00000ea0: 7465 6420 6672 6f6d 2069 742e 0a0a 2020  ted from it...  
+00000eb0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00000ec0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00000ed0: 6765 7428 7365 6c66 2c0a 2020 2020 2020  get(self,.      
+00000ee0: 2020 2020 2020 6b65 793a 2074 7970 696e        key: typin
+00000ef0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d2c  g.Optional[str],
+00000f00: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00000f10: 6175 6c74 3a20 7479 7069 6e67 2e4f 7074  ault: typing.Opt
+00000f20: 696f 6e61 6c5b 7479 7069 6e67 2e41 6e79  ional[typing.Any
+00000f30: 5d20 3d20 4e6f 6e65 293a 0a20 2020 2020  ] = None):.     
+00000f40: 2020 2027 2727 2052 6574 7572 6e73 2074     ''' Returns t
+00000f50: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00000f60: 6974 656d 2061 7373 6967 6e65 6420 746f  item assigned to
+00000f70: 206b 6579 206f 7220 6465 6661 756c 7420   key or default 
+00000f80: 7768 656e 206e 6f74 2066 6f75 6e64 2028  when not found (
+00000f90: 6d61 7463 6865 7320 5079 7468 6f6e 2773  matches Python's
+00000fa0: 2064 6963 7469 6f6e 6172 7920 6675 6e63   dictionary func
+00000fb0: 7469 6f6e 206f 6620 7468 6520 7361 6d65  tion of the same
+00000fc0: 206e 616d 6529 2e0a 0a20 2020 2020 2020   name)...       
+00000fd0: 203a 7061 7261 6d20 6b65 793a 2054 6865   :param key: The
+00000fe0: 2069 6465 6e74 6966 6965 7220 666f 7220   identifier for 
+00000ff0: 7468 6520 636f 6c6c 6563 7469 6f6e 206d  the collection m
+00001000: 656d 6265 722e 0a20 2020 2020 2020 203a  ember..        :
+00001010: 7479 7065 206b 6579 3a20 7479 7069 6e67  type key: typing
+00001020: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
+00001030: 2020 2020 2020 203a 7061 7261 6d20 6465         :param de
+00001040: 6661 756c 743a 204f 7074 696f 6e61 6c20  fault: Optional 
+00001050: 6172 6775 6d65 6e74 2066 6f72 2074 6865  argument for the
+00001060: 2076 616c 7565 2074 6f20 7265 7475 726e   value to return
+00001070: 2069 6620 2a6b 6579 2a20 6973 206e 6f74   if *key* is not
+00001080: 2066 6f75 6e64 2e0a 2020 2020 2020 2020   found..        
+00001090: 3a74 7970 6520 6465 6661 756c 743a 2074  :type default: t
+000010a0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
+000010b0: 7970 696e 672e 416e 795d 0a20 2020 2020  yping.Any].     
+000010c0: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
+000010d0: 6173 730a 0a20 2020 2064 6566 2069 7465  ass..    def ite
+000010e0: 6d73 2873 656c 6629 202d 3e20 7479 7069  ms(self) -> typi
+000010f0: 6e67 2e4c 6973 743a 0a20 2020 2020 2020  ng.List:.       
+00001100: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
+00001110: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
+00001120: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
+00001130: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
+00001140: 6f6e 2773 2064 6963 742e 6974 656d 7328  on's dict.items(
+00001150: 2920 6675 6e63 7469 6f6e 616c 6974 7929  ) functionality)
+00001160: 2e0a 0a20 2020 2020 2020 203a 7274 7970  ...        :rtyp
+00001170: 653a 2074 7970 696e 672e 4c69 7374 0a20  e: typing.List. 
+00001180: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001190: 286b 6579 2c20 7661 6c75 6529 2070 6169  (key, value) pai
+000011a0: 7273 2066 6f72 2065 6163 6820 6d65 6d62  rs for each memb
+000011b0: 6572 206f 6620 7468 6973 2063 6f6c 6c65  er of this colle
+000011c0: 6374 696f 6e2e 0a20 2020 2020 2020 2027  ction..        '
+000011d0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000011e0: 0a20 2020 2064 6566 206b 6579 7328 7365  .    def keys(se
+000011f0: 6c66 2920 2d3e 2074 7970 696e 672e 4c69  lf) -> typing.Li
+00001200: 7374 5b73 7472 5d3a 0a20 2020 2020 2020  st[str]:.       
+00001210: 2027 2727 2052 6574 7572 6e20 7468 6520   ''' Return the 
+00001220: 6964 656e 7469 6669 6572 7320 6f66 2063  identifiers of c
+00001230: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
+00001240: 7320 286d 6174 6368 696e 6720 5079 7468  s (matching Pyth
+00001250: 6f6e 2773 2064 6963 742e 6b65 7973 2829  on's dict.keys()
+00001260: 2066 756e 6374 696f 6e61 6c69 7479 292e   functionality).
+00001270: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00001280: 3a20 7479 7069 6e67 2e4c 6973 745b 7374  : typing.List[st
+00001290: 725d 0a20 2020 2020 2020 203a 7265 7475  r].        :retu
+000012a0: 726e 3a20 7468 6520 6964 656e 7469 6669  rn: the identifi
+000012b0: 6572 7320 666f 7220 6561 6368 206d 656d  ers for each mem
+000012c0: 6265 7220 6f66 2074 6869 7320 636f 6c6c  ber of this coll
+000012d0: 6563 7469 6f6e 2e0a 2020 2020 2020 2020  ection..        
+000012e0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000012f0: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
+00001300: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+00001310: 2e4c 6973 743a 0a20 2020 2020 2020 2027  .List:.        '
+00001320: 2727 2052 6574 7572 6e20 7468 6520 7661  '' Return the va
+00001330: 6c75 6573 206f 6620 636f 6c6c 6563 7469  lues of collecti
+00001340: 6f6e 2028 6d61 7463 6869 6e67 2050 7974  on (matching Pyt
+00001350: 686f 6e27 7320 6469 6374 2e76 616c 7565  hon's dict.value
+00001360: 7328 2920 6675 6e63 7469 6f6e 616c 6974  s() functionalit
+00001370: 7929 2e0a 0a20 2020 2020 2020 203a 7274  y)...        :rt
+00001380: 7970 653a 2074 7970 696e 672e 4c69 7374  ype: typing.List
+00001390: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000013a0: 3a20 7468 6520 6d65 6d62 6572 7320 6f66  : the members of
+000013b0: 2074 6869 7320 636f 6c6c 6563 7469 6f6e   this collection
+000013c0: 2e0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
+000013d0: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+000013e0: 6465 6620 5f5f 6765 7469 7465 6d5f 5f28  def __getitem__(
+000013f0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00001400: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00001410: 5d29 202d 3e20 2747 656e 6572 6963 5479  ]) -> 'GenericTy
+00001420: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
+00001430: 200a 0a20 2020 2020 2020 203a 7061 7261   ..        :para
+00001440: 6d20 6b65 793a 200a 2020 2020 2020 2020  m key: .        
+00001450: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
+00001460: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00001470: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
+00001480: 3a20 2747 656e 6572 6963 5479 7065 270a  : 'GenericType'.
+00001490: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
+000014a0: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
+000014b0: 6620 5f5f 7365 7469 7465 6d5f 5f28 7365  f __setitem__(se
+000014c0: 6c66 2c20 6b65 793a 2074 7970 696e 672e  lf, key: typing.
+000014d0: 556e 696f 6e5b 696e 742c 2073 7472 5d2c  Union[int, str],
+000014e0: 2076 616c 7565 3a20 2747 656e 6572 6963   value: 'Generic
+000014f0: 5479 7065 2729 3a0a 2020 2020 2020 2020  Type'):.        
+00001500: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+00001510: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+00001520: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00001530: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00001540: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
+00001550: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
+00001560: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
+00001570: 2027 4765 6e65 7269 6354 7970 6527 0a20   'GenericType'. 
+00001580: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001590: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+000015a0: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
+000015b0: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
+000015c0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
+000015d0: 2d3e 2027 4765 6e65 7269 6354 7970 6527  -> 'GenericType'
+000015e0: 3a0a 2020 2020 2020 2020 2727 2720 0a0a  :.        ''' ..
+000015f0: 2020 2020 2020 2020 3a70 6172 616d 206b          :param k
+00001600: 6579 3a20 0a20 2020 2020 2020 203a 7479  ey: .        :ty
+00001610: 7065 206b 6579 3a20 7479 7069 6e67 2e55  pe key: typing.U
+00001620: 6e69 6f6e 5b69 6e74 2c20 7374 725d 0a20  nion[int, str]. 
+00001630: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
+00001640: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
+00001650: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001660: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+00001670: 5f69 7465 725f 5f28 7365 6c66 2920 2d3e  _iter__(self) ->
+00001680: 2074 7970 696e 672e 4974 6572 6174 6f72   typing.Iterator
+00001690: 5b27 4765 6e65 7269 6354 7970 6527 5d3a  ['GenericType']:
+000016a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000016b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+000016c0: 7970 696e 672e 4974 6572 6174 6f72 5b27  yping.Iterator['
+000016d0: 4765 6e65 7269 6354 7970 6527 5d0a 2020  GenericType'].  
+000016e0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+000016f0: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00001700: 5f5f 6e65 7874 5f5f 2873 656c 6629 202d  __next__(self) -
+00001710: 3e20 2747 656e 6572 6963 5479 7065 273a  > 'GenericType':
+00001720: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+00001730: 2020 2020 2020 203a 7274 7970 653a 2027         :rtype: '
+00001740: 4765 6e65 7269 6354 7970 6527 0a20 2020  GenericType'.   
+00001750: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00001760: 2070 6173 730a 0a20 2020 2064 6566 205f   pass..    def _
+00001770: 5f6c 656e 5f5f 2873 656c 6629 202d 3e20  _len__(self) -> 
+00001780: 696e 743a 0a20 2020 2020 2020 2027 2727  int:.        '''
+00001790: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
+000017a0: 653a 2069 6e74 0a20 2020 2020 2020 2027  e: int.        '
+000017b0: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+000017c0: 0a0a 636c 6173 7320 6270 795f 7374 7275  ..class bpy_stru
+000017d0: 6374 3a0a 2020 2020 2727 2720 6275 696c  ct:.    ''' buil
+000017e0: 742d 696e 2062 6173 6520 636c 6173 7320  t-in base class 
+000017f0: 666f 7220 616c 6c20 636c 6173 7365 7320  for all classes 
+00001800: 696e 2062 7079 2e74 7970 6573 2e0a 2020  in bpy.types..  
+00001810: 2020 2727 270a 0a20 2020 2069 645f 6461    '''..    id_da
+00001820: 7461 203d 204e 6f6e 650a 2020 2020 2727  ta = None.    ''
+00001830: 2720 5468 6520 6062 7079 2e74 7970 6573  ' The `bpy.types
+00001840: 2e49 4460 206f 626a 6563 7420 7468 6973  .ID` object this
+00001850: 2064 6174 6162 6c6f 636b 2069 7320 6672   datablock is fr
+00001860: 6f6d 206f 7220 4e6f 6e65 2c20 286e 6f74  om or None, (not
+00001870: 2061 7661 696c 6162 6c65 2066 6f72 2061   available for a
+00001880: 6c6c 2064 6174 6120 7479 7065 7329 2727  ll data types)''
+00001890: 270a 0a20 2020 2064 6566 2061 735f 706f  '..    def as_po
+000018a0: 696e 7465 7228 7365 6c66 2920 2d3e 2069  inter(self) -> i
+000018b0: 6e74 3a0a 2020 2020 2020 2020 2727 2720  nt:.        ''' 
+000018c0: 5265 7475 726e 7320 7468 6520 6d65 6d6f  Returns the memo
+000018d0: 7279 2061 6464 7265 7373 2077 6869 6368  ry address which
+000018e0: 2068 6f6c 6473 2061 2070 6f69 6e74 6572   holds a pointer
+000018f0: 2074 6f20 426c 656e 6465 7227 7320 696e   to Blender's in
+00001900: 7465 726e 616c 2064 6174 610a 0a20 2020  ternal data..   
+00001910: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
+00001920: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00001930: 3a20 696e 7420 286d 656d 6f72 7920 6164  : int (memory ad
+00001940: 6472 6573 7329 2e0a 2020 2020 2020 2020  dress)..        
+00001950: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+00001960: 0a0a 2020 2020 6465 6620 6472 6976 6572  ..    def driver
+00001970: 5f61 6464 2873 656c 662c 0a20 2020 2020  _add(self,.     
+00001980: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00001990: 7468 3a20 7479 7069 6e67 2e4f 7074 696f  th: typing.Optio
+000019a0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
+000019b0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+000019c0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+000019d0: 6e61 6c5b 696e 745d 203d 202d 3129 202d  nal[int] = -1) -
+000019e0: 3e20 2746 4375 7276 6527 3a0a 2020 2020  > 'FCurve':.    
+000019f0: 2020 2020 2727 2720 4164 6473 2064 7269      ''' Adds dri
+00001a00: 7665 7228 7329 2074 6f20 7468 6520 6769  ver(s) to the gi
+00001a10: 7665 6e20 7072 6f70 6572 7479 0a0a 2020  ven property..  
+00001a20: 2020 2020 2020 3a70 6172 616d 2070 6174        :param pat
+00001a30: 683a 2070 6174 6820 746f 2074 6865 2070  h: path to the p
+00001a40: 726f 7065 7274 7920 746f 2064 7269 7665  roperty to drive
+00001a50: 2c20 616e 616c 6f67 6f75 7320 746f 2074  , analogous to t
+00001a60: 6865 2066 6375 7276 6527 7320 6461 7461  he fcurve's data
+00001a70: 2070 6174 682e 0a20 2020 2020 2020 203a   path..        :
+00001a80: 7479 7065 2070 6174 683a 2074 7970 696e  type path: typin
+00001a90: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00001aa0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00001ab0: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
+00001ac0: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
+00001ad0: 7920 6472 6976 652e 2044 6566 6175 6c74  y drive. Default
+00001ae0: 7320 746f 202d 3120 666f 7220 616c 6c20  s to -1 for all 
+00001af0: 696e 6469 6365 7320 6f72 2061 2073 696e  indices or a sin
+00001b00: 676c 6520 6368 616e 6e65 6c20 6966 2074  gle channel if t
+00001b10: 6865 2070 726f 7065 7274 7920 6973 206e  he property is n
+00001b20: 6f74 2061 6e20 6172 7261 792e 0a20 2020  ot an array..   
+00001b30: 2020 2020 203a 7479 7065 2069 6e64 6578       :type index
 00001b40: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00001b50: 6c5b 696e 745d 203d 202d 312c 0a20 2020  l[int] = -1,.   
-00001b60: 2020 2020 2020 2020 2066 7261 6d65 3a20           frame: 
-00001b70: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001b80: 666c 6f61 745d 203d 2027 6270 792e 636f  float] = 'bpy.co
-00001b90: 6e74 6578 742e 7363 656e 652e 6672 616d  ntext.scene.fram
-00001ba0: 655f 6375 7272 656e 7427 2c0a 2020 2020  e_current',.    
-00001bb0: 2020 2020 2020 2020 6772 6f75 703a 2074          group: t
-00001bc0: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00001bd0: 7472 5d20 3d20 2222 2920 2d3e 2062 6f6f  tr] = "") -> boo
-00001be0: 6c3a 0a20 2020 2020 2020 2027 2727 2052  l:.        ''' R
-00001bf0: 656d 6f76 6520 6120 6b65 7966 7261 6d65  emove a keyframe
-00001c00: 2066 726f 6d20 7468 6973 2070 726f 7065   from this prope
-00001c10: 7274 6965 7320 6663 7572 7665 2e0a 0a20  rties fcurve... 
-00001c20: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
-00001c30: 7461 5f70 6174 683a 2070 6174 6820 746f  ta_path: path to
-00001c40: 2074 6865 2070 726f 7065 7274 7920 746f   the property to
-00001c50: 2072 656d 6f76 6520 6120 6b65 792c 2061   remove a key, a
-00001c60: 6e61 6c6f 676f 7573 2074 6f20 7468 6520  nalogous to the 
-00001c70: 6663 7572 7665 2773 2064 6174 6120 7061  fcurve's data pa
-00001c80: 7468 2e0a 2020 2020 2020 2020 3a74 7970  th..        :typ
-00001c90: 6520 6461 7461 5f70 6174 683a 2074 7970  e data_path: typ
-00001ca0: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00001cb0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-00001cc0: 2069 6e64 6578 3a20 6172 7261 7920 696e   index: array in
-00001cd0: 6465 7820 6f66 2074 6865 2070 726f 7065  dex of the prope
-00001ce0: 7274 7920 746f 2072 656d 6f76 6520 6120  rty to remove a 
-00001cf0: 6b65 792e 2044 6566 6175 6c74 7320 746f  key. Defaults to
-00001d00: 202d 3120 7265 6d6f 7669 6e67 2061 6c6c   -1 removing all
-00001d10: 2069 6e64 6963 6573 206f 7220 6120 7369   indices or a si
-00001d20: 6e67 6c65 2063 6861 6e6e 656c 2069 6620  ngle channel if 
-00001d30: 7468 6520 7072 6f70 6572 7479 2069 7320  the property is 
-00001d40: 6e6f 7420 616e 2061 7272 6179 2e0a 2020  not an array..  
-00001d50: 2020 2020 2020 3a74 7970 6520 696e 6465        :type inde
-00001d60: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
-00001d70: 616c 5b69 6e74 5d0a 2020 2020 2020 2020  al[int].        
-00001d80: 3a70 6172 616d 2066 7261 6d65 3a20 5468  :param frame: Th
-00001d90: 6520 6672 616d 6520 6f6e 2077 6869 6368  e frame on which
-00001da0: 2074 6865 206b 6579 6672 616d 6520 6973   the keyframe is
-00001db0: 2064 656c 6574 6564 2c20 6465 6661 756c   deleted, defaul
-00001dc0: 7469 6e67 2074 6f20 7468 6520 6375 7272  ting to the curr
-00001dd0: 656e 7420 6672 616d 652e 0a20 2020 2020  ent frame..     
-00001de0: 2020 203a 7479 7065 2066 7261 6d65 3a20     :type frame: 
-00001df0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001e00: 666c 6f61 745d 0a20 2020 2020 2020 203a  float].        :
-00001e10: 7061 7261 6d20 6772 6f75 703a 2054 6865  param group: The
-00001e20: 206e 616d 6520 6f66 2074 6865 2067 726f   name of the gro
-00001e30: 7570 2074 6865 2046 2d43 7572 7665 2073  up the F-Curve s
-00001e40: 686f 756c 6420 6265 2061 6464 6564 2074  hould be added t
-00001e50: 6f20 6966 2069 7420 646f 6573 6e27 7420  o if it doesn't 
-00001e60: 6578 6973 7420 7965 742e 0a20 2020 2020  exist yet..     
-00001e70: 2020 203a 7479 7065 2067 726f 7570 3a20     :type group: 
-00001e80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00001e90: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
-00001ea0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
-00001eb0: 2020 3a72 6574 7572 6e3a 2053 7563 6365    :return: Succe
-00001ec0: 7373 206f 6620 6b65 7966 7261 6d65 2064  ss of keyframe d
-00001ed0: 656c 6574 696f 6e2e 0a20 2020 2020 2020  eletion..       
-00001ee0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00001ef0: 730a 0a20 2020 2064 6566 206b 6579 6672  s..    def keyfr
-00001f00: 616d 655f 696e 7365 7274 280a 2020 2020  ame_insert(.    
-00001f10: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00001f20: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
-00001f30: 6174 683a 2074 7970 696e 672e 4f70 7469  ath: typing.Opti
-00001f40: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
-00001f50: 2020 2020 2020 2069 6e64 6578 3a20 7479         index: ty
-00001f60: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
-00001f70: 745d 203d 202d 312c 0a20 2020 2020 2020  t] = -1,.       
-00001f80: 2020 2020 2066 7261 6d65 3a20 7479 7069       frame: typi
-00001f90: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
-00001fa0: 745d 203d 2027 6270 792e 636f 6e74 6578  t] = 'bpy.contex
-00001fb0: 742e 7363 656e 652e 6672 616d 655f 6375  t.scene.frame_cu
-00001fc0: 7272 656e 7427 2c0a 2020 2020 2020 2020  rrent',.        
-00001fd0: 2020 2020 6772 6f75 703a 2074 7970 696e      group: typin
-00001fe0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
-00001ff0: 3d20 2222 2c0a 2020 2020 2020 2020 2020  = "",.          
-00002000: 2020 6f70 7469 6f6e 733a 2074 7970 696e    options: typin
-00002010: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
-00002020: 672e 416e 795d 203d 2027 7365 7428 2927  g.Any] = 'set()'
-00002030: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
-00002040: 2020 2027 2727 2049 6e73 6572 7420 6120     ''' Insert a 
-00002050: 6b65 7966 7261 6d65 206f 6e20 7468 6520  keyframe on the 
-00002060: 7072 6f70 6572 7479 2067 6976 656e 2c20  property given, 
-00002070: 6164 6469 6e67 2066 6375 7276 6573 2061  adding fcurves a
-00002080: 6e64 2061 6e69 6d61 7469 6f6e 2064 6174  nd animation dat
-00002090: 6120 7768 656e 206e 6563 6573 7361 7279  a when necessary
-000020a0: 2e20 5468 6973 2069 7320 7468 6520 6d6f  . This is the mo
-000020b0: 7374 2073 696d 706c 6520 6578 616d 706c  st simple exampl
-000020c0: 6520 6f66 2069 6e73 6572 7469 6e67 2061  e of inserting a
-000020d0: 206b 6579 6672 616d 6520 6672 6f6d 2070   keyframe from p
-000020e0: 7974 686f 6e2e 204e 6f74 6520 7468 6174  ython. Note that
-000020f0: 2077 6865 6e20 6b65 7969 6e67 2064 6174   when keying dat
-00002100: 6120 7061 7468 7320 7768 6963 6820 636f  a paths which co
-00002110: 6e74 6169 6e20 6e65 7374 6564 2070 726f  ntain nested pro
-00002120: 7065 7274 6965 7320 7468 6973 206d 7573  perties this mus
-00002130: 7420 6265 2064 6f6e 6520 6672 6f6d 2074  t be done from t
-00002140: 6865 2060 4944 6020 7375 6263 6c61 7373  he `ID` subclass
-00002150: 2c20 696e 2074 6869 7320 6361 7365 2074  , in this case t
-00002160: 6865 2060 4172 6d61 7475 7265 6020 7261  he `Armature` ra
-00002170: 7468 6572 2074 6861 6e20 7468 6520 626f  ther than the bo
-00002180: 6e65 2e0a 0a20 2020 2020 2020 203a 7061  ne...        :pa
-00002190: 7261 6d20 6461 7461 5f70 6174 683a 2070  ram data_path: p
-000021a0: 6174 6820 746f 2074 6865 2070 726f 7065  ath to the prope
-000021b0: 7274 7920 746f 206b 6579 2c20 616e 616c  rty to key, anal
-000021c0: 6f67 6f75 7320 746f 2074 6865 2066 6375  ogous to the fcu
-000021d0: 7276 6527 7320 6461 7461 2070 6174 682e  rve's data path.
-000021e0: 0a20 2020 2020 2020 203a 7479 7065 2064  .        :type d
-000021f0: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
-00002200: 2e4f 7074 696f 6e61 6c5b 7374 725d 0a20  .Optional[str]. 
-00002210: 2020 2020 2020 203a 7061 7261 6d20 696e         :param in
-00002220: 6465 783a 2061 7272 6179 2069 6e64 6578  dex: array index
-00002230: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
-00002240: 2074 6f20 6b65 792e 2044 6566 6175 6c74   to key. Default
-00002250: 7320 746f 202d 3120 7768 6963 6820 7769  s to -1 which wi
-00002260: 6c6c 206b 6579 2061 6c6c 2069 6e64 6963  ll key all indic
-00002270: 6573 206f 7220 6120 7369 6e67 6c65 2063  es or a single c
-00002280: 6861 6e6e 656c 2069 6620 7468 6520 7072  hannel if the pr
-00002290: 6f70 6572 7479 2069 7320 6e6f 7420 616e  operty is not an
-000022a0: 2061 7272 6179 2e0a 2020 2020 2020 2020   array..        
-000022b0: 3a74 7970 6520 696e 6465 783a 2074 7970  :type index: typ
-000022c0: 696e 672e 4f70 7469 6f6e 616c 5b69 6e74  ing.Optional[int
-000022d0: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-000022e0: 2066 7261 6d65 3a20 5468 6520 6672 616d   frame: The fram
-000022f0: 6520 6f6e 2077 6869 6368 2074 6865 206b  e on which the k
-00002300: 6579 6672 616d 6520 6973 2069 6e73 6572  eyframe is inser
-00002310: 7465 642c 2064 6566 6175 6c74 696e 6720  ted, defaulting 
-00002320: 746f 2074 6865 2063 7572 7265 6e74 2066  to the current f
-00002330: 7261 6d65 2e0a 2020 2020 2020 2020 3a74  rame..        :t
-00002340: 7970 6520 6672 616d 653a 2074 7970 696e  ype frame: typin
-00002350: 672e 4f70 7469 6f6e 616c 5b66 6c6f 6174  g.Optional[float
-00002360: 5d0a 2020 2020 2020 2020 3a70 6172 616d  ].        :param
-00002370: 2067 726f 7570 3a20 5468 6520 6e61 6d65   group: The name
-00002380: 206f 6620 7468 6520 6772 6f75 7020 7468   of the group th
-00002390: 6520 462d 4375 7276 6520 7368 6f75 6c64  e F-Curve should
-000023a0: 2062 6520 6164 6465 6420 746f 2069 6620   be added to if 
-000023b0: 6974 2064 6f65 736e 2774 2065 7869 7374  it doesn't exist
-000023c0: 2079 6574 2e0a 2020 2020 2020 2020 3a74   yet..        :t
-000023d0: 7970 6520 6772 6f75 703a 2074 7970 696e  ype group: typin
-000023e0: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-000023f0: 2020 2020 2020 2020 3a70 6172 616d 2066          :param f
-00002400: 6c61 673a 200a 2020 2020 2020 2020 3a74  lag: .        :t
-00002410: 7970 6520 666c 6167 3a20 7479 7069 6e67  ype flag: typing
-00002420: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-00002430: 2e53 6574 5d0a 2020 2020 2020 2020 3a70  .Set].        :p
-00002440: 6172 616d 206f 7074 696f 6e73 3a20 202d  aram options:  -
-00002450: 2060 6049 4e53 4552 544b 4559 5f4e 4545   ``INSERTKEY_NEE
-00002460: 4445 4460 6020 4f6e 6c79 2069 6e73 6572  DED`` Only inser
-00002470: 7420 6b65 7966 7261 6d65 7320 7768 6572  t keyframes wher
-00002480: 6520 7468 6579 2772 6520 6e65 6564 6564  e they're needed
-00002490: 2069 6e20 7468 6520 7265 6c65 7661 6e74   in the relevant
-000024a0: 2046 2d43 7572 7665 732e 202d 2060 6049   F-Curves. - ``I
-000024b0: 4e53 4552 544b 4559 5f56 4953 5541 4c60  NSERTKEY_VISUAL`
-000024c0: 6020 496e 7365 7274 206b 6579 6672 616d  ` Insert keyfram
-000024d0: 6573 2062 6173 6564 206f 6e20 2776 6973  es based on 'vis
-000024e0: 7561 6c20 7472 616e 7366 6f72 6d73 272e  ual transforms'.
-000024f0: 202d 2060 6049 4e53 4552 544b 4559 5f58   - ``INSERTKEY_X
-00002500: 595a 5f54 4f5f 5247 4260 6020 436f 6c6f  YZ_TO_RGB`` Colo
-00002510: 7220 666f 7220 6e65 776c 7920 6164 6465  r for newly adde
-00002520: 6420 7472 616e 7366 6f72 6d61 7469 6f6e  d transformation
-00002530: 2046 2d43 7572 7665 7320 284c 6f63 6174   F-Curves (Locat
-00002540: 696f 6e2c 2052 6f74 6174 696f 6e2c 2053  ion, Rotation, S
-00002550: 6361 6c65 2920 6973 2062 6173 6564 206f  cale) is based o
-00002560: 6e20 7468 6520 7472 616e 7366 6f72 6d20  n the transform 
-00002570: 6178 6973 2e20 2d20 6060 494e 5345 5254  axis. - ``INSERT
-00002580: 4b45 595f 5245 504c 4143 4560 6020 4f6e  KEY_REPLACE`` On
-00002590: 6c79 2072 6570 6c61 6365 2061 6c72 6561  ly replace alrea
-000025a0: 6479 2065 7869 7374 696e 6720 6b65 7966  dy existing keyf
-000025b0: 7261 6d65 732e 202d 2060 6049 4e53 4552  rames. - ``INSER
-000025c0: 544b 4559 5f41 5641 494c 4142 4c45 6060  TKEY_AVAILABLE``
-000025d0: 204f 6e6c 7920 696e 7365 7274 2069 6e74   Only insert int
-000025e0: 6f20 616c 7265 6164 7920 6578 6973 7469  o already existi
-000025f0: 6e67 2046 2d43 7572 7665 732e 202d 2060  ng F-Curves. - `
-00002600: 6049 4e53 4552 544b 4559 5f43 5943 4c45  `INSERTKEY_CYCLE
-00002610: 5f41 5741 5245 6060 2054 616b 6520 6379  _AWARE`` Take cy
-00002620: 636c 6963 2065 7874 7261 706f 6c61 7469  clic extrapolati
-00002630: 6f6e 2069 6e74 6f20 6163 636f 756e 7420  on into account 
-00002640: 2843 7963 6c65 2d41 7761 7265 204b 6579  (Cycle-Aware Key
-00002650: 696e 6720 6f70 7469 6f6e 292e 0a20 2020  ing option)..   
-00002660: 2020 2020 203a 7479 7065 206f 7074 696f       :type optio
-00002670: 6e73 3a20 7479 7069 6e67 2e4f 7074 696f  ns: typing.Optio
-00002680: 6e61 6c5b 7479 7069 6e67 2e41 6e79 5d0a  nal[typing.Any].
-00002690: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000026a0: 626f 6f6c 0a20 2020 2020 2020 203a 7265  bool.        :re
-000026b0: 7475 726e 3a20 5375 6363 6573 7320 6f66  turn: Success of
-000026c0: 206b 6579 6672 616d 6520 696e 7365 7274   keyframe insert
-000026d0: 696f 6e2e 0a20 2020 2020 2020 2027 2727  ion..        '''
-000026e0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-000026f0: 2020 2064 6566 206b 6579 7328 7365 6c66     def keys(self
-00002700: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
-00002710: 0a20 2020 2020 2020 2027 2727 2052 6574  .        ''' Ret
-00002720: 7572 6e73 2074 6865 206b 6579 7320 6f66  urns the keys of
-00002730: 2074 6869 7320 6f62 6a65 6374 7320 6375   this objects cu
-00002740: 7374 6f6d 2070 726f 7065 7274 6965 7320  stom properties 
-00002750: 286d 6174 6368 6573 2050 7974 686f 6e27  (matches Python'
-00002760: 7320 6469 6374 696f 6e61 7279 2066 756e  s dictionary fun
-00002770: 6374 696f 6e20 6f66 2074 6865 2073 616d  ction of the sam
-00002780: 6520 6e61 6d65 292e 0a0a 2020 2020 2020  e name)...      
-00002790: 2020 3a72 7479 7065 3a20 7479 7069 6e67    :rtype: typing
-000027a0: 2e41 6e79 0a20 2020 2020 2020 203a 7265  .Any.        :re
-000027b0: 7475 726e 3a20 6375 7374 6f6d 2070 726f  turn: custom pro
-000027c0: 7065 7274 7920 6b65 7973 2e0a 2020 2020  perty keys..    
-000027d0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-000027e0: 7061 7373 0a0a 2020 2020 6465 6620 7061  pass..    def pa
-000027f0: 7468 5f66 726f 6d5f 6964 2873 656c 662c  th_from_id(self,
-00002800: 2070 726f 7065 7274 793a 2074 7970 696e   property: typin
-00002810: 672e 4f70 7469 6f6e 616c 5b73 7472 5d20  g.Optional[str] 
-00002820: 3d20 2222 2920 2d3e 2073 7472 3a0a 2020  = "") -> str:.  
-00002830: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00002840: 7320 7468 6520 6461 7461 2070 6174 6820  s the data path 
-00002850: 6672 6f6d 2074 6865 2049 4420 746f 2074  from the ID to t
-00002860: 6869 7320 6f62 6a65 6374 2028 7374 7269  his object (stri
-00002870: 6e67 292e 0a0a 2020 2020 2020 2020 3a70  ng)...        :p
-00002880: 6172 616d 2070 726f 7065 7274 793a 204f  aram property: O
-00002890: 7074 696f 6e61 6c20 7072 6f70 6572 7479  ptional property
-000028a0: 206e 616d 6520 7768 6963 6820 6361 6e20   name which can 
-000028b0: 6265 2075 7365 6420 6966 2074 6865 2070  be used if the p
-000028c0: 6174 6820 6973 2074 6f20 6120 7072 6f70  ath is to a prop
-000028d0: 6572 7479 206f 6620 7468 6973 206f 626a  erty of this obj
-000028e0: 6563 742e 0a20 2020 2020 2020 203a 7479  ect..        :ty
-000028f0: 7065 2070 726f 7065 7274 793a 2074 7970  pe property: typ
-00002900: 696e 672e 4f70 7469 6f6e 616c 5b73 7472  ing.Optional[str
-00002910: 5d0a 2020 2020 2020 2020 3a72 7479 7065  ].        :rtype
-00002920: 3a20 7374 720a 2020 2020 2020 2020 3a72  : str.        :r
-00002930: 6574 7572 6e3a 2060 6270 792e 7479 7065  eturn: `bpy.type
-00002940: 732e 6270 795f 7374 7275 6374 2e69 645f  s.bpy_struct.id_
-00002950: 6461 7461 6020 746f 2074 6869 7320 7374  data` to this st
-00002960: 7275 6374 2061 6e64 2070 726f 7065 7274  ruct and propert
-00002970: 7920 2877 6865 6e20 6769 7665 6e29 2e0a  y (when given)..
-00002980: 2020 2020 2020 2020 2727 270a 2020 2020          '''.    
-00002990: 2020 2020 7061 7373 0a0a 2020 2020 6465      pass..    de
-000029a0: 6620 7061 7468 5f72 6573 6f6c 7665 2873  f path_resolve(s
-000029b0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-000029c0: 2020 2020 2020 2020 2020 7061 7468 3a20            path: 
-000029d0: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-000029e0: 7374 725d 2c0a 2020 2020 2020 2020 2020  str],.          
-000029f0: 2020 2020 2020 2020 2020 2063 6f65 7263             coerc
-00002a00: 653a 2074 7970 696e 672e 4f70 7469 6f6e  e: typing.Option
-00002a10: 616c 5b62 6f6f 6c5d 203d 2054 7275 6529  al[bool] = True)
-00002a20: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
-00002a30: 7475 726e 7320 7468 6520 7072 6f70 6572  turns the proper
-00002a40: 7479 2066 726f 6d20 7468 6520 7061 7468  ty from the path
-00002a50: 2c20 7261 6973 6520 616e 2065 7863 6570  , raise an excep
-00002a60: 7469 6f6e 2077 6865 6e20 6e6f 7420 666f  tion when not fo
-00002a70: 756e 642e 0a0a 2020 2020 2020 2020 3a70  und...        :p
-00002a80: 6172 616d 2070 6174 683a 2070 6174 6820  aram path: path 
-00002a90: 7768 6963 6820 7468 6973 2070 726f 7065  which this prope
-00002aa0: 7274 7920 7265 736f 6c76 6573 2e0a 2020  rty resolves..  
-00002ab0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
-00002ac0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
-00002ad0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
-00002ae0: 7061 7261 6d20 636f 6572 6365 3a20 6f70  param coerce: op
-00002af0: 7469 6f6e 616c 2061 7267 756d 656e 742c  tional argument,
-00002b00: 2077 6865 6e20 5472 7565 2c20 7468 6520   when True, the 
-00002b10: 7072 6f70 6572 7479 2077 696c 6c20 6265  property will be
-00002b20: 2063 6f6e 7665 7274 6564 2069 6e74 6f20   converted into 
-00002b30: 6974 7320 5079 7468 6f6e 2072 6570 7265  its Python repre
-00002b40: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
-00002b50: 2020 203a 7479 7065 2063 6f65 7263 653a     :type coerce:
-00002b60: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
-00002b70: 5b62 6f6f 6c5d 0a20 2020 2020 2020 2027  [bool].        '
-00002b80: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
-00002b90: 0a20 2020 2064 6566 2070 6f70 2873 656c  .    def pop(sel
-00002ba0: 662c 0a20 2020 2020 2020 2020 2020 206b  f,.            k
-00002bb0: 6579 3a20 7479 7069 6e67 2e4f 7074 696f  ey: typing.Optio
-00002bc0: 6e61 6c5b 7374 725d 2c0a 2020 2020 2020  nal[str],.      
-00002bd0: 2020 2020 2020 6465 6661 756c 743a 2074        default: t
-00002be0: 7970 696e 672e 4f70 7469 6f6e 616c 5b74  yping.Optional[t
-00002bf0: 7970 696e 672e 416e 795d 203d 204e 6f6e  yping.Any] = Non
-00002c00: 6529 3a0a 2020 2020 2020 2020 2727 2720  e):.        ''' 
-00002c10: 5265 6d6f 7665 2061 6e64 2072 6574 7572  Remove and retur
-00002c20: 6e20 7468 6520 7661 6c75 6520 6f66 2074  n the value of t
-00002c30: 6865 2063 7573 746f 6d20 7072 6f70 6572  he custom proper
-00002c40: 7479 2061 7373 6967 6e65 6420 746f 206b  ty assigned to k
-00002c50: 6579 206f 7220 6465 6661 756c 7420 7768  ey or default wh
-00002c60: 656e 206e 6f74 2066 6f75 6e64 2028 6d61  en not found (ma
-00002c70: 7463 6865 7320 5079 7468 6f6e 2773 2064  tches Python's d
-00002c80: 6963 7469 6f6e 6172 7920 6675 6e63 7469  ictionary functi
-00002c90: 6f6e 206f 6620 7468 6520 7361 6d65 206e  on of the same n
-00002ca0: 616d 6529 2e0a 0a20 2020 2020 2020 203a  ame)...        :
-00002cb0: 7061 7261 6d20 6b65 793a 2054 6865 206b  param key: The k
-00002cc0: 6579 2061 7373 6f63 6961 7465 6420 7769  ey associated wi
-00002cd0: 7468 2074 6865 2063 7573 746f 6d20 7072  th the custom pr
-00002ce0: 6f70 6572 7479 2e0a 2020 2020 2020 2020  operty..        
-00002cf0: 3a74 7970 6520 6b65 793a 2074 7970 696e  :type key: typin
-00002d00: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
-00002d10: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
-00002d20: 6566 6175 6c74 3a20 4f70 7469 6f6e 616c  efault: Optional
-00002d30: 2061 7267 756d 656e 7420 666f 7220 7468   argument for th
-00002d40: 6520 7661 6c75 6520 746f 2072 6574 7572  e value to retur
-00002d50: 6e20 6966 202a 6b65 792a 2069 7320 6e6f  n if *key* is no
-00002d60: 7420 666f 756e 642e 0a20 2020 2020 2020  t found..       
-00002d70: 203a 7479 7065 2064 6566 6175 6c74 3a20   :type default: 
-00002d80: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
-00002d90: 7479 7069 6e67 2e41 6e79 5d0a 2020 2020  typing.Any].    
-00002da0: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00002db0: 7061 7373 0a0a 2020 2020 6465 6620 7072  pass..    def pr
-00002dc0: 6f70 6572 7479 5f6f 7665 7272 6964 6162  operty_overridab
-00002dd0: 6c65 5f6c 6962 7261 7279 5f73 6574 2873  le_library_set(s
-00002de0: 656c 662c 2070 726f 7065 7274 792c 206f  elf, property, o
-00002df0: 7665 7272 6964 6162 6c65 2920 2d3e 2062  verridable) -> b
-00002e00: 6f6f 6c3a 0a20 2020 2020 2020 2027 2727  ool:.        '''
-00002e10: 2044 6566 696e 6520 6120 7072 6f70 6572   Define a proper
-00002e20: 7479 2061 7320 6f76 6572 7269 6461 626c  ty as overridabl
-00002e30: 6520 6f72 206e 6f74 2028 6f6e 6c79 2066  e or not (only f
-00002e40: 6f72 2063 7573 746f 6d20 7072 6f70 6572  or custom proper
-00002e50: 7469 6573 2129 2e0a 0a20 2020 2020 2020  ties!)...       
-00002e60: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
-00002e70: 2020 2020 2020 3a72 6574 7572 6e3a 2054        :return: T
-00002e80: 7275 6520 7768 656e 2074 6865 206f 7665  rue when the ove
-00002e90: 7272 6964 6162 6c65 2073 7461 7475 7320  rridable status 
-00002ea0: 6f66 2074 6865 2070 726f 7065 7274 7920  of the property 
-00002eb0: 7761 7320 7375 6363 6573 7366 756c 6c79  was successfully
-00002ec0: 2073 6574 2e0a 2020 2020 2020 2020 2727   set..        ''
-00002ed0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00002ee0: 2020 2020 6465 6620 7072 6f70 6572 7479      def property
-00002ef0: 5f75 6e73 6574 2873 656c 662c 2070 726f  _unset(self, pro
-00002f00: 7065 7274 7929 3a0a 2020 2020 2020 2020  perty):.        
-00002f10: 2727 2720 556e 7365 7420 6120 7072 6f70  ''' Unset a prop
-00002f20: 6572 7479 2c20 7769 6c6c 2075 7365 2064  erty, will use d
-00002f30: 6566 6175 6c74 2076 616c 7565 2061 6674  efault value aft
-00002f40: 6572 7761 7264 2e0a 0a20 2020 2020 2020  erward...       
-00002f50: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
-00002f60: 730a 0a20 2020 2064 6566 2074 7970 655f  s..    def type_
-00002f70: 7265 6361 7374 2873 656c 6629 202d 3e20  recast(self) -> 
-00002f80: 2762 7079 5f73 7472 7563 7427 3a0a 2020  'bpy_struct':.  
-00002f90: 2020 2020 2020 2727 2720 5265 7475 726e        ''' Return
-00002fa0: 2061 206e 6577 2069 6e73 7461 6e63 652c   a new instance,
-00002fb0: 2074 6869 7320 6973 206e 6565 6465 6420   this is needed 
-00002fc0: 6265 6361 7573 6520 7479 7065 7320 7375  because types su
-00002fd0: 6368 2061 7320 7465 7874 7572 6573 2063  ch as textures c
-00002fe0: 616e 2062 6520 6368 616e 6765 6420 6174  an be changed at
-00002ff0: 2072 756e 7469 6d65 2e0a 0a20 2020 2020   runtime...     
-00003000: 2020 203a 7274 7970 653a 2027 6270 795f     :rtype: 'bpy_
-00003010: 7374 7275 6374 270a 2020 2020 2020 2020  struct'.        
-00003020: 3a72 6574 7572 6e3a 2061 206e 6577 2069  :return: a new i
-00003030: 6e73 7461 6e63 6520 6f66 2074 6869 7320  nstance of this 
-00003040: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00003050: 7479 7065 2069 6e69 7469 616c 697a 6564  type initialized
-00003060: 2061 6761 696e 2e0a 2020 2020 2020 2020   again..        
-00003070: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
-00003080: 0a0a 2020 2020 6465 6620 7661 6c75 6573  ..    def values
-00003090: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
-000030a0: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
-000030b0: 2720 5265 7475 726e 7320 7468 6520 7661  ' Returns the va
-000030c0: 6c75 6573 206f 6620 7468 6973 206f 626a  lues of this obj
-000030d0: 6563 7473 2063 7573 746f 6d20 7072 6f70  ects custom prop
-000030e0: 6572 7469 6573 2028 6d61 7463 6865 7320  erties (matches 
-000030f0: 5079 7468 6f6e 2773 2064 6963 7469 6f6e  Python's diction
-00003100: 6172 7920 6675 6e63 7469 6f6e 206f 6620  ary function of 
-00003110: 7468 6520 7361 6d65 206e 616d 6529 2e0a  the same name)..
-00003120: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00003130: 2074 7970 696e 672e 416e 790a 2020 2020   typing.Any.    
-00003140: 2020 2020 3a72 6574 7572 6e3a 2063 7573      :return: cus
-00003150: 746f 6d20 7072 6f70 6572 7479 2076 616c  tom property val
-00003160: 7565 732e 0a20 2020 2020 2020 2027 2727  ues..        '''
-00003170: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
-00003180: 2020 2064 6566 205f 5f67 6574 6974 656d     def __getitem
-00003190: 5f5f 2873 656c 662c 206b 6579 3a20 7479  __(self, key: ty
-000031a0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-000031b0: 7374 725d 2920 2d3e 2027 7479 7069 6e67  str]) -> 'typing
-000031c0: 2e41 6e79 273a 0a20 2020 2020 2020 2027  .Any':.        '
-000031d0: 2727 200a 0a20 2020 2020 2020 203a 7061  '' ..        :pa
-000031e0: 7261 6d20 6b65 793a 200a 2020 2020 2020  ram key: .      
-000031f0: 2020 3a74 7970 6520 6b65 793a 2074 7970    :type key: typ
-00003200: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003210: 7472 5d0a 2020 2020 2020 2020 3a72 7479  tr].        :rty
-00003220: 7065 3a20 2774 7970 696e 672e 416e 7927  pe: 'typing.Any'
-00003230: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003240: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003250: 6566 205f 5f73 6574 6974 656d 5f5f 2873  ef __setitem__(s
-00003260: 656c 662c 206b 6579 3a20 7479 7069 6e67  elf, key: typing
-00003270: 2e55 6e69 6f6e 5b69 6e74 2c20 7374 725d  .Union[int, str]
-00003280: 2c20 7661 6c75 653a 2027 7479 7069 6e67  , value: 'typing
-00003290: 2e41 6e79 2729 3a0a 2020 2020 2020 2020  .Any'):.        
-000032a0: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
-000032b0: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
-000032c0: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-000032d0: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
-000032e0: 7374 725d 0a20 2020 2020 2020 203a 7061  str].        :pa
-000032f0: 7261 6d20 7661 6c75 653a 200a 2020 2020  ram value: .    
-00003300: 2020 2020 3a74 7970 6520 7661 6c75 653a      :type value:
-00003310: 2027 7479 7069 6e67 2e41 6e79 270a 2020   'typing.Any'.  
-00003320: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00003330: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
-00003340: 5f5f 6465 6c69 7465 6d5f 5f28 7365 6c66  __delitem__(self
-00003350: 2c20 6b65 793a 2074 7970 696e 672e 556e  , key: typing.Un
-00003360: 696f 6e5b 696e 742c 2073 7472 5d29 202d  ion[int, str]) -
-00003370: 3e20 2774 7970 696e 672e 416e 7927 3a0a  > 'typing.Any':.
-00003380: 2020 2020 2020 2020 2727 2720 0a0a 2020          ''' ..  
-00003390: 2020 2020 2020 3a70 6172 616d 206b 6579        :param key
-000033a0: 3a20 0a20 2020 2020 2020 203a 7479 7065  : .        :type
-000033b0: 206b 6579 3a20 7479 7069 6e67 2e55 6e69   key: typing.Uni
-000033c0: 6f6e 5b69 6e74 2c20 7374 725d 0a20 2020  on[int, str].   
-000033d0: 2020 2020 203a 7274 7970 653a 2027 7479       :rtype: 'ty
-000033e0: 7069 6e67 2e41 6e79 270a 2020 2020 2020  ping.Any'.      
-000033f0: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
-00003400: 7373 0a0a 0a63 6c61 7373 2062 7079 5f70  ss...class bpy_p
-00003410: 726f 705f 636f 6c6c 6563 7469 6f6e 2874  rop_collection(t
-00003420: 7970 696e 672e 4765 6e65 7269 635b 4765  yping.Generic[Ge
-00003430: 6e65 7269 6354 7970 655d 293a 0a20 2020  nericType]):.   
-00003440: 2027 2727 2062 7569 6c74 2d69 6e20 636c   ''' built-in cl
-00003450: 6173 7320 7573 6564 2066 6f72 2061 6c6c  ass used for all
-00003460: 2063 6f6c 6c65 6374 696f 6e73 2e0a 2020   collections..  
-00003470: 2020 2727 270a 0a20 2020 2064 6566 2066    '''..    def f
-00003480: 696e 6428 7365 6c66 2c20 6b65 793a 2074  ind(self, key: t
-00003490: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-000034a0: 7472 5d29 202d 3e20 696e 743a 0a20 2020  tr]) -> int:.   
-000034b0: 2020 2020 2027 2727 2052 6574 7572 6e73       ''' Returns
-000034c0: 2074 6865 2069 6e64 6578 206f 6620 6120   the index of a 
-000034d0: 6b65 7920 696e 2061 2063 6f6c 6c65 6374  key in a collect
-000034e0: 696f 6e20 6f72 202d 3120 7768 656e 206e  ion or -1 when n
-000034f0: 6f74 2066 6f75 6e64 2028 6d61 7463 6865  ot found (matche
-00003500: 7320 5079 7468 6f6e 2773 2073 7472 696e  s Python's strin
-00003510: 6720 6669 6e64 2066 756e 6374 696f 6e20  g find function 
-00003520: 6f66 2074 6865 2073 616d 6520 6e61 6d65  of the same name
-00003530: 292e 0a0a 2020 2020 2020 2020 3a70 6172  )...        :par
-00003540: 616d 206b 6579 3a20 5468 6520 6964 656e  am key: The iden
-00003550: 7469 6669 6572 2066 6f72 2074 6865 2063  tifier for the c
-00003560: 6f6c 6c65 6374 696f 6e20 6d65 6d62 6572  ollection member
-00003570: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003580: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
-00003590: 6f6e 616c 5b73 7472 5d0a 2020 2020 2020  onal[str].      
-000035a0: 2020 3a72 7479 7065 3a20 696e 740a 2020    :rtype: int.  
-000035b0: 2020 2020 2020 3a72 6574 7572 6e3a 2069        :return: i
-000035c0: 6e64 6578 206f 6620 7468 6520 6b65 792e  ndex of the key.
-000035d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000035e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000035f0: 6566 2066 6f72 6561 6368 5f67 6574 2873  ef foreach_get(s
-00003600: 656c 662c 2061 7474 722c 2073 6571 293a  elf, attr, seq):
-00003610: 0a20 2020 2020 2020 2027 2727 2054 6869  .        ''' Thi
-00003620: 7320 6973 2061 2066 756e 6374 696f 6e20  s is a function 
-00003630: 746f 2067 6976 6520 6661 7374 2061 6363  to give fast acc
-00003640: 6573 7320 746f 2061 7474 7269 6275 7465  ess to attribute
-00003650: 7320 7769 7468 696e 2061 2063 6f6c 6c65  s within a colle
-00003660: 6374 696f 6e2e 204f 6e6c 7920 776f 726b  ction. Only work
-00003670: 7320 666f 7220 2762 6173 6963 2074 7970  s for 'basic typ
-00003680: 6527 2070 726f 7065 7274 6965 7320 2862  e' properties (b
-00003690: 6f6f 6c2c 2069 6e74 2061 6e64 2066 6c6f  ool, int and flo
-000036a0: 6174 2921 204d 756c 7469 2d64 696d 656e  at)! Multi-dimen
-000036b0: 7369 6f6e 616c 2061 7272 6179 7320 286c  sional arrays (l
-000036c0: 696b 6520 6172 7261 7920 6f66 2076 6563  ike array of vec
-000036d0: 746f 7273 2920 7769 6c6c 2062 6520 666c  tors) will be fl
-000036e0: 6174 7465 6e65 6420 696e 746f 2073 6571  attened into seq
-000036f0: 2e0a 0a20 2020 2020 2020 2027 2727 0a20  ...        '''. 
-00003700: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003710: 2064 6566 2066 6f72 6561 6368 5f73 6574   def foreach_set
-00003720: 2873 656c 662c 2061 7474 722c 2073 6571  (self, attr, seq
-00003730: 293a 0a20 2020 2020 2020 2027 2727 2054  ):.        ''' T
-00003740: 6869 7320 6973 2061 2066 756e 6374 696f  his is a functio
-00003750: 6e20 746f 2067 6976 6520 6661 7374 2061  n to give fast a
-00003760: 6363 6573 7320 746f 2061 7474 7269 6275  ccess to attribu
-00003770: 7465 7320 7769 7468 696e 2061 2063 6f6c  tes within a col
-00003780: 6c65 6374 696f 6e2e 204f 6e6c 7920 776f  lection. Only wo
-00003790: 726b 7320 666f 7220 2762 6173 6963 2074  rks for 'basic t
-000037a0: 7970 6527 2070 726f 7065 7274 6965 7320  ype' properties 
-000037b0: 2862 6f6f 6c2c 2069 6e74 2061 6e64 2066  (bool, int and f
-000037c0: 6c6f 6174 2921 2073 6571 206d 7573 7420  loat)! seq must 
-000037d0: 6265 2075 6e69 2d64 696d 656e 7369 6f6e  be uni-dimension
-000037e0: 616c 2c20 6d75 6c74 692d 6469 6d65 6e73  al, multi-dimens
-000037f0: 696f 6e61 6c20 6172 7261 7973 2028 6c69  ional arrays (li
-00003800: 6b65 2061 7272 6179 206f 6620 7665 6374  ke array of vect
-00003810: 6f72 7329 2077 696c 6c20 6265 2072 652d  ors) will be re-
-00003820: 6372 6561 7465 6420 6672 6f6d 2069 742e  created from it.
-00003830: 0a0a 2020 2020 2020 2020 2727 270a 2020  ..        '''.  
-00003840: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00003850: 6465 6620 6765 7428 7365 6c66 2c0a 2020  def get(self,.  
-00003860: 2020 2020 2020 2020 2020 6b65 793a 2074            key: t
-00003870: 7970 696e 672e 4f70 7469 6f6e 616c 5b73  yping.Optional[s
-00003880: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-00003890: 2064 6566 6175 6c74 3a20 7479 7069 6e67   default: typing
-000038a0: 2e4f 7074 696f 6e61 6c5b 7479 7069 6e67  .Optional[typing
-000038b0: 2e41 6e79 5d20 3d20 4e6f 6e65 293a 0a20  .Any] = None):. 
-000038c0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
-000038d0: 6e73 2074 6865 2076 616c 7565 206f 6620  ns the value of 
-000038e0: 7468 6520 6974 656d 2061 7373 6967 6e65  the item assigne
-000038f0: 6420 746f 206b 6579 206f 7220 6465 6661  d to key or defa
-00003900: 756c 7420 7768 656e 206e 6f74 2066 6f75  ult when not fou
-00003910: 6e64 2028 6d61 7463 6865 7320 5079 7468  nd (matches Pyth
-00003920: 6f6e 2773 2064 6963 7469 6f6e 6172 7920  on's dictionary 
-00003930: 6675 6e63 7469 6f6e 206f 6620 7468 6520  function of the 
-00003940: 7361 6d65 206e 616d 6529 2e0a 0a20 2020  same name)...   
-00003950: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
-00003960: 2054 6865 2069 6465 6e74 6966 6965 7220   The identifier 
-00003970: 666f 7220 7468 6520 636f 6c6c 6563 7469  for the collecti
-00003980: 6f6e 206d 656d 6265 722e 0a20 2020 2020  on member..     
-00003990: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
-000039a0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
-000039b0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
-000039c0: 6d20 6465 6661 756c 743a 204f 7074 696f  m default: Optio
-000039d0: 6e61 6c20 6172 6775 6d65 6e74 2066 6f72  nal argument for
-000039e0: 2074 6865 2076 616c 7565 2074 6f20 7265   the value to re
-000039f0: 7475 726e 2069 6620 2a6b 6579 2a20 6973  turn if *key* is
-00003a00: 206e 6f74 2066 6f75 6e64 2e0a 2020 2020   not found..    
-00003a10: 2020 2020 3a74 7970 6520 6465 6661 756c      :type defaul
-00003a20: 743a 2074 7970 696e 672e 4f70 7469 6f6e  t: typing.Option
-00003a30: 616c 5b74 7970 696e 672e 416e 795d 0a20  al[typing.Any]. 
-00003a40: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-00003a50: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
-00003a60: 2069 7465 6d73 2873 656c 6629 202d 3e20   items(self) -> 
-00003a70: 7479 7069 6e67 2e4c 6973 743a 0a20 2020  typing.List:.   
-00003a80: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
-00003a90: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
-00003aa0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
-00003ab0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
-00003ac0: 5079 7468 6f6e 2773 2064 6963 742e 6974  Python's dict.it
-00003ad0: 656d 7328 2920 6675 6e63 7469 6f6e 616c  ems() functional
-00003ae0: 6974 7929 2e0a 0a20 2020 2020 2020 203a  ity)...        :
-00003af0: 7274 7970 653a 2074 7970 696e 672e 4c69  rtype: typing.Li
-00003b00: 7374 0a20 2020 2020 2020 203a 7265 7475  st.        :retu
-00003b10: 726e 3a20 286b 6579 2c20 7661 6c75 6529  rn: (key, value)
-00003b20: 2070 6169 7273 2066 6f72 2065 6163 6820   pairs for each 
-00003b30: 6d65 6d62 6572 206f 6620 7468 6973 2063  member of this c
-00003b40: 6f6c 6c65 6374 696f 6e2e 0a20 2020 2020  ollection..     
-00003b50: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
-00003b60: 6173 730a 0a20 2020 2064 6566 206b 6579  ass..    def key
-00003b70: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
-00003b80: 672e 4c69 7374 5b73 7472 5d3a 0a20 2020  g.List[str]:.   
-00003b90: 2020 2020 2027 2727 2052 6574 7572 6e20       ''' Return 
-00003ba0: 7468 6520 6964 656e 7469 6669 6572 7320  the identifiers 
-00003bb0: 6f66 2063 6f6c 6c65 6374 696f 6e20 6d65  of collection me
-00003bc0: 6d62 6572 7320 286d 6174 6368 696e 6720  mbers (matching 
-00003bd0: 5079 7468 6f6e 2773 2064 6963 742e 6b65  Python's dict.ke
-00003be0: 7973 2829 2066 756e 6374 696f 6e61 6c69  ys() functionali
-00003bf0: 7479 292e 0a0a 2020 2020 2020 2020 3a72  ty)...        :r
-00003c00: 7479 7065 3a20 7479 7069 6e67 2e4c 6973  type: typing.Lis
-00003c10: 745b 7374 725d 0a20 2020 2020 2020 203a  t[str].        :
-00003c20: 7265 7475 726e 3a20 7468 6520 6964 656e  return: the iden
-00003c30: 7469 6669 6572 7320 666f 7220 6561 6368  tifiers for each
-00003c40: 206d 656d 6265 7220 6f66 2074 6869 7320   member of this 
-00003c50: 636f 6c6c 6563 7469 6f6e 2e0a 2020 2020  collection..    
-00003c60: 2020 2020 2727 270a 2020 2020 2020 2020      '''.        
-00003c70: 7061 7373 0a0a 2020 2020 6465 6620 7661  pass..    def va
-00003c80: 6c75 6573 2873 656c 6629 202d 3e20 7479  lues(self) -> ty
-00003c90: 7069 6e67 2e4c 6973 743a 0a20 2020 2020  ping.List:.     
-00003ca0: 2020 2027 2727 2052 6574 7572 6e20 7468     ''' Return th
-00003cb0: 6520 7661 6c75 6573 206f 6620 636f 6c6c  e values of coll
-00003cc0: 6563 7469 6f6e 2028 6d61 7463 6869 6e67  ection (matching
-00003cd0: 2050 7974 686f 6e27 7320 6469 6374 2e76   Python's dict.v
-00003ce0: 616c 7565 7328 2920 6675 6e63 7469 6f6e  alues() function
-00003cf0: 616c 6974 7929 2e0a 0a20 2020 2020 2020  ality)...       
-00003d00: 203a 7274 7970 653a 2074 7970 696e 672e   :rtype: typing.
-00003d10: 4c69 7374 0a20 2020 2020 2020 203a 7265  List.        :re
-00003d20: 7475 726e 3a20 7468 6520 6d65 6d62 6572  turn: the member
-00003d30: 7320 6f66 2074 6869 7320 636f 6c6c 6563  s of this collec
-00003d40: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
-00003d50: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
-00003d60: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
-00003d70: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
-00003d80: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00003d90: 2073 7472 5d29 202d 3e20 2747 656e 6572   str]) -> 'Gener
-00003da0: 6963 5479 7065 273a 0a20 2020 2020 2020  icType':.       
-00003db0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00003dc0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
-00003dd0: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
-00003de0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
-00003df0: 2073 7472 5d0a 2020 2020 2020 2020 3a72   str].        :r
-00003e00: 7479 7065 3a20 2747 656e 6572 6963 5479  type: 'GenericTy
-00003e10: 7065 270a 2020 2020 2020 2020 2727 270a  pe'.        '''.
-00003e20: 2020 2020 2020 2020 7061 7373 0a0a 2020          pass..  
-00003e30: 2020 6465 6620 5f5f 7365 7469 7465 6d5f    def __setitem_
-00003e40: 5f28 7365 6c66 2c20 6b65 793a 2074 7970  _(self, key: typ
-00003e50: 696e 672e 556e 696f 6e5b 696e 742c 2073  ing.Union[int, s
-00003e60: 7472 5d2c 2076 616c 7565 3a20 2747 656e  tr], value: 'Gen
-00003e70: 6572 6963 5479 7065 2729 3a0a 2020 2020  ericType'):.    
-00003e80: 2020 2020 2727 2720 0a0a 2020 2020 2020      ''' ..      
-00003e90: 2020 3a70 6172 616d 206b 6579 3a20 0a20    :param key: . 
-00003ea0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
-00003eb0: 3a20 7479 7069 6e67 2e55 6e69 6f6e 5b69  : typing.Union[i
-00003ec0: 6e74 2c20 7374 725d 0a20 2020 2020 2020  nt, str].       
-00003ed0: 203a 7061 7261 6d20 7661 6c75 653a 200a   :param value: .
-00003ee0: 2020 2020 2020 2020 3a74 7970 6520 7661          :type va
-00003ef0: 6c75 653a 2027 4765 6e65 7269 6354 7970  lue: 'GenericTyp
-00003f00: 6527 0a20 2020 2020 2020 2027 2727 0a20  e'.        '''. 
-00003f10: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-00003f20: 2064 6566 205f 5f64 656c 6974 656d 5f5f   def __delitem__
-00003f30: 2873 656c 662c 206b 6579 3a20 7479 7069  (self, key: typi
-00003f40: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003f50: 725d 2920 2d3e 2027 4765 6e65 7269 6354  r]) -> 'GenericT
-00003f60: 7970 6527 3a0a 2020 2020 2020 2020 2727  ype':.        ''
-00003f70: 2720 0a0a 2020 2020 2020 2020 3a70 6172  ' ..        :par
-00003f80: 616d 206b 6579 3a20 0a20 2020 2020 2020  am key: .       
-00003f90: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
-00003fa0: 6e67 2e55 6e69 6f6e 5b69 6e74 2c20 7374  ng.Union[int, st
-00003fb0: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
-00003fc0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
-00003fd0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-00003fe0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-00003ff0: 6566 205f 5f69 7465 725f 5f28 7365 6c66  ef __iter__(self
-00004000: 2920 2d3e 2074 7970 696e 672e 4974 6572  ) -> typing.Iter
-00004010: 6174 6f72 5b27 4765 6e65 7269 6354 7970  ator['GenericTyp
-00004020: 6527 5d3a 0a20 2020 2020 2020 2027 2727  e']:.        '''
-00004030: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
-00004040: 653a 2074 7970 696e 672e 4974 6572 6174  e: typing.Iterat
-00004050: 6f72 5b27 4765 6e65 7269 6354 7970 6527  or['GenericType'
-00004060: 5d0a 2020 2020 2020 2020 2727 270a 2020  ].        '''.  
-00004070: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
-00004080: 6465 6620 5f5f 6e65 7874 5f5f 2873 656c  def __next__(sel
-00004090: 6629 202d 3e20 2747 656e 6572 6963 5479  f) -> 'GenericTy
-000040a0: 7065 273a 0a20 2020 2020 2020 2027 2727  pe':.        '''
-000040b0: 200a 0a20 2020 2020 2020 203a 7274 7970   ..        :rtyp
-000040c0: 653a 2027 4765 6e65 7269 6354 7970 6527  e: 'GenericType'
-000040d0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
-000040e0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
-000040f0: 6566 205f 5f6c 656e 5f5f 2873 656c 6629  ef __len__(self)
-00004100: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
-00004110: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
-00004120: 7274 7970 653a 2069 6e74 0a20 2020 2020  rtype: int.     
+00001b50: 6c5b 696e 745d 0a20 2020 2020 2020 203a  l[int].        :
+00001b60: 7274 7970 653a 2027 4643 7572 7665 270a  rtype: 'FCurve'.
+00001b70: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00001b80: 2054 6865 2064 7269 7665 7228 7329 2061   The driver(s) a
+00001b90: 6464 6564 2e0a 2020 2020 2020 2020 2727  dded..        ''
+00001ba0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00001bb0: 2020 2020 6465 6620 6472 6976 6572 5f72      def driver_r
+00001bc0: 656d 6f76 6528 7365 6c66 2c0a 2020 2020  emove(self,.    
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 7061 7468 3a20 7479 7069 6e67 2e4f    path: typing.O
+00001bf0: 7074 696f 6e61 6c5b 7374 725d 2c0a 2020  ptional[str],.  
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c10: 2020 2020 696e 6465 783a 2074 7970 696e      index: typin
+00001c20: 672e 4f70 7469 6f6e 616c 5b69 6e74 5d20  g.Optional[int] 
+00001c30: 3d20 2d31 2920 2d3e 2062 6f6f 6c3a 0a20  = -1) -> bool:. 
+00001c40: 2020 2020 2020 2027 2727 2052 656d 6f76         ''' Remov
+00001c50: 6520 6472 6976 6572 2873 2920 6672 6f6d  e driver(s) from
+00001c60: 2074 6865 2067 6976 656e 2070 726f 7065   the given prope
+00001c70: 7274 790a 0a20 2020 2020 2020 203a 7061  rty..        :pa
+00001c80: 7261 6d20 7061 7468 3a20 7061 7468 2074  ram path: path t
+00001c90: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
+00001ca0: 6f20 6472 6976 652c 2061 6e61 6c6f 676f  o drive, analogo
+00001cb0: 7573 2074 6f20 7468 6520 6663 7572 7665  us to the fcurve
+00001cc0: 2773 2064 6174 6120 7061 7468 2e0a 2020  's data path..  
+00001cd0: 2020 2020 2020 3a74 7970 6520 7061 7468        :type path
+00001ce0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+00001cf0: 6c5b 7374 725d 0a20 2020 2020 2020 203a  l[str].        :
+00001d00: 7061 7261 6d20 696e 6465 783a 2061 7272  param index: arr
+00001d10: 6179 2069 6e64 6578 206f 6620 7468 6520  ay index of the 
+00001d20: 7072 6f70 6572 7479 2064 7269 7665 2e20  property drive. 
+00001d30: 4465 6661 756c 7473 2074 6f20 2d31 2066  Defaults to -1 f
+00001d40: 6f72 2061 6c6c 2069 6e64 6963 6573 206f  or all indices o
+00001d50: 7220 6120 7369 6e67 6c65 2063 6861 6e6e  r a single chann
+00001d60: 656c 2069 6620 7468 6520 7072 6f70 6572  el if the proper
+00001d70: 7479 2069 7320 6e6f 7420 616e 2061 7272  ty is not an arr
+00001d80: 6179 2e0a 2020 2020 2020 2020 3a74 7970  ay..        :typ
+00001d90: 6520 696e 6465 783a 2074 7970 696e 672e  e index: typing.
+00001da0: 4f70 7469 6f6e 616c 5b69 6e74 5d0a 2020  Optional[int].  
+00001db0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+00001dc0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+00001dd0: 726e 3a20 5375 6363 6573 7320 6f66 2064  rn: Success of d
+00001de0: 7269 7665 7220 7265 6d6f 7661 6c2e 0a20  river removal.. 
+00001df0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00001e00: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00001e10: 2067 6574 2873 656c 662c 0a20 2020 2020   get(self,.     
+00001e20: 2020 2020 2020 206b 6579 3a20 7479 7069         key: typi
+00001e30: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00001e40: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
+00001e50: 6661 756c 743a 2074 7970 696e 672e 4f70  fault: typing.Op
+00001e60: 7469 6f6e 616c 5b74 7970 696e 672e 416e  tional[typing.An
+00001e70: 795d 203d 204e 6f6e 6529 3a0a 2020 2020  y] = None):.    
+00001e80: 2020 2020 2727 2720 5265 7475 726e 7320      ''' Returns 
+00001e90: 7468 6520 7661 6c75 6520 6f66 2074 6865  the value of the
+00001ea0: 2063 7573 746f 6d20 7072 6f70 6572 7479   custom property
+00001eb0: 2061 7373 6967 6e65 6420 746f 206b 6579   assigned to key
+00001ec0: 206f 7220 6465 6661 756c 7420 7768 656e   or default when
+00001ed0: 206e 6f74 2066 6f75 6e64 2028 6d61 7463   not found (matc
+00001ee0: 6865 7320 5079 7468 6f6e 2773 2064 6963  hes Python's dic
+00001ef0: 7469 6f6e 6172 7920 6675 6e63 7469 6f6e  tionary function
+00001f00: 206f 6620 7468 6520 7361 6d65 206e 616d   of the same nam
+00001f10: 6529 2e0a 0a20 2020 2020 2020 203a 7061  e)...        :pa
+00001f20: 7261 6d20 6b65 793a 2054 6865 206b 6579  ram key: The key
+00001f30: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
+00001f40: 2074 6865 2063 7573 746f 6d20 7072 6f70   the custom prop
+00001f50: 6572 7479 2e0a 2020 2020 2020 2020 3a74  erty..        :t
+00001f60: 7970 6520 6b65 793a 2074 7970 696e 672e  ype key: typing.
+00001f70: 4f70 7469 6f6e 616c 5b73 7472 5d0a 2020  Optional[str].  
+00001f80: 2020 2020 2020 3a70 6172 616d 2064 6566        :param def
+00001f90: 6175 6c74 3a20 4f70 7469 6f6e 616c 2061  ault: Optional a
+00001fa0: 7267 756d 656e 7420 666f 7220 7468 6520  rgument for the 
+00001fb0: 7661 6c75 6520 746f 2072 6574 7572 6e20  value to return 
+00001fc0: 6966 202a 6b65 792a 2069 7320 6e6f 7420  if *key* is not 
+00001fd0: 666f 756e 642e 0a20 2020 2020 2020 203a  found..        :
+00001fe0: 7479 7065 2064 6566 6175 6c74 3a20 7479  type default: ty
+00001ff0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7479  ping.Optional[ty
+00002000: 7069 6e67 2e41 6e79 5d0a 2020 2020 2020  ping.Any].      
+00002010: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00002020: 7373 0a0a 2020 2020 6465 6620 6964 5f70  ss..    def id_p
+00002030: 726f 7065 7274 6965 735f 636c 6561 7228  roperties_clear(
+00002040: 7365 6c66 293a 0a20 2020 2020 2020 2027  self):.        '
+00002050: 2727 200a 0a20 2020 2020 2020 2027 2727  '' ..        '''
+00002060: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002070: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
+00002080: 7469 6573 5f65 6e73 7572 6528 7365 6c66  ties_ensure(self
+00002090: 2920 2d3e 2074 7970 696e 672e 416e 793a  ) -> typing.Any:
+000020a0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000020b0: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
+000020c0: 7970 696e 672e 416e 790a 2020 2020 2020  yping.Any.      
+000020d0: 2020 3a72 6574 7572 6e3a 2074 6865 2070    :return: the p
+000020e0: 6172 656e 7420 6772 6f75 7020 666f 7220  arent group for 
+000020f0: 616e 2052 4e41 2073 7472 7563 7427 7320  an RNA struct's 
+00002100: 6375 7374 6f6d 2049 4450 726f 7065 7274  custom IDPropert
+00002110: 6965 732e 0a20 2020 2020 2020 2027 2727  ies..        '''
+00002120: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002130: 2020 2064 6566 2069 645f 7072 6f70 6572     def id_proper
+00002140: 7469 6573 5f75 6928 7365 6c66 2c20 6b65  ties_ui(self, ke
+00002150: 793a 2074 7970 696e 672e 4f70 7469 6f6e  y: typing.Option
+00002160: 616c 5b74 7970 696e 672e 416e 795d 2920  al[typing.Any]) 
+00002170: 2d3e 2074 7970 696e 672e 416e 793a 0a20  -> typing.Any:. 
+00002180: 2020 2020 2020 2027 2727 200a 0a20 2020         ''' ..   
+00002190: 2020 2020 203a 7061 7261 6d20 6b65 793a       :param key:
+000021a0: 2020 5374 7269 6e67 206e 616d 6520 6f66    String name of
+000021b0: 2074 6865 2070 726f 7065 7274 792e 0a20   the property.. 
+000021c0: 2020 2020 2020 203a 7479 7065 206b 6579         :type key
+000021d0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000021e0: 6c5b 7479 7069 6e67 2e41 6e79 5d0a 2020  l[typing.Any].  
+000021f0: 2020 2020 2020 3a72 7479 7065 3a20 7479        :rtype: ty
+00002200: 7069 6e67 2e41 6e79 0a20 2020 2020 2020  ping.Any.       
+00002210: 203a 7265 7475 726e 3a20 5265 7475 726e   :return: Return
+00002220: 2061 6e20 6f62 6a65 6374 2075 7365 6420   an object used 
+00002230: 746f 206d 616e 6167 6520 616e 2049 4450  to manage an IDP
+00002240: 726f 7065 7274 7927 7320 5549 2064 6174  roperty's UI dat
+00002250: 612e 0a20 2020 2020 2020 2027 2727 0a20  a..        '''. 
+00002260: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
+00002270: 2064 6566 2069 735f 7072 6f70 6572 7479   def is_property
+00002280: 5f68 6964 6465 6e28 7365 6c66 2c20 7072  _hidden(self, pr
+00002290: 6f70 6572 7479 2920 2d3e 2062 6f6f 6c3a  operty) -> bool:
+000022a0: 0a20 2020 2020 2020 2027 2727 2043 6865  .        ''' Che
+000022b0: 636b 2069 6620 6120 7072 6f70 6572 7479  ck if a property
+000022c0: 2069 7320 6869 6464 656e 2e0a 0a20 2020   is hidden...   
+000022d0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+000022e0: 6c0a 2020 2020 2020 2020 3a72 6574 7572  l.        :retur
+000022f0: 6e3a 2054 7275 6520 7768 656e 2074 6865  n: True when the
+00002300: 2070 726f 7065 7274 7920 6973 2068 6964   property is hid
+00002310: 6465 6e2e 0a20 2020 2020 2020 2027 2727  den..        '''
+00002320: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+00002330: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+00002340: 7479 5f6f 7665 7272 6964 6162 6c65 5f6c  ty_overridable_l
+00002350: 6962 7261 7279 2873 656c 662c 2070 726f  ibrary(self, pro
+00002360: 7065 7274 7929 202d 3e20 626f 6f6c 3a0a  perty) -> bool:.
+00002370: 2020 2020 2020 2020 2727 2720 4368 6563          ''' Chec
+00002380: 6b20 6966 2061 2070 726f 7065 7274 7920  k if a property 
+00002390: 6973 206f 7665 7272 6964 6162 6c65 2e0a  is overridable..
+000023a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000023b0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+000023c0: 6574 7572 6e3a 2054 7275 6520 7768 656e  eturn: True when
+000023d0: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+000023e0: 206f 7665 7272 6964 6162 6c65 2e0a 2020   overridable..  
+000023f0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00002400: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00002410: 6973 5f70 726f 7065 7274 795f 7265 6164  is_property_read
+00002420: 6f6e 6c79 2873 656c 662c 2070 726f 7065  only(self, prope
+00002430: 7274 7929 202d 3e20 626f 6f6c 3a0a 2020  rty) -> bool:.  
+00002440: 2020 2020 2020 2727 2720 4368 6563 6b20        ''' Check 
+00002450: 6966 2061 2070 726f 7065 7274 7920 6973  if a property is
+00002460: 2072 6561 646f 6e6c 792e 0a0a 2020 2020   readonly...    
+00002470: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00002480: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00002490: 3a20 5472 7565 2077 6865 6e20 7468 6520  : True when the 
+000024a0: 7072 6f70 6572 7479 2069 7320 7265 6164  property is read
+000024b0: 6f6e 6c79 2028 6e6f 7420 7772 6974 6162  only (not writab
+000024c0: 6c65 292e 0a20 2020 2020 2020 2027 2727  le)..        '''
+000024d0: 0a20 2020 2020 2020 2070 6173 730a 0a20  .        pass.. 
+000024e0: 2020 2064 6566 2069 735f 7072 6f70 6572     def is_proper
+000024f0: 7479 5f73 6574 2873 656c 662c 2070 726f  ty_set(self, pro
+00002500: 7065 7274 792c 0a20 2020 2020 2020 2020  perty,.         
+00002510: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00002520: 686f 7374 3a20 7479 7069 6e67 2e4f 7074  host: typing.Opt
+00002530: 696f 6e61 6c5b 626f 6f6c 5d20 3d20 5472  ional[bool] = Tr
+00002540: 7565 2920 2d3e 2062 6f6f 6c3a 0a20 2020  ue) -> bool:.   
+00002550: 2020 2020 2027 2727 2043 6865 636b 2069       ''' Check i
+00002560: 6620 6120 7072 6f70 6572 7479 2069 7320  f a property is 
+00002570: 7365 742c 2075 7365 2066 6f72 2074 6573  set, use for tes
+00002580: 7469 6e67 206f 7065 7261 746f 7220 7072  ting operator pr
+00002590: 6f70 6572 7469 6573 2e0a 0a20 2020 2020  operties...     
+000025a0: 2020 203a 7061 7261 6d20 6768 6f73 743a     :param ghost:
+000025b0: 2055 7365 6420 666f 7220 6f70 6572 6174   Used for operat
+000025c0: 6f72 7320 7468 6174 2072 652d 7275 6e20  ors that re-run 
+000025d0: 7769 7468 2070 7265 7669 6f75 7320 7365  with previous se
+000025e0: 7474 696e 6773 2e20 496e 2074 6869 7320  ttings. In this 
+000025f0: 6361 7365 2074 6865 2070 726f 7065 7274  case the propert
+00002600: 7920 6973 206e 6f74 206d 6172 6b65 6420  y is not marked 
+00002610: 6173 2073 6574 2c20 7965 7420 7468 6520  as set, yet the 
+00002620: 7661 6c75 6520 6672 6f6d 2074 6865 2070  value from the p
+00002630: 7265 7669 6f75 7320 6578 6563 7574 696f  revious executio
+00002640: 6e20 6973 2075 7365 642e 2049 6e20 7261  n is used. In ra
+00002650: 7265 2063 6173 6573 2079 6f75 206d 6179  re cases you may
+00002660: 2077 616e 7420 746f 2073 6574 2074 6869   want to set thi
+00002670: 7320 6f70 7469 6f6e 2074 6f20 6661 6c73  s option to fals
+00002680: 652e 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+00002690: 2067 686f 7374 3a20 7479 7069 6e67 2e4f   ghost: typing.O
+000026a0: 7074 696f 6e61 6c5b 626f 6f6c 5d0a 2020  ptional[bool].  
+000026b0: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
+000026c0: 6f6c 0a20 2020 2020 2020 203a 7265 7475  ol.        :retu
+000026d0: 726e 3a20 5472 7565 2077 6865 6e20 7468  rn: True when th
+000026e0: 6520 7072 6f70 6572 7479 2068 6173 2062  e property has b
+000026f0: 6565 6e20 7365 742e 0a20 2020 2020 2020  een set..       
+00002700: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00002710: 730a 0a20 2020 2064 6566 2069 7465 6d73  s..    def items
+00002720: 2873 656c 6629 202d 3e20 7479 7069 6e67  (self) -> typing
+00002730: 2e41 6e79 3a0a 2020 2020 2020 2020 2727  .Any:.        ''
+00002740: 2720 5265 7475 726e 7320 7468 6520 6974  ' Returns the it
+00002750: 656d 7320 6f66 2074 6869 7320 6f62 6a65  ems of this obje
+00002760: 6374 7320 6375 7374 6f6d 2070 726f 7065  cts custom prope
+00002770: 7274 6965 7320 286d 6174 6368 6573 2050  rties (matches P
+00002780: 7974 686f 6e27 7320 6469 6374 696f 6e61  ython's dictiona
+00002790: 7279 2066 756e 6374 696f 6e20 6f66 2074  ry function of t
+000027a0: 6865 2073 616d 6520 6e61 6d65 292e 0a0a  he same name)...
+000027b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+000027c0: 7479 7069 6e67 2e41 6e79 0a20 2020 2020  typing.Any.     
+000027d0: 2020 203a 7265 7475 726e 3a20 6375 7374     :return: cust
+000027e0: 6f6d 2070 726f 7065 7274 7920 6b65 792c  om property key,
+000027f0: 2076 616c 7565 2070 6169 7273 2e0a 2020   value pairs..  
+00002800: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
+00002810: 2020 7061 7373 0a0a 2020 2020 6465 6620    pass..    def 
+00002820: 6b65 7966 7261 6d65 5f64 656c 6574 6528  keyframe_delete(
+00002830: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00002840: 662c 0a20 2020 2020 2020 2020 2020 2064  f,.            d
+00002850: 6174 615f 7061 7468 3a20 7479 7069 6e67  ata_path: typing
+00002860: 2e4f 7074 696f 6e61 6c5b 7374 725d 2c0a  .Optional[str],.
+00002870: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00002880: 783a 2074 7970 696e 672e 4f70 7469 6f6e  x: typing.Option
+00002890: 616c 5b69 6e74 5d20 3d20 2d31 2c0a 2020  al[int] = -1,.  
+000028a0: 2020 2020 2020 2020 2020 6672 616d 653a            frame:
+000028b0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+000028c0: 5b66 6c6f 6174 5d20 3d20 2762 7079 2e63  [float] = 'bpy.c
+000028d0: 6f6e 7465 7874 2e73 6365 6e65 2e66 7261  ontext.scene.fra
+000028e0: 6d65 5f63 7572 7265 6e74 272c 0a20 2020  me_current',.   
+000028f0: 2020 2020 2020 2020 2067 726f 7570 3a20           group: 
+00002900: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00002910: 7374 725d 203d 2022 2229 202d 3e20 626f  str] = "") -> bo
+00002920: 6f6c 3a0a 2020 2020 2020 2020 2727 2720  ol:.        ''' 
+00002930: 5265 6d6f 7665 2061 206b 6579 6672 616d  Remove a keyfram
+00002940: 6520 6672 6f6d 2074 6869 7320 7072 6f70  e from this prop
+00002950: 6572 7469 6573 2066 6375 7276 652e 0a0a  erties fcurve...
+00002960: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+00002970: 6174 615f 7061 7468 3a20 7061 7468 2074  ata_path: path t
+00002980: 6f20 7468 6520 7072 6f70 6572 7479 2074  o the property t
+00002990: 6f20 7265 6d6f 7665 2061 206b 6579 2c20  o remove a key, 
+000029a0: 616e 616c 6f67 6f75 7320 746f 2074 6865  analogous to the
+000029b0: 2066 6375 7276 6527 7320 6461 7461 2070   fcurve's data p
+000029c0: 6174 682e 0a20 2020 2020 2020 203a 7479  ath..        :ty
+000029d0: 7065 2064 6174 615f 7061 7468 3a20 7479  pe data_path: ty
+000029e0: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+000029f0: 725d 0a20 2020 2020 2020 203a 7061 7261  r].        :para
+00002a00: 6d20 696e 6465 783a 2061 7272 6179 2069  m index: array i
+00002a10: 6e64 6578 206f 6620 7468 6520 7072 6f70  ndex of the prop
+00002a20: 6572 7479 2074 6f20 7265 6d6f 7665 2061  erty to remove a
+00002a30: 206b 6579 2e20 4465 6661 756c 7473 2074   key. Defaults t
+00002a40: 6f20 2d31 2072 656d 6f76 696e 6720 616c  o -1 removing al
+00002a50: 6c20 696e 6469 6365 7320 6f72 2061 2073  l indices or a s
+00002a60: 696e 676c 6520 6368 616e 6e65 6c20 6966  ingle channel if
+00002a70: 2074 6865 2070 726f 7065 7274 7920 6973   the property is
+00002a80: 206e 6f74 2061 6e20 6172 7261 792e 0a20   not an array.. 
+00002a90: 2020 2020 2020 203a 7479 7065 2069 6e64         :type ind
+00002aa0: 6578 3a20 7479 7069 6e67 2e4f 7074 696f  ex: typing.Optio
+00002ab0: 6e61 6c5b 696e 745d 0a20 2020 2020 2020  nal[int].       
+00002ac0: 203a 7061 7261 6d20 6672 616d 653a 2054   :param frame: T
+00002ad0: 6865 2066 7261 6d65 206f 6e20 7768 6963  he frame on whic
+00002ae0: 6820 7468 6520 6b65 7966 7261 6d65 2069  h the keyframe i
+00002af0: 7320 6465 6c65 7465 642c 2064 6566 6175  s deleted, defau
+00002b00: 6c74 696e 6720 746f 2074 6865 2063 7572  lting to the cur
+00002b10: 7265 6e74 2066 7261 6d65 2e0a 2020 2020  rent frame..    
+00002b20: 2020 2020 3a74 7970 6520 6672 616d 653a      :type frame:
+00002b30: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002b40: 5b66 6c6f 6174 5d0a 2020 2020 2020 2020  [float].        
+00002b50: 3a70 6172 616d 2067 726f 7570 3a20 5468  :param group: Th
+00002b60: 6520 6e61 6d65 206f 6620 7468 6520 6772  e name of the gr
+00002b70: 6f75 7020 7468 6520 462d 4375 7276 6520  oup the F-Curve 
+00002b80: 7368 6f75 6c64 2062 6520 6164 6465 6420  should be added 
+00002b90: 746f 2069 6620 6974 2064 6f65 736e 2774  to if it doesn't
+00002ba0: 2065 7869 7374 2079 6574 2e0a 2020 2020   exist yet..    
+00002bb0: 2020 2020 3a74 7970 6520 6772 6f75 703a      :type group:
+00002bc0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00002bd0: 5b73 7472 5d0a 2020 2020 2020 2020 3a72  [str].        :r
+00002be0: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+00002bf0: 2020 203a 7265 7475 726e 3a20 5375 6363     :return: Succ
+00002c00: 6573 7320 6f66 206b 6579 6672 616d 6520  ess of keyframe 
+00002c10: 6465 6c65 7469 6f6e 2e0a 2020 2020 2020  deletion..      
+00002c20: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00002c30: 7373 0a0a 2020 2020 6465 6620 6b65 7966  ss..    def keyf
+00002c40: 7261 6d65 5f69 6e73 6572 7428 0a20 2020  rame_insert(.   
+00002c50: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
+00002c60: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00002c70: 7061 7468 3a20 7479 7069 6e67 2e4f 7074  path: typing.Opt
+00002c80: 696f 6e61 6c5b 7374 725d 2c0a 2020 2020  ional[str],.    
+00002c90: 2020 2020 2020 2020 696e 6465 783a 2074          index: t
+00002ca0: 7970 696e 672e 4f70 7469 6f6e 616c 5b69  yping.Optional[i
+00002cb0: 6e74 5d20 3d20 2d31 2c0a 2020 2020 2020  nt] = -1,.      
+00002cc0: 2020 2020 2020 6672 616d 653a 2074 7970        frame: typ
+00002cd0: 696e 672e 4f70 7469 6f6e 616c 5b66 6c6f  ing.Optional[flo
+00002ce0: 6174 5d20 3d20 2762 7079 2e63 6f6e 7465  at] = 'bpy.conte
+00002cf0: 7874 2e73 6365 6e65 2e66 7261 6d65 5f63  xt.scene.frame_c
+00002d00: 7572 7265 6e74 272c 0a20 2020 2020 2020  urrent',.       
+00002d10: 2020 2020 2067 726f 7570 3a20 7479 7069       group: typi
+00002d20: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00002d30: 203d 2022 222c 0a20 2020 2020 2020 2020   = "",.         
+00002d40: 2020 206f 7074 696f 6e73 3a20 7479 7069     options: typi
+00002d50: 6e67 2e4f 7074 696f 6e61 6c5b 7479 7069  ng.Optional[typi
+00002d60: 6e67 2e41 6e79 5d20 3d20 2773 6574 2829  ng.Any] = 'set()
+00002d70: 2729 202d 3e20 626f 6f6c 3a0a 2020 2020  ') -> bool:.    
+00002d80: 2020 2020 2727 2720 496e 7365 7274 2061      ''' Insert a
+00002d90: 206b 6579 6672 616d 6520 6f6e 2074 6865   keyframe on the
+00002da0: 2070 726f 7065 7274 7920 6769 7665 6e2c   property given,
+00002db0: 2061 6464 696e 6720 6663 7572 7665 7320   adding fcurves 
+00002dc0: 616e 6420 616e 696d 6174 696f 6e20 6461  and animation da
+00002dd0: 7461 2077 6865 6e20 6e65 6365 7373 6172  ta when necessar
+00002de0: 792e 2054 6869 7320 6973 2074 6865 206d  y. This is the m
+00002df0: 6f73 7420 7369 6d70 6c65 2065 7861 6d70  ost simple examp
+00002e00: 6c65 206f 6620 696e 7365 7274 696e 6720  le of inserting 
+00002e10: 6120 6b65 7966 7261 6d65 2066 726f 6d20  a keyframe from 
+00002e20: 7079 7468 6f6e 2e20 4e6f 7465 2074 6861  python. Note tha
+00002e30: 7420 7768 656e 206b 6579 696e 6720 6461  t when keying da
+00002e40: 7461 2070 6174 6873 2077 6869 6368 2063  ta paths which c
+00002e50: 6f6e 7461 696e 206e 6573 7465 6420 7072  ontain nested pr
+00002e60: 6f70 6572 7469 6573 2074 6869 7320 6d75  operties this mu
+00002e70: 7374 2062 6520 646f 6e65 2066 726f 6d20  st be done from 
+00002e80: 7468 6520 6049 4460 2073 7562 636c 6173  the `ID` subclas
+00002e90: 732c 2069 6e20 7468 6973 2063 6173 6520  s, in this case 
+00002ea0: 7468 6520 6041 726d 6174 7572 6560 2072  the `Armature` r
+00002eb0: 6174 6865 7220 7468 616e 2074 6865 2062  ather than the b
+00002ec0: 6f6e 652e 0a0a 2020 2020 2020 2020 3a70  one...        :p
+00002ed0: 6172 616d 2064 6174 615f 7061 7468 3a20  aram data_path: 
+00002ee0: 7061 7468 2074 6f20 7468 6520 7072 6f70  path to the prop
+00002ef0: 6572 7479 2074 6f20 6b65 792c 2061 6e61  erty to key, ana
+00002f00: 6c6f 676f 7573 2074 6f20 7468 6520 6663  logous to the fc
+00002f10: 7572 7665 2773 2064 6174 6120 7061 7468  urve's data path
+00002f20: 2e0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00002f30: 6461 7461 5f70 6174 683a 2074 7970 696e  data_path: typin
+00002f40: 672e 4f70 7469 6f6e 616c 5b73 7472 5d0a  g.Optional[str].
+00002f50: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
+00002f60: 6e64 6578 3a20 6172 7261 7920 696e 6465  ndex: array inde
+00002f70: 7820 6f66 2074 6865 2070 726f 7065 7274  x of the propert
+00002f80: 7920 746f 206b 6579 2e20 4465 6661 756c  y to key. Defaul
+00002f90: 7473 2074 6f20 2d31 2077 6869 6368 2077  ts to -1 which w
+00002fa0: 696c 6c20 6b65 7920 616c 6c20 696e 6469  ill key all indi
+00002fb0: 6365 7320 6f72 2061 2073 696e 676c 6520  ces or a single 
+00002fc0: 6368 616e 6e65 6c20 6966 2074 6865 2070  channel if the p
+00002fd0: 726f 7065 7274 7920 6973 206e 6f74 2061  roperty is not a
+00002fe0: 6e20 6172 7261 792e 0a20 2020 2020 2020  n array..       
+00002ff0: 203a 7479 7065 2069 6e64 6578 3a20 7479   :type index: ty
+00003000: 7069 6e67 2e4f 7074 696f 6e61 6c5b 696e  ping.Optional[in
+00003010: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
+00003020: 6d20 6672 616d 653a 2054 6865 2066 7261  m frame: The fra
+00003030: 6d65 206f 6e20 7768 6963 6820 7468 6520  me on which the 
+00003040: 6b65 7966 7261 6d65 2069 7320 696e 7365  keyframe is inse
+00003050: 7274 6564 2c20 6465 6661 756c 7469 6e67  rted, defaulting
+00003060: 2074 6f20 7468 6520 6375 7272 656e 7420   to the current 
+00003070: 6672 616d 652e 0a20 2020 2020 2020 203a  frame..        :
+00003080: 7479 7065 2066 7261 6d65 3a20 7479 7069  type frame: typi
+00003090: 6e67 2e4f 7074 696f 6e61 6c5b 666c 6f61  ng.Optional[floa
+000030a0: 745d 0a20 2020 2020 2020 203a 7061 7261  t].        :para
+000030b0: 6d20 6772 6f75 703a 2054 6865 206e 616d  m group: The nam
+000030c0: 6520 6f66 2074 6865 2067 726f 7570 2074  e of the group t
+000030d0: 6865 2046 2d43 7572 7665 2073 686f 756c  he F-Curve shoul
+000030e0: 6420 6265 2061 6464 6564 2074 6f20 6966  d be added to if
+000030f0: 2069 7420 646f 6573 6e27 7420 6578 6973   it doesn't exis
+00003100: 7420 7965 742e 0a20 2020 2020 2020 203a  t yet..        :
+00003110: 7479 7065 2067 726f 7570 3a20 7479 7069  type group: typi
+00003120: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003130: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003140: 666c 6167 3a20 0a20 2020 2020 2020 203a  flag: .        :
+00003150: 7479 7065 2066 6c61 673a 2074 7970 696e  type flag: typin
+00003160: 672e 4f70 7469 6f6e 616c 5b74 7970 696e  g.Optional[typin
+00003170: 672e 5365 745d 0a20 2020 2020 2020 203a  g.Set].        :
+00003180: 7061 7261 6d20 6f70 7469 6f6e 733a 2020  param options:  
+00003190: 2d20 6060 494e 5345 5254 4b45 595f 4e45  - ``INSERTKEY_NE
+000031a0: 4544 4544 6060 204f 6e6c 7920 696e 7365  EDED`` Only inse
+000031b0: 7274 206b 6579 6672 616d 6573 2077 6865  rt keyframes whe
+000031c0: 7265 2074 6865 7927 7265 206e 6565 6465  re they're neede
+000031d0: 6420 696e 2074 6865 2072 656c 6576 616e  d in the relevan
+000031e0: 7420 462d 4375 7276 6573 2e20 2d20 6060  t F-Curves. - ``
+000031f0: 494e 5345 5254 4b45 595f 5649 5355 414c  INSERTKEY_VISUAL
+00003200: 6060 2049 6e73 6572 7420 6b65 7966 7261  `` Insert keyfra
+00003210: 6d65 7320 6261 7365 6420 6f6e 2027 7669  mes based on 'vi
+00003220: 7375 616c 2074 7261 6e73 666f 726d 7327  sual transforms'
+00003230: 2e20 2d20 6060 494e 5345 5254 4b45 595f  . - ``INSERTKEY_
+00003240: 5859 5a5f 544f 5f52 4742 6060 2043 6f6c  XYZ_TO_RGB`` Col
+00003250: 6f72 2066 6f72 206e 6577 6c79 2061 6464  or for newly add
+00003260: 6564 2074 7261 6e73 666f 726d 6174 696f  ed transformatio
+00003270: 6e20 462d 4375 7276 6573 2028 4c6f 6361  n F-Curves (Loca
+00003280: 7469 6f6e 2c20 526f 7461 7469 6f6e 2c20  tion, Rotation, 
+00003290: 5363 616c 6529 2069 7320 6261 7365 6420  Scale) is based 
+000032a0: 6f6e 2074 6865 2074 7261 6e73 666f 726d  on the transform
+000032b0: 2061 7869 732e 202d 2060 6049 4e53 4552   axis. - ``INSER
+000032c0: 544b 4559 5f52 4550 4c41 4345 6060 204f  TKEY_REPLACE`` O
+000032d0: 6e6c 7920 7265 706c 6163 6520 616c 7265  nly replace alre
+000032e0: 6164 7920 6578 6973 7469 6e67 206b 6579  ady existing key
+000032f0: 6672 616d 6573 2e20 2d20 6060 494e 5345  frames. - ``INSE
+00003300: 5254 4b45 595f 4156 4149 4c41 424c 4560  RTKEY_AVAILABLE`
+00003310: 6020 4f6e 6c79 2069 6e73 6572 7420 696e  ` Only insert in
+00003320: 746f 2061 6c72 6561 6479 2065 7869 7374  to already exist
+00003330: 696e 6720 462d 4375 7276 6573 2e20 2d20  ing F-Curves. - 
+00003340: 6060 494e 5345 5254 4b45 595f 4359 434c  ``INSERTKEY_CYCL
+00003350: 455f 4157 4152 4560 6020 5461 6b65 2063  E_AWARE`` Take c
+00003360: 7963 6c69 6320 6578 7472 6170 6f6c 6174  yclic extrapolat
+00003370: 696f 6e20 696e 746f 2061 6363 6f75 6e74  ion into account
+00003380: 2028 4379 636c 652d 4177 6172 6520 4b65   (Cycle-Aware Ke
+00003390: 7969 6e67 206f 7074 696f 6e29 2e0a 2020  ying option)..  
+000033a0: 2020 2020 2020 3a74 7970 6520 6f70 7469        :type opti
+000033b0: 6f6e 733a 2074 7970 696e 672e 4f70 7469  ons: typing.Opti
+000033c0: 6f6e 616c 5b74 7970 696e 672e 416e 795d  onal[typing.Any]
+000033d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000033e0: 2062 6f6f 6c0a 2020 2020 2020 2020 3a72   bool.        :r
+000033f0: 6574 7572 6e3a 2053 7563 6365 7373 206f  eturn: Success o
+00003400: 6620 6b65 7966 7261 6d65 2069 6e73 6572  f keyframe inser
+00003410: 7469 6f6e 2e0a 2020 2020 2020 2020 2727  tion..        ''
+00003420: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003430: 2020 2020 6465 6620 6b65 7973 2873 656c      def keys(sel
+00003440: 6629 202d 3e20 7479 7069 6e67 2e41 6e79  f) -> typing.Any
+00003450: 3a0a 2020 2020 2020 2020 2727 2720 5265  :.        ''' Re
+00003460: 7475 726e 7320 7468 6520 6b65 7973 206f  turns the keys o
+00003470: 6620 7468 6973 206f 626a 6563 7473 2063  f this objects c
+00003480: 7573 746f 6d20 7072 6f70 6572 7469 6573  ustom properties
+00003490: 2028 6d61 7463 6865 7320 5079 7468 6f6e   (matches Python
+000034a0: 2773 2064 6963 7469 6f6e 6172 7920 6675  's dictionary fu
+000034b0: 6e63 7469 6f6e 206f 6620 7468 6520 7361  nction of the sa
+000034c0: 6d65 206e 616d 6529 2e0a 0a20 2020 2020  me name)...     
+000034d0: 2020 203a 7274 7970 653a 2074 7970 696e     :rtype: typin
+000034e0: 672e 416e 790a 2020 2020 2020 2020 3a72  g.Any.        :r
+000034f0: 6574 7572 6e3a 2063 7573 746f 6d20 7072  eturn: custom pr
+00003500: 6f70 6572 7479 206b 6579 732e 0a20 2020  operty keys..   
+00003510: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003520: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
+00003530: 6174 685f 6672 6f6d 5f69 6428 7365 6c66  ath_from_id(self
+00003540: 2c20 7072 6f70 6572 7479 3a20 7479 7069  , property: typi
+00003550: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003560: 203d 2022 2229 202d 3e20 7374 723a 0a20   = "") -> str:. 
+00003570: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00003580: 6e73 2074 6865 2064 6174 6120 7061 7468  ns the data path
+00003590: 2066 726f 6d20 7468 6520 4944 2074 6f20   from the ID to 
+000035a0: 7468 6973 206f 626a 6563 7420 2873 7472  this object (str
+000035b0: 696e 6729 2e0a 0a20 2020 2020 2020 203a  ing)...        :
+000035c0: 7061 7261 6d20 7072 6f70 6572 7479 3a20  param property: 
+000035d0: 4f70 7469 6f6e 616c 2070 726f 7065 7274  Optional propert
+000035e0: 7920 6e61 6d65 2077 6869 6368 2063 616e  y name which can
+000035f0: 2062 6520 7573 6564 2069 6620 7468 6520   be used if the 
+00003600: 7061 7468 2069 7320 746f 2061 2070 726f  path is to a pro
+00003610: 7065 7274 7920 6f66 2074 6869 7320 6f62  perty of this ob
+00003620: 6a65 6374 2e0a 2020 2020 2020 2020 3a74  ject..        :t
+00003630: 7970 6520 7072 6f70 6572 7479 3a20 7479  ype property: ty
+00003640: 7069 6e67 2e4f 7074 696f 6e61 6c5b 7374  ping.Optional[st
+00003650: 725d 0a20 2020 2020 2020 203a 7274 7970  r].        :rtyp
+00003660: 653a 2073 7472 0a20 2020 2020 2020 203a  e: str.        :
+00003670: 7265 7475 726e 3a20 6062 7079 2e74 7970  return: `bpy.typ
+00003680: 6573 2e62 7079 5f73 7472 7563 742e 6964  es.bpy_struct.id
+00003690: 5f64 6174 6160 2074 6f20 7468 6973 2073  _data` to this s
+000036a0: 7472 7563 7420 616e 6420 7072 6f70 6572  truct and proper
+000036b0: 7479 2028 7768 656e 2067 6976 656e 292e  ty (when given).
+000036c0: 0a20 2020 2020 2020 2027 2727 0a20 2020  .        '''.   
+000036d0: 2020 2020 2070 6173 730a 0a20 2020 2064       pass..    d
+000036e0: 6566 2070 6174 685f 7265 736f 6c76 6528  ef path_resolve(
+000036f0: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00003700: 2020 2020 2020 2020 2020 2070 6174 683a             path:
+00003710: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003720: 5b73 7472 5d2c 0a20 2020 2020 2020 2020  [str],.         
+00003730: 2020 2020 2020 2020 2020 2020 636f 6572              coer
+00003740: 6365 3a20 7479 7069 6e67 2e4f 7074 696f  ce: typing.Optio
+00003750: 6e61 6c5b 626f 6f6c 5d20 3d20 5472 7565  nal[bool] = True
+00003760: 293a 0a20 2020 2020 2020 2027 2727 2052  ):.        ''' R
+00003770: 6574 7572 6e73 2074 6865 2070 726f 7065  eturns the prope
+00003780: 7274 7920 6672 6f6d 2074 6865 2070 6174  rty from the pat
+00003790: 682c 2072 6169 7365 2061 6e20 6578 6365  h, raise an exce
+000037a0: 7074 696f 6e20 7768 656e 206e 6f74 2066  ption when not f
+000037b0: 6f75 6e64 2e0a 0a20 2020 2020 2020 203a  ound...        :
+000037c0: 7061 7261 6d20 7061 7468 3a20 7061 7468  param path: path
+000037d0: 2077 6869 6368 2074 6869 7320 7072 6f70   which this prop
+000037e0: 6572 7479 2072 6573 6f6c 7665 732e 0a20  erty resolves.. 
+000037f0: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
+00003800: 683a 2074 7970 696e 672e 4f70 7469 6f6e  h: typing.Option
+00003810: 616c 5b73 7472 5d0a 2020 2020 2020 2020  al[str].        
+00003820: 3a70 6172 616d 2063 6f65 7263 653a 206f  :param coerce: o
+00003830: 7074 696f 6e61 6c20 6172 6775 6d65 6e74  ptional argument
+00003840: 2c20 7768 656e 2054 7275 652c 2074 6865  , when True, the
+00003850: 2070 726f 7065 7274 7920 7769 6c6c 2062   property will b
+00003860: 6520 636f 6e76 6572 7465 6420 696e 746f  e converted into
+00003870: 2069 7473 2050 7974 686f 6e20 7265 7072   its Python repr
+00003880: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
+00003890: 2020 2020 3a74 7970 6520 636f 6572 6365      :type coerce
+000038a0: 3a20 7479 7069 6e67 2e4f 7074 696f 6e61  : typing.Optiona
+000038b0: 6c5b 626f 6f6c 5d0a 2020 2020 2020 2020  l[bool].        
+000038c0: 2727 270a 2020 2020 2020 2020 7061 7373  '''.        pass
+000038d0: 0a0a 2020 2020 6465 6620 706f 7028 7365  ..    def pop(se
+000038e0: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+000038f0: 6b65 793a 2074 7970 696e 672e 4f70 7469  key: typing.Opti
+00003900: 6f6e 616c 5b73 7472 5d2c 0a20 2020 2020  onal[str],.     
+00003910: 2020 2020 2020 2064 6566 6175 6c74 3a20         default: 
+00003920: 7479 7069 6e67 2e4f 7074 696f 6e61 6c5b  typing.Optional[
+00003930: 7479 7069 6e67 2e41 6e79 5d20 3d20 4e6f  typing.Any] = No
+00003940: 6e65 293a 0a20 2020 2020 2020 2027 2727  ne):.        '''
+00003950: 2052 656d 6f76 6520 616e 6420 7265 7475   Remove and retu
+00003960: 726e 2074 6865 2076 616c 7565 206f 6620  rn the value of 
+00003970: 7468 6520 6375 7374 6f6d 2070 726f 7065  the custom prope
+00003980: 7274 7920 6173 7369 676e 6564 2074 6f20  rty assigned to 
+00003990: 6b65 7920 6f72 2064 6566 6175 6c74 2077  key or default w
+000039a0: 6865 6e20 6e6f 7420 666f 756e 6420 286d  hen not found (m
+000039b0: 6174 6368 6573 2050 7974 686f 6e27 7320  atches Python's 
+000039c0: 6469 6374 696f 6e61 7279 2066 756e 6374  dictionary funct
+000039d0: 696f 6e20 6f66 2074 6865 2073 616d 6520  ion of the same 
+000039e0: 6e61 6d65 292e 0a0a 2020 2020 2020 2020  name)...        
+000039f0: 3a70 6172 616d 206b 6579 3a20 5468 6520  :param key: The 
+00003a00: 6b65 7920 6173 736f 6369 6174 6564 2077  key associated w
+00003a10: 6974 6820 7468 6520 6375 7374 6f6d 2070  ith the custom p
+00003a20: 726f 7065 7274 792e 0a20 2020 2020 2020  roperty..       
+00003a30: 203a 7479 7065 206b 6579 3a20 7479 7069   :type key: typi
+00003a40: 6e67 2e4f 7074 696f 6e61 6c5b 7374 725d  ng.Optional[str]
+00003a50: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00003a60: 6465 6661 756c 743a 204f 7074 696f 6e61  default: Optiona
+00003a70: 6c20 6172 6775 6d65 6e74 2066 6f72 2074  l argument for t
+00003a80: 6865 2076 616c 7565 2074 6f20 7265 7475  he value to retu
+00003a90: 726e 2069 6620 2a6b 6579 2a20 6973 206e  rn if *key* is n
+00003aa0: 6f74 2066 6f75 6e64 2e0a 2020 2020 2020  ot found..      
+00003ab0: 2020 3a74 7970 6520 6465 6661 756c 743a    :type default:
+00003ac0: 2074 7970 696e 672e 4f70 7469 6f6e 616c   typing.Optional
+00003ad0: 5b74 7970 696e 672e 416e 795d 0a20 2020  [typing.Any].   
+00003ae0: 2020 2020 2027 2727 0a20 2020 2020 2020       '''.       
+00003af0: 2070 6173 730a 0a20 2020 2064 6566 2070   pass..    def p
+00003b00: 726f 7065 7274 795f 6f76 6572 7269 6461  roperty_overrida
+00003b10: 626c 655f 6c69 6272 6172 795f 7365 7428  ble_library_set(
+00003b20: 7365 6c66 2c20 7072 6f70 6572 7479 2c20  self, property, 
+00003b30: 6f76 6572 7269 6461 626c 6529 202d 3e20  overridable) -> 
+00003b40: 626f 6f6c 3a0a 2020 2020 2020 2020 2727  bool:.        ''
+00003b50: 2720 4465 6669 6e65 2061 2070 726f 7065  ' Define a prope
+00003b60: 7274 7920 6173 206f 7665 7272 6964 6162  rty as overridab
+00003b70: 6c65 206f 7220 6e6f 7420 286f 6e6c 7920  le or not (only 
+00003b80: 666f 7220 6375 7374 6f6d 2070 726f 7065  for custom prope
+00003b90: 7274 6965 7321 292e 0a0a 2020 2020 2020  rties!)...      
+00003ba0: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
+00003bb0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00003bc0: 5472 7565 2077 6865 6e20 7468 6520 6f76  True when the ov
+00003bd0: 6572 7269 6461 626c 6520 7374 6174 7573  erridable status
+00003be0: 206f 6620 7468 6520 7072 6f70 6572 7479   of the property
+00003bf0: 2077 6173 2073 7563 6365 7373 6675 6c6c   was successfull
+00003c00: 7920 7365 742e 0a20 2020 2020 2020 2027  y set..        '
+00003c10: 2727 0a20 2020 2020 2020 2070 6173 730a  ''.        pass.
+00003c20: 0a20 2020 2064 6566 2070 726f 7065 7274  .    def propert
+00003c30: 795f 756e 7365 7428 7365 6c66 2c20 7072  y_unset(self, pr
+00003c40: 6f70 6572 7479 293a 0a20 2020 2020 2020  operty):.       
+00003c50: 2027 2727 2055 6e73 6574 2061 2070 726f   ''' Unset a pro
+00003c60: 7065 7274 792c 2077 696c 6c20 7573 6520  perty, will use 
+00003c70: 6465 6661 756c 7420 7661 6c75 6520 6166  default value af
+00003c80: 7465 7277 6172 642e 0a0a 2020 2020 2020  terward...      
+00003c90: 2020 2727 270a 2020 2020 2020 2020 7061    '''.        pa
+00003ca0: 7373 0a0a 2020 2020 6465 6620 7479 7065  ss..    def type
+00003cb0: 5f72 6563 6173 7428 7365 6c66 2920 2d3e  _recast(self) ->
+00003cc0: 2027 6270 795f 7374 7275 6374 273a 0a20   'bpy_struct':. 
+00003cd0: 2020 2020 2020 2027 2727 2052 6574 7572         ''' Retur
+00003ce0: 6e20 6120 6e65 7720 696e 7374 616e 6365  n a new instance
+00003cf0: 2c20 7468 6973 2069 7320 6e65 6564 6564  , this is needed
+00003d00: 2062 6563 6175 7365 2074 7970 6573 2073   because types s
+00003d10: 7563 6820 6173 2074 6578 7475 7265 7320  uch as textures 
+00003d20: 6361 6e20 6265 2063 6861 6e67 6564 2061  can be changed a
+00003d30: 7420 7275 6e74 696d 652e 0a0a 2020 2020  t runtime...    
+00003d40: 2020 2020 3a72 7479 7065 3a20 2762 7079      :rtype: 'bpy
+00003d50: 5f73 7472 7563 7427 0a20 2020 2020 2020  _struct'.       
+00003d60: 203a 7265 7475 726e 3a20 6120 6e65 7720   :return: a new 
+00003d70: 696e 7374 616e 6365 206f 6620 7468 6973  instance of this
+00003d80: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+00003d90: 2074 7970 6520 696e 6974 6961 6c69 7a65   type initialize
+00003da0: 6420 6167 6169 6e2e 0a20 2020 2020 2020  d again..       
+00003db0: 2027 2727 0a20 2020 2020 2020 2070 6173   '''.        pas
+00003dc0: 730a 0a20 2020 2064 6566 2076 616c 7565  s..    def value
+00003dd0: 7328 7365 6c66 2920 2d3e 2074 7970 696e  s(self) -> typin
+00003de0: 672e 416e 793a 0a20 2020 2020 2020 2027  g.Any:.        '
+00003df0: 2727 2052 6574 7572 6e73 2074 6865 2076  '' Returns the v
+00003e00: 616c 7565 7320 6f66 2074 6869 7320 6f62  alues of this ob
+00003e10: 6a65 6374 7320 6375 7374 6f6d 2070 726f  jects custom pro
+00003e20: 7065 7274 6965 7320 286d 6174 6368 6573  perties (matches
+00003e30: 2050 7974 686f 6e27 7320 6469 6374 696f   Python's dictio
+00003e40: 6e61 7279 2066 756e 6374 696f 6e20 6f66  nary function of
+00003e50: 2074 6865 2073 616d 6520 6e61 6d65 292e   the same name).
+00003e60: 0a0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
+00003e70: 3a20 7479 7069 6e67 2e41 6e79 0a20 2020  : typing.Any.   
+00003e80: 2020 2020 203a 7265 7475 726e 3a20 6375       :return: cu
+00003e90: 7374 6f6d 2070 726f 7065 7274 7920 7661  stom property va
+00003ea0: 6c75 6573 2e0a 2020 2020 2020 2020 2727  lues..        ''
+00003eb0: 270a 2020 2020 2020 2020 7061 7373 0a0a  '.        pass..
+00003ec0: 2020 2020 6465 6620 5f5f 6765 7469 7465      def __getite
+00003ed0: 6d5f 5f28 7365 6c66 2c20 6b65 793a 2074  m__(self, key: t
+00003ee0: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00003ef0: 2073 7472 5d29 202d 3e20 2774 7970 696e   str]) -> 'typin
+00003f00: 672e 416e 7927 3a0a 2020 2020 2020 2020  g.Any':.        
+00003f10: 2727 2720 0a0a 2020 2020 2020 2020 3a70  ''' ..        :p
+00003f20: 6172 616d 206b 6579 3a20 0a20 2020 2020  aram key: .     
+00003f30: 2020 203a 7479 7065 206b 6579 3a20 7479     :type key: ty
+00003f40: 7069 6e67 2e55 6e69 6f6e 5b69 6e74 2c20  ping.Union[int, 
+00003f50: 7374 725d 0a20 2020 2020 2020 203a 7274  str].        :rt
+00003f60: 7970 653a 2027 7479 7069 6e67 2e41 6e79  ype: 'typing.Any
+00003f70: 270a 2020 2020 2020 2020 2727 270a 2020  '.        '''.  
+00003f80: 2020 2020 2020 7061 7373 0a0a 2020 2020        pass..    
+00003f90: 6465 6620 5f5f 7365 7469 7465 6d5f 5f28  def __setitem__(
+00003fa0: 7365 6c66 2c20 6b65 793a 2074 7970 696e  self, key: typin
+00003fb0: 672e 556e 696f 6e5b 696e 742c 2073 7472  g.Union[int, str
+00003fc0: 5d2c 2076 616c 7565 3a20 2774 7970 696e  ], value: 'typin
+00003fd0: 672e 416e 7927 293a 0a20 2020 2020 2020  g.Any'):.       
+00003fe0: 2027 2727 200a 0a20 2020 2020 2020 203a   ''' ..        :
+00003ff0: 7061 7261 6d20 6b65 793a 200a 2020 2020  param key: .    
+00004000: 2020 2020 3a74 7970 6520 6b65 793a 2074      :type key: t
+00004010: 7970 696e 672e 556e 696f 6e5b 696e 742c  yping.Union[int,
+00004020: 2073 7472 5d0a 2020 2020 2020 2020 3a70   str].        :p
+00004030: 6172 616d 2076 616c 7565 3a20 0a20 2020  aram value: .   
+00004040: 2020 2020 203a 7479 7065 2076 616c 7565       :type value
+00004050: 3a20 2774 7970 696e 672e 416e 7927 0a20  : 'typing.Any'. 
+00004060: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
+00004070: 2020 2070 6173 730a 0a20 2020 2064 6566     pass..    def
+00004080: 205f 5f64 656c 6974 656d 5f5f 2873 656c   __delitem__(sel
+00004090: 662c 206b 6579 3a20 7479 7069 6e67 2e55  f, key: typing.U
+000040a0: 6e69 6f6e 5b69 6e74 2c20 7374 725d 2920  nion[int, str]) 
+000040b0: 2d3e 2027 7479 7069 6e67 2e41 6e79 273a  -> 'typing.Any':
+000040c0: 0a20 2020 2020 2020 2027 2727 200a 0a20  .        ''' .. 
+000040d0: 2020 2020 2020 203a 7061 7261 6d20 6b65         :param ke
+000040e0: 793a 200a 2020 2020 2020 2020 3a74 7970  y: .        :typ
+000040f0: 6520 6b65 793a 2074 7970 696e 672e 556e  e key: typing.Un
+00004100: 696f 6e5b 696e 742c 2073 7472 5d0a 2020  ion[int, str].  
+00004110: 2020 2020 2020 3a72 7479 7065 3a20 2774        :rtype: 't
+00004120: 7970 696e 672e 416e 7927 0a20 2020 2020  yping.Any'.     
 00004130: 2020 2027 2727 0a20 2020 2020 2020 2070     '''.        p
 00004140: 6173 730a 0a0a 636c 6173 7320 6270 795f  ass...class bpy_
 00004150: 7072 6f70 5f61 7272 6179 2874 7970 696e  prop_array(typin
 00004160: 672e 4765 6e65 7269 635b 4765 6e65 7269  g.Generic[Generi
 00004170: 6354 7970 655d 293a 0a20 2020 2064 6566  cType]):.    def
 00004180: 2066 6f72 6561 6368 5f67 6574 2873 656c   foreach_get(sel
 00004190: 662c 2061 7474 722c 2073 6571 293a 0a20  f, attr, seq):.
```

### Comparing `fake-bpy-module-latest-20230427/bpy/utils/__init__.py` & `fake-bpy-module-latest-20230428/bpy/utils/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 import typing
 import bpy.types
 
-from . import previews
 from . import units
+from . import previews
 
 GenericType = typing.TypeVar("GenericType")
 
 
 def app_template_paths(*, path: typing.Optional[str] = None) -> typing.Any:
     ''' Returns valid application template paths.
```

### Comparing `fake-bpy-module-latest-20230427/bpy/utils/previews.py` & `fake-bpy-module-latest-20230428/bpy/utils/previews.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy/utils/units.py` & `fake-bpy-module-latest-20230428/bpy/utils/units.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/anim_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/anim_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,16 +108,16 @@
     '''
 
     pass
 
 
 def bake_action_objects_iter(
         object_action_pairs: typing.
-        Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object'],
+        Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence'],
         **kwargs):
     ''' An coroutine that bakes actions for multiple objects.
 
     :param object_action_pairs: Sequence of object action tuples, action is the destination for the baked data. When None a new action will be created.
-    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Sequence', 'bpy.types.Object']
+    :type object_action_pairs: typing.Union['bpy.types.Action', 'bpy.types.Object', 'bpy.types.Sequence']
     '''
 
     pass
```

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/image_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/image_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/io_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/io_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/mesh_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/mesh_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/node_shader_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/node_shader_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/object_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/object_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/view3d_utils.py` & `fake-bpy-module-latest-20230428/bpy_extras/view3d_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_extras/wm_utils/progress_report.py` & `fake-bpy-module-latest-20230428/bpy_extras/wm_utils/progress_report.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/bpy_types.py` & `fake-bpy-module-latest-20230428/bpy_types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/PKG-INFO` & `fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fake-bpy-module-latest
-Version: 20230427
+Version: 20230428
 Summary: Collection of the fake Blender Python API module for the code completion.
 Home-page: https://github.com/nutti/fake-bpy-module
 Author: nutti
 Author-email: nutti.metro@gmail.com
 Maintainer: nutti
 Maintainer-email: nutti.metro@gmail.com
 License: MIT
```

### Comparing `fake-bpy-module-latest-20230427/fake_bpy_module_latest.egg-info/SOURCES.txt` & `fake-bpy-module-latest-20230428/fake_bpy_module_latest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/chainingiterators.py` & `fake-bpy-module-latest-20230428/freestyle/chainingiterators.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/functions.py` & `fake-bpy-module-latest-20230428/freestyle/functions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/predicates.py` & `fake-bpy-module-latest-20230428/freestyle/predicates.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/shaders.py` & `fake-bpy-module-latest-20230428/freestyle/shaders.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/types.py` & `fake-bpy-module-latest-20230428/freestyle/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/utils/ContextFunctions.py` & `fake-bpy-module-latest-20230428/freestyle/utils/ContextFunctions.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/freestyle/utils/__init__.py` & `fake-bpy-module-latest-20230428/freestyle/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/capabilities.py` & `fake-bpy-module-latest-20230428/gpu/capabilities.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/matrix.py` & `fake-bpy-module-latest-20230428/gpu/matrix.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/platform.py` & `fake-bpy-module-latest-20230428/gpu/platform.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/shader.py` & `fake-bpy-module-latest-20230428/gpu/shader.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/state.py` & `fake-bpy-module-latest-20230428/gpu/state.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/texture.py` & `fake-bpy-module-latest-20230428/gpu/texture.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu/types.py` & `fake-bpy-module-latest-20230428/gpu/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu_extras/batch.py` & `fake-bpy-module-latest-20230428/gpu_extras/batch.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/gpu_extras/presets.py` & `fake-bpy-module-latest-20230428/gpu_extras/presets.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/idprop/types.py` & `fake-bpy-module-latest-20230428/idprop/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/imbuf/__init__.py` & `fake-bpy-module-latest-20230428/imbuf/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/imbuf/types.py` & `fake-bpy-module-latest-20230428/imbuf/types.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/keyingsets_builtins.py` & `fake-bpy-module-latest-20230428/keyingsets_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/keyingsets_utils.py` & `fake-bpy-module-latest-20230428/keyingsets_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/mathutils/__init__.py` & `fake-bpy-module-latest-20230428/mathutils/__init__.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/mathutils/bvhtree.py` & `fake-bpy-module-latest-20230428/mathutils/bvhtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/mathutils/geometry.py` & `fake-bpy-module-latest-20230428/mathutils/geometry.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/mathutils/kdtree.py` & `fake-bpy-module-latest-20230428/mathutils/kdtree.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/mathutils/noise.py` & `fake-bpy-module-latest-20230428/mathutils/noise.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/nodeitems_builtins.py` & `fake-bpy-module-latest-20230428/nodeitems_builtins.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/nodeitems_utils.py` & `fake-bpy-module-latest-20230428/nodeitems_utils.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/rna_info.py` & `fake-bpy-module-latest-20230428/rna_info.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/rna_keymap_ui.py` & `fake-bpy-module-latest-20230428/rna_keymap_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/rna_prop_ui.py` & `fake-bpy-module-latest-20230428/rna_prop_ui.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/rna_xml.py` & `fake-bpy-module-latest-20230428/rna_xml.py`

 * *Files identical despite different names*

### Comparing `fake-bpy-module-latest-20230427/setup.py` & `fake-bpy-module-latest-20230428/setup.py`

 * *Files identical despite different names*

