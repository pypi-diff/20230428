# Comparing `tmp/trex-apis-1.0.0.tar.gz` & `tmp/trex-apis-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex-apis-1.0.0.tar", last modified: Mon Apr 17 03:30:13 2023, max compression
+gzip compressed data, was "trex-apis-1.0.1.tar", last modified: Fri Apr 28 10:20:58 2023, max compression
```

## Comparing `trex-apis-1.0.0.tar` & `trex-apis-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.528474 trex-apis-1.0.0/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-17 03:30:13.528585 trex-apis-1.0.0/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.0/README.md
--rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-17 03:30:13.529000 trex-apis-1.0.0/setup.cfg
--rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-04-17 03:27:06.000000 trex-apis-1.0.0/setup.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.517962 trex-apis-1.0.0/trex_apis.egg-info/
--rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/PKG-INFO
--rw-r--r--   0 jacklok    (501) staff       (20)     1164 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/SOURCES.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/dependency_links.txt
--rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/requires.txt
--rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-04-17 03:30:13.000000 trex-apis-1.0.0/trex_apis.egg-info/top_level.txt
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.518481 trex-apis-1.0.0/trexapi/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.0/trexapi/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)      728 2023-01-03 04:03:16.000000 trex-apis-1.0.0/trexapi/conf.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.525039 trex-apis-1.0.0/trexapi/controllers/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.0/trexapi/controllers/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7466 2023-03-08 14:11:16.000000 trex-apis-1.0.0/trexapi/controllers/api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.0/trexapi/controllers/app_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    35717 2023-04-12 10:19:52.000000 trex-apis-1.0.0/trexapi/controllers/customer_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.0/trexapi/controllers/customer_membership_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.0/trexapi/controllers/customer_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.0/trexapi/controllers/loyalty_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    10939 2023-03-21 01:50:25.000000 trex-apis-1.0.0/trexapi/controllers/outlet_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.0/trexapi/controllers/payment_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.0/trexapi/controllers/pos_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    27328 2023-04-12 09:15:21.000000 trex-apis-1.0.0/trexapi/controllers/reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.0/trexapi/controllers/user_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.0/trexapi/controllers/user_reward_api_routes.py
--rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.0/trexapi/controllers/voucher_api_routes.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.525512 trex-apis-1.0.0/trexapi/decorators/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.0/trexapi/decorators/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     4555 2023-03-21 09:28:04.000000 trex-apis-1.0.0/trexapi/decorators/api_decorators.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.526841 trex-apis-1.0.0/trexapi/forms/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.0/trexapi/forms/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.0/trexapi/forms/customer_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     7220 2023-02-20 04:25:05.000000 trex-apis-1.0.0/trexapi/forms/reward_api_forms.py
--rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.0/trexapi/forms/user_api_forms.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.527208 trex-apis-1.0.0/trexapi/libs/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.0/trexapi/libs/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.0/trexapi/libs/flask_auth_wrapper.py
-drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-17 03:30:13.528196 trex-apis-1.0.0/trexapi/utils/
--rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.0/trexapi/utils/__init__.py
--rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.0/trexapi/utils/api_helpers.py
--rw-r--r--   0 jacklok    (501) staff       (20)    74352 2023-04-12 06:10:24.000000 trex-apis-1.0.0/trexapi/utils/reward_transaction_helper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.080119 trex-apis-1.0.1/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-28 10:20:58.080278 trex-apis-1.0.1/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)       25 2021-06-30 02:28:26.000000 trex-apis-1.0.1/README.md
+-rw-r--r--   0 jacklok    (501) staff       (20)       75 2023-04-28 10:20:58.080863 trex-apis-1.0.1/setup.cfg
+-rw-r--r--   0 jacklok    (501) staff       (20)      713 2023-04-28 10:15:51.000000 trex-apis-1.0.1/setup.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.056928 trex-apis-1.0.1/trex_apis.egg-info/
+-rw-r--r--   0 jacklok    (501) staff       (20)      447 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/PKG-INFO
+-rw-r--r--   0 jacklok    (501) staff       (20)     1283 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/SOURCES.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        1 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/dependency_links.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)       23 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/requires.txt
+-rw-r--r--   0 jacklok    (501) staff       (20)        8 2023-04-28 10:20:57.000000 trex-apis-1.0.1/trex_apis.egg-info/top_level.txt
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.057376 trex-apis-1.0.1/trexapi/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:30:07.000000 trex-apis-1.0.1/trexapi/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      837 2023-04-19 06:13:09.000000 trex-apis-1.0.1/trexapi/conf.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.071145 trex-apis-1.0.1/trexapi/controllers/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-06-30 02:45:28.000000 trex-apis-1.0.1/trexapi/controllers/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11544 2023-04-24 08:15:59.000000 trex-apis-1.0.1/trexapi/controllers/api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2259 2022-11-14 14:26:16.000000 trex-apis-1.0.1/trexapi/controllers/app_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    35834 2023-04-25 09:25:42.000000 trex-apis-1.0.1/trexapi/controllers/customer_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     6945 2023-04-13 05:36:42.000000 trex-apis-1.0.1/trexapi/controllers/customer_membership_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4750 2023-01-30 07:03:11.000000 trex-apis-1.0.1/trexapi/controllers/customer_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    12965 2023-03-24 05:50:51.000000 trex-apis-1.0.1/trexapi/controllers/loyalty_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    11098 2023-04-24 10:10:40.000000 trex-apis-1.0.1/trexapi/controllers/outlet_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1430 2022-09-26 04:18:01.000000 trex-apis-1.0.1/trexapi/controllers/payment_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    22728 2023-01-13 04:39:15.000000 trex-apis-1.0.1/trexapi/controllers/pos_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    27329 2023-04-18 07:01:48.000000 trex-apis-1.0.1/trexapi/controllers/reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7315 2023-04-20 09:46:08.000000 trex-apis-1.0.1/trexapi/controllers/sales_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)      998 2023-04-18 06:08:18.000000 trex-apis-1.0.1/trexapi/controllers/transaction_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    36081 2023-04-03 08:51:30.000000 trex-apis-1.0.1/trexapi/controllers/user_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     2980 2023-01-30 02:56:35.000000 trex-apis-1.0.1/trexapi/controllers/user_reward_api_routes.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    15185 2023-04-07 15:27:24.000000 trex-apis-1.0.1/trexapi/controllers/voucher_api_routes.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.072252 trex-apis-1.0.1/trexapi/decorators/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-01 08:42:13.000000 trex-apis-1.0.1/trexapi/decorators/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     4555 2023-04-18 09:35:03.000000 trex-apis-1.0.1/trexapi/decorators/api_decorators.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.075430 trex-apis-1.0.1/trexapi/forms/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-12 06:42:53.000000 trex-apis-1.0.1/trexapi/forms/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7419 2023-02-08 10:14:32.000000 trex-apis-1.0.1/trexapi/forms/customer_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     7285 2023-04-18 02:42:03.000000 trex-apis-1.0.1/trexapi/forms/reward_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1547 2023-04-18 02:41:54.000000 trex-apis-1.0.1/trexapi/forms/sales_api_forms.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     3344 2023-01-18 01:16:56.000000 trex-apis-1.0.1/trexapi/forms/user_api_forms.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.076455 trex-apis-1.0.1/trexapi/libs/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-05 10:17:19.000000 trex-apis-1.0.1/trexapi/libs/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1143 2021-07-05 10:57:23.000000 trex-apis-1.0.1/trexapi/libs/flask_auth_wrapper.py
+drwxr-xr-x   0 jacklok    (501) staff       (20)        0 2023-04-28 10:20:58.078380 trex-apis-1.0.1/trexapi/utils/
+-rw-r--r--   0 jacklok    (501) staff       (20)        0 2021-07-08 10:01:06.000000 trex-apis-1.0.1/trexapi/utils/__init__.py
+-rw-r--r--   0 jacklok    (501) staff       (20)     1347 2022-12-20 01:23:01.000000 trex-apis-1.0.1/trexapi/utils/api_helpers.py
+-rw-r--r--   0 jacklok    (501) staff       (20)    76256 2023-04-24 10:05:07.000000 trex-apis-1.0.1/trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.0/setup.py` & `trex-apis-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
      name='trex-apis',  
