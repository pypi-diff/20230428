# Comparing `tmp/pyxecm-0.0.10.tar.gz` & `tmp/pyxecm-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.10.tar", last modified: Fri Apr 28 18:54:35 2023, max compression
+gzip compressed data, was "pyxecm-0.0.11.tar", last modified: Fri Apr 28 21:55:58 2023, max compression
```

## Comparing `pyxecm-0.0.10.tar` & `pyxecm-0.0.11.tar`

### file list

```diff
@@ -1,22 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:54:35.649446 pyxecm-0.0.10/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-04-28 18:54:15.000000 pyxecm-0.0.10/LICENSE
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 18:54:35.648446 pyxecm-0.0.10/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-28 18:54:15.000000 pyxecm-0.0.10/README.md
--rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-28 18:54:24.000000 pyxecm-0.0.10/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 18:54:35.649446 pyxecm-0.0.10/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:54:35.637446 pyxecm-0.0.10/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:54:35.646446 pyxecm-0.0.10/src/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      138 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    28270 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)     3784 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   211912 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   115022 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10226 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-28 18:54:15.000000 pyxecm-0.0.10/src/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 18:54:35.648446 pyxecm-0.0.10/src/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 18:54:35.000000 pyxecm-0.0.10/src/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2023-04-28 18:54:35.000000 pyxecm-0.0.10/src/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 18:54:35.000000 pyxecm-0.0.10/src/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 18:54:35.000000 pyxecm-0.0.10/src/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 18:54:35.000000 pyxecm-0.0.10/src/pyxecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:55:58.745713 pyxecm-0.0.11/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-04-28 21:55:41.000000 pyxecm-0.0.11/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 21:55:58.744713 pyxecm-0.0.11/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-28 21:55:41.000000 pyxecm-0.0.11/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-04-28 21:55:47.000000 pyxecm-0.0.11/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-28 21:55:58.745713 pyxecm-0.0.11/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:55:58.732712 pyxecm-0.0.11/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:55:58.739713 pyxecm-0.0.11/src/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      163 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28270 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   219758 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   115022 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1586 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10226 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   224230 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     2394 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2695 2023-04-28 21:55:41.000000 pyxecm-0.0.11/src/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:55:58.741713 pyxecm-0.0.11/src/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 21:55:58.000000 pyxecm-0.0.11/src/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      578 2023-04-28 21:55:58.000000 pyxecm-0.0.11/src/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 21:55:58.000000 pyxecm-0.0.11/src/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 21:55:58.000000 pyxecm-0.0.11/src/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-28 21:55:58.000000 pyxecm-0.0.11/src/pyxecm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 21:55:58.744713 pyxecm-0.0.11/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_otac.py
+-rw-rw-rw-   0 root         (0) root         (0)     9518 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2766 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_otds.py
+-rw-rw-rw-   0 root         (0) root         (0)      597 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)      788 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_translate.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-28 21:55:41.000000 pyxecm-0.0.11/tests/test_web.py
```

### Comparing `pyxecm-0.0.10/LICENSE` & `pyxecm-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/PKG-INFO` & `pyxecm-0.0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.10
+Version: 0.0.11
 Summary: A library to connect to Opentext Extended ECM
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyxecm-0.0.10/pyproject.toml` & `pyxecm-0.0.11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36"]
   description = "A library to connect to Opentext Extended ECM"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.10"
+  version = "0.0.11"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.10/src/pyxecm/k8s.py` & `pyxecm-0.0.11/src/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm/otac.py` & `pyxecm-0.0.11/src/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm/otcs.py` & `pyxecm-0.0.11/src/pyxecm/otcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,17 @@
 addExternalSystemConnection: Add Extended ECM external system connection
 
 createTransportWorkbench: Create a Workbench in the Transport Volume
 unpackTransportPackage: Unpack an existing Transport Package into an existing Workbench
 deployWorkbench: Deploy an existing Workbench
 deployTransport: Main method to deploy a transport. This uses subfunctions to upload,
                  unpackage and deploy the transport, and creates the required workbench
+replaceInXmlFiles: Replaces all occurrences of the search pattern with the replace string in all
+                   XML files in the directory and its subdirectories.
+replaceTransportPlaceholders: Search and replace strings in the XML files of the transport packlage
 
 getWorkspaceTypes: Get all workspace types configured in Extended ECM
 getBusinessObjectType: Get information for a specific business object type
 getWorkspaceCreateForm: Get the Workspace create form
 getWorkspace: get a workspace node
 getWorkspaceByNameAndType: Lookup workspace based on workspace name and workspace type name
 createWorkspace: Create a new business workspace
