# Comparing `tmp/aioxnat-0.0.4.tar.gz` & `tmp/aioxnat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioxnat-0.0.4.tar", last modified: Wed Apr  5 18:59:15 2023, max compression
+gzip compressed data, was "aioxnat-0.0.5.tar", last modified: Tue Apr 18 13:44:21 2023, max compression
```

## Comparing `aioxnat-0.0.4.tar` & `aioxnat-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:15.432974 aioxnat-0.0.4/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-01 23:22:46.000000 aioxnat-0.0.4/LICENSE.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      441 2023-04-05 18:59:15.432974 aioxnat-0.0.4/PKG-INFO
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:15.432974 aioxnat-0.0.4/aioxnat/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      220 2023-04-02 01:16:57.000000 aioxnat-0.0.4/aioxnat/__init__.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     8585 2023-04-02 00:56:56.000000 aioxnat-0.0.4/aioxnat/objects.py
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)    10691 2023-04-05 18:34:38.000000 aioxnat-0.0.4/aioxnat/rest.py
-drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-05 18:59:15.432974 aioxnat-0.0.4/aioxnat.egg-info/
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      441 2023-04-05 18:59:15.000000 aioxnat-0.0.4/aioxnat.egg-info/PKG-INFO
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      229 2023-04-05 18:59:15.000000 aioxnat-0.0.4/aioxnat.egg-info/SOURCES.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-05 18:59:15.000000 aioxnat-0.0.4/aioxnat.egg-info/dependency_links.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       14 2023-04-05 18:59:15.000000 aioxnat-0.0.4/aioxnat.egg-info/requires.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-05 18:59:15.000000 aioxnat-0.0.4/aioxnat.egg-info/top_level.txt
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-05 18:59:15.432974 aioxnat-0.0.4/setup.cfg
--rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      884 2023-04-05 18:57:18.000000 aioxnat-0.0.4/setup.py
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-18 13:44:21.834761 aioxnat-0.0.5/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     1067 2023-04-01 23:22:46.000000 aioxnat-0.0.5/LICENSE.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      400 2023-04-18 13:44:21.834761 aioxnat-0.0.5/PKG-INFO
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-18 13:44:21.834761 aioxnat-0.0.5/aioxnat/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      410 2023-04-18 13:39:44.000000 aioxnat-0.0.5/aioxnat/__init__.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     5880 2023-04-17 21:13:22.000000 aioxnat-0.0.5/aioxnat/objects.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     6758 2023-04-17 18:53:33.000000 aioxnat-0.0.5/aioxnat/protocols.py
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)     7392 2023-04-18 13:35:52.000000 aioxnat-0.0.5/aioxnat/rest.py
+drwxrwxr-x   0 kwilkinson  (1000) kwilkinson  (1000)        0 2023-04-18 13:44:21.834761 aioxnat-0.0.5/aioxnat.egg-info/
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      400 2023-04-18 13:44:21.000000 aioxnat-0.0.5/aioxnat.egg-info/PKG-INFO
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      256 2023-04-18 13:44:21.000000 aioxnat-0.0.5/aioxnat.egg-info/SOURCES.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        1 2023-04-18 13:44:21.000000 aioxnat-0.0.5/aioxnat.egg-info/dependency_links.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       14 2023-04-18 13:44:21.000000 aioxnat-0.0.5/aioxnat.egg-info/requires.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)        8 2023-04-18 13:44:21.000000 aioxnat-0.0.5/aioxnat.egg-info/top_level.txt
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)      678 2023-04-17 14:47:52.000000 aioxnat-0.0.5/pyproject.toml
+-rw-rw-r--   0 kwilkinson  (1000) kwilkinson  (1000)       38 2023-04-18 13:44:21.834761 aioxnat-0.0.5/setup.cfg
```

### Comparing `aioxnat-0.0.4/LICENSE.txt` & `aioxnat-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioxnat-0.0.4/aioxnat/objects.py` & `aioxnat-0.0.5/aioxnat/objects.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,46 @@
 import dataclasses, enum, functools, re, pathlib
-import abc, typing
+import typing
 
-Ps = typing.ParamSpec("Ps")
-Ta = typing.TypeVar("Ta")
+from aioxnat.protocols import *
 
