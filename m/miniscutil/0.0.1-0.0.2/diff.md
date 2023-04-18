# Comparing `tmp/miniscutil-0.0.1.tar.gz` & `tmp/miniscutil-0.0.2.tar.gz`

## Comparing `miniscutil-0.0.1.tar` & `miniscutil-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,29 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/__about__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/__init__.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/adapt.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/deepeq.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/dispatch.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/misc.py
--rw-r--r--   0        0        0     9452 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/sum.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 miniscutil-0.0.1/miniscutil/type_util.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_classdispatch.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_deepeq.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_humansize.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_ofdict.py
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/test_typing.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.0.1/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.0.1/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 miniscutil-0.0.1/README.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 miniscutil-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 miniscutil-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/__about__.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/misc.py
+-rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.0.2/miniscutil/type_util.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_humansize.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.0.2/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 miniscutil-0.0.2/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 miniscutil-0.0.2/PKG-INFO
```

### Comparing `miniscutil-0.0.1/miniscutil/adapt.py` & `miniscutil-0.0.2/miniscutil/adapt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import defaultdict
 from contextvars import ContextVar
 import datetime
 from enum import Enum
 from functools import singledispatch
-from typing import Any, Callable, Type, get_origin
+from typing import Any, Callable, NewType, Type, get_origin
 import uuid
 
 from .dispatch import Dispatcher, classdispatch
-from .type_util import as_optional
+from .type_util import as_newtype, as_optional
 
 """ Implementation of PEP-246 https://peps.python.org/pep-0246/#specification
 
 I'm not sure it quite captures the spirit of the PEP because adapt doesn't necessarily _wrap_ the input.
 """
 
 
@@ -79,14 +79,19 @@
     Y = as_optional(X)
     if Y is not None:
         if x is None:
             return x
         else:
             return restore(Y, x)
 
+    S = as_newtype(X)
+    if S is not None:
+        r = restore(S, x)
+        return X(r)
+
     if get_origin(X) is None and isinstance(x, X):
         return x
     adapt = getattr(X, "__adapt__", None)
     if adapt is not None:
         r = adapt(x)
         if r is not NotImplemented:
             return r
```

### Comparing `miniscutil-0.0.1/miniscutil/asyncio_helpers.py` & `miniscutil-0.0.2/miniscutil/asyncio_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Callable,
     Coroutine,
     Generic,
     Iterable,
     Iterator,
     Optional,
     TypeVar,
+    Union,
 )
 import concurrent.futures
 import os
 import sys
 import time
 
 T = TypeVar("T")
@@ -83,15 +84,23 @@
         self._items.extend(items)
         if len(self) > 0:
             self._event.set()
 
     def __len__(self):
         return len(self._items)
 
-    async def pop_many(self, limit=None):
+    def tolist(self):
+        return list(self._items)
+
+    async def wait_pop_many(self, limit=None):
+        """Waits for at least one element to be in the queue and returns the whole queue.
+
+        Args:
+            limit(int | None): If an integer, will never return more than that many items.
+        """
         if len(self._items) == 0:
             await self._event.wait()
         assert len(self._items) > 0
         if (limit is None) or (0 < len(self._items) <= limit):
             result = list(self._items)
             self._items.clear()
         else:
@@ -99,24 +108,29 @@
             result = []
             while len(result) < limit:
                 result.append(self._items.popleft())
         if len(self._items) == 0:
             self._event.clear()
         return result
 
-    async def pop(self):
-        xs = await self.pop_many(limit=1)
+    async def wait_pop(self):
+        xs = await self.wait_pop_many(limit=1)
         assert len(xs) == 1
         return xs[0]
 
+    def pop_all(self):
+        xs = self.tolist()
+        self.clear()
+        return xs
+
     def __aiter__(self):
         return self
 
     async def __anext__(self):
-        return await self.pop()
+        return await self.wait_pop()
 
     def clear(self):
         self._event.clear()
         self._items.clear()
 
 
 class AsyncMap(AsyncIterable[T], Generic[T]):
