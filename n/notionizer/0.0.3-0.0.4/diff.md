# Comparing `tmp/notionizer-0.0.3.tar.gz` & `tmp/notionizer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/notionizer-0.0.3.tar", last modified: Thu Sep  1 08:19:56 2022, max compression
+gzip compressed data, was "notionizer-0.0.4.tar", last modified: Tue Apr 18 09:33:34 2023, max compression
```

## Comparing `notionizer-0.0.3.tar` & `notionizer-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,40 @@
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2022-09-01 08:19:56.596153 notionizer-0.0.3/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2022-09-01 08:19:56.596153 notionizer-0.0.3/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.3/README.md
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2022-09-01 08:19:56.596153 notionizer-0.0.3/notionizer/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      829 2022-06-17 18:16:57.000000 notionizer-0.0.3/notionizer/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      258 2022-04-10 11:21:06.000000 notionizer-0.0.3/notionizer/exception.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1772 2022-06-15 23:40:53.000000 notionizer-0.0.3/notionizer/functions.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2369 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/http_request.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2258 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/notion.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9014 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/object_adt.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     5199 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/object_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    24893 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/objects.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4858 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/properties_basic.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3950 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/properties_db.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4509 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/properties_page.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4492 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/properties_property.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42420 2022-09-01 08:14:17.000000 notionizer-0.0.3/notionizer/query.py
--rw-r--r--   0 sungyo    (1000) sungyo    (1000)       94 2022-06-17 18:50:31.000000 notionizer-0.0.3/notionizer/settings.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2022-09-01 08:19:56.596153 notionizer-0.0.3/notionizer.egg-info/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2022-09-01 08:19:56.000000 notionizer-0.0.3/notionizer.egg-info/PKG-INFO
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      584 2022-09-01 08:19:56.000000 notionizer-0.0.3/notionizer.egg-info/SOURCES.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2022-09-01 08:19:56.000000 notionizer-0.0.3/notionizer.egg-info/dependency_links.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2022-09-01 08:19:56.000000 notionizer-0.0.3/notionizer.egg-info/requires.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2022-09-01 08:19:56.000000 notionizer-0.0.3/notionizer.egg-info/top_level.txt
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2022-09-01 08:19:56.596153 notionizer-0.0.3/setup.cfg
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      993 2022-09-01 08:19:37.000000 notionizer-0.0.3/setup.py
-drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2022-09-01 08:19:56.596153 notionizer-0.0.3/test/
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.3/test/__init__.py
--rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1715 2022-08-31 15:39:51.000000 notionizer-0.0.3/test/test_objects.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-04-18 09:33:34.236627 notionizer-0.0.4/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      368 2022-06-22 11:05:47.000000 notionizer-0.0.4/README.md
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.232627 notionizer-0.0.4/notionizer/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      732 2023-02-17 11:30:57.000000 notionizer-0.0.4/notionizer/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2153 2023-02-09 05:51:58.000000 notionizer-0.0.4/notionizer/enum.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      316 2023-02-20 04:58:37.000000 notionizer-0.0.4/notionizer/exception.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1780 2023-02-21 08:17:05.000000 notionizer-0.0.4/notionizer/functions.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2535 2023-02-27 08:37:50.000000 notionizer-0.0.4/notionizer/http_request.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3977 2023-02-27 08:22:48.000000 notionizer-0.0.4/notionizer/notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     9289 2023-02-15 01:34:21.000000 notionizer-0.0.4/notionizer/object_adt.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     7170 2023-02-17 07:10:08.000000 notionizer-0.0.4/notionizer/object_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2380 2023-02-27 08:22:48.000000 notionizer-0.0.4/notionizer/object_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    16955 2023-02-21 09:11:19.000000 notionizer-0.0.4/notionizer/object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4950 2023-02-20 05:16:22.000000 notionizer-0.0.4/notionizer/object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1587 2023-02-13 07:50:42.000000 notionizer-0.0.4/notionizer/object_user.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     6254 2023-02-22 07:23:08.000000 notionizer-0.0.4/notionizer/properties_basic.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     3950 2023-02-21 10:19:28.000000 notionizer-0.0.4/notionizer/properties_db.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4924 2023-02-22 07:21:57.000000 notionizer-0.0.4/notionizer/properties_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4513 2023-02-21 08:37:01.000000 notionizer-0.0.4/notionizer/properties_property.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    42566 2023-02-21 09:16:09.000000 notionizer-0.0.4/notionizer/query.py
+-rw-r--r--   0 sungyo    (1000) sungyo    (1000)      126 2023-02-27 08:38:48.000000 notionizer-0.0.4/notionizer/settings.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/notionizer.egg-info/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      777 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/PKG-INFO
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      855 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        1 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        9 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/requires.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       16 2023-04-18 09:33:34.000000 notionizer-0.0.4/notionizer.egg-info/top_level.txt
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)       38 2023-04-18 09:33:34.236627 notionizer-0.0.4/setup.cfg
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      993 2023-04-18 09:33:03.000000 notionizer-0.0.4/setup.py
+drwxrwxr-x   0 sungyo    (1000) sungyo    (1000)        0 2023-04-18 09:33:34.236627 notionizer-0.0.4/test/
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)        0 2022-06-14 09:15:51.000000 notionizer-0.0.4/test/__init__.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     1986 2023-02-21 05:40:06.000000 notionizer-0.0.4/test/test_block.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      638 2023-02-21 12:44:32.000000 notionizer-0.0.4/test/test_notion.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     4912 2023-02-09 07:32:20.000000 notionizer-0.0.4/test/test_notion1.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      398 2023-02-21 12:44:32.000000 notionizer-0.0.4/test/test_notion_getdatabase.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2647 2023-02-21 07:46:13.000000 notionizer-0.0.4/test/test_object_database.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)     2596 2023-02-27 08:22:48.000000 notionizer-0.0.4/test/test_object_page.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)      169 2023-02-15 02:03:42.000000 notionizer-0.0.4/test/test_objects.py
+-rw-rw-r--   0 sungyo    (1000) sungyo    (1000)    14244 2023-02-13 05:30:10.000000 notionizer-0.0.4/test/test_query.py
```

### Comparing `notionizer-0.0.3/PKG-INFO` & `notionizer-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.3/notionizer/__init__.py` & `notionizer-0.0.4/notionizer/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-
-# __all__ = ["query", "notion", "objects", "exception"]
-
 from .notion import Notion
 
