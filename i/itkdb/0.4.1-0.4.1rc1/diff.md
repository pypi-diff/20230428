# Comparing `tmp/itkdb-0.4.1.tar.gz` & `tmp/itkdb-0.4.1rc1.tar.gz`

## Comparing `itkdb-0.4.1.tar` & `itkdb-0.4.1rc1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 itkdb-0.4.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 itkdb-0.4.1/.linkcheckerrc
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 itkdb-0.4.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 itkdb-0.4.1/add_attachment.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 itkdb-0.4.1/add_comment.py
--rwxr-xr-x   0        0        0    36494 2020-02-02 00:00:00.000000 itkdb-0.4.1/generatePlots.py
--rwxr-xr-x   0        0        0    27894 2020-02-02 00:00:00.000000 itkdb-0.4.1/getContentSummary.py
--rwxr-xr-x   0        0        0    20487 2020-02-02 00:00:00.000000 itkdb-0.4.1/getInventory.py
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 itkdb-0.4.1/mkdocs.yml
--rwxr-xr-x   0        0        0    27949 2020-02-02 00:00:00.000000 itkdb-0.4.1/registerComponent.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 itkdb-0.4.1/tbump.toml
--rwxr-xr-x   0        0        0      982 2020-02-02 00:00:00.000000 itkdb-0.4.1/ci/pre-commit-update.sh
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/config.md
--rw-r--r--   0        0        0    18833 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/examples.md
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/history.md
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/index.md
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/install.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/macros.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/.overrides/main.html
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/.snippets/abbrs.txt
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/.snippets/links.txt
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/assets/css/custom.css
--rw-r--r--   0        0        0    23475 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/assets/images/logo.svg
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/meta/authors.md
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/meta/faq.md
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/reference/gen_ref_nav.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 itkdb-0.4.1/docs/reference/cli/itkdb.md
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/_version.py
--rw-r--r--   0        0        0    14035 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/client.py
--rw-r--r--   0        0        0     8034 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/commandline.py
--rw-r--r--   0        0        0    12467 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/core.py
--rw-r--r--   0        0        0     4397 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/py.typed
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/responses.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/typing.py
--rw-r--r--   0        0        0     8985 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/utils.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/caching/__init__.py
--rw-r--r--   0        0        0     3610 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/caching/adapter.py
--rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/caching/controller.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/caching/utils.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/1x1.jpg
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/1x1.sh
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/CERN_chain.pem
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/README.md
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/__init__.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/data/tiny.root
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/models/__init__.py
--rw-r--r--   0        0        0     7524 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/models/file.py
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/models/institution.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/settings/__init__.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 itkdb-0.4.1/src/itkdb/settings/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_cli.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_client.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_image.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_response.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_scripts.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_session.py
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_user.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/test_utils.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_attachments.py
--rw-r--r--   0        0        0     6334 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_binaryData.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_cache.py
--rw-r--r--   0        0        0     6522 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_components.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_institution.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_projects.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_session.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_shipments.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_stats.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_summary.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_testproperties.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_tests.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_user.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/test_warning.py
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_attachments.test_add_attachment.json
--rw-r--r--   0        0        0    94089 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json
--rw-r--r--   0        0        0     7917 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_image.json
--rw-r--r--   0        0        0    11021 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json
--rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_plainText.json
--rw-r--r--   0        0        0   304955 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json
--rw-r--r--   0        0        0     3939 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_issue4.json
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_add_comment.json
--rw-r--r--   0        0        0    28946 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0    32318 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_get.json
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_bulk.json
--rw-r--r--   0        0        0     4499 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_info_code.json
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_info_serial.json
--rw-r--r--   0        0        0   112349 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json
--rw-r--r--   0        0        0   108642 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json
--rw-r--r--   0        0        0   245837 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_componentsv1.json
--rw-r--r--   0        0        0   245811 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_componentsv2.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_institution.test_get.json
--rw-r--r--   0        0        0   101372 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_institution.test_pagination.json
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_projects.test_list_projects.json
--rw-r--r--   0        0        0    32478 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json
--rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.trashUnassembled.json
--rw-r--r--   0        0        0     5912 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_session.test_fake_route.json
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_session.test_invalid_project.json
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_session.test_missing_required.json
--rw-r--r--   0        0        0    12679 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_session.test_no_bearer.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_session.test_unauthorized.json
--rw-r--r--   0        0        0    19435 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_stats.test_get.json
--rw-r--r--   0        0        0   509788 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_summary.test_get_summary.json
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json
--rw-r--r--   0        0        0    19982 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_tests.test_list_test_types.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_anonymous_login.json
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_bad_login.json
--rw-r--r--   0        0        0    17319 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_good_login.json
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 itkdb-0.4.1/tests/integration/cassettes/test_warnings.test_get_component.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 itkdb-0.4.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 itkdb-0.4.1/COPYING
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 itkdb-0.4.1/LICENSE
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 itkdb-0.4.1/README.md
--rw-r--r--   0        0        0     7722 2020-02-02 00:00:00.000000 itkdb-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9157 2020-02-02 00:00:00.000000 itkdb-0.4.1/PKG-INFO
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