@@ -122,14 +125,16 @@
 
 import os
 import logging
 import requests
 import json
 import urllib.parse
 from datetime import datetime
+import zipfile
+import re
 
 logger = logging.getLogger(os.path.basename(__file__))
 
 requestJsonHeaders = {
     "accept": "application/json;charset=utf-8",
     "Content-Type": "application/json",
 }
@@ -2790,23 +2795,27 @@
                     )
                 )
                 return None
 
     # end method definition
 
     def deployTransport(
-        self, package_url: str, package_name: str, package_description: str = ""
+        self, package_url: str, package_name: str, package_description: str = "", replacements: list = []
     ):
         """Main method to deploy a transport. This uses subfunctions to upload,
            unpackage and deploy the transport, and creates the required workbench.
 
         Args:
             package_url (string): URL to download the transport package.
             package_name (string): name of the transport package ZIP file
             package_description (string): description of the transport package
+            replacements (list of dicts): list of replacement values to be applied
+                                          to all XML files in transport; dict needs to have two values:
+                                         * placeholder: text to replace
+                                         * value: text to replace with
         Return:
             Deploy response (json) or None if the deployment fails.
         """
 
         # Preparation: get volume IDs for Transport Warehouse (root volume and Transport Packages)
         response = self.getVolume(525)
         transport_root_volume_id = self.getResultValue(response, "id")
