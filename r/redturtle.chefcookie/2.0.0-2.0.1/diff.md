# Comparing `tmp/redturtle.chefcookie-2.0.0.tar.gz` & `tmp/redturtle.chefcookie-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redturtle.chefcookie-2.0.0.tar", last modified: Tue Aug 16 10:50:02 2022, max compression
+gzip compressed data, was "redturtle.chefcookie-2.0.1.tar", last modified: Tue Nov  8 16:44:09 2022, max compression
```

## Comparing `redturtle.chefcookie-2.0.0.tar` & `redturtle.chefcookie-2.0.1.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.250787 redturtle.chefcookie-2.0.0/
--rw-r--r--   0 cekk       (501) staff       (20)     2065 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       58 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)      586 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      660 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      503 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     5871 2022-08-16 10:50:02.251336 redturtle.chefcookie-2.0.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     1362 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.228174 redturtle.chefcookie-2.0.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7901 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       83 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)      352 2022-08-16 10:50:02.251877 redturtle.chefcookie-2.0.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2447 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.221760 redturtle.chefcookie-2.0.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.228505 redturtle.chefcookie-2.0.0/src/redturtle/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.233096 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/
--rw-r--r--   0 cekk       (501) staff       (20)      137 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.234696 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     4054 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py
--rw-r--r--   0 cekk       (501) staff       (20)     1508 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      888 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/controlpanel.py
--rw-r--r--   0 cekk       (501) staff       (20)    18192 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/cookie_config.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.234980 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/overrides/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.236302 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.240121 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/
--rw-r--r--   0 cekk       (501) staff       (20)      368 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/.babelrc
--rw-r--r--   0 cekk       (501) staff       (20)      437 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/.eslintrc.js
--rw-r--r--   0 cekk       (501) staff       (20)      202 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/.gitignore
--rw-r--r--   0 cekk       (501) staff       (20)        8 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/.nvmrc
--rw-r--r--   0 cekk       (501) staff       (20)      183 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/.prettierrc
--rw-r--r--   0 cekk       (501) staff       (20)     1071 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE
--rw-r--r--   0 cekk       (501) staff       (20)    21073 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/README.md
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.241948 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/
--rw-r--r--   0 cekk       (501) staff       (20)     1912 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js
--rw-r--r--   0 cekk       (501) staff       (20)    87005 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.242656 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/
--rw-r--r--   0 cekk       (501) staff       (20)     5864 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html
--rw-r--r--   0 cekk       (501) staff       (20)    11340 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js
--rw-r--r--   0 cekk       (501) staff       (20)   933160 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js
--rw-r--r--   0 cekk       (501) staff       (20)     3924 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/package.json
--rw-r--r--   0 cekk       (501) staff       (20)   810910 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock
--rw-r--r--   0 cekk       (501) staff       (20)     1969 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/cookie-settings.png
--rw-r--r--   0 cekk       (501) staff       (20)    19718 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js
--rw-r--r--   0 cekk       (501) staff       (20)    11501 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js
--rw-r--r--   0 cekk       (501) staff       (20)     7376 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/styles.css
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.242958 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/templates/
--rw-r--r--   0 cekk       (501) staff       (20)      309 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/templates/get_chefcookie_js.pt
--rw-r--r--   0 cekk       (501) staff       (20)     2671 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/viewlets.py
--rw-r--r--   0 cekk       (501) staff       (20)     1526 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)    11801 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/defaults.py
--rw-r--r--   0 cekk       (501) staff       (20)    10151 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.244615 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.223311 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.245186 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      525 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo
--rw-r--r--   0 cekk       (501) staff       (20)     9001 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.223586 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.245773 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)     6459 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo
--rw-r--r--   0 cekk       (501) staff       (20)    12413 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po
--rw-r--r--   0 cekk       (501) staff       (20)      643 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/manual.pot
--rw-r--r--   0 cekk       (501) staff       (20)     9060 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot
--rw-r--r--   0 cekk       (501) staff       (20)     1756 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      516 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      273 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.223955 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.247486 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      186 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      532 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/controlpanel.xml
--rw-r--r--   0 cekk       (501) staff       (20)      195 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/metadata.xml
--rw-r--r--   0 cekk       (501) staff       (20)      218 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/registry.xml
--rw-r--r--   0 cekk       (501) staff       (20)      118 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.247774 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      130 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.248526 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      438 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/restapi/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      494 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/restapi/get.py
--rw-r--r--   0 cekk       (501) staff       (20)     1024 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     1595 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.249265 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.249526 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/robot/
--rw-r--r--   0 cekk       (501) staff       (20)     2011 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/robot/test_example.robot
--rw-r--r--   0 cekk       (501) staff       (20)      955 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/test_robot.py
--rw-r--r--   0 cekk       (501) staff       (20)     2428 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/test_setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.250553 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/
--rw-r--r--   0 cekk       (501) staff       (20)      396 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     2632 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/adapters.py
--rw-r--r--   0 cekk       (501) staff       (20)      605 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     4704 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/transform.py
--rw-r--r--   0 cekk       (501) staff       (20)     3037 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/upgrades.py
--rw-r--r--   0 cekk       (501) staff       (20)      798 2022-08-16 10:50:01.000000 redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/upgrades.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-08-16 10:50:02.230564 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     5871 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3990 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      145 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       10 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      218 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)       10 2022-08-16 10:50:02.000000 redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.809518 redturtle.chefcookie-2.0.1/
+-rw-r--r--   0 cekk       (501) staff       (20)     2159 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       58 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      586 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      660 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      503 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)     5991 2022-11-08 16:44:09.809677 redturtle.chefcookie-2.0.1/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     1362 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.788282 redturtle.chefcookie-2.0.1/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7901 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       83 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      352 2022-11-08 16:44:09.810145 redturtle.chefcookie-2.0.1/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2411 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.782801 redturtle.chefcookie-2.0.1/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.788533 redturtle.chefcookie-2.0.1/src/redturtle/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.793262 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/
+-rw-r--r--   0 cekk       (501) staff       (20)      137 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.794890 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4054 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1508 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      888 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/controlpanel.py
+-rw-r--r--   0 cekk       (501) staff       (20)    18192 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/cookie_config.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.795125 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/overrides/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/overrides/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.796291 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/.gitkeep
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.800084 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/
+-rw-r--r--   0 cekk       (501) staff       (20)      368 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/.babelrc
+-rw-r--r--   0 cekk       (501) staff       (20)      437 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/.eslintrc.js
+-rw-r--r--   0 cekk       (501) staff       (20)      202 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/.gitignore
+-rw-r--r--   0 cekk       (501) staff       (20)        8 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/.nvmrc
+-rw-r--r--   0 cekk       (501) staff       (20)      183 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/.prettierrc
+-rw-r--r--   0 cekk       (501) staff       (20)     1071 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE
+-rw-r--r--   0 cekk       (501) staff       (20)    21073 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/README.md
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.801514 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_js/
+-rw-r--r--   0 cekk       (501) staff       (20)     1912 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js
+-rw-r--r--   0 cekk       (501) staff       (20)    87005 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.802098 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_tests/
+-rw-r--r--   0 cekk       (501) staff       (20)     5864 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html
+-rw-r--r--   0 cekk       (501) staff       (20)    11340 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js
+-rw-r--r--   0 cekk       (501) staff       (20)   933160 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js
+-rw-r--r--   0 cekk       (501) staff       (20)     3924 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/package.json
+-rw-r--r--   0 cekk       (501) staff       (20)   810910 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock
+-rw-r--r--   0 cekk       (501) staff       (20)     1969 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/cookie-settings.png
+-rw-r--r--   0 cekk       (501) staff       (20)    19718 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js
+-rw-r--r--   0 cekk       (501) staff       (20)    11501 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js
+-rw-r--r--   0 cekk       (501) staff       (20)     7376 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/styles.css
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.802341 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/templates/
+-rw-r--r--   0 cekk       (501) staff       (20)      309 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/templates/get_chefcookie_js.pt
+-rw-r--r--   0 cekk       (501) staff       (20)     2671 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/viewlets.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1526 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    11801 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/defaults.py
+-rw-r--r--   0 cekk       (501) staff       (20)    10151 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.803855 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.784255 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.804324 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)      525 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)     9001 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.784539 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.804887 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)     6459 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo
+-rw-r--r--   0 cekk       (501) staff       (20)    12413 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po
+-rw-r--r--   0 cekk       (501) staff       (20)      643 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/manual.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     9060 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot
+-rw-r--r--   0 cekk       (501) staff       (20)     1756 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      516 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.784941 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.806367 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      186 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      105 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      532 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/controlpanel.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      195 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      218 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      118 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.806664 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      130 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/uninstall/browserlayer.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.807336 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/restapi/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      438 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/restapi/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      494 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/restapi/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1024 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1595 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.808068 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.808297 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/robot/
+-rw-r--r--   0 cekk       (501) staff       (20)     2011 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/robot/test_example.robot
+-rw-r--r--   0 cekk       (501) staff       (20)      955 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/test_robot.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2428 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/test_setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.809306 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/
+-rw-r--r--   0 cekk       (501) staff       (20)      396 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2632 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/adapters.py
+-rw-r--r--   0 cekk       (501) staff       (20)      605 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     4704 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/transform.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3037 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)      798 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/upgrades.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2022-11-08 16:44:09.790721 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)     5991 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     3990 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      145 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      218 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       10 2022-11-08 16:44:09.000000 redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/top_level.txt
```

### Comparing `redturtle.chefcookie-2.0.0/CHANGES.rst` & `redturtle.chefcookie-2.0.1/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2.0.1 (2022-11-08)
+------------------
+
+- Remove unused python_requires in setup.py
+  [cekk]
+
+
 2.0.0 (2022-08-16)
 ------------------
 
 - [BREAKING CHANGE] Store list of accepted_providers in ascii-way. If you update to this version, you need to force re-accept cookies for example using a different prefix.
   [cekk]
