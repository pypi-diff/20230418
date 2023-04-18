# Comparing `tmp/rf_userpoollibrary-0.8-py3-none-any.whl.zip` & `tmp/rf_userpoollibrary-0.9b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9923 bytes, number of entries: 9
--rw-rw-r--  2.0 unx    16834 b- defN 21-Apr-07 05:13 UserpoolLibrary/UserpoolLibrary.py
--rw-rw-r--  2.0 unx     1570 b- defN 21-Apr-07 05:13 UserpoolLibrary/Utils.py
--rw-rw-r--  2.0 unx     1166 b- defN 21-Apr-07 05:13 UserpoolLibrary/__init__.py
--rw-rw-r--  2.0 unx     1122 b- defN 21-Apr-07 05:13 UserpoolLibrary/version.py
--rw-rw-r--  2.0 unx     1072 b- defN 21-Apr-07 05:15 rf_userpoollibrary-0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2964 b- defN 21-Apr-07 05:15 rf_userpoollibrary-0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 21-Apr-07 05:15 rf_userpoollibrary-0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       16 b- defN 21-Apr-07 05:15 rf_userpoollibrary-0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      771 b- defN 21-Apr-07 05:15 rf_userpoollibrary-0.8.dist-info/RECORD
-9 files, 25607 bytes uncompressed, 8587 bytes compressed:  66.5%
+Zip file size: 10234 bytes, number of entries: 9
+-rw-r--r--  2.0 unx    18307 b- defN 23-Apr-18 15:53 UserpoolLibrary/UserpoolLibrary.py
+-rw-r--r--  2.0 unx     1570 b- defN 21-Feb-02 17:58 UserpoolLibrary/Utils.py
+-rw-r--r--  2.0 unx     1166 b- defN 21-Feb-02 17:58 UserpoolLibrary/__init__.py
+-rw-r--r--  2.0 unx     1124 b- defN 23-Apr-18 15:53 UserpoolLibrary/version.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-Apr-18 15:55 rf_userpoollibrary-0.9b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2966 b- defN 23-Apr-18 15:55 rf_userpoollibrary-0.9b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 15:55 rf_userpoollibrary-0.9b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Apr-18 15:55 rf_userpoollibrary-0.9b1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      781 b- defN 23-Apr-18 15:55 rf_userpoollibrary-0.9b1.dist-info/RECORD
+9 files, 27094 bytes uncompressed, 8878 bytes compressed:  67.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: UserpoolLibrary/__init__.py
 Comment: 
 
 Filename: UserpoolLibrary/version.py
 Comment: 
 
-Filename: rf_userpoollibrary-0.8.dist-info/LICENSE
+Filename: rf_userpoollibrary-0.9b1.dist-info/LICENSE
 Comment: 
 
-Filename: rf_userpoollibrary-0.8.dist-info/METADATA
+Filename: rf_userpoollibrary-0.9b1.dist-info/METADATA
 Comment: 
 
-Filename: rf_userpoollibrary-0.8.dist-info/WHEEL
+Filename: rf_userpoollibrary-0.9b1.dist-info/WHEEL
 Comment: 
 
-Filename: rf_userpoollibrary-0.8.dist-info/top_level.txt
+Filename: rf_userpoollibrary-0.9b1.dist-info/top_level.txt
 Comment: 
 
-Filename: rf_userpoollibrary-0.8.dist-info/RECORD
+Filename: rf_userpoollibrary-0.9b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## UserpoolLibrary/UserpoolLibrary.py

