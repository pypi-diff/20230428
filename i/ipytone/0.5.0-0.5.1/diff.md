# Comparing `tmp/ipytone-0.5.0.tar.gz` & `tmp/ipytone-0.5.1.tar.gz`

## Comparing `ipytone-0.5.0.tar` & `ipytone-0.5.1.tar`

### file list

```diff
@@ -1,132 +1,131 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ipytone-0.5.0/.coveragerc
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipytone-0.5.0/.eslintignore
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 ipytone-0.5.0/.eslintrc.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipytone-0.5.0/.npmignore
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ipytone-0.5.0/.npmrc
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 ipytone-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ipytone-0.5.0/.prettierignore
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ipytone-0.5.0/.prettierrc
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 ipytone-0.5.0/.readthedocs.yaml
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 ipytone-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ipytone-0.5.0/environment-dev.yml
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ipytone-0.5.0/environment.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ipytone-0.5.0/install.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone.json
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ipytone-0.5.0/package.json
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipytone-0.5.0/setup.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ipytone-0.5.0/tsconfig.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 ipytone-0.5.0/webpack.config.js
--rw-r--r--   0        0        0   158118 2020-02-02 00:00:00.000000 ipytone-0.5.0/yarn.lock
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/Makefile
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/advanced.md
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/api-hidden.rst
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/api.rst
--rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/audio_samples.md
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/conf.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/demo.rst
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/envelope_data1.npy
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/envelope_data2.npy
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/environment-jupyterlite.yml
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/environment.yml
--rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/getting_started.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/index.rst
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/installing.rst
--rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/instrument.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/jupyterlite_config.json
--rw-r--r--   0        0        0    57264 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/kick.wav
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/make.bat
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/observe_link.md
--rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/quick_demo.ipynb
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/release_notes.rst
--rw-r--r--   0        0        0   154000 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/snare.wav
--rw-r--r--   0        0        0    10169 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/timeline.md
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/user_guide.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_static/favicon.ico
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_static/helper.js
--rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_static/ipytone_logo_dark.svg
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_static/ipytone_logo_light.svg
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_templates/ipytone-class-template.rst
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/_templates/ipytone-module-template.rst
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.0/docs/source/_static/embed-bundle.js.LICENSE.txt
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/_frontend.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/_version.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/analysis.py
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/base.py
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/callback.py
--rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/channel.py
--rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/core.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/dynamics.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/effect.py
--rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/envelope.py
--rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/event.py
--rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/filter.py
--rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/graph.py
--rw-r--r--   0        0        0    37789 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/instrument.py
--rw-r--r--   0        0        0    13344 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/observe.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/serialization.py
--rw-r--r--   0        0        0    14393 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/signal.py
--rw-r--r--   0        0        0    29762 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/source.py
--rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/transport.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/utils.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/package.json
--rw-r--r--   0        0        0    93775 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/367.bdd52b6ea2f774bcff76.js
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/480.be1ddfc39ba5d544636f.js
--rw-r--r--   0        0        0   346407 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/488.5753e6f448307feab910.js
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/488.5753e6f448307feab910.js.LICENSE.txt
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/568.f3a0ffd66144f0685fb9.js
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/remoteEntry.689677fb9842e28f18f5.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/style.js
--rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/nbextension/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/nbextension/static/extension.js
--rw-r--r--   0        0        0   442417 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/nbextension/static/index.js
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0        0        0  2173621 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/nbextension/static/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/__init__.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/conftest.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_analysis.py
--rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_base.py
--rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_channel.py
--rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_core.py
--rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_dynamics.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_effect.py
--rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_envelope.py
--rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_event.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_filter.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_graph.py
--rw-r--r--   0        0        0    14383 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_instrument.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_nbextension_path.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_observe.py
--rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_signal.py
--rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_source.py
--rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_transport.py
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ipytone-0.5.0/ipytone/tests/test_utils.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/extension.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/index.ts
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/plugin.ts
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/serializers.ts
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/utils.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/version.ts
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget.ts
--rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_analysis.ts
--rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_base.ts
--rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_channel.ts
--rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_core.ts
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_dynamics.ts
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_effect.ts
--rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_envelope.ts
--rw-r--r--   0        0        0    12232 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_event.ts
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_filter.ts
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_graph.ts
--rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_instrument.ts
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_observe.ts
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_signal.ts
--rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_source.ts
--rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 ipytone-0.5.0/src/widget_transport.ts
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 ipytone-0.5.0/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ipytone-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ipytone-0.5.0/README.md
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 ipytone-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ipytone-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 ipytone-0.5.1/.coveragerc
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 ipytone-0.5.1/.eslintignore
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 ipytone-0.5.1/.eslintrc.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipytone-0.5.1/.npmignore
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 ipytone-0.5.1/.npmrc
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 ipytone-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 ipytone-0.5.1/.prettierignore
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 ipytone-0.5.1/.prettierrc
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 ipytone-0.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 ipytone-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 ipytone-0.5.1/environment-dev.yml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 ipytone-0.5.1/environment.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 ipytone-0.5.1/install.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone.json
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 ipytone-0.5.1/package.json
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipytone-0.5.1/setup.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ipytone-0.5.1/tsconfig.json
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 ipytone-0.5.1/webpack.config.js
+-rw-r--r--   0        0        0   158118 2020-02-02 00:00:00.000000 ipytone-0.5.1/yarn.lock
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/advanced.md
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/api-hidden.rst
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/api.rst
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/audio_samples.md
+-rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/demo.rst
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/envelope_data1.npy
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/envelope_data2.npy
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/environment-jupyterlite.yml
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/environment.yml
+-rw-r--r--   0        0        0     7938 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/getting_started.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/installing.rst
+-rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/instrument.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/jupyterlite_config.json
+-rw-r--r--   0        0        0    57264 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/kick.wav
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/make.bat
+-rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/observe_link.md
+-rw-r--r--   0        0        0     9312 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/quick_demo.ipynb
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/release_notes.rst
+-rw-r--r--   0        0        0   154000 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/snare.wav
+-rw-r--r--   0        0        0    10169 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/timeline.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/user_guide.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_static/favicon.ico
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_static/helper.js
+-rw-r--r--   0        0        0     3576 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_static/ipytone_logo_dark.svg
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_static/ipytone_logo_light.svg
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_templates/ipytone-class-template.rst
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/_templates/ipytone-module-template.rst
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.1/docs/source/_static/embed-bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/_frontend.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/_version.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/analysis.py
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/base.py
+-rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/callback.py
+-rw-r--r--   0        0        0    15424 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/channel.py
+-rw-r--r--   0        0        0    22074 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/core.py
+-rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/dynamics.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/effect.py
+-rw-r--r--   0        0        0     4935 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/envelope.py
+-rw-r--r--   0        0        0    13186 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/event.py
+-rw-r--r--   0        0        0    12498 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/filter.py
+-rw-r--r--   0        0        0     4772 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/graph.py
+-rw-r--r--   0        0        0    37789 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/instrument.py
+-rw-r--r--   0        0        0    13344 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/observe.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/serialization.py
+-rw-r--r--   0        0        0    14393 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/signal.py
+-rw-r--r--   0        0        0    29762 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/source.py
+-rw-r--r--   0        0        0    12966 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/transport.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/utils.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/package.json
+-rw-r--r--   0        0        0    93775 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/367.7d2ea1a518646959ac15.js
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/480.be1ddfc39ba5d544636f.js
+-rw-r--r--   0        0        0   346407 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/488.5753e6f448307feab910.js
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/488.5753e6f448307feab910.js.LICENSE.txt
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/568.f3a0ffd66144f0685fb9.js
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/remoteEntry.e41cd2b06af3a21c8dc3.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/style.js
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/nbextension/extension.js
+-rw-r--r--   0        0        0   442417 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/nbextension/index.js
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/nbextension/index.js.LICENSE.txt
+-rw-r--r--   0        0        0  2173621 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/__init__.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/conftest.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_analysis.py
+-rw-r--r--   0        0        0     5474 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_base.py
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_channel.py
+-rw-r--r--   0        0        0     7256 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_core.py
+-rw-r--r--   0        0        0     2957 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_dynamics.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_effect.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_envelope.py
+-rw-r--r--   0        0        0    10159 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_event.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_filter.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_graph.py
+-rw-r--r--   0        0        0    14383 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_instrument.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_observe.py
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_signal.py
+-rw-r--r--   0        0        0    12158 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_source.py
+-rw-r--r--   0        0        0     5583 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_transport.py
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 ipytone-0.5.1/ipytone/tests/test_utils.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/extension.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/index.ts
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/plugin.ts
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/serializers.ts
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/utils.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/version.ts
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget.ts
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_analysis.ts
+-rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_base.ts
+-rw-r--r--   0        0        0     6955 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_channel.ts
+-rw-r--r--   0        0        0    14124 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_core.ts
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_dynamics.ts
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_effect.ts
+-rw-r--r--   0        0        0     5433 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_envelope.ts
+-rw-r--r--   0        0        0    12232 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_event.ts
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_filter.ts
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_graph.ts
+-rw-r--r--   0        0        0    15442 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_instrument.ts
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_observe.ts
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_signal.ts
+-rw-r--r--   0        0        0    21625 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_source.ts
+-rw-r--r--   0        0        0     7411 2020-02-02 00:00:00.000000 ipytone-0.5.1/src/widget_transport.ts
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 ipytone-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 ipytone-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 ipytone-0.5.1/README.md
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 ipytone-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4553 2020-02-02 00:00:00.000000 ipytone-0.5.1/PKG-INFO
```

