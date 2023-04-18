# Comparing `tmp/fastapi_simple_pagination-1.2.4.tar.gz` & `tmp/fastapi_simple_pagination-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_simple_pagination-1.2.4.tar", max compression
+gzip compressed data, was "fastapi_simple_pagination-1.3.0.tar", max compression
```

## Comparing `fastapi_simple_pagination-1.2.4.tar` & `fastapi_simple_pagination-1.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      240 2023-02-06 17:53:10.890056 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/__init__.py
--rw-r--r--   0        0        0      584 2023-02-06 17:53:10.890056 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/common.py
--rw-r--r--   0        0        0     2465 2023-03-13 13:01:27.765115 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/cursor_pagination.py
--rw-r--r--   0        0        0     2004 2023-02-06 16:43:13.077613 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/deps.py
--rw-r--r--   0        0        0        0 2023-02-06 16:43:13.077613 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/py.typed
--rw-r--r--   0        0        0     3999 2023-02-06 20:51:57.966754 fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/schemas.py
--rw-r--r--   0        0        0      751 2023-03-13 13:02:32.065116 fastapi_simple_pagination-1.2.4/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 fastapi_simple_pagination-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      240 2023-02-06 17:53:10.890056 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/__init__.py
+-rw-r--r--   0        0        0      561 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/common.py
+-rw-r--r--   0        0        0     2287 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/cursor_pagination.py
+-rw-r--r--   0        0        0     2000 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/deps.py
+-rw-r--r--   0        0        0        0 2023-02-06 16:43:13.077613 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/py.typed
+-rw-r--r--   0        0        0     4108 2023-04-18 13:07:42.699712 fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/schemas.py
+-rw-r--r--   0        0        0      751 2023-04-18 13:08:01.381787 fastapi_simple_pagination-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 fastapi_simple_pagination-1.3.0/PKG-INFO
```

### Comparing `fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/common.py` & `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from typing import Any, List, Optional, Protocol, TypeVar
 
 from pydantic import BaseModel, ConstrainedInt
 
-_Item = TypeVar("_Item", bound=BaseModel)
-_OtherItem = TypeVar("_OtherItem", bound=BaseModel)
+Item = TypeVar("Item")
+OtherItem = TypeVar("OtherItem", bound=BaseModel)
 
 
 class QuerySize(ConstrainedInt):
     le = 100
     gt = 0
 
 
-class PaginatedMethodProtocol(Protocol[_Item]):
+class PaginatedMethodProtocol(Protocol[Item]):
     async def __call__(
         self,
         *,
         offset: Optional[int] = None,
         size: Optional[int] = None,
         **kwargs: Any,
-    ) -> List[_Item]:
+    ) -> List[Item]:
         ...
 
 
 class CountItems(Protocol):
     async def __call__(self, **kwargs: Any) -> int:
         ...
```

### Comparing `fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/cursor_pagination.py` & `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/cursor_pagination.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from asyncio import create_task
 from dataclasses import dataclass
 from typing import Any, Callable, List
 
 from fastapi import Query, Request
-from pydantic import AnyHttpUrl, NonNegativeInt, parse_obj_as
+from pydantic import HttpUrl, NonNegativeInt, parse_obj_as
 
-from .common import CountItems, PaginatedMethodProtocol, QuerySize, _Item, _OtherItem
+from .common import CountItems, Item, OtherItem, PaginatedMethodProtocol, QuerySize
 from .schemas import CursorPage
 
 
-def _identity(item: _Item) -> _Item:
+def _identity(item: Any) -> Any:
     return item
 
 
 @dataclass()
 class CursorPaginationParams:
     request: Request
     offset: NonNegativeInt = Query(
@@ -23,54 +22,50 @@
     size: QuerySize = Query(
         default=10,
         description="Size of the page.",
     )
 
     async def paginated(
         self,
-        items_getter: PaginatedMethodProtocol[_Item],
+        items_getter: PaginatedMethodProtocol[Item],
         item_counter: CountItems,
-        item_mapper: Callable[[_Item], _OtherItem] = _identity,
+        item_mapper: Callable[[Item], OtherItem] = _identity,
         **kwargs: Any,
-    ) -> CursorPage[_OtherItem]:
-        item_list = create_task(
-            items_getter(size=self.size, offset=self.offset, **kwargs)
-        )
-        item_count = create_task(item_counter(**kwargs))
-        has_next = create_task(
-            items_getter(offset=self.offset + self.size, size=1, **kwargs)
-        )
-        items = [item_mapper(i) for i in await item_list]
+    ) -> CursorPage[OtherItem]:
+        item_list = await items_getter(size=self.size, offset=self.offset, **kwargs)
+        item_count = await item_counter(**kwargs)
+        has_next = self.offset + self.size < item_count
+        items = [item_mapper(i) for i in item_list]
 
