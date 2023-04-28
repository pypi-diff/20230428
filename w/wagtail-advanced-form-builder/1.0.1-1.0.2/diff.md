# Comparing `tmp/wagtail-advanced-form-builder-1.0.1.tar.gz` & `tmp/wagtail-advanced-form-builder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wagtail-advanced-form-builder-1.0.1.tar", last modified: Fri Apr 28 02:20:37 2023, max compression
+gzip compressed data, was "dist/wagtail-advanced-form-builder-1.0.2.tar", last modified: Fri Apr 28 02:41:19 2023, max compression
```

## Comparing `wagtail-advanced-form-builder-1.0.1.tar` & `wagtail-advanced-form-builder-1.0.2.tar`

### file list

```diff
@@ -1,156 +1,156 @@
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.950534 wagtail-advanced-form-builder-1.0.1/
--rw-r--r--   0 richardblake   (502) staff       (20)      176 2020-10-07 18:46:22.000000 wagtail-advanced-form-builder-1.0.1/MANIFEST.in
--rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:20:37.950013 wagtail-advanced-form-builder-1.0.1/PKG-INFO
--rw-r--r--   0 richardblake   (502) staff       (20)     1621 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/README.md
--rw-r--r--   0 richardblake   (502) staff       (20)       79 2020-10-07 08:36:01.000000 wagtail-advanced-form-builder-1.0.1/dev-requirements.txt
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.848203 wagtail-advanced-form-builder-1.0.1/docs/
--rw-r--r--   0 richardblake   (502) staff       (20)     6148 2023-04-27 21:09:10.000000 wagtail-advanced-form-builder-1.0.1/docs/.DS_Store
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.848893 wagtail-advanced-form-builder-1.0.1/docs/contributing/
--rw-r--r--   0 richardblake   (502) staff       (20)     1231 2020-10-12 06:42:38.000000 wagtail-advanced-form-builder-1.0.1/docs/contributing/contributing.md
--rw-r--r--   0 richardblake   (502) staff       (20)       32 2020-10-12 06:17:08.000000 wagtail-advanced-form-builder-1.0.1/docs/extra.css
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.857773 wagtail-advanced-form-builder-1.0.1/docs/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      627 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/basic_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      652 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/checkbox_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      716 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/checkboxes_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      678 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/dropdown_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      347 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/email_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      308 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/hidden_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      582 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/html_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      571 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/multi_line_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/multi_select_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      556 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/number_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      661 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/radio_field.md
--rw-r--r--   0 richardblake   (502) staff       (20)      241 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/fields/url_field.md
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.860164 wagtail-advanced-form-builder-1.0.1/docs/getting_started/
--rw-r--r--   0 richardblake   (502) staff       (20)      377 2020-10-12 00:46:04.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/installing.md
--rw-r--r--   0 richardblake   (502) staff       (20)     1613 2020-10-12 07:09:40.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/out_of_the_box.md
--rw-r--r--   0 richardblake   (502) staff       (20)     4012 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/docs/getting_started/using_your_own_page_models.md
--rw-r--r--   0 richardblake   (502) staff       (20)      361 2020-10-14 03:24:47.000000 wagtail-advanced-form-builder-1.0.1/docs/index.md
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.864454 wagtail-advanced-form-builder-1.0.1/docs/screenshots/
--rw-r--r--   0 richardblake   (502) staff       (20)     6148 2020-11-09 01:57:33.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/.DS_Store
--rw-r--r--   0 richardblake   (502) staff       (20)   179457 2020-10-14 03:20:44.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/custom-form-builder-page.png
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.882748 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)   131975 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-basic-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    86006 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkbox-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   122117 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkboxes-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   111163 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-dropdown-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    39635 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-hidden-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)    73032 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-html-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   118420 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiline-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   113896 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiselect-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   118837 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-number-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   114023 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-radio-field.png
--rw-r--r--   0 richardblake   (502) staff       (20)   265511 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/docs/screenshots/waf-form-fields.png
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.884806 wagtail-advanced-form-builder-1.0.1/docs/usage/
--rw-r--r--   0 richardblake   (502) staff       (20)       11 2020-10-13 20:12:41.000000 wagtail-advanced-form-builder-1.0.1/docs/usage/settings.md
--rw-r--r--   0 richardblake   (502) staff       (20)       93 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/requirements.txt
--rw-r--r--   0 richardblake   (502) staff       (20)       38 2023-04-28 02:20:37.950698 wagtail-advanced-form-builder-1.0.1/setup.cfg
--rw-r--r--   0 richardblake   (502) staff       (20)     1323 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/setup.py
--rw-r--r--   0 richardblake   (502) staff       (20)       84 2020-10-07 08:37:02.000000 wagtail-advanced-form-builder-1.0.1/test-requirements.txt
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.889592 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2023-04-28 02:20:01.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      271 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/apps.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.896525 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)       94 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      526 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/base_static_block.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.909170 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      250 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)     1780 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/base_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      363 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/blank_condition_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      468 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkbox_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      745 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      580 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/condition_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      757 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/conditional_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      490 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/dropdown_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      306 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/email_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      618 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      699 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/html_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      385 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multi_line_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      521 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      354 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/number_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      475 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/radio_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      317 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/single_line_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      325 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/url_field_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/inline_form_block.py
--rw-r--r--   0 richardblake   (502) staff       (20)     1724 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/constants.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.910657 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/
--rw-r--r--   0 richardblake   (502) staff       (20)       55 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)     3242 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/advanced_form_builder.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.913807 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      520 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      237 2020-11-16 10:31:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/side_by_side_checkbox_select_multiple_widget.py
--rw-r--r--   0 richardblake   (502) staff       (20)      212 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/side_by_side_radio_select_widget.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.918075 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/
--rw-r--r--   0 richardblake   (502) staff       (20)    53059 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0001_initial.py
--rw-r--r--   0 richardblake   (502) staff       (20)    43466 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py
--rw-r--r--   0 richardblake   (502) staff       (20)    45293 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/__init__.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.924568 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/
--rw-r--r--   0 richardblake   (502) staff       (20)      154 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      848 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py
--rw-r--r--   0 richardblake   (502) staff       (20)      300 2020-10-13 08:19:00.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form.py
--rw-r--r--   0 richardblake   (502) staff       (20)     2498 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)    14149 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py
--rw-r--r--   0 richardblake   (502) staff       (20)      631 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)      324 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_page.py
--rw-r--r--   0 richardblake   (502) staff       (20)      621 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_field.py
--rw-r--r--   0 richardblake   (502) staff       (20)      329 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_page.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.837631 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838101 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.925351 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/
--rw-r--r--   0 richardblake   (502) staff       (20)     1310 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.928421 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/
--rw-r--r--   0 richardblake   (502) staff       (20)    20265 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js
--rw-r--r--   0 richardblake   (502) staff       (20)    23187 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js
--rw-r--r--   0 richardblake   (502) staff       (20)     1004 2023-04-27 23:38:42.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838544 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.838891 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.929818 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/
--rw-r--r--   0 richardblake   (502) staff       (20)     7632 2023-04-28 02:20:01.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js
--rw-r--r--   0 richardblake   (502) staff       (20)     8386 2020-12-11 00:23:59.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.930609 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/
--rw-r--r--   0 richardblake   (502) staff       (20)     1140 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.839371 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.840926 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.839685 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.931505 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)      104 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/base_static_block.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.932674 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/
--rw-r--r--   0 richardblake   (502) staff       (20)       99 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/inline_form_block.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.935152 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/
--rw-r--r--   0 richardblake   (502) staff       (20)      131 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_error.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_help_text.html
--rw-r--r--   0 richardblake   (502) staff       (20)      108 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_label.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.939474 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/
--rw-r--r--   0 richardblake   (502) staff       (20)      773 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      563 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      832 2020-11-16 10:35:17.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      822 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html
--rw-r--r--   0 richardblake   (502) staff       (20)      463 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/text_area_field.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.941916 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/
--rw-r--r--   0 richardblake   (502) staff       (20)      555 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html
--rw-r--r--   0 richardblake   (502) staff       (20)      335 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form_builder.html
--rw-r--r--   0 richardblake   (502) staff       (20)      179 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/no_script_notification.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.945033 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/
--rw-r--r--   0 richardblake   (502) staff       (20)      594 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html
--rw-r--r--   0 richardblake   (502) staff       (20)      442 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_complete.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_end.html
--rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_start.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.945957 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/
--rw-r--r--   0 richardblake   (502) staff       (20)     1164 2020-11-16 10:37:13.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.946975 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/
--rw-r--r--   0 richardblake   (502) staff       (20)      234 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/html_output_widget.html
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.948708 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/
--rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/__init__.py
--rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py
--rw-r--r--   0 richardblake   (502) staff       (20)      367 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/utils.py
--rw-r--r--   0 richardblake   (502) staff       (20)      452 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/wagtail_hooks.py
-drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:20:37.894284 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/
--rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/PKG-INFO
--rw-r--r--   0 richardblake   (502) staff       (20)     6893 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/SOURCES.txt
--rw-r--r--   0 richardblake   (502) staff       (20)        1 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/dependency_links.txt
--rw-r--r--   0 richardblake   (502) staff       (20)        1 2020-11-16 09:23:33.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/not-zip-safe
--rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/requires.txt
--rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:20:37.000000 wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/top_level.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.054578 wagtail-advanced-form-builder-1.0.2/
+-rw-r--r--   0 richardblake   (502) staff       (20)      176 2020-10-07 18:46:22.000000 wagtail-advanced-form-builder-1.0.2/MANIFEST.in
+-rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:41:19.054028 wagtail-advanced-form-builder-1.0.2/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)     1621 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/README.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       79 2020-10-07 08:36:01.000000 wagtail-advanced-form-builder-1.0.2/dev-requirements.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.927574 wagtail-advanced-form-builder-1.0.2/docs/
+-rw-r--r--   0 richardblake   (502) staff       (20)     6148 2023-04-27 21:09:10.000000 wagtail-advanced-form-builder-1.0.2/docs/.DS_Store
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.928255 wagtail-advanced-form-builder-1.0.2/docs/contributing/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1231 2020-10-12 06:42:38.000000 wagtail-advanced-form-builder-1.0.2/docs/contributing/contributing.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       32 2020-10-12 06:17:08.000000 wagtail-advanced-form-builder-1.0.2/docs/extra.css
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.936299 wagtail-advanced-form-builder-1.0.2/docs/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      627 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/basic_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      652 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/checkbox_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      716 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/checkboxes_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      678 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/dropdown_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      347 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/email_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      308 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/hidden_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      582 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/html_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      571 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/multi_line_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/multi_select_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      556 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/number_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      661 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/radio_field.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      241 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/fields/url_field.md
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.938587 wagtail-advanced-form-builder-1.0.2/docs/getting_started/
+-rw-r--r--   0 richardblake   (502) staff       (20)      377 2020-10-12 00:46:04.000000 wagtail-advanced-form-builder-1.0.2/docs/getting_started/installing.md
+-rw-r--r--   0 richardblake   (502) staff       (20)     1613 2020-10-12 07:09:40.000000 wagtail-advanced-form-builder-1.0.2/docs/getting_started/out_of_the_box.md
+-rw-r--r--   0 richardblake   (502) staff       (20)     4012 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/docs/getting_started/using_your_own_page_models.md
+-rw-r--r--   0 richardblake   (502) staff       (20)      361 2020-10-14 03:24:47.000000 wagtail-advanced-form-builder-1.0.2/docs/index.md
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.944111 wagtail-advanced-form-builder-1.0.2/docs/screenshots/
+-rw-r--r--   0 richardblake   (502) staff       (20)     6148 2020-11-09 01:57:33.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/.DS_Store
+-rw-r--r--   0 richardblake   (502) staff       (20)   179457 2020-10-14 03:20:44.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/custom-form-builder-page.png
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.971137 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)   131975 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-basic-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    86006 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-checkbox-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   122117 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-checkboxes-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   111163 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-dropdown-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    39635 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-hidden-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)    73032 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-html-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   118420 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-multiline-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   113896 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-multiselect-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   118837 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-number-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   114023 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-radio-field.png
+-rw-r--r--   0 richardblake   (502) staff       (20)   265511 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/docs/screenshots/waf-form-fields.png
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.973247 wagtail-advanced-form-builder-1.0.2/docs/usage/
+-rw-r--r--   0 richardblake   (502) staff       (20)       11 2020-10-13 20:12:41.000000 wagtail-advanced-form-builder-1.0.2/docs/usage/settings.md
+-rw-r--r--   0 richardblake   (502) staff       (20)       93 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/requirements.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)       38 2023-04-28 02:41:19.054777 wagtail-advanced-form-builder-1.0.2/setup.cfg
+-rw-r--r--   0 richardblake   (502) staff       (20)     1323 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/setup.py
+-rw-r--r--   0 richardblake   (502) staff       (20)       84 2020-10-07 08:37:02.000000 wagtail-advanced-form-builder-1.0.2/test-requirements.txt
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.976786 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2023-04-28 02:41:01.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      271 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/apps.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.981340 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)       94 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      526 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/base_static_block.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.994247 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      250 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1780 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/base_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      363 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/blank_condition_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      468 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/checkbox_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      745 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      580 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/condition_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      757 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/conditional_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      490 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/dropdown_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      306 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/email_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      618 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      699 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/html_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      385 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/multi_line_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      521 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      354 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/number_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      475 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/radio_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      317 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/single_line_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      325 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/url_field_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/inline_form_block.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     1724 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/constants.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.996417 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/
+-rw-r--r--   0 richardblake   (502) staff       (20)       55 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     3242 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/advanced_form_builder.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.008662 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      520 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      528 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      237 2020-11-16 10:31:42.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/side_by_side_checkbox_select_multiple_widget.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      212 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/side_by_side_radio_select_widget.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.014420 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/
+-rw-r--r--   0 richardblake   (502) staff       (20)    53059 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0001_initial.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    43466 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    45293 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/__init__.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.025351 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/
+-rw-r--r--   0 richardblake   (502) staff       (20)      154 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      848 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      300 2020-10-13 08:19:00.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_form.py
+-rw-r--r--   0 richardblake   (502) staff       (20)     2498 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)    14149 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      631 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/email_form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      324 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/email_form_page.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      621 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/form_field.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      329 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/form_page.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.921160 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.921443 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.026509 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1310 2023-04-28 02:41:14.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.028973 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/
+-rw-r--r--   0 richardblake   (502) staff       (20)    17399 2023-04-28 02:41:14.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js
+-rw-r--r--   0 richardblake   (502) staff       (20)    23182 2023-04-28 02:41:14.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js
+-rw-r--r--   0 richardblake   (502) staff       (20)     1004 2023-04-28 02:41:14.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.921649 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.921854 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.031386 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/
+-rw-r--r--   0 richardblake   (502) staff       (20)     7632 2023-04-28 02:20:01.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js
+-rw-r--r--   0 richardblake   (502) staff       (20)     8386 2020-12-11 00:23:59.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.033380 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1140 2020-11-16 09:21:25.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.922116 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.923331 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.922408 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.033985 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)      104 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/admin/blocks/base_static_block.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.035270 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/
+-rw-r--r--   0 richardblake   (502) staff       (20)       99 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/blocks/inline_form_block.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.038553 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/
+-rw-r--r--   0 richardblake   (502) staff       (20)      131 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_error.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_help_text.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      108 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/field_helpers/field_label.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.043426 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/
+-rw-r--r--   0 richardblake   (502) staff       (20)      773 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      563 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      832 2020-11-16 10:35:17.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      822 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      463 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/text_area_field.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.045820 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/
+-rw-r--r--   0 richardblake   (502) staff       (20)      555 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      335 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form_builder.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      179 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/no_script_notification.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.049937 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/
+-rw-r--r--   0 richardblake   (502) staff       (20)      594 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      442 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_complete.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_end.html
+-rw-r--r--   0 richardblake   (502) staff       (20)      113 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form_wrapper_start.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.050759 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/
+-rw-r--r--   0 richardblake   (502) staff       (20)     1164 2020-11-16 10:37:13.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.051653 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/
+-rw-r--r--   0 richardblake   (502) staff       (20)      234 2020-10-07 06:27:49.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/widgets/html_output_widget.html
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:19.053088 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templatetags/
+-rw-r--r--   0 richardblake   (502) staff       (20)        0 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templatetags/__init__.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      654 2020-10-07 06:27:44.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      367 2023-04-27 02:51:32.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/utils.py
+-rw-r--r--   0 richardblake   (502) staff       (20)      452 2023-04-28 02:13:52.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/wagtail_hooks.py
+drwxr-xr-x   0 richardblake   (502) staff       (20)        0 2023-04-28 02:41:18.979761 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/
+-rw-r--r--   0 richardblake   (502) staff       (20)     2766 2023-04-28 02:41:18.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/PKG-INFO
+-rw-r--r--   0 richardblake   (502) staff       (20)     6893 2023-04-28 02:41:18.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)        1 2023-04-28 02:41:18.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)        1 2020-11-16 09:23:33.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/not-zip-safe
+-rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:41:18.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/requires.txt
+-rw-r--r--   0 richardblake   (502) staff       (20)       41 2023-04-28 02:41:18.000000 wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/top_level.txt
```

### Comparing `wagtail-advanced-form-builder-1.0.1/PKG-INFO` & `wagtail-advanced-form-builder-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtail-advanced-form-builder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wagtail Advanced Form Builder
 Home-page: https://github.com/octavenz/wagtail-advanced-form-builder
 Author: Richard Blake (Octave)
 Author-email: richard.blake@octave.nz
 License: BSD
 Description: # Wagtail Advanced Form Builder
