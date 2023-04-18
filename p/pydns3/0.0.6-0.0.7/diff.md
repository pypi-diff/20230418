# Comparing `tmp/pydns3-0.0.6.tar.gz` & `tmp/pydns3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydns3-0.0.6.tar", last modified: Thu Mar 30 08:50:07 2023, max compression
+gzip compressed data, was "pydns3-0.0.7.tar", last modified: Tue Apr 18 21:34:59 2023, max compression
```

## Comparing `pydns3-0.0.6.tar` & `pydns3-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,36 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-03-30 08:50:07.731953 pydns3-0.0.6/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      243 2023-03-26 23:42:47.000000 pydns3-0.0.6/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.727953 pydns3-0.0.6/pydns/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      562 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2930 2023-03-29 22:18:25.000000 pydns3-0.0.6/pydns/answer.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/client/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1173 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/client/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1073 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/client/https.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3070 2023-03-29 22:16:54.000000 pydns3-0.0.6/pydns/client/standard.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/codec/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      719 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/codec/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5991 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/codec/base.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/codec/sequence/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      291 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/codec/sequence/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1231 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/codec/sequence/fields.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     3886 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/codec/sequence/sequence.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2152 2023-03-30 05:42:51.000000 pydns3-0.0.6/pydns/content.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/edns/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      197 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/edns/__init__.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1414 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/edns/record.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2591 2023-03-29 22:05:52.000000 pydns3-0.0.6/pydns/enum.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1406 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/exceptions.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2107 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/flags.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     4182 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/message.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      383 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/question.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/server/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      132 2023-03-26 23:42:47.000000 pydns3-0.0.6/pydns/server/__init__.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns/server/backend/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      994 2023-03-30 07:56:17.000000 pydns3-0.0.6/pydns/server/backend/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     5293 2023-03-30 08:28:49.000000 pydns3-0.0.6/pydns/server/backend/blacklist.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4062 2023-03-30 07:56:43.000000 pydns3-0.0.6/pydns/server/backend/cache.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1278 2023-03-30 07:26:09.000000 pydns3-0.0.6/pydns/server/backend/forwarder.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     2647 2023-03-30 08:23:38.000000 pydns3-0.0.6/pydns/server/backend/memory.py
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     5159 2023-03-29 00:23:06.000000 pydns3-0.0.6/pydns/server/server.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-30 08:50:07.731953 pydns3-0.0.6/pydns3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-03-30 08:50:07.000000 pydns3-0.0.6/pydns3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      769 2023-03-30 08:50:07.000000 pydns3-0.0.6/pydns3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-30 08:50:07.000000 pydns3-0.0.6/pydns3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       47 2023-03-30 08:50:07.000000 pydns3-0.0.6/pydns3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-03-30 08:50:07.000000 pydns3-0.0.6/pydns3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-03-30 08:50:07.731953 pydns3-0.0.6/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      791 2023-03-30 08:04:51.000000 pydns3-0.0.6/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-04-18 21:34:59.377124 pydns3-0.0.7/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      243 2023-03-26 23:42:47.000000 pydns3-0.0.7/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      562 2023-04-18 21:16:11.000000 pydns3-0.0.7/pydns/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2967 2023-04-18 21:26:07.000000 pydns3-0.0.7/pydns/answer.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/client/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1173 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/client/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1073 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/client/https.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3070 2023-03-29 22:16:54.000000 pydns3-0.0.7/pydns/client/standard.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2388 2023-04-18 21:26:19.000000 pydns3-0.0.7/pydns/content.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/edns/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      197 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/edns/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1450 2023-04-18 21:10:55.000000 pydns3-0.0.7/pydns/edns/record.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2591 2023-03-29 22:05:52.000000 pydns3-0.0.7/pydns/enum.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1406 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/exceptions.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2107 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/flags.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4206 2023-04-18 21:11:10.000000 pydns3-0.0.7/pydns/message.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      398 2023-04-18 21:11:13.000000 pydns3-0.0.7/pydns/question.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/server/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      132 2023-03-26 23:42:47.000000 pydns3-0.0.7/pydns/server/__init__.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns/server/backend/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      994 2023-03-30 07:56:17.000000 pydns3-0.0.7/pydns/server/backend/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     5293 2023-03-30 08:28:49.000000 pydns3-0.0.7/pydns/server/backend/blacklist.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4062 2023-03-30 07:56:43.000000 pydns3-0.0.7/pydns/server/backend/cache.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1278 2023-03-30 07:26:09.000000 pydns3-0.0.7/pydns/server/backend/forwarder.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2647 2023-03-30 08:23:38.000000 pydns3-0.0.7/pydns/server/backend/memory.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5159 2023-03-29 00:23:06.000000 pydns3-0.0.7/pydns/server/server.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:34:59.377124 pydns3-0.0.7/pydns3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      688 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      628 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       58 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        6 2023-04-18 21:34:59.000000 pydns3-0.0.7/pydns3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-18 21:34:59.377124 pydns3-0.0.7/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      813 2023-04-18 21:34:36.000000 pydns3-0.0.7/setup.py
```

### Comparing `pydns3-0.0.6/PKG-INFO` & `pydns3-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydns3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Python DNS Library. DNS Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydns
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydns3-0.0.6/pydns/__init__.py` & `pydns3-0.0.7/pydns/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/answer.py` & `pydns3-0.0.7/pydns/answer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 DNS Answer Record Instance/Format
 """
 from typing import Optional, Type
 from abc import abstractmethod
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Protocol
 from typing_extensions import Self
 
-from .codec import *
+from pystructs import Context, Domain, Int, Int16, Int32, struct
+
 from .content import Content, Literal
 from .enum import RType, RClass
 from . import content
 
 #** Variables **#
 __all__ = ['BaseAnswer', 'Answer', 'PreRequisite', 'Update']
 
@@ -31,15 +32,15 @@
     # else just encapsulate in sized-bytes object
     if size is not None:
         return Literal[rtype, size]
     raise ValueError(f'unsupported rtype: {rtype.name!r}')
 
 #** Classes **#
 
-@make_sequence
+@struct
 class Header:
     name:   Domain
     rtype:  Int[16, RType, 'RType']
     rclass: Int[16, RClass, 'RClass']
     ttl:    Int32
 
 class BaseAnswer(Protocol):
@@ -89,12 +90,12 @@
         content = rclass.decode(ctx, raw)
         return cls(header.name, header.ttl, content, header.rclass)
 
 @dataclass
 class PreRequisite(Answer):
     """Alias for Answer in UPDATE action DNS Requests with Sensible Defaults"""
     ttl:     int = 0
-    content: Content = field(default_factory=content.ANY)
+    content: Content = field(default=content.ANY)
 
 class Update(Answer):
     """Alias of Answer in UPDATE action DNS Requests"""
     pass
```

### Comparing `pydns3-0.0.6/pydns/client/__init__.py` & `pydns3-0.0.7/pydns/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/client/https.py` & `pydns3-0.0.7/pydns/client/https.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/client/standard.py` & `pydns3-0.0.7/pydns/client/standard.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/content.py` & `pydns3-0.0.7/pydns/content.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 DNS Standard Content Sequences
 """