```diff
@@ -20,14 +20,15 @@
 
 import re
 import requests
 import logging
 import json
 import socket
 from os import environ
+from robot.api import logger
 from UserpoolLibrary.Utils import retry
 from UserpoolLibrary.version import VERSION
 
 from robotlibcore import (HybridCore,
                           keyword)
 
 __version__ = VERSION
@@ -92,14 +93,16 @@
     |             "currencyCode": "USD",
     |             "category": "CAT1,CAT2",
     |             "status": "ACTIVE",
     |             "email": "user@email.com",
     |             "mobileNo": "12345678910",
     |             "ip": "192.168.1.1",
     |             "hostName": "hostname",
+    |             "customField": "<key1>=<value1>,<key2>=<value2>",
+    |             "notes": "<string>"
     |             "modifiedDate": "2020-01-13T06:02:25.0850053Z"
     |           }
 
 
     - Borrow USER by ``currency_code``
     |               |               | =currency_code=   | =category=    |
     | ${user2}      | `Borrow User` | RMB               |               |
@@ -112,14 +115,16 @@
     |             "currencyCode": "RMB",
     |             "category": "CAT1,CAT2,CAT3",
     |             "status": "ACTIVE",
     |             "email": "user@email.com",
     |             "mobileNo": "12345678910",
     |             "ip": "192.168.1.1",
     |             "hostName": "hostname",
+    |             "customField": "<key1>=<value1>,<key2>=<value2>",
+    |             "notes": "<string>"
     |             "modifiedDate": "2020-01-13T06:02:25.0850053Z"
     |           }
 
 
     - Borrow User by ``currency_code`` and ``category``
     | ${user3}      | `Borrow User` | RMB               | CAT1          |
     | `Return User` | ${user}       |                   |               |
@@ -130,14 +135,16 @@
     |             "passWord": "sample_password,
     |             "currencyCode": "RMB",
     |             "category": "CAT1,CAT2,CAT3",
     |             "status": "ACTIVE",
     |             "email": "user@email.com",
     |             "mobileNo": "12345678910",
     |             "ip": "192.168.1.1",
+    |             "customField": "<key1>=<value1>,<key2>=<value2>",
+    |             "notes": "<string>"
     |             "hostName": "hostname",
     |             "modifiedDate": "2020-01-13T06:02:25.0850053Z"
     |           }
 
 
     - Borrow User by ``category``
     | ${user4}      | `Borrow User` | ${EMPTY}          | CAT1          |
@@ -150,14 +157,16 @@
     |             "currencyCode": "IDR",
     |             "category": "CAT1,CAT2",
     |             "status": "ACTIVE",
     |             "email": "user@email.com",
     |             "mobileNo": "12345678910",
     |             "ip": "192.168.1.1",
     |             "hostName": "hostname",
+    |             "customField": "<key1>=<value1>,<key2>=<value2>",
+    |             "notes": "<string>"
     |             "modifiedDate": "2020-01-13T06:02:25.0850053Z"
     |           }
 
     = Borrowed User Object =
 
     Borrow User returns a json object containing the following information:
     | =Attribute=           | =Type=    | =Description=                 |
@@ -184,14 +193,16 @@
     |   "currencyCode": "PHP",
     |   "category": "NORMAL",
     |   "status": "ACTIVE",
     |   "email": "user@email.com",
     |   "mobileNo": "12345678910",
     |   "ip": "192.168.1.1",
     |   "hostName": "hostname",
+    |   "customField": "<key1>=<value1>,<key2>=<value2>",
+    |   "notes": "<string>"
     |   "modifiedDate": "2020-01-13T06:02:25.0850053Z"
     | }
 
     == Accessing User Data ==
 
     The borrowed user data can be accessed by using either the dot(.) \
         syntax or by invoking the key inside a square bracket(['key']).
@@ -355,24 +366,43 @@
         |           }
         | ${count} = 1
         """
         user_id = user['id']
 
         return self._update_user_profile(user_id, email, mobileNo)
 
+    def _parse_custom_field(self, user):
+        """
+        Parses the custom field from the returned user of the userpool.
+
+        The custom field must be a comma separated values following this format:
+        format: "<key1>=<value1>,<key2>=<value2>"
+        """
+        parsedCustomField = user
+        # del parsedCustomField['customField']
+        if user['customField'] is not None:
+            keyValues = user['customField'].split(',')
+            for keyValue in keyValues:
+                if '=' in keyValue:
+                    value = keyValue.split('=')
+                    parsedCustomField[value[0]] = value[1]
+                else:
+                    logger.info(f'{keyValue} is an invalid value')
+            logger.info(parsedCustomField)
+        return parsedCustomField
+
     def _get_free_user(self, currency_code=None, category=None):
         request_url = self.base_url + "/borrow/single"
 
         LOGGER.info(f'Retrying user')
 
         params = {'currencyCode': '',
                   'category': '',
                   'ip': self.machineIp,
                   'hostName': self.machineHostName}
-
         if currency_code:
             params.update({"currencyCode": currency_code})
         if category:
             category = (category.replace(' ', '')).split(',')
             params.update({"category": category})
 
         LOGGER.debug(f'Params {params}')
@@ -380,15 +410,17 @@
         response = requests.get(request_url, params=params)
         response.raise_for_status()
 
         json_response = response.json()
         LOGGER.debug(f'Retrieved free user {json_response}')
 
         if bool(json_response):
-            return json_response
+            logger.info(json_response)
+            user = self._parse_custom_field(json_response)
+            return user
 
         raise Exception('No user found')
 
     def _free_user(self, user_id):
         request_url = self.base_url + "/return/single/" + str(user_id)
 
         response = requests.post(request_url)
@@ -439,15 +471,16 @@
         response = requests.get(request_url)
         response.raise_for_status()
 
         json_response = response.json()
         LOGGER.debug(f'Retrieved free user {json_response}')
 
         if bool(response):
-            return json_response
+            user = self._parse_custom_field(json_response)
+            return user
 
         return None
 
     def _get_machine_hostname(self):
         """Uses python 3 socket library to get the machine IP and hostname.
         """
         try:
```

