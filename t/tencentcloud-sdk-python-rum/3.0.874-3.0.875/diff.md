# Comparing `tmp/tencentcloud-sdk-python-rum-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-rum-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.874.tar", last modified: Mon Apr 17 00:43:22 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-rum-3.0.875.tar", last modified: Tue Apr 18 00:49:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-rum-3.0.874.tar` & `tencentcloud-sdk-python-rum-3.0.875.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/
--rw-r--r--   0 root         (0) root         (0)    56021 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/rum_client.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)   161360 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:43:22.000000 tencentcloud-sdk-python-rum-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/
+-rw-r--r--   0 root         (0) root         (0)    59777 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/rum_client.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171124 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:49:15.000000 tencentcloud-sdk-python-rum-3.0.875/setup.cfg
```

### Comparing `tencentcloud-sdk-python-rum-3.0.874/README.rst` & `tencentcloud-sdk-python-rum-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/rum_client.py` & `tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/rum_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,14 +375,106 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeAppDimensionMetrics(self, request):
+        """用于查询 app 监控多维分析数据
+
+        :param request: Request instance for DescribeAppDimensionMetrics.
+        :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppDimensionMetricsRequest`
+        :rtype: :class:`tencentcloud.rum.v20210622.models.DescribeAppDimensionMetricsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAppDimensionMetrics", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAppDimensionMetricsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAppMetricsData(self, request):
+        """获取 app 监控指标数据
+
+        :param request: Request instance for DescribeAppMetricsData.
+        :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppMetricsDataRequest`
+        :rtype: :class:`tencentcloud.rum.v20210622.models.DescribeAppMetricsDataResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAppMetricsData", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAppMetricsDataResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAppSingleCaseDetailList(self, request):
+        """查询 app 监控个例样本详情列表
+
+        :param request: Request instance for DescribeAppSingleCaseDetailList.
+        :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseDetailListRequest`
+        :rtype: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseDetailListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAppSingleCaseDetailList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAppSingleCaseDetailListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribeAppSingleCaseList(self, request):
+        """查询 app 监控个例聚合列表
+
+        :param request: Request instance for DescribeAppSingleCaseList.
+        :type request: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseListRequest`
+        :rtype: :class:`tencentcloud.rum.v20210622.models.DescribeAppSingleCaseListResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAppSingleCaseList", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAppSingleCaseListResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeData(self, request):
         """转发monitor查询
 
         :param request: Request instance for DescribeData.
         :type request: :class:`tencentcloud.rum.v20210622.models.DescribeDataRequest`
         :rtype: :class:`tencentcloud.rum.v20210622.models.DescribeDataResponse`
```

### Comparing `tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/errorcodes.py` & `tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-rum-3.0.874/tencentcloud/rum/v20210622/models.py` & `tencentcloud-sdk-python-rum-3.0.875/tencentcloud/rum/v20210622/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -846,14 +846,330 @@
 
 
     def _deserialize(self, params):
         self.Msg = params.get("Msg")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeAppDimensionMetricsRequest(AbstractModel):
+    """DescribeAppDimensionMetrics请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectID: app 项目ID
+        :type ProjectID: int
+        :param From: 查询的表名
+        :type From: str
+        :param Fields: 查询指标 fields
+        :type Fields: str
+        :param Filter: 查询的过滤条件
+        :type Filter: str
+        :param FilterSimple: 查询简单过滤条件
+        :type FilterSimple: str
+        :param GroupBy: group by 条件
+        :type GroupBy: list of str
+        :param OrderBy: order by 条件
+        :type OrderBy: list of str
+        :param Limit: limit 参数
+        :type Limit: int
+        :param Offset: offset 参数
+        :type Offset: int
+        :param BusinessContext: 业务上下文参数
+        :type BusinessContext: str
+        """
+        self.ProjectID = None
+        self.From = None
+        self.Fields = None
+        self.Filter = None
+        self.FilterSimple = None
+        self.GroupBy = None
+        self.OrderBy = None
+        self.Limit = None
+        self.Offset = None
+        self.BusinessContext = None
+
+
+    def _deserialize(self, params):
+        self.ProjectID = params.get("ProjectID")
+        self.From = params.get("From")
+        self.Fields = params.get("Fields")
+        self.Filter = params.get("Filter")
+        self.FilterSimple = params.get("FilterSimple")
+        self.GroupBy = params.get("GroupBy")
+        self.OrderBy = params.get("OrderBy")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.BusinessContext = params.get("BusinessContext")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAppDimensionMetricsResponse(AbstractModel):
+    """DescribeAppDimensionMetrics返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 查询数据返回
+        :type Data: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Data = params.get("Data")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeAppMetricsDataRequest(AbstractModel):
+    """DescribeAppMetricsData请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectID: app 项目ID
+        :type ProjectID: int
+        :param From: 查询的表名
+        :type From: str
+        :param Fields: 查询指标 field
+        :type Fields: str
+        :param Filter: 查询的过滤条件
+        :type Filter: str
+        :param FilterSimple: 查询简单过滤条件
+        :type FilterSimple: str
+        :param GroupBy: group by 条件
+        :type GroupBy: list of str
+        :param OrderBy: order by 条件
+        :type OrderBy: list of str
+        :param Limit: limit 参数
+        :type Limit: int
+        :param Offset: offset 参数
+        :type Offset: int
+        :param GroupByModifier: group by 参数
+        :type GroupByModifier: str
+        """
+        self.ProjectID = None
+        self.From = None
+        self.Fields = None
+        self.Filter = None
+        self.FilterSimple = None
+        self.GroupBy = None
+        self.OrderBy = None
+        self.Limit = None
+        self.Offset = None
+        self.GroupByModifier = None
+
+
+    def _deserialize(self, params):
+        self.ProjectID = params.get("ProjectID")
+        self.From = params.get("From")
+        self.Fields = params.get("Fields")
+        self.Filter = params.get("Filter")
+        self.FilterSimple = params.get("FilterSimple")
+        self.GroupBy = params.get("GroupBy")
+        self.OrderBy = params.get("OrderBy")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        self.GroupByModifier = params.get("GroupByModifier")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAppMetricsDataResponse(AbstractModel):
+    """DescribeAppMetricsData返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 查询数据返回
+        :type Data: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Data = params.get("Data")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeAppSingleCaseDetailListRequest(AbstractModel):
+    """DescribeAppSingleCaseDetailList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectID: app 项目ID
+        :type ProjectID: int
+        :param From: 查询的表名
+        :type From: str
+        :param Fields: 查询指标 field
+        :type Fields: str
+        :param Filter: 查询的过滤条件
+        :type Filter: str
+        :param FilterSimple: 查询简单过滤条件
+        :type FilterSimple: str
+        :param GroupBy: group by 条件
+        :type GroupBy: list of str
+        :param OrderBy: order by 条件
+        :type OrderBy: list of str
+        :param Limit: limit 参数
+        :type Limit: int
+        :param Offset: offset 参数
+        :type Offset: int
+        """
+        self.ProjectID = None
+        self.From = None
+        self.Fields = None
+        self.Filter = None
+        self.FilterSimple = None
+        self.GroupBy = None
+        self.OrderBy = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.ProjectID = params.get("ProjectID")
+        self.From = params.get("From")
+        self.Fields = params.get("Fields")
+        self.Filter = params.get("Filter")
+        self.FilterSimple = params.get("FilterSimple")
+        self.GroupBy = params.get("GroupBy")
+        self.OrderBy = params.get("OrderBy")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAppSingleCaseDetailListResponse(AbstractModel):
+    """DescribeAppSingleCaseDetailList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 查询数据返回
+        :type Data: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Data = params.get("Data")
+        self.RequestId = params.get("RequestId")
+
+
+class DescribeAppSingleCaseListRequest(AbstractModel):
+    """DescribeAppSingleCaseList请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ProjectID: app 项目 ID
+        :type ProjectID: int
+        :param From: 查询的表名
+        :type From: str
+        :param Fields: 查询指标 field
+        :type Fields: str
+        :param Filter: 查询的过滤条件
+        :type Filter: str
+        :param FilterSimple: 查询简单过滤条件
+        :type FilterSimple: str
+        :param GroupBy: group by 条件
+        :type GroupBy: list of str
+        :param OrderBy: order by 条件
+        :type OrderBy: list of str
+        :param Limit: limit 参数
+        :type Limit: int
+        :param Offset: offset 参数
+        :type Offset: int
+        """
+        self.ProjectID = None
+        self.From = None
+        self.Fields = None
+        self.Filter = None
+        self.FilterSimple = None
+        self.GroupBy = None
+        self.OrderBy = None
+        self.Limit = None
+        self.Offset = None
+
+
+    def _deserialize(self, params):
+        self.ProjectID = params.get("ProjectID")
+        self.From = params.get("From")
+        self.Fields = params.get("Fields")
+        self.Filter = params.get("Filter")
+        self.FilterSimple = params.get("FilterSimple")
+        self.GroupBy = params.get("GroupBy")
+        self.OrderBy = params.get("OrderBy")
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAppSingleCaseListResponse(AbstractModel):
+    """DescribeAppSingleCaseList返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Data: 查询数据返回
+        :type Data: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Data = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Data = params.get("Data")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDataCustomUrlRequest(AbstractModel):
     """DescribeDataCustomUrl请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-rum-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-rum-3.0.875/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-rum-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.875/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.874/tencentcloud_sdk_python_rum.egg-info/PKG-INFO` & `tencentcloud-sdk-python-rum-3.0.875/tencentcloud_sdk_python_rum.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-rum
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Rum SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-rum-3.0.874/setup.py` & `tencentcloud-sdk-python-rum-3.0.875/setup.py`

 * *Files identical despite different names*

