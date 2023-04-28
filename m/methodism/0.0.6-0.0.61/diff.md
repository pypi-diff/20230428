# Comparing `tmp/methodism-0.0.6.tar.gz` & `tmp/methodism-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.0.6.tar", last modified: Thu Apr 27 12:27:02 2023, max compression
+gzip compressed data, was "methodism-0.0.61.tar", last modified: Fri Apr 28 10:29:21 2023, max compression
```

## Comparing `methodism-0.0.6.tar` & `methodism-0.0.61.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 12:27:02.975041 methodism-0.0.6/
--rw-rw-rw-   0        0        0     2881 2023-04-27 12:27:02.975041 methodism-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2399 2023-04-27 08:27:37.000000 methodism-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 12:27:02.957406 methodism-0.0.6/base/
--rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.6/base/__init__.py
--rw-rw-rw-   0        0        0     3559 2023-04-27 07:18:17.000000 methodism-0.0.6/base/costumizing.py
--rw-rw-rw-   0        0        0      708 2023-04-26 06:02:02.000000 methodism-0.0.6/base/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.6/base/error_messages.py
--rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.6/base/helper.py
--rw-rw-rw-   0        0        0     3449 2023-04-27 12:26:20.000000 methodism-0.0.6/base/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 12:27:02.975041 methodism-0.0.6/methodism.egg-info/
--rw-rw-rw-   0        0        0     2881 2023-04-27 12:27:02.000000 methodism-0.0.6/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-27 12:27:02.000000 methodism-0.0.6/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 12:27:02.000000 methodism-0.0.6/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-04-27 12:27:02.000000 methodism-0.0.6/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-04-27 12:26:29.000000 methodism-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-04-27 12:27:02.975041 methodism-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.338079 methodism-0.0.61/
+-rw-rw-rw-   0        0        0     2917 2023-04-28 10:29:21.338079 methodism-0.0.61/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-04-28 10:28:06.000000 methodism-0.0.61/README.md
+drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.306810 methodism-0.0.61/methodism/
+-rw-rw-rw-   0        0        0        0 2023-04-26 06:59:17.000000 methodism-0.0.61/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      718 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.0.61/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     1239 2023-04-26 05:50:16.000000 methodism-0.0.61/methodism/helper.py
+-rw-rw-rw-   0        0        0     3294 2023-04-28 10:28:06.000000 methodism-0.0.61/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-04-28 10:29:21.322436 methodism-0.0.61/methodism.egg-info/
+-rw-rw-rw-   0        0        0     2917 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-28 10:29:21.000000 methodism-0.0.61/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      604 2023-04-28 10:28:51.000000 methodism-0.0.61/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-04-28 10:29:21.338079 methodism-0.0.61/setup.cfg
```

### Comparing `methodism-0.0.6/PKG-INFO` & `methodism-0.0.61/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.6
+Version: 0.0.61
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,19 @@
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
 ### filelar
-* ``base/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
-* ``base/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
-* ``base/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
-* ``base/helper.py`` Yordamchi funksiyalar joylangan file.   
-* ``base/main.py`` Asosiy class yozilgan file
+* ``methodism/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
+* ``methodism/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
+* ``methodism/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
+* ``methodism/helper.py`` Yordamchi funksiyalar joylangan file.   
+* ``methodism/main.py`` Asosiy class yozilgan file
 
 
 
 ## Ishlatish ketma ketligi
 
 #### Birinchi navbatda kerakli kutubxonalarni o'rnatib olishingiz kerak
 #### From GitHub
@@ -42,20 +42,20 @@
 ```  
 #### From PyPi
 ``` python
   pip install Django==4.2 django-rest-framework==0.1.0 djangorestframework==3.14.0
 ```  
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
-class ga esa `base/main.py` dagi `METHODIZM` classidan vorislik bering.  
+class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from base.main import METHODIZM
+from methodism.main import METHODIZM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
 class YourClass(METHODIZM):
```

### Comparing `methodism-0.0.6/README.md` & `methodism-0.0.61/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
 ### filelar
