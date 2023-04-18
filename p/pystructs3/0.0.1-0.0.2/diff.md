# Comparing `tmp/pystructs3-0.0.1.tar.gz` & `tmp/pystructs3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystructs3-0.0.1.tar", last modified: Tue Apr 18 21:14:28 2023, max compression
+gzip compressed data, was "pystructs3-0.0.2.tar", last modified: Tue Apr 18 21:32:43 2023, max compression
```

## Comparing `pystructs3-0.0.1.tar` & `pystructs3-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:14:28.943255 pystructs3-0.0.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.1/LICENSE
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:14:28.943255 pystructs3-0.0.1/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.1/README.md
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:14:28.943255 pystructs3-0.0.1/pystructs/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      559 2023-04-18 07:09:08.000000 pystructs3-0.0.1/pystructs/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     7813 2023-04-18 20:55:01.000000 pystructs3-0.0.1/pystructs/base.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1762 2023-04-18 20:47:11.000000 pystructs3-0.0.1/pystructs/codec.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:14:28.943255 pystructs3-0.0.1/pystructs/struct/
--rw-r--r--   0 andrew    (1000) andrew    (1000)      310 2023-04-18 07:09:01.000000 pystructs3-0.0.1/pystructs/struct/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2994 2023-04-18 20:44:41.000000 pystructs3-0.0.1/pystructs/struct/fields.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4806 2023-04-18 20:53:05.000000 pystructs3-0.0.1/pystructs/struct/struct.py
-drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:14:28.943255 pystructs3-0.0.1/pystructs3.egg-info/
--rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:14:28.000000 pystructs3-0.0.1/pystructs3.egg-info/PKG-INFO
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      337 2023-04-18 21:14:28.000000 pystructs3-0.0.1/pystructs3.egg-info/SOURCES.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-18 21:14:28.000000 pystructs3-0.0.1/pystructs3.egg-info/dependency_links.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-18 21:14:28.000000 pystructs3-0.0.1/pystructs3.egg-info/requires.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-18 21:14:28.000000 pystructs3-0.0.1/pystructs3.egg-info/top_level.txt
--rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-18 21:14:28.943255 pystructs3-0.0.1/setup.cfg
--rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-18 21:10:22.000000 pystructs3-0.0.1/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.243517 pystructs3-0.0.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1075 2023-04-18 21:12:24.000000 pystructs3-0.0.2/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:32:43.243517 pystructs3-0.0.2/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      798 2023-04-18 21:13:45.000000 pystructs3-0.0.2/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.239517 pystructs3-0.0.2/pystructs/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      559 2023-04-18 07:09:08.000000 pystructs3-0.0.2/pystructs/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     7711 2023-04-18 21:28:14.000000 pystructs3-0.0.2/pystructs/base.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1792 2023-04-18 21:30:34.000000 pystructs3-0.0.2/pystructs/codec.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.239517 pystructs3-0.0.2/pystructs/struct/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      310 2023-04-18 07:09:01.000000 pystructs3-0.0.2/pystructs/struct/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3020 2023-04-18 21:30:44.000000 pystructs3-0.0.2/pystructs/struct/fields.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4806 2023-04-18 20:53:05.000000 pystructs3-0.0.2/pystructs/struct/struct.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-04-18 21:32:43.243517 pystructs3-0.0.2/pystructs3.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1277 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      337 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       30 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       10 2023-04-18 21:32:43.000000 pystructs3-0.0.2/pystructs3.egg-info/top_level.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-04-18 21:32:43.243517 pystructs3-0.0.2/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      763 2023-04-18 21:32:25.000000 pystructs3-0.0.2/setup.py
```

### Comparing `pystructs3-0.0.1/LICENSE` & `pystructs3-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.1/PKG-INFO` & `pystructs3-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.1/README.md` & `pystructs3-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.1/pystructs/__init__.py` & `pystructs3-0.0.2/pystructs/__init__.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.1/pystructs/base.py` & `pystructs3-0.0.2/pystructs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,35 +16,30 @@
     'SizedBytes',
     'StaticBytes',
     'Domain',
 ]
 
 #** Functions **#
 