-     version='1.0.0',
+     version='1.0.1',
      author="Jack Lok",
      author_email="sglok77@gmail.com",
      description="TRex APIs package",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://bitbucket.org/lokjac/trex-apis",
      packages=setuptools.find_packages(),
```

### Comparing `trex-apis-1.0.0/trex_apis.egg-info/SOURCES.txt` & `trex-apis-1.0.1/trex_apis.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,24 @@
 trexapi/controllers/customer_membership_api_routes.py
 trexapi/controllers/customer_reward_api_routes.py
 trexapi/controllers/loyalty_api_routes.py
 trexapi/controllers/outlet_api_routes.py
 trexapi/controllers/payment_api_routes.py
 trexapi/controllers/pos_api_routes.py
 trexapi/controllers/reward_api_routes.py
+trexapi/controllers/sales_api_routes.py
+trexapi/controllers/transaction_api_routes.py
 trexapi/controllers/user_api_routes.py
 trexapi/controllers/user_reward_api_routes.py
 trexapi/controllers/voucher_api_routes.py
 trexapi/decorators/__init__.py
 trexapi/decorators/api_decorators.py
 trexapi/forms/__init__.py
 trexapi/forms/customer_api_forms.py
 trexapi/forms/reward_api_forms.py
+trexapi/forms/sales_api_forms.py
 trexapi/forms/user_api_forms.py
 trexapi/libs/__init__.py
 trexapi/libs/flask_auth_wrapper.py
 trexapi/utils/__init__.py
 trexapi/utils/api_helpers.py
 trexapi/utils/reward_transaction_helper.py