-        return self._build_page(await item_count, items, len(await has_next) > 0)
+        return self._build_page(item_count, items, has_next)
 
     def _build_page(
-        self, item_count: int, item_list: List[_Item], has_next: bool
-    ) -> CursorPage[_Item]:
+        self, item_count: int, item_list: List[OtherItem], has_next: bool
+    ) -> CursorPage[OtherItem]:
         return CursorPage(
             items=item_list,
             count=item_count,
-            current=parse_obj_as(AnyHttpUrl, str(self.request.url)),
-            next_url=self._build_next_url(item_list) if has_next else None,
+            current=parse_obj_as(HttpUrl, str(self.request.url)),
+            next_url=self._build_next_url() if has_next else None,
             previous_url=self._build_previous_url() if self.offset > 0 else None,
             size=self.size,
             offset=self.offset,
         )
 
-    def _build_next_url(self, items: List[_Item]):
+    def _build_next_url(self) -> HttpUrl:
         new_url = self.request.url.remove_query_params(
             ["offset", "size"]
         ).include_query_params(
-            offset=self.offset + len(items),
+            offset=self.offset + self.size,
             size=self.size,
         )
 
-        return parse_obj_as(AnyHttpUrl, str(new_url))
+        return parse_obj_as(HttpUrl, str(new_url))
 
-    def _build_previous_url(self):
+    def _build_previous_url(self) -> HttpUrl:
         offset = self.offset - self.size
         if offset < 0:
             offset = 0
         new_url = self.request.url.remove_query_params(
             ["offset", "size"]
         ).include_query_params(offset=offset, size=self.size)
-        return parse_obj_as(AnyHttpUrl, str(new_url))
+        return parse_obj_as(HttpUrl, str(new_url))
```

### Comparing `fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/deps.py` & `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/deps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import dataclasses
 import math
 import typing
 
 import fastapi
 from pydantic import AnyHttpUrl, parse_obj_as
 
-from .common import _Item
+from .common import Item
 from .schemas import Page
 
 
 @dataclasses.dataclass(frozen=True)
-class PaginationRequestParams(typing.Generic[_Item]):
+class PaginationRequestParams(typing.Generic[Item]):
     request: fastapi.Request
     page: int = fastapi.Query(1, description="The page number to query.")
     size: int = fastapi.Query(10, description="The page size.")
 
     def get_next(self, total_count: int):
         if self.page * self.size < total_count:
             url = self.request.url.replace_query_params(
@@ -46,16 +46,16 @@
         raw_url = str(
             self.request.url.replace_query_params(page=last_page, size=self.size)
         )
 
         return parse_obj_as(AnyHttpUrl, raw_url)
 
     def paginated(
-        self, items: typing.List[_Item], total_count: typing.Optional[int] = None
-    ) -> Page[_Item]:
+        self, items: typing.List[Item], total_count: typing.Optional[int] = None
+    ) -> Page[Item]:
         count = total_count or len(items)
         return Page(
             count=count,
             items=items[: self.size],
             page=self.page,
             next=self.get_next(count),
             previous=self.get_previous(count),
```

### Comparing `fastapi_simple_pagination-1.2.4/fastapi_simple_pagination/schemas.py` & `fastapi_simple_pagination-1.3.0/fastapi_simple_pagination/schemas.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,26 @@
-from asyncio import Task, create_task
-from typing import Awaitable, Callable, Generic, List, Optional, Type
+from __future__ import annotations
 
-from pydantic import AnyHttpUrl, Field, NonNegativeInt, PositiveInt
+from asyncio import Task, create_task, ensure_future
+from typing import Any, Awaitable, Callable, Generic, List, Optional, Type, TypeVar
+
+from pydantic import (
+    AnyHttpUrl,
+    Field,
+    HttpUrl,
+    NonNegativeInt,
+    PositiveInt,
+    parse_obj_as,
+)
 from pydantic.generics import GenericModel
 
-from .common import _Item, _OtherItem
+from .common import Item, OtherItem
 
 
-class Page(GenericModel, Generic[_Item]):
+class Page(GenericModel, Generic[Item]):
     count: int = Field(
         default=...,
         description="The total number of items in the database.",
     )
     previous: Optional[AnyHttpUrl] = Field(
         default=None,
         description="The URL to the previous page.",
@@ -33,95 +42,94 @@
         description="The URL to refresh the current page.",
     )
 
     page: int = Field(
         default=...,
         description="The current page number.",
     )
-    items: List[_Item] = Field(
+    items: List[Item] = Field(
         default=...,
         description="The item list on this page.",
     )
 
     def map(
         self,
-        mapper: Callable[[_Item], _OtherItem],
-        type_: Optional[Type[_OtherItem]] = None,
-    ) -> "Page[_OtherItem]":
+        mapper: Callable[[Item], OtherItem],
+        type_: Optional[Type[OtherItem]] = None,
+    ) -> "Page[OtherItem]":
         items = [mapper(item) for item in self.items]
         return self._build_new_page(items, type_)
 
     def _build_new_page(
-        self, items: List[_OtherItem], type_: Optional[Type[_OtherItem]] = None
-    ) -> "Page[_OtherItem]":
+        self, items: List[OtherItem], type_: Optional[Type[OtherItem]] = None
+    ) -> "Page[OtherItem]":
         new_page = Page(  # type: ignore
             items=items,
             **dict(self),
         )
         if type_ is not None:
             return Page[type_].parse_obj(new_page)  # type: ignore
         return new_page
 
     async def map_async(
         self,
-        mapper: Callable[[_Item], Awaitable[_OtherItem]],
-        type_: Optional[Type[_OtherItem]] = None,
-    ) -> "Page[_OtherItem]":
-        item_tasks: List[Task[_OtherItem]] = [
+        mapper: Callable[[Item], Awaitable[OtherItem]],
+        type_: Optional[Type[OtherItem]] = None,
+    ) -> "Page[OtherItem]":
+        item_tasks: List[Task[OtherItem]] = [
             create_task(mapper(item)) for item in self.items  # type: ignore
         ]
         return self._build_new_page([await task for task in item_tasks], type_)
 
