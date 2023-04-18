# Comparing `tmp/tencentcloud-sdk-python-waf-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-waf-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.874.tar", last modified: Mon Apr 17 00:54:35 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-waf-3.0.875.tar", last modified: Tue Apr 18 01:05:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-waf-3.0.874.tar` & `tencentcloud-sdk-python-waf-3.0.875.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)    42104 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/waf_client.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158204 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:54:35.000000 tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)    43870 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/waf_client.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164697 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 01:05:19.000000 tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-waf-3.0.874/README.rst` & `tencentcloud-sdk-python-waf-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/waf_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,14 +575,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribePeakPoints(self, request):
+        """查询业务和攻击概要趋势
+
+        :param request: Request instance for DescribePeakPoints.
+        :type request: :class:`tencentcloud.waf.v20180125.models.DescribePeakPointsRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.DescribePeakPointsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePeakPoints", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePeakPointsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def DescribePeakValue(self, request):
+        """获取业务和攻击概览峰值
+
+        :param request: Request instance for DescribePeakValue.
+        :type request: :class:`tencentcloud.waf.v20180125.models.DescribePeakValueRequest`
+        :rtype: :class:`tencentcloud.waf.v20180125.models.DescribePeakValueResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribePeakValue", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribePeakValueResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribePolicyStatus(self, request):
         """获取防护状态以及生效的实例id
 
         :param request: Request instance for DescribePolicyStatus.
         :type request: :class:`tencentcloud.waf.v20180125.models.DescribePolicyStatusRequest`
         :rtype: :class:`tencentcloud.waf.v20180125.models.DescribePolicyStatusResponse`
```

### Comparing `tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.874/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/waf/v20180125/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2344,14 +2344,176 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self.Data = IpHitItemsData()
             self.Data._deserialize(params.get("Data"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribePeakPointsRequest(AbstractModel):
+    """DescribePeakPoints请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FromTime: 查询起始时间
+        :type FromTime: str
+        :param ToTime: 查询终止时间
+        :type ToTime: str
+        :param Domain: 查询的域名，如果查询所有域名数据，该参数不填写
+        :type Domain: str
+        :param Edition: 只有两个值有效，sparta-waf，clb-waf，不传则不过滤
+        :type Edition: str
+        :param InstanceID: WAF实例ID，不传则不过滤
+        :type InstanceID: str
+        :param MetricName: 六个值可选：
+access-峰值qps趋势图
+botAccess- bot峰值qps趋势图
+down-下行峰值带宽趋势图
+up-上行峰值带宽趋势图
+attack-Web攻击总数趋势图
+cc-CC攻击总数趋势图
+        :type MetricName: str
+        """
+        self.FromTime = None
+        self.ToTime = None
+        self.Domain = None
+        self.Edition = None
+        self.InstanceID = None
+        self.MetricName = None
+
+
+    def _deserialize(self, params):
+        self.FromTime = params.get("FromTime")
+        self.ToTime = params.get("ToTime")
+        self.Domain = params.get("Domain")
+        self.Edition = params.get("Edition")
+        self.InstanceID = params.get("InstanceID")
+        self.MetricName = params.get("MetricName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePeakPointsResponse(AbstractModel):
+    """DescribePeakPoints返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Points: 数据点
+        :type Points: list of PeakPointsItem
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Points = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Points") is not None:
+            self.Points = []
+            for item in params.get("Points"):
+                obj = PeakPointsItem()
+                obj._deserialize(item)
+                self.Points.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
+class DescribePeakValueRequest(AbstractModel):
+    """DescribePeakValue请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FromTime: 查询起始时间
+        :type FromTime: str
+        :param ToTime: 查询结束时间
+        :type ToTime: str
+        :param Domain: 需要查询的域名，当前用户所有域名可以不传
+        :type Domain: str
+        :param Edition: 只有两个值有效，sparta-waf，clb-waf，不传则不过滤
+        :type Edition: str
+        :param InstanceID: WAF实例ID，不传则不过滤
+        :type InstanceID: str
+        :param MetricName: 五个值可选：
+access-峰值qps
+down-下行峰值带宽
+up-上行峰值带宽
+attack-Web攻击总数
+cc-CC攻击总数趋势图
+        :type MetricName: str
+        """
+        self.FromTime = None
+        self.ToTime = None
+        self.Domain = None
+        self.Edition = None
+        self.InstanceID = None
+        self.MetricName = None
+
+
+    def _deserialize(self, params):
+        self.FromTime = params.get("FromTime")
+        self.ToTime = params.get("ToTime")
+        self.Domain = params.get("Domain")
+        self.Edition = params.get("Edition")
+        self.InstanceID = params.get("InstanceID")
+        self.MetricName = params.get("MetricName")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribePeakValueResponse(AbstractModel):
+    """DescribePeakValue返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Access: QPS峰值
+        :type Access: int
+        :param Up: 上行带宽峰值，单位B
+        :type Up: int
+        :param Down: 下行带宽峰值，单位B
+        :type Down: int
+        :param Attack: Web攻击总数
+        :type Attack: int
+        :param Cc: CC攻击总数
+        :type Cc: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Access = None
+        self.Up = None
+        self.Down = None
+        self.Attack = None
+        self.Cc = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Access = params.get("Access")
+        self.Up = params.get("Up")
+        self.Down = params.get("Down")
+        self.Attack = params.get("Attack")
+        self.Cc = params.get("Cc")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribePolicyStatusRequest(AbstractModel):
     """DescribePolicyStatus请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4125,14 +4287,63 @@
     def _deserialize(self, params):
         if params.get("WafThreatenIntelligenceDetails") is not None:
             self.WafThreatenIntelligenceDetails = WafThreatenIntelligenceDetails()
             self.WafThreatenIntelligenceDetails._deserialize(params.get("WafThreatenIntelligenceDetails"))
         self.RequestId = params.get("RequestId")
 
 
+class PeakPointsItem(AbstractModel):
+    """PeakPoints数组项
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Time: 秒级别时间戳
+        :type Time: int
+        :param Access: QPS
+        :type Access: int
+        :param Up: 上行带宽峰值，单位B
+        :type Up: int
+        :param Down: 下行带宽峰值，单位B
+        :type Down: int
+        :param Attack: Web攻击次数
+        :type Attack: int
+        :param Cc: CC攻击次数
+        :type Cc: int
+        :param BotAccess: Bot qps
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BotAccess: int
+        """
+        self.Time = None
+        self.Access = None
+        self.Up = None
+        self.Down = None
+        self.Attack = None
+        self.Cc = None
+        self.BotAccess = None
+
+
+    def _deserialize(self, params):
+        self.Time = params.get("Time")
+        self.Access = params.get("Access")
+        self.Up = params.get("Up")
+        self.Down = params.get("Down")
+        self.Attack = params.get("Attack")
+        self.Cc = params.get("Cc")
+        self.BotAccess = params.get("BotAccess")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class PortInfo(AbstractModel):
     """防护域名端口配置信息
 
     """
 
 
 class PortItem(AbstractModel):
```

### Comparing `tencentcloud-sdk-python-waf-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-waf-3.0.875/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-waf-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.875/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-waf-3.0.874/setup.py` & `tencentcloud-sdk-python-waf-3.0.875/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-waf-3.0.874/tencentcloud_sdk_python_waf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-waf-3.0.875/tencentcloud_sdk_python_waf.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-waf
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Waf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

