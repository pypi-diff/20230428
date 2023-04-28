# Comparing `tmp/avnet-scotty-2023.3.tar.gz` & `tmp/avnet-scotty-2023.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet-scotty-2023.3.tar", last modified: Wed Apr  5 12:59:56 2023, max compression
+gzip compressed data, was "avnet-scotty-2023.4.tar", last modified: Fri Apr 28 08:20:55 2023, max compression
```

## Comparing `avnet-scotty-2023.3.tar` & `avnet-scotty-2023.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 12:59:56.766027 avnet-scotty-2023.3/
--rw-r--r--   0 root         (0) root         (0)    32879 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    17413 2023-04-05 12:59:56.766027 avnet-scotty-2023.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    17115 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 12:59:56.762026 avnet-scotty-2023.3/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17413 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      356 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-05 12:59:56.000000 avnet-scotty-2023.3/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 12:59:56.762026 avnet-scotty-2023.3/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/bumper/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     6488 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/scotty
--rwxr-xr-x   0 root         (0) root         (0)     1580 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 12:59:56.766027 avnet-scotty-2023.3/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 12:59:56.766027 avnet-scotty-2023.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1002 2023-04-05 12:59:48.000000 avnet-scotty-2023.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/
+-rw-r--r--   0 root         (0) root         (0)    32879 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    18391 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    18093 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18391 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 08:20:55.000000 avnet-scotty-2023.4/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/bumper/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6703 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     1580 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 08:20:55.465273 avnet-scotty-2023.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-04-28 08:20:47.000000 avnet-scotty-2023.4/setup.py
```

### Comparing `avnet-scotty-2023.3/LICENSE` & `avnet-scotty-2023.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.3/PKG-INFO` & `avnet-scotty-2023.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.3
+Version: 2023.4
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -80,14 +80,34 @@
     default parameters if the build directory has not been setup.
   - ``bitbake``: Build a Yocto target.
   - ``shell``: Run a shell in the Yocto build environment.
   - ``command``: Run a command in the Yocto build environment.
   - ``docker-update``: Update Scotty build container.
   - ``info``: Print out information.
 
+Setup your build
+----------------
+
+With
+
+.. code-block:: bash
+
+   $ scotty setup
+
+you can configure your build through our interactive UI.
+
+.. note::
+
+  .. code-block:: bash
+
+    $ scotty setup --force
+
+  Will allow you to redo the configuration at any point
+
+
 Building a full image
 ---------------------
 
 A single command is enough to download the sources and build an image:
 
 .. code-block:: bash
 
@@ -98,14 +118,43 @@
 The build target can be customized:
 
 .. code-block:: bash
 
    $ scotty bitbake core-image-minimal
    $ scotty bitbake -- core-image-minimal -c populate_sdk
 
+.. note::
+
+  The available images/SDKs can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info images
+
+Recommended hardware setup
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+For building software pacakges with ``Scotty`` we recommend the following minimal hardware setup
+
+For base images
+
+- 4 Cores / 8 threads CPU
+- 16GB RAM
+- 200GB HDD
+
+For SDKs
+
+- 16 Cores / 32 threads CPU
+- 64Gb RAM
+- 500GB HDD
+
+.. note::
+
+  Other combinations do work as well, but keep in mind that we at least require 2GB of RAM per available CPU thread
+
 Using Scotty as a helper
 ------------------------
 
 ``Scotty`` can be used to open a shell with a sourced Yocto environment:
 
 .. code-block:: bash
 
@@ -152,23 +201,25 @@
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 - ``--extra-layer``: Add an extra local layer.
 - ``--extra-conf``: Add an extra configuration entry in local.conf.
 - ``--extra-env``: Pass on additional environment variables.
 - ``--sstate-mirrors``: Do use any sstate mirror (default = false).
 - ``--features-layers-set``: The set of Avnet Embedded extra layers to use.
-  Supported values are:
-  - ``bsp``: Only BSP related layers.
-  - ``distro``: BSP and distro related layers.
-  - ``examples``: All above layers and example layers.
-  - ``simpleswitch``: BSP, distro and simpleswitch related layers.
-  - ``simpleswitch_examples``: All above layers and example layers.
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 
+.. note::
+
+  The currently available ``--features-layers-set`` can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info feature-sets
+
 Supported bitbake, shell and command arguments
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - ``--build-dir``: Set build subdirectory, subdirectory of ``build``. Can be
   used to have different builds in the same ``build`` folder.
 
 Scripting configuration
@@ -376,7 +427,15 @@
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
+
+scotty-layers.ext.yaml
+======================
+
+``scotty`` will additionally scan for ``scotty-layers.ext.yaml`` in the checked out repositories.
+These files are written in the same syntax as ``scotty-layers.yaml`` and allow the standard ``scotty-layers.yaml`` to be extended.
+
+The files have to be placed in the root of the bitbake layer.
```

### Comparing `avnet-scotty-2023.3/README.rst` & `avnet-scotty-2023.4/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,34 @@
     default parameters if the build directory has not been setup.
   - ``bitbake``: Build a Yocto target.
   - ``shell``: Run a shell in the Yocto build environment.
   - ``command``: Run a command in the Yocto build environment.
   - ``docker-update``: Update Scotty build container.
   - ``info``: Print out information.
 