-from typing import Optional, Type, Tuple
+from typing import Optional, Type, Tuple, ClassVar, Any
 from typing_extensions import Self
 
-from .codec import *
+from pystructs import *
+
 from .enum import RType
 
 #** Variables **#
 __all__ = [
     'NULL',
     'ANY',
     'CNAME',
@@ -20,26 +21,34 @@
     'A',
     'AAAA',
     'SRV',
 ]
 
 #** Functions **#
 
-def content(cls: Optional[type] = None, rtype: Optional[RType] = None):
+def content(cls: Optional[type] = None, rtype: Optional[RType] = None) -> 'Content':
     """generate content class w/ given rtype"""
     def wrapper(cls):
         cls.rtype = rtype or RType[cls.__name__] 
-        return make_sequence(cls)
-    return wrapper if cls is None else wrapper(cls)
+        return make_struct(cls)
+    return wrapper if cls is None else wrapper(cls) #type: ignore
 
 #** Classes **#
 
-class Content(Sequence):
+class Content:
     rtype: ClassVar[RType]
 
+    @classmethod
+    def encode(cls, ctx: Context) -> bytes:
+        raise NotImplementedError
+
+    @classmethod
+    def decode(cls, ctx: Context, raw: bytes) -> Any:
+        raise NotImplementedError
+
 @content
 class NULL(Content):
     pass
 
 @content
 class ANY(Content):
     pass