```

### Comparing `redturtle.chefcookie-2.0.0/DEVELOP.rst` & `redturtle.chefcookie-2.0.1/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/LICENSE.GPL` & `redturtle.chefcookie-2.0.1/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/LICENSE.rst` & `redturtle.chefcookie-2.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/PKG-INFO` & `redturtle.chefcookie-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.chefcookie
-Version: 2.0.0
+Version: 2.0.1
 Summary: Cookie policy integration with chefookie
 Home-page: https://github.com/collective/redturtle.chefcookie
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.chefcookie
 Project-URL: Source, https://github.com/RedTurtle/redturtle.chefcookie
@@ -79,14 +79,21 @@
         
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
+        2.0.1 (2022-11-08)
+        ------------------
+        
+        - Remove unused python_requires in setup.py
+          [cekk]
+        
+        
         2.0.0 (2022-08-16)
         ------------------
         
         - [BREAKING CHANGE] Store list of accepted_providers in ascii-way. If you update to this version, you need to force re-accept cookies for example using a different prefix.
           [cekk]
         
         
@@ -181,9 +188,8 @@
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
 Provides-Extra: test
```

### Comparing `redturtle.chefcookie-2.0.0/README.rst` & `redturtle.chefcookie-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/docs/conf.py` & `redturtle.chefcookie-2.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/setup.py` & `redturtle.chefcookie-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="redturtle.chefcookie",
-    version="2.0.0",
+    version="2.0.1",
     description="Cookie policy integration with chefookie",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Plone",