+Setup your build
+----------------
+
+With
+
+.. code-block:: bash
+
+   $ scotty setup
+
+you can configure your build through our interactive UI.
+
+.. note::
+
+  .. code-block:: bash
+
+    $ scotty setup --force
+
+  Will allow you to redo the configuration at any point
+
+
 Building a full image
 ---------------------
 
 A single command is enough to download the sources and build an image:
 
 .. code-block:: bash
 
@@ -88,14 +108,43 @@
 The build target can be customized:
 
 .. code-block:: bash
 
    $ scotty bitbake core-image-minimal
    $ scotty bitbake -- core-image-minimal -c populate_sdk
 
+.. note::
+
+  The available images/SDKs can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info images
+
+Recommended hardware setup
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+For building software pacakges with ``Scotty`` we recommend the following minimal hardware setup
+
+For base images
+
+- 4 Cores / 8 threads CPU
+- 16GB RAM
+- 200GB HDD
+
+For SDKs
+
+- 16 Cores / 32 threads CPU
+- 64Gb RAM
+- 500GB HDD
+
+.. note::
+
+  Other combinations do work as well, but keep in mind that we at least require 2GB of RAM per available CPU thread
+
 Using Scotty as a helper
 ------------------------
 
 ``Scotty`` can be used to open a shell with a sourced Yocto environment:
 
 .. code-block:: bash
 
@@ -142,23 +191,25 @@
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 - ``--extra-layer``: Add an extra local layer.
 - ``--extra-conf``: Add an extra configuration entry in local.conf.
 - ``--extra-env``: Pass on additional environment variables.
 - ``--sstate-mirrors``: Do use any sstate mirror (default = false).
 - ``--features-layers-set``: The set of Avnet Embedded extra layers to use.
-  Supported values are:
-  - ``bsp``: Only BSP related layers.
-  - ``distro``: BSP and distro related layers.
-  - ``examples``: All above layers and example layers.
-  - ``simpleswitch``: BSP, distro and simpleswitch related layers.
-  - ``simpleswitch_examples``: All above layers and example layers.
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 
+.. note::
+
+  The currently available ``--features-layers-set`` can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info feature-sets
+
 Supported bitbake, shell and command arguments
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - ``--build-dir``: Set build subdirectory, subdirectory of ``build``. Can be
   used to have different builds in the same ``build`` folder.
 
 Scripting configuration
@@ -366,7 +417,15 @@
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
+
+scotty-layers.ext.yaml
+======================
+
+``scotty`` will additionally scan for ``scotty-layers.ext.yaml`` in the checked out repositories.
+These files are written in the same syntax as ``scotty-layers.yaml`` and allow the standard ``scotty-layers.yaml`` to be extended.
+
+The files have to be placed in the root of the bitbake layer.
```

### Comparing `avnet-scotty-2023.3/avnet_scotty.egg-info/PKG-INFO` & `avnet-scotty-2023.4/avnet_scotty.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2023.3
+Version: 2023.4
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Home-page: https://github.com/avnet-embedded/simplecore-tools
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -80,14 +80,34 @@
     default parameters if the build directory has not been setup.
   - ``bitbake``: Build a Yocto target.
   - ``shell``: Run a shell in the Yocto build environment.
   - ``command``: Run a command in the Yocto build environment.
   - ``docker-update``: Update Scotty build container.
   - ``info``: Print out information.
 
+Setup your build
+----------------
+
+With
+
+.. code-block:: bash
+
+   $ scotty setup
+
+you can configure your build through our interactive UI.
+
+.. note::
+
+  .. code-block:: bash
+
+    $ scotty setup --force
+
+  Will allow you to redo the configuration at any point
+
+
 Building a full image
 ---------------------
 
 A single command is enough to download the sources and build an image:
 
 .. code-block:: bash
 
@@ -98,14 +118,43 @@
 The build target can be customized:
 
 .. code-block:: bash
 
    $ scotty bitbake core-image-minimal
    $ scotty bitbake -- core-image-minimal -c populate_sdk
 
+.. note::
+
+  The available images/SDKs can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info images
+
+Recommended hardware setup
+^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+For building software pacakges with ``Scotty`` we recommend the following minimal hardware setup
+
+For base images
+
+- 4 Cores / 8 threads CPU
+- 16GB RAM
+- 200GB HDD
+
+For SDKs
+
+- 16 Cores / 32 threads CPU
+- 64Gb RAM
+- 500GB HDD
+
+.. note::
+
+  Other combinations do work as well, but keep in mind that we at least require 2GB of RAM per available CPU thread
+
 Using Scotty as a helper
 ------------------------
 
 ``Scotty`` can be used to open a shell with a sourced Yocto environment:
 
 .. code-block:: bash
 