-from .objects import User
-from .objects import UserProperty
-from .objects import Database
-from .objects import Page
-from .objects import Property
-from .objects import NumberFormat
-from .objects import OptionColor
-from .objects import RollupFunction
+from .object_user import UserProperty, User
+from .object_database import Database
+from .object_page import Page
+from .object_database import Property
+from .enum import OptionColor, NumberFormat, RollupFunction
 
 from .exception import NotionApiException
 from .exception import NotionApiPropertyException
 from .exception import NotionApiPropertyUnassignedException
 from .exception import NotionApiQueoryException
 
 __version__ = "0.0.1"
```

### Comparing `notionizer-0.0.3/notionizer/functions.py` & `notionizer-0.0.4/notionizer/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from functools import wraps
 from typing import List
 from typing import Any
 from typing import Dict
 from typing import Callable
+import re
 
 
 def pdir(obj: object, level: str = 'public') -> List[str]:
     attr_list = dir(obj)
     if level == 'hide':
         attr_list = [a for a in attr_list if a[:2] != '__']
     elif level == 'public':
@@ -53,9 +54,8 @@
     def wrapper_function(*args: List[Any], **kwargs: Dict[str, Any]) -> None:
         if 'instance_id' in kwargs:
             del kwargs['instance_id']
             init_function(*args, **kwargs)
         else:
             init_function(*args, **kwargs)
 
-    return wrapper_function
-
+    return wrapper_function
```

### Comparing `notionizer-0.0.3/notionizer/http_request.py` & `notionizer-0.0.4/notionizer/http_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,34 +39,37 @@
 
     def get(self: T_HttpRequest, url: str) -> Tuple[T_HttpRequest, Dict[str, Any]]:
         return self._request('GET', url, {})
 
     def patch(self: T_HttpRequest, url: str, payload: Dict[str, Any]) -> Tuple[T_HttpRequest, Dict[str, Any]]:
         return self._request('PATCH', url, payload)
 
+    def delete(self: T_HttpRequest, url: str):
+        return self._request('DELETE', url, {})
+
     def _request(self: T_HttpRequest, request_type: str, url: str, payload: Dict[str, Any]) -> Tuple[T_HttpRequest,
                                                                                                      Dict[str, Any]]:
         """
 
         :param request_type: 'POST' or 'GET'
         :param url: fully assembled url
         :param payload:
         :return: python data type object(dictionay and list)
         """
-        _logger.debug('url: ' + self.base_url + url)
-        _logger.debug('payload:' + str(payload))
+        _logger.debug( f'[{request_type}] url[{self.base_url + url}] payload: {payload}')
+        # _logger.debug('payload:' + str(payload))
         payload_json = ''
         if payload:
             payload_json = json.dumps(payload)
         request_url: str = self.base_url + url
         result_json: str = requests.request(request_type, request_url, headers=self.__headers,
                                             data=payload_json, timeout=self.timeout).text
 
         result: Dict[str, Any] = json.loads(result_json)
         _logger.debug(f"result: {result}")
         if result['object'] == 'error':
             status = result['status']
             code = result['code']
             message = result['message']
-            raise HttpRequestError(f'[{status}] {code}: {message}, {payload} from: {request_url}')
+            raise HttpRequestError(f'[{status}] {code}: {message}, header: {self.__headers} body: {payload} from: {request_url}')
 
         return self, result
```

### Comparing `notionizer-0.0.3/notionizer/notion.py` & `notionizer-0.0.4/notionizer/object_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,83 +1,56 @@
-"""
-Notion API
+from typing import Dict, Any
 
+import notionizer.object_adt
+import notionizer.object_basic
+import notionizer.functions
+import notionizer.http_request
 
-"""
+ImmutableProperty = notionizer.object_adt.ImmutableProperty
+NotionUpdateObject = notionizer.object_basic.NotionUpdateObject
+UserBaseObject = notionizer.object_basic.UserBaseObject
+notion_object_init_handler = notionizer.functions.notion_object_init_handler
+HttpRequest = notionizer.http_request.HttpRequest
 
-import logging as _logging
-_log = _logging.getLogger(__name__)
-_logging.basicConfig(format='%(asctime)s [%(filename)s:%(lineno)s|%(levelname)s] %(funcName)s(): %(message)s')
 
