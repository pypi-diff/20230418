# Comparing `tmp/django_user_notification-0.8.0.tar.gz` & `tmp/django_user_notification-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_user_notification-0.8.0.tar", max compression
+gzip compressed data, was "django_user_notification-0.8.1.tar", max compression
```

## Comparing `django_user_notification-0.8.0.tar` & `django_user_notification-0.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django_user_notification-0.8.0/LICENSE
--rw-r--r--   0        0        0     4502 2023-04-12 10:50:30.392725 django_user_notification-0.8.0/README.md
--rw-r--r--   0        0        0       22 2023-04-12 11:14:59.782011 django_user_notification-0.8.0/notification/__init__.py
--rw-r--r--   0        0        0     3805 2023-04-12 10:58:28.320016 django_user_notification-0.8.0/notification/admin.py
--rw-r--r--   0        0        0      156 2023-03-06 01:45:02.889012 django_user_notification-0.8.0/notification/apps.py
--rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/backends/__init__.py
--rw-r--r--   0        0        0     4088 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/backends/aliyunsms.py
--rw-r--r--   0        0        0     3967 2023-04-12 11:07:43.899930 django_user_notification-0.8.0/notification/backends/dingchatbot.py
--rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django_user_notification-0.8.0/notification/backends/dingtodotask.py
--rw-r--r--   0        0        0     4591 2023-04-12 11:07:59.491019 django_user_notification-0.8.0/notification/backends/dingworkmessage.py
--rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django_user_notification-0.8.0/notification/backends/dummy.py
--rw-r--r--   0        0        0     2417 2023-04-12 11:08:12.028162 django_user_notification-0.8.0/notification/backends/email.py
--rw-r--r--   0        0        0     2216 2023-04-12 11:08:29.622794 django_user_notification-0.8.0/notification/backends/websocket.py
--rw-r--r--   0        0        0     6710 2023-04-12 11:12:05.725862 django_user_notification-0.8.0/notification/base.py
--rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/consumers.py
--rw-r--r--   0        0        0     3989 2023-04-12 11:09:49.072702 django_user_notification-0.8.0/notification/migrations/0001_initial.py
--rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django_user_notification-0.8.0/notification/migrations/0002_auto_20220808_0736.py
--rw-r--r--   0        0        0      885 2022-08-10 09:10:18.668000 django_user_notification-0.8.0/notification/migrations/0003_auto_20220810_1710.py
--rw-r--r--   0        0        0     1093 2022-08-12 07:05:54.107684 django_user_notification-0.8.0/notification/migrations/0004_auto_20220812_0705.py
--rw-r--r--   0        0        0      884 2023-01-29 05:37:49.837884 django_user_notification-0.8.0/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py
--rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/migrations/__init__.py
--rw-r--r--   0        0        0     5188 2023-04-12 11:05:18.719018 django_user_notification-0.8.0/notification/models.py
--rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django_user_notification-0.8.0/notification/static/css/hide_admin_original.css
--rw-r--r--   0        0        0      174 2023-04-12 10:53:45.477657 django_user_notification-0.8.0/notification/urls.py
--rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django_user_notification-0.8.0/notification/utils.py
--rw-r--r--   0        0        0     1701 2023-04-12 11:14:59.787743 django_user_notification-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     5738 1970-01-01 00:00:00.000000 django_user_notification-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11347 2022-08-01 06:35:17.000000 django_user_notification-0.8.1/LICENSE
+-rw-r--r--   0        0        0     4648 2023-04-13 02:57:49.997974 django_user_notification-0.8.1/README.md
+-rw-r--r--   0        0        0       22 2023-04-18 07:02:27.476163 django_user_notification-0.8.1/notification/__init__.py
+-rw-r--r--   0        0        0     3805 2023-04-12 10:58:28.320016 django_user_notification-0.8.1/notification/admin.py
+-rw-r--r--   0        0        0      156 2023-03-06 01:45:02.889012 django_user_notification-0.8.1/notification/apps.py
+-rw-r--r--   0        0        0     1301 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/backends/__init__.py
+-rw-r--r--   0        0        0     4088 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/backends/aliyunsms.py
+-rw-r--r--   0        0        0     3967 2023-04-12 11:07:43.899930 django_user_notification-0.8.1/notification/backends/dingchatbot.py
+-rw-r--r--   0        0        0     4170 2022-08-08 06:38:56.158235 django_user_notification-0.8.1/notification/backends/dingtodotask.py
+-rw-r--r--   0        0        0     4599 2023-04-18 06:59:20.038967 django_user_notification-0.8.1/notification/backends/dingworkmessage.py
+-rw-r--r--   0        0        0     1193 2022-08-08 08:42:41.480190 django_user_notification-0.8.1/notification/backends/dummy.py
+-rw-r--r--   0        0        0     2417 2023-04-12 11:08:12.028162 django_user_notification-0.8.1/notification/backends/email.py
+-rw-r--r--   0        0        0     2216 2023-04-12 11:08:29.622794 django_user_notification-0.8.1/notification/backends/websocket.py
+-rw-r--r--   0        0        0     6710 2023-04-12 11:12:05.725862 django_user_notification-0.8.1/notification/base.py
+-rw-r--r--   0        0        0     1208 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/consumers.py
+-rw-r--r--   0        0        0     3989 2023-04-12 11:09:49.072702 django_user_notification-0.8.1/notification/migrations/0001_initial.py
+-rw-r--r--   0        0        0      630 2022-08-08 07:36:05.355986 django_user_notification-0.8.1/notification/migrations/0002_auto_20220808_0736.py
+-rw-r--r--   0        0        0      885 2022-08-10 09:10:18.668000 django_user_notification-0.8.1/notification/migrations/0003_auto_20220810_1710.py
+-rw-r--r--   0        0        0     1093 2022-08-12 07:05:54.107684 django_user_notification-0.8.1/notification/migrations/0004_auto_20220812_0705.py
+-rw-r--r--   0        0        0      884 2023-01-29 05:37:49.837884 django_user_notification-0.8.1/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py
+-rw-r--r--   0        0        0        0 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/migrations/__init__.py
+-rw-r--r--   0        0        0     5188 2023-04-12 11:05:18.719018 django_user_notification-0.8.1/notification/models.py
+-rw-r--r--   0        0        0      109 2022-08-01 03:08:17.000000 django_user_notification-0.8.1/notification/static/css/hide_admin_original.css
+-rw-r--r--   0        0        0      174 2023-04-12 10:53:45.477657 django_user_notification-0.8.1/notification/urls.py
+-rw-r--r--   0        0        0      785 2022-08-04 10:27:11.874598 django_user_notification-0.8.1/notification/utils.py
+-rw-r--r--   0        0        0     1685 2023-04-18 07:02:27.482911 django_user_notification-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     5884 1970-01-01 00:00:00.000000 django_user_notification-0.8.1/PKG-INFO
```

### Comparing `django_user_notification-0.8.0/LICENSE` & `django_user_notification-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/README.md` & `django_user_notification-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,23 @@
     "dingtalktodotask": {
         "app_key": "Your App Key",
         "app_secret": "Your App Secret",
     },
 }
 ```
 
+Add `tinymce.urls` to `urls.py` for your project:
+```python
+urlpatterns = [
+    ...
+    path('tinymce/', include('tinymce.urls')),
+    ...
+]
+```
+
 Let's send a notification
 
 ``` {.python}
 from django.contrib.auth import get_user_model
 from notification.backends import notify_by_email, notify_by_dingtalk_workmessage
 
 User = get_user_model()
