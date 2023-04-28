# Comparing `tmp/netsuite_python-1.5.5.tar.gz` & `tmp/netsuite_python-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuite_python-1.5.5.tar", last modified: Tue Apr 25 18:31:14 2023, max compression
+gzip compressed data, was "netsuite_python-1.5.6.tar", last modified: Fri Apr 28 19:27:15 2023, max compression
```

## Comparing `netsuite_python-1.5.5.tar` & `netsuite_python-1.5.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.458414 netsuite_python-1.5.5/
--rw-rw-rw-   0        0        0     5636 2023-04-25 18:31:14.458414 netsuite_python-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     5306 2023-04-25 18:29:11.000000 netsuite_python-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.440415 netsuite_python-1.5.5/netsuite/
--rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.5/netsuite/Netsuite.py
--rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/NetsuiteToken.py
--rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.443414 netsuite_python-1.5.5/netsuite/api_clients/
--rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.5/netsuite/api_clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.446414 netsuite_python-1.5.5/netsuite/api_clients/api/
--rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.5/netsuite/api_clients/api/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.5/netsuite/api_clients/api/query_api.py
--rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.5.5/netsuite/api_clients/api/restlet_api.py
--rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.5/netsuite/api_clients/api_client.py
--rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.5/netsuite/api_clients/configuration.py
--rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.5/netsuite/api_clients/rest.py
--rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/exceptions.py
--rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/module_loading.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.448414 netsuite_python-1.5.5/netsuite/netsuite_rest_client/
--rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.5/netsuite/netsuite_rest_client/__init__.py
--rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.5/netsuite/netsuite_rest_client/rest_api_client.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.449418 netsuite_python-1.5.5/netsuite/scripts/
--rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/scripts/__init__.py
--rw-rw-rw-   0        0        0    11109 2023-04-25 18:27:59.000000 netsuite_python-1.5.5/netsuite/scripts/cli.py
--rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.5/netsuite/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.452415 netsuite_python-1.5.5/netsuite/storages/
--rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/BaseStorage.py
--rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/InMemoryStorage.py
--rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/JSONStorage.py
--rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.5/netsuite/storages/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 18:31:14.457414 netsuite_python-1.5.5/netsuite_python.egg-info/
--rw-rw-rw-   0        0        0     5636 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       81 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-25 18:31:14.000000 netsuite_python-1.5.5/netsuite_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 18:31:14.459414 netsuite_python-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0      961 2023-04-25 18:31:05.000000 netsuite_python-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.744088 netsuite_python-1.5.6/
+-rw-rw-rw-   0        0        0     5438 2023-04-28 19:27:15.743086 netsuite_python-1.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5108 2023-04-25 19:14:38.000000 netsuite_python-1.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.713521 netsuite_python-1.5.6/netsuite/
+-rw-rw-rw-   0        0        0    12072 2023-04-25 18:30:40.000000 netsuite_python-1.5.6/netsuite/Netsuite.py
+-rw-rw-rw-   0        0        0      494 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/NetsuiteToken.py
+-rw-rw-rw-   0        0        0       74 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.720638 netsuite_python-1.5.6/netsuite/api_clients/
+-rw-rw-rw-   0        0        0      235 2023-04-09 19:43:22.000000 netsuite_python-1.5.6/netsuite/api_clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.725638 netsuite_python-1.5.6/netsuite/api_clients/api/
+-rw-rw-rw-   0        0        0       59 2023-04-09 19:48:25.000000 netsuite_python-1.5.6/netsuite/api_clients/api/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-04-09 19:49:23.000000 netsuite_python-1.5.6/netsuite/api_clients/api/query_api.py
+-rw-rw-rw-   0        0        0     2249 2023-04-09 19:48:25.000000 netsuite_python-1.5.6/netsuite/api_clients/api/restlet_api.py
+-rw-rw-rw-   0        0        0    25577 2023-04-09 19:51:26.000000 netsuite_python-1.5.6/netsuite/api_clients/api_client.py
+-rw-rw-rw-   0        0        0     8466 2023-03-23 15:55:18.000000 netsuite_python-1.5.6/netsuite/api_clients/configuration.py
+-rw-rw-rw-   0        0        0    13259 2023-04-06 18:39:08.000000 netsuite_python-1.5.6/netsuite/api_clients/rest.py
+-rw-rw-rw-   0        0        0      243 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/exceptions.py
+-rw-rw-rw-   0        0        0     3921 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.728076 netsuite_python-1.5.6/netsuite/netsuite_rest_client/
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:05:59.000000 netsuite_python-1.5.6/netsuite/netsuite_rest_client/__init__.py
+-rw-rw-rw-   0        0        0      463 2023-04-17 18:07:52.000000 netsuite_python-1.5.6/netsuite/netsuite_rest_client/rest_api_client.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.731085 netsuite_python-1.5.6/netsuite/scripts/
+-rw-rw-rw-   0        0        0        0 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11984 2023-04-28 19:26:48.000000 netsuite_python-1.5.6/netsuite/scripts/cli.py
+-rw-rw-rw-   0        0        0     6300 2023-04-17 18:30:20.000000 netsuite_python-1.5.6/netsuite/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.738086 netsuite_python-1.5.6/netsuite/storages/
+-rw-rw-rw-   0        0        0      324 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/storages/BaseStorage.py
+-rw-rw-rw-   0        0        0      653 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/storages/InMemoryStorage.py
+-rw-rw-rw-   0        0        0     1594 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/storages/JSONStorage.py
+-rw-rw-rw-   0        0        0      119 2023-02-12 19:28:31.000000 netsuite_python-1.5.6/netsuite/storages/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-28 19:27:15.742087 netsuite_python-1.5.6/netsuite_python.egg-info/
+-rw-rw-rw-   0        0        0     5438 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       81 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-28 19:27:15.000000 netsuite_python-1.5.6/netsuite_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-28 19:27:15.744088 netsuite_python-1.5.6/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-04-28 19:27:00.000000 netsuite_python-1.5.6/setup.py
```

### Comparing `netsuite_python-1.5.5/PKG-INFO` & `netsuite_python-1.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-Metadata-Version: 2.1
-Name: netsuite_python
-Version: 1.5.5
-Summary: Python SDK for Netsuite API with Flask Integration
-Home-page: https://bitbucket.org/theapiguys/netsuite_python
-Author: Will @ TheAPIGuys
-Author-email: will@theapiguys.com
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 # README #
 