-GenericTypeFactory = (
-    typing.Callable[[type[Ta]], Ta] |
-    typing.Callable[typing.Concatenate[type[Ta], Ps], Ta])
-"""
-Outline of callable which produces an object of
-the given type.
-"""
+project_object_dataclass = dataclasses.dataclass(slots=True, frozen=True)
 
-Validator = (
-    typing.Callable[[Ta], bool] |
-    typing.Callable[typing.Concatenate[Ta, Ps], bool])
-"""
-Callable returning whether object passes
-validation.
-"""
 
 @typing.overload
-def validator(**params) -> Validator:
+def validator(**params) -> _Validator:
     ...
 
 
 @typing.overload
-def validator(vfn: Validator, /) -> Validator:
+def validator(vfn: _Validator, /) -> _Validator:
     ...
 
 
-def validator(vfn: Validator | None = None, **params):
+def validator(vfn: _Validator | None = None, **params):
     """
     Marks some callable as a validator function.
     """
 
-    def wrapper(vfn: Validator):
+    def wrapper(vfn: _Validator):
 
         @functools.wraps(vfn)
         def inner(*args, **kwds):
             return vfn(*args, **kwds)
 
         ret = functools.partial(inner, **params)
         setattr(ret, "__is_validator__", True)
         return ret
 
     if vfn:
         return wrapper(vfn)
     return wrapper
 
 
-def isvalidator(vfn: typing.Callable) -> bool:
-    """
-    Whether this callable is a validator.
-    """
-
-    return (callable(vfn) and getattr(vfn, "__is_validator__", False))
-
-
-def members(enumt: type[enum.StrEnum]):
+def _members(enumt: type[enum.StrEnum]):
     return enumt.__members__
 
 
 class ScanQuality(enum.StrEnum):
     USABLE = enum.auto()
     GOOD = enum.auto()
     FAIR = enum.auto()
@@ -76,95 +54,14 @@
     UNKNOWN = enum.auto()
 
 
 class ScanTaskType(enum.StrEnum):
     UNKNOWN = enum.auto()
 
 
-@typing.runtime_checkable
-class ProjectObject(typing.Protocol):
-    """
-    An element in the heirarchy of an XNAT
-    project.
-    """
-
-    __validators__: typing.Iterable[Validator[typing.Self, Ps]] = () #type: ignore[valid-type]
-
-    @functools.cached_property
-    def is_valid(self):
-        """
-        Whether or not this `ProjectObject` is
-        valid according to it's validators.
-        """
-
-        return all([vfn(self) for vfn in self.__validators__])
-
-    @property
-    @abc.abstractmethod
-    def name(self) -> str:
-        """
-        The name associated with this object.
-        """
-
-    @abc.abstractmethod
-    def into_mapping(self) -> typing.Mapping[str, str]:
-        """
-        Transforms this object into a mapping of
-        it's values.
-        """
-
-    @classmethod
-    @abc.abstractmethod
-    def from_mapping(cls, mapping: typing.Mapping[str, str]) -> typing.Self:
-        """
-        Transforms the given mapping into a this
-        `ProjectObject` type.
-        """
-
-    @classmethod
-    def insert_validator(cls, vfn: Validator[typing.Self, Ps]) -> None:
-        """
-        Inserts a validator into this object's
-        series of validators.
-        """
-
-        tmp = set(cls.__validators__)
-        if vfn in tmp:
-            raise ValueError("validator already included.")
-
-        tmp.add(vfn) #type: ignore[arg-type]
-        cls.__validators__ = tuple(tmp)
-
-    @classmethod
-    def remove_validator(cls, vfn: Validator[typing.Self, Ps]) -> None:
-        """
-        Removes a validator from the series of
-        validators.
-        """
-
-        tmp = set(cls.__validators__)
-        if vfn not in tmp:
-            raise ValueError("validator not in validators.")
-
-        tmp.remove(vfn) #type: ignore[arg-type]
-        cls.__validators__ = tuple(tmp)
-
-    def __init_subclass__(cls):
-        # Find and 'register' validators.
-        for name in dir(cls):
-            attr = getattr(cls, name, None)
-            if not (attr and isvalidator(attr)):
-                continue
-
-            try:
-                cls.insert_validator(attr)
-            except ValueError:
-                ... # validator already inserted.
-
-
 class BaseExperiment(ProjectObject):
     id: str
     label: str
     project: str
 
     @functools.cached_property
     def session_number(self): #NOTE: might be HCP specific.