@@ -44,15 +44,14 @@
     },
     license="GPL version 2",
     packages=find_packages("src", exclude=["ez_setup", "node_modules"]),
     namespace_packages=["redturtle"],
     package_dir={"": "src"},
     include_package_data=True,
     zip_safe=False,
-    python_requires="==2.7, >=3.6",
     install_requires=[
         "setuptools",
         "plone.api",
         "BeautifulSoup4==4.9.3;python_version<'3'",
         "BeautifulSoup4>=4.9.3;python_version>='3'",
     ],
     extras_require={
```

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/chefcookie_consent_registry.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/configure.zcml` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/controlpanel.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/controlpanel.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/cookie_config.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/cookie_config.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/LICENSE`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/README.md` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/README.md`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_js/_helper.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_js/script.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_tests/index.html`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/_tests/script.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/chefcookie.min.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/package.json` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/package.json`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/chefcookie/yarn.lock`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/cookie-settings.png` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/cookie-settings.png`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/redturtle_chefcookie.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/redturtle_chefcookie_tech.js`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/static/styles.css` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/static/styles.css`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/browser/viewlets.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/configure.zcml` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/defaults.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/defaults.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/interfaces.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/interfaces.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/README.rst` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/README.rst`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.mo`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/en/LC_MESSAGES/redturtle.chefcookie.po`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.mo`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/it/LC_MESSAGES/redturtle.chefcookie.po`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/manual.pot` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/manual.pot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/redturtle.chefcookie.pot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/update.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/update.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/locales/update.sh` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/locales/update.sh`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/profiles/default/controlpanel.xml` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/profiles/default/controlpanel.xml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/setuphandlers.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/testing.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/testing.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/robot/test_example.robot` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/test_robot.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/test_robot.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/tests/test_setup.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/adapters.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/adapters.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/configure.zcml` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/configure.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/transformers/transform.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/transformers/transform.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/upgrades.py` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/upgrades.py`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle/chefcookie/upgrades.zcml` & `redturtle.chefcookie-2.0.1/src/redturtle/chefcookie/upgrades.zcml`

 * *Files identical despite different names*

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/PKG-INFO` & `redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redturtle.chefcookie
-Version: 2.0.0
+Version: 2.0.1
 Summary: Cookie policy integration with chefookie
 Home-page: https://github.com/collective/redturtle.chefcookie
 Author: RedTurtle
 Author-email: info@redturtle.it
 License: GPL version 2
 Project-URL: PyPI, https://pypi.python.org/pypi/redturtle.chefcookie
 Project-URL: Source, https://github.com/RedTurtle/redturtle.chefcookie
@@ -79,14 +79,21 @@
         
         - RedTurtle, info@redturtle.it
         
         
         Changelog
         =========
         
+        2.0.1 (2022-11-08)
+        ------------------
+        
+        - Remove unused python_requires in setup.py
+          [cekk]
+        
+        
         2.0.0 (2022-08-16)
         ------------------
         
         - [BREAKING CHANGE] Store list of accepted_providers in ascii-way. If you update to this version, you need to force re-accept cookies for example using a different prefix.
           [cekk]
         
         
@@ -181,9 +188,8 @@
 Classifier: Framework :: Plone :: 5.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Requires-Python: ==2.7, >=3.6
 Provides-Extra: test
```

### Comparing `redturtle.chefcookie-2.0.0/src/redturtle.chefcookie.egg-info/SOURCES.txt` & `redturtle.chefcookie-2.0.1/src/redturtle.chefcookie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