+
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-## QUICK START ##
+# QUICK START #
 
-### Prerequisite  Setup ###
+## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
-        * Rest Web Services
-        * Rest Web Services
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -44,84 +32,99 @@
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
 
 
- ### Setup The Easy Way  ###
+## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
 
 #### Usage ####
-```
+```python
 # import Netsuite Package
 from netsuite import Netsuite
 # import the generated Client
 from netsuite_rest_client import apis, rest_api_client
+# import models
+from netsuite_rest_client.model.customer import Customer
 # instantiate the SDK
 netsuite = Netsuite()
 # Instantiate the generated Client
 rest_client = rest_api_client.RestApiClient(netsuite)
 # Instantiate the generated API endpoints using the generated client
 customer_api = apis.CustomerApi(rest_client)
 
+
 ```
 
- #### Notes ####
+#### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
       * Certificate ID
         * A Certificate can be generated once you register the package with CLI with 'netsuite generate-certificate' 
         * Cert ID is available under Setup -> Integration -> OAuth 2.0 Client Credentials once the certificate is uploaded.
 
-## Setup the hard way ##
+## Use Restlets ##
+saved search example ref: https://timdietrich.me/blog/netsuite-saved-search-api/
+```python
+# import restlet client
+restlet_client = netsuite.RESTLET_CLIENT.restlet_api
+# create body params 
+body_params = {"searchID": 'customsearch184275'}
+# call restlet
+print(restlet_client.execute_restlet(script=1999, deploy=1, body_params=body))
+```
+
+## Regenerating the API Client with more records types
+re-run ```netsuite generate-rest-client```
+* when asked about using more record types, choose option that lets you set them
+* pick record types from the list
+* complete prompts
+
+## Uploading x509 certificate to Netsuite ##
+* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
+* Click `Create-New` button
+    * Entity: The User created for TAG
+    * ROLE: Role created for this integration
+    * Application: Application Created for this integration
+    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
+* Copy the Certificate ID
+
+
+# Other Commands #
 
 ## Generating x509 certificate for Netsuite ###
  * Run `netsuite generate-certificate`
    * Domain: theapiguys.com
    * Organization: TAG 
    * Department: DEV
    * City: BOSTON
    * State: MA
    * Country: US
    * Email: will@theapiguys.com
  
  * It will store the cert in a file in the root of the project under config/netsuite
 
-## Uploading x509 certificate to Netsuite ##
-* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
-* Click `Create-New` button
-    * Entity: The User created for TAG
-    * ROLE: Role created for this integration
-    * Application: Application Created for this integration
-    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
-* Copy the Certificate ID
 
-## Generate Netsuite Client ##
-* Run command to generate sdk using openapi 3.0 
-* method is generate_swagger_client
-* visit link returned from method and download result 
-* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
-        * Netsuite Application Name
-        * Allow None
-        * Use Datetime
+        * Netsuite Application Name 
         * Storage Class
       
     * If you want to save to file
         * Provide a valid path for netsuite-credentials.json
         * else the credentials will be echoed out
     * To confirm, check the netsuite credentials path you entered, or the default, and there should be a json file with all
       the info you entered. Verify the details.
@@ -130,31 +133,8 @@
 * Run `$netsuite get-access-token`
     * Use the defaults or repeat the info used above for
         * Path to Netsuite Credentials
     * Confirm the app name to be refreshed, if single app, just use default
 * That's it! You should now have a valid token to use with the Netsuite API.
 
 
-## Usage ##
-
-
-It is pretty simple to get started using the SDK once you have a valid token.
-
-### Setup Netsuite ###
-```
-from netsuite import Netsuite
-import netsuite_client
-from netsuite_client.api.customer_api import CustomerApi
-
-netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
-
-customer_api = CustomerApi(netsuite.REST_CLIENT)
-
-print(customer_api.customer_id_get(id=1617260))
-```
-
-## Example Usage ##
- ```
- print(ns_contact_api.contact_id_get(id=1413220))
- ```
-
```