-def singleton(cls: Type[Codec]):
-    """spawn singleton codec type"""
-    return cls()
-
-def codec(name: str, base: Type[Codec], **kwargs) -> Codec:
+def codec(name: str, base: Type[Codec], **kwargs) -> Type[Codec]:
     """spawn new singleton codec type"""
-    new_codec = type(name, (base, ), kwargs)
-    return new_codec()
+    return type(name, (base, ), kwargs)
 
 #** Classes **#
 
 class Const(Codec):
     """
     Bytes Constant to Inlcude in Serialized Data
     """
     size:      int
     init:      bool = False
     default:   bytes
     base_type: type
 
-    def __class_getitem__(cls, const: bytes) -> Codec:
+    def __class_getitem__(cls, const: bytes) -> Type[Codec]:
         """generate const type w/ given const"""
         name = cls.__name__
         return codec(f'{name}[{const!r}]', cls, 
             size=len(const), default=const, base_type=bytes)
 
     @classmethod
     def encode(cls, ctx: Context, value: bytes) -> bytes:
@@ -64,15 +59,15 @@
 
     Examples: Int[16], Int[32], Int[64, MyIntEnum]
     """
     size: ClassVar[int]
     wrap: ClassVar[Callable[[int], Any]]
     base_type: type
  
-    def __class_getitem__(cls, s: Union[int, tuple]) -> Codec:
+    def __class_getitem__(cls, s: Union[int, tuple]) -> Type[Codec]:
         """generate custom Int subclass with the given options"""
         size = s if isinstance(s, int) else s[0]
         wrap = s[1] if isinstance(s, tuple) and len(s) > 1 else lambda x: x
         name = s[2] if isinstance(s, tuple) and len(s) > 2 else cls.__name__
         assert size % 8 == 0, 'size must be multiple of eight'
         cname = f'{name}[{size}]'
         return codec(cname, cls, size=size // 8, wrap=wrap, base_type=int)
@@ -96,15 +91,15 @@
 
     Example: IpAddr['ipv4'] or IpAddr['ipv6']
     """
     size:      int
     ip_type:   Union[Type[IPv4Address], Type[IPv6Address]]
     base_type: Union[type, tuple] = (str, bytes)
 
-    def __class_getitem__(cls, iptype: str) -> Codec:
+    def __class_getitem__(cls, iptype: str) -> Type[Codec]:
         """generate ipv4 or ipv6 ipaddress supporting codec type"""
         assert iptype in ('ipv4', 'ipv6'), 'invalid ipaddress type'
         size = 4 if iptype == 'ipv4' else 16
         addr = IPv4Address if iptype == 'ipv4' else IPv6Address
         return codec(f'IPv{iptype[-1]}', cls, size=size, ip_type=addr)
 
     @classmethod
@@ -114,15 +109,14 @@
         return packed
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> Union[IPv4Address, IPv6Address]:
         data = ctx.slice(raw, cls.size)
         return cls.ip_type(data)
 
-@singleton
 class MacAddr(Codec):
     """
     Serialized MacAddress Codec
     """
     base_type: type       = str
     replace:   re.Pattern = re.compile('[:.-]')
   
@@ -141,15 +135,15 @@
     Variable Sized Bytes Codec with Length Denoted by Prefixed Integer
 
     Example: SizedBytes[32]
     """
     hint:      Codec
     base_type: type
  
-    def __class_getitem__(cls, hint: int) -> Codec:
+    def __class_getitem__(cls, hint: int) -> Type[Codec]:
         name   = cls.__name__
         hcodec = Int[hint]
         return codec(f'{name}[{hint!r}]', cls, hint=hcodec, base_type=bytes)
 
     @classmethod
     def encode(cls, ctx: Context, content: bytes) -> bytes:
         hint = cls.hint.encode(ctx, len(content))
@@ -166,30 +160,29 @@
     Variable Staticly Sized Bytes Codec of a Pre-Determined Length
 
     Example: StaticBytes[32]
     """
     size:      int
     base_type: type
 
