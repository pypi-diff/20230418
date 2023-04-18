# Comparing `tmp/tencentcloud-sdk-python-teo-3.0.874.tar.gz` & `tmp/tencentcloud-sdk-python-teo-3.0.875.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.874.tar", last modified: Mon Apr 17 00:51:16 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-teo-3.0.875.tar", last modified: Tue Apr 18 00:58:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-teo-3.0.874.tar` & `tencentcloud-sdk-python-teo-3.0.875.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/
--rw-r--r--   0 root         (0) root         (0)      737 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24724 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     5379 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    20875 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   504803 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    81864 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-04-17 00:51:15.000000 tencentcloud-sdk-python-teo-3.0.874/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-04-17 00:51:16.000000 tencentcloud-sdk-python-teo-3.0.874/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24724 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     5379 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    21320 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   504803 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    81864 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-04-18 00:58:37.000000 tencentcloud-sdk-python-teo-3.0.875/setup.cfg
```

### Comparing `tencentcloud-sdk-python-teo-3.0.874/README.rst` & `tencentcloud-sdk-python-teo-3.0.875/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,17 @@
 
 # 非法条件-非法参数值-参数值长度超出限制。
 INVALIDPARAMETER_ERRINVALIDCONDITIONVALUETOOLONGVALUE = 'InvalidParameter.ErrInvalidConditionValueTooLongValue'
 
 # 非法条件-非法参数值-正则表达式数量超出限制。
 INVALIDPARAMETER_ERRINVALIDCONDITIONVALUETOOMANYREGULAR = 'InvalidParameter.ErrInvalidConditionValueTooManyRegular'
 
+# 非法条件-非法参数值-参数值数量超出限制。
+INVALIDPARAMETER_ERRINVALIDCONDITIONVALUETOOMANYVALUES = 'InvalidParameter.ErrInvalidConditionValueTooManyValues'
+
 # 非法条件-非法参数值-通配符数量超出限制。
 INVALIDPARAMETER_ERRINVALIDCONDITIONVALUETOOMANYWILDCARD = 'InvalidParameter.ErrInvalidConditionValueTooManyWildcard'
 
 # 非法条件-非法参数值-参数值数量为0。
 INVALIDPARAMETER_ERRINVALIDCONDITIONVALUEZEROLENGTH = 'InvalidParameter.ErrInvalidConditionValueZeroLength'
 
 # 开启 Grpc 协议支持需要同时开启 HTTP/2 协议支持。
@@ -247,14 +250,17 @@
 
 # 无效的自定义错误页面。
 INVALIDPARAMETER_INVALIDERRORPAGEREDIRECTURL = 'InvalidParameter.InvalidErrorPageRedirectUrl'
 
 # 无效的HTTPS。
 INVALIDPARAMETER_INVALIDHTTPS = 'InvalidParameter.InvalidHttps'
 
+# 无效的HTTPS证书。
+INVALIDPARAMETER_INVALIDHTTPSCERTINFO = 'InvalidParameter.InvalidHttpsCertInfo'
+
 # 加密套件与TLS版本不匹配。
 INVALIDPARAMETER_INVALIDHTTPSCIPHERSUITEANDTLSVERSION = 'InvalidParameter.InvalidHttpsCipherSuiteAndTlsVersion'
 
 # 无效的HTTPS HSTS。
 INVALIDPARAMETER_INVALIDHTTPSHSTSMAXAGE = 'InvalidParameter.InvalidHttpsHstsMaxAge'
 
 # 无效的HTTPS TLS版本。
@@ -543,7 +549,10 @@
 UNAUTHORIZEDOPERATION_NOPERMISSION = 'UnauthorizedOperation.NoPermission'
 
 # 后端服务器发生未知错误。
 UNAUTHORIZEDOPERATION_UNKNOWN = 'UnauthorizedOperation.Unknown'
 
 # 操作不支持。
 UNSUPPORTEDOPERATION = 'UnsupportedOperation'
+
+# 别称域名不支持目标域名源站类型为对象存储。
+UNSUPPORTEDOPERATION_TARGETNAMEORIGINTYPECOS = 'UnsupportedOperation.TargetNameOriginTypeCos'
```

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud/__init__.py` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-teo-3.0.874/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.875/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-teo-3.0.874/tencentcloud_sdk_python_teo.egg-info/PKG-INFO` & `tencentcloud-sdk-python-teo-3.0.875/tencentcloud_sdk_python_teo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-teo
-Version: 3.0.874
+Version: 3.0.875
 Summary: Tencent Cloud Teo SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-teo-3.0.874/setup.py` & `tencentcloud-sdk-python-teo-3.0.875/setup.py`

 * *Files identical despite different names*