-from notionizer.http_request import HttpRequest
-from notionizer.objects import Database
-from notionizer.objects import Page
-from notionizer.objects import User
 
+_log = __import__('logging').getLogger(__name__)
 
-class Notion:
-    f"""
-    Notion
 
-    'Notion' is basic object of 'notionized' module.
+class UserProperty(ImmutableProperty):
+    """
+    User Property for Database, Page: 'created_by' and 'last_edited_by'
     """
 
-    def __init__(self, secret_key: str):
-        self.__secret_key = secret_key
-        self._request: HttpRequest = HttpRequest(secret_key)
-
-    def get_database(self, database_id: str) -> Database:
-        """
-        get 'Database' Object by 'database_id'
+    def __set__(self, owner: NotionUpdateObject, value: Dict[str, Any]) -> None:
+        obj = User(owner._request, value)
+        super().__set__(owner, obj)
 
-        https://www.notion.so/myworkspace/a8aec43384f447ed84390e8e42c2e089?v=...
-                                         |---------- Database ID --------|
-        :param database_id:
-        :return: Database
-        """
 
-        result = self._request.get('v1/databases/' + database_id)
-        db_object: Database = Database(*result)
-        return db_object
-
-    def get_page(self, page_id: str) -> Page:
-        """
-        get 'Page' object by 'page id'
-        :param page_id:
-        :return: Page
-        """
-        page_object: Page = Page(*self._request.get('v1/pages/' + page_id))
-        return page_object
+class User(NotionUpdateObject, UserBaseObject):
+    """
+    User Object
+    """
+    _api_url = 'v1/users/'
 
-    def get_user(self, user_id: str) -> User:
-        """
-        get 'User' object by 'user id'.
-        :param user_id:
-        :return: User
+    @notion_object_init_handler
+    def __init__(self, request: HttpRequest, data: Dict[str, Any]):
         """
-        user_object: User = User(*self._request.get('v1/users/' + user_id))
-        return user_object
 
-    def get_all_users(self) -> list:
+        :param request:
+        :param data:
         """
-        get a paginated list of 'Users for the workspace(user and bots)'.
-        :return: List[User]
-        """
-        request: HttpRequest
-        user_list = list()
-
-        request, result = self._request.get('v1/users')
-
-        for obj in result['results']:
-            user_list.append(User(request, obj))
-        return user_list
+        self._update_event_status = False
+        super().__init__(request, data)
 
-    def get_me(self) -> User:
+    def update_info(self) -> None:
         """
-        get the 'bot User' itself associated with the API token
-        :return: User
+        get all information of user. If already updated, stop and doesn't make request event.
+        :return: None
         """
-        me: User = User(*self._request.get('v1/users/me'))
-        return me
+        if self._update_event_status:
+            return
 
-    def get_block(self, block_id: str):
-        pass
+        url = self._api_url + str(self.id)
+        request, data = self._request.get(url)
+        _log.debug(f"{type(self).__init__}")
+        type(self)(request, data, instance_id=data['id'])
```

### Comparing `notionizer-0.0.3/notionizer/object_adt.py` & `notionizer-0.0.4/notionizer/object_adt.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,18 @@
 class DictionaryObject(MutableMapping[str, Any]):
     """
     'DictionaryObject Descriptor' which used for 'Key-Value' object. Immutable is 'default'.
     """
 
     def __init__(self, name: str, owner: Any = None, data: Optional[Dict[str, Any]] = None, mutable: bool = False):
         """
-        Initilize '_DictionaryObject'.
+        Initilize 'DictionaryObject'.
 
         :param name: str (property name)
-        :param owner: NotionObject (other name is parent)
+        :param owner: NotionBaseObject (other name is parent)
         :param data: if it assigned, object doesn't need 'additianl assigning event'.
         :param mutable: bool (default: False)
         """
 
         self.name = name
         self._mutable = mutable
 
@@ -110,15 +110,15 @@
             mutable_status = self._mutable
             self._mutable = True
             for k, v in value.items():
                 self.__setitem__(k, get_proper_object(k, v, self))
             self._mutable = mutable_status
         else:
             _log.debug(f"{self.name}, {owner}, {self._data}")
-            raise NotionApiPropertyException(f"values of '_DictionaryObject' already assigned")
+            raise NotionApiPropertyException(f"values of 'DictionaryObject' already assigned")
 
     # Implement MutableMapping method
     def __getitem__(self, key):
         return self._data[key]
 
     def __iter__(self):
         return iter(self._data)
@@ -149,14 +149,20 @@
         return len(self._data)
 
     def keys(self) -> KeysView[str]:
         return self._data.keys()
 
 
 class ListObject(MutableSequence[Any]):
+    """
+    Implementation 'Emulating container type', generally 'list' object in python.
+    use 'ListObject' itself, or inherit and override specific method as developer wants.
+
+    ref) https://docs.python.org/3/reference/datamodel.html#emulating-container-types
+    """
 
     def __init__(self, name, owner, data: list=None, mutable=False):
 
         self.name = name
         self._mutable = mutable
         self._data = list()
 
@@ -193,15 +199,15 @@
 
     def __set__(self, owner, value: list):
 
         assert type(value) == list
         # _log.debug(f"owner, value, {repr(owner)}, {repr(value)}")
 
         if self._data:
-            raise NotionApiPropertyException("values of '_ListObject' already assigned")
+            raise NotionApiPropertyException("values of 'ListObject' already assigned")
 
         mutable_status = self._mutable
 
         self._mutable = True
         for e in value:
             # _log.debug(f"{e}")
             proper_obj = get_proper_object(self.name, e, self)
```

### Comparing `notionizer-0.0.3/notionizer/objects.py` & `notionizer-0.0.4/notionizer/object_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,97 +7,64 @@
 
 Fallow rules make python object safety from user assignment event.
 
 
 - Only mutable properties defined 'in class' manually as 'MutableProperty' descriptor.
 - Other properties are defined 'Immutable Property' dynamically.
 - Some properties has own 'object' and 'array', which in python are 'dictionay' and 'list'. It's
-  replace as '_DictionaryObject' and '_ListObject'. These are 'immutable' as default. But 'mutable' parameter makes
+  replace as 'DictionaryObject' and 'ListObject'. These are 'immutable' as default. But 'mutable' parameter makes
   these 'mutable' object.
 
 """
 