```

### Comparing `trex-apis-1.0.0/trexapi/conf.py` & `trex-apis-1.0.1/trexapi/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,7 +9,9 @@
 SECRET_KEY                                                      = os.environ.get('SECRET_KEY')
 VERSION                                                         = '0.0.1'
 UPDATED_DATE                                                    = '5 July 2021'
 
 API_TOKEN_EXPIRY_LENGTH_IN_MINUTE                               = os.environ.get('API_TOKEN_EXPIRY_LENGTH_IN_MINUTE') 
 
 API_ERR_CODE_INVALID_ACTIVATION_CODE                            = 'invalid.activation.code';
+
+EARN_INSTANT_REWARD_URL                                         = os.environ.get('EARN_INSTANT_REWARD_URL')
```

### Comparing `trex-apis-1.0.0/trexapi/controllers/api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/api_routes.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from trexlib.utils.string_util import random_string, is_not_empty
 from flask.json import jsonify
 from datetime import datetime, timedelta
 from trexapi import conf as api_conf
 from trexlib.utils.crypto_util import encrypt_json
 from trexapi.decorators.api_decorators import auth_token_required
 from trexapi.libs.flask_auth_wrapper import HTTPBasicAuthWrapper
+from trexmodel.models.datastore.loyalty_models import LoyaltyDeviceSetting
+from trexmodel.models.datastore.pos_models import POSSetting
 
 #logger = logging.getLogger('api')
 logger = logging.getLogger('debug')
 
 auth = HTTPBasicAuth()
 #auth = HTTPBasicAuthWrapper()
 
@@ -136,62 +138,129 @@
     
 class AuthenticateAPIResource(APIBaseResource):  
     
     @auth.login_required
     def post(self):
         username    = auth.current_user()
         
-        acct_id = request.headers.get('x-acct-id')
-        api_key = request.headers.get('x-api-key')
+        acct_id     = request.headers.get('x-acct-id')
+        api_key     = request.headers.get('x-api-key')
+        outlet_key  = request.headers.get('x-outlet-key')
         
         logger.debug('acct_id=%s', acct_id)    
         logger.debug('api_key=%s', api_key)