```

### Comparing `wagtail-advanced-form-builder-1.0.1/README.md` & `wagtail-advanced-form-builder-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/.DS_Store` & `wagtail-advanced-form-builder-1.0.2/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/contributing/contributing.md` & `wagtail-advanced-form-builder-1.0.2/docs/contributing/contributing.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/basic_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/basic_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/checkbox_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/checkbox_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/checkboxes_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/checkboxes_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/dropdown_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/dropdown_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/html_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/html_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/multi_line_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/multi_line_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/multi_select_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/multi_select_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/number_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/number_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/fields/radio_field.md` & `wagtail-advanced-form-builder-1.0.2/docs/fields/radio_field.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/getting_started/out_of_the_box.md` & `wagtail-advanced-form-builder-1.0.2/docs/getting_started/out_of_the_box.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/getting_started/using_your_own_page_models.md` & `wagtail-advanced-form-builder-1.0.2/docs/getting_started/using_your_own_page_models.md`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/.DS_Store` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/.DS_Store`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/custom-form-builder-page.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/custom-form-builder-page.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-basic-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-basic-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkbox-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-checkbox-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-checkboxes-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-checkboxes-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-dropdown-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-dropdown-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-hidden-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-hidden-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-html-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-html-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiline-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-multiline-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-multiselect-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-multiselect-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-number-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-number-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/fields/waf-radio-field.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/fields/waf-radio-field.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/docs/screenshots/waf-form-fields.png` & `wagtail-advanced-form-builder-1.0.2/docs/screenshots/waf-form-fields.png`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/setup.py` & `wagtail-advanced-form-builder-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/base_static_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/base_static_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/base_field_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/base_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/checkboxes_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/condition_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/condition_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/conditional_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/conditional_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/hidden_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/html_field_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/html_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/fields/multiselect_field_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/blocks/inline_form_block.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/blocks/inline_form_block.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/constants.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/constants.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/advanced_form_builder.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/advanced_form_builder.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/checkbox_input_widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/forms/widgets/html_output_widget.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0001_initial.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0002_auto_20201116_2241.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/migrations/0003_switch_streamfield_to_use_json_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_email_form.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/abstract_advanced_form_mixin.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/email_form_field.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/email_form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/models/form_field.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/models/form_field.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/css/style.css`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/admin.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -38,24 +38,24 @@
             return t.default
         } : function() {
             return t
         };
         return n.d(e, "a", e), e
     }, n.o = function(t, e) {
         return Object.prototype.hasOwnProperty.call(t, e)
-    }, n.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", n(n.s = 71)
+    }, n.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", n(n.s = 70)
 }([function(t, e, n) {
     (function(e) {
         var n = function(t) {
             return t && t.Math == Math && t
         };
         t.exports = n("object" == typeof globalThis && globalThis) || n("object" == typeof window && window) || n("object" == typeof self && self) || n("object" == typeof e && e) || function() {
             return this
         }() || Function("return this")()
-    }).call(this, n(42))
+    }).call(this, n(40))
 }, function(t, e) {
     t.exports = function(t) {
         try {
             return !!t()
         } catch (t) {
             return !0
         }
@@ -75,114 +75,114 @@
         })[1]
     }))
 }, function(t, e) {
     t.exports = function(t) {
         return "object" == typeof t ? null !== t : "function" == typeof t
     }
 }, function(t, e, n) {
+    var r = n(3),
+        i = n(9),
+        o = n(21);
+    t.exports = r ? function(t, e, n) {
+        return i.f(t, e, o(1, n))
+    } : function(t, e, n) {
+        return t[e] = n, t
+    }
+}, function(t, e, n) {
     var r = n(0),
         i = n(12).f,
-        o = n(6),
-        u = n(37),
+        o = n(5),
+        u = n(36),
         a = n(15),
-        c = n(46),
-        f = n(52);
+        c = n(44),
+        f = n(50);
     t.exports = function(t, e) {
-        var n, s, l, d, p, v = t.target,
+        var n, s, l, p, d, v = t.target,
             h = t.global,
-            g = t.stat;
-        if (n = h ? r : g ? r[v] || a(v, {}) : (r[v] || {}).prototype)
+            y = t.stat;
+        if (n = h ? r : y ? r[v] || a(v, {}) : (r[v] || {}).prototype)
             for (s in e) {
-                if (d = e[s], l = t.noTargetGet ? (p = i(n, s)) && p.value : n[s], !f(h ? s : v + (g ? "." : "#") + s, t.forced) && void 0 !== l) {
-                    if (typeof d == typeof l) continue;
-                    c(d, l)
-                }(t.sham || l && l.sham) && o(d, "sham", !0), u(n, s, d, t)
+                if (p = e[s], l = t.noTargetGet ? (d = i(n, s)) && d.value : n[s], !f(h ? s : v + (y ? "." : "#") + s, t.forced) && void 0 !== l) {
+                    if (typeof p == typeof l) continue;
+                    c(p, l)
+                }(t.sham || l && l.sham) && o(p, "sham", !0), u(n, s, p, t)
             }
     }
-}, function(t, e, n) {
-    var r = n(3),
-        i = n(8),
-        o = n(20);
-    t.exports = r ? function(t, e, n) {
-        return i.f(t, e, o(1, n))
-    } : function(t, e, n) {
-        return t[e] = n, t
-    }
 }, function(t, e) {
     t.exports = function(t) {
         if (null == t) throw TypeError("Can't call method on " + t);
         return t
     }
 }, function(t, e, n) {
+    var r = n(4);
+    t.exports = function(t) {
+        if (!r(t)) throw TypeError(String(t) + " is not an object");
+        return t
+    }
+}, function(t, e, n) {
     var r = n(3),
-        i = n(25),
-        o = n(9),
-        u = n(21),
+        i = n(24),
+        o = n(8),
+        u = n(23),
         a = Object.defineProperty;
     e.f = r ? a : function(t, e, n) {
         if (o(t), e = u(e, !0), o(n), i) try {
             return a(t, e, n)
         } catch (t) {}
         if ("get" in n || "set" in n) throw TypeError("Accessors not supported");
         return "value" in n && (t[e] = n.value), t
     }
 }, function(t, e, n) {
-    var r = n(4);
+    var r = n(18),
+        i = Math.min;
     t.exports = function(t) {
-        if (!r(t)) throw TypeError(String(t) + " is not an object");
-        return t
+        return t > 0 ? i(r(t), 9007199254740991) : 0
     }
 }, function(t, e, n) {
     var r = n(0),
-        i = n(29),
+        i = n(28),
         o = n(2),
-        u = n(31),
-        a = n(35),
-        c = n(53),
+        u = n(30),
+        a = n(34),
+        c = n(55),
         f = i("wks"),
         s = r.Symbol,
         l = c ? s : s && s.withoutSetter || u;
     t.exports = function(t) {
         return o(f, t) || (a && o(s, t) ? f[t] = s[t] : f[t] = l("Symbol." + t)), f[t]
     }
 }, function(t, e, n) {
-    var r = n(18),
-        i = Math.min;
-    t.exports = function(t) {
-        return t > 0 ? i(r(t), 9007199254740991) : 0
-    }
-}, function(t, e, n) {
     var r = n(3),
-        i = n(43),
-        o = n(20),
+        i = n(41),
+        o = n(21),
         u = n(13),
-        a = n(21),
+        a = n(23),
         c = n(2),
-        f = n(25),
+        f = n(24),
         s = Object.getOwnPropertyDescriptor;
     e.f = r ? s : function(t, e) {
         if (t = u(t), e = a(e, !0), f) try {
             return s(t, e)
         } catch (t) {}
         if (c(t, e)) return o(!i.f.call(t, e), t[e])
     }
 }, function(t, e, n) {
-    var r = n(24),
+    var r = n(22),
         i = n(7);
     t.exports = function(t) {
         return r(i(t))
     }
 }, function(t, e) {
     var n = {}.toString;
     t.exports = function(t) {
         return n.call(t).slice(8, -1)
     }
 }, function(t, e, n) {
     var r = n(0),
-        i = n(6);
+        i = n(5);
     t.exports = function(t, e) {
         try {
             i(r, t, e)
         } catch (n) {
             r[t] = e
         }
         return e
@@ -198,42 +198,14 @@
     var n = Math.ceil,
         r = Math.floor;
     t.exports = function(t) {
         return isNaN(t = +t) ? 0 : (t > 0 ? r : n)(t)
     }
 }, function(t, e) {
     t.exports = ["constructor", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "toLocaleString", "toString", "valueOf"]
-}, function(t, e) {
-    t.exports = function(t, e) {
-        return {
-            enumerable: !(1 & t),
-            configurable: !(2 & t),
-            writable: !(4 & t),
-            value: e
-        }
-    }
-}, function(t, e, n) {
-    var r = n(4);
-    t.exports = function(t, e) {
-        if (!r(t)) return t;
-        var n, i;
-        if (e && "function" == typeof(n = t.toString) && !r(i = n.call(t))) return i;
-        if ("function" == typeof(n = t.valueOf) && !r(i = n.call(t))) return i;
-        if (!e && "function" == typeof(n = t.toString) && !r(i = n.call(t))) return i;
-        throw TypeError("Can't convert object to primitive value")
-    }
-}, function(t, e, n) {
-    var r = n(48),
-        i = n(0),
-        o = function(t) {
-            return "function" == typeof t ? t : void 0
-        };
-    t.exports = function(t, e) {
-        return arguments.length < 2 ? o(r[t]) || o(i[t]) : r[t] && r[t][e] || i[t] && i[t][e]
-    }
 }, function(t, e, n) {
     var r = n(3),
         i = n(1),
         o = n(2),
         u = Object.defineProperty,
         a = {},
         c = function(t) {
@@ -253,27 +225,46 @@
             };
             f ? u(t, 1, {
                 enumerable: !0,
                 get: c
             }) : t[1] = 1, n.call(t, s, l)
         }))
     }
+}, function(t, e) {
+    t.exports = function(t, e) {
+        return {
+            enumerable: !(1 & t),
+            configurable: !(2 & t),
+            writable: !(4 & t),
+            value: e
+        }
+    }
 }, function(t, e, n) {
     var r = n(1),
         i = n(14),
         o = "".split;
     t.exports = r((function() {
         return !Object("z").propertyIsEnumerable(0)
     })) ? function(t) {
         return "String" == i(t) ? o.call(t, "") : Object(t)
     } : Object
 }, function(t, e, n) {
+    var r = n(4);
+    t.exports = function(t, e) {
+        if (!r(t)) return t;
+        var n, i;
+        if (e && "function" == typeof(n = t.toString) && !r(i = n.call(t))) return i;
+        if ("function" == typeof(n = t.valueOf) && !r(i = n.call(t))) return i;
+        if (!e && "function" == typeof(n = t.toString) && !r(i = n.call(t))) return i;
+        throw TypeError("Can't convert object to primitive value")
+    }
+}, function(t, e, n) {
     var r = n(3),
         i = n(1),
-        o = n(26);
+        o = n(25);
     t.exports = !r && !i((function() {
         return 7 != Object.defineProperty(o("div"), "a", {
             get: function() {
                 return 7
             }
         }).a
     }))
@@ -288,22 +279,22 @@
 }, function(t, e, n) {
     var r = n(16),
         i = Function.toString;
     "function" != typeof r.inspectSource && (r.inspectSource = function(t) {
         return i.call(t)
     }), t.exports = r.inspectSource
 }, function(t, e, n) {
-    var r = n(29),
-        i = n(31),
+    var r = n(28),
+        i = n(30),
         o = r("keys");
     t.exports = function(t) {
         return o[t] || (o[t] = i(t))
     }
 }, function(t, e, n) {
-    var r = n(30),
+    var r = n(29),
         i = n(16);
     (t.exports = function(t, e) {
         return i[t] || (i[t] = void 0 !== e ? e : {})
     })("versions", []).push({
         version: "3.8.1",
         mode: r ? "pure" : "global",
         copyright: "© 2020 Denis Pushkarev (zloirock.ru)"
@@ -313,30 +304,39 @@
 }, function(t, e) {
     var n = 0,
         r = Math.random();
     t.exports = function(t) {
         return "Symbol(" + String(void 0 === t ? "" : t) + ")_" + (++n + r).toString(36)
     }
 }, function(t, e, n) {
+    var r = n(46),
+        i = n(0),
+        o = function(t) {
+            return "function" == typeof t ? t : void 0
+        };
+    t.exports = function(t, e) {
+        return arguments.length < 2 ? o(r[t]) || o(i[t]) : r[t] && r[t][e] || i[t] && i[t][e]
+    }
+}, function(t, e, n) {
     var r = n(2),
         i = n(13),
         o = n(33).indexOf,
         u = n(17);
     t.exports = function(t, e) {
         var n, a = i(t),
             c = 0,
             f = [];
         for (n in a) !r(u, n) && r(a, n) && f.push(n);
         for (; e.length > c;) r(a, n = e[c++]) && (~o(f, n) || f.push(n));
         return f
     }
 }, function(t, e, n) {
     var r = n(13),
-        i = n(11),
-        o = n(50),
+        i = n(10),
+        o = n(48),
         u = function(t) {
             return function(e, n, u) {
                 var a, c = r(e),
                     f = i(c.length),
                     s = o(u, f);
                 if (t && n != n) {
                     for (; f > s;)
@@ -348,112 +348,99 @@
             }
         };
     t.exports = {
         includes: u(!0),
         indexOf: u(!1)
     }
 }, function(t, e, n) {
-    var r = n(7);
-    t.exports = function(t) {
-        return Object(r(t))
-    }
-}, function(t, e, n) {
     var r = n(1);
     t.exports = !!Object.getOwnPropertySymbols && !r((function() {
         return !String(Symbol())
     }))
 }, function(t, e, n) {
     "use strict";
-    var r = n(40).forEach,
-        i = n(41),
-        o = n(23),
+    var r = n(37).forEach,
+        i = n(39),
+        o = n(20),
         u = i("forEach"),
         a = o("forEach");
     t.exports = u && a ? [].forEach : function(t) {
         return r(this, t, arguments.length > 1 ? arguments[1] : void 0)
     }
 }, function(t, e, n) {
     var r = n(0),
-        i = n(6),
+        i = n(5),
         o = n(2),
         u = n(15),
-        a = n(27),
-        c = n(44),
+        a = n(26),
+        c = n(42),
         f = c.get,
         s = c.enforce,
         l = String(String).split("String");
     (t.exports = function(t, e, n, a) {
         var c, f = !!a && !!a.unsafe,
-            d = !!a && !!a.enumerable,
-            p = !!a && !!a.noTargetGet;
-        "function" == typeof n && ("string" != typeof e || o(n, "name") || i(n, "name", e), (c = s(n)).source || (c.source = l.join("string" == typeof e ? e : ""))), t !== r ? (f ? !p && t[e] && (d = !0) : delete t[e], d ? t[e] = n : i(t, e, n)) : d ? t[e] = n : u(e, n)
+            p = !!a && !!a.enumerable,
+            d = !!a && !!a.noTargetGet;
+        "function" == typeof n && ("string" != typeof e || o(n, "name") || i(n, "name", e), (c = s(n)).source || (c.source = l.join("string" == typeof e ? e : ""))), t !== r ? (f ? !d && t[e] && (p = !0) : delete t[e], p ? t[e] = n : i(t, e, n)) : p ? t[e] = n : u(e, n)
     })(Function.prototype, "toString", (function() {
         return "function" == typeof this && f(this).source || a(this)
     }))
 }, function(t, e, n) {
-    var r = n(14);
-    t.exports = Array.isArray || function(t) {
-        return "Array" == r(t)
-    }
-}, function(t, e, n) {
-    var r = n(4),
-        i = n(38),
-        o = n(10)("species");
-    t.exports = function(t, e) {
-        var n;
-        return i(t) && ("function" != typeof(n = t.constructor) || n !== Array && !i(n.prototype) ? r(n) && null === (n = n[o]) && (n = void 0) : n = void 0), new(void 0 === n ? Array : n)(0 === e ? 0 : e)
-    }
-}, function(t, e, n) {
-    var r = n(54),
-        i = n(24),
-        o = n(34),
-        u = n(11),
-        a = n(39),
+    var r = n(51),
+        i = n(22),
+        o = n(38),
+        u = n(10),
+        a = n(53),
         c = [].push,
         f = function(t) {
             var e = 1 == t,
                 n = 2 == t,
                 f = 3 == t,
                 s = 4 == t,
                 l = 6 == t,
-                d = 7 == t,
-                p = 5 == t || l;
-            return function(v, h, g, y) {
-                for (var m, x, b = o(v), w = i(b), S = r(h, g, 3), O = u(w.length), C = 0, E = y || a, T = e ? E(v, O) : n || d ? E(v, 0) : void 0; O > C; C++)
-                    if ((p || C in w) && (x = S(m = w[C], C, b), t))
-                        if (e) T[C] = x;
-                        else if (x) switch (t) {
+                p = 7 == t,
+                d = 5 == t || l;
+            return function(v, h, y, m) {
+                for (var g, b, x = o(v), w = i(x), O = r(h, y, 3), S = u(w.length), L = 0, j = m || a, E = e ? j(v, S) : n || p ? j(v, 0) : void 0; S > L; L++)
+                    if ((d || L in w) && (b = O(g = w[L], L, x), t))
+                        if (e) E[L] = b;
+                        else if (b) switch (t) {
                     case 3:
                         return !0;
                     case 5:
-                        return m;
+                        return g;
                     case 6:
-                        return C;
+                        return L;
                     case 2:
-                        c.call(T, m)
+                        c.call(E, g)
                 } else switch (t) {
                     case 4:
                         return !1;
                     case 7:
-                        c.call(T, m)
+                        c.call(E, g)
                 }
-                return l ? -1 : f || s ? s : T
+                return l ? -1 : f || s ? s : E
             }
         };
     t.exports = {
         forEach: f(0),
         map: f(1),
         filter: f(2),
         some: f(3),
         every: f(4),
         find: f(5),
         findIndex: f(6),
         filterOut: f(7)
     }
 }, function(t, e, n) {
+    var r = n(7);
+    t.exports = function(t) {
+        return Object(r(t))
+    }
+}, function(t, e, n) {
     "use strict";
     var r = n(1);
     t.exports = function(t, e) {
         var n = [][t];
         return !!n && r((function() {
             n.call(null, e || function() {
                 throw 1
@@ -479,43 +466,43 @@
             1: 2
         }, 1);
     e.f = o ? function(t) {
         var e = i(this, t);
         return !!e && e.enumerable
     } : r
 }, function(t, e, n) {
-    var r, i, o, u = n(45),
+    var r, i, o, u = n(43),
         a = n(0),
         c = n(4),
-        f = n(6),
+        f = n(5),
         s = n(2),
         l = n(16),
-        d = n(28),
-        p = n(17),
+        p = n(27),
+        d = n(17),
         v = a.WeakMap;
     if (u) {
         var h = l.state || (l.state = new v),
-            g = h.get,
-            y = h.has,
-            m = h.set;
+            y = h.get,
+            m = h.has,
+            g = h.set;
         r = function(t, e) {
-            return e.facade = t, m.call(h, t, e), e
+            return e.facade = t, g.call(h, t, e), e
         }, i = function(t) {
-            return g.call(h, t) || {}
+            return y.call(h, t) || {}
         }, o = function(t) {
-            return y.call(h, t)
+            return m.call(h, t)
         }
     } else {
-        var x = d("state");
-        p[x] = !0, r = function(t, e) {
-            return e.facade = t, f(t, x, e), e
+        var b = p("state");
+        d[b] = !0, r = function(t, e) {
+            return e.facade = t, f(t, b, e), e
         }, i = function(t) {
-            return s(t, x) ? t[x] : {}
+            return s(t, b) ? t[b] : {}
         }, o = function(t) {
-            return s(t, x)
+            return s(t, b)
         }
     }
     t.exports = {
         set: r,
         get: i,
         has: o,
         enforce: function(t) {
@@ -527,33 +514,33 @@
                 if (!c(e) || (n = i(e)).type !== t) throw TypeError("Incompatible receiver, " + t + " required");
                 return n
             }
         }
     }
 }, function(t, e, n) {
     var r = n(0),
-        i = n(27),
+        i = n(26),
         o = r.WeakMap;
     t.exports = "function" == typeof o && /native code/.test(i(o))
 }, function(t, e, n) {
     var r = n(2),
-        i = n(47),
+        i = n(45),
         o = n(12),
-        u = n(8);
+        u = n(9);
     t.exports = function(t, e) {
         for (var n = i(e), a = u.f, c = o.f, f = 0; f < n.length; f++) {
             var s = n[f];
             r(t, s) || a(t, s, c(e, s))
         }
     }
 }, function(t, e, n) {
-    var r = n(22),
-        i = n(49),
-        o = n(51),
-        u = n(9);
+    var r = n(31),
+        i = n(47),
+        o = n(49),
+        u = n(8);
     t.exports = r("Reflect", "ownKeys") || function(t) {
         var e = i.f(u(t)),
             n = o.f;
         return n ? e.concat(n(t)) : e
     }
 }, function(t, e, n) {
     var r = n(0);
@@ -585,18 +572,15 @@
             return String(t).replace(i, ".").toLowerCase()
         },
         a = o.data = {},
         c = o.NATIVE = "N",
         f = o.POLYFILL = "P";
     t.exports = o
 }, function(t, e, n) {
-    var r = n(35);
-    t.exports = r && !Symbol.sham && "symbol" == typeof Symbol.iterator
-}, function(t, e, n) {
-    var r = n(55);
+    var r = n(52);
     t.exports = function(t, e, n) {
         if (r(t), void 0 === e) return t;
         switch (n) {
             case 0:
                 return function() {
                     return t.call(e)
                 };
@@ -619,90 +603,106 @@
     }
 }, function(t, e) {
     t.exports = function(t) {
         if ("function" != typeof t) throw TypeError(String(t) + " is not a function");
         return t
     }
 }, function(t, e, n) {
-    var r = n(10),
+    var r = n(4),
+        i = n(54),
+        o = n(11)("species");
+    t.exports = function(t, e) {
+        var n;
+        return i(t) && ("function" != typeof(n = t.constructor) || n !== Array && !i(n.prototype) ? r(n) && null === (n = n[o]) && (n = void 0) : n = void 0), new(void 0 === n ? Array : n)(0 === e ? 0 : e)
+    }
+}, function(t, e, n) {
+    var r = n(14);
+    t.exports = Array.isArray || function(t) {
+        return "Array" == r(t)
+    }
+}, function(t, e, n) {
+    var r = n(34);
+    t.exports = r && !Symbol.sham && "symbol" == typeof Symbol.iterator
+}, function(t, e, n) {
+    var r = n(11),
         i = n(57),
-        o = n(8),
+        o = n(9),
         u = r("unscopables"),
         a = Array.prototype;
     null == a[u] && o.f(a, u, {
         configurable: !0,
         value: i(null)
     }), t.exports = function(t) {
         a[u][t] = !0
     }
 }, function(t, e, n) {
-    var r, i = n(9),
+    var r, i = n(8),
         o = n(58),
         u = n(19),
         a = n(17),
         c = n(60),
-        f = n(26),
-        s = n(28),
+        f = n(25),
+        s = n(27),
         l = s("IE_PROTO"),
-        d = function() {},
-        p = function(t) {
+        p = function() {},
+        d = function(t) {
             return "<script>" + t + "<\/script>"
         },
         v = function() {
             try {
                 r = document.domain && new ActiveXObject("htmlfile")
             } catch (t) {}
             var t, e;
             v = r ? function(t) {
-                t.write(p("")), t.close();
+                t.write(d("")), t.close();
                 var e = t.parentWindow.Object;
                 return t = null, e
-            }(r) : ((e = f("iframe")).style.display = "none", c.appendChild(e), e.src = String("javascript:"), (t = e.contentWindow.document).open(), t.write(p("document.F=Object")), t.close(), t.F);
+            }(r) : ((e = f("iframe")).style.display = "none", c.appendChild(e), e.src = String("javascript:"), (t = e.contentWindow.document).open(), t.write(d("document.F=Object")), t.close(), t.F);
             for (var n = u.length; n--;) delete v.prototype[u[n]];
             return v()
         };
     a[l] = !0, t.exports = Object.create || function(t, e) {
         var n;
-        return null !== t ? (d.prototype = i(t), n = new d, d.prototype = null, n[l] = t) : n = v(), void 0 === e ? n : o(n, e)
+        return null !== t ? (p.prototype = i(t), n = new p, p.prototype = null, n[l] = t) : n = v(), void 0 === e ? n : o(n, e)
     }
 }, function(t, e, n) {
     var r = n(3),
-        i = n(8),
-        o = n(9),
+        i = n(9),
+        o = n(8),
         u = n(59);
     t.exports = r ? Object.defineProperties : function(t, e) {
         o(t);
         for (var n, r = u(e), a = r.length, c = 0; a > c;) i.f(t, n = r[c++], e[n]);
         return t
     }
 }, function(t, e, n) {
     var r = n(32),
         i = n(19);
     t.exports = Object.keys || function(t) {
         return r(t, i)
     }
 }, function(t, e, n) {
-    var r = n(22);
+    var r = n(31);
     t.exports = r("document", "documentElement")
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
-        i = n(36);
+    var r = n(6),
+        i = n(35);
     r({
         target: "Array",
         proto: !0,
         forced: [].forEach != i
     }, {
         forEach: i
     })
 }, function(t, e, n) {
     var r = n(0),
         i = n(63),
-        o = n(36),
-        u = n(6);
+        o = n(35),
+        u = n(5);
     for (var a in i) {
         var c = r[a],
             f = c && c.prototype;
         if (f && f.forEach !== o) try {
             u(f, "forEach", o)
         } catch (t) {
             f.forEach = o
@@ -738,25 +738,18 @@
         SVGTransformList: 0,
         SourceBufferList: 0,
         StyleSheetList: 0,
         TextTrackCueList: 0,
         TextTrackList: 0,
         TouchList: 0
     }
-}, , , , function(t, e, n) {
-    var r, i, o = n(0),
-        u = n(75),
-        a = o.process,
-        c = a && a.versions,
-        f = c && c.v8;
-    f ? i = (r = f.split("."))[0] + r[1] : u && (!(r = u.match(/Edge\/(\d+)/)) || r[1] >= 74) && (r = u.match(/Chrome\/(\d+)/)) && (i = r[1]), t.exports = i && +i
-}, , , , function(t, e, n) {
+}, , , , , , , function(t, e, n) {
     "use strict";
     n.r(e);
-    n(72), n(76), n(61), n(77), n(78), n(62);
+    n(71), n(61), n(72), n(73), n(62);
 
     function r(t, e) {
         if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
     }
 
     function i(t, e) {
         for (var n = 0; n < e.length; n++) {
@@ -766,252 +759,128 @@
     }
 
     function o(t, e, n) {
         return e && i(t.prototype, e), n && i(t, n), t
     }
     var u = function() {
             function t() {
-                r(this, t), this.registeredFieldNames = [], this.fields = $(".waf--field"), this.formRulesContainers = $(".waf--form-rules"), this.uniqueFieldCounter = 0
+                r(this, t), this.registeredFieldNames = [], this.fields = $(".waf--field")
             }
             return o(t, [{
                 key: "swapRulesInputsForSelectDropdowns",
                 value: function() {
                     var t = this;
                     this.registeredFieldNames.length && $(".waf--form-rules .waf--rule-condition").each((function(e, n) {
                         var r = $(n),
                             i = [],
                             o = r.parents(".waf--field").find('input[type="text"]').first().val(),
-                            u = r.parents("#form-list").first().find(".waf--html-field"),
+                            u = $(".waf--html-field"),
                             a = [];
                         u.each((function(t, e) {
                             a.push($(e).find('input[type="text"]').first().val())
                         }));
                         for (var c = 0; c < t.registeredFieldNames.length; c++)
                             if (t.registeredFieldNames[c] !== o && -1 === a.indexOf(t.registeredFieldNames[c])) {
                                 var f = document.createElement("option");
                                 f.value = t.registeredFieldNames[c], f.text = t.registeredFieldNames[c], i.push(f)
                             } var s = r.find('input[type="text"][name$="field_name"]').first();
                         if (s.length) {
                             s.parent().parent().addClass("choice_field widget-select");
                             var l = s.val(),
-                                d = document.createElement("select");
-                            d.id = s.attr("id"), d.name = s.attr("name");
-                            for (var p = 0; p < i.length; p++) d.appendChild(i[p]);
-                            s.replaceWith(d), $(d).val(l)
+                                p = document.createElement("select");
+                            p.id = s.attr("id"), p.name = s.attr("name");
+                            for (var d = 0; d < i.length; d++) p.appendChild(i[d]);
+                            s.replaceWith(p), $(p).val(l)
                         } else {
                             var v = r.find("select").first(),
                                 h = v.val();
                             v.empty();
-                            for (var g = 0; g < i.length; g++) v[0].appendChild(i[g]);
+                            for (var y = 0; y < i.length; y++) v[0].appendChild(i[y]);
                             v.val(h)
                         }
                     }))
                 }
             }, {
                 key: "toggleRulesContainers",
                 value: function() {
-                    this.formRulesContainers = $(".waf--form-rules"), this.registeredFieldNames.length > 1 ? (this.formRulesContainers.show(), this.formRulesContainers.siblings("label").show(), this.swapRulesInputsForSelectDropdowns()) : (this.formRulesContainers.hide(), this.formRulesContainers.siblings("label").hide())
+                    this.formRulesContainers = $(".waf--form-rules"), this.registeredFieldNames.length > 1 && this.swapRulesInputsForSelectDropdowns()
                 }
             }, {
                 key: "registerFieldNames",
                 value: function() {
                     var t = this;
                     this.registeredFieldNames = [], this.fields = $(".waf--field"), this.fields.each((function(e, n) {
-                        var r, i, o, u, a = $(n),
-                            c = a.parents('div[id^="form-"][id$="-container"]').first();
-                        if (c.length || (c = a.parents('div[id^="field-list"]').first()), "1" !== c.find('input[type="hidden"][id$="-deleted"]').first().attr("value")) {
-                            var f = a.find('input[type="text"]').first(),
-                                s = f.val();
-                            void 0 !== s && "" !== s && t.registeredFieldNames.push(s), f.unbind("keyup change"), f.on("keyup change", (r = function() {
+                        var r, i, o, u, a = $(n);
+                        if ("1" !== a.parents("section").first().parent("div").find('input[type="hidden"][id$="-deleted"]').first().attr("value")) {
+                            var c = a.find('input[type="text"]').first(),
+                                f = c.val();
+                            void 0 !== f && "" !== f && t.registeredFieldNames.push(f), c.unbind("keyup change"), c.on("keyup change", (r = function() {
                                 t.registerFieldNames()
                             }, i = 500, function() {
                                 var t = this,
                                     e = arguments,
                                     n = function() {
                                         u = null, o || r.apply(t, e)
                                     },
                                     a = o && !u;
                                 clearTimeout(u), u = setTimeout(n, i), a && r.apply(t, e)
                             }))
                         }
                     })), this.toggleRulesContainers()
                 }
-            }, {
-                key: "initField",
-                value: function(t) {
-                    var e = t.parents(".c-sf-container__block-container").first(),
-                        n = t.find("> .field"),
-                        r = e.find(".c-sf-block__header");
-                    if (!e.find("[data-expand-trigger]").length) {
-                        t.attr("id", "field-list-".concat(this.uniqueFieldCounter));
-                        var i = !1;
-                        n.each((function(t, e) {
-                            if (t > 0) {
-                                var n = $(e);
-                                n.find("div.error").length || (n.hide(), i = !0)
-                            }
-                        })), $('<a href="#" data-expand-trigger="field-list-'.concat(this.uniqueFieldCounter, '">').concat(i ? "Configure field" : "Collapse field", "</a>")).insertBefore(r.find("h3").first()), this.uniqueFieldCounter += 1
-                    }
-                }
-            }, {
-                key: "initFieldDisplay",
-                value: function() {
-                    var t = this;
-                    this.fields.each((function(e, n) {
-                        t.initField($(n))
-                    }))
-                }
-            }, {
-                key: "initExpandTrigger",
-                value: function(t) {
-                    var e = t.attr("data-expand-trigger"),
-                        n = $("#".concat(e)).find("> .field");
-                    "Collapse field" === t.html() ? (n.each((function(t) {
-                        t > 0 && $(this).hide()
-                    })), t.html("Configure field")) : (n.each((function() {
-                        $(this).show()
-                    })), t.html("Collapse field"))
-                }
-            }, {
-                key: "initExpandTriggers",
-                value: function() {
-                    var t = this;
-                    this.expandTriggers = $("[data-expand-trigger]"), this.expandTriggers.on("click", (function(e) {
-                        e.preventDefault(), t.initExpandTrigger($(e.currentTarget))
-                    }))
-                }
             }]), t
         }(),
         a = function() {
             function t() {
                 r(this, t), this.mutationObserverConfig = {
                     attributes: !0,
                     childList: !0,
                     characterData: !0,
                     subTree: !0
-                }, this.streamfieldList = $("#form-list")[0], this.formRulesLists = $("[id$=-rules-conditions-list]")
+                }, this.streamfieldList = $(".waf--field").first().parents("[data-streamfield-stream-container]"), this.streamfieldList.length || (this.streamfieldList = $("[data-streamfield-stream-container]")), this.formRulesLists = $('[data-contentpath="conditions"]').find("[data-streamfield-stream-container]")
             }
             return o(t, [{
                 key: "monitorMutations",
                 value: function() {
                     var t = this;
                     this.newFieldMutationObserver = new MutationObserver((function(e) {
                         e.forEach((function(e) {
                             var n = e.addedNodes;
-                            if (null !== n) {
-                                t.fieldRegistry.registerFieldNames();
-                                var r = $(n);
-                                r.each((function(e, n) {
-                                    var i = $(n);
-                                    t.fieldRegistry.initField(i);
-                                    var o = r.find("[data-expand-trigger]");
-                                    o.unbind("click"), o.on("click", (function(e) {
-                                        e.preventDefault(), t.fieldRegistry.initExpandTrigger($(e.currentTarget))
-                                    }))
-                                })), r.find("[id$=-rules-conditions-list]").each((function(e, n) {
-                                    t.newRuleMutationObserver.observe(n, t.mutationObserverConfig)
-                                }))
-                            }
+                            null !== n && (t.fieldRegistry.registerFieldNames(), $(n).find('[data-contentpath="conditions"]').find("[data-streamfield-stream-container]").each((function(e, n) {
+                                t.newRuleMutationObserver.observe(n, t.mutationObserverConfig)
+                            })))
                         }))
-                    })), this.newFieldMutationObserver.observe(this.streamfieldList, this.mutationObserverConfig), this.newRuleMutationObserver = new MutationObserver((function(e) {
+                    })), this.streamfieldList.each((function(e, n) {
+                        t.newFieldMutationObserver.observe(n, t.mutationObserverConfig)
+                    })), this.newRuleMutationObserver = new MutationObserver((function(e) {
                         e.forEach((function(e) {
                             null !== e.addedNodes && t.fieldRegistry.registerFieldNames()
                         }))
                     })), this.formRulesLists.each((function(e, n) {
                         t.newRuleMutationObserver.observe(n, t.mutationObserverConfig)
-                    })), $(this.streamfieldList).find('[id^="form-"][id$="-delete"]').on("click", (function(e) {
+                    })), $(this.streamfieldList).find('.button[title="Delete"]').on("click", (function(e) {
                         t.fieldRegistry.registerFieldNames()
                     }))
                 }
             }, {
                 key: "init",
                 value: function() {
-                    this.fieldRegistry = new u, this.fieldRegistry.registerFieldNames(), this.fieldRegistry.initFieldDisplay(), this.fieldRegistry.initExpandTriggers(), this.monitorMutations()
+                    this.fieldRegistry = new u, this.fieldRegistry.registerFieldNames(), this.monitorMutations()
                 }
             }]), t
         }();
     $(document).ready((function() {
         (new a).init()
     }))
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
-        i = n(1),
-        o = n(38),
-        u = n(4),
-        a = n(34),
-        c = n(11),
-        f = n(73),
-        s = n(39),
-        l = n(74),
-        d = n(10),
-        p = n(67),
-        v = d("isConcatSpreadable"),
-        h = p >= 51 || !i((function() {
-            var t = [];
-            return t[v] = !1, t.concat()[0] !== t
-        })),
-        g = l("concat"),
-        y = function(t) {
-            if (!u(t)) return !1;
-            var e = t[v];
-            return void 0 !== e ? !!e : o(t)
-        };
-    r({
-        target: "Array",
-        proto: !0,
-        forced: !h || !g
-    }, {
-        concat: function(t) {
-            var e, n, r, i, o, u = a(this),
-                l = s(u, 0),
-                d = 0;
-            for (e = -1, r = arguments.length; e < r; e++)
-                if (y(o = -1 === e ? u : arguments[e])) {
-                    if (d + (i = c(o.length)) > 9007199254740991) throw TypeError("Maximum allowed index exceeded");
-                    for (n = 0; n < i; n++, d++) n in o && f(l, d, o[n])
-                } else {
-                    if (d >= 9007199254740991) throw TypeError("Maximum allowed index exceeded");
-                    f(l, d++, o)
-                } return l.length = d, l
-        }
-    })
-}, function(t, e, n) {
-    "use strict";
-    var r = n(21),
-        i = n(8),
-        o = n(20);
-    t.exports = function(t, e, n) {
-        var u = r(e);
-        u in t ? i.f(t, u, o(0, n)) : t[u] = n
-    }
-}, function(t, e, n) {
-    var r = n(1),
-        i = n(10),
-        o = n(67),
-        u = i("species");
-    t.exports = function(t) {
-        return o >= 51 || !r((function() {
-            var e = [];
-            return (e.constructor = {})[u] = function() {
-                return {
-                    foo: 1
-                }
-            }, 1 !== e[t](Boolean).foo
-        }))
-    }
-}, function(t, e, n) {
-    var r = n(22);
-    t.exports = r("navigator", "userAgent") || ""
-}, function(t, e, n) {
-    "use strict";
-    var r = n(5),
-        i = n(40).find,
+    var r = n(6),
+        i = n(37).find,
         o = n(56),
-        u = n(23),
+        u = n(20),
         a = !0,
         c = u("find");
     "find" in [] && Array(1).find((function() {
         a = !1
     })), r({
         target: "Array",
         proto: !0,
@@ -1019,18 +888,18 @@
     }, {
         find: function(t) {
             return i(this, t, arguments.length > 1 ? arguments[1] : void 0)
         }
     }), o("find")
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
+    var r = n(6),
         i = n(33).indexOf,
-        o = n(41),
-        u = n(23),
+        o = n(39),
+        u = n(20),
         a = [].indexOf,
         c = !!a && 1 / [1].indexOf(1, -0) < 0,
         f = o("indexOf"),
         s = u("indexOf", {
             ACCESSORS: !0,
             1: 0
         });
@@ -1041,15 +910,15 @@
     }, {
         indexOf: function(t) {
             return c ? a.apply(this, arguments) || 0 : i(this, t, arguments.length > 1 ? arguments[1] : void 0)
         }
     })
 }, function(t, e, n) {
     var r = n(3),
-        i = n(8).f,
+        i = n(9).f,
         o = Function.prototype,
         u = o.toString,
         a = /^\s*function ([^ (]*)/;
     r && !("name" in o) && i(o, "name", {
         configurable: !0,
         get: function() {
             try {
```

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/formbuilder.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -38,24 +38,24 @@
             return t.default
         } : function() {
             return t
         };
         return n.d(e, "a", e), e
     }, n.o = function(t, e) {
         return Object.prototype.hasOwnProperty.call(t, e)
-    }, n.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", n(n.s = 79)
+    }, n.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", n(n.s = 74)
 }([function(t, e, n) {
     (function(e) {
         var n = function(t) {
             return t && t.Math == Math && t
         };
         t.exports = n("object" == typeof globalThis && globalThis) || n("object" == typeof window && window) || n("object" == typeof self && self) || n("object" == typeof e && e) || function() {
             return this
         }() || Function("return this")()
-    }).call(this, n(42))
+    }).call(this, n(40))
 }, function(t, e) {
     t.exports = function(t) {
         try {
             return !!t()
         } catch (t) {
             return !0
         }
@@ -75,114 +75,114 @@
         })[1]
     }))
 }, function(t, e) {
     t.exports = function(t) {
         return "object" == typeof t ? null !== t : "function" == typeof t
     }
 }, function(t, e, n) {
+    var r = n(3),
+        o = n(9),
+        i = n(21);
+    t.exports = r ? function(t, e, n) {
+        return o.f(t, e, i(1, n))
+    } : function(t, e, n) {
+        return t[e] = n, t
+    }
+}, function(t, e, n) {
     var r = n(0),
         o = n(12).f,
-        i = n(6),
-        u = n(37),
+        i = n(5),
+        u = n(36),
         c = n(15),
-        a = n(46),
-        f = n(52);
+        a = n(44),
+        f = n(50);
     t.exports = function(t, e) {
         var n, l, s, p, v, d = t.target,
             h = t.global,
             g = t.stat;
         if (n = h ? r : g ? r[d] || c(d, {}) : (r[d] || {}).prototype)
             for (l in e) {
                 if (p = e[l], s = t.noTargetGet ? (v = o(n, l)) && v.value : n[l], !f(h ? l : d + (g ? "." : "#") + l, t.forced) && void 0 !== s) {
                     if (typeof p == typeof s) continue;
                     a(p, s)
                 }(t.sham || s && s.sham) && i(p, "sham", !0), u(n, l, p, t)
             }
     }
-}, function(t, e, n) {
-    var r = n(3),
-        o = n(8),
-        i = n(20);
-    t.exports = r ? function(t, e, n) {
-        return o.f(t, e, i(1, n))
-    } : function(t, e, n) {
-        return t[e] = n, t
-    }
 }, function(t, e) {
     t.exports = function(t) {
         if (null == t) throw TypeError("Can't call method on " + t);
         return t
     }
 }, function(t, e, n) {
+    var r = n(4);
+    t.exports = function(t) {
+        if (!r(t)) throw TypeError(String(t) + " is not an object");
+        return t
+    }
+}, function(t, e, n) {
     var r = n(3),
-        o = n(25),
-        i = n(9),
-        u = n(21),
+        o = n(24),
+        i = n(8),
+        u = n(23),
         c = Object.defineProperty;
     e.f = r ? c : function(t, e, n) {
         if (i(t), e = u(e, !0), i(n), o) try {
             return c(t, e, n)
         } catch (t) {}
         if ("get" in n || "set" in n) throw TypeError("Accessors not supported");
         return "value" in n && (t[e] = n.value), t
     }
 }, function(t, e, n) {
-    var r = n(4);
+    var r = n(18),
+        o = Math.min;
     t.exports = function(t) {
-        if (!r(t)) throw TypeError(String(t) + " is not an object");
-        return t
+        return t > 0 ? o(r(t), 9007199254740991) : 0
     }
 }, function(t, e, n) {
     var r = n(0),
-        o = n(29),
+        o = n(28),
         i = n(2),
-        u = n(31),
-        c = n(35),
-        a = n(53),
+        u = n(30),
+        c = n(34),
+        a = n(55),
         f = o("wks"),
         l = r.Symbol,
         s = a ? l : l && l.withoutSetter || u;
     t.exports = function(t) {
         return i(f, t) || (c && i(l, t) ? f[t] = l[t] : f[t] = s("Symbol." + t)), f[t]
     }
 }, function(t, e, n) {
-    var r = n(18),
-        o = Math.min;
-    t.exports = function(t) {
-        return t > 0 ? o(r(t), 9007199254740991) : 0
-    }
-}, function(t, e, n) {
     var r = n(3),
-        o = n(43),
-        i = n(20),
+        o = n(41),
+        i = n(21),
         u = n(13),
-        c = n(21),
+        c = n(23),
         a = n(2),
-        f = n(25),
+        f = n(24),
         l = Object.getOwnPropertyDescriptor;
     e.f = r ? l : function(t, e) {
         if (t = u(t), e = c(e, !0), f) try {
             return l(t, e)
         } catch (t) {}
         if (a(t, e)) return i(!o.f.call(t, e), t[e])
     }
 }, function(t, e, n) {
-    var r = n(24),
+    var r = n(22),
         o = n(7);
     t.exports = function(t) {
         return r(o(t))
     }
 }, function(t, e) {
     var n = {}.toString;
     t.exports = function(t) {
         return n.call(t).slice(8, -1)
     }
 }, function(t, e, n) {
     var r = n(0),
-        o = n(6);
+        o = n(5);
     t.exports = function(t, e) {
         try {
             o(r, t, e)
         } catch (n) {
             r[t] = e
         }
         return e
@@ -198,42 +198,14 @@
     var n = Math.ceil,
         r = Math.floor;
     t.exports = function(t) {
         return isNaN(t = +t) ? 0 : (t > 0 ? r : n)(t)
     }
 }, function(t, e) {
     t.exports = ["constructor", "hasOwnProperty", "isPrototypeOf", "propertyIsEnumerable", "toLocaleString", "toString", "valueOf"]
-}, function(t, e) {
-    t.exports = function(t, e) {
-        return {
-            enumerable: !(1 & t),
-            configurable: !(2 & t),
-            writable: !(4 & t),
-            value: e
-        }
-    }
-}, function(t, e, n) {
-    var r = n(4);
-    t.exports = function(t, e) {
-        if (!r(t)) return t;
-        var n, o;
-        if (e && "function" == typeof(n = t.toString) && !r(o = n.call(t))) return o;
-        if ("function" == typeof(n = t.valueOf) && !r(o = n.call(t))) return o;
-        if (!e && "function" == typeof(n = t.toString) && !r(o = n.call(t))) return o;
-        throw TypeError("Can't convert object to primitive value")
-    }
-}, function(t, e, n) {
-    var r = n(48),
-        o = n(0),
-        i = function(t) {
-            return "function" == typeof t ? t : void 0
-        };
-    t.exports = function(t, e) {
-        return arguments.length < 2 ? i(r[t]) || i(o[t]) : r[t] && r[t][e] || o[t] && o[t][e]
-    }
 }, function(t, e, n) {
     var r = n(3),
         o = n(1),
         i = n(2),
         u = Object.defineProperty,
         c = {},
         a = function(t) {
@@ -253,27 +225,46 @@
             };
             f ? u(t, 1, {
                 enumerable: !0,
                 get: a
             }) : t[1] = 1, n.call(t, l, s)
         }))
     }