-* ``base/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
-* ``base/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
-* ``base/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
-* ``base/helper.py`` Yordamchi funksiyalar joylangan file.   
-* ``base/main.py`` Asosiy class yozilgan file
+* ``methodism/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
+* ``methodism/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
+* ``methodism/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
+* ``methodism/helper.py`` Yordamchi funksiyalar joylangan file.   
+* ``methodism/main.py`` Asosiy class yozilgan file
 
 
 
 ## Ishlatish ketma ketligi
 
 #### Birinchi navbatda kerakli kutubxonalarni o'rnatib olishingiz kerak
 #### From GitHub
@@ -28,20 +28,20 @@
 ```  
 #### From PyPi
 ``` python
   pip install Django==4.2 django-rest-framework==0.1.0 djangorestframework==3.14.0
 ```  
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
-class ga esa `base/main.py` dagi `METHODIZM` classidan vorislik bering.  
+class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from base.main import METHODIZM
+from methodism.main import METHODIZM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
 class YourClass(METHODIZM):
```

### Comparing `methodism-0.0.6/base/costumizing.py` & `methodism-0.0.61/methodism/costumizing.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,84 +4,85 @@
 #
 #  Tashkent, Uzbekistan
 
 
 from django.contrib.auth import get_user_model, authenticate
 from rest_framework.authentication import TokenAuthentication, get_authorization_header, BasicAuthentication
 from rest_framework.generics import GenericAPIView
-
-from base.error_messages import MESSAGE
 from rest_framework import exceptions
+
+from methodism.helper import custom_response
+from methodism.error_messages import MESSAGE
 import base64, binascii
 
 
 # Custom Holatdagi bazi classlar sizga ishlashganda optimallik uchun xizmat qiladi
 class CustomBasicAuthentication(BasicAuthentication):
     def authenticate(self, request):
         auth = get_authorization_header(request).split()
 
         if not auth or auth[0].lower() != b'basic':
             return None
 
         if len(auth) == 1:
-            msg = self.response_funk(False, message=MESSAGE['InvalidBasicHeader1'])
+            msg = custom_response(False, message=MESSAGE['InvalidBasicHeader1'])
             raise exceptions.AuthenticationFailed(msg)
         elif len(auth) > 2:
-            msg = self.response_funk(False, message=MESSAGE['InvalidBasicHeader2'])
+            msg = custom_response(False, message=MESSAGE['InvalidBasicHeader2'])
             raise exceptions.AuthenticationFailed(msg)
 
         try:
             try:
                 auth_decoded = base64.b64decode(auth[1]).decode('utf-8')
             except UnicodeDecodeError:
                 auth_decoded = base64.b64decode(auth[1]).decode('latin-1')
             auth_parts = auth_decoded.partition(':')
         except (TypeError, UnicodeDecodeError, binascii.Error):
-            msg = self.response_funk(False, message=MESSAGE['InvalidBasicHeader3'])
+            msg = custom_response(False, message=MESSAGE['InvalidBasicHeader3'])
             raise exceptions.AuthenticationFailed(msg)
 
         userid, password = auth_parts[0], auth_parts[2]
         return self.authenticate_credentials(userid, password, request)
 
     def authenticate_credentials(self, userid, password, request=None):
         credentials = {
             get_user_model().USERNAME_FIELD: userid,
             'password': password
         }
         user = authenticate(request=request, **credentials)
 
         if user is None:
-            raise exceptions.AuthenticationFailed(self.response_funk(False, message=MESSAGE['UserPasswordError']))
+            raise exceptions.AuthenticationFailed(custom_response(False, message=MESSAGE['UserPasswordError']))
 
         if not user.is_active:
-            raise exceptions.AuthenticationFailed(self.response_funk(False, message=MESSAGE['UserDeleted']))
+            raise exceptions.AuthenticationFailed(custom_response(False, message=MESSAGE['UserDeleted']))
 
         return (user, None)
 
     def authenticate_header(self, request):
         return 'Basic realm="%s"' % self.www_authenticate_realm
 
 
 class CustomGenericAPIView(GenericAPIView):
     def permission_denied(self, request, message=None, code=None):
         if request.authenticators and not request.successful_authenticator:
-            raise exceptions.NotAuthenticated(self.response_funk(False, message=MESSAGE['NotAuthenticated']))
+            raise exceptions.NotAuthenticated(custom_response(False, message=MESSAGE['NotAuthenticated']))
         raise exceptions.PermissionDenied(detail=MESSAGE['PermissionDenied'], code=code)
 
 
 class BearerAuth(TokenAuthentication):
     keyword = 'Bearer'
 
     def authenticate_credentials(self, key):
         model = self.get_model()
         try:
             token = model.objects.select_related('user').get(key=key)
         except model.DoesNotExist:
-            raise exceptions.AuthenticationFailed(self.response_funk(False, message=MESSAGE['Unauthenticated']))
+            raise exceptions.AuthenticationFailed(custom_response(False, message=MESSAGE['Unauthenticated']))
 
         if not token.user.is_active:
-            raise exceptions.AuthenticationFailed(self.response_funk(False, message=MESSAGE['UserNot']))
+            raise exceptions.AuthenticationFailed(custom_response(False, message=MESSAGE['UserNot']))
 
         if token.user.deleted:
-            raise exceptions.AuthenticationFailed(self.response_funk(False, message=MESSAGE['UserDeleted']))
+            raise exceptions.AuthenticationFailed(custom_response(False, message=MESSAGE['UserDeleted']))
 
         return super(BearerAuth, self).authenticate_credentials(key)
```

### Comparing `methodism-0.0.6/base/decors.py` & `methodism-0.0.61/methodism/decors.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 #  Please contact before making any changes
 #
 #  Tashkent, Uzbekistan
 
 from rest_framework.response import Response
 
-from base.error_messages import MESSAGE
-from base.helper import custom_response
+from methodism.error_messages import MESSAGE
+from methodism.helper import custom_response
 
 
 # asosiy decorator
 def method_and_params_checker(funk):
     def wrapper(self, req, *args, **kwargs):
         params = req.data.get('params')
         method = req.data.get("method")
```

### Comparing `methodism-0.0.6/base/error_messages.py` & `methodism-0.0.61/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.6/base/helper.py` & `methodism-0.0.61/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.0.6/base/main.py` & `methodism-0.0.61/methodism/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 from rest_framework.authtoken.models import Token
 from rest_framework.response import Response
 from rest_framework.permissions import AllowAny
 
 from re import compile as re_compile
 
-from base.costumizing import CustomGenericAPIView
-from base.decors import method_and_params_checker
-from base.error_messages import MESSAGE
-from base.helper import custom_response, exception_data
+from methodism.costumizing import CustomGenericAPIView
+from methodism.decors import method_and_params_checker
+from methodism.error_messages import MESSAGE
+from methodism.helper import custom_response, exception_data
 
 
 class METHODIZM(CustomGenericAPIView):
     """
                         Main Class | METHODIZM
     file -> Asosiy funksiyalar joylashgan fileni ko'rsating
     token_key -> Token Secret kalitini ko'rsating (default=Bearer)
     auth_headers -> API headersda ushlab olinishi kerak bo'lgan kalitni ko'rsating (default=Authorization)
     token_class -> Ro'yxatdan o'tganligini ko'rsatuvchi classni ko'rsating -> (default=Token)
     not_auth_methods -> Ro'yxatdan o'tish talab qilinmaydigan funksiyalarni ko'rsating | list ko'rinishida
-    response_funk -> Imkon qadar teginilmagan ma'qul!
 
     Bunga qo'shimcha boshqa Custom holardagi avtorizatsiyalardan ham foydalanishingiz mumkin
 
     EXP:
         authentication_classes = CustomBasicAuthentication,
         permission_classes = IsAuthenticated,
 
@@ -36,42 +35,41 @@
     """
 
     file = "__main__"
     token_key = "Bearer"
     auth_headers = 'Authorization'
     token_class = Token
     not_auth_methods = []  # def hello_world() => hello.world
-    response_funk = custom_response  # must be funk(status, data, method ,message) return dict {}
 
     @method_and_params_checker
     def post(self, requests, *args, **kwargs):
         method = requests.data.get("method")
         params = requests.data.get("params")
         headers = requests.headers
         if method not in self.not_auth_methods:
             authorization = headers.get(self.auth_headers, '')
             pattern = re_compile(self.token_key + r" (.+)")
 
             if not pattern.match(authorization):