-from notionizer.http_request import HttpRequest
-
-from notionizer.object_basic import NotionObject
-from notionizer.object_basic import UserObject
-from notionizer.object_adt import DictionaryObject
-from notionizer.properties_property import PropertiesProperty
-from notionizer.functions import notion_object_init_handler
-from notionizer.functions import from_plain_text_to_rich_text_array
-from notionizer.properties_basic import TitleProperty, DbPropertyObject
-from notionizer.object_adt import ImmutableProperty, MutableProperty
-from notionizer.properties_db import DbPropertyRelation
-
-from notionizer.query import Query
-from notionizer.query import filter
-from notionizer.query import T_Filter
-from notionizer.query import T_Sorts
+import notionizer.http_request
+import notionizer.object_basic
+import notionizer.object_adt
+import notionizer.properties_property
+import notionizer.functions
+import notionizer.properties_basic
+import notionizer.properties_db
+import notionizer.query
 
 from typing import Optional
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Union
 from typing import Set
+from typing import KeysView
 
+# import notionizer.object_page
 
-_log = __import__('logging').getLogger(__name__)
-
-
-class NotionBasicObject(NotionObject):
-    """
-    '_NotionBasicObject' with '_update' method which update information and refresh itself.
-    """
-    _instances: Dict[str, Any] = {}
-
-    _api_url: str
-    id: ImmutableProperty
-
-    def __new__(cls, request: HttpRequest, data: Dict[str, Any], instance_id: Optional[str] = None
-                , **kwargs) -> 'NotionBasicObject':
-        """
-        construct '_NotionBasicObject' class.
-
-        check 'key' value and if instance is exist, reuse instance with renewed namespace.
-        :param request:
-        :param data:
-        :param instance_id:
-        """
+from notionizer.object_page import Page
 
-        _log.debug(" ".join(map(str, ('NotionBasicObject:', cls))))
-        instance: 'NotionBasicObject' = super(NotionBasicObject, cls).__new__(cls, data)  # type: ignore
 
-        # assign 'new namespace' with 'unassigned descriptors'.
-        if instance_id:
-            NotionBasicObject._instances[instance_id].__dict__ = instance.__dict__
-        else:
-            instance_id = str(data['id'])
-            NotionBasicObject._instances[instance_id] = instance
+ImmutableProperty = notionizer.object_adt.ImmutableProperty
+UserProperty = notionizer.object_user.UserProperty
+# Page = notionizer.object_page.Page
+Query = notionizer.query.Query
+filter = notionizer.query.filter
+T_Filter = notionizer.query.T_Filter
+T_Sorts = notionizer.query.T_Sorts
+
+
+HttpRequest = notionizer.http_request.HttpRequest
+NotionBaseObject = notionizer.object_basic.NotionBaseObject
+NotionUpdateObject = notionizer.object_basic.NotionUpdateObject
+UserBaseObject = notionizer.object_basic.UserBaseObject
+DictionaryObject = notionizer.object_adt.DictionaryObject
+MutableProperty = notionizer.object_adt.MutableProperty
+PropertiesProperty = notionizer.properties_property.PropertiesProperty
+notion_object_init_handler = notionizer.functions.notion_object_init_handler
+from_plain_text_to_rich_text_array = notionizer.functions.from_plain_text_to_rich_text_array
+DbPropertyObject = notionizer.properties_basic.DbPropertyObject
+TitleProperty = notionizer.properties_basic.TitleProperty
+DbPropertyRelation = notionizer.properties_db.DbPropertyRelation
 
-        return instance
-
-    def __init__(self, request: HttpRequest, data: Dict[str, Any], instance_id: Optional[str] = None):
-        """
-
-        :param request:
-        :param data:
-        :param instance_id:
-        """
-        _log.debug(" ".join(map(str, ('NotionBasicObject:', self))))
-        self._request: HttpRequest = request
-        super().__init__(data)
-
-    def _update(self, property_name: str, contents: Dict[str, Any]) -> None:
-        url = self._api_url + str(self.id)
-        request, data = self._request.patch(url, {property_name: contents})
-        # update property of object using 'id' value.
-        cls: type(NotionBasicObject) = type(self)  # type: ignore
-        # update instance
-        cls(request, data, instance_id=str(data['id']))
+_log = __import__('logging').getLogger(__name__)
 
 
 class QueriedPageIterator:
     """
     database Queried Page Iterator
     """
 