@@ -193,15 +207,15 @@
     def create_task(
         self, coro: Coroutine[Any, Any, T], name: Optional[str] = None
     ) -> asyncio.Task[T]:
         return self._loop.create_task(coro, name=name)
 
 
 async def wrap_iterator(
-    it: Callable[[], Iterator[T]] | Iterator[T], executor=None
+    it: Union[Callable[[], Iterator[T]], Iterator[T]], executor=None
 ) -> AsyncIterator[T]:
     """Make a blocking iterator into an async iterator by running the iterator in a separate thread.
 
     We assume that the iterator is thread safe (motivating use case: iterating over a sqlite cursor).
     If argument is a callable, then we run the callable in a separate thread too.
     We also assume that a thread pool executor is set.
     """
```

### Comparing `miniscutil-0.0.1/miniscutil/current.py` & `miniscutil-0.0.2/miniscutil/current.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,19 @@
         self.__class__.CURRENT.reset(t)
 
     @classmethod
     def current(cls: Type[T]) -> T:
         """The current value of the singleton class."""
         c = cls.CURRENT.get(None)
         if c is None:
-            c = cls.default()
+            try:
+                c = cls.default()
+            except NotImplementedError:
+                c = cls()
+            assert isinstance(c, cls)
             cls.CURRENT.set(c)
         return c
 
     @classmethod
     def set_current(cls, t, exist_ok=False):
         if (cls.CURRENT.get(None) is not None) and not exist_ok:
             logging.warning(
```

### Comparing `miniscutil-0.0.1/miniscutil/deep.py` & `miniscutil-0.0.2/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/miniscutil/deepeq.py` & `miniscutil-0.0.2/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/miniscutil/dispatch.py` & `miniscutil-0.0.2/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/miniscutil/misc.py` & `miniscutil-0.0.2/miniscutil/misc.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     TypeVar,
 )
 from functools import partial
 import math
 import functools
 
 
-
 X = TypeVar("X")
 Y = TypeVar("Y")
 Z = TypeVar("Z")
 
 
 if hasattr(functools, "cache"):
     cache = functools.cache
@@ -70,24 +69,39 @@
     return DictDiff(
         add=k2.difference(k1),
         rm=k1.difference(k2),
         mod={k: (v1, d2[k]) for k, v1 in d1.items() if (k in d2) and (d2[k] != v1)},
     )
 
 
-def map_keys(f: Callable[[X], Y], d: dict[X,Z]) -> dict[Y,Z]:
+def map_keys(f: Callable[[X], Y], d: dict[X, Z]) -> dict[Y, Z]:
     return {f(k): v for k, v in d.items()}
 
 
-def map_values(f: Callable[[X], Y], d: dict[Z,X]) -> dict[Z,Y]:
+def map_values(f: Callable[[X], Y], d: dict[Z, X]) -> dict[Z, Y]:
     return {k: f(v) for k, v in d.items()}
 
+
 def partition(
     pred: Callable[[X], bool], iterable: Iterable[X]
 ) -> Tuple[Iterable[X], Iterable[X]]:
     """Use a predicate to partition entries into false entries and true entries.
 
     ref: https://docs.python.org/3/library/itertools.html
     """
     # partition(is_odd, range(10)) --> 0 2 4 6 8   and  1 3 5 7 9
     t1, t2 = tee(iterable)
     return filterfalse(pred, t1), filter(pred, t2)
+
+
+def append_url_params(url: str, **params) -> str:
+    """Add the given query params dictionary to the given url."""
+    from urllib.parse import urlparse, parse_qsl, urlencode, urlunparse
+
+    # https://stackoverflow.com/questions/2506379/add-params-to-given-url-in-python
+    parts = urlparse(url)
+    query = dict(parse_qsl(parts.query))
+    query.update(params)
+    parts = parts._replace(query=urlencode(query))
+    result = urlunparse(parts)
+    assert isinstance(result, str)
+    return result
```

### Comparing `miniscutil-0.0.1/miniscutil/ofdict.py` & `miniscutil-0.0.2/miniscutil/ofdict.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,110 @@
+from collections import ChainMap
 from dataclasses import fields, is_dataclass
 from datetime import datetime
 from enum import Enum
 from functools import singledispatch