-                return Response(self.response_funk(status=False, method=method, message=MESSAGE['NotAuthenticated']))
+                return Response(custom_response(status=False, method=method, message=MESSAGE['NotAuthenticated']))
             input_token = pattern.findall(authorization)[0]
 
             # Authorize
             token = self.token_class.objects.filter(key=input_token).first()
             if not token:
-                return Response(self.response_funk(status=False, method=method, message=MESSAGE['AuthToken']))
+                return Response(custom_response(status=False, method=method, message=MESSAGE['AuthToken']))
             requests.user = token.user
         try:
             funk = getattr(self.file, method.replace('.', '_').replace('-', '_'))
         except AttributeError:
-            return Response(self.response_funk(False, method=method, message=MESSAGE['MethodDoesNotExist']))
+            return Response(custom_response(False, method=method, message=MESSAGE['MethodDoesNotExist']))
         except Exception as e:
-            return Response(self.response_funk(False, method=method, message=MESSAGE['UndefinedError'],
-                                               data=exception_data(e)))
+            return Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
+                                            data=exception_data(e)))
         res = map(funk, [requests], [params])
         try:
             response = Response(list(res)[0])
             response.data.update({'method': method})
         except Exception as e:
-            response = Response(self.response_funk(False, method=method, message=MESSAGE['UndefinedError'],
-                                                   data=exception_data(e)))
+            response = Response(custom_response(False, method=method, message=MESSAGE['UndefinedError'],
+                                                data=exception_data(e)))
         return response
```

### Comparing `methodism-0.0.6/methodism.egg-info/PKG-INFO` & `methodism-0.0.61/methodism.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.0.6
+Version: 0.0.61
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -21,19 +21,19 @@
 ```
 ## About
 Ushbu Kutubxona Egamberdiyev Xudoyberdi Tomonidan yaratilgan bo'lib tog'ridan tog'ri django 
 kutubxonasi ustiga qurulgan. Bu sizga API lar yozganda uni tez ishlatish va tezroq API yozish imkoni beradi.
 Avtomatik tarzda siz yozgan funksiyani method ga aylantirgan holatda api hosil qiladi
 
 ### filelar
-* ``base/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
-* ``base/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
-* ``base/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
-* ``base/helper.py`` Yordamchi funksiyalar joylangan file.   
-* ``base/main.py`` Asosiy class yozilgan file
+* ``methodism/costumizing.py``  ushbu file tayyor bir qator claslarni custum holarga o'tqazilgan varianti hisoblandi.  
+* ``methodism/decors.py`` Ushbu file kerakli bo'lgan decoratorlarni yozish uchun ishlatiluvchi file.
+* ``methodism/error_messages.py`` bo'lishi mumkin bo'lgan xatoliklar yig'ilgan lug'at ko'rinishidagi file.   
+* ``methodism/helper.py`` Yordamchi funksiyalar joylangan file.   
+* ``methodism/main.py`` Asosiy class yozilgan file
 
 
 
 ## Ishlatish ketma ketligi
 
 #### Birinchi navbatda kerakli kutubxonalarni o'rnatib olishingiz kerak
 #### From GitHub
@@ -42,20 +42,20 @@
 ```  
 #### From PyPi
 ``` python
   pip install Django==4.2 django-rest-framework==0.1.0 djangorestframework==3.14.0
 ```  
 
 Yuklab olib bo'lgach O'zingizga  `views.py` faylida kerakli bo'lgan classni yozing va uni `urls.py` ga ulang,
-class ga esa `base/main.py` dagi `METHODIZM` classidan vorislik bering.  
+class ga esa `methodism/main.py` dagi `METHODIZM` classidan vorislik bering.  
 ### Example in `views.py`
 
 
 ```python
-from base.main import METHODIZM
+from methodism.main import METHODIZM
 
 # agar bundan foydalansangiz settings.INSTALLED_APPS ga 'rest_framework.authtoken' ni qo'shib qo'ying
 from rest_framework.authtoken.models import Token 
 
 
 class YourClass(METHODIZM):
```

### Comparing `methodism-0.0.6/pyproject.toml` & `methodism-0.0.61/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.0.6"
+version = "0.0.61"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.0.6/setup.cfg` & `methodism-0.0.61/setup.cfg`

 * *Files identical despite different names*