@@ -185,15 +82,15 @@
         return cls(**parsed)
 
     @validator
     def _valid_id(self):
         return bool(re.match(r".*[a-zA-Z0-9].*", self.id))
 
 
-@dataclasses.dataclass(slots=True, frozen=True)
+@project_object_dataclass
 class Experiment(BaseExperiment):
     id: str
     xsiType: str
     subject_id: str
     project: str
     label: str
     URI: str
@@ -214,30 +111,30 @@
     @functools.cached_property
     def subtype(self) -> enum.StrEnum:
         """
         Associated purpose of this scan in
         addition to the task type.
         """
 
-        pattern = r"^.*_(%s).*$" % r"|".join(members(self.__subtype_enum__).values())
+        pattern = r"^.*_(%s).*$" % r"|".join(_members(self.__subtype_enum__).values())
         tmp = re.findall(pattern, self.series_description)
 
         try:
             return self.__subtype_enum__(tmp[0])
         except IndexError:
             return self.__subtype_enum__("UNKNOWN")
 
     @functools.cached_property
     def task(self) -> enum.StrEnum:
         """
         Associated task or purpose for which this
         scan was taken.
         """
 
-        pattern = r"^.*(%s).*$" % r"|".join(members(self.__tasktype_enum__).values())
+        pattern = r"^.*(%s).*$" % r"|".join(_members(self.__tasktype_enum__).values())
         tmp = re.findall(pattern, self.series_description)
 
         try:
             return self.__tasktype_enum__(tmp[0])
         except IndexError:
             return self.__tasktype_enum__("UNKNOWN")
 
@@ -255,38 +152,38 @@
 
     def set_subtypes(self, enumt: type[enum.StrEnum]):
         """
         Sets the enumerator used to identify what
         the sub type of the scan could be.
         """
 
-        if "UNKNOWN" not in members(enumt):
+        if "UNKNOWN" not in _members(enumt):
             raise AttributeError("Enum type must have member 'UNKNOWN'.")
         self.__subtype_enum__ = enumt
 
     def set_tasktypes(self, enumt: type[enum.StrEnum]):
         """
         Sets the enumerator used to identify what
         the task type could be.
         """
 
-        if "UNKNOWN" not in members(enumt):
+        if "UNKNOWN" not in _members(enumt):
             raise AttributeError("Enum type must have member 'UNKNOWN'.")
         self.__tasktype_enum__ = enumt
 
     @validator
     def _valid_subtype(self):
         return (self.subtype.value != "UNKNOWN")
 
     @validator
     def _valid_tasktype(self):
         return (self.task.value != "UNKNOWN")
 
 
-@dataclasses.dataclass(slots=True, frozen=True)
+@project_object_dataclass
 class Scan(BaseScan):
     id: str
     data_type: str
     series_description: str
     quality: ScanQuality
     URI: str
     experiment: Experiment
@@ -314,26 +211,26 @@
         parsed["format"] = parsed.pop("file_format", "")
         parsed["size"] = parsed.pop("Size", "")
         parsed["tags"] = parsed.pop("file_tags", "")
 
         return cls(**parsed)
 
 
-@dataclasses.dataclass(slots=True, frozen=True)
+@project_object_dataclass
 class FileData(BaseFileData):
     content: str
     size: str
     tags: str | tuple[str]
     cat_id: str
     digest: str
     collection: str
     format: str
     URI: str
 
 
-ExperimentFactory = GenericTypeFactory[Experiment, Ps]
+ExperimentFactory = _GenericTypeFactory[Experiment, Ps]
 """
 Callable which produces an `Experiment` object.
 """
 
-ScanFactory = GenericTypeFactory[Scan, Ps]
+ScanFactory = _GenericTypeFactory[Scan, Ps]
 """Callable which produces a `Scan` object."""
```