+import inspect
 import json
 from pathlib import Path
 from typing import (
     Any,
+    ClassVar,
     Dict,
     List,
     Literal,
     NewType,
     Optional,
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 import logging
 from .dispatch import classdispatch
-from .type_util import as_list, as_optional, is_optional
+from .type_util import as_list, as_newtype, as_optional, as_set, is_optional
 
 try:
     from typing import TypeGuard
 except ImportError:
     from typing_extensions import TypeGuard
 
+
 T = TypeVar("T")
 logger = logging.getLogger(__name__)
 
 JsonLike = Optional[Union[dict, list, str, bool, int, float]]
 JsonKey = Optional[Union[str, int, float, bool]]
 
 
 def is_json_key(key: Any) -> TypeGuard[JsonKey]:
     return isinstance(key, (str, int, float, bool, type(None)))
 
 
+def ofdict_dataclass(A: Type[T], a: JsonLike) -> T:
+    assert is_dataclass(A)
+    d2 = {}
+    for f in fields(A):
+        if not isinstance(a, dict):
+            raise TypeError(
+                f"Error while decoding dataclass {A}, expected a dict but got {a} : {type(a)}"
+            )
+        k = f.name
+        if k not in a:
+            if f.type is not None and is_optional(f.type):
+                v = None
+            else:
+                raise ValueError(
+                    f"Missing {f.name} on input dict. Decoding {a} to type {A}."
+                )
+        else:
+            v = a[k]
+        if f.type is not None:
+            d2[k] = ofdict(f.type, v)
+        else:
+            d2[k] = v
+    return A(**d2)  # type: ignore
+
+
 @classdispatch
 def ofdict(A: Type[T], a: JsonLike) -> T:
     """Converts an ``a`` to an instance of ``A``, calling recursively if necessary.
 
     We assume that ``a`` is a nested type made of dicts, lists and scalars.
 
     The main usecase is to be able to treat dataclasses as a schema for json.
     Ideally, ``ofdict`` should be defined such that ``ofdict(type(x), json.loads(MyJsonEncoder().dumps(x)))`` is deep-equal to ``x`` for all ``x``.
 
     Similar to ` cattrs.structure <https://cattrs.readthedocs.io/en/latest/structuring.html#what-you-can-structure-and-how/>`_.
+
+    [todo] I am hoping to retire this in favour of Pydantic.
     """
+    if isinstance(A, str):
+        raise TypeError(
+            f"please make sure your class {A} is referred using types and not string-escaped types"
+        )
+    S = as_newtype(A)
+    if S is not None:
+        return A(ofdict(S, a))
+    if inspect.isclass(A) and issubclass(A, OfDictUnion):
+        class_key = getattr(A, "_class_key", "__class__")
+        ct = getattr(A, "_class_table", None)
+        if ct is None:
+            raise TypeError(f"failed to find class table for {A}")
+        assert isinstance(a, dict)
+        C: Optional[type] = a.get(class_key, None)
+        if C is None:
+            raise TypeError(
+                f"ofdict for a subclass of 'OfDictUnion' must include a '{class_key}' key."
+            )
+        if not issubclass(C, A):
+            raise TypeError(f"Expected {C} to be a subclass of {A}")
+        A = C  # type: ignore
+
     if A is Any:
         return a  # type: ignore
     if A is type(None) and a is None:
         return a  # type: ignore
     if get_origin(A) is Literal:
         values = get_args(A)
         if a in values:
@@ -72,57 +125,50 @@
         return od(a)
     adapt = getattr(A, "__adapt__", None)
     if adapt is not None:
         result = adapt(a)
         if result is not None:
             return result
     if is_dataclass(A):
-        d2 = {}
-        for f in fields(A):
-            if not isinstance(a, dict):
-                raise TypeError(
-                    f"Error while decoding dataclass {A}, expected a dict but got {a} : {type(a)}"
-                )
-            k = f.name
-            if k not in a:
-                if f.type is not None and is_optional(f.type):
-                    v = None
-                else:
-                    raise ValueError(
-                        f"Missing {f.name} on input dict. Decoding {a} to type {A}."
-                    )
-            else:
-                v = a[k]
-            if f.type is not None:
-                d2[k] = ofdict(f.type, v)
-            else:
-                d2[k] = v
-        return A(**d2)
+        return ofdict_dataclass(A, a)  # type: ignore
     if A in [float, str, int, bytes]:  # [todo] etc
         if isinstance(a, A):
-            return a
+            return a  # type: ignore
         else:
             raise TypeError(f"Expected an {A} but was {type(a)}")
-
-    if (not get_origin(A)) and isinstance(a, A):
-        return a
+    try:
+        if isinstance(a, A):
+            return a  # type: ignore
+    except TypeError:
+        pass
     raise NotImplementedError(f"No implementation of ofdict for {A}.")
 
 
 @ofdict.register(list)
 def _list_ofdict(A, a):
     if not isinstance(a, list):
         raise TypeError(f"Expected a list but got a {type(a)}")
     X = as_list(A)
     if X is not None:
         return [ofdict(X, y) for y in a]
     else:
         return a
 
 
+@ofdict.register(set)
+def _set_ofdict(A, a):
+    if not isinstance(a, list):
+        raise TypeError(f"Expected a list but got a {type(a)}")
+    X = as_set(A)
+    if X is not None:
+        return set(ofdict(X, y) for y in a)
+    else:
+        return set(a)
+
+
 @ofdict.register(dict)
 def _dict_ofdict(A, a):
     if not isinstance(a, dict):
         raise TypeError(f"Expected a {A} but got {type(a)}")
     o = get_origin(A)
     if o is None:
         return a
@@ -186,21 +232,50 @@
                     for field in fields(item)
                 ]
             )
         return True
     raise NotImplementedError(f"Don't know how to validate {t}")
 
 