-    def __class_getitem__(cls, size: int) -> Codec:
+    def __class_getitem__(cls, size: int) -> Type[Codec]:
         name = cls.__name__
         return codec(f'{name}[{size!r}]', cls, size=size, base_type=bytes)
 
     @classmethod
     def encode(cls, ctx: Context, content: bytes) -> bytes:
         assert len(content) <= cls.size, f'len(content) >= {cls.size} bytes'
         ctx.index += cls.size
         content = content.ljust(cls.size, b'\x00')
         return content
 
     @classmethod
     def decode(cls, ctx: Context, raw: bytes) -> bytes:
         return ctx.slice(raw, cls.size).rstrip(b'\x00')
 
-@singleton
 class Domain(Codec):
     """
     DNS Style Domain Serialization w/ Index Pointers to Eliminate Duplicates
     """
     ptr_mask:  int  = 0xC0
     base_type: type = bytes
```

### Comparing `pystructs3-0.0.1/pystructs/codec.py` & `pystructs3-0.0.2/pystructs/codec.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Base Codec Definitions
 """
 from abc import abstractmethod
 from dataclasses import dataclass, field
-from typing import Dict, Protocol, Any
+from typing import Dict, Protocol, Any, ClassVar
 from typing_extensions import runtime_checkable
 
 #** Variables **#
 __all__ = ['Context', 'Codec']
 
 #** Classes **#
 
@@ -44,16 +44,16 @@
         """
         self.index_to_domain[index] = domain
         self.domain_to_index[domain] = index
 
 @runtime_checkable
 class Codec(Protocol):
     """Encoding/Decoding Codec Protocol"""
-    init:      bool = True
-    default:   Any  = None
+    init:      ClassVar[bool] = True
+    default:   ClassVar[Any]  = None
     base_type: type
 
     @classmethod
     @abstractmethod
     def encode(cls, ctx: Context, value: Any) -> bytes:
         raise NotImplementedError
```

### Comparing `pystructs3-0.0.1/pystructs/struct/fields.py` & `pystructs3-0.0.2/pystructs/struct/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     def __class_getitem__(cls, hint: type) -> Self:
         return cls(hint)
 
 @dataclass
 class Field:
     name:     str
-    type:     Codec
+    type:     Type[Codec]
     init:     bool = True
     default:  Any  = None
     dataattr: bool = True
 
 @dataclass
 class Spec:
     default:         Any                         = MISSING
@@ -86,20 +86,20 @@
     init:            Optional[bool]              = None
     repr:            bool                        = True
     hash:            Optional[bool]              = None
     compare:         bool                        = True
     metadata:        Optional[Mapping[Any, Any]] = None
     kw_only:         bool                        = False
  
-    def compile(self, name: str, anno: Codec) -> Tuple[Field, DataField]:
+    def compile(self, name: str, anno: Type[Codec]) -> Tuple[Field, DataField]:
         """compile field-spec into official field"""
         init = anno.init if self.init is None else anno.init
         return (Field(name, anno, init), DataField(
             default=not_missing(self.default, anno.default),
-            default_factory=self.default_factory or MISSING,
+            default_factory=self.default_factory or MISSING, #type: ignore
             init=init,
             repr=self.repr,
             hash=self.hash,
             compare=self.compare,
             metadata=self.metadata or {},
             kw_only=self.kw_only,
         ))
```

### Comparing `pystructs3-0.0.1/pystructs/struct/struct.py` & `pystructs3-0.0.2/pystructs/struct/struct.py`

 * *Files identical despite different names*

### Comparing `pystructs3-0.0.1/pystructs3.egg-info/PKG-INFO` & `pystructs3-0.0.2/pystructs3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystructs3
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dataclass-Like Serialization Helpers for More Complex Data-Types
 Home-page: https://github.com/imgurbot12/pystruct
 Author: Andrew Scott
 Author-email: imgurbot12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pystructs3-0.0.1/setup.py` & `pystructs3-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 setup(
     name='pystructs3',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author='Andrew Scott',
     author_email='imgurbot12@gmail.com',
     url='https://github.com/imgurbot12/pystruct',
     description="Dataclass-Like Serialization Helpers for More Complex Data-Types",
     long_description=readme,
     long_description_content_type="text/markdown",
```