+        logger.debug('outlet_key=%s', outlet_key)
         
-        is_authenticated = False
+        is_authenticated    = False
+        is_authorized       = False
         output_json = {}
         
         if is_not_empty(acct_id) and is_not_empty(api_key):
             db_client = create_db_client(caller_info="AuthenticateAPIResource.post")
             with db_client.context():
                 merchant_acct = MerchantAcct.fetch(acct_id)
             
                 if merchant_acct:
                     if api_key == merchant_acct.api_key:
                         merchant_user               = MerchantUser.get_by_username(username)
-                        (expiry_datetime, token)    = self.generate_token(acct_id, username)
-                        #session['auth_username']    = username
-                        #session['acct_id']          = acct_id
                         
-                        logger.debug('token=%s', token)
-                        logger.debug('expiry_datetime=%s', expiry_datetime)
-                        logger.debug('auth_username=%s', username)
-            
-                        output_json =  {
-                                        'auth_token'        : token,
-                                        'expires_in'        : int(api_conf.API_TOKEN_EXPIRY_LENGTH_IN_MINUTE) * 60,
-                                        #'expiry_datetime'   : expiry_datetime.strftime('%d-%m-%Y %h:%M:$S'),
-                                        'granted_outlet'    : merchant_user.granted_outlet_details_list,
-                                        'username'          : merchant_user.username,
-                                        'name'              : merchant_user.name,
-                                        'is_admin'          : merchant_user.is_admin,
-                                        'granted_access'    : merchant_user.permission.get('granted_access'),
-                                        'gravatar_url'      : merchant_user.gravatar_url,
-                                        }
-            
-                        logger.debug('output_json=%s', output_json)
+                        is_authorized = self.is_outlet_authorized(merchant_user, outlet_key)
+                        logger.debug('outlet is_authorized=%s', is_authorized)
                         
-                        is_authenticated = True
+                        if is_authorized:
+                            (expiry_datetime, token)    = self.generate_token(acct_id, username)
+                            #session['auth_username']    = username
+                            #session['acct_id']          = acct_id
+                            
+                            logger.debug('token=%s', token)
+                            logger.debug('expiry_datetime=%s', expiry_datetime)
+                            logger.debug('auth_username=%s', username)
+                
+                            output_json =  {
+                                            'auth_token'        : token,
+                                            'expires_in'        : int(api_conf.API_TOKEN_EXPIRY_LENGTH_IN_MINUTE) * 60,
+                                            #'expiry_datetime'   : expiry_datetime.strftime('%d-%m-%Y %h:%M:$S'),
+                                            'granted_outlet'    : merchant_user.granted_outlet_details_list,
+                                            'username'          : merchant_user.username,
+                                            'name'              : merchant_user.name,
+                                            'is_admin'          : merchant_user.is_admin,
+                                            'granted_access'    : merchant_user.permission.get('granted_access'),
+                                            'gravatar_url'      : merchant_user.gravatar_url,
+                                            }
+                
+                            logger.debug('output_json=%s', output_json)
+                            
+                            is_authenticated = True
                     
             if is_authenticated:
                 return output_json
+            elif is_authorized==False:
+                abort(400, msg=["User is not authorized due to outlet is not granted"])
                     
-        abort(401)
-        
+        abort(400, msg=["Failed to authenticate"])
         
+    
+    def is_outlet_authorized(self, merchant_user, outlet_key):
+        return True    
 