### Comparing `itkdb-0.4.1/.gitlab-ci.yml` & `itkdb-0.4.1rc1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/.pre-commit-config.yaml` & `itkdb-0.4.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/generatePlots.py` & `itkdb-0.4.1rc1/generatePlots.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/getContentSummary.py` & `itkdb-0.4.1rc1/getContentSummary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/getInventory.py` & `itkdb-0.4.1rc1/getInventory.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/mkdocs.yml` & `itkdb-0.4.1rc1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/registerComponent.py` & `itkdb-0.4.1rc1/registerComponent.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tbump.toml` & `itkdb-0.4.1rc1/tbump.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e34 2e31 220a 0a23 2045  t = "0.4.1"..# E
-00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
-00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
-00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
-00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
-00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
-00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
-00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
-00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
-000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
-000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
-000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
-000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
-000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
-000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
-00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
-00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
-00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
-00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 342e  mp version: 0.4.
-00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
-00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
-00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
-00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
-00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
-000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
-000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
-000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
-000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
-000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
-000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
-00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
-00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
-00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
-00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
-00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
-00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
-00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
-00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
-00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
-00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
-000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
-000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
-000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
-000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
-000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
-000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
-00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 6c65  ADME.md"..[[file
-00000310: 5d5d 0a73 7263 203d 2022 7079 7072 6f6a  ]].src = "pyproj
-00000320: 6563 742e 746f 6d6c 220a 7665 7273 696f  ect.toml".versio
-00000330: 6e5f 7465 6d70 6c61 7465 203d 2022 7b6d  n_template = "{m
-00000340: 616a 6f72 7d2e 7b6d 696e 6f72 7d22 0a73  ajor}.{minor}".s
-00000350: 6561 7263 6820 3d20 2269 746b 6462 2e64  earch = "itkdb.d
-00000360: 6f63 732e 6365 726e 2e63 682f 7b63 7572  ocs.cern.ch/{cur
-00000370: 7265 6e74 5f76 6572 7369 6f6e 7d22 0a0a  rent_version}"..
-00000380: 5b5b 6669 6c65 5d5d 0a73 7263 203d 2022  [[file]].src = "
-00000390: 7372 632f 6974 6b64 622f 636c 6965 6e74  src/itkdb/client
-000003a0: 2e70 7922 0a76 6572 7369 6f6e 5f74 656d  .py".version_tem
-000003b0: 706c 6174 6520 3d20 227b 6d61 6a6f 727d  plate = "{major}
-000003c0: 2e7b 6d69 6e6f 727d 220a 7365 6172 6368  .{minor}".search
-000003d0: 203d 2022 6974 6b64 622e 646f 6373 2e63   = "itkdb.docs.c
-000003e0: 6572 6e2e 6368 2f7b 6375 7272 656e 745f  ern.ch/{current_
-000003f0: 7665 7273 696f 6e7d 220a 0a5b 5b66 6965  version}"..[[fie
-00000400: 6c64 5d5d 0a23 2074 6865 206e 616d 6520  ld]].# the name 
-00000410: 6f66 2074 6865 2066 6965 6c64 0a6e 616d  of the field.nam
-00000420: 6520 3d20 2263 616e 6469 6461 7465 220a  e = "candidate".
-00000430: 2320 7468 6520 6465 6661 756c 7420 7661  # the default va
-00000440: 6c75 6520 746f 2075 7365 2c20 6966 2074  lue to use, if t
-00000450: 6865 7265 2069 7320 6e6f 206d 6174 6368  here is no match
-00000460: 0a64 6566 6175 6c74 203d 2022 220a       .default = "".
+00000010: 7420 3d20 2230 2e34 2e31 7263 3122 0a0a  t = "0.4.1rc1"..
+00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
+00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
+00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
+00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
+00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
+00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
+00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
+00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
+000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
+000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
+000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
+000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
+000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
+000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
+00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
+00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
+00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
+00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
+00000140: 2242 756d 7020 7665 7273 696f 6e3a 2030  "Bump version: 0
+00000150: 2e34 2e31 7263 3120 e286 9220 7b6e 6577  .4.1rc1 ... {new
+00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
+00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
+00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
+00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
+000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
+000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
+000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
+000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
+000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
+000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
+00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
+00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
+00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
+00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
+00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
+00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
+00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
+00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
+00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
+00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
+000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
+000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
+000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
+000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
+000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
+000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
+00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
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

### Comparing `itkdb-0.4.1/ci/pre-commit-update.sh` & `itkdb-0.4.1rc1/ci/pre-commit-update.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/config.md` & `itkdb-0.4.1rc1/docs/config.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/examples.md` & `itkdb-0.4.1rc1/docs/examples.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/history.md` & `itkdb-0.4.1rc1/docs/history.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/index.md` & `itkdb-0.4.1rc1/docs/index.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/install.md` & `itkdb-0.4.1rc1/docs/install.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/assets/css/custom.css` & `itkdb-0.4.1rc1/docs/assets/css/custom.css`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/assets/images/logo.svg` & `itkdb-0.4.1rc1/docs/assets/images/logo.svg`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/meta/faq.md` & `itkdb-0.4.1rc1/docs/meta/faq.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/docs/reference/gen_ref_nav.py` & `itkdb-0.4.1rc1/docs/reference/gen_ref_nav.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/client.py` & `itkdb-0.4.1rc1/src/itkdb/client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/commandline.py` & `itkdb-0.4.1rc1/src/itkdb/commandline.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/core.py` & `itkdb-0.4.1rc1/src/itkdb/core.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/exceptions.py` & `itkdb-0.4.1rc1/src/itkdb/exceptions.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/responses.py` & `itkdb-0.4.1rc1/src/itkdb/responses.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/utils.py` & `itkdb-0.4.1rc1/src/itkdb/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/caching/adapter.py` & `itkdb-0.4.1rc1/src/itkdb/caching/adapter.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/caching/controller.py` & `itkdb-0.4.1rc1/src/itkdb/caching/controller.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/caching/utils.py` & `itkdb-0.4.1rc1/src/itkdb/caching/utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/data/1x1.sh` & `itkdb-0.4.1rc1/src/itkdb/data/1x1.sh`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/data/CERN_chain.pem` & `itkdb-0.4.1rc1/src/itkdb/data/CERN_chain.pem`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/data/README.md` & `itkdb-0.4.1rc1/src/itkdb/data/README.md`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/models/file.py` & `itkdb-0.4.1rc1/src/itkdb/models/file.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/src/itkdb/models/institution.py` & `itkdb-0.4.1rc1/src/itkdb/models/institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/conftest.py` & `itkdb-0.4.1rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_cli.py` & `itkdb-0.4.1rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_client.py` & `itkdb-0.4.1rc1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_image.py` & `itkdb-0.4.1rc1/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_response.py` & `itkdb-0.4.1rc1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_scripts.py` & `itkdb-0.4.1rc1/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_session.py` & `itkdb-0.4.1rc1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_user.py` & `itkdb-0.4.1rc1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/test_utils.py` & `itkdb-0.4.1rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_attachments.py` & `itkdb-0.4.1rc1/tests/integration/test_attachments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_binaryData.py` & `itkdb-0.4.1rc1/tests/integration/test_binaryData.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_cache.py` & `itkdb-0.4.1rc1/tests/integration/test_cache.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_components.py` & `itkdb-0.4.1rc1/tests/integration/test_components.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_institution.py` & `itkdb-0.4.1rc1/tests/integration/test_institution.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_session.py` & `itkdb-0.4.1rc1/tests/integration/test_session.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_shipments.py` & `itkdb-0.4.1rc1/tests/integration/test_shipments.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_summary.py` & `itkdb-0.4.1rc1/tests/integration/test_summary.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_testproperties.py` & `itkdb-0.4.1rc1/tests/integration/test_testproperties.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_tests.py` & `itkdb-0.4.1rc1/tests/integration/test_tests.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_user.py` & `itkdb-0.4.1rc1/tests/integration/test_user.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/test_warning.py` & `itkdb-0.4.1rc1/tests/integration/test_warning.py`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_attachments.test_add_attachment.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_add_attachment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_attachments.test_list_all_attachments.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_image.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_image_model_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_plainText.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_plainText.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_get_zipfile.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_binaryData.test_issue4.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_binaryData.test_issue4.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_add_comment.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_add_comment.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_bulk.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_bulk.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_info_code.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_code.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_get_component_info_serial.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_get_component_info_serial.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_components_componentTypev2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_componentsv1.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv1.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_components.test_list_componentsv2.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_components.test_list_componentsv2.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_institution.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_institution.test_pagination.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_institution.test_pagination.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_projects.test_list_projects.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_projects.test_list_projects.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listComponentTypes.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInstitutions.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_scripts.test_getInventory.listInventory.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_session.test_fake_route.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_fake_route.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_session.test_invalid_project.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_invalid_project.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_session.test_missing_required.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_missing_required.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_session.test_no_bearer.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_session.test_no_bearer.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_shipments.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_stats.test_get.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_stats.test_get.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_summary.test_get_summary.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_summary.test_get_summary.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_testproperties.test_delete_test_property.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_create_attachment_image_eos.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_tests.test_list_test_types.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_tests.test_list_test_types.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_anonymous_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_anonymous_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_bad_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_bad_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_user.test_user_good_login.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_user.test_user_good_login.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/tests/integration/cassettes/test_warnings.test_get_component.json` & `itkdb-0.4.1rc1/tests/integration/cassettes/test_warnings.test_get_component.json`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/.gitignore` & `itkdb-0.4.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/COPYING` & `itkdb-0.4.1rc1/COPYING`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/LICENSE` & `itkdb-0.4.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/README.md` & `itkdb-0.4.1rc1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# ITk DB v0.4.1
+# ITk DB v0.4.1rc1
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

### Comparing `itkdb-0.4.1/pyproject.toml` & `itkdb-0.4.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `itkdb-0.4.1/PKG-INFO` & `itkdb-0.4.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itkdb
-Version: 0.4.1
+Version: 0.4.1rc1
 Summary: Python wrapper to interface with ITk DB.
 Project-URL: Documentation, https://itkdb.docs.cern.ch/0.4/
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/sw/db/itkdb
 Author-email: Giordon Stark <kratsg@gmail.com>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>
@@ -41,15 +41,15 @@
 Requires-Dist: urllib3>=1.26.11
 Provides-Extra: contrib
 Requires-Dist: html2text; extra == 'contrib'
 Provides-Extra: eos
 Requires-Dist: pycurl; extra == 'eos'
 Description-Content-Type: text/markdown
 
-# ITk DB v0.4.1
+# ITk DB v0.4.1rc1
 
 Python wrapper around the ITk Production Database API.
 
 ---
 
 <!-- sync the following div with docs/index.md -->
 <div align="center">
```