+}, function(t, e) {
+    t.exports = function(t, e) {
+        return {
+            enumerable: !(1 & t),
+            configurable: !(2 & t),
+            writable: !(4 & t),
+            value: e
+        }
+    }
 }, function(t, e, n) {
     var r = n(1),
         o = n(14),
         i = "".split;
     t.exports = r((function() {
         return !Object("z").propertyIsEnumerable(0)
     })) ? function(t) {
         return "String" == o(t) ? i.call(t, "") : Object(t)
     } : Object
 }, function(t, e, n) {
+    var r = n(4);
+    t.exports = function(t, e) {
+        if (!r(t)) return t;
+        var n, o;
+        if (e && "function" == typeof(n = t.toString) && !r(o = n.call(t))) return o;
+        if ("function" == typeof(n = t.valueOf) && !r(o = n.call(t))) return o;
+        if (!e && "function" == typeof(n = t.toString) && !r(o = n.call(t))) return o;
+        throw TypeError("Can't convert object to primitive value")
+    }
+}, function(t, e, n) {
     var r = n(3),
         o = n(1),
-        i = n(26);
+        i = n(25);
     t.exports = !r && !o((function() {
         return 7 != Object.defineProperty(i("div"), "a", {
             get: function() {
                 return 7
             }
         }).a
     }))
@@ -288,22 +279,22 @@
 }, function(t, e, n) {
     var r = n(16),
         o = Function.toString;
     "function" != typeof r.inspectSource && (r.inspectSource = function(t) {
         return o.call(t)
     }), t.exports = r.inspectSource
 }, function(t, e, n) {
-    var r = n(29),
-        o = n(31),
+    var r = n(28),
+        o = n(30),
         i = r("keys");
     t.exports = function(t) {
         return i[t] || (i[t] = o(t))
     }
 }, function(t, e, n) {
-    var r = n(30),
+    var r = n(29),
         o = n(16);
     (t.exports = function(t, e) {
         return o[t] || (o[t] = void 0 !== e ? e : {})
     })("versions", []).push({
         version: "3.8.1",
         mode: r ? "pure" : "global",
         copyright: "© 2020 Denis Pushkarev (zloirock.ru)"
@@ -313,30 +304,39 @@
 }, function(t, e) {
     var n = 0,
         r = Math.random();
     t.exports = function(t) {
         return "Symbol(" + String(void 0 === t ? "" : t) + ")_" + (++n + r).toString(36)
     }
 }, function(t, e, n) {
+    var r = n(46),
+        o = n(0),
+        i = function(t) {
+            return "function" == typeof t ? t : void 0
+        };
+    t.exports = function(t, e) {
+        return arguments.length < 2 ? i(r[t]) || i(o[t]) : r[t] && r[t][e] || o[t] && o[t][e]
+    }
+}, function(t, e, n) {
     var r = n(2),
         o = n(13),
         i = n(33).indexOf,
         u = n(17);
     t.exports = function(t, e) {
         var n, c = o(t),
             a = 0,
             f = [];
         for (n in c) !r(u, n) && r(c, n) && f.push(n);
         for (; e.length > a;) r(c, n = e[a++]) && (~i(f, n) || f.push(n));
         return f
     }
 }, function(t, e, n) {
     var r = n(13),
-        o = n(11),
-        i = n(50),
+        o = n(10),
+        i = n(48),
         u = function(t) {
             return function(e, n, u) {
                 var c, a = r(e),
                     f = o(a.length),
                     l = i(u, f);
                 if (t && n != n) {
                     for (; f > l;)
@@ -348,70 +348,52 @@
             }
         };
     t.exports = {
         includes: u(!0),
         indexOf: u(!1)
     }
 }, function(t, e, n) {
-    var r = n(7);
-    t.exports = function(t) {
-        return Object(r(t))
-    }
-}, function(t, e, n) {
     var r = n(1);
     t.exports = !!Object.getOwnPropertySymbols && !r((function() {
         return !String(Symbol())
     }))
 }, function(t, e, n) {
     "use strict";
-    var r = n(40).forEach,
-        o = n(41),
-        i = n(23),
+    var r = n(37).forEach,
+        o = n(39),
+        i = n(20),
         u = o("forEach"),
         c = i("forEach");
     t.exports = u && c ? [].forEach : function(t) {
         return r(this, t, arguments.length > 1 ? arguments[1] : void 0)
     }
 }, function(t, e, n) {
     var r = n(0),
-        o = n(6),
+        o = n(5),
         i = n(2),
         u = n(15),
-        c = n(27),
-        a = n(44),
+        c = n(26),
+        a = n(42),
         f = a.get,
         l = a.enforce,
         s = String(String).split("String");
     (t.exports = function(t, e, n, c) {
         var a, f = !!c && !!c.unsafe,
             p = !!c && !!c.enumerable,
             v = !!c && !!c.noTargetGet;
         "function" == typeof n && ("string" != typeof e || i(n, "name") || o(n, "name", e), (a = l(n)).source || (a.source = s.join("string" == typeof e ? e : ""))), t !== r ? (f ? !v && t[e] && (p = !0) : delete t[e], p ? t[e] = n : o(t, e, n)) : p ? t[e] = n : u(e, n)
     })(Function.prototype, "toString", (function() {
         return "function" == typeof this && f(this).source || c(this)
     }))
 }, function(t, e, n) {
-    var r = n(14);
-    t.exports = Array.isArray || function(t) {
-        return "Array" == r(t)
-    }
-}, function(t, e, n) {
-    var r = n(4),
-        o = n(38),
-        i = n(10)("species");
-    t.exports = function(t, e) {
-        var n;
-        return o(t) && ("function" != typeof(n = t.constructor) || n !== Array && !o(n.prototype) ? r(n) && null === (n = n[i]) && (n = void 0) : n = void 0), new(void 0 === n ? Array : n)(0 === e ? 0 : e)
-    }
-}, function(t, e, n) {
-    var r = n(54),
-        o = n(24),
-        i = n(34),
-        u = n(11),
-        c = n(39),
+    var r = n(51),
+        o = n(22),
+        i = n(38),
+        u = n(10),
+        c = n(53),
         a = [].push,
         f = function(t) {
             var e = 1 == t,
                 n = 2 == t,
                 f = 3 == t,
                 l = 4 == t,
                 s = 6 == t,
@@ -446,14 +428,19 @@
         some: f(3),
         every: f(4),
         find: f(5),
         findIndex: f(6),
         filterOut: f(7)
     }
 }, function(t, e, n) {
+    var r = n(7);
+    t.exports = function(t) {
+        return Object(r(t))
+    }
+}, function(t, e, n) {
     "use strict";
     var r = n(1);
     t.exports = function(t, e) {
         var n = [][t];
         return !!n && r((function() {
             n.call(null, e || function() {
                 throw 1
@@ -479,21 +466,21 @@
             1: 2
         }, 1);
     e.f = i ? function(t) {
         var e = o(this, t);
         return !!e && e.enumerable
     } : r
 }, function(t, e, n) {
-    var r, o, i, u = n(45),
+    var r, o, i, u = n(43),
         c = n(0),
         a = n(4),
-        f = n(6),
+        f = n(5),
         l = n(2),
         s = n(16),
-        p = n(28),
+        p = n(27),
         v = n(17),
         d = c.WeakMap;
     if (u) {
         var h = s.state || (s.state = new d),
             g = h.get,
             y = h.has,
             x = h.set;
@@ -527,33 +514,33 @@
                 if (!a(e) || (n = o(e)).type !== t) throw TypeError("Incompatible receiver, " + t + " required");
                 return n
             }
         }
     }
 }, function(t, e, n) {
     var r = n(0),
-        o = n(27),
+        o = n(26),
         i = r.WeakMap;
     t.exports = "function" == typeof i && /native code/.test(o(i))
 }, function(t, e, n) {
     var r = n(2),
-        o = n(47),
+        o = n(45),
         i = n(12),
-        u = n(8);
+        u = n(9);
     t.exports = function(t, e) {
         for (var n = o(e), c = u.f, a = i.f, f = 0; f < n.length; f++) {
             var l = n[f];
             r(t, l) || c(t, l, a(e, l))
         }
     }
 }, function(t, e, n) {
-    var r = n(22),
-        o = n(49),
-        i = n(51),
-        u = n(9);
+    var r = n(31),
+        o = n(47),
+        i = n(49),
+        u = n(8);
     t.exports = r("Reflect", "ownKeys") || function(t) {
         var e = o.f(u(t)),
             n = i.f;
         return n ? e.concat(n(t)) : e
     }
 }, function(t, e, n) {
     var r = n(0);
@@ -585,18 +572,15 @@
             return String(t).replace(o, ".").toLowerCase()
         },
         c = i.data = {},
         a = i.NATIVE = "N",
         f = i.POLYFILL = "P";
     t.exports = i
 }, function(t, e, n) {
-    var r = n(35);
-    t.exports = r && !Symbol.sham && "symbol" == typeof Symbol.iterator
-}, function(t, e, n) {
-    var r = n(55);
+    var r = n(52);
     t.exports = function(t, e, n) {
         if (r(t), void 0 === e) return t;
         switch (n) {
             case 0:
                 return function() {
                     return t.call(e)
                 };
@@ -619,33 +603,49 @@
     }
 }, function(t, e) {
     t.exports = function(t) {
         if ("function" != typeof t) throw TypeError(String(t) + " is not a function");
         return t
     }
 }, function(t, e, n) {
-    var r = n(10),
+    var r = n(4),
+        o = n(54),
+        i = n(11)("species");
+    t.exports = function(t, e) {
+        var n;
+        return o(t) && ("function" != typeof(n = t.constructor) || n !== Array && !o(n.prototype) ? r(n) && null === (n = n[i]) && (n = void 0) : n = void 0), new(void 0 === n ? Array : n)(0 === e ? 0 : e)
+    }
+}, function(t, e, n) {
+    var r = n(14);
+    t.exports = Array.isArray || function(t) {
+        return "Array" == r(t)
+    }
+}, function(t, e, n) {
+    var r = n(34);
+    t.exports = r && !Symbol.sham && "symbol" == typeof Symbol.iterator
+}, function(t, e, n) {
+    var r = n(11),
         o = n(57),
-        i = n(8),
+        i = n(9),
         u = r("unscopables"),
         c = Array.prototype;
     null == c[u] && i.f(c, u, {
         configurable: !0,
         value: o(null)
     }), t.exports = function(t) {
         c[u][t] = !0
     }
 }, function(t, e, n) {
-    var r, o = n(9),
+    var r, o = n(8),
         i = n(58),
         u = n(19),
         c = n(17),
         a = n(60),
-        f = n(26),
-        l = n(28),
+        f = n(25),
+        l = n(27),
         s = l("IE_PROTO"),
         p = function() {},
         v = function(t) {
             return "<script>" + t + "<\/script>"
         },
         d = function() {
             try {
@@ -662,47 +662,47 @@
         };
     c[s] = !0, t.exports = Object.create || function(t, e) {
         var n;
         return null !== t ? (p.prototype = o(t), n = new p, p.prototype = null, n[s] = t) : n = d(), void 0 === e ? n : i(n, e)
     }
 }, function(t, e, n) {
     var r = n(3),
-        o = n(8),
-        i = n(9),
+        o = n(9),
+        i = n(8),
         u = n(59);
     t.exports = r ? Object.defineProperties : function(t, e) {
         i(t);
         for (var n, r = u(e), c = r.length, a = 0; c > a;) o.f(t, n = r[a++], e[n]);
         return t
     }
 }, function(t, e, n) {
     var r = n(32),
         o = n(19);
     t.exports = Object.keys || function(t) {
         return r(t, o)
     }
 }, function(t, e, n) {
-    var r = n(22);
+    var r = n(31);
     t.exports = r("document", "documentElement")
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
-        o = n(36);
+    var r = n(6),
+        o = n(35);
     r({
         target: "Array",
         proto: !0,
         forced: [].forEach != o
     }, {
         forEach: o
     })
 }, function(t, e, n) {
     var r = n(0),
         o = n(63),
-        i = n(36),
-        u = n(6);
+        i = n(35),
+        u = n(5);
     for (var c in o) {
         var a = r[c],
             f = a && a.prototype;
         if (f && f.forEach !== i) try {
             u(f, "forEach", i)
         } catch (t) {
             f.forEach = i
@@ -740,16 +740,16 @@
         StyleSheetList: 0,
         TextTrackCueList: 0,
         TextTrackList: 0,
         TouchList: 0
     }
 }, function(t, e, n) {
     "use strict";
-    var r, o, i = n(81),
-        u = n(82),
+    var r, o, i = n(76),
+        u = n(77),
         c = RegExp.prototype.exec,
         a = String.prototype.replace,
         f = c,
         l = (r = /a/, o = /b*/g, c.call(r, "a"), c.call(o, "a"), 0 !== r.lastIndex || 0 !== o.lastIndex),
         s = u.UNSUPPORTED_Y || u.BROKEN_CARET,
         p = void 0 !== /()??/.exec("")[1];
     (l || p || s) && (f = function(t) {
@@ -760,49 +760,49 @@
             h = 0,
             g = t;
         return f && (-1 === (v = v.replace("y", "")).indexOf("g") && (v += "g"), g = String(t).slice(u.lastIndex), u.lastIndex > 0 && (!u.multiline || u.multiline && "\n" !== t[u.lastIndex - 1]) && (d = "(?: " + d + ")", g = " " + g, h++), n = new RegExp("^(?:" + d + ")", v)), p && (n = new RegExp("^" + d + "$(?!\\s)", v)), l && (e = u.lastIndex), r = c.call(f ? n : u, g), f ? r ? (r.input = r.input.slice(h), r[0] = r[0].slice(h), r.index = u.lastIndex, u.lastIndex += r[0].length) : u.lastIndex = 0 : l && r && (u.lastIndex = u.global ? r.index + r[0].length : e), p && r && r.length > 1 && a.call(r[0], n, (function() {
             for (o = 1; o < arguments.length - 2; o++) void 0 === arguments[o] && (r[o] = void 0)
         })), r
     }), t.exports = f
 }, function(t, e, n) {
-    var r = n(84);
+    var r = n(79);
     t.exports = function(t) {
         if (r(t)) throw TypeError("The method doesn't accept regular expressions");
         return t
     }
 }, function(t, e, n) {
-    var r = n(10)("match");
+    var r = n(11)("match");
     t.exports = function(t) {
         var e = /./;
         try {
             "/./" [t](e)
         } catch (n) {
             try {
                 return e[r] = !1, "/./" [t](e)
             } catch (t) {}
         }
         return !1
     }
-}, , function(t, e, n) {
+}, function(t, e, n) {
     "use strict";
-    var r = n(5),
+    var r = n(6),
         o = n(64);
     r({
         target: "RegExp",
         proto: !0,
         forced: /./.exec !== o
     }, {
         exec: o
     })
 }, function(t, e) {
     t.exports = "\t\n\v\f\r                　\u2028\u2029\ufeff"
-}, , , , , , , , , , function(t, e, n) {
+}, , , , , , function(t, e, n) {
     "use strict";
     n.r(e);
-    n(61), n(80), n(68), n(83), n(85), n(86), n(91), n(92), n(62);
+    n(61), n(75), n(67), n(78), n(80), n(81), n(86), n(87), n(62);
 
     function r(t) {
         var e = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
             n = document.getElementsByName(t);
         return n.length ? e ? n[0] : n : null
     }
 
@@ -919,32 +919,32 @@
                     }))
                 }(t), a(), t.style.display = "block", (e = document.getElementsByClassName("waf--field-container--error")).length && e[0].scrollIntoView()
             }
             var e
         }()
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
+    var r = n(6),
         o = n(33).includes,
         i = n(56);
     r({
         target: "Array",
         proto: !0,
-        forced: !n(23)("indexOf", {
+        forced: !n(20)("indexOf", {
             ACCESSORS: !0,
             1: 0
         })
     }, {
         includes: function(t) {
             return o(this, t, arguments.length > 1 ? arguments[1] : void 0)
         }
     }), i("includes")
 }, function(t, e, n) {
     "use strict";
-    var r = n(9);
+    var r = n(8);
     t.exports = function() {
         var t = r(this),
             e = "";
         return t.global && (e += "g"), t.ignoreCase && (e += "i"), t.multiline && (e += "m"), t.dotAll && (e += "s"), t.unicode && (e += "u"), t.sticky && (e += "y"), e
     }
 }, function(t, e, n) {
     "use strict";
@@ -958,21 +958,21 @@
         return t.lastIndex = 2, null != t.exec("abcd")
     })), e.BROKEN_CARET = r((function() {
         var t = o("^r", "gy");
         return t.lastIndex = 2, null != t.exec("str")
     }))
 }, function(t, e, n) {
     "use strict";
-    var r, o = n(5),
+    var r, o = n(6),
         i = n(12).f,
-        u = n(11),
+        u = n(10),
         c = n(65),
         a = n(7),
         f = n(66),
-        l = n(30),
+        l = n(29),
         s = "".endsWith,
         p = Math.min,
         v = f("endsWith");
     o({
         target: "String",
         proto: !0,
         forced: !!(l || v || (r = i(String.prototype, "endsWith"), !r || r.writable)) && !v
@@ -986,43 +986,43 @@
                 i = String(t);
             return s ? s.call(e, i, o) : e.slice(o - i.length, o) === i
         }
     })
 }, function(t, e, n) {
     var r = n(4),
         o = n(14),
-        i = n(10)("match");
+        i = n(11)("match");
     t.exports = function(t) {
         var e;
         return r(t) && (void 0 !== (e = t[i]) ? !!e : "RegExp" == o(t))
     }
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
+    var r = n(6),
         o = n(65),
         i = n(7);
     r({
         target: "String",
         proto: !0,
         forced: !n(66)("includes")
     }, {
         includes: function(t) {
             return !!~String(i(this)).indexOf(o(t), arguments.length > 1 ? arguments[1] : void 0)
         }
     })
 }, function(t, e, n) {
     "use strict";
-    var r = n(87),
-        o = n(9),
-        i = n(34),
-        u = n(11),
+    var r = n(82),
+        o = n(8),
+        i = n(38),
+        u = n(10),
         c = n(18),
         a = n(7),
-        f = n(88),
-        l = n(90),
+        f = n(83),
+        l = n(85),
         s = Math.max,
         p = Math.min,
         v = Math.floor,
         d = /\$([$&'`]|\d\d?|<[^>]*>)/g,
         h = /\$([$&'`]|\d\d?)/g;
     r("replace", 2, (function(t, e, n, r) {
         var g = r.REGEXP_REPLACE_SUBSTITUTES_UNDEFINED_CAPTURE,
@@ -1095,20 +1095,20 @@
                 }
                 return void 0 === c ? "" : c
             }))
         }
     }))
 }, function(t, e, n) {
     "use strict";
-    n(68);
-    var r = n(37),
+    n(67);
+    var r = n(36),
         o = n(1),
-        i = n(10),
+        i = n(11),
         u = n(64),
-        c = n(6),
+        c = n(5),
         a = i("species"),
         f = !o((function() {
             var t = /./;
             return t.exec = function() {
                 var t = [];
                 return t.groups = {
                     a: "7"
@@ -1168,15 +1168,15 @@
                 return b.call(t, this)
             })
         }
         s && c(RegExp.prototype[d], "sham", !0)
     }
 }, function(t, e, n) {
     "use strict";
-    var r = n(89).charAt;
+    var r = n(84).charAt;
     t.exports = function(t, e, n) {
         return e + (n ? r(t, e).length : 1)
     }
 }, function(t, e, n) {
     var r = n(18),
         o = n(7),
         i = function(t) {
@@ -1202,21 +1202,21 @@
             return i
         }
         if ("RegExp" !== r(t)) throw TypeError("RegExp#exec called on incompatible receiver");
         return o.call(t, e)
     }
 }, function(t, e, n) {
     "use strict";
-    var r, o = n(5),
+    var r, o = n(6),
         i = n(12).f,
-        u = n(11),
+        u = n(10),
         c = n(65),
         a = n(7),
         f = n(66),
-        l = n(30),
+        l = n(29),
         s = "".startsWith,
         p = Math.min,
         v = f("startsWith");
     o({
         target: "String",
         proto: !0,
         forced: !!(l || v || (r = i(String.prototype, "startsWith"), !r || r.writable)) && !v
@@ -1227,28 +1227,28 @@
             var n = u(p(arguments.length > 1 ? arguments[1] : void 0, e.length)),
                 r = String(t);
             return s ? s.call(e, r, n) : e.slice(n, n + r.length) === r
         }
     })
 }, function(t, e, n) {
     "use strict";
-    var r = n(5),
-        o = n(93).trim;
+    var r = n(6),
+        o = n(88).trim;
     r({
         target: "String",
         proto: !0,
-        forced: n(94)("trim")
+        forced: n(89)("trim")
     }, {
         trim: function() {
             return o(this)
         }
     })
 }, function(t, e, n) {
     var r = n(7),
-        o = "[" + n(69) + "]",
+        o = "[" + n(68) + "]",
         i = RegExp("^" + o + o + "*"),
         u = RegExp(o + o + "*$"),
         c = function(t) {
             return function(e) {
                 var n = String(r(e));
                 return 1 & t && (n = n.replace(i, "")), 2 & t && (n = n.replace(u, "")), n
             }
@@ -1256,14 +1256,14 @@
     t.exports = {
         start: c(1),
         end: c(2),
         trim: c(3)
     }
 }, function(t, e, n) {
     var r = n(1),
-        o = n(69);
+        o = n(68);
     t.exports = function(t) {
         return r((function() {
             return !!o[t]() || "​᠎" != "​᠎" [t]() || o[t].name !== t
         }))
     }
 }]);