+class ProgramDeviceAuthenticate(AuthenticateAPIResource):
+    def is_outlet_authorized(self, merchant_user, outlet_key):
+        if merchant_user.is_admin:
+            return True
+        else:
+            data_in_json        = request.get_json()
+            activation_code     = data_in_json.get('activation_code')
+            device_setting      = LoyaltyDeviceSetting.get_by_activation_code(activation_code)
+            assigned_outlet_key = device_setting.assigned_outlet_key
+            
+            logger.debug('device assigned outlet name=%s', device_setting.assigned_outlet_entity.name)
+            
+            if outlet_key == device_setting.assigned_outlet_key:
+                logger.debug('login outlet is same as device setting assigned outlet')
+                if outlet_key in merchant_user.granted_outlet:
+                    logger.debug('login outlet is authorized by login merchant user granted outlet')
+                    if assigned_outlet_key in merchant_user.granted_outlet:
+                        logger.debug('device assigned outlet is authorized by login merchant user granted outlet')
+                        return True
+                    else:
+                        logger.debug('device setting assigned outlet is not granted outlet')
+                else:
+                    logger.debug('login outlet is not granted outlet')    
+            else:
+                logger.debug('login outlet is not same as device setting assigned outlet')
+                        
+        return False
+            
+class POSDeviceAuthenticate(AuthenticateAPIResource):
+    def is_outlet_authorized(self, merchant_user, outlet_key):
+        if merchant_user.is_admin:
+            return True
+        else:
+            data_in_json        = request.get_json()
+            activation_code     = data_in_json.get('activation_code')
+            device_setting      = POSSetting.get_by_activation_code(activation_code)
+            assigned_outlet_key = device_setting.assigned_outlet_key
+            
+            logger.debug('device assigned outlet name=%s', device_setting.assigned_outlet_entity.name)
+            
+            if outlet_key == device_setting.assigned_outlet_key:
+                logger.debug('login outlet is same as device setting assigned outlet')
+                if outlet_key in merchant_user.granted_outlet:
+                    logger.debug('login outlet is authorized by login merchant user granted outlet')
+                    if assigned_outlet_key in merchant_user.granted_outlet:
+                        logger.debug('device assigned outlet is authorized by login merchant user granted outlet')
+                        return True
+                    else:
+                        logger.debug('device setting assigned outlet is not granted outlet')
+                else:
+                    logger.debug('login outlet is not granted outlet')    
+            else:
+                logger.debug('login outlet is not same as device setting assigned outlet')
+        
+        return False            
 
 class SecureAPIResource(AuthenticateAPIResource):  
     
     def __init__(self):
         super(SecureAPIResource, self).__init__()  
     
     
@@ -202,13 +271,15 @@
         return 'Ping'             
     
      
 api.add_resource(APIResource,                   '/')
 api.add_resource(APIVersionResource,            '/version')
 api.add_resource(CheckAuthTokenResource,        '/auth-check')
 
