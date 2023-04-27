# Comparing `tmp/django-semantic-admin-0.3.8.tar.gz` & `tmp/django-semantic-admin-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-semantic-admin-0.3.8.tar", max compression
+gzip compressed data, was "django-semantic-admin-0.3.9.tar", max compression
```

## Comparing `django-semantic-admin-0.3.8.tar` & `django-semantic-admin-0.3.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1061 2021-01-03 08:39:14.916989 django-semantic-admin-0.3.8/LICENSE
--rw-r--r--   0        0        0     3747 2022-09-22 03:04:45.792434 django-semantic-admin-0.3.8/README.md
--rw-r--r--   0        0        0      906 2023-02-04 06:27:42.638325 django-semantic-admin-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      200 2020-04-13 13:22:33.163975 django-semantic-admin-0.3.8/semantic_admin/__init__.py
--rw-r--r--   0        0        0    10030 2022-02-22 00:33:50.068349 django-semantic-admin-0.3.8/semantic_admin/admin.py
--rw-r--r--   0        0        0     6330 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/awesomesearch.py
--rw-r--r--   0        0        0     1011 2022-09-21 12:59:05.927992 django-semantic-admin-0.3.8/semantic_admin/fields.py
--rw-r--r--   0        0        0      816 2021-05-09 13:10:15.238013 django-semantic-admin-0.3.8/semantic_admin/filters/__init__.py
--rw-r--r--   0        0        0     1987 2021-01-10 09:47:42.053909 django-semantic-admin-0.3.8/semantic_admin/filters/filters.py
--rw-r--r--   0        0        0     3376 2022-09-22 00:26:51.019695 django-semantic-admin-0.3.8/semantic_admin/filters/filterset.py
--rw-r--r--   0        0        0      346 2021-12-11 02:53:54.477730 django-semantic-admin-0.3.8/semantic_admin/helpers.py
--rw-r--r--   0        0        0     9513 2022-01-09 02:14:13.924155 django-semantic-admin-0.3.8/semantic_admin/static/admin/js/actions.js
--rw-r--r--   0        0        0    19008 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/static/admin/js/admin/DateTimeShortcuts.js
--rw-r--r--   0        0        0     6336 2020-04-13 13:22:33.163975 django-semantic-admin-0.3.8/semantic_admin/static/admin/js/admin/RelatedObjectLookups.js
--rw-r--r--   0        0        0     1654 2022-11-05 02:36:28.411094 django-semantic-admin-0.3.8/semantic_admin/static/admin/js/calendar.js
--rw-r--r--   0        0        0    15004 2021-05-09 02:55:52.517274 django-semantic-admin-0.3.8/semantic_admin/static/admin/js/inlines.js
--rw-r--r--   0        0        0     5525 2021-01-04 08:05:50.148569 django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/django-white.svg
--rw-r--r--   0        0        0     1099 2022-09-21 13:28:42.566821 django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/semantic-admin.css
--rw-r--r--   0        0        0     2448 2021-09-18 07:54:26.882778 django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/semanticWidgets.js
--rw-r--r--   0        0        0     1693 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/unsemantic.css
--rw-r--r--   0        0        0     1477 2022-03-12 23:46:14.973957 django-semantic-admin-0.3.8/semantic_admin/templates/admin/actions.html
--rw-r--r--   0        0        0      443 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/auth/user/add_form.html
--rw-r--r--   0        0        0     7904 2022-12-16 23:20:54.679078 django-semantic-admin-0.3.8/semantic_admin/templates/admin/base.html
--rw-r--r--   0        0        0      164 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/base_site.html
--rw-r--r--   0        0        0     6984 2022-09-21 14:50:19.955772 django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_form.html
--rw-r--r--   0        0        0     3652 2022-09-21 14:35:12.996202 django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_list.html
--rw-r--r--   0        0        0     1653 2022-01-12 11:59:50.127017 django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_list_results.html
--rw-r--r--   0        0        0      695 2021-05-09 08:32:32.517782 django-semantic-admin-0.3.8/semantic_admin/templates/admin/date_hierarchy.html
--rw-r--r--   0        0        0      250 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/delete_button.html
--rw-r--r--   0        0        0     2968 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.8/semantic_admin/templates/admin/delete_confirmation.html
--rw-r--r--   0        0        0     2864 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.8/semantic_admin/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0        0        0     2550 2020-04-26 07:09:47.986523 django-semantic-admin-0.3.8/semantic_admin/templates/admin/edit_inline/stacked.html
--rw-r--r--   0        0        0     4494 2022-09-21 13:15:41.021475 django-semantic-admin-0.3.8/semantic_admin/templates/admin/edit_inline/tabular.html
--rw-r--r--   0        0        0      733 2021-05-08 22:15:40.037355 django-semantic-admin-0.3.8/semantic_admin/templates/admin/filter.html
--rw-r--r--   0        0        0      108 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/includes/fieldset.html
--rw-r--r--   0        0        0     1657 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/templates/admin/includes/fieldset_content.html
--rw-r--r--   0        0        0      248 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.8/semantic_admin/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0        0        0     3378 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/templates/admin/index.html
--rw-r--r--   0        0        0     2299 2022-11-05 02:36:28.411094 django-semantic-admin-0.3.8/semantic_admin/templates/admin/login.html
--rw-r--r--   0        0        0     1518 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/main.html
--rw-r--r--   0        0        0     2492 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/templates/admin/menu.html
--rw-r--r--   0        0        0     1921 2021-05-10 11:32:58.008732 django-semantic-admin-0.3.8/semantic_admin/templates/admin/object_history.html
--rw-r--r--   0        0        0      596 2021-05-08 23:48:04.735684 django-semantic-admin-0.3.8/semantic_admin/templates/admin/pagination.html
--rw-r--r--   0        0        0     1542 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/templates/admin/portal.html
--rw-r--r--   0        0        0     1119 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/save_buttons.html
--rw-r--r--   0        0        0      979 2021-01-06 02:00:30.829827 django-semantic-admin-0.3.8/semantic_admin/templates/admin/search_form.html
--rw-r--r--   0        0        0      390 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/admin/submit_line.html
--rw-r--r--   0        0        0     1455 2021-01-30 04:35:53.944492 django-semantic-admin-0.3.8/semantic_admin/templates/admin/widgets/related_widget_wrapper.html
--rw-r--r--   0        0        0      797 2021-05-11 12:11:34.845740 django-semantic-admin-0.3.8/semantic_admin/templates/registration/logged_out.html
--rw-r--r--   0        0        0       33 2021-05-09 13:29:47.052939 django-semantic-admin-0.3.8/semantic_admin/templates/registration/login.html
--rw-r--r--   0        0        0      671 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_change_done.html
--rw-r--r--   0        0        0     2325 2021-05-11 12:11:34.845740 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_change_form.html
--rw-r--r--   0        0        0      505 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_complete.html
--rw-r--r--   0        0        0     1374 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_confirm.html
--rw-r--r--   0        0        0      669 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_done.html
--rw-r--r--   0        0        0      971 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_form.html
--rw-r--r--   0        0        0      442 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/action_checkbox.html
--rw-r--r--   0        0        0       94 2021-05-09 01:12:54.192892 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/changelist_checkbox.html
--rw-r--r--   0        0        0       48 2021-05-09 00:55:05.184815 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/checkbox.html
--rw-r--r--   0        0        0      176 2021-05-09 00:53:25.277561 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_option.html
--rw-r--r--   0        0        0      814 2021-05-09 00:53:13.813639 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_select.html
--rw-r--r--   0        0        0      500 2020-05-04 02:05:44.342871 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/chooser.html
--rw-r--r--   0        0        0      583 2021-01-06 10:50:55.496825 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/clearable_file_input.html
--rw-r--r--   0        0        0      269 2021-01-05 03:25:34.193194 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/date.html
--rw-r--r--   0        0        0      273 2021-01-05 03:25:27.625263 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/datetime.html
--rw-r--r--   0        0        0      207 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/input_autocomplete_off.html
--rw-r--r--   0        0        0      265 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/input_option.html
--rw-r--r--   0        0        0      124 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/multiwidget.html
--rw-r--r--   0        0        0      396 2021-01-10 11:33:13.868736 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/radio.html
--rw-r--r--   0        0        0      219 2021-01-10 11:33:29.732622 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/radio_option.html
--rw-r--r--   0        0        0      612 2021-01-05 07:53:16.093791 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/select.html
--rw-r--r--   0        0        0      145 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/select_time.html
--rw-r--r--   0        0        0       76 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/text.html
--rw-r--r--   0        0        0      170 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/textarea.html
--rw-r--r--   0        0        0      267 2021-01-05 03:27:22.208053 django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/time.html
--rw-r--r--   0        0        0        0 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.8/semantic_admin/templatetags/__init__.py
--rw-r--r--   0        0        0     4656 2022-01-16 02:13:45.696323 django-semantic-admin-0.3.8/semantic_admin/templatetags/awesomesearch.py
--rw-r--r--   0        0        0     5990 2021-05-09 01:11:55.961632 django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_admin_list.py
--rw-r--r--   0        0        0     3125 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_app_list.py
--rw-r--r--   0        0        0     2573 2021-05-09 08:51:32.800131 django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_filters.py
--rw-r--r--   0        0        0    10511 2022-09-21 14:50:19.955772 django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_utils.py
--rw-r--r--   0        0        0     2623 2021-05-08 20:41:26.038586 django-semantic-admin-0.3.8/semantic_admin/utils.py
--rw-r--r--   0        0        0        0 2020-04-13 13:22:33.207974 django-semantic-admin-0.3.8/semantic_admin/views/__init__.py
--rw-r--r--   0        0        0     1632 2022-09-21 13:28:42.566821 django-semantic-admin-0.3.8/semantic_admin/views/autocomplete.py
--rw-r--r--   0        0        0     1375 2021-05-09 01:04:58.058754 django-semantic-admin-0.3.8/semantic_admin/widgets/__init__.py
--rw-r--r--   0        0        0      287 2021-05-09 01:04:22.491169 django-semantic-admin-0.3.8/semantic_admin/widgets/admin.py
--rw-r--r--   0        0        0      810 2022-02-22 00:36:25.602026 django-semantic-admin-0.3.8/semantic_admin/widgets/autocomplete.py
--rw-r--r--   0        0        0     2375 2021-01-30 06:28:38.157252 django-semantic-admin-0.3.8/semantic_admin/widgets/widgets.py
--rw-r--r--   0        0        0     5127 2023-02-05 23:46:50.612020 django-semantic-admin-0.3.8/setup.py
--rw-r--r--   0        0        0     4554 2023-02-05 23:46:50.612421 django-semantic-admin-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-01-03 08:39:14.916989 django-semantic-admin-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3747 2022-09-22 03:04:45.792434 django-semantic-admin-0.3.9/README.md
+-rw-r--r--   0        0        0      901 2023-04-27 23:13:58.752266 django-semantic-admin-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      200 2020-04-13 13:22:33.163975 django-semantic-admin-0.3.9/semantic_admin/__init__.py
+-rw-r--r--   0        0        0    10030 2022-02-22 00:33:50.068349 django-semantic-admin-0.3.9/semantic_admin/admin.py
+-rw-r--r--   0        0        0     6330 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/awesomesearch.py
+-rw-r--r--   0        0        0     1011 2022-09-21 12:59:05.927992 django-semantic-admin-0.3.9/semantic_admin/fields.py
+-rw-r--r--   0        0        0      816 2021-05-09 13:10:15.238013 django-semantic-admin-0.3.9/semantic_admin/filters/__init__.py
+-rw-r--r--   0        0        0     1987 2021-01-10 09:47:42.053909 django-semantic-admin-0.3.9/semantic_admin/filters/filters.py
+-rw-r--r--   0        0        0     3376 2022-09-22 00:26:51.019695 django-semantic-admin-0.3.9/semantic_admin/filters/filterset.py
+-rw-r--r--   0        0        0      346 2021-12-11 02:53:54.477730 django-semantic-admin-0.3.9/semantic_admin/helpers.py
+-rw-r--r--   0        0        0     9513 2022-01-09 02:14:13.924155 django-semantic-admin-0.3.9/semantic_admin/static/admin/js/actions.js
+-rw-r--r--   0        0        0    19008 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/static/admin/js/admin/DateTimeShortcuts.js
+-rw-r--r--   0        0        0     6336 2020-04-13 13:22:33.163975 django-semantic-admin-0.3.9/semantic_admin/static/admin/js/admin/RelatedObjectLookups.js
+-rw-r--r--   0        0        0     1654 2022-11-05 02:36:28.411094 django-semantic-admin-0.3.9/semantic_admin/static/admin/js/calendar.js
+-rw-r--r--   0        0        0    15004 2021-05-09 02:55:52.517274 django-semantic-admin-0.3.9/semantic_admin/static/admin/js/inlines.js
+-rw-r--r--   0        0        0     5525 2021-01-04 08:05:50.148569 django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/django-white.svg
+-rw-r--r--   0        0        0     1099 2022-09-21 13:28:42.566821 django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/semantic-admin.css
+-rw-r--r--   0        0        0     2448 2021-09-18 07:54:26.882778 django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/semanticWidgets.js
+-rw-r--r--   0        0        0     1693 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/unsemantic.css
+-rw-r--r--   0        0        0     1477 2022-03-12 23:46:14.973957 django-semantic-admin-0.3.9/semantic_admin/templates/admin/actions.html
+-rw-r--r--   0        0        0      443 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     7904 2022-12-16 23:20:54.679078 django-semantic-admin-0.3.9/semantic_admin/templates/admin/base.html
+-rw-r--r--   0        0        0      164 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/base_site.html
+-rw-r--r--   0        0        0     6984 2022-09-21 14:50:19.955772 django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_form.html
+-rw-r--r--   0        0        0     3652 2022-09-21 14:35:12.996202 django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_list.html
+-rw-r--r--   0        0        0     1653 2022-01-12 11:59:50.127017 django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_list_results.html
+-rw-r--r--   0        0        0      695 2021-05-09 08:32:32.517782 django-semantic-admin-0.3.9/semantic_admin/templates/admin/date_hierarchy.html
+-rw-r--r--   0        0        0      250 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/delete_button.html
+-rw-r--r--   0        0        0     2968 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.9/semantic_admin/templates/admin/delete_confirmation.html
+-rw-r--r--   0        0        0     2864 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.9/semantic_admin/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     2550 2020-04-26 07:09:47.986523 django-semantic-admin-0.3.9/semantic_admin/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0        0        0     4494 2022-09-21 13:15:41.021475 django-semantic-admin-0.3.9/semantic_admin/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0        0        0      733 2021-05-08 22:15:40.037355 django-semantic-admin-0.3.9/semantic_admin/templates/admin/filter.html
+-rw-r--r--   0        0        0      108 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0     1657 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/templates/admin/includes/fieldset_content.html
+-rw-r--r--   0        0        0      248 2021-05-11 12:11:34.841769 django-semantic-admin-0.3.9/semantic_admin/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0        0        0     3378 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/templates/admin/index.html
+-rw-r--r--   0        0        0     2299 2022-11-05 02:36:28.411094 django-semantic-admin-0.3.9/semantic_admin/templates/admin/login.html
+-rw-r--r--   0        0        0     1518 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/main.html
+-rw-r--r--   0        0        0     2492 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/templates/admin/menu.html
+-rw-r--r--   0        0        0     1921 2021-05-10 11:32:58.008732 django-semantic-admin-0.3.9/semantic_admin/templates/admin/object_history.html
+-rw-r--r--   0        0        0      596 2021-05-08 23:48:04.735684 django-semantic-admin-0.3.9/semantic_admin/templates/admin/pagination.html
+-rw-r--r--   0        0        0     1542 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/templates/admin/portal.html
+-rw-r--r--   0        0        0     1119 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/save_buttons.html
+-rw-r--r--   0        0        0      979 2021-01-06 02:00:30.829827 django-semantic-admin-0.3.9/semantic_admin/templates/admin/search_form.html
+-rw-r--r--   0        0        0      390 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/admin/submit_line.html
+-rw-r--r--   0        0        0     1455 2021-01-30 04:35:53.944492 django-semantic-admin-0.3.9/semantic_admin/templates/admin/widgets/related_widget_wrapper.html
+-rw-r--r--   0        0        0      797 2021-05-11 12:11:34.845740 django-semantic-admin-0.3.9/semantic_admin/templates/registration/logged_out.html
+-rw-r--r--   0        0        0       33 2021-05-09 13:29:47.052939 django-semantic-admin-0.3.9/semantic_admin/templates/registration/login.html
+-rw-r--r--   0        0        0      671 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_change_done.html
+-rw-r--r--   0        0        0     2325 2021-05-11 12:11:34.845740 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_change_form.html
+-rw-r--r--   0        0        0      505 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_complete.html
+-rw-r--r--   0        0        0     1374 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_confirm.html
+-rw-r--r--   0        0        0      669 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_done.html
+-rw-r--r--   0        0        0      971 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_form.html
+-rw-r--r--   0        0        0      442 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/action_checkbox.html
+-rw-r--r--   0        0        0       94 2021-05-09 01:12:54.192892 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/changelist_checkbox.html
+-rw-r--r--   0        0        0       48 2021-05-09 00:55:05.184815 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/checkbox.html
+-rw-r--r--   0        0        0      176 2021-05-09 00:53:25.277561 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_option.html
+-rw-r--r--   0        0        0      814 2021-05-09 00:53:13.813639 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_select.html
+-rw-r--r--   0        0        0      500 2020-05-04 02:05:44.342871 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/chooser.html
+-rw-r--r--   0        0        0      583 2021-01-06 10:50:55.496825 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/clearable_file_input.html
+-rw-r--r--   0        0        0      269 2021-01-05 03:25:34.193194 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/date.html
+-rw-r--r--   0        0        0      273 2021-01-05 03:25:27.625263 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/datetime.html
+-rw-r--r--   0        0        0      207 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/input_autocomplete_off.html
+-rw-r--r--   0        0        0      265 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/input_option.html
+-rw-r--r--   0        0        0      124 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/multiwidget.html
+-rw-r--r--   0        0        0      396 2021-01-10 11:33:13.868736 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/radio.html
+-rw-r--r--   0        0        0      219 2021-01-10 11:33:29.732622 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/radio_option.html
+-rw-r--r--   0        0        0      612 2021-01-05 07:53:16.093791 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/select.html
+-rw-r--r--   0        0        0      145 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/select_time.html
+-rw-r--r--   0        0        0       76 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/text.html
+-rw-r--r--   0        0        0      170 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/textarea.html
+-rw-r--r--   0        0        0      267 2021-01-05 03:27:22.208053 django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/time.html
+-rw-r--r--   0        0        0        0 2020-04-13 13:22:33.203974 django-semantic-admin-0.3.9/semantic_admin/templatetags/__init__.py
+-rw-r--r--   0        0        0     4656 2022-01-16 02:13:45.696323 django-semantic-admin-0.3.9/semantic_admin/templatetags/awesomesearch.py
+-rw-r--r--   0        0        0     5990 2021-05-09 01:11:55.961632 django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_admin_list.py
+-rw-r--r--   0        0        0     3125 2022-09-22 03:04:45.796434 django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_app_list.py
+-rw-r--r--   0        0        0     2573 2021-05-09 08:51:32.800131 django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_filters.py
+-rw-r--r--   0        0        0    10511 2022-09-21 14:50:19.955772 django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_utils.py
+-rw-r--r--   0        0        0     2623 2021-05-08 20:41:26.038586 django-semantic-admin-0.3.9/semantic_admin/utils.py
+-rw-r--r--   0        0        0        0 2020-04-13 13:22:33.207974 django-semantic-admin-0.3.9/semantic_admin/views/__init__.py
+-rw-r--r--   0        0        0     1632 2022-09-21 13:28:42.566821 django-semantic-admin-0.3.9/semantic_admin/views/autocomplete.py
+-rw-r--r--   0        0        0     1375 2021-05-09 01:04:58.058754 django-semantic-admin-0.3.9/semantic_admin/widgets/__init__.py
+-rw-r--r--   0        0        0      287 2021-05-09 01:04:22.491169 django-semantic-admin-0.3.9/semantic_admin/widgets/admin.py
+-rw-r--r--   0        0        0      810 2022-02-22 00:36:25.602026 django-semantic-admin-0.3.9/semantic_admin/widgets/autocomplete.py
+-rw-r--r--   0        0        0     2375 2021-01-30 06:28:38.157252 django-semantic-admin-0.3.9/semantic_admin/widgets/widgets.py
+-rw-r--r--   0        0        0     5122 2023-04-27 23:14:04.480230 django-semantic-admin-0.3.9/setup.py
+-rw-r--r--   0        0        0     4549 2023-04-27 23:14:04.480649 django-semantic-admin-0.3.9/PKG-INFO
```

### Comparing `django-semantic-admin-0.3.8/LICENSE` & `django-semantic-admin-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/README.md` & `django-semantic-admin-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/pyproject.toml` & `django-semantic-admin-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "django-semantic-admin"
-version = "0.3.8"
+version = "0.3.9"
 description = "Django Semantic UI Admin theme"
 authors = ["Alex <globophobe@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/globophobe/django-semantic-admin"
 repository = "https://github.com/globophobe/django-semantic-admin"
 keywords = ["django", "admin", "theme"]
 classifiers = ["Framework :: Django", "Development Status :: 4 - Beta", "Operating System :: OS Independent"]
 packages = [{ include = "semantic_admin" }]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8"
 django = ">=3.2"
 
 [tool.poetry.dev-dependencies]
 flake8 = "*"
 black = "*"
 isort = "*"
 Pillow = "*"
```

### Comparing `django-semantic-admin-0.3.8/semantic_admin/admin.py` & `django-semantic-admin-0.3.9/semantic_admin/admin.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/awesomesearch.py` & `django-semantic-admin-0.3.9/semantic_admin/awesomesearch.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/fields.py` & `django-semantic-admin-0.3.9/semantic_admin/fields.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/filters/__init__.py` & `django-semantic-admin-0.3.9/semantic_admin/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/filters/filters.py` & `django-semantic-admin-0.3.9/semantic_admin/filters/filters.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/filters/filterset.py` & `django-semantic-admin-0.3.9/semantic_admin/filters/filterset.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/admin/js/actions.js` & `django-semantic-admin-0.3.9/semantic_admin/static/admin/js/actions.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/admin/js/admin/DateTimeShortcuts.js` & `django-semantic-admin-0.3.9/semantic_admin/static/admin/js/admin/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/admin/js/admin/RelatedObjectLookups.js` & `django-semantic-admin-0.3.9/semantic_admin/static/admin/js/admin/RelatedObjectLookups.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/admin/js/calendar.js` & `django-semantic-admin-0.3.9/semantic_admin/static/admin/js/calendar.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/admin/js/inlines.js` & `django-semantic-admin-0.3.9/semantic_admin/static/admin/js/inlines.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/django-white.svg` & `django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/django-white.svg`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/semantic-admin.css` & `django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/semantic-admin.css`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/semanticWidgets.js` & `django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/semanticWidgets.js`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/static/semantic_admin/unsemantic.css` & `django-semantic-admin-0.3.9/semantic_admin/static/semantic_admin/unsemantic.css`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/actions.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/base.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_form.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_list.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/change_list_results.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/date_hierarchy.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/delete_confirmation.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/delete_selected_confirmation.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/edit_inline/stacked.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/edit_inline/tabular.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/filter.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/includes/fieldset_content.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/includes/fieldset_content.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/index.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/login.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/main.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/main.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/menu.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/menu.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/object_history.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/pagination.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/portal.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/portal.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/save_buttons.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/save_buttons.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/search_form.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/admin/widgets/related_widget_wrapper.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/logged_out.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_change_done.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_change_form.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_confirm.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_done.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/registration/password_reset_form.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_select.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/checkbox_select.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/clearable_file_input.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templates/semantic_ui/forms/widgets/select.html` & `django-semantic-admin-0.3.9/semantic_admin/templates/semantic_ui/forms/widgets/select.html`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templatetags/awesomesearch.py` & `django-semantic-admin-0.3.9/semantic_admin/templatetags/awesomesearch.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_admin_list.py` & `django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_admin_list.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_app_list.py` & `django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_app_list.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_filters.py` & `django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_filters.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/templatetags/semantic_utils.py` & `django-semantic-admin-0.3.9/semantic_admin/templatetags/semantic_utils.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/utils.py` & `django-semantic-admin-0.3.9/semantic_admin/utils.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/views/autocomplete.py` & `django-semantic-admin-0.3.9/semantic_admin/views/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/widgets/__init__.py` & `django-semantic-admin-0.3.9/semantic_admin/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/widgets/autocomplete.py` & `django-semantic-admin-0.3.9/semantic_admin/widgets/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/semantic_admin/widgets/widgets.py` & `django-semantic-admin-0.3.9/semantic_admin/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `django-semantic-admin-0.3.8/setup.py` & `django-semantic-admin-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,23 +22,23 @@
                     'templates/semantic_ui/forms/widgets/*']}
 
 install_requires = \
 ['django>=3.2']
 
 setup_kwargs = {
     'name': 'django-semantic-admin',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Django Semantic UI Admin theme',
     'long_description': 'Django Semantic UI admin theme\n------------------------------\n<img src="https://raw.githubusercontent.com/globophobe/django-semantic-admin/master/docs/screenshots/change-list.png" alt="django-semantic-admin"/>\n\nA completely free (MIT) [Semantic UI](https://semantic-ui.com/) admin theme for Django. Actually, this is my 3rd admin theme for Django. The first was forgettable, and the second was with [Pure CSS](https://purecss.io/). Pure CSS was great, but lacked JavaScript components.\n\nSemantic UI looks professional, and has great JavaScript components.\n\nLog in to the demo with username `django` and password `semantic-admin`: https://semantic-admin.com\n\nDocumentation is on [GitHub Pages](https://globophobe.github.io/django-semantic-admin/).\n\nWhy?\n----\n* Looks professional, with a nice sidebar.\n* Responsive design, even [tables can stack](https://semantic-ui.com/collections/table.html#stacking) responsively on mobile.\n* JavaScript datepicker and timepicker components.\n* JavaScript selects, including multiple selections, which integrate well with Django autocomplete fields.\n* Semantic UI has libraries for [React](https://react.semantic-ui.com/) and [Vue](https://semantic-ui-vue.github.io/#/), in addition to jQuery. This means this package can be used to style the admin, and custom views can be added with React or Vue components with the same style.\n\n\nInstall\n-------\n\nInstall from PyPI:\n\n```\npip install django-semantic-admin\n```\n\nAdd to `settings.py` before `django.contrib.admin`:\n\n```python\nINSTALLED_APPS = [\n    "semantic_admin",\n    "django.contrib.admin",\n    ...\n]\n```\n\nUsage\n-----\n\nInstead of `admin.ModelAdmin`, `admin.StackedInline`, or `admin.TabularInline`:\n\n```python\nclass ExampleStackedInline(admin.StackedInline):\n    pass\n\nclass ExampleTabularInline(admin.TabularInline):\n    pass\n\nclass ExampleAdmin(admin.ModelAdmin):\n    inlines = (ExampleStackedInline, ExampleTabularInline)\n```\n\nInherit from their `Semantic` equivalents:\n\n```python\nfrom semantic_admin import SemanticModelAdmin, SemanticStackedInline, SemanticTabularInline\n\nclass ExampleStackedInline(SemanticStackedInline):\n    pass\n\nclass ExampleTabularInline(SemanticTabularInline):\n    pass\n\nclass ExampleAdmin(SemanticModelAdmin):\n    inlines = (ExampleStackedInline, ExampleTabularInline)\n```\n\nAwesome optional features\n-------------------------\n\n1. Optional integration with [django_filter](https://github.com/carltongibson/django-filter):\n\n<img src="https://raw.githubusercontent.com/globophobe/django-semantic-admin/master/docs/screenshots/django-filter.png" width="335" alt="django-filter" />\n\nTo enable this awesome feature, add `filterset_class` to your Django admin:\n\n```python\nfrom semantic_admin.filters import SemanticFilterSet\n\nclass DemoFilter(SemanticFilterSet):\n    class Meta:\n        model = Demo\n        fields = ("demo_field",)\n\nclass DemoAdmin(SemanticModelAdmin):\n    filterset_class = DemoFilter\n```\n\n2. HTML preview in Django `autocomplete_fields`:\n\n<img src="https://raw.githubusercontent.com/globophobe/django-semantic-admin/master/docs/screenshots/html5-autocomplete.png" width="670" alt="html5-autocomplete" />\n\nTo enable this awesome feature, add the `semantic_autocomplete` property to your Django model:\n\n```python\nclass DemoModel(models.Model):\n    @property\n    def semantic_autocomplete(self):\n        html = self.get_img()\n        return format_html(html)\n```\n\nContributing\n------------\n\nInstall dependencies with `poetry install`. The demo is built with [invoke tasks](https://github.com/globophobe/django-semantic-admin/blob/master/demo/tasks.py). For example, `cd demo; invoke build`.\n\n\nNotes\n-----\nPlease note, this package uses [Fomantic UI](https://fomantic-ui.com/) the official community fork of Semantic UI.\n',
     'author': 'Alex',
     'author_email': 'globophobe@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/globophobe/django-semantic-admin',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `django-semantic-admin-0.3.8/PKG-INFO` & `django-semantic-admin-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: django-semantic-admin
-Version: 0.3.8
+Version: 0.3.9
 Summary: Django Semantic UI Admin theme
 Home-page: https://github.com/globophobe/django-semantic-admin
 License: MIT
 Keywords: django,admin,theme
 Author: Alex
 Author-email: globophobe@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

