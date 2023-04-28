# Comparing `tmp/itkdb-0.4.0rc9.tar.gz` & `tmp/itkdb-0.4.1rc1.tar.gz`

## Comparing `itkdb-0.4.0rc9.tar` & `itkdb-0.4.1rc1.tar`

### file list

```diff
@@ -1,103 +1,121 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/.flake8
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/.gitlab-ci.yml
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/MANIFEST.in
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/add_comment.py
--rwxr-xr-x   0        0        0    36498 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/generatePlots.py
--rwxr-xr-x   0        0        0    27898 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/getContentSummary.py
--rwxr-xr-x   0        0        0    20491 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/getInventory.py
--rwxr-xr-x   0        0        0    27953 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/registerComponent.py
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tbump.toml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/_version.py
--rw-r--r--   0        0        0     8768 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/client.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/commandline.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/core.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/exceptions.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/responses.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/utilities.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    10778 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     9105 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/data/README.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/models/image.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/models/text.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/models/zip.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/__init__.py
--rw-r--r--   0        0        0     4001 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/conftest.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_cli.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_client.py
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_image.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_response.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_scripts.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_session.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_user.py
--rw-r--r--   0        0        0     4870 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_cache.py
--rw-r--r--   0        0        0     6539 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_institution.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_session.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_user.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3934 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/LICENSE
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/README.md
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/pyproject.toml
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 itkdb-0.4.0rc9/PKG-INFO
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/.gitlab-ci.yml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/.linkcheckerrc
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/add_attachment.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/add_comment.py
+-rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/generatePlots.py
+-rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/getContentSummary.py
+-rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/getInventory.py
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/mkdocs.yml
+-rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/registerComponent.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tbump.toml
+-rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/ci/pre-commit-update.sh
+-rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/config.md
+-rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/examples.md
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/history.md
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/index.md
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/install.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/macros.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/.overrides/main.html
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/.snippets/abbrs.txt
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/.snippets/links.txt
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/assets/css/custom.css
+-rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/assets/images/logo.svg
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/meta/authors.md
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/meta/faq.md
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/reference/gen_ref_nav.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/docs/reference/cli/itkdb.md
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/__init__.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/_version.py
+-rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/client.py
+-rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/commandline.py
+-rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/core.py
+-rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/py.typed
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/responses.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/typing.py
+-rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/utils.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/caching/__init__.py
+-rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/caching/adapter.py
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/caching/controller.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/caching/utils.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/1x1.jpg
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/1x1.sh
+-rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/CERN_chain.pem
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/README.md
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/data/tiny.root
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/models/__init__.py
+-rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/models/file.py
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/models/institution.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/settings/__init__.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/src/itkdb/settings/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_cli.py
+-rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_client.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_image.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_response.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_scripts.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_session.py
+-rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_user.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/test_utils.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_attachments.py
+-rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_binaryData.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_cache.py
+-rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_components.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_institution.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_projects.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_session.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_shipments.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_stats.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_summary.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_testproperties.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_tests.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_user.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/test_warning.py
+-rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_add_attachment.json
+-rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
+-rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image.json
+-rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_plainText.json
+-rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
+-rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_issue4.json
+-rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_add_comment.json
+-rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get.json
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_bulk.json
+-rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_code.json
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_serial.json
+-rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
+-rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
+-rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv1.json
+-rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv2.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_get.json
+-rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_pagination.json
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_projects.test_list_projects.json
+-rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
+-rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_fake_route.json
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_invalid_project.json
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_missing_required.json
+-rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_no_bearer.json
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_unauthorized.json
+-rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_stats.test_get.json
+-rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_summary.test_get_summary.json
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
+-rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_list_test_types.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_anonymous_login.json
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_bad_login.json
+-rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_good_login.json
+-rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/tests/integration/cassettes/test_warnings.test_get_component.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/COPYING
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/LICENSE
+-rw-r--r--   0        0        0     7264 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/README.md
+-rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     9163 2020-02-02 00:00:00.000000 itkdb-0.4.1rc1/PKG-INFO
```

### Comparing `itkdb-0.4.0rc9/.pre-commit-config.yaml` & `itkdb-0.4.1rc1/.pre-commit-config.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -1,140 +1,107 @@
 ci:
   autoupdate_commit_msg: "chore: update pre-commit hooks"
-  autoupdate_schedule: monthly
+  autofix_commit_msg: "style: pre-commit fixes"
 
 exclude: |
   (?x)^(
     add_attachment.py|
     add_comment.py|
     generatePlots.py|
     getContentSummary.py|
     getInventory.py|
     registerComponent.py|
     tests/integration/cassettes/.*.json
   )$
 
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.10.0
+    rev: "23.3.0"
     hooks:
       - id: black-jupyter
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: "v4.4.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
+        exclude: mkdocs.yml
+      - id: check-yaml
+        name: check-yaml (unsafe)
+        files: mkdocs.yml
+        args: ["--unsafe"]
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
+      - id: name-tests-test
+        args: ["--pytest-test-first"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: "v1.10.0"
     hooks:
-      - id: python-check-blanket-noqa
-      - id: python-check-blanket-type-ignore
-      - id: python-no-eval
-      - id: python-use-type-annotations
       - id: rst-backticks
       - id: rst-directive-colons
       - id: rst-inline-touching-normal
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.3"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
 
   - repo: https://github.com/asottile/blacken-docs
-    rev: v1.12.1
+    rev: "1.13.0"
     hooks:
       - id: blacken-docs
         additional_dependencies: [black==22.8.0]
 
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
-    hooks:
-      - id: isort
-        args: ["-a", "from __future__ import annotations"] # Python 3.7+
-
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.1.0
-    hooks:
-      - id: pyupgrade
-        args: ["--py37-plus"]
-
-  - repo: https://github.com/pre-commit/mirrors-clang-format
-    rev: v14.0.6
-    hooks:
-      - id: clang-format
-        types_or: [c++, c, cuda]
-
-  - repo: https://github.com/hadialqattan/pycln
-    rev: v2.1.1
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: v0.0.262
     hooks:
-      - id: pycln
-        args: [--config=pyproject.toml]
+      - id: ruff
+        args: ["--fix", "--show-fixes"]
 
-  - repo: https://github.com/asottile/yesqa
-    rev: v1.4.0
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: "v1.2.0"
     hooks:
-      - id: yesqa
-        exclude: docs/conf.py
-        additional_dependencies: &flake8_dependencies
-          - flake8-bugbear
-          - flake8-print
-
-  - repo: https://github.com/pycqa/flake8
-    rev: 5.0.4
-    hooks:
-      - id: flake8
-        exclude: docs/conf.py
-        additional_dependencies: *flake8_dependencies
-
-  - repo: https://github.com/pycqa/bandit
-    rev: 1.7.4
-    hooks:
-      - id: bandit
+      - id: mypy
         files: src
-
-  #- repo: https://github.com/pre-commit/mirrors-mypy
-  #  rev: v0.982
-  #  hooks:
-  #    - id: mypy
-  #      files: src
-  #      args: [--show-error-codes]
+        args: []
+        additional_dependencies:
+          [
+            "attrs",
+            "python-dotenv",
+            "click",
+            "importlib_resources",
+            "types-requests",
+            "types-python-jose",
+            "types-pycurl",
+          ]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
         exclude: |
           (?x)^(
             .*\.json |
             .*\.pem
           )$
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
-    rev: v0.8.0.4
+    rev: "v0.9.0.2"
     hooks:
       - id: shellcheck
 
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
-
-  - repo: https://github.com/mgedmin/check-manifest
-    rev: "0.48"
-    hooks:
-      - id: check-manifest
-        stages: [manual]
```

### Comparing `itkdb-0.4.0rc9/generatePlots.py` & `itkdb-0.4.1rc1/generatePlots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # generatePlots.py -- generate plots of component numbers as a function of time in the ITkPD
 
 import logging
 
 import sys, os
 from collections import Counter
-from itkdb.utilities import colouredLogger
+from itkdb.utils import ColouredLogger
 from itkdb.core import Session
 
-logging.setLoggerClass(colouredLogger)
+logging.setLoggerClass(ColouredLogger)
 log = logging.getLogger('generatePlots')
 log.setLevel(logging.INFO)
 
 
 class PlotMaker(object):
     def __init__(self, session):
         self.session = session
```

### Comparing `itkdb-0.4.0rc9/getContentSummary.py` & `itkdb-0.4.1rc1/getContentSummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # getContentSummary.py -- a class providing an interface for getting component counts summary info from the ITk Production Database
 
 import logging
 import sys, datetime
 import click
 
-from itkdb.utilities import colours, colouredLogger
+from itkdb.utils import Colours, ColouredLogger
 from itkdb.core import Session
 
-logging.setLoggerClass(colouredLogger)
+logging.setLoggerClass(ColouredLogger)
 log = logging.getLogger('getContentSummary')
 log.setLevel(logging.INFO)
 
 # Define our cancel exception for &CANCEL calls
 class Cancel(Exception):
     pass
 
@@ -41,15 +41,15 @@
         log.info('Finished successfully.')
         sys.exit(0)
 
     # Print a list of names and codes in list (assuming it has those keys) with nice printing
     def __printNamesAndCodes(self, list):
         print(
             '    {0}{1}{2:<60} {3:<20}{4}'.format(
-                colours.BOLD_SEQ, colours.WHITE, 'Name:', 'Code:', colours.RESET_SEQ
+                Colours.BOLD_SEQ, Colours.WHITE, 'Name:', 'Code:', Colours.RESET_SEQ
             )
         )
         for item in list:
             print('    {0:<60} {1:<20}'.format(item['name'], item['code']))
 
     # Define a function to provide a prompt to the user and have them select from options
     # Used to get codes from the user, so options includes all possible codes for the current parameter
@@ -388,54 +388,54 @@
                 except Cancel:
                     break
 
                 # Report the specified parameters to the user
                 log.info('Using:\n')
                 print(
                     '    {0}{1}Project{2}        = {3}'.format(
-                        colours.BOLD_SEQ, colours.WHITE, colours.RESET_SEQ, project
+                        Colours.BOLD_SEQ, Colours.WHITE, Colours.RESET_SEQ, project
                     )
                 )
                 print(
                     '    {0}{1}Component type{2} = {3}'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
-                        colours.RESET_SEQ,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
+                        Colours.RESET_SEQ,
                         component_type,
                     )
                 )
                 print(
                     '    {0}{1}Types{2}          = {3}'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
-                        colours.RESET_SEQ,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
+                        Colours.RESET_SEQ,
                         ', '.join(types),
                     )
                 )
                 print(
                     '    {0}{1}Institutions{2}   = {3}'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
-                        colours.RESET_SEQ,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
+                        Colours.RESET_SEQ,
                         ', '.join(institutions),
                     )
                 )
                 print(
                     '    {0}{1}Lower date{2}     = {3}'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
-                        colours.RESET_SEQ,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
+                        Colours.RESET_SEQ,
                         '-'.join(date_lower),
                     )
                 )
                 print(
                     '    {0}{1}Upper date{2}     = {3}'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
-                        colours.RESET_SEQ,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
+                        Colours.RESET_SEQ,
                         '-'.join(date_upper),
                     )
                 )
                 log.info('Getting count information from the database.')
 
                 # Check if the component has stages
                 stages_DETAILED = component['stages']