+def todict_dataclass(x: Any):
+    assert is_dataclass(x)
+    r = {}
+    for field in fields(x):
+        k = field.name
+        v = getattr(x, k)
+        if is_optional(field.type) and v is None:
+            continue
+        # [todo] shouldn't this not be recursive?
+        r[k] = todict(v)
+    return r
+
+
 @singledispatch
 def todict(x: Any) -> JsonLike:
     """Converts the given object to a JSON-compatible object.
 
     This should not recurse on the arguments. Just return one of dict, list, tuple, str, int, float, bool, or None.
     `MyJsonEncoder` will run todict recursively on any child objects.
     """
+    if isinstance(x, OfDictUnion):
+        j = _todict_core(x)
+        cls = type(x)
+        root = cls._root_class
+        class_key = root._class_key
+        assert issubclass(cls, root)
+        assert cls in cls._class_table
+        assert isinstance(j, dict)
+        assert class_key not in j
+        j[class_key] = cls.__name__
+        return j
+    else:
+        return _todict_core(x)
+
+
+def _todict_core(x: Any):
     if isinstance(x, (str, int, float, bool)):
         return x
     if x is None:
         return x
     # Something like PEP-246
     conform = getattr(x, "__todict__", None)
     if conform is not None:
@@ -213,22 +288,15 @@
         if result is not NotImplemented:
             return result
     if isinstance(x, tuple):
         return list(x)
     if isinstance(x, (list, dict)):
         return x
     if is_dataclass(x):
-        r = {}
-        for field in fields(x):
-            k = field.name
-            v = getattr(x, k)
-            if is_optional(field.type) and v is None:
-                continue
-            r[k] = todict(v)
-        return r
+        return todict_dataclass(x)
     raise NotImplementedError(f"Don't know how to convert {type(x)}")
 
 
 @todict.register(Enum)
 def _todict_enum(x):
     return x.value
 
@@ -239,18 +307,24 @@
 
 
 @todict.register(Path)
 def _todict_path(x):
     return str(x)
 
 
