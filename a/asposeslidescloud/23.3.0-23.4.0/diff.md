# Comparing `tmp/asposeslidescloud-23.3.0.tar.gz` & `tmp/asposeslidescloud-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-23.3.0.tar", last modified: Fri Mar 24 19:31:05 2023, max compression
+gzip compressed data, was "dist/asposeslidescloud-23.4.0.tar", last modified: Sun Apr 23 12:37:00 2023, max compression
```

## Comparing `asposeslidescloud-23.3.0.tar` & `asposeslidescloud-23.4.0.tar`

### file list

```diff
@@ -1,268 +1,270 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-03-24 19:30:41.000000 asposeslidescloud-23.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7675 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7287 2023-03-24 19:30:44.000000 asposeslidescloud-23.3.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    17905 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28194 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      246 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1317247 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    17688 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    18977 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19140 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9725 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8034 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    25610 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4827 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)     9958 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5294 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6003 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5966 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    20135 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    11286 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14248 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7722 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    28850 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6348 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6404 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8656 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7749 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    17369 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    12213 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    12171 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)    15341 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5385 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7774 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7607 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15954 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    20604 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2023-03-24 19:30:38.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    17671 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14060 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10460 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15420 2023-03-24 19:30:39.000000 asposeslidescloud-23.3.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7675 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11145 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-24 19:31:05.000000 asposeslidescloud-23.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2023-03-24 19:30:50.000000 asposeslidescloud-23.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-04-23 12:36:30.000000 asposeslidescloud-23.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8064 2023-04-23 12:36:34.000000 asposeslidescloud-23.4.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    18067 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    28194 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      246 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1421835 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    17850 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    18977 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48257 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6280 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    19140 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4726 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8034 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    25610 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3772 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4827 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)     9958 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5294 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6003 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5966 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    20135 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    11286 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14248 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7722 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    28850 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6348 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6404 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8656 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7370 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6868 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7749 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    17369 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    12213 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    12171 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)    15341 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5385 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7774 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7607 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15954 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    17671 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14060 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10460 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15420 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8452 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11248 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2023-04-23 12:36:41.000000 asposeslidescloud-23.4.0/setup.py
```

### Comparing `asposeslidescloud-23.3.0/LICENSE` & `asposeslidescloud-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/PKG-INFO` & `asposeslidescloud-23.4.0/README`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: asposeslidescloud
-Version: 23.3.0
-Summary: Aspose.Slides Cloud SDK for Python
-Home-page: 
-Author: Victor Putrov
-Author-email: vistor.putrov@aspose.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -36,14 +23,22 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.4
+
+* Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
+* Added **UpdateTableCell** method to update table cells.
+* Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
+* Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
+* New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
+
 ## Enhancements in Version 23.3
 
 * Added **options** parameter to **SplitOnline** and **SplitAndSaveOnline** methods. Those options are the same as for other split & convert methods.
 * Added **ShowHiddenSlides** boolean property to **ImageExportOptions** class.
 
 ## Enhancements in Version 23.2
```

### Comparing `asposeslidescloud-23.3.0/README` & `asposeslidescloud-23.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: asposeslidescloud
+Version: 23.4.0
+Summary: Aspose.Slides Cloud SDK for Python
+Home-page: 
+Author: Victor Putrov
+Author-email: vistor.putrov@aspose.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -23,14 +36,22 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.4
+
+* Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
+* Added **UpdateTableCell** method to update table cells.
+* Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
+* Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
+* New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
+
 ## Enhancements in Version 23.3
 
 * Added **options** parameter to **SplitOnline** and **SplitAndSaveOnline** methods. Those options are the same as for other split & convert methods.
 * Added **ShowHiddenSlides** boolean property to **ImageExportOptions** class.
 
 ## Enhancements in Version 23.2
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/__init__.py` & `asposeslidescloud-23.4.0/asposeslidescloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,16 @@
 from asposeslidescloud.models.summary_zoom_frame import SummaryZoomFrame
 from asposeslidescloud.models.summary_zoom_section import SummaryZoomSection
 from asposeslidescloud.models.superscript_element import SuperscriptElement
 from asposeslidescloud.models.svg_export_options import SvgExportOptions
 from asposeslidescloud.models.swf_export_options import SwfExportOptions
 from asposeslidescloud.models.table import Table
 from asposeslidescloud.models.table_cell import TableCell