@@ -591,18 +591,18 @@
 
                 # Print the count info, using alphabetically order for institution codes
                 for institution in sorted(component_counts.keys()):
                     if institution == 'TOTAL':
                         continue
                     print(
                         '    {0}{1}{2}{3}:'.format(
-                            colours.BOLD_SEQ,
-                            colours.WHITE,
+                            Colours.BOLD_SEQ,
+                            Colours.WHITE,
                             institution,
-                            colours.RESET_SEQ,
+                            Colours.RESET_SEQ,
                         )
                     )
 
                     # When printing the counts at each stage, print the stage codes in the order determined by stage_order
                     for number in sorted(stage_order.keys(), key=int):
                         print(
                             '        {0:<15} = {1}'.format(
@@ -615,15 +615,15 @@
                             'TOTAL', component_counts[institution]['TOTAL']
                         )
                     )
 
                 # Print overall counts
                 print(
                     '    {0}{1}{2}{3}:'.format(
-                        colours.BOLD_SEQ, colours.WHITE, 'TOTAL', colours.RESET_SEQ
+                        Colours.BOLD_SEQ, Colours.WHITE, 'TOTAL', Colours.RESET_SEQ
                     )
                 )
                 for number in sorted(stage_order.keys(), key=int):
                     print(
                         '        {0:<15} = {1}'.format(
                             stage_order[number],
                             component_counts['TOTAL'][stage_order[number]],
```

### Comparing `itkdb-0.4.0rc9/getInventory.py` & `itkdb-0.4.1rc1/getInventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # getInventory.py -- get a list of components specific to an institution from the ITkPD
 
 import argparse, sys, os, json, time
 import logging
 import click
 
-from itkdb.utilities import colours, colouredLogger
+from itkdb.utils import Colours, ColouredLogger
 from itkdb import Client
 
-logging.setLoggerClass(colouredLogger)
+logging.setLoggerClass(ColouredLogger)
 log = logging.getLogger('getContentSummary')
 log.setLevel(logging.INFO)
 
 # Define our inventory object
 class Inventory(object):
 
     # Read in our args
@@ -32,15 +32,15 @@
         with open(self.savePath, 'w') as file:
             json.dump(data, file)
 
     # Print a list of names and codes for a dictionary obtained from the ITkPD
     def __printNamesAndCodes(self, list):
         print(
             u'    {0}{1}{2:<60} {3:<20}{4}'.format(
-                colours.BOLD_SEQ, colours.WHITE, 'Name:', 'Code:', colours.RESET_SEQ
+                Colours.BOLD_SEQ, Colours.WHITE, 'Name:', 'Code:', Colours.RESET_SEQ
             )
         )
         for item in list:
             print(u'    {0:<60} {1:<20}'.format(item['name'], item['code']))
 
     # Generate a list of institutions (and save that list to json)
     def listInstitutions(self):
@@ -185,26 +185,26 @@
             'qaState': 'QA State',
         }
         form = '        {code:<40}{type:<15}{currentStage:<20}{dummy:<15}{currentGrade:<20}{reworked:<15}{trashed:<15}{assembled:<15}{qaPassed:<15}{qaState:<15}'
         for institution, componentTypes in inventory.items():
             for componentType, components in componentTypes.items():
                 print(
                     u'    {0}{1}{2} / {3} :{4}\n'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
                         institution,
                         componentType,
-                        colours.RESET_SEQ,
+                        Colours.RESET_SEQ,
                     )
                 )
                 print(
-                    colours.BOLD_SEQ
-                    + colours.WHITE
+                    Colours.BOLD_SEQ
+                    + Colours.WHITE
                     + form.format(**header)
-                    + colours.RESET_SEQ
+                    + Colours.RESET_SEQ
                 )
                 for component in components:
                     print(form.format(**component))
         if self.savePath != None:
             self.__save(
                 {
                     'timestamp': timestamp,
@@ -315,26 +315,26 @@
             'qaState': 'QA State',
         }
         form = '        {code:<40}{type:<15}{currentStage:<20}{dummy:<15}{currentGrade:<20}{assembled:<15}{qaPassed:<15}{qaState:<15}'
         for institution, componentTypes in inventory.items():
             for componentType, components in componentTypes.items():
                 print(
                     u'    {0}{1}{2} / {3} :{4}\n'.format(
-                        colours.BOLD_SEQ,
-                        colours.WHITE,
+                        Colours.BOLD_SEQ,
+                        Colours.WHITE,
                         institution,
                         componentType,
-                        colours.RESET_SEQ,
+                        Colours.RESET_SEQ,
                     )
                 )
                 print(
-                    colours.BOLD_SEQ
-                    + colours.WHITE
+                    Colours.BOLD_SEQ
+                    + Colours.WHITE
                     + form.format(**header)
-                    + colours.RESET_SEQ
+                    + Colours.RESET_SEQ
                 )
                 for component in components:
                     print(form.format(**component))
 
         # Confirm that the user wants to trash the filtered components
         if self.__getConfirm(
             'Please type \'confirm_trash\' to trash the above components or \'quit\' to cancel this action:',
```

### Comparing `itkdb-0.4.0rc9/registerComponent.py` & `itkdb-0.4.1rc1/registerComponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python
 # registerComponent.py -- interface for registering components in the ITk Production Database from the command line
 
 import logging
 import json
 import sys
 import click
-from itkdb.utilities import colours, colouredLogger
+from itkdb.utils import colours, ColouredLogger
 from itkdb.core import Session
 
-logging.setLoggerClass(colouredLogger)
+logging.setLoggerClass(ColouredLogger)
 log = logging.getLogger(__name__)
 log.setLevel(logging.INFO)
 
 # Define an exception for raising during &CANCEL calls
 class Cancel(Exception):
     pass
```

### Comparing `itkdb-0.4.0rc9/tbump.toml` & `itkdb-0.4.1rc1/tbump.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e34 2e30 7263 3922 0a0a  t = "0.4.0rc9"..
+00000010: 7420 3d20 2230 2e34 2e31 7263 3122 0a0a  t = "0.4.1rc1"..
 00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
 00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
 00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
 00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
 00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
 00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
 00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
@@ -15,15 +15,15 @@
 000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
 000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
 00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
 00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
 00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
 00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
 00000140: 2242 756d 7020 7665 7273 696f 6e3a 2030  "Bump version: 0
-00000150: 2e34 2e30 7263 3920 e286 9220 7b6e 6577  .4.0rc9 ... {new
+00000150: 2e34 2e31 7263 3120 e286 9220 7b6e 6577  .4.1rc1 ... {new
 00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
 00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
 00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
 00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
 000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
 000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
 000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
@@ -43,15 +43,30 @@
 000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
 000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
 000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
 000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
 000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
 000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
 00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
-00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
-00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
-00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
-00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
-00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
-00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
-00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
-00000380: 2222 0a                                  "".
+00000310: 5b5b 6669 6c65 5d5d 0a73 7263 203d 2022  [[file]].src = "
+00000320: 7079 7072 6f6a 6563 742e 746f 6d6c 220a  pyproject.toml".
+00000330: 7665 7273 696f 6e5f 7465 6d70 6c61 7465  version_template
+00000340: 203d 2022 7b6d 616a 6f72 7d2e 7b6d 696e   = "{major}.{min
+00000350: 6f72 7d22 0a73 6561 7263 6820 3d20 2269  or}".search = "i
+00000360: 746b 6462 2e64 6f63 732e 6365 726e 2e63  tkdb.docs.cern.c
+00000370: 682f 7b63 7572 7265 6e74 5f76 6572 7369  h/{current_versi
+00000380: 6f6e 7d22 0a0a 5b5b 6669 6c65 5d5d 0a73  on}"..[[file]].s
+00000390: 7263 203d 2022 7372 632f 6974 6b64 622f  rc = "src/itkdb/
+000003a0: 636c 6965 6e74 2e70 7922 0a76 6572 7369  client.py".versi
+000003b0: 6f6e 5f74 656d 706c 6174 6520 3d20 227b  on_template = "{
+000003c0: 6d61 6a6f 727d 2e7b 6d69 6e6f 727d 220a  major}.{minor}".
+000003d0: 7365 6172 6368 203d 2022 6974 6b64 622e  search = "itkdb.
+000003e0: 646f 6373 2e63 6572 6e2e 6368 2f7b 6375  docs.cern.ch/{cu
+000003f0: 7272 656e 745f 7665 7273 696f 6e7d 220a  rrent_version}".
+00000400: 0a5b 5b66 6965 6c64 5d5d 0a23 2074 6865  .[[field]].# the
+00000410: 206e 616d 6520 6f66 2074 6865 2066 6965   name of the fie
+00000420: 6c64 0a6e 616d 6520 3d20 2263 616e 6469  ld.name = "candi
+00000430: 6461 7465 220a 2320 7468 6520 6465 6661  date".# the defa
+00000440: 756c 7420 7661 6c75 6520 746f 2075 7365  ult value to use
+00000450: 2c20 6966 2074 6865 7265 2069 7320 6e6f  , if there is no
+00000460: 206d 6174 6368 0a64 6566 6175 6c74 203d   match.default =
+00000470: 2022 220a                                 "".
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/commandline.py` & `itkdb-0.4.1rc1/src/itkdb/commandline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,236 +1,290 @@
 from __future__ import annotations
 
 import json
 import logging
-import os
 import sys
+from pathlib import Path
 
 import click
 
-from . import core, settings, utilities
+from . import core, settings, utils
 from ._version import __version__
 
-logging.basicConfig(format=utilities.FORMAT_STRING, level=logging.INFO)
+logging.basicConfig(format=utils.FORMAT_STRING, level=logging.INFO)
 log = logging.getLogger(__name__)
 
 _session = core.Session()
 
 
-def project(func):
+def opt_project(func):
+    """
+    Click option for project.
+    """
     return click.option("--project", default="S", help="Project", show_default=True)(
         func
     )
 
 
-def component_type(func):
+def opt_component_type(func):
+    """
+    Click option for component type.
+    """
     return click.option(
         "--component-type",
         help="Code for the type of component to query. Run list-component-types to find what types are available.",
         show_default=True,
     )(func)
 
 
-def component_code(func):
+def opt_component_code(func):
+    """
+    Click option for component code.
+    """
     return click.option(
         "--component", help="Component code or component serial number", required=True
     )(func)
 
 
-@click.group(context_settings=dict(help_option_names=["-h", "--help"]))
+@click.group(context_settings={"help_option_names": ["-h", "--help"]})
 @click.version_option(version=__version__)
 @click.option(
-    "--accessCode1",
+    "--access-code1",
     prompt=not (bool(settings.ITKDB_ACCESS_CODE1)),
     default=settings.ITKDB_ACCESS_CODE1,
     show_default=True,
 )
 @click.option(
-    "--accessCode2",
+    "--access-code2",
     prompt=not (bool(settings.ITKDB_ACCESS_CODE2)),
     default=settings.ITKDB_ACCESS_CODE2,
     show_default=True,
 )
 @click.option("--auth-url", default=settings.ITKDB_AUTH_URL, show_default=True)
 @click.option("--site-url", default=settings.ITKDB_SITE_URL, show_default=True)
 @click.option(
     "--save-auth",
     help="Filename to save authenticated user to for persistence between requests",
     default=".auth",
+    type=click.Path(path_type=Path, exists=False, writable=True, resolve_path=True),
 )
-def itkdb(accesscode1, accesscode2, auth_url, site_url, save_auth):
-    global _session
+def itkdb(access_code1, access_code2, auth_url, site_url, save_auth):
+    """
+    Top-level pass-through.
+    """
     _session.prefix_url = site_url
-    _session.user._prefix_url = auth_url
-    _session.user._accessCode1 = accesscode1
-    _session.user._accessCode2 = accesscode2
-    _session.user._save_auth = save_auth
-    _session.user._load()
+    _session.user._prefix_url = auth_url  # pylint: disable=protected-access
+    _session.user._access_code1 = access_code1  # pylint: disable=protected-access
+    _session.user._access_code2 = access_code2  # pylint: disable=protected-access
+    _session.user._save_auth = save_auth  # pylint: disable=protected-access
+    _session.user._load()  # pylint: disable=protected-access
 
 
 @itkdb.command()
 def authenticate():
+    """
+    Authenticate using the provided access codes (environment variable or command line).
+    """
     _session.user.authenticate()
     click.echo(
-        "You have signed in as {}. Your token expires in {}s.".format(
-            _session.user.name, _session.user.expires_in
-        )
+        "You have signed in as {_session.user.name}. Your token expires in {_session.user.expires_in}s."
     )
 
 
 @itkdb.command()
 def stats():
+    """
+    List overall statistics for ITk Production Database.
+    """
     click.echo(
         json.dumps(
             _session.get("getItkpdOverallStatistics").json()["statistics"], indent=2
         )
     )
     sys.exit(0)
 
 
 @itkdb.command()
 def list_institutes():
+    """
+    List all institutions.
+    """
     click.echo(
         json.dumps(_session.get("listInstitutions").json()["pageItemList"], indent=2)
     )
     sys.exit(0)
 
 
 # NB: list_component_type_codes is the same as this, but use jq
 #  $ itkdb list-component-types --project P | jq '[.[] | {code: .code, name: .name}]'
 @itkdb.command()
-@project
+@opt_project
 def list_component_types(project):
+    """
+    List component types for a project.
+    """
     data = {"project": project}
     click.echo(
         json.dumps(
             _session.get("listComponentTypes", json=data).json()["pageItemList"],
             indent=2,
         )
     )
     sys.exit(0)
 
 
 @itkdb.command()
-@project
-@component_type
+@opt_project
+@opt_component_type
 def list_components(project, component_type):
+    """
+    List components registered for a given component type.
+    """
     data = {"project": project}
     if component_type:
         data.update({"componentType": component_type})
     click.echo(
         json.dumps(
             _session.get("listComponents", json=data).json()["itemList"], indent=2
         )
     )
     sys.exit(0)
 
 
 # currently broken FYI
 @itkdb.command()
 def list_all_attachments():
+    """
+    List all attachments physically stored in the ITk Production Database.
+    """
     click.echo(
         json.dumps(
             _session.get("uu-app-binarystore/listBinaries").json()["itemList"], indent=2
         )
     )
     sys.exit(0)
 
 
 @itkdb.command()
 def list_projects():
+    """
+    List the projects.
+    """
     click.echo(json.dumps(_session.get("listProjects").json()["itemList"], indent=2))
     sys.exit(0)
 
 
 @itkdb.command()
-@project
-@component_type
+@opt_project
+@opt_component_type
 def list_test_types(project, component_type):
+    """
+    List the test types for a component type.
+    """
     data = {"project": project, "componentType": component_type}
     click.echo(
         json.dumps(
             _session.get("listTestTypes", json=data).json()["pageItemList"], indent=2
         )
     )
     sys.exit(0)
 
 
 @itkdb.command()
-@component_code
+@opt_component_code
 def get_component_info(component):
+    """
+    Get information about a component.
+    """
     data = {"component": component}
     click.echo(json.dumps(_session.get("getComponent", json=data).json(), indent=2))
     sys.exit(0)
 
 
 @itkdb.command()
-@project
+@opt_project
 def summary(project):
+    """
+    Summarize some information about institutions, component types, and test types per component.
+    """
     header_str = "====={0:^100s}====="
     click.echo(header_str.format("Institutes"))
     institutes = _session.get("listInstitutions").json()["pageItemList"]
     for institute in institutes:
-        click.echo("{name} ({code})".format(**institute))
+        click.echo(f"{institute['name']} ({institute['code']})")
 
     click.echo(header_str.format("Strip component types"))
-    componentTypes = _session.get(
+    component_types = _session.get(
         "listComponentTypes", json={"project": project}
     ).json()["pageItemList"]
 
-    for componentType in componentTypes:
-        click.echo("{name} ({code}) {state}".format(**componentType))
+    for component_type in component_types:
+        click.echo(
+            f"{component_type['name']} ({component_type['code']}) {component_type['state']}"
+        )
 
     click.echo(header_str.format("Test types by component"))
-    for componentType in componentTypes:
-        click.echo("Test types for {code}".format(**componentType))
+    for component_type in component_types:
+        click.echo(f"Test types for {component_type['code']}")
         test_types = _session.get(
             "listTestTypes",
-            json={"project": project, "componentType": componentType["code"]},
+            json={"project": project, "componentType": component_type["code"]},
         ).json()["pageItemList"]
         for test_type in test_types:
-            click.echo("  {name} ({code}) {state}".format(**test_type))
+            click.echo(
+                f"  {test_type['name']} ({test_type['code']}) {test_type['state']}"
+            )
 
 
 @itkdb.command()
-@component_code
+@opt_component_code
 @click.option("--title", help="Short description", required=True)
 @click.option("-d", "--description", help="Description of attachment", required=True)
 @click.option(
-    "-f", "--file", help="File to attach", required=True, type=click.Path(exists=True)
+    "-f",
+    "--file",
+    help="File to attach",
+    required=True,
+    type=click.Path(path_type=Path, exists=True),
 )
 @click.option("--filename", help="If specified, override filename of attachment")
 @click.option(
     "--file-type", help="The type of the file being uploaded", default="text/plain"
 )
 def add_attachment(component, title, description, file, filename, file_type):
-    filename = filename if filename else os.path.basename(file)
+    """
+    Add an attachment to a component.
+    """
+    filename = filename if filename else file.name
 
     data = {
         "component": component,
         "title": title,
         "description": description,
         "type": "file",
         "url": filename,
     }
-    with open(file, "rb") as fp:
-        attachment = {"data": (filename, fp, file_type)}
+    with file.open("rb") as fpointer:
+        attachment = {"data": (filename, fpointer, file_type)}
         click.echo(
             json.dumps(
                 _session.post(
                     "createComponentAttachment", data=data, files=attachment
                 ).json(),
                 indent=2,
             )
         )
     sys.exit(0)
 
 
 @itkdb.command()
-@component_code
+@opt_component_code
 @click.option("-m", "--message", help="Comment to add to component", required=True)
 def add_comment(component, message):
+    """
+    Add a comment to a component.
+    """
     data = {"component": component, "comments": [message]}
     click.echo(
         json.dumps(_session.post("createComponentComment", json=data).json(), indent=2)
     )
     sys.exit(0)
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/core.py` & `itkdb-0.4.1rc1/src/itkdb/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,101 +1,111 @@
 from __future__ import annotations
 
 import logging
-import os
 import pickle  # nosec
 import time
+from pathlib import Path
 
 import cachecontrol.caches.file_cache
 import requests
 from cachecontrol.heuristics import ExpiresAfter
 from jose import jwt
 from requests.status_codes import codes
 
-from . import exceptions
-from ._version import __version__
-from .caching import CacheControlAdapter, CacheController
-from .settings import settings
+from itkdb import exceptions
+from itkdb._version import __version__
+from itkdb.caching import CacheControlAdapter, CacheController
+from itkdb.settings import settings
 
 log = logging.getLogger(__name__)
 
 
 class User:
+    """
+    Class for managing user tokens and authentication flow.
+
+    Args:
+        access_code1 (str): ITkPD Access Code 1
+        access_code2 (str): ITkPD Access Code 2
+        audience (str): ITkPD OIDC Audience
+        prefix_url (str): The prefix for all non-absolute URIs
+        jwt_options (dict): Additional JWT options to pass through
+        save_auth (pathlib.Path | str | None): If set, save authentication information to the file path specified
+
+    !!! note "Changed in version 0.4.0"
+        - renamed `accessCode1` / `accessCode2` to `access_code1` / `access_code2`
+
+    """
+
     def __init__(
         self,
-        accessCode1=settings.ITKDB_ACCESS_CODE1,
-        accessCode2=settings.ITKDB_ACCESS_CODE2,
+        access_code1=settings.ITKDB_ACCESS_CODE1,
+        access_code2=settings.ITKDB_ACCESS_CODE2,
         audience=settings.ITKDB_ACCESS_AUDIENCE,
         prefix_url=settings.ITKDB_AUTH_URL,
-        jwtOptions=None,
-        save_auth=None,
+        jwt_options=None,
+        save_auth: Path | str | None = None,
     ):
-
         # session handling (for injection in tests)
         self._session = requests.Session()
         self._session.headers.update({"User-Agent": f"itkdb/{__version__}"})
         # store last call to authenticate
         self._response = None
         self._status_code = None
         # store jwks for validation/verification
         self._jwks = None
         # store information after authorization occurs
         self._access_token = None
         self._raw_id_token = None
         self._id_token = None
         # initialization configuration
-        self._accessCode1 = accessCode1
-        self._accessCode2 = accessCode2
+        self._access_code1 = access_code1
+        self._access_code2 = access_code2
         self._audience = audience
         self._prefix_url = prefix_url
-        # update jwtOptions if provided
-        self._jwtOptions = {"leeway": 2}  # **jwtOptions, python3 only
-        self._jwtOptions.update(jwtOptions or {})
+        # update jwt_options if provided
+        self._jwt_options = {
+            "leeway": int(settings.ITKDB_LEEWAY)
+        }  # **jwt_options, python3 only
+        self._jwt_options.update(jwt_options or {})
         # serialization/persistence
-        self._save_auth = save_auth
+        self._save_auth: Path | None = Path(save_auth) if save_auth else None
         self._load()
 
     def _load(self):
-        if self._save_auth and os.path.isfile(self._save_auth):
+        if self._save_auth and self._save_auth.is_file():
             try:
-                with open(self._save_auth, "rb") as _pickle_file:
+                with self._save_auth.open("rb") as _pickle_file:
                     saved_user = pickle.load(_pickle_file)  # nosec
                 if saved_user.is_expired():
                     log.warning(
-                        "Saved user session is expired in {}. Creating a new one.".format(
-                            self._save_auth
-                        )
+                        "Saved user session is expired in %s. Creating a new one.",
+                        self._save_auth,
                     )
                     return False
                 if saved_user.is_authenticated():
                     self.__dict__.update(saved_user.__dict__)
                     return True
             except pickle.UnpicklingError:
                 log.warning(
-                    "Unable to load user session from {}. Creating a new one.".format(
-                        self._save_auth
-                    )
-                )
-            except KeyError:  # python2 specific error
-                log.warning(
-                    "Unable to load user session from {}. Creating a new one.".format(
-                        self._save_auth
-                    )
+                    "Unable to load user session from %s. Creating a new one.",
+                    self._save_auth,
                 )
         return False
 
-    def _dump(self):
+    def _dump(self) -> bool:
         if self.is_authenticated() and not self.is_expired() and self._save_auth:
-            with open(self._save_auth, "wb") as fp:
+            with self._save_auth.open("wb") as fpointer:
                 try:
-                    pickle.dump(self, fp, pickle.HIGHEST_PROTOCOL)
+                    pickle.dump(self, fpointer, pickle.HIGHEST_PROTOCOL)
                     return True
                 except (pickle.PicklingError, AttributeError, TypeError):
-                    log.warning(f"Unable to save user session to {self._save_auth}.")
+                    log.warning("Unable to save user session to %s.", self._save_auth)
             return False
+        return False
 
     def _load_jwks(self, force=False):
         if self._jwks is None or force:
             self._jwks = self._session.get(
                 "https://uuidentity.plus4u.net/uu-oidc-maing02/bb977a99f4cc4c37a2afce3fd599d0a7/oidc/listKeys"
             ).json()
 
@@ -103,102 +113,159 @@
         if self._raw_id_token:
             self._load_jwks()
             self._id_token = jwt.decode(
                 self._raw_id_token,
                 self._jwks,
                 algorithms="RS256",
                 audience=self._audience,
-                options=self._jwtOptions,
+                options=self._jwt_options,
             )
 
-    def authenticate(self):
+    def authenticate(self) -> bool:
+        """
+        Authenticate the current user if not already authenticated.
+
+        If the current user session is expired, this will attempt to reauthenticate.
+        """
         # if not expired, do nothing
         if self.is_authenticated():
             if not self.is_expired():
                 return True
             log.warning("User session is expired. Creating a new one.")
 
         # session-less request
         response = self._session.post(
             requests.compat.urljoin(self._prefix_url, "grantToken"),
             json={
                 "grant_type": "password",
-                "accessCode1": self._accessCode1,
-                "accessCode2": self._accessCode2,
+                "accessCode1": self._access_code1,
+                "accessCode2": self._access_code2,
                 "scope": settings.ITKDB_ACCESS_SCOPE,
             },
         )
         self._response = response
         self._status_code = response.status_code
         self._access_token = response.json().get("access_token")
         self._raw_id_token = response.json().get("id_token")
         self._id_token = None
 
         # handle parsing the id token
         self._parse_id_token()
 
         if not self.is_authenticated():
             raise exceptions.ResponseException(self._response)
-        else:
-            self._dump()
+
+        self._dump()
+        return True
 
     @property
-    def accessCode1(self):
-        return self._accessCode1
+    def access_code1(self) -> str:
+        """
+        The first access code.
+        """
+        return self._access_code1
 
     @property
-    def accessCode2(self):
-        return self._accessCode2
+    def access_code2(self) -> str:
+        """
+        The second access code.
+        """
+        return self._access_code2
 
     @property
-    def access_token(self):
+    def access_token(self) -> str:
+        """
+        The opaque access token for the user.
+        """
         return self._access_token
 
     @property
-    def id_token(self):
+    def id_token(self) -> dict[str, str | list[str] | int]:
+        """
+        The parsed JWT identity token for the user.
+        """
         return self._id_token if self._id_token else {}
 
     @property
-    def name(self):
+    def name(self) -> str:
+        """
+        The name for the user.
+        """
         return self.id_token.get("name", "")
 
     @property
-    def expires_at(self):
+    def expires_at(self) -> int:
+        """
+        The Epoch Unix Timestamp that the user session expires at.
+        """
         return self.id_token.get("exp", 0)
 
     @property
-    def expires_in(self):
+    def expires_in(self) -> int:
+        """
+        The time until expiration in seconds.
+        """
         expires_in = self.expires_at - time.time()
         return 0 if expires_in < 0 else int(expires_in)
 
     @property
-    def identity(self):
+    def identity(self) -> str:
+        """
+        The identity for the user in the ITk Production Database.
+        """
         return self.id_token.get("uuidentity", "")
 
     @property
-    def bearer(self):
+    def bearer(self) -> str:
+        """
+        The bearer token for the user.
+        """
         return self._raw_id_token if self._raw_id_token else ""
 
-    def is_authenticated(self):
+    def is_authenticated(self) -> bool:
+        """
+        Whether current user is authenticated.
+        """
         return bool(
             self._status_code == codes["ok"]
             and self._access_token
             and self._raw_id_token
         )
 
-    def is_expired(self):
-        return not (self.expires_in > 0)
+    def is_expired(self) -> bool:
+        """
+        Whether current user session is expired.
+        """
+        return not self.expires_in > 0
 
     def __repr__(self):
-        return "{:s}(name={:s}, expires_in={:d}s)".format(
-            self.__class__.__name__, self.name, self.expires_in
-        )
+        return f"{self.__class__.__name__:s}(name={self.name:s}, expires_in={self.expires_in:d}s)"
 
 
 class Session(requests.Session):
+    """
+    Lightweight wrapper around `requests.Session` with basic error-handling, auto-(re)authentication, and URI prefixing.
+
+    For more information, see python requests.
+
+    Attributes:
+        STATUS_EXCEPTIONS (dict): Mapping from status code to [itkdb.exceptions][]
+        SUCCESS_STATUSES (dict): List of status codes that are OK
+        auth (callable): Call [itkdb.core.Session.authorize][]
+        prefix_url (str): The prefix for all non-absolute URIs
+        user (itkdb.core.User): The user object for authentication
+
+    Args:
+        user (itkdb.core.User): A user object. Create one if not specified.
+        prefix_url (str): The prefix url to use for all requests.
+        save_auth (pathlib.Path | str | None): A file path to where to save authentication information.
+        cache (str): A CacheControl.caches object for cache (default: cachecontrol.caches.file_cache.FileCache). Set to False to disable cache.
+        expires_after (dict): The arguments are the same as the datetime.timedelta object. This will override or add the Expires header and override or set the Cache-Control header to public.
+    """
+
     STATUS_EXCEPTIONS = {
         codes["bad_gateway"]: exceptions.ServerError,
         codes["bad_request"]: exceptions.BadRequest,
         codes["conflict"]: exceptions.Conflict,
         codes["found"]: exceptions.Redirect,
         codes["forbidden"]: exceptions.Forbidden,
         codes["gateway_timeout"]: exceptions.ServerError,
@@ -210,56 +277,52 @@
         codes["unauthorized"]: exceptions.Forbidden,
         codes["unavailable_for_legal_reasons"]: exceptions.UnavailableForLegalReasons,
     }
     SUCCESS_STATUSES = {codes["created"], codes["ok"]}
 
     def __init__(
         self,
-        user=None,
+        user: User = None,
         prefix_url=settings.ITKDB_SITE_URL,
-        save_auth=None,
-        cache=True,
+        save_auth: Path | str | None = None,
+        cache: bool = True,
         expires_after=None,
     ):
-        """
-        user (itkdb.core.User): A user object. Create one if not specified.
-        prefix_url (str): The prefix url to use for all requests.
-        save_auth (str): A file path to where to save authentication information.
-        cache (str): A CacheControl.caches object for cache (default: cachecontrol.caches.file_cache.FileCache). Set to False to disable cache.
-        expires_after (dict): The arguments are the same as the datetime.timedelta object. This will override or add the Expires header and override or set the Cache-Control header to public.
-        """
         super().__init__()
         self.headers.update({"User-Agent": f"itkdb/{__version__}"})
         self.user = user if user else User(save_auth=save_auth)
-        self.auth = self._authorize
+        self.auth = self.authorize
         self.prefix_url = prefix_url
         # store last call
         self._response = None
 
         cache_options = {}
         if cache:
             cache = (
                 cachecontrol.caches.file_cache.FileCache(".webcache")
                 if cache is True
                 else cache
             )
-            cache_options.update(dict(cache=cache))
+            cache_options.update({"cache": cache})
 
         # handle expirations for cache
         if expires_after and isinstance(expires_after, dict):
-            cache_options.update(dict(heuristic=ExpiresAfter(**expires_after)))
+            cache_options.update({"heuristic": ExpiresAfter(**expires_after)})
 
         if cache_options:
             # add caching
             super().mount(
                 self.prefix_url,
                 CacheControlAdapter(controller_class=CacheController, **cache_options),
             )
 
-    def _authorize(self, req):
+    def authorize(self, req):
+        """
+        Add authentication information to the request by updating the headers.
+        """
         if req.url.startswith(settings.ITKDB_SITE_URL):
             self.user.authenticate()
             req.headers.update({"Authorization": f"Bearer {self.user.bearer:s}"})
         return req
 
     def _normalize_url(self, url):
         return requests.compat.urljoin(self.prefix_url, url)
@@ -277,23 +340,23 @@
         request.url = self._normalize_url(request.url)
         return super().prepare_request(request)
 
     def send(self, request, **kwargs):
         response = super().send(request, **kwargs)
         self._response = response
         log.debug(
-            "Response: {} ({} bytes)".format(
-                response.status_code, response.headers.get("content-length")
-            )
+            "Response: %s (%s bytes)",
+            response.status_code,
+            response.headers.get("content-length"),
         )
         self._check_response(response)
         return response
 
     def request(self, method, url, *args, **kwargs):
         url = self._normalize_url(url)
         return super().request(method, url, *args, **kwargs)
 
     def __call__(self, *args, **kwargs):
         if len(args) == 1:
             return self.send(self.prepare_request(*args), **kwargs)
-        else:
-            return self.request(*args, **kwargs)
+
+        return self.request(*args, **kwargs)
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/exceptions.py` & `itkdb-0.4.1rc1/src/itkdb/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 """Provide exception classes for the itkdb package."""
 
 from __future__ import annotations
 
 import json
 import sys
+from contextlib import suppress
 
-from .utilities import pretty_print
+from .utils import pretty_print
 
 try:
     from json.decoder import JSONDecodeError
 except ImportError:
     JSONDecodeError = ValueError
 
 try:
     from html2text import html2text
 except ImportError:
 
-    def html2text(x):
-        return x
+    def html2text(string):
+        """
+        Pass-through function.
+        """
+        return string
 
 
 if sys.version_info[0] == 2:
     from urlparse import urlparse
 else:
     from urllib.parse import urlparse
 
@@ -38,31 +42,29 @@
     """Indicate that there was an error with the completed HTTP request."""
 
     def __init__(self, response, additional_message=None):
         """Initialize a ResponseException instance.
         :param response: A requests.response instance.
         """
         self.response = response
-        message = "received {} HTTP response for following request\n{}".format(
-            response.status_code, pretty_print(response.request)
-        )
+        message = f"received {response.status_code} HTTP response for following request\n{pretty_print(response.request)}"
 
         try:
             if additional_message is None:
                 additional_message = json.dumps(response.json(), indent=2)
 
         except JSONDecodeError:
             additional_message = response.text.strip()
 
         if additional_message:
-            if "text/html" in response.headers["content-type"]:
+            if "text/html" in response.headers.get("content-type", ""):
                 additional_message = html2text(additional_message)
 
-            message = "{}\n\nThe following details may help:\n{}".format(
-                message, additional_message
+            message = (
+                f"{message}\n\nThe following details may help:\n{additional_message}"
             )
         super().__init__(message)
 
 
 class BadJSON(ResponseException):
     """Indicate the response did not contain valid JSON."""
 
@@ -76,23 +78,22 @@
 
 
 class Forbidden(ResponseException):
     """Indicate the authentication is not permitted for the request."""
 
     def __init__(self, response):
         additional_message = None
-        try:
+
+        with suppress(JSONDecodeError):
             additional_message = (
                 response.json()
                 .get("uuAppErrorMap", {})
                 .get("uu-app-workspace/authorization/userIsNotAuthorized", {})
                 .get("message", None)
             )
-        except JSONDecodeError:
-            pass
         super().__init__(response, additional_message)
 
 
 class NotFound(ResponseException):
     """Indicate that the requested URL was not found."""
 
 
@@ -110,15 +111,15 @@
         :param response: A requests.response instance containing a location
         header.
 
         """
         path = urlparse(response.headers["location"]).path
         self.path = path[:-5] if path.endswith(".json") else path
         self.response = response
-        ITkDBException.__init__(self, f"Redirect to {self.path}")
+        super().__init__(f"Redirect to {self.path}")
 
 
 class ServerError(ResponseException):
     """Indicate issues on the server end preventing request fulfillment."""
 
 
 class SpecialError(ResponseException):
@@ -133,15 +134,15 @@
         """
         self.response = response
 
         resp_dict = self.response.json()  # assumes valid JSON
         self.message = resp_dict.get("message", "")
         self.reason = resp_dict.get("reason", "")
         self.special_errors = resp_dict.get("special_errors", [])
-        ITkDBException.__init__(self, f"Special error {self.message!r}")
+        super().__init__(f"Special error {self.message!r}")
 
 
 class TooLarge(ResponseException):
     """Indicate that the request data exceeds the allowed limit."""
 
 
 class UnavailableForLegalReasons(ResponseException):
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/responses.py` & `itkdb-0.4.1rc1/src/itkdb/responses.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,42 +3,91 @@
 import json
 import logging
 
 log = logging.getLogger(__name__)
 
 
 class PagedResponse:
+    """
+    A generator that handles paginated responses by requesting the next page as you need it.
+    """
+
     def __init__(self, session, response, limit=-1, key="pageItemList"):
         self._pages = []
         self._session = session
         self._load(response)
         self.yielded = 0
         self.limit = limit if limit and limit > 0 else self.total
         self.key = key
 
     @property
-    def pages(self):
+    def pages(self) -> list:
+        """
+        A list of pages fetched.
+        """
         return self._pages
 
     @property
-    def last_page(self):
+    def last_page(self) -> dict:
+        """
+        The most recent page retrieved.
+        """
         return self.pages[-1]
 
     @property
-    def data(self):
+    def data(self) -> dict | list[dict]:
+        """
+        The data contained on the most recent page retrieved.
+        """
         return self.last_page.get(self.key)
 
+    @property
+    def error(self) -> dict:
+        """
+        The uuAppErrorMap for the current page.
+        """
+        return self.last_page.get("uuAppErrorMap", {})
+
+    @property
+    def page_info(self) -> dict:
+        """
+        The pageInfo for the current page.
+        """
+        return self.last_page.get("pageInfo", {})
+
+    @property
+    def page_index(self) -> int:
+        """
+        The pageIndex for the current page.
+
+        If there is no pageIndex, returns -1.
+        """
+        return self.page_info.get("pageIndex", -1)
+
+    @property
+    def page_size(self) -> int:
+        """
+        The pageSize for the current page.
+
+        If there is no pageSize, returns -1.
+        """
+        return self.page_info.get("pageSize", -1)
+
+    @property
+    def total(self) -> int:
+        """
+        The total number of items (reported from the current page).
+
+        If there is no total, returns -1.
+        """
+        return self.page_info.get("total", -1)
+
     def _load(self, response):
         self._response = response
         self._pages.append(response.json())
-        self.error = self.last_page.get("uuAppErrorMap")
-        self.page_info = self.last_page.get("pageInfo", {})
-        self.page_index = self.page_info.get("pageIndex")
-        self.page_size = self.page_info.get("pageSize")
-        self.total = self.page_info.get("total")
         # nb: list_index is only for the last page
         self._list_index = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
@@ -51,22 +100,14 @@
         self._list_index += 1
         self.yielded += 1
         return self.data[self._list_index - 1]
 
     def __bool__(self):
         return bool(self.total)
 
-    # python2 compatibility
-    def __nonzero__(self):
-        return self.__bool__()
-
-    # python2 compatibility
-    def next(self):
-        return self.__next__()
-
     def _next_page(self):
         body = json.loads(self._response.request.body)
         body.update(
             {"pageInfo": {"pageIndex": self.page_index + 1, "pageSize": self.page_size}}
         )
         self._response.request.prepare_body(data=None, files=None, json=body)
         response = self._session.send(self._response.request)
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/caching/adapter.py` & `itkdb-0.4.1rc1/src/itkdb/caching/adapter.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from cachecontrol.adapter import CacheControlAdapter as BaseAdapter
 from cachecontrol.filewrapper import CallbackFileWrapper
 
 from . import utils
 
 
 class CacheControlAdapter(BaseAdapter):
+    """
+    Adapter for handling cache requests.
+    """
+
     invalidating_methods = {"POST", "PUT", "DELETE"}
 
     def build_response(
         self, request, response, from_cache=False, cacheable_methods=None
     ):
         """
         Build a response by making a request or using the cache.
@@ -51,28 +55,31 @@
 
             # We always cache the 301 responses
             elif response.status == 301:
                 self.controller.cache_response(request, response)
             else:
                 # Wrap the response file with a wrapper that will cache the
                 #   response when the stream has been consumed.
-                response._fp = CallbackFileWrapper(
-                    response._fp,
+                response._fp = CallbackFileWrapper(  # pylint: disable=protected-access
+                    response._fp,  # pylint: disable=protected-access
                     functools.partial(
                         self.controller.cache_response, request, response
                     ),
                 )
                 if response.chunked:
-                    super_update_chunk_length = response._update_chunk_length
+                    super_update_chunk_length = (
+                        response._update_chunk_length  # pylint: disable=protected-access
+                    )
 
                     def _update_chunk_length(self):
                         super_update_chunk_length()
                         if self.chunk_left == 0:
-                            self._fp._close()
+                            self._fp._close()  # pylint: disable=protected-access
 
+                    # pylint: disable-next=protected-access
                     response._update_chunk_length = types.MethodType(
                         _update_chunk_length, response
                     )
 
         resp = super().build_response(request, response)
 
         # See if we should invalidate the cache.
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/caching/controller.py` & `itkdb-0.4.1rc1/src/itkdb/caching/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,29 +10,33 @@
 
 from . import utils
 
 logger = logging.getLogger(__name__)
 
 
 class CacheController(BaseController):
+    """
+    Controller for handling caching.
+    """
+
     def cached_request(self, request):
         """
         Return a cached response if it exists in the cache, otherwise
         return False.
         """
         cache_url = self.cache_url(utils.build_url(request))
         logger.debug('Looking up "%s" in the cache', cache_url)
-        cc = self.parse_cache_control(request.headers)
+        cc_headers = self.parse_cache_control(request.headers)
 
         # Bail out if the request insists on fresh data
-        if "no-cache" in cc:
+        if "no-cache" in cc_headers:
             logger.debug('Request header has "no-cache", cache bypassed')
             return False
 
-        if "max-age" in cc and cc["max-age"] == 0:
+        if "max-age" in cc_headers and cc_headers["max-age"] == 0:
             logger.debug('Request header has "max_age" as 0, cache bypassed')
             return False
 
         # Request allows serving from the cache, let's see if we find something
         cache_data = self.cache.get(cache_url)
         if cache_data is None:
             logger.debug("No cache entry available")
@@ -95,22 +99,22 @@
             if expires is not None:
                 expire_time = calendar.timegm(expires) - date
                 freshness_lifetime = max(0, expire_time)
                 logger.debug("Freshness lifetime from expires: %i", freshness_lifetime)
 
         # Determine if we are setting freshness limit in the
         # request. Note, this overrides what was in the response.
-        if "max-age" in cc:
-            freshness_lifetime = cc["max-age"]
+        if "max-age" in cc_headers:
+            freshness_lifetime = cc_headers["max-age"]
             logger.debug(
                 "Freshness lifetime from request max-age: %i", freshness_lifetime
             )
 
-        if "min-fresh" in cc:
-            min_fresh = cc["min-fresh"]
+        if "min-fresh" in cc_headers:
+            min_fresh = cc_headers["min-fresh"]
             # adjust our current age by our min fresh
             current_age += min_fresh
             logger.debug("Adjusted current age from min-fresh: %i", current_age)
 
         # Return entry if it is fresh enough
         if freshness_lifetime > current_age:
             logger.debug('The response is "fresh", returning cached response')
@@ -166,22 +170,22 @@
             and "content-length" in response_headers
             and response_headers["content-length"].isdigit()
             and int(response_headers["content-length"]) != len(body)
         ):
             return
 
         cc_req = self.parse_cache_control(request.headers)
-        cc = self.parse_cache_control(response_headers)
+        cc_headers = self.parse_cache_control(response_headers)
 
         cache_url = self.cache_url(utils.build_url(request))
         logger.debug('Updating cache with response from "%s"', cache_url)
 
         # Delete it from the cache if we happen to have it stored there
         no_store = False
-        if "no-store" in cc:
+        if "no-store" in cc_headers:
             no_store = True
             logger.debug('Response header has "no-store"')
         if "no-store" in cc_req:
             no_store = True
             logger.debug('Request header has "no-store"')
         if no_store and self.cache.get(cache_url):
             logger.debug('Purging existing cache entry to honor "no-store"')
@@ -212,28 +216,27 @@
             self.cache.set(cache_url, self.serializer.dumps(request, response))
 
         # Add to the cache if the response headers demand it. If there
         # is no date header then we can't do anything about expiring
         # the cache.
         elif "date" in response_headers:
             # cache when there is a max-age > 0
-            if "max-age" in cc and cc["max-age"] > 0:
+            if "max-age" in cc_headers and cc_headers["max-age"] > 0:
                 logger.debug("Caching b/c date exists and max-age > 0")
                 self.cache.set(
                     cache_url, self.serializer.dumps(request, response, body=body)
                 )
 
             # If the request can expire, it means we should cache it
             # in the meantime.
-            elif "expires" in response_headers:
-                if response_headers["expires"]:
-                    logger.debug("Caching b/c of expires header")
-                    self.cache.set(
-                        cache_url, self.serializer.dumps(request, response, body=body)
-                    )
+            elif "expires" in response_headers and response_headers["expires"]:
+                logger.debug("Caching b/c of expires header")
+                self.cache.set(
+                    cache_url, self.serializer.dumps(request, response, body=body)
+                )
 
     def update_cached_response(self, request, response):
         """On a 304 we will get a new set of headers that we want to
         update our cached value with, assuming we have one.
         This should only ever be called when we've sent an ETag and
         gotten a 304 as the response.
         """
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/caching/utils.py` & `itkdb-0.4.1rc1/src/itkdb/caching/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,19 +9,20 @@
     # Python 2
     from urllib import urlencode
 
     from urlparse import urlparse
 
 
 def build_url(request):
+    """
+    Build the url including the query params + body, encoding as needed
+    """
     if request.body:
         parsed = urlparse(request.url)
         if request.headers.get("content-type") == "application/json":
             parsed_body = json.loads(request.body)
         else:
             parsed_body = request.body
         query = "&".join([parsed.query, urlencode({"body": parsed_body})])
         # return '{parsed.scheme}://{parsed.netloc}{parsed.path}?{query}'
-        return "{:s}://{:s}{:s}?{:s}".format(
-            parsed.scheme, parsed.netloc, parsed.path, query
-        )
+        return f"{parsed.scheme:s}://{parsed.netloc:s}{parsed.path:s}?{query:s}"
     return request.url
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/data/1x1.sh` & `itkdb-0.4.1rc1/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/src/itkdb/data/README.md` & `itkdb-0.4.1rc1/src/itkdb/data/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,7 +34,16 @@
 
 A 1x1 pixel image is used for testing image uploads in the database. This is
 done via `1x1.sh` and `1x1.jpg` which should be good enough integration testing.
 
 See
 [stackoverflow](https://stackoverflow.com/questions/2253404/what-is-the-smallest-valid-jpeg-file-size-in-bytes)
 for where this came from.
+
+## ROOT
+
+A small ROOT file `tiny.root` is used for testing identification of ROOT files.
+This was created via `ROOT`:
+
+```
+TFile::Open("tiny.root", "NEW")
+```
```

### Comparing `itkdb-0.4.0rc9/src/itkdb/models/institution.py` & `itkdb-0.4.1rc1/src/itkdb/models/institution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,139 @@
 from __future__ import annotations
 
 import attr
 
 
 def make_item(data):
+    """
+    make Item.
+    """
     return Item(code=data["code"], id=data["id"], name=data["name"])
 
 
 def make_component_type(data):
+    """
+    make ComponentType.
+    """
     return ComponentType(
         name=data["name"],
         code=data["code"],
-        itemList=list(map(make_item, data["itemList"])),
+        item_list=list(map(make_item, data["itemList"])),
     )
 
 
 def make_contacts(data):
+    """
+    make Contact.
+    """
     return Contact(
         email=data.get("email"), phone=data.get("phone"), web=data.get("web")
     )
 
 
 def make_address(data):
+    """
+    make Address.
+    """
     return Address(
         building=data.get("building"),
         city=data.get("city"),
         state=data.get("state"),
         street=data.get("street"),
-        zipCode=data.get("zipCode"),
+        zip_code=data.get("zipCode"),
     )
 
 
 def make_institution(data):
+    """
+    make Institution.
+    """
     return Institution(
         address=make_address(data["address"]),
         code=data["code"],
-        componentType=list(map(make_component_type, data["componentType"])),
+        component_type=list(map(make_component_type, data["componentType"])),
         contacts=make_contacts(data["contacts"]),
         id=data["id"],
         latitude=data["latitude"],
         longitude=data["longitude"],
         name=data["name"],
         supervisor=data["supervisor"],
     )
 
 
 def make_institution_list(data):
+    """
+    make InstitutionList.
+    """
     return InstitutionList(institutions=list(map(make_institution, data)))
 
 
 @attr.s
 class Item:
+    """
+    institution item.
+    """
+
     code = attr.ib()
-    id = attr.ib()
+    id = attr.ib()  # pylint: disable=invalid-name
     name = attr.ib()
 
 
 @attr.s
 class ComponentType:
+    """
+    component type.
+    """
+
     code = attr.ib()
-    itemList = attr.ib()
+    item_list = attr.ib()
     name = attr.ib()
 
 
 @attr.s
 class Contact:
+    """
+    institution contact.
+    """
+
     email = attr.ib()
     phone = attr.ib()
     web = attr.ib()
 
 
 @attr.s
 class Address:
+    """
+    institution address.
+    """
+
     building = attr.ib()
     city = attr.ib()
     state = attr.ib()
     street = attr.ib()
-    zipCode = attr.ib()
+    zip_code = attr.ib()
 
 
 @attr.s
 class Institution:
+    """
+    institution.
+    """
+
     address = attr.ib()
     code = attr.ib()
-    componentType = attr.ib()
+    component_type = attr.ib()
     contacts = attr.ib()
-    id = attr.ib()
+    id = attr.ib()  # pylint: disable=invalid-name
     latitude = attr.ib()
     longitude = attr.ib()
     name = attr.ib()
     supervisor = attr.ib()
 
 
 @attr.s
 class InstitutionList:
+    """
+    list of institutions.
+    """
+
     institutions = attr.ib(type=list)
```

### Comparing `itkdb-0.4.0rc9/tests/conftest.py` & `itkdb-0.4.1rc1/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import base64
 import gzip
 import json
 import socket
 import time
+import uuid
 from sys import platform
 from urllib.parse import parse_qs, quote, urlparse
 
 import betamax
 import pytest
+import requests
 from betamax_serializers import pretty_json
 
 import itkdb
 
 placeholders = {
-    "accessCode1": itkdb.settings.ITKDB_ACCESS_CODE1,
-    "accessCode2": itkdb.settings.ITKDB_ACCESS_CODE2,
+    "access_code1": itkdb.settings.ITKDB_ACCESS_CODE1,
+    "access_code2": itkdb.settings.ITKDB_ACCESS_CODE2,
 }
 
 
 def filter_requests_record(interaction, current_cassette):
     headers = interaction.data["request"]["headers"]
     bearer_token = headers.get("Authorization")
 
@@ -61,21 +63,29 @@
         current_cassette.placeholders.append(
             betamax.cassette.cassette.Placeholder(
                 placeholder="EOS_TOKEN", replace=quote(eos_token[0])
             )
         )
 
 
-def filter_requests_playback(interaction, current_cassette):
-    # get rid of the token in the body
+def filter_requests_playback(interaction, _):
+    # dynamically generate a token for uploading files at a different specific path
     if interaction.data["request"]["uri"].endswith("/requestUploadEosFile"):
         response = interaction.as_response()
 
         data = response.json()
-        data["token"] = "EOS_TOKEN"
+
+        eos_path = f"/eos/atlas/test/itkpd/test/itkdb/{uuid.uuid4()}"
+        eos_request = requests.post(
+            f"https://itkpd2eos.unicornuniversity.net/generate-token?path={eos_path}&permissions=rw"
+        )
+        eos_token = eos_request.json()["token"]
+
+        data["token"] = eos_token
+        data["url"] = f"https://eosatlas.cern.ch{eos_path}"
         enc_data = base64.b64encode(
             gzip.compress(json.dumps(data).encode(response.encoding))
         ).decode()
 
         interaction.data["response"]["body"]["base64_string"] = enc_data
 
 
@@ -88,15 +98,15 @@
     for key, value in placeholders.items():
         config.define_cassette_placeholder(f"<{key.upper()}>", replace=value)
 
 
 @pytest.fixture(scope="session")
 def auth_user():
     user = itkdb.core.User()
-    user._jwtOptions = {
+    user._jwt_options = {
         "verify_signature": False,
         "verify_iat": False,
         "verify_exp": False,
         "verify_aud": False,
     }
     with betamax.Betamax(
         user._session, cassette_library_dir=itkdb.settings.ITKDB_CASSETTE_LIBRARY_DIR
@@ -104,19 +114,24 @@
         user.authenticate()
         user._id_token["exp"] = time.time() + 3600
         yield user
 
 
 @pytest.fixture(scope="module")
 def auth_session(auth_user):
-    yield itkdb.core.Session(user=auth_user)
+    return itkdb.core.Session(user=auth_user)
 
 
 @pytest.fixture(scope="module")
 def auth_client(auth_user):
-    yield itkdb.Client(user=auth_user)
+    return itkdb.Client(user=auth_user)
+
+
+@pytest.fixture(autouse=True)
+def _add_itkdb(doctest_namespace):
+    doctest_namespace["itkdb"] = itkdb
 
 
 # Temporarily work around issue with gethostbyname on OS X
 #  - see https://betamax.readthedocs.io/en/latest/long_term_usage.html#known-issues
 if platform == "darwin":
-    socket.gethostbyname = lambda x: "127.0.0.1"
+    socket.gethostbyname = lambda _: "127.0.0.1"
```

### Comparing `itkdb-0.4.0rc9/tests/test_cli.py` & `itkdb-0.4.1rc1/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pytest
 from click.testing import CliRunner
 
 import itkdb
 from itkdb import commandline
 
 
-@pytest.fixture(scope="function")
+@pytest.fixture()
 def recorder_session(auth_user, monkeypatch):
     monkeypatch.setattr(commandline._session, "user", auth_user)
     with betamax.Betamax(
         commandline._session,
         cassette_library_dir=itkdb.settings.ITKDB_CASSETTE_LIBRARY_DIR,
     ) as recorder:
         yield recorder
@@ -33,15 +33,15 @@
     elapsed = end - start
     assert result.exit_code == 0
     assert itkdb.__version__ in result.stdout
     # make sure it took less than a second
     assert elapsed < 1.0
 
 
-def test_authenticate(recorder_session):
+def test_authenticate(recorder_session):  # noqa: ARG001
     runner = CliRunner()
     result = runner.invoke(commandline.itkdb, ["authenticate"])
     assert result.exit_code == 0
     assert "You have signed in as" in result.output
 
 
 def test_stats(recorder_session):
```

### Comparing `itkdb-0.4.0rc9/tests/test_client.py` & `itkdb-0.4.1rc1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/test_image.py` & `itkdb-0.4.1rc1/tests/test_image.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,23 +5,27 @@
 import itkdb
 
 
 @pytest.fixture()
 def response(mocker):
     response = mocker.MagicMock()
     response.headers = {"content-disposition": "inline; filename=myfilename.ext"}
-    response.content = b"Some binary content that pretends to be an image"
+    response.iter_content = mocker.MagicMock(
+        return_value=iter([b"Some binary content that pretends to be an image"])
+    )
     return response
 
 
 def test_make_image(response):
-    image = itkdb.models.Image.from_response(response)
-    assert isinstance(image, itkdb.models.Image)
-    assert image.filename == "myfilename.ext"
-    assert len(image.getvalue()) == 48
+    image = itkdb.models.ImageFile.from_response(response)
+    assert isinstance(image, itkdb.models.ImageFile)
+    assert image.suggested_filename == "myfilename.ext"
+    assert len(image) == 48
+    assert image.size == 48
 
 
-def test_save_image(tmpdir, response):
-    image = itkdb.models.Image.from_response(response)
-    temp = tmpdir.join("saved_image.jpg")
-    nbytes = image.save(filename=temp.strpath)
+def test_save_image(tmp_path, response):
+    image = itkdb.models.ImageFile.from_response(response)
+    temp = tmp_path.joinpath("saved_image.jpg")
+    nbytes = image.save(filename=temp)
     assert nbytes == 48
+    assert temp.stat().st_size == 48
```

### Comparing `itkdb-0.4.0rc9/tests/test_response.py` & `itkdb-0.4.1rc1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/test_scripts.py` & `itkdb-0.4.1rc1/tests/test_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import os
 import sys
 from types import SimpleNamespace
 
 import betamax
+import getInventory
 import pytest
 
-import getInventory
 import itkdb
 
-sys.path.append(os.path.realpath(os.path.dirname(__file__) + "/.."))
+sys.path.append(os.path.realpath(os.path.dirname(__file__) + "/.."))  # noqa: PTH120
 
 
 @pytest.mark.parametrize(
     "param",
     [
         ("listInstitutions", "INST"),
         ("listComponentTypes", None),
```

### Comparing `itkdb-0.4.0rc9/tests/test_session.py` & `itkdb-0.4.1rc1/tests/test_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     assert (
         auth_session._normalize_url("https://google.com/resource")
         == "https://google.com/resource"
     )
 
 
 def test_expires_after(auth_user):
-    assert itkdb.core.Session(expires_after=dict(days=1))
+    assert itkdb.core.Session(user=auth_user, expires_after={"days": 1})
 
 
 def test_no_bearer(auth_session, mocker):
     spy = mocker.spy(auth_session.user, "authenticate")
     with betamax.Betamax(auth_session).use_cassette("test_session.test_no_bearer"):
         response = auth_session.get("https://google.com/")
```

### Comparing `itkdb-0.4.0rc9/tests/test_user.py` & `itkdb-0.4.1rc1/tests/test_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # set some things on user that we expect to persist or not persist
 _name = "Test User"
 _identity = "Test Identity"
 _response = "A response"
 _status_code = 200
 _access_token = "4cce$$T0k3n"
 _raw_id_token = "R4w1DT0k3n"
-_accessCode1 = "4cce$$C0d31"
-_accessCode2 = "4cce$$C0d32"
+_access_code1 = "4cce$$C0d31"
+_access_code2 = "4cce$$C0d32"
 
 
-@pytest.fixture
+@pytest.fixture()
 def user_temp(tmp_path):
     temp = tmp_path / "auth.pkl"
     assert temp.exists() is False
 
     u = itkdb.core.User(
         save_auth=temp,
-        accessCode1=_accessCode1,
-        accessCode2=_accessCode2,
-        jwtOptions={
+        access_code1=_access_code1,
+        access_code2=_access_code2,
+        jwt_options={
             "verify_signature": False,
             "verify_iat": False,
             "verify_aud": False,
         },
     )
     u._name = _name
     u._id_token = {"exp": time.time() + 3600, "name": _name, "uuidentity": _identity}
@@ -96,17 +96,17 @@
     assert user.is_expired() is False
 
 
 def test_user_repr(user_temp):
     assert str(user_temp[0])
 
 
-def test_user_accessCodes(user_temp):
-    assert user_temp[0].accessCode1 == _accessCode1
-    assert user_temp[0].accessCode2 == _accessCode2
+def test_user_access_codes(user_temp):
+    assert user_temp[0].access_code1 == _access_code1
+    assert user_temp[0].access_code2 == _access_code2
 
 
 def test_user_unpicklable(user_temp, caplog):
     user, temp = user_temp
     session = itkdb.core.Session(user=user)
     assert temp.exists() is False
     with caplog.at_level(logging.INFO, "itkdb"):
@@ -120,15 +120,15 @@
     user, temp = user_temp
     # set up first user and check that we can dump
     session = itkdb.core.Session(user=user)
     assert temp.exists() is False
     assert session.user._dump()
     assert temp.exists()
     assert temp.stat().st_size
-    with open(user._save_auth, "rb") as fp:
+    with user._save_auth.open("rb") as fp:
         assert pickle.load(fp)
 
     # check if we can reload user
     session.user._id_token = None
     assert session.user._load()
     assert session.user.name == _name
     del session
```

### Comparing `itkdb-0.4.0rc9/tests/test_utils.py` & `itkdb-0.4.1rc1/tests/test_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 
 import pytest
 import requests
 
 import itkdb
 
 
+def test_true():
+    assert True
+
+
 def test_build_url_utils(mocker):
     request = mocker.MagicMock()
     request.url = "https://itkpd-test.unicorncollege.cz/createTestRunAttachment"
     request.body = b"abytestring"
     assert (
         itkdb.caching.utils.build_url(request)
         == "https://itkpd-test.unicorncollege.cz/createTestRunAttachment?&body=abytestring"
@@ -21,147 +25,175 @@
 def test_pretty_print():
     request = requests.Request(
         "POST",
         "https://stackoverflow.com",
         headers={"User-Agent": "Test"},
         json={"hello": "world"},
     )
-    text = itkdb.utilities.pretty_print(request)
+    text = itkdb.utils.pretty_print(request)
     assert (
         text
         == 'Host: stackoverflow.com\r\nPOST / HTTP/1.1\r\nUser-Agent: Test\r\nContent-Length: 18\r\nContent-Type: application/json\r\n\r\n{"hello": "world"}'
     )
 
 
 def test_merge_url():
     assert (
-        itkdb.utilities.merge_url_query_params(
+        itkdb.utils.merge_url_query_params(
             "https://itkpd-test.unicorncollege.cz/createTestRunAttachment",
             {"param1": "value1"},
         )
         == "https://itkpd-test.unicorncollege.cz/createTestRunAttachment?param1=value1"
     )
     assert (
-        itkdb.utilities.merge_url_query_params(
+        itkdb.utils.merge_url_query_params(
             "https://itkpd-test.unicorncollege.cz/createTestRunAttachment?param2=value2",
             {"param1": "value1"},
         )
         == "https://itkpd-test.unicorncollege.cz/createTestRunAttachment?param2=value2&param1=value1"
     )
 
 
 @pytest.mark.parametrize(
-    "fname,ftype",
+    ("fname", "ftype"),
     [
         ("data.txt", "text/plain"),
         ("data.png", "image/png"),
         ("data.root", "application/octet-stream"),
     ],
     ids=["text", "image", "root"],
 )
 def test_get_file_components(mocker, tmp_path, fname, ftype):
     mocker.patch("magic.from_file", return_value=ftype)
     mocker.patch("requests.utils.guess_filename", return_value=fname)
 
     fpath = tmp_path / fname
     fpath.write_text("this is a data file")
 
-    fn, fp, ft, fh = itkdb.utilities.get_file_components(
+    fn, fp, ft, fh = itkdb.utils.get_file_components(
         {"data": (fname, fpath.open("rb"), ftype, {"a": "b"})}
     )
     assert fn == fname
     assert isinstance(fp, io.IOBase)
     assert ft == ftype
     assert fh == {"a": "b"}
     fp.close()
 
-    fn, fp, ft, fh = itkdb.utilities.get_file_components(
+    fn, fp, ft, fh = itkdb.utils.get_file_components(
         {"data": (fname, fpath.open("rb"), ftype)}
     )
     assert fn == fname
     assert isinstance(fp, io.IOBase)
     assert ft == ftype
     assert fh == {}
     fp.close()
 
-    fn, fp, ft, fh = itkdb.utilities.get_file_components(
+    fn, fp, ft, fh = itkdb.utils.get_file_components(
         {"data": (fname, fpath.open("rb"))}
     )
     assert fn == fname
     assert isinstance(fp, io.IOBase)
     assert ft == ftype
     assert fh == {}
     fp.close()
 
-    fn, fp, ft, fh = itkdb.utilities.get_file_components({"data": fpath.open("rb")})
+    fn, fp, ft, fh = itkdb.utils.get_file_components({"data": fpath.open("rb")})
     assert fn == fname
     assert isinstance(fp, io.IOBase)
     assert ft == ftype
     assert fh == {}
     fp.close()
 
 
+def test_get_file_components_image_type():
+    fname = itkdb.data / "1x1.jpg"
+    with fname.open("rb") as fpointer:
+        fn, fp, ft, fh = itkdb.utils.get_file_components({"data": fpointer})
+        assert ft == "image/jpeg"
+
+    with fname.open(encoding="utf-8") as fpointer:
+        fn, fp, ft, fh = itkdb.utils.get_file_components({"data": (fname, fpointer)})
+        assert ft == "image/jpeg"
+
+
 def test_get_file_components_too_many():
-    with pytest.raises(ValueError):
-        itkdb.utilities.get_file_components({"data": None, "another_file": None})
+    with pytest.raises(
+        ValueError, match="creating a single attachment but you specified 2 files"
+    ):
+        itkdb.utils.get_file_components({"data": None, "another_file": None})
 
 
 def test_is_image():
     fn = itkdb.data / "1x1.jpg"
     with fn.open("rb") as fp:
-        assert itkdb.utilities.is_image(str(fn), fp)
+        assert itkdb.utils.is_image(str(fn), fp)
 
 
 def test_is_image_bad_path():
     fn = itkdb.data / "1x1.jpg"
     with fn.open("rb") as fp:
-        assert itkdb.utilities.is_image("/an/absolutely/fake/path", fp)
+        assert itkdb.utils.is_image("/an/absolutely/fake/path", fp)
 
 
 def test_is_not_image():
     fn = itkdb.data / "1x1.sh"
     with fn.open("rb") as fp:
-        assert not itkdb.utilities.is_image(str(fn), fp)
+        assert not itkdb.utils.is_image(str(fn), fp)
+
+
+def test_is_root():
+    fn = itkdb.data / "tiny.root"
+    with fn.open("rb") as fp:
+        assert itkdb.utils.is_root(str(fn), fp)
+
+
+def test_is_not_root():
+    fn = itkdb.data / "1x1.jpg"
+    with fn.open("rb") as fp:
+        assert not itkdb.utils.is_root(str(fn), fp)
 
 
 @pytest.mark.parametrize(
-    "fpath,ftype,mode",
+    ("fpath", "ftype"),
     [
-        (itkdb.data / "1x1.jpg", "image/jpeg", "rb"),
-        (itkdb.data / "1x1.sh", "text/x-shellscript", "rb"),
-        (itkdb.data / "1x1.sh", "text/x-shellscript", "r"),
+        (itkdb.data / "1x1.jpg", "image/jpeg"),
+        (itkdb.data / "1x1.sh", "text/x-shellscript"),
+        (itkdb.data / "1x1.sh", "text/x-shellscript"),
+        (itkdb.data / "tiny.root", "application/octet-stream"),
     ],
-    ids=["jpeg", "shellscript-binary", "shellscript"],
+    ids=["jpeg", "shellscript-binary", "shellscript", "root"],
 )
-def test_get_mimetype_path(fpath, ftype, mode):
-    assert itkdb.utilities.get_mimetype(fpath, None) == ftype
+def test_get_mimetype_path(fpath, ftype):
+    assert itkdb.utils.get_mimetype(fpath, None) == ftype
 
 
 @pytest.mark.parametrize(
-    "fpath,ftype,mode",
+    ("fpath", "ftype", "mode"),
     [
         (itkdb.data / "1x1.jpg", "image/jpeg", "rb"),
         (itkdb.data / "1x1.sh", "text/x-shellscript", "rb"),
         (itkdb.data / "1x1.sh", "text/x-shellscript", "r"),
+        (itkdb.data / "tiny.root", "application/octet-stream", "rb"),
     ],
-    ids=["jpeg", "shellscript-binary", "shellscript"],
+    ids=["jpeg", "shellscript-binary", "shellscript", "root"],
 )
 def test_get_mimetype_io(fpath, ftype, mode):
     with fpath.open(mode) as fp:
-        assert itkdb.utilities.get_mimetype("/an/abs/fake/path", fp) == ftype
+        assert itkdb.utils.get_mimetype("/an/abs/fake/path", fp) == ftype
         assert fp.tell() == 0
 
 
 @pytest.mark.parametrize(
-    "fpath,fsize,mode",
+    ("fpath", "fsize", "mode"),
     [
         (itkdb.data / "1x1.jpg", 125, "rb"),
         (itkdb.data / "1x1.sh", 820, "rb"),
         (itkdb.data / "1x1.sh", 820, "r"),
+        (itkdb.data / "tiny.root", 399, "rb"),
     ],
-    ids=["jpeg", "shellscript-binary", "shellscript"],
+    ids=["jpeg", "shellscript-binary", "shellscript", "root"],
 )
 def test_get_filesize(fpath, fsize, mode):
     with fpath.open(mode) as fp:
-        assert itkdb.utilities.get_filesize(fpath, None) == fsize
-        assert itkdb.utilities.get_filesize("/an/abs/fake/path", fp) == fsize
+        assert itkdb.utils.get_filesize(fpath, None) == fsize
+        assert itkdb.utils.get_filesize("/an/abs/fake/path", fp) == fsize
         assert fp.tell() == 0
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_attachments.py` & `itkdb-0.4.1rc1/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/test_binaryData.py` & `itkdb-0.4.1rc1/tests/integration/test_binaryData.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+import logging
+
 import betamax
 
 import itkdb
 
 
 def test_get_image(auth_session):
     with betamax.Betamax(auth_session).use_cassette("test_binaryData.test_get_image"):
@@ -22,17 +24,17 @@
     with betamax.Betamax(auth_client).use_cassette("test_binaryData.test_get_image"):
         image = auth_client.get(
             "uu-app-binarystore/getBinaryData",
             json={
                 "code": "bc2eccc58366655352582970d3f81bf46f15a48cf0cb98d74e21463f1dc4dcb9"
             },
         )
-        assert isinstance(image, itkdb.models.Image)
-        assert image.filename == "PB6.CR2"
-        assert image.format == "cr2"
+        assert isinstance(image, itkdb.models.ImageFile)
+        assert image.suggested_filename == "PB6.CR2"
+        assert image.extension == "cr2"
         temp = tmpdir.join("saved_image.cr2")
         nbytes = image.save(filename=temp.strpath)
         assert nbytes == 1166
 
 
 def test_get_plain_text(auth_session):
     with betamax.Betamax(auth_session).use_cassette(
@@ -55,17 +57,17 @@
     ):
         text = auth_client.get(
             "uu-app-binarystore/getBinaryData",
             json={
                 "code": "5fd40be3b9f9ada57fa47fe4d8b3c48b26055d5d1c6306d76eb2181d20089879"
             },
         )
-        assert isinstance(text, itkdb.models.Text)
-        assert text.filename == "for_gui test3.txt"
-        assert text.format == "txt"
+        assert isinstance(text, itkdb.models.TextFile)
+        assert text.suggested_filename == "for_gui test3.txt"
+        assert text.extension == "txt"
         temp = tmpdir.join("saved_text.txt")
         nbytes = text.save(filename=temp.strpath)
         assert nbytes == 23
 
 
 def test_issue4(auth_session):
     with betamax.Betamax(auth_session).use_cassette("test_binaryData.test_issue4"):
@@ -86,17 +88,17 @@
         text = auth_client.get(
             "uu-app-binarystore/getBinaryData",
             json={
                 "code": "fe4f85dd3740c53956c22bb4324065b8",
                 "contentDisposition": "attachment",
             },
         )
-        assert isinstance(text, itkdb.models.Text)
-        assert text.filename == "VPA37913-W00221_Striptest_Segment_4_001.dat"
-        assert text.format == "dat"
+        assert isinstance(text, itkdb.models.TextFile)
+        assert text.suggested_filename == "VPA37913-W00221_Striptest_Segment_4_001.dat"
+        assert text.extension == "dat"
         temp = tmpdir.join("saved_text.dat")
         nbytes = text.save(filename=temp.strpath)
         assert nbytes == 1000
 
 
 def test_get_zipfile(auth_session):
     with betamax.Betamax(auth_session).use_cassette(
@@ -115,33 +117,49 @@
 def test_get_zipfile_model(auth_client, tmpdir):
     with betamax.Betamax(auth_client).use_cassette("test_binaryData.test_get_zipfile"):
         zipfile = auth_client.get(
             "uu-app-binarystore/getBinaryData",
             json={"code": "143b2c7182137ff619968f4cc41a18ca"},
         )
         assert isinstance(zipfile, itkdb.models.ZipFile)
-        assert zipfile.filename == "configuration_MODULETHERMALCYCLING.zip"
-        assert zipfile.format == "zip"
+        assert zipfile.suggested_filename == "configuration_MODULETHERMALCYCLING.zip"
+        assert zipfile.extension == "zip"
+        assert zipfile.size == 226988
+        assert zipfile.size_fmt == "221.7KiB"
         temp = tmpdir.join("saved_zipfile.zip")
         nbytes = zipfile.save(filename=temp.strpath)
         assert nbytes == 226988
 
 
-def test_get_image_model_eos(tmpdir, auth_client):
+def test_get_image_model_eos(tmpdir, auth_client, caplog):
     with betamax.Betamax(auth_client).use_cassette(
         "test_binaryData.test_get_image_model_eos", preserve_exact_body_bytes=True
     ):
-
         auth = auth_client.post(
             "https://itkpd2eos.unicornuniversity.net/generate-token?path=/eos/atlas/test/itkpd/c/c/c/cccac749f4f3d5e493a0186ca9e42803"
         )
-        image = auth_client.get(
-            f'https://eosatlas.cern.ch/eos/atlas/test/itkpd/c/c/c/cccac749f4f3d5e493a0186ca9e42803?authz={auth["token"]}',
-            verify=itkdb.data / "CERN_chain.pem",
-        )
 
-        assert isinstance(image, itkdb.models.Image)
-        assert image.filename is None
-        assert image.format == "jpg"
+        # NB: this will not work if you want to try to spy it
+        # spy = mocker.spy(super(auth_client.__class__, auth_client).get, "__func__")
+        with caplog.at_level(logging.INFO, "itkdb.client"):
+            image = auth_client.get(
+                f'https://eosatlas.cern.ch/eos/atlas/test/itkpd/c/c/c/cccac749f4f3d5e493a0186ca9e42803?authz={auth["token"]}',
+            )
+            assert (
+                "Identified a cern.ch request, will attach CERN SSL chain to request by overriding `verify`"
+                in caplog.text
+            )
+            assert (
+                "Identified a request that potentially downloads larger amounts of data, will execute chunked requests (stream=True)"
+                in caplog.text
+            )
+            assert (
+                "Changing the mimetype for the response from EOS from 'application/octet-stream' to 'image/jpeg'"
+                in caplog.text
+            )
+
+        assert isinstance(image, itkdb.models.ImageFile)
+        assert image.suggested_filename is None
+        assert image.extension == "jpg"
         temp = tmpdir.join("saved_image.jpg")
         nbytes = image.save(filename=temp.strpath)
         assert nbytes == 125
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_cache.py` & `itkdb-0.4.1rc1/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/test_components.py` & `itkdb-0.4.1rc1/tests/integration/test_components.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         response = auth_client.get(
             "getComponentBulk", json={"component": ["54f134b9975bebc851c4671d0ccbb489"]}
         )
         assert response
         assert isinstance(response, list)
 
 
-def test_add_comment(tmpdir, auth_session):
+def test_add_comment(auth_session):
     with betamax.Betamax(auth_session).use_cassette("test_components.test_add_comment"):
         component = "20USE000000086"
         message = "this is a test message"
         data = {"component": component, "comments": [message]}
         response = auth_session.post("createComponentComment", json=data)
         assert response.status_code == 200
         response = response.json()
@@ -150,22 +150,21 @@
                 foundComment = True
                 break
 
         assert foundComment
 
 
 # https://uuapp.plus4u.net/uu-bookkit-maing01/78462435-41f76117152c4c6e947f498339998055/book/page?code=41219994
-def test_create_attachment_image_eos(tmpdir, auth_client, monkeypatch):
+def test_create_attachment_image_eos(auth_client, monkeypatch):
     monkeypatch.setattr(auth_client, "_use_eos", True)
 
     image = itkdb.data / "1x1.jpg"
     with betamax.Betamax(auth_client).use_cassette(
         "test_components.test_create_attachment_image_eos"
     ):
-
         component_before = auth_client.get(
             "getComponent", json={"component": "7f633f626f5466b2a72c1be7cd4cb8bc"}
         )
 
         with image.open("rb") as fp:
             data = {
                 "component": "7f633f626f5466b2a72c1be7cd4cb8bc",
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_institution.py` & `itkdb-0.4.1rc1/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/test_session.py` & `itkdb-0.4.1rc1/tests/integration/test_session.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,40 +2,40 @@
 
 import betamax
 import pytest
 
 import itkdb
 
 
-@pytest.mark.xfail
+@pytest.mark.xfail()
 def test_fake_route(auth_session):
-    with betamax.Betamax(auth_session).use_cassette("test_session.test_fake_route"):
-        with pytest.raises(itkdb.exceptions.NotFound):
-            auth_session.get("aFakeRoute")
+    with betamax.Betamax(auth_session).use_cassette(
+        "test_session.test_fake_route"
+    ), pytest.raises(itkdb.exceptions.NotFound):
+        auth_session.get("aFakeRoute")
 
 
 def test_invalid_project(auth_session):
     with betamax.Betamax(auth_session).use_cassette(
         "test_session.test_invalid_project"
-    ):
-        with pytest.raises(itkdb.exceptions.BadRequest):
-            auth_session.get(
-                "listComponents", json={"project": "Fake", "pageInfo": {"pageSize": 1}}
-            )
+    ), pytest.raises(itkdb.exceptions.BadRequest):
+        auth_session.get(
+            "listComponents", json={"project": "Fake", "pageInfo": {"pageSize": 1}}
+        )
 
 
 def test_missing_required(auth_session):
     with betamax.Betamax(auth_session).use_cassette(
         "test_session.test_missing_required"
-    ):
-        with pytest.raises(itkdb.exceptions.BadRequest):
-            auth_session.get("getComponent", json={"pageInfo": {"pageSize": 1}})
+    ), pytest.raises(itkdb.exceptions.BadRequest):
+        auth_session.get("getComponent", json={"pageInfo": {"pageSize": 1}})
 
 
-@pytest.mark.xfail
+@pytest.mark.xfail()
 def test_unauthorized():
-    session = itkdb.core.Session(user=itkdb.core.User(accessCode1="", accessCode2=""))
-    with betamax.Betamax(session).use_cassette("test_session.test_unauthorized"):
-        with pytest.raises(itkdb.exceptions.Forbidden):
-            session.get(
-                "listComponents", json={"project": "S", "pageInfo": {"pageSize": 1}}
-            )
+    session = itkdb.core.Session(user=itkdb.core.User(access_code1="", access_code2=""))
+    with betamax.Betamax(session).use_cassette(
+        "test_session.test_unauthorized"
+    ), pytest.raises(itkdb.exceptions.Forbidden):
+        session.get(
+            "listComponents", json={"project": "S", "pageInfo": {"pageSize": 1}}
+        )
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_shipments.py` & `itkdb-0.4.1rc1/tests/integration/test_shipments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from __future__ import annotations
 
 import betamax
 
 import itkdb
 
 
-def test_create_attachment_image_eos(tmpdir, auth_client, monkeypatch):
+def test_create_attachment_image_eos(auth_client, monkeypatch):
     monkeypatch.setattr(auth_client, "_use_eos", True)
 
     image = itkdb.data / "1x1.jpg"
     with betamax.Betamax(auth_client).use_cassette(
         "test_shipments.test_create_attachment_image_eos"
     ):
-
         shipment_before = auth_client.get(
             "getShipment", json={"shipment": "61149203db062f000b98a75a"}
         )
 
         with image.open("rb") as fp:
             data = {
                 "shipment": "61149203db062f000b98a75a",
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_summary.py` & `itkdb-0.4.1rc1/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/test_testproperties.py` & `itkdb-0.4.1rc1/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/test_tests.py` & `itkdb-0.4.1rc1/tests/integration/test_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,21 @@
         assert response
         assert "pageItemList" in response
         assert "componentType" in response
         assert "pageInfo" in response
         assert "uuAppErrorMap" in response
 
 
-def test_create_attachment_image_eos(tmpdir, auth_client, monkeypatch):
+def test_create_attachment_image_eos(auth_client, monkeypatch):
     monkeypatch.setattr(auth_client, "_use_eos", True)
 
     image = itkdb.data / "1x1.jpg"
     with betamax.Betamax(auth_client).use_cassette(
         "test_tests.test_create_attachment_image_eos"
     ):
-
         testRun_before = auth_client.get(
             "getTestRun",
             json={"testRun": "5dde2c1279bc5c000a61d5e2", "outputType": "object"},
         )
 
         with image.open("rb") as fp:
             data = {
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_user.py` & `itkdb-0.4.1rc1/tests/integration/test_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,67 +4,69 @@
 
 import betamax
 import pytest
 
 import itkdb
 
 # because expiration will fail (since we cache this information) skip the verification of expiration
-jwtOptions = {
+jwt_options = {
     "verify_signature": False,
     "verify_iat": False,
     "verify_exp": False,
     "verify_aud": False,
 }
 
 
 def test_user_create():
-    user = itkdb.core.User(accessCode1="foo", accessCode2="bar")
+    user = itkdb.core.User(access_code1="foo", access_code2="bar")
     assert user.access_token is None
-    assert user.bearer == ""
+    assert not user.bearer
     assert user.id_token == {}
-    assert user.name == ""
+    assert not user.name
     assert user.expires_at == 0
     assert user.expires_in == 0
     assert user.is_expired()
 
 
 # NB: because we are using betamax - the ID token which is invalid after 2
 # hours is kept so user.is_expired() will be true for testing, do not assert it
-def test_user_anonymous_login(caplog):
-    user = itkdb.core.User(accessCode1="", accessCode2="", jwtOptions=jwtOptions)
+def test_user_anonymous_login():
+    user = itkdb.core.User(access_code1="", access_code2="", jwt_options=jwt_options)
     with betamax.Betamax(user._session).use_cassette(
         "test_user.test_user_anonymous_login"
     ):
         with pytest.raises(itkdb.exceptions.ResponseException):
             user.authenticate()
         assert user.is_authenticated() is False
         assert user._response is not None
         assert user._response.status_code == 500
 
 
-def test_user_bad_login(caplog):
-    user = itkdb.core.User(accessCode1="foo", accessCode2="bar", jwtOptions=jwtOptions)
+def test_user_bad_login():
+    user = itkdb.core.User(
+        access_code1="foo", access_code2="bar", jwt_options=jwt_options
+    )
     with betamax.Betamax(user._session).use_cassette("test_user.test_user_bad_login"):
         with pytest.raises(itkdb.exceptions.ResponseException):
             user.authenticate()
         assert user.is_authenticated() is False
         assert user._response is not None
         assert user._response.status_code == 401
 
 
 # NB: because we are using betamax - the ID token which is invalid after 2
 # hours is kept so user.is_expired() will be true for testing, do not assert it
 def test_user_good_login(caplog):
-    user = itkdb.core.User(jwtOptions=jwtOptions)
+    user = itkdb.core.User(jwt_options=jwt_options)
     with betamax.Betamax(user._session).use_cassette("test_user.test_user_good_login"):
         with caplog.at_level(logging.INFO, "itkdb"):
             user.authenticate()
-            assert caplog.text == ""
+            assert not caplog.text
         assert user.is_authenticated()
         assert user._response
 
 
 def test_user_identity():
-    user = itkdb.core.User(jwtOptions=jwtOptions)
+    user = itkdb.core.User(jwt_options=jwt_options)
     with betamax.Betamax(user._session).use_cassette("test_user.test_user_good_login"):
         user.authenticate()
         assert user.identity
```

### Comparing `itkdb-0.4.0rc9/tests/integration/test_warning.py` & `itkdb-0.4.1rc1/tests/integration/test_warning.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 import logging
 
 import betamax
 
 
 def test_get_component(auth_client, caplog):
-    with betamax.Betamax(auth_client).use_cassette("test_warnings.test_get_component"):
-        with caplog.at_level(logging.WARNING, "itkdb.core"):
-            auth_client.get(
-                "getComponent", json={"component": "20USE000000086", "ignoreme": "fake"}
-            )
-            assert "cern-itkpd-main/getComponent/unsupportedKeys" in caplog.text
-            assert "ignoreme" in caplog.text
-            caplog.clear()
+    with betamax.Betamax(auth_client).use_cassette(
+        "test_warnings.test_get_component"
+    ), caplog.at_level(logging.WARNING, "itkdb.core"):
+        auth_client.get(
+            "getComponent", json={"component": "20USE000000086", "ignoreme": "fake"}
+        )
+        assert "cern-itkpd-main/getComponent/unsupportedKeys" in caplog.text
+        assert "ignoreme" in caplog.text
+        caplog.clear()
 
 
 def test_delete_test_property(auth_client, caplog):
     with betamax.Betamax(auth_client).use_cassette(
         "test_testproperties.test_delete_test_property"
-    ):
-        with caplog.at_level(logging.WARNING, "itkdb.core"):
-            # first create, then delete
-            auth_client.post(
-                "createTestTypeProperty",
-                json={
-                    "id": "603665218f621e000aeada88",
-                    "code": "TESTDELETEME",
-                    "name": "Test Delete Me",
-                    "dataType": "string",
-                },
-            )
-            assert "UuApp::Oidc::Session" in caplog.text
-            caplog.clear()
-
-            auth_client.post(
-                "deleteTestTypeProperty",
-                json={"id": "603665218f621e000aeada88", "code": "TESTDELETEME"},
-            )
-            assert "UuApp::Oidc::Session" in caplog.text
-            caplog.clear()
+    ), caplog.at_level(logging.WARNING, "itkdb.core"):
+        # first create, then delete
+        auth_client.post(
+            "createTestTypeProperty",
+            json={
+                "id": "603665218f621e000aeada88",
+                "code": "TESTDELETEME",
+                "name": "Test Delete Me",
+                "dataType": "string",
+            },
+        )
+        assert "UuApp::Oidc::Session" in caplog.text
+        caplog.clear()
+
+        auth_client.post(
+            "deleteTestTypeProperty",
+            json={"id": "603665218f621e000aeada88", "code": "TESTDELETEME"},
+        )
+        assert "UuApp::Oidc::Session" in caplog.text
+        caplog.clear()
```

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'http_interactions'": "{0: {'response': {'headers': {'Content-Disposition': ['inline; "*

 * *                        'filename="PB6.CR2"\']}}}}'}*

```diff
@@ -42,15 +42,15 @@
                     "Cache-Control": [
                         "max-age=60, private"
                     ],
                     "Connection": [
                         "Keep-Alive"
                     ],
                     "Content-Disposition": [
-                        "inline; filename=PB6.CR2"
+                        "inline; filename=\"PB6.CR2\""
                     ],
                     "Content-Length": [
                         "35819362"
                     ],
                     "Content-Type": [
                         "image/x-canon-cr2"
                     ],
```

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'http_interactions'": "{0: {'response': {'headers': {'Content-Disposition': ['inline; "*

 * *                        'filename="for_gui test3.txt"\']}}}}'}*

```diff
@@ -43,15 +43,15 @@
                     "Cache-Control": [
                         "max-age=60, private"
                     ],
                     "Connection": [
                         "Keep-Alive"
                     ],
                     "Content-Disposition": [
-                        "inline; filename=for_gui test3.txt"
+                        "inline; filename=\"for_gui test3.txt\""
                     ],
                     "Content-Encoding": [
                         "gzip"
                     ],
                     "Content-Type": [
                         "text/plain; charset=UTF-8"
                     ],
```

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998372395833334%*

 * *Differences: {"'http_interactions'": "{0: {'response': {'headers': {'Content-Disposition': ['attachment; "*

 * *                        'filename="VPA37913-W00221_Striptest_Segment_4_001.dat"\']}}}}'}*

```diff
@@ -48,15 +48,15 @@
                     "Cache-Control": [
                         "max-age=60, private"
                     ],
                     "Connection": [
                         "Keep-Alive"
                     ],
                     "Content-Disposition": [
-                        "attachment; filename=VPA37913-W00221_Striptest_Segment_4_001.dat"
+                        "attachment; filename=\"VPA37913-W00221_Striptest_Segment_4_001.dat\""
                     ],
                     "Content-Length": [
                         "54104"
                     ],
                     "Content-Type": [
                         "text"
                     ],
```

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/.gitignore` & `itkdb-0.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/COPYING` & `itkdb-0.4.1rc1/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.0rc9/LICENSE` & `itkdb-0.4.1rc1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 itkdb - Python wrapper to interface with ITk DB
-Copyright (C) 2018-2020  Giordon Stark
+Copyright (C) 2018-2022  Giordon Stark
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
```