+    def validate_page(self, page_model: Type[_Page]) -> _Page:
+        return parse_obj_as(page_model, self)
+
 
-class CursorPage(GenericModel, Generic[_Item]):
+class CursorPage(GenericModel, Generic[Item]):
     """An offset and size paginated list."""
 
     offset: NonNegativeInt = Field(
         description="The offset where to start retrieving.",
     )
     size: PositiveInt = Field(
         description="The size of the page.",
     )
     count: NonNegativeInt = Field(
         description="How many items are saved in the store.",
     )
-    current: AnyHttpUrl = Field(
+    current: HttpUrl = Field(
         description="The URL of the current page.",
     )
-    next_url: Optional[AnyHttpUrl] = Field(
+    next_url: Optional[HttpUrl] = Field(
         description="The next page URL.",
     )
-    previous_url: Optional[AnyHttpUrl] = Field(
+    previous_url: Optional[HttpUrl] = Field(
         description="The previous page URL.",
     )
-    items: List[_Item] = Field(description="The items of the page.")
+    items: List[Item] = Field(description="The items of the page.")
 
-    def map(
-        self,
-        mapper: Callable[[_Item], _OtherItem],
-        type_: Optional[Type[_OtherItem]] = None,
-    ) -> "CursorPage[_OtherItem]":
+    def map(self, mapper: Callable[[Item], OtherItem]) -> "CursorPage[OtherItem]":
         items = [mapper(item) for item in self.items]
-        return self._build_new_page(items, type_)
+        return self._build_new_page(items)
 
-    def _build_new_page(
-        self, items: List[_OtherItem], type_: Optional[Type[_OtherItem]] = None
-    ) -> "CursorPage[_OtherItem]":
+    def _build_new_page(self, items: List[OtherItem]) -> "CursorPage[OtherItem]":
         new_page = CursorPage(  # type: ignore
             items=items,
             **self.dict(exclude={"items"}),
         )
 
-        if type_ is not None:
-            return Page[type_].parse_obj(new_page)  # type: ignore
-
         return new_page
 
     async def map_async(
-        self,
-        mapper: Callable[[_Item], Awaitable[_OtherItem]],
-        type_: Optional[Type[_OtherItem]] = None,
-    ) -> "CursorPage[_OtherItem]":
-        item_tasks: List[Task[_OtherItem]] = [
-            create_task(mapper(item)) for item in self.items  # type: ignore
+        self, mapper: Callable[[Item], Awaitable[OtherItem]]
+    ) -> "CursorPage[OtherItem]":
+        item_tasks: List[Task[OtherItem]] = [
+            ensure_future(mapper(item)) for item in self.items
         ]
-        return self._build_new_page([await task for task in item_tasks], type_)
+        return self._build_new_page([await task for task in item_tasks])
+
+    def validate_page(self, page_model: Type[_CursorPage]) -> _CursorPage:
+        return parse_obj_as(page_model, self)
+
+
+_CursorPage = TypeVar("_CursorPage", bound=CursorPage[Any])
+_Page = TypeVar("_Page", bound=CursorPage[Any])
```

### Comparing `fastapi_simple_pagination-1.2.4/pyproject.toml` & `fastapi_simple_pagination-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 authors = ["Francisco Del Roio <francipvb@hotmail.com>"]
 description = "Simple and generic pagination dependencies for FastAPI."
 exclude = ["tests/"]
 name = "fastapi-simple-pagination"
-version = "1.2.4"
+version = "1.3.0"
 
 [tool.poetry.dependencies]
 fastapi = "<1.0.0"
 pydantic = "<2.0.0"
 python = ">=3.8.1, <4.0.0"
```

