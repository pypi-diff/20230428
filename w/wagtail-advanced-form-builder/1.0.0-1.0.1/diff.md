# Comparing `tmp/wagtail-advanced-form-builder-1.0.0.tar.gz` & `tmp/wagtail-advanced-form-builder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-advanced-form-builder-1.0.0.tar", last modified: Fri Apr 28 00:09:01 2023, max compression
+gzip compressed data, was "dist/wagtail-advanced-form-builder-1.0.1.tar", last modified: Fri Apr 28 02:20:37 2023, max compression
```

## Comparing `wagtail-advanced-form-builder-1.0.0.tar` & `wagtail-advanced-form-builder-1.0.1.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.102157 wagtail-advanced-form-builder-1.0.0/
--rw-r--r--   0 richardblake   (502) staff       (20)      176 2020-10-07 18:46:22.000000 wagtail-advanced-form-builder-1.0.0/MANIFEST.in
--rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 00:09:01.101863 wagtail-advanced-form-builder-1.0.0/PKG-INFO
--rw-r--r--   0 richardblake   (502) staff       (20)     1621 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/README.md
--rw-r--r--   0 richardblake   (502) staff       (20)       79 2020-10-07 08:36:01.000000 wagtail-advanced-form-builder-1.0.0/dev-requirements.txt
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.021623 wagtail-advanced-form-builder-1.0.0/docs/
--rw-r--r--   0 richardblake   (502) staff       (20)     6148 2023-04-27 21:09:10.000000 wagtail-advanced-form-builder-1.0.0/docs/.DS_Store
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.022645 wagtail-advanced-form-builder-1.0.0/docs/contributing/
--rw-r--r--   0 richardblake   (502) staff       (20)     1231 2020-10-12 06:42:38.000000 wagtail-advanced-form-builder-1.0.0/docs/contributing/contributing.md
--rw-r--r--   0 richardblake   (502) staff       (20)       32 2020-10-12 06:17:08.000000 wagtail-advanced-form-builder-1.0.0/docs/extra.css
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.031648 wagtail-advanced-form-builder-1.0.0/docs/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      627 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/basic_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      652 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/checkbox_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      716 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/checkboxes_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      678 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/dropdown_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      347 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/email_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      308 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/hidden_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      582 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/html_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      571 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/multi_line_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/multi_select_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      556 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/number_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      661 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/radio_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      241 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/fields/url_field.md
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.033833 wagtail-advanced-form-builder-1.0.0/docs/getting_started/
--rw-r--r--   0 richardblake   (502) staff       (20)      377 2020-10-12 00:46:04.000000 wagtail-advanced-form-builder-1.0.0/docs/getting_started/installing.md
--rw-r--r--   0 richardblake   (502) staff       (20)     1613 2020-10-12 07:09:40.000000 wagtail-advanced-form-builder-1.0.0/docs/getting_started/out_of_the_box.md
--rw-r--r--   0 richardblake   (502) staff       (20)     4012 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/docs/getting_started/using_your_own_page_models.md
--rw-r--r--   0 richardblake   (502) staff       (20)      361 2020-10-14 03:24:47.000000 wagtail-advanced-form-builder-1.0.0/docs/index.md
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.038713 wagtail-advanced-form-builder-1.0.0/docs/screenshots/
--rw-r--r--   0 richardblake   (502) staff       (20)     6148 2020-11-09 01:57:33.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/.DS_Store
--rw-r--r--   0 richardblake   (502) staff       (20)   179457 2020-10-14 03:20:44.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/custom-form-builder-page.png
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.056265 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)   131975 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-basic-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    86006 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-checkbox-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   122117 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-checkboxes-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   111163 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-dropdown-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    39635 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-hidden-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    73032 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-html-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   118420 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-multiline-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   113896 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-multiselect-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   118837 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-number-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   114023 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-radio-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   265511 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/docs/screenshots/waf-form-fields.png
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.057211 wagtail-advanced-form-builder-1.0.0/docs/usage/
--rw-r--r--   0 richardblake   (502) staff       (20)       11 2020-10-13 20:12:41.000000 wagtail-advanced-form-builder-1.0.0/docs/usage/settings.md
--rw-r--r--   0 richardblake   (502) staff       (20)       93 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/requirements.txt
--rw-r--r--   0 richardblake   (502) staff       (20)       38 2023-04-28 00:09:01.102250 wagtail-advanced-form-builder-1.0.0/setup.cfg
--rw-r--r--   0 richardblake   (502) staff       (20)     1323 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/setup.py
--rw-r--r--   0 richardblake   (502) staff       (20)       84 2020-10-07 08:37:02.000000 wagtail-advanced-form-builder-1.0.0/test-requirements.txt
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.059954 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      271 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/apps.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.065018 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)       94 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      526 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/base_static_block.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.075531 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      250 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)     1780 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/base_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      363 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/blank_condition_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      468 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/checkbox_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      745 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      580 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/condition_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      757 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/conditional_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      490 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/dropdown_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      306 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/email_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      618 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      699 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/html_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      385 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/multi_line_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      521 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      354 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/number_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      475 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/radio_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      317 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/single_line_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      325 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/url_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/inline_form_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)     1724 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/constants.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.076467 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/
--rw-r--r--   0 richardblake   (502) staff       (20)       55 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)     3242 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/advanced_form_builder.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.079205 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      520 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      237 2020-11-16 10:31:42.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/side_by_side_checkbox_select_multiple_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      212 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/side_by_side_radio_select_widget.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.081939 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/
--rw-r--r--   0 richardblake   (502) staff       (20)    53059 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0001_initial.py
--rw-r--r--   0 richardblake   (502) staff       (20)    43466 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py
--rw-r--r--   0 richardblake   (502) staff       (20)    45293 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/__init__.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.086526 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/
--rw-r--r--   0 richardblake   (502) staff       (20)      154 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      848 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py
--rw-r--r--   0 richardblake   (502) staff       (20)      300 2020-10-13 08:19:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_form.py
--rw-r--r--   0 richardblake   (502) staff       (20)     2498 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)    14149 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py
--rw-r--r--   0 richardblake   (502) staff       (20)      631 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/email_form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)      324 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/email_form_page.py
--rw-r--r--   0 richardblake   (502) staff       (20)      621 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)      329 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/form_page.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.010854 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.011167 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.086904 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/
--rw-r--r--   0 richardblake   (502) staff       (20)     1310 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.089372 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/
--rw-r--r--   0 richardblake   (502) staff       (20)    20265 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js
--rw-r--r--   0 richardblake   (502) staff       (20)    23187 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js
--rw-r--r--   0 richardblake   (502) staff       (20)     1004 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.011591 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.012034 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.090262 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/
--rw-r--r--   0 richardblake   (502) staff       (20)     7154 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js
--rw-r--r--   0 richardblake   (502) staff       (20)     8386 2020-12-11 00:23:59.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.090804 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/
--rw-r--r--   0 richardblake   (502) staff       (20)     1140 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.012807 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.014887 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.013151 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.091231 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)      104 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/base_static_block.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.091953 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)       99 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/inline_form_block.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.093670 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/
--rw-r--r--   0 richardblake   (502) staff       (20)      131 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_error.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_help_text.html
--rw-r--r--   0 richardblake   (502) staff       (20)      108 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_label.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.096012 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      773 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      563 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      832 2020-11-16 10:35:17.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      822 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      463 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/text_area_field.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.097538 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/
--rw-r--r--   0 richardblake   (502) staff       (20)      555 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html
--rw-r--r--   0 richardblake   (502) staff       (20)      335 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form_builder.html
--rw-r--r--   0 richardblake   (502) staff       (20)      179 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/no_script_notification.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.099890 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/
--rw-r--r--   0 richardblake   (502) staff       (20)      594 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html
--rw-r--r--   0 richardblake   (502) staff       (20)      442 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_complete.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_end.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_start.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.100300 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/
--rw-r--r--   0 richardblake   (502) staff       (20)     1164 2020-11-16 10:37:13.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.100682 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/
--rw-r--r--   0 richardblake   (502) staff       (20)      234 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/html_output_widget.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.101295 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templatetags/
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templatetags/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py
--rw-r--r--   0 richardblake   (502) staff       (20)      367 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/utils.py
--rw-r--r--   0 richardblake   (502) staff       (20)      452 2023-04-27 23:43:26.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/wagtail_hooks.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 00:09:01.063326 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/
--rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 00:09:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/PKG-INFO
--rw-r--r--   0 richardblake   (502) staff       (20)     6893 2023-04-28 00:09:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/SOURCES.txt
--rw-r--r--   0 richardblake   (502) staff       (20)        1 2023-04-28 00:09:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/dependency_links.txt
--rw-r--r--   0 richardblake   (502) staff       (20)        1 2020-11-16 09:23:33.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/not-zip-safe
--rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 00:09:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/requires.txt
--rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 00:09:00.000000 wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/top_level.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.950534 wagtail-advanced-form-builder-1.0.1/
+-rw-r--r--   0 richardblake   (502) staff       (20)      176 2020-10-07 18:46:22.000000 wagtail-advanced-form-builder-1.0.1/MANIFEST.in
+-rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:20:37.950013 wagtail-advanced-form-builder-1.0.1/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)     1621 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/README.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       79 2020-10-07 08:36:01.000000 wagtail-advanced-form-builder-1.0.1/dev-requirements.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.848203 wagtail-advanced-form-builder-1.0.1/docs/
+-rw-r--r--   0 richardblake   (502) staff       (20)     6148 2023-04-27 21:09:10.000000 wagtail-advanced-form-builder-1.0.1/docs/.DS_Store
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.848893 wagtail-advanced-form-builder-1.0.1/docs/contributing/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1231 2020-10-12 06:42:38.000000 wagtail-advanced-form-builder-1.0.1/docs/contributing/contributing.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       32 2020-10-12 06:17:08.000000 wagtail-advanced-form-builder-1.0.1/docs/extra.css
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.857773 wagtail-advanced-form-builder-1.0.1/docs/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      627 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/basic_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      652 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/checkbox_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      716 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/checkboxes_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      678 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/dropdown_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      347 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/email_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      308 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/hidden_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      582 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/html_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      571 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/multi_line_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/multi_select_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      556 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/number_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      661 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/radio_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      241 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/url_field.md
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.860164 wagtail-advanced-form-builder-1.0.1/docs/getting_started/
+-rw-r--r--   0 richardblake   (502) staff       (20)      377 2020-10-12 00:46:04.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/installing.md
+-rw-r--r--   0 richardblake   (502) staff       (20)     1613 2020-10-12 07:09:40.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/out_of_the_box.md
+-rw-r--r--   0 richardblake   (502) staff       (20)     4012 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/using_your_own_page_models.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      361 2020-10-14 03:24:47.000000 wagtail-advanced-form-builder-1.0.1/docs/index.md
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.864454 wagtail-advanced-form-builder-1.0.1/docs/screenshots/
+-rw-r--r--   0 richardblake   (502) staff       (20)     6148 2020-11-09 01:57:33.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/.DS_Store
+-rw-r--r--   0 richardblake   (502) staff       (20)   179457 2020-10-14 03:20:44.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/custom-form-builder-page.png
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.882748 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)   131975 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-basic-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    86006 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkbox-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   122117 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkboxes-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   111163 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-dropdown-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    39635 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-hidden-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    73032 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-html-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   118420 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiline-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   113896 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiselect-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   118837 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-number-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   114023 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-radio-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   265511 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/waf-form-fields.png
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.884806 wagtail-advanced-form-builder-1.0.1/docs/usage/
+-rw-r--r--   0 richardblake   (502) staff       (20)       11 2020-10-13 20:12:41.000000 wagtail-advanced-form-builder-1.0.1/docs/usage/settings.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       93 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/requirements.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)       38 2023-04-28 02:20:37.950698 wagtail-advanced-form-builder-1.0.1/setup.cfg
+-rw-r--r--   0 richardblake   (502) staff       (20)     1323 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/setup.py
+-rw-r--r--   0 richardblake   (502) staff       (20)       84 2020-10-07 08:37:02.000000 wagtail-advanced-form-builder-1.0.1/test-requirements.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.889592 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2023-04-28 02:20:01.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      271 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/apps.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.896525 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)       94 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      526 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/base_static_block.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.909170 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      250 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1780 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/base_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      363 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/blank_condition_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      468 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkbox_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      745 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      580 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/condition_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      757 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/conditional_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      490 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/dropdown_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      306 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/email_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      618 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      699 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/html_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      385 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multi_line_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      521 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      354 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/number_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      475 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/radio_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      317 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/single_line_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      325 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/url_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/inline_form_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1724 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/constants.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.910657 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/
+-rw-r--r--   0 richardblake   (502) staff       (20)       55 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     3242 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/advanced_form_builder.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.913807 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      520 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      237 2020-11-16 10:31:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/side_by_side_checkbox_select_multiple_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      212 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/side_by_side_radio_select_widget.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.918075 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/
+-rw-r--r--   0 richardblake   (502) staff       (20)    53059 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0001_initial.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    43466 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    45293 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/__init__.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.924568 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/
+-rw-r--r--   0 richardblake   (502) staff       (20)      154 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      848 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      300 2020-10-13 08:19:00.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     2498 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    14149 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      631 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      324 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_page.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      621 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      329 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_page.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.837631 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838101 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.925351 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1310 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.928421 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/
+-rw-r--r--   0 richardblake   (502) staff       (20)    20265 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js
+-rw-r--r--   0 richardblake   (502) staff       (20)    23187 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js
+-rw-r--r--   0 richardblake   (502) staff       (20)     1004 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838544 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838891 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.929818 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/
+-rw-r--r--   0 richardblake   (502) staff       (20)     7632 2023-04-28 02:20:01.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js
+-rw-r--r--   0 richardblake   (502) staff       (20)     8386 2020-12-11 00:23:59.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.930609 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1140 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.839371 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.840926 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.839685 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.931505 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)      104 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/base_static_block.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.932674 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)       99 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/inline_form_block.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.935152 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/
+-rw-r--r--   0 richardblake   (502) staff       (20)      131 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_error.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_help_text.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      108 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_label.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.939474 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      773 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      563 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      832 2020-11-16 10:35:17.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      822 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      463 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/text_area_field.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.941916 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/
+-rw-r--r--   0 richardblake   (502) staff       (20)      555 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      335 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form_builder.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      179 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/no_script_notification.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.945033 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/
+-rw-r--r--   0 richardblake   (502) staff       (20)      594 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      442 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_complete.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_end.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_start.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.945957 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1164 2020-11-16 10:37:13.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.946975 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/
+-rw-r--r--   0 richardblake   (502) staff       (20)      234 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/html_output_widget.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.948708 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      367 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/utils.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      452 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/wagtail_hooks.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.894284 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/
+-rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)     6893 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)        1 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)        1 2020-11-16 09:23:33.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/not-zip-safe
+-rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/requires.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/top_level.txt
```

### Comparing `wagtail-advanced-form-builder-1.0.0/PKG-INFO` & `wagtail-advanced-form-builder-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtail-advanced-form-builder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wagtail Advanced Form Builder
 Home-page: https://github.com/octavenz/wagtail-advanced-form-builder
 Author: Richard Blake (Octave)
 Author-email: richard.blake@octave.nz
 License: BSD
 Description: # Wagtail Advanced Form Builder