```

### Comparing `django_user_notification-0.8.0/notification/admin.py` & `django_user_notification-0.8.1/notification/admin.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/__init__.py` & `django_user_notification-0.8.1/notification/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/aliyunsms.py` & `django_user_notification-0.8.1/notification/backends/aliyunsms.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/dingchatbot.py` & `django_user_notification-0.8.1/notification/backends/dingchatbot.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/dingtodotask.py` & `django_user_notification-0.8.1/notification/backends/dingtodotask.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/dingworkmessage.py` & `django_user_notification-0.8.1/notification/backends/dingworkmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
             raise ValueError("Render message failed: %s" % e)
 
     def make_content(
         self, title, content, recipients, recipient_field, **kwargs
     ) -> dict:
         return {
             "msgtype": self.message_subtype,
-            self.msgtype: {"title": title, "text": content},
+            self.message_subtype: {"title": title, "text": content},
         }
 
     def get_access_token(self):
         url = "https://oapi.dingtalk.com/gettoken"
         params = {
             "appkey": self.app_key,
             "appsecret": self.app_secret,
```

### Comparing `django_user_notification-0.8.0/notification/backends/dummy.py` & `django_user_notification-0.8.1/notification/backends/dummy.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/email.py` & `django_user_notification-0.8.1/notification/backends/email.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/backends/websocket.py` & `django_user_notification-0.8.1/notification/backends/websocket.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/base.py` & `django_user_notification-0.8.1/notification/base.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/consumers.py` & `django_user_notification-0.8.1/notification/consumers.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/migrations/0001_initial.py` & `django_user_notification-0.8.1/notification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/migrations/0002_auto_20220808_0736.py` & `django_user_notification-0.8.1/notification/migrations/0002_auto_20220808_0736.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/migrations/0003_auto_20220810_1710.py` & `django_user_notification-0.8.1/notification/migrations/0003_auto_20220810_1710.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/migrations/0004_auto_20220812_0705.py` & `django_user_notification-0.8.1/notification/migrations/0004_auto_20220812_0705.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py` & `django_user_notification-0.8.1/notification/migrations/0005_alter_message_id_alter_messagetemplate_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/models.py` & `django_user_notification-0.8.1/notification/models.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/notification/utils.py` & `django_user_notification-0.8.1/notification/utils.py`

 * *Files identical despite different names*

### Comparing `django_user_notification-0.8.0/pyproject.toml` & `django_user_notification-0.8.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 [tool.commitizen]
-version = "0.8.0"
+version = "0.8.1"
 changelog_start_rev = "0.7.0"
 tag_format = "v$major.$minor.$patch$prerelease"
-version_files = [
-    "pyproject.toml:version",
-    "notification/__init__.py"
-]
+version_files = ["pyproject.toml:version", "notification/__init__.py"]
 
 [tool.poetry]
 name = "django-user-notification"
-version = "0.8.0"
+version = "0.8.1"
 description = "Django message notification package"
 authors = ["Aiden Lu <allaher@icloud.com>"]
 readme = "README.md"
 keywords = ["notification", "django"]
-packages = [
-    { include = "notification" },
-]
+packages = [{ include = "notification" }]
 homepage = "https://github.com/aiden520/django-user-notification"
 repository = "https://github.com/aiden520/django-user-notification"
 classifiers = [
     "Intended Audience :: Developers",
     "Environment :: Web Environment",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 license = "Apache-2.0"
-include = [
-    "LICENSE",
-]
+include = ["LICENSE"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 django = ">=3.1"
 requests = "^2.27.1"
-channels = { version=">=3.0.4", optional=true }
-alibabacloud-dysmsapi20170525 = { version=">=2.0.16", optional=true }
+channels = { version = ">=3.0.4", optional = true }
+alibabacloud-dysmsapi20170525 = { version = ">=2.0.16", optional = true }
 markdownify = ">=0.11.2"
 django-tinymce = "^3.6.1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 pytest = "^6.2.5"
```

### Comparing `django_user_notification-0.8.0/PKG-INFO` & `django_user_notification-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-user-notification
-Version: 0.8.0
+Version: 0.8.1
 Summary: Django message notification package
 Home-page: https://github.com/aiden520/django-user-notification
 License: Apache-2.0
 Keywords: notification,django
 Author: Aiden Lu
 Author-email: allaher@icloud.com
 Requires-Python: >=3.8
@@ -105,14 +105,23 @@
     "dingtalktodotask": {
         "app_key": "Your App Key",
         "app_secret": "Your App Secret",
     },
 }
 ```
 
+Add `tinymce.urls` to `urls.py` for your project:
+```python
+urlpatterns = [
+    ...
+    path('tinymce/', include('tinymce.urls')),
+    ...
+]
+```
+
 Let's send a notification
 
 ``` {.python}
 from django.contrib.auth import get_user_model
 from notification.backends import notify_by_email, notify_by_dingtalk_workmessage
 
 User = get_user_model()
```