## UserpoolLibrary/version.py

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = '0.8'
+VERSION = '0.9b1'
```

## Comparing `rf_userpoollibrary-0.8.dist-info/LICENSE` & `rf_userpoollibrary-0.9b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rf_userpoollibrary-0.8.dist-info/METADATA` & `rf_userpoollibrary-0.9b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rf-userpoollibrary
-Version: 0.8
+Version: 0.9b1
 Summary: Test Library for userpool support.
 Home-page: https://github.com/MainSystemDev/UserpoolLibrary
 Author: Shiela Buitizon
 Author-email: shiela.buitizon@mnltechnology.com
 License: Type license() to see the full license text
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `rf_userpoollibrary-0.8.dist-info/RECORD` & `rf_userpoollibrary-0.9b1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-UserpoolLibrary/UserpoolLibrary.py,sha256=CkOuCgrllRpjGm6Yutl8pNEYaxLPeZaDb6loyRKEe0E,16834
+UserpoolLibrary/UserpoolLibrary.py,sha256=juMjbv8zIuGVJ4D50Gjrfj0-aprcGUefx-0uu3MSK6A,18307
 UserpoolLibrary/Utils.py,sha256=OQia_7Jgrj8V4k9EuNq9Q9qWAiBNGaY9p9VQ4J2P1mo,1570
 UserpoolLibrary/__init__.py,sha256=IRx_z-c0GrfZk3XgQUWG2B7ZMgjW9Qvf94e_C_2UXls,1166
-UserpoolLibrary/version.py,sha256=tfZLUKRv4_6-xtb1oqgmdynHPqgzfcerO-sRZYmsRao,1122
-rf_userpoollibrary-0.8.dist-info/LICENSE,sha256=OjWkSK0ve0yCXLlsw-7TTfFJMorgICeKeGRyICPvjdI,1072
-rf_userpoollibrary-0.8.dist-info/METADATA,sha256=-pGF34OMi8xuA5N_q4Y8CdgerJga7sdTYBRg8l16pvE,2964
-rf_userpoollibrary-0.8.dist-info/WHEEL,sha256=p46_5Uhzqz6AzeSosiOnxK-zmFja1i22CrQCjmYe8ec,92
-rf_userpoollibrary-0.8.dist-info/top_level.txt,sha256=1fE9zy8Vz-vNjh1mQYMX8EZwKWk-r3ngWzS1v7J1NoU,16
-rf_userpoollibrary-0.8.dist-info/RECORD,,
+UserpoolLibrary/version.py,sha256=-pp7f5tiFfxNEjlT9DWRQIHO_RYthcwOGJJjX9jqQnE,1124
+rf_userpoollibrary-0.9b1.dist-info/LICENSE,sha256=OjWkSK0ve0yCXLlsw-7TTfFJMorgICeKeGRyICPvjdI,1072
+rf_userpoollibrary-0.9b1.dist-info/METADATA,sha256=bNALYj_2l7oq6Sdulo0s7_r68b3id_bH0QD2TLgFb8c,2966
+rf_userpoollibrary-0.9b1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rf_userpoollibrary-0.9b1.dist-info/top_level.txt,sha256=1fE9zy8Vz-vNjh1mQYMX8EZwKWk-r3ngWzS1v7J1NoU,16
+rf_userpoollibrary-0.9b1.dist-info/RECORD,,
```

