# Comparing `tmp/jupyterlab_daw-0.1.0.tar.gz` & `tmp/jupyterlab_daw-0.2.0.tar.gz`

## Comparing `jupyterlab_daw-0.1.0.tar` & `jupyterlab_daw-0.2.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.dir-locals.el
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.eslintignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.eslintrc.js
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.prettierrc
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.stylelintrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/babel.config.js
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/install.json
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jest.config.js
--rw-r--r--   0        0        0     3798 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/setup.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/tsconfig.json
--rw-r--r--   0        0        0   406238 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/yarn.lock
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/__mocks__/tone.ts
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/_version.py
--rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/build_log.json
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/package.json
--rw-r--r--   0        0        0    35060 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/lib_index_js.323a51fbb0d6f5584b4f.js
--rw-r--r--   0        0        0    34993 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/lib_index_js.323a51fbb0d6f5584b4f.js.map
--rw-r--r--   0        0        0    29080 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/remoteEntry.eff0e60b31d4b1e7493c.js
--rw-r--r--   0        0        0    27849 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/remoteEntry.eff0e60b31d4b1e7493c.js.map
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/style.js
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js.map
--rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js
--rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js.map
--rw-r--r--   0        0        0  2292198 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js
--rw-r--r--   0        0        0  2581426 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js.map
--rw-r--r--   0        0        0     5643 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/nb_examples/Untitled.ipynb
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/nb_examples/ipylab.ipynb
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/commands.ts
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/iconimports.ts
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/index.ts
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/model.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/svg.d.ts
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/tokens.ts
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/__tests__/commands.spec.ts
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/__tests__/model.spec.ts
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/index.ts
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/meter.tsx
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/transport.tsx
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/__tests__/meter.spec.tsx
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/__tests__/transport.spec.tsx
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/components/__tests__/__snapshots__/meter.spec.tsx.snap
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/util/animation.tsx
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/util/draw.tsx
--rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/util/__tests__/animation.spec.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/util/__tests__/draw.spec.tsx
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/widgets/index.ts
--rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/src/widgets/topbar.tsx
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/index.js
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/icons/mute.svg
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/icons/pause.svg
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/icons/play.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/icons/speaker.svg
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/style/icons/stop.svg
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/testutils/jest-setup-files.js
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   125826 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/yarn.lock
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/ui-tests/tests/topbar-transport.spec.ts
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/.gitignore
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/LICENSE
--rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/README.md
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyterlab_daw-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.dir-locals.el
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.eslintignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.eslintrc.js
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.prettierrc
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.stylelintrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/babel.config.js
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/install.json
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jest.config.js
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/setup.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   406238 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/yarn.lock
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/__mocks__/tone.ts
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/_version.py
+-rw-r--r--   0        0        0    21480 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/build_log.json
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/package.json
+-rw-r--r--   0        0        0    35664 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/lib_index_js.95af1f24f73d35dc11c8.js
+-rw-r--r--   0        0        0    36132 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/lib_index_js.95af1f24f73d35dc11c8.js.map
+-rw-r--r--   0        0        0    29080 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/remoteEntry.70aeeb9727eed1e13870.js
+-rw-r--r--   0        0        0    27849 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/remoteEntry.70aeeb9727eed1e13870.js.map
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/style.js
+-rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js.map
+-rw-r--r--   0        0        0    12058 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js
+-rw-r--r--   0        0        0    13790 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js.map
+-rw-r--r--   0        0        0  2292198 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js
+-rw-r--r--   0        0        0  2581426 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js.map
+-rw-r--r--   0        0        0     6167 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/nb_examples/Untitled.ipynb
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/nb_examples/ipylab.ipynb
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/commands.ts
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/iconimports.ts
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/index.ts
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/model.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/svg.d.ts
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/tokens.ts
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/__tests__/commands.spec.ts
+-rw-r--r--   0        0        0     3603 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/__tests__/model.spec.ts
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/index.ts
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/meter.tsx
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/transport.tsx
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/__tests__/meter.spec.tsx
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/__tests__/transport.spec.tsx
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/components/__tests__/__snapshots__/meter.spec.tsx.snap
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/util/animation.tsx
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/util/draw.tsx
+-rw-r--r--   0        0        0     1794 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/util/__tests__/animation.spec.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/util/__tests__/draw.spec.tsx
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/widgets/index.ts
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/src/widgets/topbar.tsx
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/index.js
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/icons/mute.svg
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/icons/pause.svg
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/icons/play.svg
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/icons/speaker.svg
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/style/icons/stop.svg
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/testutils/jest-setup-files.js
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   125826 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/ui-tests/tests/topbar-transport.spec.ts
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3520 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/README.md
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 jupyterlab_daw-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_daw-0.1.0/.dir-locals.el` & `jupyterlab_daw-0.2.0/.dir-locals.el`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/.eslintrc.js` & `jupyterlab_daw-0.2.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/RELEASE.md` & `jupyterlab_daw-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jest.config.js` & `jupyterlab_daw-0.2.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/package.json` & `jupyterlab_daw-0.2.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'author'": "{'name': 'Benoit Bovy'}", "'version'": "'0.2.0'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "author": {
         "email": "benbovy@gmail.com",
-        "name": "Beno\u00eet Bovy"
+        "name": "Benoit Bovy"
     },
     "bugs": {
         "url": "https://github.com/benbovy/jupyterlab-daw/issues"
     },
     "dependencies": {
         "@jupyterlab/application": "^3.6.0",
         "@jupyterlab/apputils": "^3.6.0",
@@ -101,9 +101,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_daw-0.1.0/tsconfig.json` & `jupyterlab_daw-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/yarn.lock` & `jupyterlab_daw-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/__mocks__/tone.ts` & `jupyterlab_daw-0.2.0/__mocks__/tone.ts`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,17 @@
     .mockImplementation(
       (clb: { (time: number): void; interval: any }): number => {
         clb(0);
         return 0;
       }
     );
   clear = jest.fn();
+  // Emitter implementation
+  on = jest.fn();
+  off = jest.fn();
 }
 
 export const Transport = new TransportClass();
 
 export function getTransport() {
   return Transport;
 }
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/build_log.json` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/package.json` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993055555555556%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.70aeeb9727eed1e13870.js'}}"}*