```

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/js/style.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -38,11 +38,11 @@
             return e.default
         } : function() {
             return e
         };
         return r.d(t, "a", t), t
     }, r.o = function(e, t) {
         return Object.prototype.hasOwnProperty.call(e, t)
-    }, r.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", r(r.s = 70)
+    }, r.p = "/wagtail_advanced_form_builder/static/wagtail_advanced_form_builder/", r(r.s = 69)
 }({
-    70: function(e, t, r) {}
+    69: function(e, t, r) {}
 });
```

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/js/formbuilder.js`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/static_src/wagtail_advanced_form_builder/scss/main.scss`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/checkbox_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/default_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/multi_checkbox_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/fields/radio_buttons_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/form/form.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/page/form.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templates/wagtail_advanced_form_builder/tags/form_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder/templatetags/wagtail_advanced_form_builder_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/PKG-INFO` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: wagtail-advanced-form-builder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wagtail Advanced Form Builder
 Home-page: https://github.com/octavenz/wagtail-advanced-form-builder
 Author: Richard Blake (Octave)
 Author-email: richard.blake@octave.nz
 License: BSD
 Description: # Wagtail Advanced Form Builder
```

### Comparing `wagtail-advanced-form-builder-1.0.1/wagtail_advanced_form_builder.egg-info/SOURCES.txt` & `wagtail-advanced-form-builder-1.0.2/wagtail_advanced_form_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