### Comparing `netsuite_python-1.5.5/README.md` & `netsuite_python-1.5.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+Metadata-Version: 2.1
+Name: netsuite_python
+Version: 1.5.6
+Summary: Python SDK for Netsuite API with Flask Integration
+Home-page: https://bitbucket.org/theapiguys/netsuite_python
+Author: Will @ TheAPIGuys
+Author-email: will@theapiguys.com
+License: UNKNOWN
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+
 # README #
 
+
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-## QUICK START ##
+# QUICK START #
 
-### Prerequisite  Setup ###
+## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
-        * Rest Web Services
-        * Rest Web Services
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -33,84 +43,99 @@
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
 
 
- ### Setup The Easy Way  ###
+## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
 
 #### Usage ####
-```
+```python
 # import Netsuite Package
 from netsuite import Netsuite
 # import the generated Client
 from netsuite_rest_client import apis, rest_api_client
+# import models
+from netsuite_rest_client.model.customer import Customer
 # instantiate the SDK
 netsuite = Netsuite()
 # Instantiate the generated Client
 rest_client = rest_api_client.RestApiClient(netsuite)
 # Instantiate the generated API endpoints using the generated client
 customer_api = apis.CustomerApi(rest_client)
 
+
 ```
 
- #### Notes ####
+#### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
       * Certificate ID
         * A Certificate can be generated once you register the package with CLI with 'netsuite generate-certificate' 
         * Cert ID is available under Setup -> Integration -> OAuth 2.0 Client Credentials once the certificate is uploaded.
 
-## Setup the hard way ##
+## Use Restlets ##
+saved search example ref: https://timdietrich.me/blog/netsuite-saved-search-api/
+```python
+# import restlet client
+restlet_client = netsuite.RESTLET_CLIENT.restlet_api
+# create body params 
+body_params = {"searchID": 'customsearch184275'}
+# call restlet
+print(restlet_client.execute_restlet(script=1999, deploy=1, body_params=body))
+```
+
+## Regenerating the API Client with more records types
+re-run ```netsuite generate-rest-client```
+* when asked about using more record types, choose option that lets you set them
+* pick record types from the list
+* complete prompts
+
+## Uploading x509 certificate to Netsuite ##
+* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
+* Click `Create-New` button
+    * Entity: The User created for TAG
+    * ROLE: Role created for this integration
+    * Application: Application Created for this integration
+    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
+* Copy the Certificate ID
+
+
+# Other Commands #
 
 ## Generating x509 certificate for Netsuite ###
  * Run `netsuite generate-certificate`
    * Domain: theapiguys.com
    * Organization: TAG 
    * Department: DEV
    * City: BOSTON
    * State: MA
    * Country: US
    * Email: will@theapiguys.com
  
  * It will store the cert in a file in the root of the project under config/netsuite
 
-## Uploading x509 certificate to Netsuite ##
-* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
-* Click `Create-New` button
-    * Entity: The User created for TAG
-    * ROLE: Role created for this integration
-    * Application: Application Created for this integration
-    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
-* Copy the Certificate ID
 
-## Generate Netsuite Client ##
-* Run command to generate sdk using openapi 3.0 
-* method is generate_swagger_client
-* visit link returned from method and download result 
-* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
-        * Netsuite Application Name
-        * Allow None
-        * Use Datetime
+        * Netsuite Application Name 
         * Storage Class
       
     * If you want to save to file
         * Provide a valid path for netsuite-credentials.json
         * else the credentials will be echoed out
     * To confirm, check the netsuite credentials path you entered, or the default, and there should be a json file with all
       the info you entered. Verify the details.
@@ -119,29 +144,10 @@
 * Run `$netsuite get-access-token`
     * Use the defaults or repeat the info used above for
         * Path to Netsuite Credentials
     * Confirm the app name to be refreshed, if single app, just use default
 * That's it! You should now have a valid token to use with the Netsuite API.
 
 
-## Usage ##
-
-
-It is pretty simple to get started using the SDK once you have a valid token.
-
-### Setup Netsuite ###
-```
-from netsuite import Netsuite
-import netsuite_client
-from netsuite_client.api.customer_api import CustomerApi
 
-netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
 
-customer_api = CustomerApi(netsuite.REST_CLIENT)
-
-print(customer_api.customer_id_get(id=1617260))
-```
 
-## Example Usage ##
- ```
- print(ns_contact_api.contact_id_get(id=1413220))
- ```
```

### Comparing `netsuite_python-1.5.5/netsuite/Netsuite.py` & `netsuite_python-1.5.6/netsuite/Netsuite.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/api_clients/api/query_api.py` & `netsuite_python-1.5.6/netsuite/api_clients/api/query_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/api_clients/api/restlet_api.py` & `netsuite_python-1.5.6/netsuite/api_clients/api/restlet_api.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/api_clients/api_client.py` & `netsuite_python-1.5.6/netsuite/api_clients/api_client.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/api_clients/configuration.py` & `netsuite_python-1.5.6/netsuite/api_clients/configuration.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/api_clients/rest.py` & `netsuite_python-1.5.6/netsuite/api_clients/rest.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/module_loading.py` & `netsuite_python-1.5.6/netsuite/module_loading.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/scripts/cli.py` & `netsuite_python-1.5.6/netsuite/scripts/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -134,14 +134,32 @@
         print(f"  5. Copy the Certificate ID for when you generate the client config")
 
 @cli.command()
 def generate_client_config():
     generate_netsuite_client_config()
 
 def generate_netsuite_client_config():