```

### Comparing `pydns3-0.0.6/pydns/edns/record.py` & `pydns3-0.0.7/pydns/edns/record.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 EDNS OPT Answer Varient Implementation
 """
 from dataclasses import dataclass
 from typing_extensions import Self
 
-from ..codec import *
+from pystructs import Context, Domain, Int, Int8, Int16, struct
+
 from ..enum import RType
 from ..answer import BaseAnswer
 
 #** Variables **#
 __all__ = ['ROOT', 'EdnsAnswer']
 
 #: root domain (according to EDNS)
 ROOT = b''
 
 #** Classes **#
 
-@make_sequence
+@struct
 class Header:
     name:           Domain
     rtype:          Int[16, RType, 'RType']
     payload_size:   Int16
     extended_rcode: Int8
     version:        Int8
     z:              Int16
```

### Comparing `pydns3-0.0.6/pydns/enum.py` & `pydns3-0.0.7/pydns/enum.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/exceptions.py` & `pydns3-0.0.7/pydns/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/flags.py` & `pydns3-0.0.7/pydns/flags.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/message.py` & `pydns3-0.0.7/pydns/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 DNS Message Object
 """
 from typing import List
 from dataclasses import dataclass, field
 from typing import Type
 from typing_extensions import Self
 
-from .codec import *
+from pystructs import Context, Domain, Int, Int16, struct
+
 from .enum import OpCode, RType, RCode
 from .flags import Flags
 from .answer import BaseAnswer, Answer, PreRequisite, Update
 from .question import Question, Zone
 from .edns import EdnsAnswer
 from .exceptions import make_error
 
@@ -43,20 +44,20 @@
         # decode answer class accordingly
         new = newcls.decode(ctx, raw)
         objects.append(new)
     return objects
 
 #** Classes **#
 
-@make_sequence
+@struct
 class PeekHeader:
     name:  Domain
     rtype: Int[16, RType, 'RType']
 
-@make_sequence
+@struct
 class Header:
     id:             Int16
     flags:          Int16 
     num_questions:  Int16
     num_answers:    Int16
     num_authority:  Int16
     num_additional: Int16
```

### Comparing `pydns3-0.0.6/pydns/server/backend/__init__.py` & `pydns3-0.0.7/pydns/server/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/server/backend/blacklist.py` & `pydns3-0.0.7/pydns/server/backend/blacklist.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/server/backend/cache.py` & `pydns3-0.0.7/pydns/server/backend/cache.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/server/backend/forwarder.py` & `pydns3-0.0.7/pydns/server/backend/forwarder.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/server/backend/memory.py` & `pydns3-0.0.7/pydns/server/backend/memory.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns/server/server.py` & `pydns3-0.0.7/pydns/server/server.py`

 * *Files identical despite different names*

### Comparing `pydns3-0.0.6/pydns3.egg-info/PKG-INFO` & `pydns3-0.0.7/pydns3.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydns3
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple Python DNS Library. DNS Packet-Parsing/Client/Server
 Home-page: https://github.com/imgurbot12/pydns
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pydns3-0.0.6/setup.py` & `pydns3-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
     name='pydns3',
-    version='0.0.6',
+    version='0.0.7',
     license='MIT',
     packages=find_packages(),
     url='https://github.com/imgurbot12/pydns',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     description='Simple Python DNS Library. DNS Packet-Parsing/Client/Server',
     python_requires='>=3.7',
     long_description=readme,
     long_description_content_type="text/markdown",
     install_requires=[
         'pypool3',
         'pyserve3',
+        'pystructs3',
         'dataclasses',
         'typing_extensions',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