+from asposeslidescloud.models.table_cell_merge_options import TableCellMergeOptions
+from asposeslidescloud.models.table_cell_split_type import TableCellSplitType
 from asposeslidescloud.models.table_column import TableColumn
 from asposeslidescloud.models.table_row import TableRow
 from asposeslidescloud.models.task import Task
 from asposeslidescloud.models.text_bounds import TextBounds
 from asposeslidescloud.models.text_element import TextElement
 from asposeslidescloud.models.text_frame_format import TextFrameFormat
 from asposeslidescloud.models.text_item import TextItem
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/api_client.py` & `asposeslidescloud-23.4.0/asposeslidescloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v23.3.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v23.4.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-23.4.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-23.4.0/asposeslidescloud/apis/slides_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -4826,14 +4826,429 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def create_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Creates table cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param dto Paragraph DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.create_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def create_table_cell_paragraph_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Creates table cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.create_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param dto Paragraph DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_table_cell_paragraph" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `create_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `create_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `create_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `create_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `create_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `create_table_cell_paragraph`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Paragraph',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def create_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Creates table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param dto Portion DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.create_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def create_table_cell_portion_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Creates table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.create_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param dto Portion DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_table_cell_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `create_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `create_table_cell_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}/portions', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Portion',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def create_table_row(self, name, slide_index, shape_index, dto, position = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Inserts the table row in the specified position. If position is not specified, the row add to the end of the table.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, dto, position, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param dto Table row data.
+        :param position Position.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableRow
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.create_table_row_with_http_info(name, slide_index, shape_index, dto, position, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_table_row_with_http_info(name, slide_index, shape_index, dto, position, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def create_table_row_with_http_info(self, name, slide_index, shape_index, dto, position = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Inserts the table row in the specified position. If position is not specified, the row add to the end of the table.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.create_table_row_with_http_info(name, slide_index, shape_index, dto, position, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param dto Table row data.
+        :param position Position.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableRow
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method create_table_row" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `create_table_row`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `create_table_row`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `create_table_row`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `create_table_row`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+
+        query_params = []
+        if position:
+            query_params.append(('position', position))  # noqa: E501
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='TableRow',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def create_watermark(self, name, shape = None, font_height = None, text = None, font_name = None, font_color = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Adds a text watermark to each slide of the presentation. Text watermark can be setup via method arguments or withing Shape DTO for detailed customization. Both options are applicable simultaneously.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, shape, font_height, text, font_name, font_color, password, folder, storage, is_async=True)
         >>> result = thread.get()
@@ -10666,14 +11081,426 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def delete_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraphs
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.delete_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def delete_table_cell_paragraph_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.delete_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraphs
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_table_cell_paragraph" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `delete_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `delete_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `delete_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `delete_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `delete_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `delete_table_cell_paragraph`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Paragraphs',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete table ell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portions
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.delete_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def delete_table_cell_portion_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete table ell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.delete_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portions
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_table_cell_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `delete_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'portion_index' is set
+        if not portion_index:
+            raise ValueError("Missing the required parameter `portion_index` when calling `delete_table_cell_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+        path_params['portionIndex'] = portion_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}/portions/{portionIndex}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Portions',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_table_row(self, name, slide_index, shape_index, row_index, with_attached_rows = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Deletes the table row.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, with_attached_rows, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param with_attached_rows Also delete all attached rows.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.delete_table_row_with_http_info(name, slide_index, shape_index, row_index, with_attached_rows, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_table_row_with_http_info(name, slide_index, shape_index, row_index, with_attached_rows, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def delete_table_row_with_http_info(self, name, slide_index, shape_index, row_index, with_attached_rows = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Deletes the table row.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.delete_table_row_with_http_info(name, slide_index, shape_index, row_index, with_attached_rows, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param with_attached_rows Also delete all attached rows.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_table_row" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `delete_table_row`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `delete_table_row`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `delete_table_row`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `delete_table_row`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+
+        query_params = []
+        if with_attached_rows:
+            query_params.append(('withAttachedRows', with_attached_rows))  # noqa: E501
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Table',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def delete_unused_layout_slides(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes unused layout slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, password, folder, storage, is_async=True)
         >>> result = thread.get()
@@ -19893,14 +20720,566 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def get_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns paragraph info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_table_cell_paragraph_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns paragraph info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_table_cell_paragraph" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `get_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `get_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `get_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `get_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `get_table_cell_paragraph`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Paragraph',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_table_cell_paragraphs(self, name, slide_index, shape_index, row_index, cell_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell paragraphs.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraphs
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_table_cell_paragraphs_with_http_info(name, slide_index, shape_index, row_index, cell_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_table_cell_paragraphs_with_http_info(name, slide_index, shape_index, row_index, cell_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_table_cell_paragraphs_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell paragraphs.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_table_cell_paragraphs_with_http_info(name, slide_index, shape_index, row_index, cell_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraphs
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_table_cell_paragraphs" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_table_cell_paragraphs`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `get_table_cell_paragraphs`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `get_table_cell_paragraphs`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `get_table_cell_paragraphs`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `get_table_cell_paragraphs`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Paragraphs',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_table_cell_portion_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_table_cell_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `get_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'portion_index' is set
+        if not portion_index:
+            raise ValueError("Missing the required parameter `portion_index` when calling `get_table_cell_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+        path_params['portionIndex'] = portion_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}/portions/{portionIndex}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Portion',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_table_cell_portions(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell portions.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portions
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_table_cell_portions_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_table_cell_portions_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_table_cell_portions_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Returns table cell portions.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_table_cell_portions_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portions
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_table_cell_portions" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_table_cell_portions`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `get_table_cell_portions`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `get_table_cell_portions`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `get_table_cell_portions`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `get_table_cell_portions`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `get_table_cell_portions`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}/portions', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Portions',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def get_theme(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide theme info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, password, folder, storage, is_async=True)
         >>> result = thread.get()
@@ -21093,14 +22472,141 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def merge_table_cells(self, name, slide_index, shape_index, table_cell_merge_options, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Merge table cells.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, table_cell_merge_options, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param table_cell_merge_options Merge settings.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.merge_table_cells_with_http_info(name, slide_index, shape_index, table_cell_merge_options, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.merge_table_cells_with_http_info(name, slide_index, shape_index, table_cell_merge_options, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def merge_table_cells_with_http_info(self, name, slide_index, shape_index, table_cell_merge_options, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Merge table cells.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.merge_table_cells_with_http_info(name, slide_index, shape_index, table_cell_merge_options, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param table_cell_merge_options Merge settings.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method merge_table_cells" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `merge_table_cells`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `merge_table_cells`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `merge_table_cells`")  # noqa: E501
+        # verify the required parameter 'table_cell_merge_options' is set
+        if not table_cell_merge_options:
+            raise ValueError("Missing the required parameter `table_cell_merge_options` when calling `merge_table_cells`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if table_cell_merge_options:
+            body_params = table_cell_merge_options
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/mergeCells', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Table',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def move_file(self, src_path, dest_path, src_storage_name = None, dest_storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Move file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(src_path, dest_path, src_storage_name, dest_storage_name, version_id, is_async=True)
         >>> result = thread.get()
@@ -27345,14 +28851,161 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def split_table_cell(self, name, slide_index, shape_index, row_index, cell_index, split_type, value, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Split table cell.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, split_type, value, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param split_type Table cell split type (SplitByWidth, SplitByHeight,SplitByColSpan or SplitByRowSpan).
+        :param value Split value. In case of splitting by column or row span, the value must be an integer number.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.split_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, split_type, value, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.split_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, split_type, value, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def split_table_cell_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, split_type, value, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Split table cell.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.split_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, split_type, value, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param split_type Table cell split type (SplitByWidth, SplitByHeight,SplitByColSpan or SplitByRowSpan).
+        :param value Split value. In case of splitting by column or row span, the value must be an integer number.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Table
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method split_table_cell" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'split_type' is set
+        if not split_type:
+            raise ValueError("Missing the required parameter `split_type` when calling `split_table_cell`")  # noqa: E501
+        # verify the value of parameter 'split_type' is valid
+        if not split_type.upper() in TableCellSplitType.__dict__:
+            raise ValueError("Invalid value for parameter `split_type` when calling `split_table_cell`")  # noqa: E501
+        # verify the required parameter 'value' is set
+        if not value:
+            raise ValueError("Missing the required parameter `value` when calling `split_table_cell`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['splitType'] = split_type  # noqa: E501
+        path_params['value'] = value  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/{splitType}/{value}', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Table',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def storage_exists(self, storage_name, **kwargs):  # noqa: E501
         """Check if storage exists  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(storage_name, is_async=True)
         >>> result = thread.get()
@@ -29717,14 +31370,582 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def update_table_cell(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update the table cell.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param dto Table cell data.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableCell
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.update_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def update_table_cell_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update the table cell.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.update_table_cell_with_http_info(name, slide_index, shape_index, row_index, cell_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param dto Table cell data.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableCell
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_table_cell" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `update_table_cell`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `update_table_cell`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `update_table_cell`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `update_table_cell`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `update_table_cell`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `update_table_cell`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='TableCell',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Updates table cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param dto Paragraph DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.update_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def update_table_cell_paragraph_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Updates table cell paragraph.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.update_table_cell_paragraph_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param dto Paragraph DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Paragraph
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_table_cell_paragraph" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `update_table_cell_paragraph`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `update_table_cell_paragraph`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Paragraph',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Updates table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param dto Portion DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.update_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def update_table_cell_portion_with_http_info(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Updates table cell portion.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.update_table_cell_portion_with_http_info(name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param cell_index Table cell index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param dto Portion DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: Portion
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_table_cell_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'cell_index' is set
+        if not cell_index:
+            raise ValueError("Missing the required parameter `cell_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'portion_index' is set
+        if not portion_index:
+            raise ValueError("Missing the required parameter `portion_index` when calling `update_table_cell_portion`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `update_table_cell_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+        path_params['cellIndex'] = cell_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+        path_params['portionIndex'] = portion_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}/cells/{cellIndex}/paragraphs/{paragraphIndex}/portions/{portionIndex}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='Portion',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_table_row(self, name, slide_index, shape_index, row_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update the table row.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, row_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param dto Table cell data.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableRow
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.update_table_row_with_http_info(name, slide_index, shape_index, row_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_table_row_with_http_info(name, slide_index, shape_index, row_index, dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def update_table_row_with_http_info(self, name, slide_index, shape_index, row_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update the table row.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.update_table_row_with_http_info(name, slide_index, shape_index, row_index, dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param row_index Row index.
+        :param dto Table cell data.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: TableRow
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method update_table_row" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `update_table_row`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `update_table_row`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `update_table_row`")  # noqa: E501
+        # verify the required parameter 'row_index' is set
+        if not row_index:
+            raise ValueError("Missing the required parameter `row_index` when calling `update_table_row`")  # noqa: E501
+        # verify the required parameter 'dto' is set
+        if not dto:
+            raise ValueError("Missing the required parameter `dto` when calling `update_table_row`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['rowIndex'] = row_index  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+        if dto:
+            body_params = dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/rows/{rowIndex}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='TableRow',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def upload_file(self, path, file, storage_name = None, **kwargs):  # noqa: E501
         """Upload file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(path, file, storage_name, is_async=True)
         >>> result = thread.get()
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/configuration.py` & `asposeslidescloud-23.4.0/asposeslidescloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 23.3.0".\
+               "SDK Package Version: 23.4.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/error_message.py` & `asposeslidescloud-23.4.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,16 @@
 from asposeslidescloud.models.summary_zoom_frame import SummaryZoomFrame
 from asposeslidescloud.models.summary_zoom_section import SummaryZoomSection
 from asposeslidescloud.models.superscript_element import SuperscriptElement
 from asposeslidescloud.models.svg_export_options import SvgExportOptions
 from asposeslidescloud.models.swf_export_options import SwfExportOptions
 from asposeslidescloud.models.table import Table
 from asposeslidescloud.models.table_cell import TableCell
+from asposeslidescloud.models.table_cell_merge_options import TableCellMergeOptions
+from asposeslidescloud.models.table_cell_split_type import TableCellSplitType
 from asposeslidescloud.models.table_column import TableColumn
 from asposeslidescloud.models.table_row import TableRow
 from asposeslidescloud.models.task import Task
 from asposeslidescloud.models.text_bounds import TextBounds
 from asposeslidescloud.models.text_element import TextElement
 from asposeslidescloud.models.text_frame_format import TextFrameFormat
 from asposeslidescloud.models.text_item import TextItem
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/audio_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_title.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/connector.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/document.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/error.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/graphical_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/html5_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/html_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/image.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/images.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/input.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/path_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/pdf_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/pdf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/picture_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/portions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/save.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/save.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/save_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/section.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/series.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_base.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/table.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,15 +55,17 @@
         'border_top': 'LineFormat',
         'border_right': 'LineFormat',
         'border_left': 'LineFormat',
         'border_bottom': 'LineFormat',
         'border_diagonal_up': 'LineFormat',
         'border_diagonal_down': 'LineFormat',
         'column_index': 'int',
-        'row_index': 'int'
+        'row_index': 'int',
+        'text_frame_format': 'TextFrameFormat',
+        'paragraphs': 'ResourceUri'
     }
 
     attribute_map = {
         'text': 'text',
         'row_span': 'rowSpan',
         'col_span': 'colSpan',
         'margin_top': 'marginTop',
@@ -76,21 +78,23 @@
         'border_top': 'borderTop',
         'border_right': 'borderRight',
         'border_left': 'borderLeft',
         'border_bottom': 'borderBottom',
         'border_diagonal_up': 'borderDiagonalUp',
         'border_diagonal_down': 'borderDiagonalDown',
         'column_index': 'columnIndex',
-        'row_index': 'rowIndex'
+        'row_index': 'rowIndex',
+        'text_frame_format': 'textFrameFormat',
+        'paragraphs': 'paragraphs'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, text=None, row_span=None, col_span=None, margin_top=None, margin_right=None, margin_left=None, margin_bottom=None, text_anchor_type=None, text_vertical_type=None, fill_format=None, border_top=None, border_right=None, border_left=None, border_bottom=None, border_diagonal_up=None, border_diagonal_down=None, column_index=None, row_index=None):  # noqa: E501
+    def __init__(self, text=None, row_span=None, col_span=None, margin_top=None, margin_right=None, margin_left=None, margin_bottom=None, text_anchor_type=None, text_vertical_type=None, fill_format=None, border_top=None, border_right=None, border_left=None, border_bottom=None, border_diagonal_up=None, border_diagonal_down=None, column_index=None, row_index=None, text_frame_format=None, paragraphs=None):  # noqa: E501
         """TableCell - a model defined in Swagger"""  # noqa: E501
 
         self._text = None
         self._row_span = None
         self._col_span = None
         self._margin_top = None
         self._margin_right = None
@@ -103,14 +107,16 @@
         self._border_right = None
         self._border_left = None
         self._border_bottom = None
         self._border_diagonal_up = None
         self._border_diagonal_down = None
         self._column_index = None
         self._row_index = None
+        self._text_frame_format = None
+        self._paragraphs = None
 
         if text is not None:
             self.text = text
         if row_span is not None:
             self.row_span = row_span
         if col_span is not None:
             self.col_span = col_span
@@ -140,14 +146,18 @@
             self.border_diagonal_up = border_diagonal_up
         if border_diagonal_down is not None:
             self.border_diagonal_down = border_diagonal_down
         if column_index is not None:
             self.column_index = column_index
         if row_index is not None:
             self.row_index = row_index
+        if text_frame_format is not None:
+            self.text_frame_format = text_frame_format
+        if paragraphs is not None:
+            self.paragraphs = paragraphs
 
     @property
     def text(self):
         """Gets the text of this TableCell.  # noqa: E501
 
         Cell text.  # noqa: E501
 
@@ -569,14 +579,58 @@
         Cell row index  # noqa: E501
 
         :param row_index: The row_index of this TableCell.  # noqa: E501
         :type: int
         """
         self._row_index = row_index
 
+    @property
+    def text_frame_format(self):
+        """Gets the text_frame_format of this TableCell.  # noqa: E501
+
+        Returns TextFrame's formatting properties.  # noqa: E501
+
+        :return: The text_frame_format of this TableCell.  # noqa: E501
+        :rtype: TextFrameFormat
+        """
+        return self._text_frame_format
+
+    @text_frame_format.setter
+    def text_frame_format(self, text_frame_format):
+        """Sets the text_frame_format of this TableCell.
+
+        Returns TextFrame's formatting properties.  # noqa: E501
+
+        :param text_frame_format: The text_frame_format of this TableCell.  # noqa: E501
+        :type: TextFrameFormat
+        """
+        self._text_frame_format = text_frame_format
+
+    @property
+    def paragraphs(self):
+        """Gets the paragraphs of this TableCell.  # noqa: E501
+
+        Get or sets list to paragraphs list  # noqa: E501
+
+        :return: The paragraphs of this TableCell.  # noqa: E501
+        :rtype: ResourceUri
+        """
+        return self._paragraphs
+
+    @paragraphs.setter
+    def paragraphs(self, paragraphs):
+        """Sets the paragraphs of this TableCell.
+
+        Get or sets list to paragraphs list  # noqa: E501
+
+        :param paragraphs: The paragraphs of this TableCell.  # noqa: E501
+        :type: ResourceUri
+        """
+        self._paragraphs = paragraphs
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/task.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/text_items.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/tiff_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/tiff_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/video_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-23.4.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud/rest.py` & `asposeslidescloud-23.4.0/asposeslidescloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-23.4.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 23.3.0
+Version: 23.4.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,22 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.4
+
+* Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
+* Added **UpdateTableCell** method to update table cells.
+* Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
+* Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
+* New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
+
 ## Enhancements in Version 23.3
 
 * Added **options** parameter to **SplitOnline** and **SplitAndSaveOnline** methods. Those options are the same as for other split & convert methods.
 * Added **ShowHiddenSlides** boolean property to **ImageExportOptions** class.
 
 ## Enhancements in Version 23.2
```

### Comparing `asposeslidescloud-23.3.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-23.4.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,16 @@
 asposeslidescloud/models/summary_zoom_frame.py
 asposeslidescloud/models/summary_zoom_section.py
 asposeslidescloud/models/superscript_element.py
 asposeslidescloud/models/svg_export_options.py
 asposeslidescloud/models/swf_export_options.py
 asposeslidescloud/models/table.py
 asposeslidescloud/models/table_cell.py
+asposeslidescloud/models/table_cell_merge_options.py
+asposeslidescloud/models/table_cell_split_type.py
 asposeslidescloud/models/table_column.py
 asposeslidescloud/models/table_row.py
 asposeslidescloud/models/task.py
 asposeslidescloud/models/text_bounds.py
 asposeslidescloud/models/text_element.py
 asposeslidescloud/models/text_frame_format.py
 asposeslidescloud/models/text_item.py
```

### Comparing `asposeslidescloud-23.3.0/setup.py` & `asposeslidescloud-23.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="23.3.0",
+    version="23.4.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