+    try:
+        netsuite = Netsuite()
+        if netsuite.api_settings.CLIENT_ID is not None:
+            from pprint import pprint
+            print("Netsuite Credentials Found.")
+            print("     CURRENT CONFIG")
+            print("-------------------------")
+            pprint(netsuite.api_settings.__dict__.get('_user_settings'), indent=4)
+            # print(f"Client ID: {netsuite.api_settings.CLIENT_ID}")
+            # print(f"Client ID: {netsuite.api_settings.CLIENT_ID}")
+            # print(f"Client ID: {netsuite.api_settings.CLIENT_ID}")
+            # print(f"Client ID: {netsuite.api_settings.CLIENT_ID}")
+            # print(f"Client ID: {netsuite.api_settings.CLIENT_ID}")
+            print("\n")
+            if prompt("Keep settings?", type=click.BOOL, default=True):
+                return
+    except Exception:
+        print("")
     print("****************************")
     print("  GENERATE NETSUITE CONFIG")
     print("****************************")
     steps_completed = False
     while not steps_completed:
         steps_completed = prompt(f"Have you created the integration record by following the steps in the README?", default='y', type=click.BOOL, show_choices=True)
         if steps_completed:
```

### Comparing `netsuite_python-1.5.5/netsuite/settings.py` & `netsuite_python-1.5.6/netsuite/settings.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/storages/InMemoryStorage.py` & `netsuite_python-1.5.6/netsuite/storages/InMemoryStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite/storages/JSONStorage.py` & `netsuite_python-1.5.6/netsuite/storages/JSONStorage.py`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/netsuite_python.egg-info/PKG-INFO` & `netsuite_python-1.5.6/netsuite_python.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: netsuite-python
-Version: 1.5.5
+Version: 1.5.6
 Summary: Python SDK for Netsuite API with Flask Integration
 Home-page: https://bitbucket.org/theapiguys/netsuite_python
 Author: Will @ TheAPIGuys
 Author-email: will@theapiguys.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # README #
 
+
 This library makes it easy to set up a Netsuite authorization without needing a frontend client using CLI utilities.
 
 ### Docs ###
 [Netsuite API Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158022624537.html)
 
 ## What do I need to get set up? ##
 * Run `pip install netsuite-python`
 * Activate your python VENV
 * If using virtual environment 
   * Activate your virtual environment
   * `netsuite = python venv/bin/keap`
 
-## QUICK START ##
+# QUICK START #
 
-### Prerequisite  Setup ###
+## Prerequisite  Setup ##
     1. Enable Services
         * Restlets
         * Rest Web Services
-        * Rest Web Services
-        * Rest Web Services
     2. Create a role for the integration with the following permissions:
         * Access Token Management
         * Log in using Access Tokens	
         * Log in using OAuth 2.0 Access Tokens	
         * OAuth 2.0 Authorized Applications Management	
         * REST Web Services	
         * SuiteApp Deployment	
@@ -44,84 +43,99 @@
         * Check Client Credentials ( MAchine to Machine Grant)
         * Under Scope Select 
             * Restlets
             * Rest Web Services
         * STORE THE CLIENT ID 
 
 
- ### Setup The Easy Way  ###
+## Setup The Easy Way  ##
 run ``` netsuite initialize ```
 * Follow the prompts
 
 * Docs will be located in the generated "netsuite_rest_client folder" at the rot of the project
 
 #### Usage ####
-```
+```python
 # import Netsuite Package
 from netsuite import Netsuite
 # import the generated Client
 from netsuite_rest_client import apis, rest_api_client
+# import models
+from netsuite_rest_client.model.customer import Customer
 # instantiate the SDK
 netsuite = Netsuite()
 # Instantiate the generated Client
 rest_client = rest_api_client.RestApiClient(netsuite)
 # Instantiate the generated API endpoints using the generated client
 customer_api = apis.CustomerApi(rest_client)
 
+
 ```
 
- #### Notes ####
+#### Notes ####
   * Requirements
     * Sandbox requires the same setup as Prod, it DOES NOT copy over
     * An administrator for the Netsuite app to follow the steps [here](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157771281570.html)
       * A user with the correct role
       * A role with the correct permissions
       * An Integration Record with the correct permissions (ensure default form is set correctly)
         * Client ID and Secret comes from this step, ensure they provide these
       * Certificate ID
         * A Certificate can be generated once you register the package with CLI with 'netsuite generate-certificate' 
         * Cert ID is available under Setup -> Integration -> OAuth 2.0 Client Credentials once the certificate is uploaded.
 