```diff
@@ -50,15 +50,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/benbovy/jupyterlab-daw",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.eff0e60b31d4b1e7493c.js",
+            "load": "static/remoteEntry.70aeeb9727eed1e13870.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlab_daw/labextension"
     },
     "keywords": [
         "jupyter",
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/lib_index_js.323a51fbb0d6f5584b4f.js` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/lib_index_js.95af1f24f73d35dc11c8.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -536,14 +536,21 @@
 
 
                 class DawExtension {
                     constructor() {
                         this._isDisposed = false;
                         this._destinationChanged = new _lumino_signaling__WEBPACK_IMPORTED_MODULE_0__.Signal(this);
                         this._transportChanged = new _lumino_signaling__WEBPACK_IMPORTED_MODULE_0__.Signal(this);
+                        const transport = (0, tone__WEBPACK_IMPORTED_MODULE_1__.getTransport)();
+                        this._transportClb = () => {
+                            this._transportChanged.emit();
+                        };
+                        transport.on('start', this._transportClb);
+                        transport.on('pause', this._transportClb);
+                        transport.on('stop', this._transportClb);
                     }
                     /**
                      * Signal emitted when the state of the destination node (speakers)
                      * is changed.
                      */
                     get destinationChanged() {
                         return this._destinationChanged;
@@ -610,21 +617,26 @@
                     /**
                      * Boolean indicating whether the model has been disposed.
                      */
                     get isDisposed() {
                         return this._isDisposed;
                     }
                     /**
-                     * Dispose model ressources.
+                     * Dispose model ressources and unbind tone signal callbacks.
                      */
                     dispose() {
                         if (this.isDisposed) {
                             return;
                         }
                         _lumino_signaling__WEBPACK_IMPORTED_MODULE_0__.Signal.clearData(this);
+                        const transport = (0, tone__WEBPACK_IMPORTED_MODULE_1__.getTransport)();
+                        transport.off('start', this._transportClb);
+                        transport.off('pause', this._transportClb);
+                        transport.off('stop', this._transportClb);
+                        this._isDisposed = true;
                     }
                 }
 
 
                 /***/
             }),
 
@@ -893,8 +905,8 @@
 
 
                 /***/
             })
 
     }
 ]);