@@ -152,23 +201,25 @@
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 - ``--extra-layer``: Add an extra local layer.
 - ``--extra-conf``: Add an extra configuration entry in local.conf.
 - ``--extra-env``: Pass on additional environment variables.
 - ``--sstate-mirrors``: Do use any sstate mirror (default = false).
 - ``--features-layers-set``: The set of Avnet Embedded extra layers to use.
-  Supported values are:
-  - ``bsp``: Only BSP related layers.
-  - ``distro``: BSP and distro related layers.
-  - ``examples``: All above layers and example layers.
-  - ``simpleswitch``: BSP, distro and simpleswitch related layers.
-  - ``simpleswitch_examples``: All above layers and example layers.
 - ``--machine-dir``: specify the directories where scotty should look for
   supported machines.
 
+.. note::
+
+  The currently available ``--features-layers-set`` can be displayed by running
+
+  .. code-block:: bash
+
+    $ scotty info feature-sets
+
 Supported bitbake, shell and command arguments
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - ``--build-dir``: Set build subdirectory, subdirectory of ``build``. Can be
   used to have different builds in the same ``build`` folder.
 
 Scripting configuration
@@ -376,7 +427,15 @@
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | supported_distros | dict   | key/value table of DISTRO name and description | supported_distros: &distros_myfeature           |
 |                   |        |                                                |    <<: [\*distros_poky]                         |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
 | add-overlays      | object | Additional selectable overlays of the feature  | add-overlays:                                   |
 |                   |        |   see `overlays section` for details           |    overlays:                                    |
 +-------------------+--------+------------------------------------------------+-------------------------------------------------+
+
+scotty-layers.ext.yaml
+======================
+
+``scotty`` will additionally scan for ``scotty-layers.ext.yaml`` in the checked out repositories.
+These files are written in the same syntax as ``scotty-layers.yaml`` and allow the standard ``scotty-layers.yaml`` to be extended.
+
+The files have to be placed in the root of the bitbake layer.
```

### Comparing `avnet-scotty-2023.3/bumper/__main__.py` & `avnet-scotty-2023.4/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.3/scotty` & `avnet-scotty-2023.4/scotty`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/simplecore-tools:2023.3"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/simplecore-tools:2023.4"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.3"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2023.4"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
@@ -110,15 +110,19 @@
 	if [ -z "${SSH_AUTH_SOCK:-}" ]; then
 		eval "$(ssh-agent)"
 		if [ -z "${SSH_AUTH_SOCK:-}" ]; then
 			error "Could not start ssh-agent and no other SSH_AUTH_SOCK found.\nPlease make sure to have a suitable ssh-agent installed and configured"
 			exit 1
 		fi
 	fi
-	ssh-add -l 2>/dev/null 1>/dev/null || ssh-add 2>/dev/null 1>/dev/null
+	if [ ! "$(ssh-add -l &>/dev/null || ssh-add &>/dev/null)" ]; then
+		# in case the operation fails, we will just map the user's ssh keys
+		# into the container
+		docker_args+=(--volume "$HOME/.ssh:/home/scotty/.ssh")
+	fi
 	ssh_auth_sock=$(readlink --canonicalize "${SSH_AUTH_SOCK}")
 	docker_args+=(--volume "${ssh_auth_sock}:/ssh-agent")
 	docker_args+=(--env "SSH_AUTH_SOCK=/ssh-agent")
 	if [ -n "${DISPLAY:-}" ]; then
 		docker_args+=(--env "DISPLAY=${DISPLAY}")
 		docker_args+=(--volume "/tmp/.X11-unix:/tmp/.X11-unix")
 	fi
@@ -147,17 +151,19 @@
 
 docker_update() {
 	info "Updating docker image"
 	docker pull "${docker_default_image}"
 }
 
 docker_update_on_demand() {
-	if [ -e "${outdir}/.do_docker_pull" ]; then
+	if [ -e "${outdir}/.do_docker_pull" ] ; then
 		rm "${outdir}/.do_docker_pull"
-		docker_update
+		if [ "${SCOTTY_USE_LOCAL_DOCKERFILE:-0}" == "0" ]; then
+			docker_update
+		fi
 	fi
 }
 
 run_in_docker() {
 	# Run a command in a new docker instance
 	local docker_instance
 	local -a docker_cmd
```

### Comparing `avnet-scotty-2023.3/scotty-runqemu` & `avnet-scotty-2023.4/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.3/scripts/vm_bundle.sh` & `avnet-scotty-2023.4/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.3/scripts/vm_create.sh.template` & `avnet-scotty-2023.4/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet-scotty-2023.3/setup.py` & `avnet-scotty-2023.4/setup.py`

 * *Files identical despite different names*

