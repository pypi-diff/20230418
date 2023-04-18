# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.874.tar", last modified: Mon Apr 17 00:29:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.875.tar", last modified: Tue Apr 18 00:38:26 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.874.tar` & `tencentcloud-sdk-python-ess-3.0.875.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    47020 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23577 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   212520 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:29:49.000000 tencentcloud-sdk-python-ess-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    49089 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23577 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   216316 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:38:26.000000 tencentcloud-sdk-python-ess-3.0.875/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.874/README.rst` & `tencentcloud-sdk-python-ess-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,37 @@
 
 class EssClient(AbstractClient):
     _apiVersion = '2020-11-11'
     _endpoint = 'ess.tencentcloudapi.com'
     _service = 'ess'
 
 
+    def BindEmployeeUserIdWithClientOpenId(self, request):
+        """将电子签系统员工userId与客户系统员工openId进行绑定
+
+        :param request: Request instance for BindEmployeeUserIdWithClientOpenId.
+        :type request: :class:`tencentcloud.ess.v20201111.models.BindEmployeeUserIdWithClientOpenIdRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.BindEmployeeUserIdWithClientOpenIdResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("BindEmployeeUserIdWithClientOpenId", params, headers=headers)
+            response = json.loads(body)
+            model = models.BindEmployeeUserIdWithClientOpenIdResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CancelFlow(self, request):
         """用于撤销签署流程
         适用场景：如果某个合同流程当前至少还有一方没有签署，则可通过该接口取消该合同流程。常用于合同发错、内容填错，需要及时撤销的场景。
         注：如果合同流程中的参与方均已签署完毕，则无法通过该接口撤销合同。
 
         :param request: Request instance for CancelFlow.
         :type request: :class:`tencentcloud.ess.v20201111.models.CancelFlowRequest`
@@ -985,14 +1008,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UnbindEmployeeUserIdWithClientOpenId(self, request):
+        """将存在绑定关系的电子签系统员工userId与客户系统员工openId进行解绑
+
+        :param request: Request instance for UnbindEmployeeUserIdWithClientOpenId.
+        :type request: :class:`tencentcloud.ess.v20201111.models.UnbindEmployeeUserIdWithClientOpenIdRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.UnbindEmployeeUserIdWithClientOpenIdResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UnbindEmployeeUserIdWithClientOpenId", params, headers=headers)
+            response = json.loads(body)
+            model = models.UnbindEmployeeUserIdWithClientOpenIdResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpdateIntegrationEmployees(self, request):
         """更新员工信息(姓名，手机号，邮件)，用户实名后无法更改姓名与手机号
 
         :param request: Request instance for UpdateIntegrationEmployees.
         :type request: :class:`tencentcloud.ess.v20201111.models.UpdateIntegrationEmployeesRequest`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.874/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.875/tencentcloud/ess/v20201111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,69 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
+    """BindEmployeeUserIdWithClientOpenId请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: OpenId与UserId二选一必填一个，当传入客户系统openId，传入的openId需与电子签员工userId绑定，且渠道channel必填，channel值为INTEGRATE，否则传入userId
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param UserId: 电子签系统员工UserId
+        :type UserId: str
+        :param OpenId: 客户系统OpenId
+        :type OpenId: str
+        """
+        self.Operator = None
+        self.UserId = None
+        self.OpenId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.UserId = params.get("UserId")
+        self.OpenId = params.get("OpenId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class BindEmployeeUserIdWithClientOpenIdResponse(AbstractModel):
+    """BindEmployeeUserIdWithClientOpenId返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 绑定是否成功，1表示成功，0表示失败
+        :type Status: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.RequestId = params.get("RequestId")
+
+
 class CallbackInfo(AbstractModel):
     """应用回调信息
 
     """
 
     def __init__(self):
         r"""
@@ -5488,14 +5543,69 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class UnbindEmployeeUserIdWithClientOpenIdRequest(AbstractModel):
+    """UnbindEmployeeUserIdWithClientOpenId请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: OpenId与UserId二选一必填一个，当传入客户系统openId，传入的openId需与电子签员工userId绑定，且渠道channel必填，channel值为INTEGRATE，否则传入userId
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param UserId: 电子签系统员工UserId
+        :type UserId: str
+        :param OpenId: 客户系统OpenId
+        :type OpenId: str
+        """
+        self.Operator = None
+        self.UserId = None
+        self.OpenId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.UserId = params.get("UserId")
+        self.OpenId = params.get("OpenId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UnbindEmployeeUserIdWithClientOpenIdResponse(AbstractModel):
+    """UnbindEmployeeUserIdWithClientOpenId返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 解绑是否成功，1表示成功，0表示失败
+        :type Status: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.RequestId = params.get("RequestId")
+
+
 class UpdateIntegrationEmployeesRequest(AbstractModel):
     """UpdateIntegrationEmployees请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ess-3.0.874/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.875/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.875/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.874/setup.py` & `tencentcloud-sdk-python-ess-3.0.875/setup.py`

 * *Files identical despite different names*