@@ -164,55 +131,15 @@
 [v] 'Page' object under created_by and last_edited_by and in people property items.
 [v] 'Property' object when the property is a people property.
 [ ] 'Block' object under created_by and last_edited_by.
 [ ] 'Rich text' object, as user mentions.
 """
 
 
-class User(NotionBasicObject, UserObject):
-    """
-    User Object
-    """
-    _api_url = 'v1/users/'
-
-    @notion_object_init_handler
-    def __init__(self, request: HttpRequest, data: Dict[str, Any]):
-        """
-
-        :param request:
-        :param data:
-        """
-        self._update_event_status = False
-        super().__init__(request, data)
-
-    def update_info(self) -> None:
-        """
-        get all information of user. If already updated, stop and doesn't make request event.
-        :return: None
-        """
-        if self._update_event_status:
-            return
-
-        url = self._api_url + str(self.id)
-        request, data = self._request.get(url)
-        _log.debug(f"{type(self).__init__}")
-        type(self)(request, data, instance_id=data['id'])
-
-
-class UserProperty(ImmutableProperty):
-    """
-    User Property for Database, Page: 'created_by' and 'last_edited_by'
-    """
-
-    def __set__(self, owner: NotionBasicObject, value: Dict[str, Any]) -> None:
-        obj = User(owner._request, value)
-        super().__set__(owner, obj)
-
-
-class Database(NotionBasicObject):
+class Database(NotionUpdateObject):
 
     _api_url = 'v1/databases/'
 
     id = ImmutableProperty()
     created_time = ImmutableProperty()
     created_by = UserProperty()
     last_edited_by = UserProperty()
@@ -226,27 +153,27 @@
     def __init__(self, request: HttpRequest, data: Dict[str, Any], update_relation: bool = True):
         """
          initilize Database instance.
 
         :param request: Notion._request
         :param data: returned from ._request
         :param update_relation: (bool) assign 'False' for 'database object' of checking relation reference
-        """
+        # """
 
         object_type = data['object']
         assert object_type == 'database', f"data type is not 'database'. (type: {object_type})"
 
         _log.debug(" ".join(map(str, ('Database:', self))))
         super().__init__(request, data)
         self._relation_reference: Dict[str, DictionaryObject] = dict()
         self._query_helper = Query(self.properties)
         if update_relation:
             self._update_relation_reference()
 
-    def __str__(self) -> str:
+    # def __str__(self) -> str:
         title = ''
         try:
             title = ": " + str(self.title)
         except:
             pass
         str_content = f"<'{self.__class__.__name__}{title}'>"
         return str_content
@@ -401,233 +328,32 @@
                     f"{db_property}('{key}') property has type {db_property._input_validation}"
 
                 value_converted = db_property._convert_to_update(value)
                 payload['properties'][key] = value_converted
 
         return Page(*self._request.post(url, payload))
 