-//# sourceMappingURL=lib_index_js.323a51fbb0d6f5584b4f.js.map
+//# sourceMappingURL=lib_index_js.95af1f24f73d35dc11c8.js.map
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/lib_index_js.323a51fbb0d6f5584b4f.js.map` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/lib_index_js.95af1f24f73d35dc11c8.js.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8482142857142857%*

 * *Differences: {"'file'": "'lib_index_js.95af1f24f73d35dc11c8.js'",*

 * * "'mappings'": "';;;;;;;;;;;;;AAAA,iEAAe,kfAAkf;;;;;;;;;;;;;;ACAjgB,iEAAe,iXAAiX,6IAA6I,6CAA6C;;;;;;;;;;;;;;ACA1jB,iEAAe,4WAA4W,6CAA6C;;;;;;;;;;;;;;ACAxa,iEAAe,kXAAkX,sBAAsB,4MAA4M,eAAe,2CAA2C;;;;;;;;;;;;;;ACA7pB,iEAAe,wXAAwX,6CAA6C;;;;;;;;;;;;;;;ACI9Y;AAE/B,SAAS,WAAW,CACzB,GAAoB,EACpB,OAA+B,EAC/B,QAAsB;IAEtB,4CAA4C;IAC5C,GAAG,CAAC,QAAQ,CAAC,UAAU,CAAC,wEAAmC,EAAE;QAC3D,KAAK,EAAE,2BAA2B;QAClC,OAAO,EAAE,GAAG,EAAE,CAAC,QAAQ,CAAC,qBAAqB,EAAE;KAChD,CAAC,CAAC;I […]*

```diff
@@ -1,10 +1,10 @@
 {
-    "file": "lib_index_js.323a51fbb0d6f5584b4f.js",
-    "mappings": "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",
+    "file": "lib_index_js.95af1f24f73d35dc11c8.js",
+    "mappings": "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",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-daw/./style/icons/mute.svg",
         "webpack://jupyterlab-daw/./style/icons/pause.svg",
         "webpack://jupyterlab-daw/./style/icons/play.svg",
         "webpack://jupyterlab-daw/./style/icons/speaker.svg",
@@ -27,15 +27,15 @@
         "export default \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\" standalone=\\\"no\\\"?>\\n<svg xmlns=\\\"http://www.w3.org/2000/svg\\\" version=\\\"1.0\\\" width=\\\"500\\\" height=\\\"500\\\" viewBox=\\\"0 0 75 75\\\">\\n  <g class=\\\"jp-icon3\\\" fill=\\\"#616161\\\" stroke=\\\"#616161\\\">\\n    <path d=\\\"M39.389,13.769 L22.235,28.606 L6,28.606 L6,47.699 L21.989,47.699 L39.389,62.75 L39.389,13.769z\\\" style=\\\"stroke-width:5;stroke-linejoin:round;\\\"/>\\n  </g>\\n  <g class=\\\"jp-icon3\\\" stroke=\\\"#616161\\\">\\n    <path class=\\\"jp-icon3\\\" d=\\\"M48,27.6a19.5,19.5 0 0 1 0,21.4M55.1,20.5a30,30 0 0 1 0,35.6M61.6,14a38.8,38.8 0 0 1 0,48.6\\\" style=\\\"fill:none;stroke-width:5;stroke-linecap:round\\\"/>\\n  </g>\\n</svg>\\n\";",
         "export default \"<?xml version=\\\"1.0\\\" encoding=\\\"UTF-8\\\" standalone=\\\"no\\\"?>\\n<svg\\n   version=\\\"1.0\\\"\\n   width=\\\"500\\\"\\n   height=\\\"500\\\"\\n   viewBox=\\\"0 0 75 75\\\"\\n   xmlns=\\\"http://www.w3.org/2000/svg\\\">\\n  <g class=\\\"jp-icon3\\\" fill=\\\"#616161\\\" stroke=\\\"#616161\\\">\\n    <path\\n       d=\\\"m 59.999999,15.000037 -45,-5e-5 0.317797,45.000025 h 44.682203 z\\\"\\n       style=\\\"stroke-width:5;stroke-linejoin:round\\\" />\\n  </g>\\n</svg>\\n\";",
         "import { JupyterFrontEnd } from '@jupyterlab/application';\nimport { ICommandPalette } from '@jupyterlab/apputils';\n\nimport { DawExtension } from './model';\nimport { CommandIDs } from './tokens';\n\nexport function addCommands(\n  app: JupyterFrontEnd,\n  palette: ICommandPalette | null,\n  dawModel: DawExtension\n): void {\n  /** Mute / Unmute main output (speakers). */\n  app.commands.addCommand(CommandIDs.dawToggleDestinationMute, {\n    label: 'Mute / Unmute Main Output',\n    execute: () => dawModel.toggleMuteDestination()\n  });\n\n  /** Start transport. */\n  app.commands.addCommand(CommandIDs.dawTransportStart, {\n    label: 'Start Transport',\n    execute: () => dawModel.transportStart()\n  });\n\n  /** Pause transport. */\n  app.commands.addCommand(CommandIDs.dawTransportPause, {\n    label: 'Pause Transport',\n    execute: () => dawModel.transportPause()\n  });\n\n  /** Stop transport. */\n  app.commands.addCommand(CommandIDs.dawTransportStop, {\n    label: 'Stop Transport',\n    execute: () => dawModel.transportStop()\n  });\n\n  if (palette !== null) {\n    palette.addItem({\n      command: CommandIDs.dawToggleDestinationMute,\n      category: 'DAW'\n    });\n\n    palette.addItem({\n      command: CommandIDs.dawTransportStart,\n      category: 'DAW'\n    });\n\n    palette.addItem({\n      command: CommandIDs.dawTransportPause,\n      category: 'DAW'\n    });\n\n    palette.addItem({\n      command: CommandIDs.dawTransportStop,\n      category: 'DAW'\n    });\n  }\n}\n",
         "import React, { useCallback, useEffect, useRef } from 'react';\n\nimport { Meter as ToneMeter, ToneAudioNode } from 'tone';\n\nimport { useAnimationFrame } from '../util/animation';\n\nexport type MeterOrientation = 'horizontal' | 'vertical';\n\nexport type MeterProps = {\n  inputNode: ToneAudioNode;\n  width: number;\n  height: number;\n  color1?: string;\n  color2?: string;\n  orientation?: MeterOrientation;\n  fps?: number;\n  thresholdValue?: number;\n  enabled?: boolean;\n};\n\n/**\n * Audio meter visualizer.\n */\nexport const Meter: React.FC<MeterProps> = ({\n  inputNode,\n  width,\n  height,\n  color1 = 'lime',\n  color2 = 'red',\n  orientation = 'vertical',\n  fps = 30,\n  thresholdValue = 0.01,\n  enabled = true\n}): JSX.Element => {\n  const meterRef = useRef<ToneMeter>(\n    new ToneMeter({ normalRange: true, channels: 2 })\n  );\n  const canvasRef = useRef<HTMLCanvasElement>(null);\n  const gradientRef = useRef<CanvasGradient | string>('lime');\n  const extentRef = useRef<number>(width);\n\n  useEffect(() => {\n    if (canvasRef.current) {\n      const ctx = canvasRef.current.getContext('2d');\n      if (ctx) {\n        let grd: CanvasGradient;\n        if (orientation === 'horizontal') {\n          grd = ctx.createLinearGradient(0, 0, width, 0);\n        } else {\n          grd = ctx.createLinearGradient(0, height, 0, 0);\n        }\n\n        grd.addColorStop(0, color1);\n        grd.addColorStop(0.5, color1);\n        grd.addColorStop(1, color2);\n\n        gradientRef.current = grd;\n      }\n    }\n\n    if (orientation === 'horizontal') {\n      extentRef.current = width;\n    } else {\n      extentRef.current = height;\n    }\n  }, [width, height, color1, color2, orientation]);\n\n  useEffect(() => {\n    const meter = meterRef.current;\n\n    // TODO: use smoothing with next Tone.js release version\n    // https://github.com/Tonejs/Tone.js/issues/882\n    meter.smoothing = 0;\n    // display 2 channels even when a mono signal goes through destination\n    meter.channelCountMode = 'explicit';\n\n    return () => {\n      meter.dispose();\n    };\n  }, []);\n\n  useEffect(() => {\n    const meter = meterRef.current;\n    if (enabled) {\n      inputNode.connect(meter);\n    }\n\n    return () => {\n      if (enabled) {\n        inputNode.disconnect(meter);\n      }\n    };\n  }, [inputNode, enabled, fps]);\n\n  const render = useCallback(\n    (ctx: CanvasRenderingContext2D) => {\n      ctx.clearRect(0, 0, width, height);\n\n      const valueLR = meterRef.current.getValue() as number[];\n\n      const thresh = thresholdValue;\n      if (valueLR[0] < thresh && valueLR[1] < thresh) {\n        return;\n      }\n\n      const extent = extentRef.current;\n      const levelL = Math.round(Math.pow(valueLR[0], 0.2) * extent);\n      const levelR = Math.round(Math.pow(valueLR[1], 0.2) * extent);\n\n      ctx.fillStyle = gradientRef.current;\n\n      if (orientation === 'horizontal') {\n        ctx.fillRect(0, 0, levelL, height / 2);\n        ctx.fillRect(0, height / 2, levelR, height);\n      } else {\n        ctx.fillRect(0, height, width / 2, -levelL);\n        ctx.fillRect(width / 2, height, width, -levelR);\n      }\n    },\n    [width, height, orientation, thresholdValue]\n  );\n\n  useAnimationFrame(\n    () => {\n      if (canvasRef.current) {\n        const context = canvasRef.current.getContext('2d');\n        if (context) {\n          render(context);\n        }\n      }\n    },\n    fps,\n    enabled\n  );\n\n  return (\n    <div>\n      <canvas ref={canvasRef} height={height} width={width} />\n    </div>\n  );\n};\n",
         "import React, { useCallback, useEffect, useState } from 'react';\n\nimport { getTransport } from 'tone';\n\nimport { useTransportDraw } from '../util/draw';\n\nexport type TransportPositionProps = {\n  state?: 'started' | 'stopped' | 'paused';\n  dirtyClassName?: string;\n};\n\nfunction getTransportPosition(): string {\n  const pos = getTransport().position.toString();\n  return pos.substr(0, pos.lastIndexOf(':')) + ':0';\n}\n\nexport const TransportPosition: React.FC<TransportPositionProps> = ({\n  state = 'stopped',\n  dirtyClassName = ''\n}): JSX.Element => {\n  const [position, setPosition] = useState<string>(getTransportPosition());\n  const [dirty, setDirty] = useState<boolean>(false);\n\n  // make sure to reset the input value when transport is stopped\n  // reset dirty when transport is started or stopped\n  useEffect(() => {\n    if (state === 'stopped') {\n      setPosition(getTransportPosition());\n      setDirty(false);\n    } else if (state === 'started') {\n      setDirty(false);\n    }\n  }, [state]);\n\n  const setPositionClb = useCallback(() => {\n    setPosition(getTransportPosition());\n  }, []);\n\n  useTransportDraw(setPositionClb, '4n');\n\n  const handleChange = (event: React.ChangeEvent<HTMLInputElement>) => {\n    const value = event.target.value;\n    setPosition(value);\n    setDirty(true);\n  };\n\n  const handleKeyDown = (event: React.KeyboardEvent<HTMLInputElement>) => {\n    if (event.key === 'Enter') {\n      getTransport().position = position;\n      // update input value with reformatted position\n      setPosition(getTransportPosition());\n      setDirty(false);\n    }\n  };\n\n  return (\n    <input\n      type=\"text\"\n      className={dirty ? dirtyClassName : ''}\n      disabled={state === 'started'}\n      value={position}\n      onChange={handleChange}\n      onKeyDown={handleKeyDown}\n    />\n  );\n};\n",
         "import { LabIcon } from '@jupyterlab/ui-components';\n\nimport speakerSvgstr from '../style/icons/speaker.svg';\nimport muteSvgstr from '../style/icons/mute.svg';\nimport playSvgstr from '../style/icons/play.svg';\nimport pauseSvgstr from '../style/icons/pause.svg';\nimport stopSvgstr from '../style/icons/stop.svg';\n\nexport const speakerIcon = new LabIcon({\n  name: 'daw:speaker',\n  svgstr: speakerSvgstr\n});\n\nexport const muteIcon = new LabIcon({\n  name: 'daw:mute',\n  svgstr: muteSvgstr\n});\n\nexport const playIcon = new LabIcon({\n  name: 'daw:play',\n  svgstr: playSvgstr\n});\n\nexport const pauseIcon = new LabIcon({\n  name: 'daw:pause',\n  svgstr: pauseSvgstr\n});\n\nexport const stopIcon = new LabIcon({\n  name: 'daw:stop',\n  svgstr: stopSvgstr\n});\n",
         "import {\n  JupyterFrontEnd,\n  JupyterFrontEndPlugin\n} from '@jupyterlab/application';\nimport { ICommandPalette } from '@jupyterlab/apputils';\n\nimport { TopBar } from './widgets';\n\nimport { addCommands } from './commands';\nimport { DawExtension } from './model';\nimport { IDawExtension } from './tokens';\n\nexport { IDawExtension } from './tokens';\n\n/**\n * Initialization data for the jupyterlab-daw extension.\n */\nconst plugin: JupyterFrontEndPlugin<IDawExtension> = {\n  id: 'jupyterlab-daw:plugin',\n  autoStart: true,\n  optional: [ICommandPalette],\n  provides: IDawExtension,\n  activate: (\n    app: JupyterFrontEnd,\n    palette: ICommandPalette | null\n  ): IDawExtension => {\n    const dawExtension = new DawExtension();\n\n    addCommands(app, palette, dawExtension);\n\n    const topBar = new TopBar(dawExtension, app.commands);\n    topBar.id = 'jp-daw-topbar';\n    app.shell.add(topBar, 'top', { rank: 1000 });\n\n    return dawExtension;\n  }\n};\n\nexport default plugin;\n",
-        "import { ISignal, Signal } from '@lumino/signaling';\n\nimport { getDestination, getTransport, start } from 'tone';\n\nimport { IDawExtension } from './tokens';\n\nexport class DawExtension implements IDawExtension {\n  /**\n   * Signal emitted when the state of the destination node (speakers)\n   * is changed.\n   */\n  get destinationChanged(): ISignal<IDawExtension, void> {\n    return this._destinationChanged;\n  }\n\n  /**\n   * Proxy for the destination node (speakers) mute.\n   */\n  get destinationMute(): boolean {\n    return getDestination().mute;\n  }\n\n  /**\n   * Mute or unmute the destination node (speakers).\n   */\n  toggleMuteDestination(): void {\n    const dest = getDestination();\n    dest.mute = !dest.mute;\n    this._destinationChanged.emit();\n  }\n\n  /**\n   * A signal emitted whenever the state of Tonejs Transport\n   * changes.\n   */\n  get transportChanged(): ISignal<IDawExtension, void> {\n    return this._transportChanged;\n  }\n\n  /**\n   * Current Tonejs transport state\n   */\n  get transportState(): 'started' | 'stopped' | 'paused' {\n    return getTransport().state;\n  }\n\n  /**\n   * Start Tone transport\n   */\n  transportStart(): void {\n    const transport = getTransport();\n    if (transport.state !== 'started') {\n      // start transport inactive if context not started\n      start();\n\n      transport.start();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Pause Tone transport\n   */\n  transportPause(): void {\n    const transport = getTransport();\n    if (transport.state === 'started') {\n      transport.pause();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Stop Tone transport\n   */\n  transportStop(): void {\n    const transport = getTransport();\n    if (transport.state !== 'stopped') {\n      transport.stop();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Boolean indicating whether the model has been disposed.\n   */\n  get isDisposed(): boolean {\n    return this._isDisposed;\n  }\n\n  /**\n   * Dispose model ressources.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n    Signal.clearData(this);\n  }\n\n  private _isDisposed = false;\n  private _destinationChanged = new Signal<IDawExtension, void>(this);\n  private _transportChanged = new Signal<IDawExtension, void>(this);\n}\n",
+        "import { ISignal, Signal } from '@lumino/signaling';\n\nimport { getDestination, getTransport, start } from 'tone';\n\nimport { IDawExtension } from './tokens';\n\nexport class DawExtension implements IDawExtension {\n  constructor() {\n    const transport = getTransport();\n\n    this._transportClb = () => { this._transportChanged.emit(); };\n    transport.on('start', this._transportClb);\n    transport.on('pause', this._transportClb);\n    transport.on('stop', this._transportClb);\n  }\n\n  /**\n   * Signal emitted when the state of the destination node (speakers)\n   * is changed.\n   */\n  get destinationChanged(): ISignal<IDawExtension, void> {\n    return this._destinationChanged;\n  }\n\n  /**\n   * Proxy for the destination node (speakers) mute.\n   */\n  get destinationMute(): boolean {\n    return getDestination().mute;\n  }\n\n  /**\n   * Mute or unmute the destination node (speakers).\n   */\n  toggleMuteDestination(): void {\n    const dest = getDestination();\n    dest.mute = !dest.mute;\n    this._destinationChanged.emit();\n  }\n\n  /**\n   * A signal emitted whenever the state of Tonejs Transport\n   * changes.\n   */\n  get transportChanged(): ISignal<IDawExtension, void> {\n    return this._transportChanged;\n  }\n\n  /**\n   * Current Tonejs transport state\n   */\n  get transportState(): 'started' | 'stopped' | 'paused' {\n    return getTransport().state;\n  }\n\n  /**\n   * Start Tone transport\n   */\n  transportStart(): void {\n    const transport = getTransport();\n    if (transport.state !== 'started') {\n      // start transport inactive if context not started\n      start();\n\n      transport.start();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Pause Tone transport\n   */\n  transportPause(): void {\n    const transport = getTransport();\n    if (transport.state === 'started') {\n      transport.pause();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Stop Tone transport\n   */\n  transportStop(): void {\n    const transport = getTransport();\n    if (transport.state !== 'stopped') {\n      transport.stop();\n      this._transportChanged.emit();\n    }\n  }\n\n  /**\n   * Boolean indicating whether the model has been disposed.\n   */\n  get isDisposed(): boolean {\n    return this._isDisposed;\n  }\n\n  /**\n   * Dispose model ressources and unbind tone signal callbacks.\n   */\n  dispose(): void {\n    if (this.isDisposed) {\n      return;\n    }\n\n    Signal.clearData(this);\n\n    const transport = getTransport();\n    transport.off('start', this._transportClb);\n    transport.off('pause', this._transportClb);\n    transport.off('stop', this._transportClb);\n\n    this._isDisposed = true;\n  }\n\n  private _transportClb: {(): void};\n  private _isDisposed = false;\n  private _destinationChanged = new Signal<IDawExtension, void>(this);\n  private _transportChanged = new Signal<IDawExtension, void>(this);\n}\n",
         "import { Token } from '@lumino/coreutils';\nimport { IDisposable } from '@lumino/disposable';\nimport { ISignal } from '@lumino/signaling';\n\nexport const EXTENSION_ID = 'jupyter.extensions.daw_plugin';\n\nexport const IDawExtension = new Token<IDawExtension>(EXTENSION_ID);\n\nexport interface IDawExtension extends IDisposable {\n  /**\n   * A signal emitted whenever the state of the audio destination\n   * (speaker) node changes (e.g., mute, volume).\n   */\n  readonly destinationChanged: ISignal<IDawExtension, void>;\n\n  /**\n   * Proxy for the destination node (speakers) mute.\n   */\n  readonly destinationMute: boolean;\n\n  /**\n   * Mute / Unmute the audio destination.\n   *\n   * This is a wrapper around Tone.getDestination.mute that allows\n   * emitting a signal.\n   */\n  toggleMuteDestination(): void;\n\n  /**\n   * A signal emitted whenever the state of Tonejs Transport\n   * changes.\n   */\n  readonly transportChanged: ISignal<IDawExtension, void>;\n\n  /**\n   * Current Tonejs transport state\n   */\n  readonly transportState: 'started' | 'stopped' | 'paused';\n\n  /**\n   * Start Tone transport\n   */\n  transportStart(): void;\n\n  /**\n   * Pause Tone transport\n   */\n  transportPause(): void;\n\n  /**\n   * Stop Tone transport\n   */\n  transportStop(): void;\n}\n\n/**\n * The command IDs used by the daw plugin.\n */\nexport enum CommandIDs {\n  dawToggleDestinationMute = 'daw:toggle-main-mute',\n  dawTransportStart = 'daw:transport-start',\n  dawTransportPause = 'daw:transport-pause',\n  dawTransportStop = 'daw:transport-stop'\n}\n",
         "import { useCallback, useEffect, useRef } from 'react';\n\n/**\n * Reusable React Hook for setting animation frames.\n *\n * @param callback - function called at each frame (fps) render\n * @param fps {number} - allow executing the callback less often than the screen refresh rate\n * @param running {boolean=} - changing the state will either start or stop the animation\n *\n */\nexport const useAnimationFrame = (\n  callback: { (): void },\n  fps: number,\n  running = true\n): void => {\n  const frameRef = useRef<number>(0);\n  const prevRef = useRef<number>(-1);\n\n  const animate = useCallback(() => {\n    const now = performance.now();\n    const delta = now - prevRef.current;\n    if (prevRef.current === -1 || delta >= 1000 / fps) {\n      callback();\n      prevRef.current = now;\n    }\n    frameRef.current = requestAnimationFrame(animate);\n  }, [callback, fps]);\n\n  useEffect(() => {\n    if (running) {\n      frameRef.current = requestAnimationFrame(animate);\n    }\n\n    return () => {\n      // delay stopping the animation (draw next 10 actual frames) so that\n      // it has a chance to clear or reset properly.\n      if (running) {\n        setTimeout(() => {\n          cancelAnimationFrame(frameRef.current);\n        }, 10000 / fps);\n      }\n    };\n  }, [running, fps, animate]);\n};\n",
         "import { useEffect, useRef } from 'react';\n\nimport { getDraw, getTransport, TimeClass } from 'tone';\n\n/**\n * React hook for Tone transport synced animations.\n */\nexport const useTransportDraw = (\n  callback: { (): void },\n  interval: string | number | TimeClass\n): void => {\n  const eventIDRef = useRef<number>(-1);\n\n  useEffect(() => {\n    const transport = getTransport();\n\n    const drawCallback = (time: any) => {\n      getDraw().schedule(callback, time);\n    };\n\n    eventIDRef.current = transport.scheduleRepeat(drawCallback, interval);\n\n    return () => {\n      transport.clear(eventIDRef.current);\n    };\n  }, [interval, callback]);\n};\n",
         "import {\n  ReactWidget,\n  Toolbar,\n  ToolbarButtonComponent,\n  UseSignal\n} from '@jupyterlab/apputils';\n\nimport { CommandRegistry } from '@lumino/commands';\nimport { Widget } from '@lumino/widgets';\n\nimport React from 'react';\n\nimport { getDestination } from 'tone';\n\nimport { Meter } from '../components/meter';\nimport { TransportPosition } from '../components/transport';\nimport {\n  speakerIcon,\n  muteIcon,\n  playIcon,\n  stopIcon,\n  pauseIcon\n} from '../iconimports';\nimport { CommandIDs, IDawExtension } from '../tokens';\n\nconst TOPBAR_CLASS = 'jp-daw-TopBar';\nconst CONTENT_CLASS = 'jp-daw-TopBar-item';\n\nexport class TopBar extends Toolbar<Widget> {\n  constructor(model: IDawExtension, commands: CommandRegistry) {\n    super();\n    this._model = model;\n    this.addClass(TOPBAR_CLASS);\n\n    const playButton = ReactWidget.create(\n      <UseSignal signal={model.transportChanged}>\n        {() => (\n          <ToolbarButtonComponent\n            icon={playIcon}\n            pressedIcon={pauseIcon}\n            pressed={model.transportState === 'started'}\n            tooltip={'start transport'}\n            pressedTooltip={'pause transport'}\n            onClick={() => {\n              if (model.transportState === 'started') {\n                commands.execute(CommandIDs.dawTransportPause);\n              } else {\n                commands.execute(CommandIDs.dawTransportStart);\n              }\n            }}\n          />\n        )}\n      </UseSignal>\n    );\n\n    this.addItem('jp-daw-topbar-play', playButton);\n\n    const stopButton = ReactWidget.create(\n      <UseSignal signal={model.transportChanged}>\n        {() => (\n          <ToolbarButtonComponent\n            icon={stopIcon}\n            tooltip={'stop transport'}\n            onClick={() => {\n              commands.execute(CommandIDs.dawTransportStop);\n            }}\n          />\n        )}\n      </UseSignal>\n    );\n\n    this.addItem('jp-daw-topbar-stop', stopButton);\n\n    const transportPosition = ReactWidget.create(\n      <UseSignal signal={model.transportChanged}>\n        {() => (\n          <TransportPosition\n            state={model.transportState}\n            dirtyClassName={'jp-daw-mod-dirty'}\n          />\n        )}\n      </UseSignal>\n    );\n\n    transportPosition.addClass('jp-daw-TransportPosition');\n    this.addItem('jp-daw-topbar-transport-position', transportPosition);\n\n    const meter = ReactWidget.create(\n      <UseSignal signal={model.destinationChanged}>\n        {() => (\n          <Meter\n            inputNode={getDestination()}\n            width={16}\n            height={21}\n            fps={20}\n            orientation={'vertical'}\n            enabled={!this._model.destinationMute}\n          />\n        )}\n      </UseSignal>\n    );\n\n    meter.addClass('jp-daw-Meter');\n    this.addItem('jp-daw-topbar-meter', meter);\n\n    const toggleMuteButton = ReactWidget.create(\n      <UseSignal signal={model.destinationChanged}>\n        {() => (\n          <ToolbarButtonComponent\n            icon={speakerIcon}\n            pressedIcon={muteIcon}\n            pressed={this._model.destinationMute}\n            tooltip={'mute'}\n            pressedTooltip={'unmute'}\n            onClick={() => {\n              commands.execute(CommandIDs.dawToggleDestinationMute);\n            }}\n          />\n        )}\n      </UseSignal>\n    );\n\n    this.addItem('jp-daw-topbar-toggle-mute', toggleMuteButton);\n  }\n\n  addItem(name: string, item: Widget): boolean {\n    item.addClass(CONTENT_CLASS);\n    return super.addItem(name, item);\n  }\n\n  private _model: IDawExtension;\n}\n"
     ],
     "version": 3
 }
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/remoteEntry.eff0e60b31d4b1e7493c.js` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/remoteEntry.70aeeb9727eed1e13870.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -182,15 +182,15 @@
     (() => {
         /******/ // This function allow to reference async chunks
         /******/
         __webpack_require__.u = (chunkId) => {
             /******/ // return url for filenames based on template
             /******/
             return "" + chunkId + "." + {
-                "lib_index_js": "323a51fbb0d6f5584b4f",
+                "lib_index_js": "95af1f24f73d35dc11c8",
                 "vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1": "26ed18b76ed10f5150a0",
                 "style_index_js": "5438e31f380a864abd20",
                 "vendors-node_modules_tone_build_esm_index_js": "4dcb5d8ed93419dbeb85"
             } [chunkId] + ".js";
             /******/
         };
         /******/
@@ -1079,8 +1079,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/jupyterlab-daw");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["jupyterlab-daw"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.eff0e60b31d4b1e7493c.js.map
+//# sourceMappingURL=remoteEntry.70aeeb9727eed1e13870.js.map
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/remoteEntry.eff0e60b31d4b1e7493c.js.map` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/remoteEntry.70aeeb9727eed1e13870.js.map`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.70aeeb9727eed1e13870.js'",*

 * * "'sourcesContent'": "{insert: [(5, '// This function allow to reference async "*

 * *                     'chunks\\n__webpack_require__.u = (chunkId) => {\\n\\t// return url for '*

 * *                     'filenames based on template\\n\\treturn "" + chunkId + "." + '*

 * *                     '{"lib_index_js":"95af1f24f73d35dc11c8","vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1":"26ed18b76ed10f5150a0","style_index […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.eff0e60b31d4b1e7493c.js",
+    "file": "remoteEntry.70aeeb9727eed1e13870.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,kRAAkR;WAChT;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCxCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC5CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WCfA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB,GAAG;WACH;WACA;;;;;WCjLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://jupyterlab-daw/webpack/container-entry",
         "webpack://jupyterlab-daw/webpack/bootstrap",
         "webpack://jupyterlab-daw/webpack/runtime/compat get default export",
@@ -25,15 +25,15 @@
     ],
     "sourcesContent": [
         "var moduleMap = {\n\t\"./index\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./extension\": () => {\n\t\treturn __webpack_require__.e(\"lib_index_js\").then(() => (() => ((__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\")))));\n\t},\n\t\"./style\": () => {\n\t\treturn Promise.all([__webpack_require__.e(\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\"), __webpack_require__.e(\"style_index_js\")]).then(() => (() => ((__webpack_require__(/*! ./style/index.js */ \"./style/index.js\")))));\n\t}\n};\nvar get = (module, getScope) => {\n\t__webpack_require__.R = getScope;\n\tgetScope = (\n\t\t__webpack_require__.o(moduleMap, module)\n\t\t\t? moduleMap[module]()\n\t\t\t: Promise.resolve().then(() => {\n\t\t\t\tthrow new Error('Module \"' + module + '\" does not exist in container.');\n\t\t\t})\n\t);\n\t__webpack_require__.R = undefined;\n\treturn getScope;\n};\nvar init = (shareScope, initScope) => {\n\tif (!__webpack_require__.S) return;\n\tvar name = \"default\"\n\tvar oldScope = __webpack_require__.S[name];\n\tif(oldScope && oldScope !== shareScope) throw new Error(\"Container initialization failed as it has already been initialized with a different share scope\");\n\t__webpack_require__.S[name] = shareScope;\n\treturn __webpack_require__.I(name, initScope);\n};\n\n// This exports getters to disallow modifications\n__webpack_require__.d(exports, {\n\tget: () => (get),\n\tinit: () => (init)\n});",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n// expose the modules object (__webpack_modules__)\n__webpack_require__.m = __webpack_modules__;\n\n// expose the module cache\n__webpack_require__.c = __webpack_module_cache__;\n\n",
         "// getDefaultExport function for compatibility with non-harmony modules\n__webpack_require__.n = (module) => {\n\tvar getter = module && module.__esModule ?\n\t\t() => (module['default']) :\n\t\t() => (module);\n\t__webpack_require__.d(getter, { a: getter });\n\treturn getter;\n};",
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
-        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"323a51fbb0d6f5584b4f\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"26ed18b76ed10f5150a0\",\"style_index_js\":\"5438e31f380a864abd20\",\"vendors-node_modules_tone_build_esm_index_js\":\"4dcb5d8ed93419dbeb85\"}[chunkId] + \".js\";\n};",
+        "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"lib_index_js\":\"95af1f24f73d35dc11c8\",\"vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1\":\"26ed18b76ed10f5150a0\",\"style_index_js\":\"5438e31f380a864abd20\",\"vendors-node_modules_tone_build_esm_index_js\":\"4dcb5d8ed93419dbeb85\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"jupyterlab-daw:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
         "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => (typeof console !== \"undefined\" && console.warn && console.warn(msg));\n\tvar uniqueName = \"jupyterlab-daw\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"jupyterlab-daw\", \"0.1.0\", () => (__webpack_require__.e(\"lib_index_js\").then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t\tregister(\"tone\", \"14.7.77\", () => (__webpack_require__.e(\"vendors-node_modules_tone_build_esm_index_js\").then(() => (() => (__webpack_require__(/*! ./node_modules/tone/build/esm/index.js */ \"./node_modules/tone/build/esm/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) scriptUrl = scripts[scripts.length - 1].src\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) typeof console !== \"undefined\" && console.warn && console.warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\ttypeof console !== \"undefined\" && console.warn && console.warn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,3,6,2])),\n\t\"webpack/sharing/consume/default/@lumino/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/coreutils\", [1,1,11,0])),\n\t\"webpack/sharing/consume/default/@lumino/signaling\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/signaling\", [1,1,10,0])),\n\t\"webpack/sharing/consume/default/tone/tone\": () => (loadStrictVersionCheckFallback(\"default\", \"tone\", [2,14,7,77], () => (__webpack_require__.e(\"vendors-node_modules_tone_build_esm_index_js\").then(() => (() => (__webpack_require__(/*! tone */ \"./node_modules/tone/build/esm/index.js\"))))))),\n\t\"webpack/sharing/consume/default/react\": () => (loadSingletonVersionCheck(\"default\", \"react\", [1,17,0,1])),\n\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/ui-components\", [1,3,6,2]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@lumino/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/signaling\",\n\t\t\"webpack/sharing/consume/default/tone/tone\",\n\t\t\"webpack/sharing/consume/default/react\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/ui-components\"\n\t]\n};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t});\n\t}\n}",
```

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js.map` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/style_index_js.5438e31f380a864abd20.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js.map` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.26ed18b76ed10f5150a0.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js.map` & `jupyterlab_daw-0.2.0/jupyterlab_daw/labextension/static/vendors-node_modules_tone_build_esm_index_js.4dcb5d8ed93419dbeb85.js.map`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/nb_examples/Untitled.ipynb` & `jupyterlab_daw-0.2.0/nb_examples/Untitled.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.995361328125%*

 * *Differences: {"'cells'": "{6: {'execution_count': 15, 'outputs': {0: {'execution_count': 15}}}, 7: "*

 * *            "{'execution_count': 16, 'outputs': [OrderedDict([('data', OrderedDict([('text/plain', "*

 * *            '["\'8:2:2.312\'"])])), (\'execution_count\', 16), (\'metadata\', OrderedDict()), '*

 * *            "('output_type', 'execute_result')])]}, 8: {'execution_count': 17, 'outputs': "*

 * *            "[OrderedDict([('data', OrderedDict([('text/plain', ['Transport()'])])), "*

 * *            "('execution_count', 17), ('metadata […]*

```diff
@@ -103,56 +103,78 @@
                 "    events=[\"A0\", \"A1\", \"A0\", None, \"F#2\", \"G2\", \"G#2\", \"A2\"],\n",
                 "    subdivision=\"16n\",\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 15,
             "id": "c831be2c-86f7-49d3-bbe3-2139652b34fd",
             "metadata": {
                 "tags": []
             },
             "outputs": [
                 {
                     "data": {
                         "text/plain": [
                             "Sequence(loop=True, loop_start=0.0, loop_end=0.0)"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 15,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "ipytone.transport.start()\n",
                 "sequence.start()"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 16,
             "id": "cc5fb056-b3af-41fc-864f-bf68e8241421",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "'8:2:2.312'"
+                        ]
+                    },
+                    "execution_count": 16,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "ipytone.transport.position"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 17,
             "id": "02191b46-1f0d-4891-b20c-b6ad3c61e6aa",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Transport()"
+                        ]
+                    },
+                    "execution_count": 17,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "ipytone.transport.pause()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -190,20 +212,31 @@
             "source": [
                 "channel1.volume.value = -50\n",
                 "channel2.volume.value = -5"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 18,
             "id": "baa91441-3fb4-48ad-8364-8c1e275fb19a",
             "metadata": {
                 "tags": []
             },
-            "outputs": [],
+            "outputs": [
+                {
+                    "data": {
+                        "text/plain": [
+                            "Transport()"
+                        ]
+                    },
+                    "execution_count": 18,
+                    "metadata": {},
+                    "output_type": "execute_result"
+                }
+            ],
             "source": [
                 "ipytone.transport.stop()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
```

### Comparing `jupyterlab_daw-0.1.0/nb_examples/ipylab.ipynb` & `jupyterlab_daw-0.2.0/nb_examples/ipylab.ipynb`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/commands.ts` & `jupyterlab_daw-0.2.0/src/commands.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/iconimports.ts` & `jupyterlab_daw-0.2.0/src/iconimports.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/index.ts` & `jupyterlab_daw-0.2.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/model.ts` & `jupyterlab_daw-0.2.0/src/model.ts`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import { ISignal, Signal } from '@lumino/signaling';
 
 import { getDestination, getTransport, start } from 'tone';
 
 import { IDawExtension } from './tokens';
 
 export class DawExtension implements IDawExtension {
+  constructor() {
+    const transport = getTransport();
+
+    this._transportClb = () => {
+      this._transportChanged.emit();
+    };
+    transport.on('start', this._transportClb);
+    transport.on('pause', this._transportClb);
+    transport.on('stop', this._transportClb);
+  }
+
   /**
    * Signal emitted when the state of the destination node (speakers)
    * is changed.
    */
   get destinationChanged(): ISignal<IDawExtension, void> {
     return this._destinationChanged;
   }
@@ -84,20 +95,29 @@
    * Boolean indicating whether the model has been disposed.
    */
   get isDisposed(): boolean {
     return this._isDisposed;
   }
 
   /**
-   * Dispose model ressources.
+   * Dispose model ressources and unbind tone signal callbacks.
    */
   dispose(): void {
     if (this.isDisposed) {
       return;
     }
+
     Signal.clearData(this);
+
+    const transport = getTransport();
+    transport.off('start', this._transportClb);
+    transport.off('pause', this._transportClb);
+    transport.off('stop', this._transportClb);
+
+    this._isDisposed = true;
   }
 
+  private _transportClb: { (): void };
   private _isDisposed = false;
   private _destinationChanged = new Signal<IDawExtension, void>(this);
   private _transportChanged = new Signal<IDawExtension, void>(this);
 }
```

### Comparing `jupyterlab_daw-0.1.0/src/tokens.ts` & `jupyterlab_daw-0.2.0/src/tokens.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/__tests__/commands.spec.ts` & `jupyterlab_daw-0.2.0/src/__tests__/commands.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/__tests__/model.spec.ts` & `jupyterlab_daw-0.2.0/src/__tests__/model.spec.ts`

 * *Files 14% similar despite different names*

```diff
@@ -96,9 +96,22 @@
         // ensure mocked transport is set in the given initial state
         Object.assign(getTransport(), { state: initState });
 
         modelFunc();
         expect(toneFunc).not.toBeCalled();
       }
     );