```

### Comparing `wagtail-advanced-form-builder-1.0.0/README.md` & `wagtail-advanced-form-builder-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/.DS_Store` & `wagtail-advanced-form-builder-1.0.1/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/contributing/contributing.md` & `wagtail-advanced-form-builder-1.0.1/docs/contributing/contributing.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/basic_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/basic_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/checkbox_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/checkbox_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/checkboxes_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/checkboxes_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/dropdown_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/dropdown_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/html_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/html_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/multi_line_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/multi_line_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/multi_select_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/multi_select_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/number_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/number_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/fields/radio_field.md` & `wagtail-advanced-form-builder-1.0.1/docs/fields/radio_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/getting_started/out_of_the_box.md` & `wagtail-advanced-form-builder-1.0.1/docs/getting_started/out_of_the_box.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/getting_started/using_your_own_page_models.md` & `wagtail-advanced-form-builder-1.0.1/docs/getting_started/using_your_own_page_models.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/.DS_Store` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/custom-form-builder-page.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/custom-form-builder-page.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-basic-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-basic-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-checkbox-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkbox-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-checkboxes-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkboxes-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-dropdown-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-dropdown-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-hidden-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-hidden-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-html-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-html-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-multiline-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiline-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-multiselect-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiselect-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-number-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-number-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/fields/waf-radio-field.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-radio-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/docs/screenshots/waf-form-fields.png` & `wagtail-advanced-form-builder-1.0.1/docs/screenshots/waf-form-fields.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/setup.py` & `wagtail-advanced-form-builder-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/base_static_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/base_static_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/base_field_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/base_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/condition_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/condition_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/conditional_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/conditional_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/html_field_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/html_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/blocks/inline_form_block.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/inline_form_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/constants.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/constants.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/advanced_form_builder.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/advanced_form_builder.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0001_initial.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/email_form_field.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/models/form_field.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -123,15 +123,24 @@
     constructor() {
         this.mutationObserverConfig = {
             attributes: true,
             childList: true,
             characterData: true,
             subTree: true,
         };
-        this.streamfieldList = $('.waf--field').first().parents('[data-streamfield-stream-container]')[0];
+
+        // Fetch the streamfield field containers so mutation observers can be attached.
+        this.streamfieldList = $('.waf--field').first().parents('[data-streamfield-stream-container]');
+
+        // Handles the case where there aren't any waf--fields on the form page yet.
+        if (!this.streamfieldList.length) {
+            this.streamfieldList = $('[data-streamfield-stream-container]');
+        }
+
+        // Fetch any existing conditions blocks on existing fields so mutation observers can be attached to them.
         this.formRulesLists = $('[data-contentpath="conditions"]').find('[data-streamfield-stream-container]');
     }
 
     monitorMutations() {
 
         this.newFieldMutationObserver = new MutationObserver(((mutations) => {
             mutations.forEach((mutation) => {
@@ -142,15 +151,17 @@
                     $nodes.find('[data-contentpath="conditions"]').find('[data-streamfield-stream-container]').each((index, element) => {
                         this.newRuleMutationObserver.observe(element, this.mutationObserverConfig);
                     });
                 }
             });
         }));
 
-        this.newFieldMutationObserver.observe(this.streamfieldList, this.mutationObserverConfig);
+        this.streamfieldList.each((index, element) => {
+            this.newFieldMutationObserver.observe(element, this.mutationObserverConfig);
+        });
 
         this.newRuleMutationObserver = new MutationObserver(((mutations) => {
             mutations.forEach((mutation) => {
                 const newNodes = mutation.addedNodes; // DOM NodeList
                 if (newNodes !== null) { // If there are new nodes added
                     this.fieldRegistry.registerFieldNames();
                 }
```

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/PKG-INFO` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtail-advanced-form-builder
-Version: 1.0.0
+Version: 1.0.1
 Summary: Wagtail Advanced Form Builder
 Home-page: https://github.com/octavenz/wagtail-advanced-form-builder
 Author: Richard Blake (Octave)
 Author-email: richard.blake@octave.nz
 License: BSD
 Description: # Wagtail Advanced Form Builder
```

### Comparing `wagtail-advanced-form-builder-1.0.0/wagtail_advanced_form_builder.egg-info/SOURCES.txt` & `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