-
-class Page(NotionBasicObject):
-    """
-    Page Object
-    """
-    properties = PropertiesProperty(object_type='page')
-    id = ImmutableProperty()
-    created_by = UserProperty()
-    last_edited_by = UserProperty()
-
-    _api_url = 'v1/pages/'
-
-    @notion_object_init_handler
-    def __init__(self, request: HttpRequest, data: Dict[str, Any]):
-
-        """
-
-        Args:
-            request: Notion._request
-            data: returned from ._request
-        """
-
-        object_type = data['object']
-        assert object_type == 'page', f"data type is not 'database'. (type: {object_type})"
-        super().__init__(request, data)
-
-    def __repr__(self) -> str:
-        return f"<Page at '{self.id}'>"
-
-    def get_properties(self) -> Dict[str, Any]:
-        """
-        return value of properties simply
-        :return: {'key' : value, ...}
-        """
-        result = dict()
-        for k, v in self.properties.items():
-            result[k] = v.get_value()
-
-        return result
-
-
-    def create_database(self,
-                        title: str = '',
-                        emoji: str = '',
-                        cover: str = '',
-                        parent: str = '',
-                        properties: list = []
-                        ) -> Database:
-
-        """
-
-        :param title:
-        :param emoji:
-        :param cover:
-        :param parent:
-        :param properties:
-        :return: Database
-
-        [Usage]
-
-        from notionizer import Property as Prop
-        from notionizer import NumberFormat as NumForm
-        from notionizer import OptionColor as OptColor
-
-        db = page.create_database(
-            title='DB Title',
-            emoji="🎉",
-            cover="https://web.image.path/image.jpg",
-            properties
-
-            notion.create_database("title", properties = [
-                Prop.RichText("text filed"),
-                Prop.Number("number", format = NumForm.dollar),
-                Prop.Select("select", option = {'opt1': OptColor.blue, 'opt2': OptColor.red}),
-                Prop.MultiSelect("multi select", option = {'opt1': OptColor.blue, 'opt2': OptColor.red}),
-                ...
-                ]
-            )
-        )
-
-        """
-
-        data: Dict[str, Any] = {'parent': {'type': 'page_id'}, 'properties': {}}
-        if parent:
-            data['parent']['page_id'] = parent
-        else:
-            data['parent']['page_id'] = self.id
-
-        if title:
-            data['title'] = from_plain_text_to_rich_text_array(title)
-
-        if emoji:
-            data['icon'] = {'type': 'emoji'}
-            data['icon']['emoji'] = emoji
-
-        if cover:
-            data['cover'] = {'type': 'external'}
-            data['cover']['external'] = {'url': cover}
-
-        # properties validation
-        prop_names = sorted(p.name for p in properties)
-        prop_types = sorted(p.prop_type for p in properties)
-        assert len(properties) == len(set(prop_names)), f"please check duplicated name of property: {str(prop_names)}"
-
-        # title property should be included.
-        if 'title' not in prop_types:
-            default_name = 'Name'
-            unused_name = default_name
-            index = 0
-            while unused_name in prop_names:
-                index += 1
-                unused_name = default_name + str(index).zfill(2)
-
-            data['properties'][unused_name] = {"title": {}}
-
-        for p in properties:
-            data['properties'][p.name] = {p.prop_type: {}}
-
-            for opt in p.arguments.keys():
-                if opt == 'options':
-                    data['properties'][p.name][p.prop_type]['options'] = []
-                    for name, color in p.arguments[opt].items():
-                        data['properties'][p.name][p.prop_type]['options'].append({'name': name, 'color': color})
-                else:
-                    data['properties'][p.name][p.prop_type][opt] = p.arguments[opt]
-
-        db_object: Database = Database(*self._request.post('v1/databases/', data))
-        return db_object
-
-
-class OptionColor:
-    """
-    Enum using for Select and Multi-Select
-    """
-    default = 'default'
-    gray = 'gray'
-    brown = 'brown'
-    orange = 'orange'
-    yellow = 'yellow'
-    green = 'green'
-    blue = 'blue'
-    purple = 'purple'
-    pink = 'pink'
-    red = 'red'
-
-
-class NumberFormat:
-    """
-    Enum using for format of Number
-    """
-    number = 'number'
-    number_with_commas = 'number_with_commas'
-    percent = 'percent'
-    dollar = 'dollar'
-    canadian_dollar = 'canadian_dollar'
-    euro = 'euro'
-    pound = 'pound'
-    yen = 'yen'
-    ruble = 'ruble'
-    rupee = 'rupee'
-    won = 'won'
-    yuan = 'yuan'
-    real = 'real'
-    lira = 'lira'
-    rupiah = 'rupiah'
-    franc = 'franc'
-    hong_kong_dollar = 'hong_kong_dollar'
-    new_zealand_dollar = 'new_zealand_dollar'
-    krona = 'krona'
-    norwegian_krone = 'norwegian_krone'
-    mexican_peso = 'mexican_peso'
-    rand = 'rand'
-    new_taiwan_dollar = 'new_taiwan_dollar'
-    danish_krone = 'danish_krone'
-    zloty = 'zloty'
-    baht = 'baht'
-    forint = 'forint'
-    koruna = 'koruna'
-    shekel = 'shekel'
-    chilean_peso = 'chilean_peso'
-    philippine_peso = 'philippine_peso'
-    dirham = 'dirham'
-    colombian_peso = 'colombian_peso'
-    riyal = 'riyal'
-    ringgit = 'ringgit'
-    leu = 'leu'
-    argentine_peso = 'argentine_peso'
-    uruguayan_peso = 'uruguayan_peso'
-
-
-class RollupFunction:
-    """
-    Enum using for rollup funtion parameter
-    """
-
-    count = "count"
-    count_values = "count_values"
-    empty = "empty"
-    not_empty = "not_empty"
-    unique = "unique"
-    show_unique = "show_unique"
-    percent_empty = "percent_empty"
-    percent_not_empty = "percent_not_empty"
-    sum = "sum"
-    average = "average"
-    median = "median"
-    min = "min"
-    max = "max"
-    range = "range"
-    earliest_date = "earliest_date"
-    latest_date = "latest_date"
-    date_range = "date_range"
-    checked = "checked"
-    unchecked = "unchecked"
-    percent_checked = "percent_checked"
-    percent_unchecked = "percent_unchecked"
-    count_per_group = "count_per_group"
-    percent_per_group = "percent_per_group"
-    show_original = "show_original"
+    # Implement MutableMapping method
+    def __getitem__(self, key):
+        raise NotImplementedError
+
+    # def __iter__(self):
+    #     raise NotImplementedError
+    #
+    # def __setitem__(self, key, value):
+    #     raise NotImplementedError
+    #
+    # def __delitem__(self, key: str) -> None:
+    #     raise NotImplementedError
+    #
+    # def __len__(self) -> int:
+    #     raise NotImplementedError
+    #
+    # def keys(self) -> KeysView[str]:
+    #     raise NotImplementedError
 
 
 class Property:
     """
     A group of property types defined for database creating.
 
     [Usage]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `notionizer-0.0.3/notionizer/properties_basic.py` & `notionizer-0.0.4/notionizer/properties_basic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from notionizer.functions import from_rich_text_array_to_plain_text, from_plain_text_to_rich_text_array, pdir
 
 from notionizer.object_adt import MutableProperty, ListObject, ImmutableProperty
-from notionizer.object_basic import NotionObject
+from notionizer.object_basic import NotionBaseObject
 
 from typing import Dict
 from typing import Tuple
 from typing import Any
 from typing import Callable
 
 from urllib import parse
@@ -47,45 +47,46 @@
         :param obj:
         :param value:
         :return:
         """
         super().__set__(obj, parse.unquote(value))
 
 