-## Setup the hard way ##
+## Use Restlets ##
+saved search example ref: https://timdietrich.me/blog/netsuite-saved-search-api/
+```python
+# import restlet client
+restlet_client = netsuite.RESTLET_CLIENT.restlet_api
+# create body params 
+body_params = {"searchID": 'customsearch184275'}
+# call restlet
+print(restlet_client.execute_restlet(script=1999, deploy=1, body_params=body))
+```
+
+## Regenerating the API Client with more records types
+re-run ```netsuite generate-rest-client```
+* when asked about using more record types, choose option that lets you set them
+* pick record types from the list
+* complete prompts
+
+## Uploading x509 certificate to Netsuite ##
+* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
+* Click `Create-New` button
+    * Entity: The User created for TAG
+    * ROLE: Role created for this integration
+    * Application: Application Created for this integration
+    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
+* Copy the Certificate ID
+
+
+# Other Commands #
 
 ## Generating x509 certificate for Netsuite ###
  * Run `netsuite generate-certificate`
    * Domain: theapiguys.com
    * Organization: TAG 
    * Department: DEV
    * City: BOSTON
    * State: MA
    * Country: US
    * Email: will@theapiguys.com
  
  * It will store the cert in a file in the root of the project under config/netsuite
 
-## Uploading x509 certificate to Netsuite ##
-* On Client's Netsuite top ribbon go to `Setup -> Integration -> OAuth 2.0 Client Credentials`
-* Click `Create-New` button
-    * Entity: The User created for TAG
-    * ROLE: Role created for this integration
-    * Application: Application Created for this integration
-    * Certificate: Click "Choose A File" and upload the PUBLIC Cert (called netsuite-certificate.pem by default)
-* Copy the Certificate ID
 
-## Generate Netsuite Client ##
-* Run command to generate sdk using openapi 3.0 
-* method is generate_swagger_client
-* visit link returned from method and download result 
-* unzip the file and copy the "netsuite_client" folder from the directory into the projects root folder
 ## Setting up Netsuite SDK in a project ##
 * Run `netsuite generate-client-config`
     * It will ask you for information obtained above: You can use all the defaults
         * Client ID
         * Netsuite Certificate ID
         * Netsuite Key File
-        * Netsuite Application Name
-        * Allow None
-        * Use Datetime
+        * Netsuite Application Name 
         * Storage Class
       
     * If you want to save to file
         * Provide a valid path for netsuite-credentials.json
         * else the credentials will be echoed out
     * To confirm, check the netsuite credentials path you entered, or the default, and there should be a json file with all
       the info you entered. Verify the details.
@@ -130,31 +144,10 @@
 * Run `$netsuite get-access-token`
     * Use the defaults or repeat the info used above for
         * Path to Netsuite Credentials
     * Confirm the app name to be refreshed, if single app, just use default
 * That's it! You should now have a valid token to use with the Netsuite API.
 
 
-## Usage ##
-
-
-It is pretty simple to get started using the SDK once you have a valid token.
-
-### Setup Netsuite ###
-```
-from netsuite import Netsuite
-import netsuite_client
-from netsuite_client.api.customer_api import CustomerApi
-
-netsuite = Netsuite(config_file=settings.NS_CREDENTIALS_PATH)
-
-customer_api = CustomerApi(netsuite.REST_CLIENT)
-
-print(customer_api.customer_id_get(id=1617260))
-```
 
-## Example Usage ##
- ```
- print(ns_contact_api.contact_id_get(id=1413220))
- ```
```

### Comparing `netsuite_python-1.5.5/netsuite_python.egg-info/SOURCES.txt` & `netsuite_python-1.5.6/netsuite_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netsuite_python-1.5.5/setup.py` & `netsuite_python-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='netsuite_python',
-    version='1.5.5',
+    version='1.5.6',
     description='Python SDK for Netsuite API with Flask Integration',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://bitbucket.org/theapiguys/netsuite_python',
     readme="README.md",
     author='Will @ TheAPIGuys',
     author_email='will@theapiguys.com',
```