+@todict.register(set)
+def _todict_set(x):
+    return list(x)
+
+
 class MyJsonEncoder(json.JSONEncoder):
     """Converts Python objects to Json.
 
     We have additional support for dataclasses and enums that are not present in the standard encoder.
+    [todo] rename to TypedJsonEncoder?
     """
 
     def encode(self, obj):
         if isinstance(obj, dict):
             # json encoder doesn't recursively encode keys.
             obj = {todict_key(k): v for k, v in obj.items()}
             assert all(is_json_key(k) for k in obj.keys())
@@ -312,21 +386,43 @@
         return [todict_rec(c) for c in j]
     elif isinstance(x, (str, int, float, bool)):
         return x
     else:
         raise TypeError(f"Don't know how to todict {type(x)}")
 
 
+class OfDictUnion:
+    _class_key: ClassVar[str] = "__class__"
+    _class_table: ClassVar[dict[str, type]]
+    _root_class: ClassVar[type["OfDictUnion"]]
+    """ Use this when you have a class hierarchy of types that you want
+    to be able to serialize using todict.
+
+    It works by also storing a  `"__class__": cls.__name__` entry on a class table.
+    When the dict is deserialised, it will look up this class name to find the subclass.
+    """
+
+    def __init_subclass__(cls, **kwargs):
+        if not hasattr(cls, "_class_table"):
+            # first time
+            cls._class_table = dict()
+            cls._root_class = cls
+        name = cls.__name__
+        assert name not in cls._class_table
+        cls._class_table[name] = cls
+        super().__init_subclass__(**kwargs)
+
+
 try:
     from pydantic import BaseModel
 
     @todict.register(BaseModel)
     def _todict_model(x: BaseModel):
         return x.dict()
 
     @ofdict.register(BaseModel)
     def _ofdict_model(ModelCls: type[BaseModel], item):
         return ModelCls.parse_obj(item)
 
-    # [todo] pydantic validation types like EmailStr etc
+    # [todo] pydantic validation types like EmailStr, SecretStr etc
 except ImportError:
     pass
```

### Comparing `miniscutil-0.0.1/miniscutil/sum.py` & `miniscutil-0.0.2/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/miniscutil/type_util.py` & `miniscutil-0.0.2/miniscutil/type_util.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+import inspect
 from typing import (
+    Any,
+    NewType,
     get_origin,
     get_args,
     Type,
     Optional,
     Union,
 )
 
@@ -30,13 +33,46 @@
             else:
                 return Union[ts]  # type: ignore
     return None
 
 
 def as_list(T: Type) -> Optional[Type]:
     """If `T = List[X]`, return `X`, otherwise return None."""
+    if T == list:
+        return Any
     o = get_origin(T)
     if o is None:
         return None
     if issubclass(o, list):
         return get_args(T)[0]
     return None
+
+
+def as_newtype(T: Type) -> Optional[Type]:
+    return getattr(T, "__supertype__", None)
+
+
+def as_set(T: Type) -> Optional[Type]:
+    if T == set:
+        return Any
+    o = get_origin(T)
+    if o is None:
+        return None
+    if issubclass(o, set):
+        return get_args(T)[0]
+    return None
+
+
+def is_subtype(T1: Type, T2: Type) -> bool:
+    """Polyfill for issubclass.
+
+    Pre 3.10 doesn't have good support for subclassing unions.
+    """
+    try:
+        return issubclass(T1, T2)
+    except TypeError:
+        if get_origin(T2) is Union:
+            return any(is_subtype(T1, a) for a in get_args(T2))
+        S = as_newtype(T2)
+        if S is not None:
+            return is_subtype(T1, S)
+        raise
```

### Comparing `miniscutil-0.0.1/tests/test_classdispatch.py` & `miniscutil-0.0.2/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/tests/test_current.py` & `miniscutil-0.0.2/tests/test_current.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass, fields
 from miniscutil import Current
 from pytest import raises
 
+
 def test_current():
     @dataclass
     class Hello(Current):
         x: int
 
         @classmethod
         def default(cls):
@@ -42,10 +43,9 @@
 
     @dataclass
     class World(Current):
         y: str
 
     assert World.CURRENT != Hello.CURRENT
 
-    with raises(NotImplementedError):
+    with raises(TypeError):
         World.current()