-class PropertyObject(NotionObject):
+class PropertyBaseObject(NotionBaseObject):
     """
     Basic Object for Data and Page Properties.
     """
     # to find which object is proper, uses '_type_defined' while assigning event.
     _type_defined = ''
 
     def __new__(cls, parent: Any, data: Dict[str, Any], parent_type: str, name: str, force_new: bool = False) \
-            -> 'PropertyObject':
-        new_cls = super(PropertyObject, cls)
+            -> 'PropertyBaseObject':
+        new_cls = super(PropertyBaseObject, cls)
         ins = new_cls.__new__(cls, data, force_new=force_new)  # type: ignore
         return ins
 
     def __init__(self, parent: Any, data: Dict[str, Any], parent_type: str, name: str, force_new: bool = False):
         """
 
         :param parent: PropertiesProperty
         :param data:
         :param parent_type:
         :param name:
         :param force_new:
         """
         self._parent: 'PropertiesProperty' = parent  # type: ignore
         self._parent_type = parent_type
-
+        # dictionary for filter
+        self._filter_body: Dict[str, Any] = dict()
         # page properties don't have 'name' property. This method assign '_name' property manually.
         self._name = name
         super().__init__(data)
 
 
-class PagePropertyObject(PropertyObject):
+class PagePropertyObject(PropertyBaseObject):
     """
     Basic Object for Data and Page Properties.
     """
 
     # to figure out which object is 'proper', uses '_type_defined' while assigning event.
     _type_defined = ''
 
@@ -97,36 +98,40 @@
 
     def get_value(self):
 
         value = getattr(self, self.type)
 
         if hasattr(value, 'keys'):
             if 'name' in value:
+                # _log.info(f"{self}, {self.type}, {value.keys()}")
                 return value['name'].replace(u'\xa0', u' ')
             else:
-                # _log.info(f"{self}, {self.type}, {value.keys()}")
-                return value
+                # _log.info(f"{self}, {self.type}, {value}")
+                # 빈 값에 대한 리턴 처리
+                # return value
+                return ''
 
         elif isinstance(value, (list, ListObject)):
             result = []
             for e in value:
                 if hasattr(e, '__getitem__') and 'name' in e:
                     result.append(e['name'].replace(u'\xa0', u' '))
                 elif hasattr(e, 'name') and e.name == 'relation':
                     result.append(e['id'])
                 elif hasattr(e, 'name'):
                     result.append(e.name.replace(u'\xa0', u' '))
                 else:
                     result.append(e)
             return tuple(result)
         else:
+            _log.info(f"{self}, {self.type}, {value}")
             return value
 
 
-class DbPropertyObject(PropertyObject):
+class DbPropertyObject(PropertyBaseObject):
     """
     Basic Object for Data and Page Properties.
     """
     # to find which object is proper, uses '_type_defined' while assigning event.
     _type_defined = ''
     _mutable = False
 
@@ -153,8 +158,36 @@
 
         :param value: nay of type
         :return: dictionary
         """
         return {self._type_defined: value}
 
     def __repr__(self) -> str:
-        return f"<'{self.__class__.__name__}: {self.name}' at {hex(id(self))}>"
+        return f"<'{self.__class__.__name__}: {self.name}' at {hex(id(self))}>"
+
+    def __lt__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__lt__' method")
+
+    def __le__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__le__' method")
+
+    def __eq__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__eq__' method")
+
+    # !=
+    def __ne__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__ne__' method")
+
+    def __gt__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__gt__' method")
+
+    def __ge__(self, other):
+        raise Exception(f"Property '{self.type}' type does not support '__ge__' method")
+
+    def __contains__(self, item):
+        raise Exception(f"Property '{self.type}' type does not support '__contains__' method")
+
+    def __and__(self, item):
+        raise Exception(f"Property '{self.type}' type does not support '__and__' method")
+
+    def __or__(self, item):
+        raise Exception(f"Property '{self.type}' type does not support '__or__' method")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `notionizer-0.0.3/notionizer/properties_db.py` & `notionizer-0.0.4/notionizer/properties_db.py`

 * *Files identical despite different names*

### Comparing `notionizer-0.0.3/notionizer/properties_page.py` & `notionizer-0.0.4/notionizer/properties_page.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from notionizer.functions import from_rich_text_array_to_plain_text
 from notionizer.functions import parse_date_object
 from notionizer.object_adt import MutableProperty
 from notionizer.properties_basic import PagePropertyObject
-from notionizer.object_basic import UserObject
+from notionizer.object_basic import UserBaseObject
 from typing import Any, Dict, List
 
 
 def parse_value_object(obj: Any) -> Any:
     """
     parse value of 'formula' and 'rollup'. 
 
@@ -79,18 +79,18 @@
         :param parent: PropertiesProperty
         :param data:
         :param parent_type:
         :param name:
         :param force_new:
         """
 
-        user_list: List[UserObject] = list()
+        user_list: List[UserBaseObject] = list()
         object_list: List[Dict[str, Any]] = data['people']
         for e in object_list:
-            user_list.append(UserObject(e))
+            user_list.append(UserBaseObject(e))
         data['people'] = user_list
         super().__init__(parent, data, parent_type, name)
 
 
 class PagePropertyMultiSelect(PagePropertyObject):
     """
     'PagePropertyMultiSelect'
