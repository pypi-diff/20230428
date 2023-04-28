# Comparing `tmp/tencentcloud-sdk-python-kms-3.0.883.tar.gz` & `tmp/tencentcloud-sdk-python-kms-3.0.884.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.883.tar", last modified: Thu Apr 27 00:36:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.884.tar", last modified: Fri Apr 28 02:26:17 2023, max compression
```

## Comparing `tencentcloud-sdk-python-kms-3.0.883.tar` & `tencentcloud-sdk-python-kms-3.0.884.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/
--rw-r--r--   0 root         (0) root         (0)    46847 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/kms_client.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96860 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-27 00:36:14.000000 tencentcloud-sdk-python-kms-3.0.883/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/
+-rw-r--r--   0 root         (0) root         (0)    50843 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/kms_client.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104577 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-28 02:26:16.000000 tencentcloud-sdk-python-kms-3.0.884/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-28 02:26:17.000000 tencentcloud-sdk-python-kms-3.0.884/setup.cfg
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/README.rst` & `tencentcloud-sdk-python-kms-3.0.884/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/kms_client.py` & `tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/kms_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -989,14 +989,106 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def PostQuantumCryptoDecrypt(self, request):
+        """本接口使用后量子密码算法密钥，解密密文，并得到明文数据。
+
+        :param request: Request instance for PostQuantumCryptoDecrypt.
+        :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoDecryptRequest`
+        :rtype: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoDecryptResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("PostQuantumCryptoDecrypt", params, headers=headers)
+            response = json.loads(body)
+            model = models.PostQuantumCryptoDecryptResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def PostQuantumCryptoEncrypt(self, request):
+        """本接口使用后量子密码算法密钥，可加密最多为4KB任意数据，可用于加密数据库密码，RSA Key，或其它较小的敏感信息。对于应用的数据加密，使用GenerateDataKey生成的DataKey进行本地数据的加解密操作。
+
+        :param request: Request instance for PostQuantumCryptoEncrypt.
+        :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoEncryptRequest`
+        :rtype: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoEncryptResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("PostQuantumCryptoEncrypt", params, headers=headers)
+            response = json.loads(body)
+            model = models.PostQuantumCryptoEncryptResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def PostQuantumCryptoSign(self, request):
+        """使用后量子密码算法签名验签密钥进行签名。
+
+        :param request: Request instance for PostQuantumCryptoSign.
+        :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoSignRequest`
+        :rtype: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoSignResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("PostQuantumCryptoSign", params, headers=headers)
+            response = json.loads(body)
+            model = models.PostQuantumCryptoSignResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def PostQuantumCryptoVerify(self, request):
+        """使用后量子密码算法密钥对签名进行验证。
+
+        :param request: Request instance for PostQuantumCryptoVerify.
+        :type request: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoVerifyRequest`
+        :rtype: :class:`tencentcloud.kms.v20190118.models.PostQuantumCryptoVerifyResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("PostQuantumCryptoVerify", params, headers=headers)
+            response = json.loads(body)
+            model = models.PostQuantumCryptoVerifyResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ReEncrypt(self, request):
         """使用指定CMK对密文重新加密。
 
         :param request: Request instance for ReEncrypt.
         :type request: :class:`tencentcloud.kms.v20190118.models.ReEncryptRequest`
         :rtype: :class:`tencentcloud.kms.v20190118.models.ReEncryptResponse`
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/errorcodes.py` & `tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.883/tencentcloud/kms/v20190118/models.py` & `tencentcloud-sdk-python-kms-3.0.884/tencentcloud/kms/v20190118/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2359,14 +2359,227 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
+class PostQuantumCryptoDecryptRequest(AbstractModel):
+    """PostQuantumCryptoDecrypt请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CiphertextBlob: 待解密的密文数据
+        :type CiphertextBlob: str
+        :param EncryptionPublicKey: PEM 格式公钥字符串，支持 RSA2048 和 SM2 公钥，用于对返回数据中的 Plaintext 值进行加密。若为空，则不对 Plaintext 值加密。
+        :type EncryptionPublicKey: str
+        :param EncryptionAlgorithm: 非对称加密算法，配合 EncryptionPublicKey 对返回数据进行加密。目前支持：SM2（以 C1C3C2 格式返回密文），SM2_C1C3C2_ASN1 （以 C1C3C2 ASN1 格式返回密文），RSAES_PKCS1_V1_5，RSAES_OAEP_SHA_1，RSAES_OAEP_SHA_256。若为空，则默认为 SM2。
+        :type EncryptionAlgorithm: str
+        """
+        self.CiphertextBlob = None
+        self.EncryptionPublicKey = None
+        self.EncryptionAlgorithm = None
+
+
+    def _deserialize(self, params):
+        self.CiphertextBlob = params.get("CiphertextBlob")
+        self.EncryptionPublicKey = params.get("EncryptionPublicKey")
+        self.EncryptionAlgorithm = params.get("EncryptionAlgorithm")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PostQuantumCryptoDecryptResponse(AbstractModel):
+    """PostQuantumCryptoDecrypt返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param KeyId: CMK的全局唯一标识
+        :type KeyId: str
+        :param PlainText: 若调用时未提供 EncryptionPublicKey，该字段值为 Base64 编码的明文，需进行 Base64 解码以获取明文。
+若调用时提供了 EncryptionPublicKey，则该字段值为使用 EncryptionPublicKey 公钥进行非对称加密后的 Base64 编码的密文。需在 Base64 解码后，使用用户上传的公钥对应的私钥进行进一步解密，以获取明文。
+        :type PlainText: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.KeyId = None
+        self.PlainText = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.KeyId = params.get("KeyId")
+        self.PlainText = params.get("PlainText")
+        self.RequestId = params.get("RequestId")
+
+
+class PostQuantumCryptoEncryptRequest(AbstractModel):
+    """PostQuantumCryptoEncrypt请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param KeyId: 调用CreateKey生成的CMK全局唯一标识符
+        :type KeyId: str
+        :param PlainText: 被加密的明文数据，该字段必须使用base64编码，原文最大长度支持4K
+        :type PlainText: str
+        """
+        self.KeyId = None
+        self.PlainText = None
+
+
+    def _deserialize(self, params):
+        self.KeyId = params.get("KeyId")
+        self.PlainText = params.get("PlainText")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PostQuantumCryptoEncryptResponse(AbstractModel):
+    """PostQuantumCryptoEncrypt返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param CiphertextBlob: 加密后的密文，base64编码。注意：本字段中打包了密文和密钥的相关信息，不是对明文的直接加密结果，只有将该字段作为PostQuantumCryptoDecrypt接口的输入参数，才可以解密出原文。
+        :type CiphertextBlob: str
+        :param KeyId: 加密使用的CMK的全局唯一标识
+        :type KeyId: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.CiphertextBlob = None
+        self.KeyId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.CiphertextBlob = params.get("CiphertextBlob")
+        self.KeyId = params.get("KeyId")
+        self.RequestId = params.get("RequestId")
+
+
+class PostQuantumCryptoSignRequest(AbstractModel):
+    """PostQuantumCryptoSign请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Message: Base64 编码的消息原文。消息原文的长度（Base64编码前的长度）不超过4096字节。
+        :type Message: str
+        :param KeyId: 密钥的唯一标识
+        :type KeyId: str
+        """
+        self.Message = None
+        self.KeyId = None
+
+
+    def _deserialize(self, params):
+        self.Message = params.get("Message")
+        self.KeyId = params.get("KeyId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PostQuantumCryptoSignResponse(AbstractModel):
+    """PostQuantumCryptoSign返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Signature: 签名值，Base64编码。可使用 PostQuantumCryptoVerify接口对签名值进行验证。
+        :type Signature: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Signature = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Signature = params.get("Signature")
+        self.RequestId = params.get("RequestId")
+
+
+class PostQuantumCryptoVerifyRequest(AbstractModel):
+    """PostQuantumCryptoVerify请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param KeyId: 密钥的唯一标识
+        :type KeyId: str
+        :param SignatureValue: 签名值，通过调用KMS PostQuantumCryptoSign签名接口生成
+        :type SignatureValue: str
+        :param Message: Base64 编码的消息原文，消息原文的长度（Base64编码前的长度）不超过4096字节。
+        :type Message: str
+        """
+        self.KeyId = None
+        self.SignatureValue = None
+        self.Message = None
+
+
+    def _deserialize(self, params):
+        self.KeyId = params.get("KeyId")
+        self.SignatureValue = params.get("SignatureValue")
+        self.Message = params.get("Message")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class PostQuantumCryptoVerifyResponse(AbstractModel):
+    """PostQuantumCryptoVerify返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SignatureValid: 签名是否有效。true：签名有效，false：签名无效。
+        :type SignatureValid: bool
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.SignatureValid = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.SignatureValid = params.get("SignatureValid")
+        self.RequestId = params.get("RequestId")
+
+
 class ReEncryptRequest(AbstractModel):
     """ReEncrypt请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/tencentcloud/__init__.py` & `tencentcloud-sdk-python-kms-3.0.884/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.883'
+__version__ = '3.0.884'
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/tencentcloud_sdk_python_kms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.884/tencentcloud_sdk_python_kms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.884/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.883
+Version: 3.0.884
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.883/setup.py` & `tencentcloud-sdk-python-kms-3.0.884/setup.py`

 * *Files identical despite different names*

