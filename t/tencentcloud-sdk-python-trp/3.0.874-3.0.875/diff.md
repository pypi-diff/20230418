# Comparing `tmp/tencentcloud-sdk-python-trp-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-trp-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.874.tar", last modified: Mon Apr 17 00:53:02 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-trp-3.0.875.tar", last modified: Tue Apr 18 01:00:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-trp-3.0.874.tar` & `tencentcloud-sdk-python-trp-3.0.875.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   132410 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)    40986 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:53:02.000000 tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139889 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)    43704 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 01:00:45.000000 tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-trp-3.0.874/README.rst` & `tencentcloud-sdk-python-trp-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,63 @@
 # limitations under the License.
 
 import warnings
 
 from tencentcloud.common.abstract_model import AbstractModel
 
 
+class AuthorizedTransferRequest(AbstractModel):
+    """AuthorizedTransfer请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BusinessSecurityData: 业务加密入参。
+        :type BusinessSecurityData: :class:`tencentcloud.trp.v20210515.models.InputEncryptData`
+        """
+        self.BusinessSecurityData = None
+
+
+    def _deserialize(self, params):
+        if params.get("BusinessSecurityData") is not None:
+            self.BusinessSecurityData = InputEncryptData()
+            self.BusinessSecurityData._deserialize(params.get("BusinessSecurityData"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class AuthorizedTransferResponse(AbstractModel):
+    """AuthorizedTransfer返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 业务出参。
+        :type Data: :class:`tencentcloud.trp.v20210515.models.OutputAuthorizedTransfer`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = OutputAuthorizedTransfer()
+            self.Data._deserialize(params.get("Data"))
+        self.RequestId = params.get("RequestId")
+
+
 class ChainData(AbstractModel):
     """上链数据
 
     """
 
     def __init__(self):
         r"""
@@ -2754,20 +2803,112 @@
             for item in params.get("TraceDataList"):
                 obj = TraceData()
                 obj._deserialize(item)
                 self.TraceDataList.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class EffectFeedbackRequest(AbstractModel):
+    """EffectFeedback请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BusinessSecurityData: 业务加密入参。
+        :type BusinessSecurityData: :class:`tencentcloud.trp.v20210515.models.InputEncryptData`
+        """
+        self.BusinessSecurityData = None
+
+
+    def _deserialize(self, params):
+        if params.get("BusinessSecurityData") is not None:
+            self.BusinessSecurityData = InputEncryptData()
+            self.BusinessSecurityData._deserialize(params.get("BusinessSecurityData"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class EffectFeedbackResponse(AbstractModel):
+    """EffectFeedback返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 业务出参。
+        :type Data: :class:`tencentcloud.trp.v20210515.models.OutputAuthorizedTransfer`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = OutputAuthorizedTransfer()
+            self.Data._deserialize(params.get("Data"))
+        self.RequestId = params.get("RequestId")
+
+
 class Ext(AbstractModel):
     """预留字段
 
     """
 
 
+class InputEncryptData(AbstractModel):
+    """业务加密入参
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EncryptMethod: 加密方式，0：AES加密；
+
+        :type EncryptMethod: int
+        :param EncryptMode: 加密算法中的块处理模式，1：CBC模式； 目前只支持CBC模式
+        :type EncryptMode: int
+        :param PaddingType: 填充模式，0：ZeroPadding；1：PKCS5Padding；2：
+PKCS7Padding。
+        :type PaddingType: int
+        :param EncryptData: 加密数据，将AuthorizedData结构体数组（数组最大长度不超过20）序列化成JSON字符串，对得到的字符串加密并填充到该字段。
+        :type EncryptData: str
+        :param IsAuthorized: 用户是否授权，本接口取值：1，已授权。
+
+        :type IsAuthorized: int
+        """
+        self.EncryptMethod = None
+        self.EncryptMode = None
+        self.PaddingType = None
+        self.EncryptData = None
+        self.IsAuthorized = None
+
+
+    def _deserialize(self, params):
+        self.EncryptMethod = params.get("EncryptMethod")
+        self.EncryptMode = params.get("EncryptMode")
+        self.PaddingType = params.get("PaddingType")
+        self.EncryptData = params.get("EncryptData")
+        self.IsAuthorized = params.get("IsAuthorized")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Job(AbstractModel):
     """通用调度任务
 
     """
 
     def __init__(self):
         r"""
@@ -3464,14 +3605,49 @@
 
 
     def _deserialize(self, params):
         self.TraceId = params.get("TraceId")
         self.RequestId = params.get("RequestId")
 
 
+class OutputAuthorizedTransfer(AbstractModel):
+    """业务出参
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Code: 推送状态，0表示成功。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Code: int
+        :param Message: 错误码。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Message: str
+        :param Value: 错误信息描述。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        """
+        self.Code = None
+        self.Message = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Code = params.get("Code")
+        self.Message = params.get("Message")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PackSpec(AbstractModel):
     """层级码配置
 
     """
 
     def __init__(self):
         r"""
@@ -3714,14 +3890,63 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ReportBatchCallbackStatusRequest(AbstractModel):
+    """ReportBatchCallbackStatus请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param BusinessSecurityData: 业务加密入参。
+        :type BusinessSecurityData: :class:`tencentcloud.trp.v20210515.models.InputEncryptData`
+        """
+        self.BusinessSecurityData = None
+
+
+    def _deserialize(self, params):
+        if params.get("BusinessSecurityData") is not None:
+            self.BusinessSecurityData = InputEncryptData()
+            self.BusinessSecurityData._deserialize(params.get("BusinessSecurityData"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ReportBatchCallbackStatusResponse(AbstractModel):
+    """ReportBatchCallbackStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 业务出参。
+        :type Data: :class:`tencentcloud.trp.v20210515.models.OutputAuthorizedTransfer`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self.Data = OutputAuthorizedTransfer()
+            self.Data._deserialize(params.get("Data"))
+        self.RequestId = params.get("RequestId")
+
+
 class ScanLog(AbstractModel):
     """扫码明细
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-trp-3.0.875/tencentcloud/trp/v20210515/trp_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class TrpClient(AbstractClient):
     _apiVersion = '2021-05-15'
     _endpoint = 'trp.tencentcloudapi.com'
     _service = 'trp'
 
 
+    def AuthorizedTransfer(self, request):
+        """接收客户侧的用户已授权的号码。
+
+        :param request: Request instance for AuthorizedTransfer.
+        :type request: :class:`tencentcloud.trp.v20210515.models.AuthorizedTransferRequest`
+        :rtype: :class:`tencentcloud.trp.v20210515.models.AuthorizedTransferResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("AuthorizedTransfer", params, headers=headers)
+            response = json.loads(body)
+            model = models.AuthorizedTransferResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateCodeBatch(self, request):
         """新增批次
 
         :param request: Request instance for CreateCodeBatch.
         :type request: :class:`tencentcloud.trp.v20210515.models.CreateCodeBatchRequest`
         :rtype: :class:`tencentcloud.trp.v20210515.models.CreateCodeBatchResponse`
 
@@ -851,14 +874,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def EffectFeedback(self, request):
+        """接收客户反馈的各环节数据
+
+        :param request: Request instance for EffectFeedback.
+        :type request: :class:`tencentcloud.trp.v20210515.models.EffectFeedbackRequest`
+        :rtype: :class:`tencentcloud.trp.v20210515.models.EffectFeedbackResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("EffectFeedback", params, headers=headers)
+            response = json.loads(body)
+            model = models.EffectFeedbackResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyCodeBatch(self, request):
         """修改批次
 
         :param request: Request instance for ModifyCodeBatch.
         :type request: :class:`tencentcloud.trp.v20210515.models.ModifyCodeBatchRequest`
         :rtype: :class:`tencentcloud.trp.v20210515.models.ModifyCodeBatchResponse`
 
@@ -1056,8 +1102,31 @@
             model = models.ModifyTraceDataRanksResponse()
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def ReportBatchCallbackStatus(self, request):
+        """接收离线筛选包回执，用于效果统计和分析。
+
+        :param request: Request instance for ReportBatchCallbackStatus.
+        :type request: :class:`tencentcloud.trp.v20210515.models.ReportBatchCallbackStatusRequest`
+        :rtype: :class:`tencentcloud.trp.v20210515.models.ReportBatchCallbackStatusResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ReportBatchCallbackStatus", params, headers=headers)
+            response = json.loads(body)
+            model = models.ReportBatchCallbackStatusResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
                 raise TencentCloudSDKException(e.message, e.message)
```

### Comparing `tencentcloud-sdk-python-trp-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-trp-3.0.875/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.874'
+__version__ = '3.0.875'
```

### Comparing `tencentcloud-sdk-python-trp-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.875/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-trp-3.0.874/setup.py` & `tencentcloud-sdk-python-trp-3.0.875/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-trp-3.0.874/tencentcloud_sdk_python_trp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-trp-3.0.875/tencentcloud_sdk_python_trp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-trp
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Trp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