### Comparing `ipytone-0.5.0/.eslintrc.json` & `ipytone-0.5.1/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/.pre-commit-config.yaml` & `ipytone-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/MANIFEST.in` & `ipytone-0.5.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/package.json` & `ipytone-0.5.1/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.5.1'"}*

```diff
@@ -87,9 +87,9 @@
         "prettier:check": "prettier --ignore-path .gitignore --check \"**/*{.ts,.tsx,.js,.jsx,.css,.json}\"",
         "watch": "run-p watch:lib watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `ipytone-0.5.0/webpack.config.js` & `ipytone-0.5.1/webpack.config.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
      * This bundle only contains the part of the JavaScript that is run on load of
      * the notebook.
      */
     {
         entry: './src/extension.ts',
         output: {
             filename: 'index.js',
-            path: path.resolve(__dirname, 'ipytone', 'nbextension', 'static'),
+            path: path.resolve(__dirname, 'ipytone', 'nbextension'),
             libraryTarget: 'amd',
         },
         module: {
             rules: rules,
         },
         devtool: 'source-map',
         externals,
```

### Comparing `ipytone-0.5.0/yarn.lock` & `ipytone-0.5.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/Makefile` & `ipytone-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/api.rst` & `ipytone-0.5.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/audio_samples.md` & `ipytone-0.5.1/docs/audio_samples.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/conf.py` & `ipytone-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/envelope_data1.npy` & `ipytone-0.5.1/docs/envelope_data1.npy`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/envelope_data2.npy` & `ipytone-0.5.1/docs/envelope_data2.npy`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/getting_started.md` & `ipytone-0.5.1/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/index.rst` & `ipytone-0.5.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/installing.rst` & `ipytone-0.5.1/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/instrument.md` & `ipytone-0.5.1/docs/instrument.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/kick.wav` & `ipytone-0.5.1/docs/kick.wav`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/make.bat` & `ipytone-0.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/observe_link.md` & `ipytone-0.5.1/docs/observe_link.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/quick_demo.ipynb` & `ipytone-0.5.1/docs/quick_demo.ipynb`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/release_notes.rst` & `ipytone-0.5.1/docs/release_notes.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 .. _release_notes:
 
 .. currentmodule:: ipytone
 
 Release Notes
 =============
 
+v0.5.1
+------
+
+Bug fixes
+~~~~~~~~~
+
+- Fixed installation issue with notebook "classic" version <7 (:issue:`109`,
+  :pull:`110`).
+
 v0.5.0
 ------
 
 Deprecated features
 ~~~~~~~~~~~~~~~~~~~
 
 - ``ipytone.destination`` is deprecated, use :py:func:`get_destination`
```

### Comparing `ipytone-0.5.0/docs/snare.wav` & `ipytone-0.5.1/docs/snare.wav`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/timeline.md` & `ipytone-0.5.1/docs/timeline.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/user_guide.rst` & `ipytone-0.5.1/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/_static/favicon.ico` & `ipytone-0.5.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/_static/ipytone_logo_dark.svg` & `ipytone-0.5.1/docs/_static/ipytone_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/_static/ipytone_logo_light.svg` & `ipytone-0.5.1/docs/_static/ipytone_logo_light.svg`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/_templates/ipytone-class-template.rst` & `ipytone-0.5.1/docs/_templates/ipytone-class-template.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/docs/_templates/ipytone-module-template.rst` & `ipytone-0.5.1/docs/_templates/ipytone-module-template.rst`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/__init__.py` & `ipytone-0.5.1/ipytone/__init__.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/analysis.py` & `ipytone-0.5.1/ipytone/analysis.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/base.py` & `ipytone-0.5.1/ipytone/base.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/callback.py` & `ipytone-0.5.1/ipytone/callback.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/channel.py` & `ipytone-0.5.1/ipytone/channel.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/core.py` & `ipytone-0.5.1/ipytone/core.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/dynamics.py` & `ipytone-0.5.1/ipytone/dynamics.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/effect.py` & `ipytone-0.5.1/ipytone/effect.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/envelope.py` & `ipytone-0.5.1/ipytone/envelope.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/event.py` & `ipytone-0.5.1/ipytone/event.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/filter.py` & `ipytone-0.5.1/ipytone/filter.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/graph.py` & `ipytone-0.5.1/ipytone/graph.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/instrument.py` & `ipytone-0.5.1/ipytone/instrument.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/observe.py` & `ipytone-0.5.1/ipytone/observe.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/serialization.py` & `ipytone-0.5.1/ipytone/serialization.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/signal.py` & `ipytone-0.5.1/ipytone/signal.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/source.py` & `ipytone-0.5.1/ipytone/source.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/transport.py` & `ipytone-0.5.1/ipytone/transport.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/utils.py` & `ipytone-0.5.1/ipytone/utils.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/labextension/package.json` & `ipytone-0.5.1/ipytone/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.e41cd2b06af3a21c8dc3.js'}}",*

 * * "'version'": "'0.5.1'"}*

```diff
@@ -41,15 +41,15 @@
         "dist/*.d.ts",
         "css/*.css"
     ],
     "homepage": "https://github.com/benbovy/ipytone",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.689677fb9842e28f18f5.js"