@@ -2840,18 +2849,25 @@
             logger.info(
                 "Transport package -> {} does already exist; existing package ID -> {}".format(
                     package_name, package_id
                 )
             )
         else:
             logger.info(
-                "Transport package -> {} does not yet exist, fetching from URL -> {}".format(
+                "Transport package -> {} does not yet exist, loading from -> {}".format(
                     package_name, package_url
                 )
             )
+            # If we have string replacements configured execute them now:
+            if replacements:
+                logger.info("Transport -> {} has replacements -> {}".format(package_name, replacements))
+                self.replaceTransportPlaceholders(package_url, replacements)
+            else:
+                logger.info("Transport -> {} has no replacements!".format(package_name))
+            # Upload package to Extended ECM:
             response = self.uploadFileToVolume(
                 package_url, package_name, "application/zip", 531
             )
             package_id = self.getResultValue(response, "id")
             if not package_id:
                 logger.error(
                     "Failed to upload transport package -> {}".format(
@@ -2953,14 +2969,116 @@
             package_description,
         )
 
         return response
 
     # end method definition
 
+    def replaceInXmlFiles(self, directory: str, search_pattern: str, replace_string: str) -> bool:
+        """ Replaces all occurrences of the search pattern with the replace string in all XML files
+            in the directory and its subdirectories.
+
+        Args:
+            directory (string): directory to traverse for XML files
+            search_pattern (sting): string to search in the XML file
+            replace_string (string): replacement string
+
+        Returns:
+            bool: True if a replacement happened, False otherwise
+        """
+        # Define the regular expression pattern to search for
+        pattern = re.compile(search_pattern)
+        found = False
+
+        # Traverse the directory and its subdirectories
+        for subdir, dirs, files in os.walk(directory):
+            for file in files:
+                # Check if the file is an XML file
+                if file.endswith(".xml"):
+                    # Read the contents of the file
+                    file_path = os.path.join(subdir, file)
+                    with open(file_path, "r") as f:
+                        contents = f.read()
+
+                    # Replace all occurrences of the search pattern with the replace string
+                    new_contents = pattern.sub(replace_string, contents)
+
+                    # Write the updated contents to the file if there were replacements
+                    if contents != new_contents:
+                        logger.info("Found search string -> {} in XML file -> {}. Updating content...".format(search_pattern, file_path))
+                        # Write the updated contents to the file
+                        with open(file_path, "w") as f:
+                            f.write(new_contents)
+                        found = True
+
+        return found
+    
+        # end method definition
+
+    def replaceTransportPlaceholders(self, zip_file_path: str, replacements: list) -> bool:
+        """ Search and replace strings in the XML files of the transport packlage
+
+        Args:
+            zip_file_path (string): path to transport zip file
+            replacements (list of dicts): list of replacement values; dict needs to have two values:
+                                         * placeholder: text to replace
+                                         * value: text to replace with
+
+        Returns:
+            Filename to the updated zip file
+        """
+
+        if not os.path.isfile(zip_file_path):
+            logger.error("Zip file -> {} not found.".format(zip_file_path))
+            return False
+
+        # Extract the zip file to a temporary directory
+        zip_file_folder = os.path.splitext(zip_file_path)[0]
+        with zipfile.ZipFile(zip_file_path, "r") as zfile:
+            zfile.extractall(zip_file_folder)
+
+        modified = False
+
+        # Replace search pattern with replace string in all XML files in the directory and its subdirectories
+        for replacement in replacements:
+            logger.info("Replace -> {} with -> {} in Transport package -> {}".format(replacement["placeholder"], replacement["value"], zip_file_folder))
+            found = self.replaceInXmlFiles(zip_file_folder, replacement["placeholder"], replacement["value"])
+            if found:
+                logger.info("Found replacement string -> {} in Transport package -> {}".format(replacement["placeholder"], zip_file_folder))
+                modified = True
+            else:
+                logger.warning("Did not find replacement string -> {} in Transport package -> {}".format(replacement["placeholder"], zip_file_folder))
+
+        if not modified:
+            logger.warning("None of the replacements have been found in transport -> {}".format(zip_file_folder))
+            return False
+
+        # Create the new zip file and add all files from the directory to it
+        new_zip_file_path = os.path.dirname(zip_file_path) + "/new_" + os.path.basename(zip_file_path)
+        logger.info("Content of transport -> {} has been modified - repacking to new zip file -> {}".format(zip_file_folder, new_zip_file_path))
+        with zipfile.ZipFile(new_zip_file_path, "w", zipfile.ZIP_DEFLATED) as zip_ref:
+            for subdir, dirs, files in os.walk(zip_file_folder):
+                for file in files:
+                    file_path = os.path.join(subdir, file)
+                    rel_path = os.path.relpath(file_path, zip_file_folder)
+                    zip_ref.write(file_path, arcname=rel_path)
+
+        # Close the new zip file and delete the temporary directory
+        zip_ref.close()
+        old_zip_file_path = os.path.dirname(zip_file_path) + "/old_" + os.path.basename(zip_file_path)
+        logger.info("Rename orginal transport zip file -> {} to -> {}".format(zip_file_path, old_zip_file_path))
+        os.rename(zip_file_path, old_zip_file_path)
+        logger.info("Rename new transport zip file -> {} to -> {}".format(new_zip_file_path, zip_file_path))
+        os.rename(new_zip_file_path, zip_file_path)
+
+        # Return the path to the new zip file
+        return True
+
+        # end method definition
+
     def getWorkspaceTypes(self):
         """Get all workspace types configured in Extended ECM.
 
         Args:
             None
         Return:
             Workspace Types (json) or None if the request fails.
@@ -5489,8 +5607,38 @@
                         supplemental_markings,
                         supplementalMarkingsResponse.status_code,
                         supplementalMarkingsResponse.text,
                     )
                 )
                 return None
 
-    # end method definition
+    # end method definition
+
+    def volumeTranslator(self, current_node_id: int, translator: object, languages: list):
+
+        # Get current node based on the ID:
+        current_node = self.getNode(current_node_id)
+        current_node_id = self.getResultValue(current_node, "id")
+
+        name = self.getResultValue(current_node, "name")
+        description = self.getResultValue(current_node, "description")
+        names_multilingual = self.getResultValue(current_node, "name_multilingual")
+        descriptions_multilingual = self.getResultValue(current_node, "description_multilingual")
+
+        for language in languages:
+            if language == "en":
+                continue
+            # Does the language not exist as metadata language or is it already translated?
+            # Then we skip this language:
+            if language in names_multilingual and names_multilingual["en"] and not names_multilingual[language]:
+                names_multilingual[language] = translator.translate("en", language, names_multilingual["en"])
+            if language in descriptions_multilingual and descriptions_multilingual["en"] and not descriptions_multilingual[language]:
+                descriptions_multilingual[language] = translator.translate("en", language, descriptions_multilingual["en"])
+
+        # Rename node multi-lingual:
+        response = self.renameNode(current_node_id, name, description, names_multilingual, descriptions_multilingual)
+
+        # Get children nodes of the current node:
+        results = self.getSubnodes(current_node_id, limit=200)["results"]
+
+        for result in results:
+            self.volumeTranslator(result["data"]["properties"]["id"], translator, languages)
```

### Comparing `pyxecm-0.0.10/src/pyxecm/otds.py` & `pyxecm-0.0.11/src/pyxecm/otds.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm/otiv.py` & `pyxecm-0.0.11/src/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm/otpd.py` & `pyxecm-0.0.11/src/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm/web.py` & `pyxecm-0.0.11/src/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.10/src/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.11/src/pyxecm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.10
+Version: 0.0.11
 Summary: A library to connect to Opentext Extended ECM
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