-merchant_api.add_resource(AuthenticateAPIResource,       '/auth')    
+merchant_api.add_resource(AuthenticateAPIResource,       '/auth')
+merchant_api.add_resource(ProgramDeviceAuthenticate,       '/program-auth')
+merchant_api.add_resource(POSDeviceAuthenticate,       '/pos-auth')
```

### Comparing `trex-apis-1.0.0/trexapi/controllers/app_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/app_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/customer_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/customer_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -555,14 +555,15 @@
         
         if customer:
             dict_properties  = ['transaction_id', 'invoice_id', 'remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
                                'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 
                                #'transact_outlet_details', 
                                'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime',
                                'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
+                               'is_membership_purchase', 'purchased_merchant_membership_key', 'is_membership_renew',
                                ]
             with db_client.context():
                 result       = CustomerTransaction.list_customer_transaction(customer, limit=limit_int)
                 for r in result:
                     transactions_list.append(r.to_dict(dict_properties=dict_properties,  date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S"))
             
             return jsonify(transactions_list)
```

### Comparing `trex-apis-1.0.0/trexapi/controllers/customer_membership_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/customer_membership_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/customer_reward_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/customer_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/loyalty_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/loyalty_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/outlet_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/outlet_api_routes.py`

 * *Files 7% similar despite different names*

```diff
@@ -106,14 +106,15 @@
         
     
     if outlet:
         dict_properties  = ['transaction_id', 'invoice_id', 'remarks', 'tax_amount', 'transact_amount', 'reward_giveaway_method',
                            'entitled_reward_summary', 'entitled_voucher_summary', 'entitled_prepaid_summary', 'transact_customer_acct',
                            'transact_datetime', 'created_datetime',  'transact_outlet_key', 'is_revert', 'reverted_datetime',
                            'transact_by_username', 'is_reward_redeemed', 'is_sales_transaction', 'allow_to_revert',
+                           'is_membership_purchase', 'purchased_merchant_membership_key', 'is_membership_renew',
                            ]
         with db_client.context():
             result       = CustomerTransaction.list_outlet_transaction(outlet, limit=limit_int)
             for r in result:
                 transactions_list.append(r.to_dict(dict_properties=dict_properties,  date_format="%d-%m-%Y", datetime_format="%d-%m-%Y %H:%M:%S"))
         
         return jsonify(transactions_list)
@@ -168,15 +169,16 @@
             if customer_transactionn.transact_outlet_key == outlet_key:
                 with db_client.context():
                     merchant_username       = get_logged_in_api_username()
                     reverted_by             = MerchantUser.get_by_username(merchant_username)
                     reverted_datetime_utc   = datetime.utcnow()
                     __revert_customer_transaction(customer_transactionn, reverted_by, reverted_datetime=reverted_datetime_utc)
                 
-                return create_rest_message(status_code=StatusCode.OK, reverted_datetime = customer_transactionn.reverted_datetime.strftime('%d-%m-%Y %H:%M:%S'))
+                return create_rest_message(status_code=StatusCode.OK, reverted_datetime = datetime.now().strftime('%d-%m-%Y %H:%M:%S'))
+                #return create_rest_message(status_code=StatusCode.OK)
             else:
                 return create_rest_message(gettext('Not allow to revert from different outlet'), status_code=StatusCode.BAD_REQUEST)
         else:    
             return create_rest_message(gettext('Failed to find redemption'), status_code=StatusCode.BAD_REQUEST)
```

### Comparing `trex-apis-1.0.0/trexapi/controllers/payment_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/payment_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/pos_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/pos_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/reward_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/reward_api_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from trexadmin.libs.http import StatusCode
 from trexmodel.models.datastore.merchant_models import Outlet,\
     MerchantAcct, MerchantUser
 from trexapi.forms.reward_api_forms import GiveRewardTransactionForm, RedeemRewardTransactionForm,\
     PrepaidTopupForm, PrepaidRedeemForm, PointRedeemForm
 from werkzeug.datastructures import ImmutableMultiDict
 from trexmodel.models.datastore.transaction_models import CustomerTransaction
-from trexapi.utils.reward_transaction_helper import create_sales_transaction,\
+from trexapi.utils.reward_transaction_helper import create_reward_transaction,\
     redeem_reward_transaction, create_topup_prepaid_transaction
 from trexapi.utils.api_helpers import get_logged_in_api_username
 from trexmodel.models.datastore.voucher_models import MerchantVoucher
 from trexapi import conf
 from trexmodel.models.datastore.prepaid_models import PrepaidSettings
 from trexadmin.libs.jinja.common_filters import format_currency_with_currency_label_filter
 from trexadmin.libs.flask.utils.flask_helper import get_merchant_configured_currency_details
@@ -124,15 +124,15 @@
              
             logger.debug('sales_amount=%s', sales_amount)
             logger.debug('tax_amount=%s', tax_amount)
             logger.debug('invoice_id=%s', invoice_id)
             logger.debug('remarks=%s', remarks)
             logger.debug('invoice_details=%s', invoice_details)
             
-            db_client = create_db_client(caller_info="givea_reward")
+            db_client = create_db_client(caller_info="give_reward")
             
             check_transaction_by_invoice_id = None
             
             if is_not_empty(invoice_id):
                 with db_client.context():
                     check_transaction_by_invoice_id = CustomerTransaction.get_by_invoice_id(invoice_id)
             
@@ -161,15 +161,15 @@
                             
                             
                             
                             transact_merchant_user = MerchantUser.get_by_username(merchant_username)
                             
                             logger.debug('going to call give_reward_transaction')
                             
-                            customer_transaction = create_sales_transaction(customer, 
+                            customer_transaction = create_reward_transaction(customer, 
                                                                             transact_outlet     = transact_outlet, 
                                                                             sales_amount        = sales_amount,
                                                                             tax_amount          = tax_amount,
                                                                             invoice_id          = invoice_id,
                                                                             remarks             = remarks,
                                                                             transact_by         = transact_merchant_user,
                                                                             transact_datetime   = transact_datetime,
```

### Comparing `trex-apis-1.0.0/trexapi/controllers/user_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/user_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/user_reward_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/user_reward_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/controllers/voucher_api_routes.py` & `trex-apis-1.0.1/trexapi/controllers/voucher_api_routes.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/decorators/api_decorators.py` & `trex-apis-1.0.1/trexapi/decorators/api_decorators.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/forms/customer_api_forms.py` & `trex-apis-1.0.1/trexapi/forms/customer_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/forms/reward_api_forms.py` & `trex-apis-1.0.1/trexapi/forms/reward_api_forms.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 '''
 
 from wtforms import StringField, DecimalField, validators
 from trexadmin.forms.base_forms import ValidationBaseForm
 from trexadmin.libs.wtforms import validators as custom_validator
 from trexadmin.libs.wtforms.fields import OptionalDateTimeField, CurrencyField, JSONField
 from flask_babel import gettext
+from trexapi.forms.sales_api_forms import SalesTransactionForm
 
-class GiveRewardTransactionForm(ValidationBaseForm):
+class GiveRewardTransactionForm(SalesTransactionForm):
     sales_amount                    = DecimalField('Sales Amount',[
                                                 validators.InputRequired(message="Sales Amount is required"),
                                             ])
     
     tax_amount                      = DecimalField('Tax Amount',[
                                                 validators.Optional()
                                             ])
```

### Comparing `trex-apis-1.0.0/trexapi/forms/user_api_forms.py` & `trex-apis-1.0.1/trexapi/forms/user_api_forms.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/libs/flask_auth_wrapper.py` & `trex-apis-1.0.1/trexapi/libs/flask_auth_wrapper.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/utils/api_helpers.py` & `trex-apis-1.0.1/trexapi/utils/api_helpers.py`

 * *Files identical despite different names*

### Comparing `trex-apis-1.0.0/trexapi/utils/reward_transaction_helper.py` & `trex-apis-1.0.1/trexapi/utils/reward_transaction_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,38 +21,70 @@
     update_prepaid_summary_with_reverted_prepaid,\
     update_reward_summary_with_reverted_reward
 from trexanalytics.bigquery_upstream_data_config import create_merchant_customer_reward_reverted_upstream_for_merchant,\
     create_merchant_customer_transaction_upstream_for_merchant,\
     create_merchant_customer_redemption_upstream_for_merchant,\
     create_merchant_customer_prepaid_upstream_for_merchant,\
     create_merchant_customer_prepaid_reverted_upstream_for_merchant,\
-    create_merchant_customer_redemption_reverted_upstream_for_merchant
+    create_merchant_customer_redemption_reverted_upstream_for_merchant,\
+    create_merchant_sales_transaction_upstream_for_merchant
 from trexmodel.models.datastore.membership_models import MerchantTierMembership
-from trexmodel.models.datastore.transaction_models import CustomerTransaction
+from trexmodel.models.datastore.transaction_models import CustomerTransaction,\
+    SalesTransaction
 from trexmodel.models.datastore.model_decorators import model_transactional
 from trexmodel.models.datastore.prepaid_models import CustomerPrepaidReward
 from trexadmin.libs.app.reward_program.reward_program_base import EntitledVoucherSummary
 from trexmodel.models.datastore.customer_models import Customer,\
     CustomerMembership, CustomerTierMembership
 from trexmodel.models.datastore.redeem_models import CustomerRedemption
 from trexlib.utils.string_util import is_not_empty
 from trexlib.utils.log_util import get_tracelog
 
 logger = logging.getLogger('debug')
 #logger = logging.getLogger('debug')
 
 
-def create_sales_transaction(customer, transact_outlet=None, sales_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
+def create_sales_transaction(transact_outlet=None, sales_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
                             transact_by=None, transact_datetime=None, invoice_details=None):
     
     logger.debug('---create_sales_transaction---')
     
     logger.debug('invoice_details=%s', invoice_details)
     
     @model_transactional(desc='create_sales_transaction')
+    def __start_transaction_for_customer_transaction(): 
+        sales_transaction = SalesTransaction.create(
+                                       transact_outlet      = transact_outlet,
+                                       
+                                       transact_amount      = sales_amount, 
+                                       tax_amount           = tax_amount,
+                                       
+                                       invoice_id           = invoice_id, 
+                                       remarks              = remarks,
+                                       
+                                       transact_by          = transact_by,
+                                       
+                                       transact_datetime    = transact_datetime,
+                                       
+                                       )
+            
+        create_merchant_sales_transaction_upstream_for_merchant(sales_transaction, streamed_datetime=transact_datetime)
+        
+        return sales_transaction
+        
+    return __start_transaction_for_customer_transaction()
+
+def create_reward_transaction(customer, transact_outlet=None, sales_amount=.0, tax_amount=.0, invoice_id=None, remarks=None, 
+                            transact_by=None, transact_datetime=None, invoice_details=None):
+    
+    logger.debug('---create_reward_transaction---')
+    
+    logger.debug('invoice_details=%s', invoice_details)
+    
+    @model_transactional(desc='create_reward_transaction')
     def __start_transaction_for_customer_transaction():
         customer_transaction = CustomerTransaction.create_system_transaction(
                                        customer, 
                                        transact_outlet      = transact_outlet,
                                        
                                        transact_amount      = sales_amount, 
                                        tax_amount           = tax_amount,
@@ -77,15 +109,15 @@
         
         return customer_transaction
         
     return __start_transaction_for_customer_transaction()
 
 def create_non_sales_system_transaction(customer, transact_datetime=None, remarks=None, system_remarks=None):
     
-    logger.debug('---create_sales_transaction---')
+    logger.debug('---create_non_sales_system_transaction---')
     
     #@model_transactional(desc='create_non_sales_system_transaction')
     def __start_transaction_for_customer_transaction():
         customer_transaction = CustomerTransaction.create_system_transaction(
                                        customer, 
                                        transact_datetime    = transact_datetime,
                                        allow_to_revert      = False,
@@ -610,21 +642,27 @@
 def revert_transaction(transaction_details, reverted_by, reverted_datetime=None, create_upstream=True):
     merchant_acct                       = transaction_details.transact_merchant_acct
     transaction_id                      = transaction_details.transaction_id
     customer_acct                       = transaction_details.transact_customer_acct
         
     if transaction_details.is_membership_purchase:
         #remove membership
-        purchased_customer_membership   = transaction_details.purchased_customer_membership_entity
-        try:
-            merchant_membership_key         = purchased_customer_membership.merchant_membership_key 
-            purchased_customer_membership.delete()
-        except:
-            logger.error('Failed due to %s', get_tracelog())
         
+        merchant_membership_key         = transaction_details.purchased_merchant_membership_key
+        merchant_membership             = transaction_details.purchased_merchant_membership_entity
+        purchased_customer_membership   = CustomerMembership.get_by_customer_and_merchant_membership(customer_acct, merchant_membership)
+        if purchased_customer_membership:
+            try:
+                 
+                purchased_customer_membership.delete()
+            except:
+                logger.error('Failed due to %s', get_tracelog())
+        
+        else:
+            logger.warn('Customer membership is not found')
         
         if is_not_empty(customer_acct.memberships_list):
             customer_acct.memberships_list.remove(merchant_membership_key)
         
         customer_acct.put()
         
         return True
```