+
+    it('should listen to Tonejs transport events', () => {
+      expect(getTransport().on).toBeCalledWith('start', expect.anything());
+      expect(getTransport().on).toBeCalledWith('pause', expect.anything());
+      expect(getTransport().on).toBeCalledWith('stop', expect.anything());
+    });
+
+    it('should stop listening to Tonejs transport events when disposed', () => {
+      model.dispose();
+      expect(getTransport().off).toBeCalledWith('start', expect.anything());
+      expect(getTransport().off).toBeCalledWith('pause', expect.anything());
+      expect(getTransport().off).toBeCalledWith('stop', expect.anything());
+    });
   });
 });
```

### Comparing `jupyterlab_daw-0.1.0/src/components/meter.tsx` & `jupyterlab_daw-0.2.0/src/components/meter.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/components/transport.tsx` & `jupyterlab_daw-0.2.0/src/components/transport.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/components/__tests__/meter.spec.tsx` & `jupyterlab_daw-0.2.0/src/components/__tests__/meter.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/components/__tests__/transport.spec.tsx` & `jupyterlab_daw-0.2.0/src/components/__tests__/transport.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/util/animation.tsx` & `jupyterlab_daw-0.2.0/src/util/animation.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/util/draw.tsx` & `jupyterlab_daw-0.2.0/src/util/draw.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/util/__tests__/animation.spec.tsx` & `jupyterlab_daw-0.2.0/src/util/__tests__/animation.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/util/__tests__/draw.spec.tsx` & `jupyterlab_daw-0.2.0/src/util/__tests__/draw.spec.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/src/widgets/topbar.tsx` & `jupyterlab_daw-0.2.0/src/widgets/topbar.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/style/base.css` & `jupyterlab_daw-0.2.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/style/icons/speaker.svg` & `jupyterlab_daw-0.2.0/style/icons/speaker.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/ui-tests/README.md` & `jupyterlab_daw-0.2.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/ui-tests/jupyter_server_test_config.py` & `jupyterlab_daw-0.2.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/ui-tests/yarn.lock` & `jupyterlab_daw-0.2.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/ui-tests/tests/topbar-transport.spec.ts` & `jupyterlab_daw-0.2.0/ui-tests/tests/topbar-transport.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/.gitignore` & `jupyterlab_daw-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/LICENSE` & `jupyterlab_daw-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/README.md` & `jupyterlab_daw-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/pyproject.toml` & `jupyterlab_daw-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_daw-0.1.0/PKG-INFO` & `jupyterlab_daw-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: jupyterlab_daw
-Version: 0.1.0
+Version: 0.2.0
 Summary: JupyterLab as a Digital Audio Workstation
 Project-URL: Homepage, https://github.com/benbovy/jupyterlab-daw
 Project-URL: Bug Tracker, https://github.com/benbovy/jupyterlab-daw/issues
 Project-URL: Repository, https://github.com/benbovy/jupyterlab-daw.git
-Author-email: Benoît Bovy <benbovy@gmail.com>
+Author-email: Benoit Bovy <benbovy@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Benoît Bovy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