@@ -137,14 +137,40 @@
 
     def get_value(self) -> Any:
         """
         parse 'rich_text' to plain 'string' and return
         """
         return from_rich_text_array_to_plain_text(self.rich_text)
 
+    def is_not_empty(self):
+        pass
+
+    def starts_with(self):
+        pass
+
+    def does_not_contain(self):
+        pass
+
+    def ends_with(self):
+        pass
+
+    def does_not_equal(self):
+        pass
+
+    def is_empty(self):
+        pass
+
+    def equals(self, string: str):
+        self._body[self._type_defined]['equals'] = string
+        return self
+
+    def contains(self):
+        pass
+
+
 
 class PagePropertyUrl(PagePropertyObject):
     """
     'PagePropertyUrl'
     """
     _type_defined = 'url'
     url = MutableProperty()
```

### Comparing `notionizer-0.0.3/notionizer/properties_property.py` & `notionizer-0.0.4/notionizer/properties_property.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from notionizer.object_adt import DictionaryObject, ImmutableProperty
-from notionizer.object_basic import _log
-from notionizer.properties_basic import PropertyObject, PagePropertyObject, DbPropertyObject
+from notionizer.properties_basic import PropertyBaseObject, PagePropertyObject, DbPropertyObject
 
 import notionizer.properties_page
 import notionizer.properties_db
 from typing import Any
 from typing import Dict
 from typing import Optional
 
+_log = __import__('logging').getLogger(__name__)
+
 
 class PropertiesProperty(DictionaryObject, ImmutableProperty):
     """
     'PropertiesProperty' for 'Database' and 'Page'. Mutable Type
     """
 
     """
@@ -72,16 +73,16 @@
         for k, v in value.items():
             property_type: str = v['type']
             if self._parent_object_type == 'database' and property_type == 'rich_text':
                 property_type = 'text'
 
             if property_type in properties_mapper:
 
-                property_cls: PropertyObject = properties_mapper.get(property_type)
-                property_ins: PropertyObject = property_cls(self, v, parent_type=self._parent_object_type, name=k)
+                property_cls: PropertyBaseObject = properties_mapper.get(property_type)
+                property_ins: PropertyBaseObject = property_cls(self, v, parent_type=self._parent_object_type, name=k)
             else:
                 if self._parent_object_type == 'database':
                     property_ins: DbPropertyObject = DbPropertyObject(self, v, parent_type=self._parent_object_type,
                                                                       force_new=True, name=k)
                 elif self._parent_object_type == 'page':
                     property_ins: PagePropertyObject = PagePropertyObject(self, v, parent_type=self._parent_object_type,
                                                                           force_new=True, name=k)
```

### Comparing `notionizer-0.0.3/notionizer/query.py` & `notionizer-0.0.4/notionizer/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 from notionizer import properties_basic
 from notionizer.properties_basic import DbPropertyObject
 from notionizer.functions import pdir
 from notionizer.exception import NotionApiQueoryException
 
 log = __import__('logging').getLogger(__name__)
 
-python_version = str(sys.version_info.major) + '.' + str(sys.version_info.minor)
+# python_version = str(sys.version_info.major) + '.' + str(sys.version_info.minor)
+python_version_current = (sys.version_info.major, sys.version_info.minor)
+
+python_version_3_8 = (3, 8)
 
 """
     filter: {
       or: [
         {
           property: 'In stock',
           checkbox: {
@@ -1009,16 +1012,15 @@
         self._body = {'property': property_name, 'direction': direction}
 
 
 """
 EXPRESSION PARSING
 """
 
-
-if python_version < '3.8':
+if python_version_current < python_version_3_8:
     T_Union = Union[_ast.AST,
                     _ast.Expr,
                     _ast.Module,
                     _ast.BoolOp,
                     _ast.Or,
                     _ast.Compare,
                     _ast.Eq,
@@ -1164,15 +1166,15 @@
     'stmt': '',
     'type_ignore': '',
     'unaryop': '',
     'withitem': '',
 }
 
 # Replaced by 'Constant' since python 3.8
-if python_version < '3.8':
+if python_version_current < python_version_3_8:
     op_map['Num'] = ''
     op_map['Str'] = ''
     op_map['NameConstant'] = ''
     op_map['Assign'] = ''
 else:
     op_map['Constant'] = ''
```

### Comparing `notionizer-0.0.3/notionizer.egg-info/PKG-INFO` & `notionizer-0.0.4/notionizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notionizer
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python wrapper for Notion API
 Home-page: https://github.com/kimsg1984/notionizer
 Author: SeonGyo Kim
 Author-email: kimsg1984@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `notionizer-0.0.3/setup.py` & `notionizer-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = fh.read()
 
 reqs = parse_requirements("requirements.txt", session=False)
 install_requires = [str(ir.requirement) for ir in reqs]
 
 setuptools.setup(
     name="notionizer",
-    version="0.0.3",
+    version="0.0.4",
     author="SeonGyo Kim",
     author_email="kimsg1984@gmail.com",
     description="Python wrapper for Notion API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kimsg1984/notionizer",
     install_requires=install_requires,
```