+            "load": "static/remoteEntry.e41cd2b06af3a21c8dc3.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipytone/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -91,9 +91,9 @@
         "prettier:check": "prettier --ignore-path .gitignore --check \"**/*{.ts,.tsx,.js,.jsx,.css,.json}\"",
         "watch": "run-p watch:lib watch:nbextension",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.5.0"
+    "version": "0.5.1"
 }
```

### Comparing `ipytone-0.5.0/ipytone/labextension/static/367.bdd52b6ea2f774bcff76.js` & `ipytone-0.5.1/ipytone/labextension/static/367.7d2ea1a518646959ac15.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -3784,11 +3784,11 @@
             exports.TransportModel = TransportModel, TransportModel.serializers = Object.assign(Object.assign({}, widget_base_1.ToneObjectModel.serializers), {
                 _bpm: {
                     deserialize: base_1.unpack_models
                 }
             }), TransportModel.model_name = "TransportModel"
         },
         147: e => {
-            e.exports = JSON.parse('{"name":"ipytone","version":"0.5.0","description":"Interactive audio in Jupyter","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","css/*.css"],"homepage":"https://github.com/benbovy/ipytone","bugs":{"url":"https://github.com/benbovy/ipytone/issues"},"license":"BSD-3-Clause","author":{"name":"Benoit Bovy","email":"benbovy@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/benbovy/ipytone.git"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:lib":"tsc","build:nbextension":"webpack","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:extensions":"yarn run build && yarn run build:labextension","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:nbextension":"rimraf ipytone/nbextension/static/index.js","clean:labextension":"rimraf ipytone/labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:labextension:dev":"jupyter labextension develop --overwrite .","lint":"yarn && yarn run prettier && yarn run eslint","lint:check":"yarn run prettier:check && yarn run eslint:check","prettier":"prettier --ignore-path .gitignore --write \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prettier:check":"prettier --ignore-path .gitignore --check \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prepack":"yarn run build:lib","watch":"run-p watch:lib watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/base-manager":"^1.0.4","tone":"~14.7.77"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^6.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.3.1","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^3.0.0-alpha.6","rimraf":"^2.6.2","source-map-loader":"^0.2.4","ts-loader":"^8","typescript":"~4","webpack":"^5","webpack-cli":"^4"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipytone/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipytone","version":"0.5.1","description":"Interactive audio in Jupyter","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","css/*.css"],"homepage":"https://github.com/benbovy/ipytone","bugs":{"url":"https://github.com/benbovy/ipytone/issues"},"license":"BSD-3-Clause","author":{"name":"Benoit Bovy","email":"benbovy@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/benbovy/ipytone.git"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:lib":"tsc","build:nbextension":"webpack","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:extensions":"yarn run build && yarn run build:labextension","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:nbextension":"rimraf ipytone/nbextension/static/index.js","clean:labextension":"rimraf ipytone/labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:labextension:dev":"jupyter labextension develop --overwrite .","lint":"yarn && yarn run prettier && yarn run eslint","lint:check":"yarn run prettier:check && yarn run eslint:check","prettier":"prettier --ignore-path .gitignore --write \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prettier:check":"prettier --ignore-path .gitignore --check \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prepack":"yarn run build:lib","watch":"run-p watch:lib watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/base-manager":"^1.0.4","tone":"~14.7.77"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^6.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.3.1","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^3.0.0-alpha.6","rimraf":"^2.6.2","source-map-loader":"^0.2.4","ts-loader":"^8","typescript":"~4","webpack":"^5","webpack-cli":"^4"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipytone/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipytone-0.5.0/ipytone/labextension/static/480.be1ddfc39ba5d544636f.js` & `ipytone-0.5.1/ipytone/labextension/static/480.be1ddfc39ba5d544636f.js`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/labextension/static/488.5753e6f448307feab910.js` & `ipytone-0.5.1/ipytone/labextension/static/488.5753e6f448307feab910.js`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/labextension/static/568.f3a0ffd66144f0685fb9.js` & `ipytone-0.5.1/ipytone/labextension/static/568.f3a0ffd66144f0685fb9.js`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/labextension/static/remoteEntry.689677fb9842e28f18f5.js` & `ipytone-0.5.1/ipytone/labextension/static/remoteEntry.e41cd2b06af3a21c8dc3.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -36,20 +36,20 @@
     }
     w.m = b, w.c = y, w.d = (e, r) => {
         for (var t in r) w.o(r, t) && !w.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, w.f = {}, w.e = e => Promise.all(Object.keys(w.f).reduce(((r, t) => (w.f[t](e, r), r)), [])), w.u = e => e + "." + {
-        367: "bdd52b6ea2f774bcff76",
+        367: "7d2ea1a518646959ac15",
         480: "be1ddfc39ba5d544636f",
         488: "5753e6f448307feab910",
         568: "f3a0ffd66144f0685fb9"
     } [e] + ".js?v=" + {
-        367: "bdd52b6ea2f774bcff76",
+        367: "7d2ea1a518646959ac15",
         480: "be1ddfc39ba5d544636f",
         488: "5753e6f448307feab910",
         568: "f3a0ffd66144f0685fb9"
     } [e], w.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
@@ -104,15 +104,15 @@
                         (!u || !u.loaded && (!n != !u.eager ? n : i > u.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     l = [];
-                return "default" === t && (u("ipytone", "0.5.0", (() => Promise.all([w.e(367), w.e(568)]).then((() => () => w(568))))), u("tone", "14.7.77", (() => w.e(488).then((() => () => w(488)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("ipytone", "0.5.1", (() => Promise.all([w.e(367), w.e(568)]).then((() => () => w(568))))), u("tone", "14.7.77", (() => w.e(488).then((() => () => w(488)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         w.g.importScripts && (e = w.g.location + "");
         var r = w.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `ipytone-0.5.0/ipytone/labextension/static/third-party-licenses.json` & `ipytone-0.5.1/ipytone/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/nbextension/static/index.js` & `ipytone-0.5.1/ipytone/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -17705,15 +17705,15 @@
                         var s = Object.prototype.toString.call(e).slice(8, -1);
                         return "Object" === s && e.constructor && (s = e.constructor.name), "Map" === s || "Set" === s ? Array.from(e) : "Arguments" === s || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(s) ? n(e, t) : void 0
                     }
                 }, e.exports.__esModule = !0, e.exports.default = e.exports
             },
             147: e => {
                 "use strict";
-                e.exports = JSON.parse('{"name":"ipytone","version":"0.5.0","description":"Interactive audio in Jupyter","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","css/*.css"],"homepage":"https://github.com/benbovy/ipytone","bugs":{"url":"https://github.com/benbovy/ipytone/issues"},"license":"BSD-3-Clause","author":{"name":"Benoit Bovy","email":"benbovy@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/benbovy/ipytone.git"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:lib":"tsc","build:nbextension":"webpack","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:extensions":"yarn run build && yarn run build:labextension","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:nbextension":"rimraf ipytone/nbextension/static/index.js","clean:labextension":"rimraf ipytone/labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:labextension:dev":"jupyter labextension develop --overwrite .","lint":"yarn && yarn run prettier && yarn run eslint","lint:check":"yarn run prettier:check && yarn run eslint:check","prettier":"prettier --ignore-path .gitignore --write \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prettier:check":"prettier --ignore-path .gitignore --check \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prepack":"yarn run build:lib","watch":"run-p watch:lib watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/base-manager":"^1.0.4","tone":"~14.7.77"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^6.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.3.1","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^3.0.0-alpha.6","rimraf":"^2.6.2","source-map-loader":"^0.2.4","ts-loader":"^8","typescript":"~4","webpack":"^5","webpack-cli":"^4"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipytone/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+                e.exports = JSON.parse('{"name":"ipytone","version":"0.5.1","description":"Interactive audio in Jupyter","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","lib/**/*.d.ts","dist/*.js","dist/*.d.ts","css/*.css"],"homepage":"https://github.com/benbovy/ipytone","bugs":{"url":"https://github.com/benbovy/ipytone/issues"},"license":"BSD-3-Clause","author":{"name":"Benoit Bovy","email":"benbovy@gmail.com"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/benbovy/ipytone.git"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:lib":"tsc","build:nbextension":"webpack","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:extensions":"yarn run build && yarn run build:labextension","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:nbextension":"rimraf ipytone/nbextension/static/index.js","clean:labextension":"rimraf ipytone/labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:labextension:dev":"jupyter labextension develop --overwrite .","lint":"yarn && yarn run prettier && yarn run eslint","lint:check":"yarn run prettier:check && yarn run eslint:check","prettier":"prettier --ignore-path .gitignore --write \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prettier:check":"prettier --ignore-path .gitignore --check \\"**/*{.ts,.tsx,.js,.jsx,.css,.json}\\"","prepack":"yarn run build:lib","watch":"run-p watch:lib watch:nbextension","watch:lib":"tsc -w","watch:nbextension":"webpack --watch","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^6","@jupyter-widgets/base-manager":"^1.0.4","tone":"~14.7.77"},"devDependencies":{"@jupyterlab/builder":"^3.0.0","@types/node":"^10.11.6","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^6.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.3.1","expect.js":"^0.3.1","fs-extra":"^7.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^3.0.0-alpha.6","rimraf":"^2.6.2","source-map-loader":"^0.2.4","ts-loader":"^8","typescript":"~4","webpack":"^5","webpack-cli":"^4"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipytone/labextension","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
         __webpack_module_cache__ = {};
 
     function __webpack_require__(e) {
         var t = __webpack_module_cache__[e];
         if (void 0 !== t) return t.exports;
```

### Comparing `ipytone-0.5.0/ipytone/nbextension/static/index.js.map` & `ipytone-0.5.1/ipytone/nbextension/index.js.map`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/conftest.py` & `ipytone-0.5.1/ipytone/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_analysis.py` & `ipytone-0.5.1/ipytone/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_base.py` & `ipytone-0.5.1/ipytone/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_channel.py` & `ipytone-0.5.1/ipytone/tests/test_channel.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_core.py` & `ipytone-0.5.1/ipytone/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_dynamics.py` & `ipytone-0.5.1/ipytone/tests/test_dynamics.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_effect.py` & `ipytone-0.5.1/ipytone/tests/test_effect.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_envelope.py` & `ipytone-0.5.1/ipytone/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_event.py` & `ipytone-0.5.1/ipytone/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_filter.py` & `ipytone-0.5.1/ipytone/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_graph.py` & `ipytone-0.5.1/ipytone/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_instrument.py` & `ipytone-0.5.1/ipytone/tests/test_instrument.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_observe.py` & `ipytone-0.5.1/ipytone/tests/test_observe.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_signal.py` & `ipytone-0.5.1/ipytone/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_source.py` & `ipytone-0.5.1/ipytone/tests/test_source.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_transport.py` & `ipytone-0.5.1/ipytone/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/ipytone/tests/test_utils.py` & `ipytone-0.5.1/ipytone/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/extension.ts` & `ipytone-0.5.1/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/plugin.ts` & `ipytone-0.5.1/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/serializers.ts` & `ipytone-0.5.1/src/serializers.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/utils.ts` & `ipytone-0.5.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget.ts` & `ipytone-0.5.1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_analysis.ts` & `ipytone-0.5.1/src/widget_analysis.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_base.ts` & `ipytone-0.5.1/src/widget_base.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_channel.ts` & `ipytone-0.5.1/src/widget_channel.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_core.ts` & `ipytone-0.5.1/src/widget_core.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_dynamics.ts` & `ipytone-0.5.1/src/widget_dynamics.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_effect.ts` & `ipytone-0.5.1/src/widget_effect.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_envelope.ts` & `ipytone-0.5.1/src/widget_envelope.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_event.ts` & `ipytone-0.5.1/src/widget_event.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_filter.ts` & `ipytone-0.5.1/src/widget_filter.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_graph.ts` & `ipytone-0.5.1/src/widget_graph.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_instrument.ts` & `ipytone-0.5.1/src/widget_instrument.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_observe.ts` & `ipytone-0.5.1/src/widget_observe.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_signal.ts` & `ipytone-0.5.1/src/widget_signal.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_source.ts` & `ipytone-0.5.1/src/widget_source.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/src/widget_transport.ts` & `ipytone-0.5.1/src/widget_transport.ts`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/.gitignore` & `ipytone-0.5.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 *.lnk
 
 
 # NPM
 # ----
 
 **/node_modules/
-ipytone/nbextension/static/index.*
+ipytone/nbextension/index.*
 ipytone/labextension/*.tgz
 .yarn/
 
 # Coverage data
 # -------------
 **/coverage/
```

### Comparing `ipytone-0.5.0/LICENSE.txt` & `ipytone-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/README.md` & `ipytone-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ipytone-0.5.0/pyproject.toml` & `ipytone-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "ipywidgets>=7.6.0",
     "numpy",
     "traittypes",
 ]
-version = "0.5.0"
+version = "0.5.1"
 
 [project.optional-dependencies]
 test = [
     "pytest>=4.6",
     "pytest-cov",
     "pytest-mock",
     "ipykernel",
@@ -56,15 +56,15 @@
 ]
 
 [project.urls]
 Homepage = "https://github.com/benbovy/ipytone"
 
 [tool.hatch.build]
 artifacts = [
-    "ipytone/nbextension/static/index.*",
+    "ipytone/nbextension/index.*",
     "ipytone/labextension/*.tgz",
     "ipytone/labextension",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
 "ipytone/nbextension" = "share/jupyter/nbextensions/ipytone"
 "ipytone/labextension" = "share/jupyter/labextensions/ipytone"
@@ -75,19 +75,19 @@
 exclude = [
     ".github",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
-    "ipytone/nbextension/static/index.js",
+    "ipytone/nbextension/index.js",
     "ipytone/labextension/package.json",
 ]
 skip-if-exists = [
-    "ipytone/nbextension/static/index.js",
+    "ipytone/nbextension/index.js",
     "ipytone/labextension/package.json",
 ]
 dependencies = [
     "hatch-jupyter-builder>=0.8.2",
 ]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
```

### Comparing `ipytone-0.5.0/PKG-INFO` & `ipytone-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipytone
-Version: 0.5.0
+Version: 0.5.1
 Summary: Interactive audio in Jupyter
 Project-URL: Homepage, https://github.com/benbovy/ipytone
 Author: Benoît Bovy
 License: Copyright (c) 2020 Benoit Bovy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