-
```

### Comparing `miniscutil-0.0.1/tests/test_deepeq.py` & `miniscutil-0.0.2/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/tests/test_ofdict.py` & `miniscutil-0.0.2/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/tests/test_typing.py` & `miniscutil-0.0.2/tests/test_typing.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from miniscutil.type_util import *
 
+
 def test_isoptional():
     assert is_optional(Optional[int])
     assert not is_optional(int)
     assert is_optional(Union[type(None), int])
     assert is_optional(Union[int, type(None)])
     assert not is_optional(Union[int, int])
```

### Comparing `miniscutil-0.0.1/.gitignore` & `miniscutil-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/LICENSE.txt` & `miniscutil-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.1/README.md` & `miniscutil-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![PyPI - Version](https://img.shields.io/pypi/v/miniscutil.svg)](https://pypi.org/project/miniscutil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/miniscutil.svg)](https://pypi.org/project/miniscutil)
 
 -----
 
 Collection of miscellaneous functions and methods that I wish were in core. I think that some of them are implemented by existing libraries.
 
+This is supposed to be a big bag of code that I use in lots of my projects, eventually they should be replaced with an existing library or moved into their own specialized library.
+
 - `dispatch.py` hijacks the dispatcher used by `functools.singledispatch` as its own class. This is used to implement a `classdispatch` decorator that can accept a type as argument.
 - `adapt`, an implementation of [PEP-246](https://peps.python.org/pep-0246/#specification)
 - `ofdict.py` converts to and from a json-like object `JsonLike = Union[str, int, float, bool, type(None), list[JsonLike], dict[str, JsonLike]]`. It overlaps a lot with `attrs`, `cattrs` and `pydantic` libraries.
 - `deep.py` implements a deepcopy-like reduction system for traversing, mapping and serializing arbitrary python objects.
 - `deepeq.py` implements a deep-equality algorithm.
 - `current.py` is a base class for implementing the singleton pattern.
 - `sum.py` discriminated sum type.
```

### Comparing `miniscutil-0.0.1/pyproject.toml` & `miniscutil-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "typing-extensions; python_version <= '3.9'"
+  "typing-extensions; python_version <= '3.9'",
+  "pydantic",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/EdAyers/sss/miniscutil#readme"
 Issues = "https://github.com/EdAyers/sss/miniscutil/issues"
 Source = "https://github.com/EdAyers/sss/miniscutil"
@@ -37,14 +38,15 @@
 path = "miniscutil/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
   "numpy",
+  "pydantic",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=miniscutil --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["37", "38", "39", "310", "311"]
```

### Comparing `miniscutil-0.0.1/PKG-INFO` & `miniscutil-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.0.1
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -13,26 +13,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
+Requires-Dist: pydantic
 Requires-Dist: typing-extensions; python_version <= '3.9'
 Description-Content-Type: text/markdown
 
 # miniscutil
 
 [![PyPI - Version](https://img.shields.io/pypi/v/miniscutil.svg)](https://pypi.org/project/miniscutil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/miniscutil.svg)](https://pypi.org/project/miniscutil)
 
 -----
 
 Collection of miscellaneous functions and methods that I wish were in core. I think that some of them are implemented by existing libraries.
 
+This is supposed to be a big bag of code that I use in lots of my projects, eventually they should be replaced with an existing library or moved into their own specialized library.
+
 - `dispatch.py` hijacks the dispatcher used by `functools.singledispatch` as its own class. This is used to implement a `classdispatch` decorator that can accept a type as argument.
 - `adapt`, an implementation of [PEP-246](https://peps.python.org/pep-0246/#specification)
 - `ofdict.py` converts to and from a json-like object `JsonLike = Union[str, int, float, bool, type(None), list[JsonLike], dict[str, JsonLike]]`. It overlaps a lot with `attrs`, `cattrs` and `pydantic` libraries.
 - `deep.py` implements a deepcopy-like reduction system for traversing, mapping and serializing arbitrary python objects.
 - `deepeq.py` implements a deep-equality algorithm.
 - `current.py` is a base class for implementing the singleton pattern.
 - `sum.py` discriminated sum type.
```

