# Comparing `tmp/iamai_adapter_cqhttp-0.6.0.post1.tar.gz` & `tmp/iamai_adapter_cqhttp-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai_adapter_cqhttp-0.6.0.post1.tar", max compression
+gzip compressed data, was "iamai_adapter_cqhttp-0.6.1.tar", max compression
```

## Comparing `iamai_adapter_cqhttp-0.6.0.post1.tar` & `iamai_adapter_cqhttp-0.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/README.md
--rw-r--r--   0        0        0     7994 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0      899 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/config.py
--rw-r--r--   0        0        0    13988 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      656 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7475 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     1319 2023-04-05 06:03:03.805478 iamai_adapter_cqhttp-0.6.0.post1/pyproject.toml
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-0.6.0.post1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/README.md
+-rw-r--r--   0        0        0     7995 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/__init__.py
+-rw-r--r--   0        0        0      899 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/config.py
+-rw-r--r--   0        0        0    14033 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/event.py
+-rw-r--r--   0        0        0      656 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/exceptions.py
+-rw-r--r--   0        0        0     7475 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/message.py
+-rw-r--r--   0        0        0     1313 2023-04-18 16:36:06.706341 iamai_adapter_cqhttp-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 iamai_adapter_cqhttp-0.6.1/PKG-INFO
```

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/__init__.py` & `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import json
 import time
 import asyncio
 from functools import partial
 from typing import TYPE_CHECKING, Any, Dict, Literal
 
 import aiohttp
+
 from iamai.utils import DataclassEncoder
 from iamai.adapter.utils import WebSocketAdapter
 from iamai.log import logger, error_or_exception
 
 from .config import Config
 from .message import CQHTTPMessage
 from .event import CQHTTPEvent, get_event_class
```

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/config.py` & `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/config.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/event.py` & `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """CQHTTP 适配器事件。"""
 import inspect
 from typing import TYPE_CHECKING, Any, Dict, Type, Union, Literal, TypeVar, Optional
 
-from iamai.event import Event
 from pydantic import Field, BaseModel
 
+from iamai.event import Event
+
 from .message import CQHTTPMessage
 
 if TYPE_CHECKING:
     from .message import T_CQMSG
     from . import CQHTTPAdapter  # noqa
 
 T_CQHTTPEvent = TypeVar("T_CQHTTPEvent", bound="CQHTTPEvent")
@@ -78,32 +79,34 @@
     """CQHTTP 事件基类"""
 
     __event__ = ""
     type: Optional[str] = Field(alias="post_type")
     time: int
     self_id: int
     self_tiny_id: Optional[str]
-    post_type: Literal["message", "message_sent",
-                       "notice", "request", "meta_event"]
+    post_type: Literal["message", "message_sent", "notice", "request", "meta_event"]
 
     @property
     def to_me(self) -> bool:
         """当前事件的 user_id 是否等于 self_id 或 self_tiny_id。"""
-        return getattr(self, "user_id") == self.self_id or getattr(self, "user_id") == self.self_tiny_id
+        return (
+            getattr(self, "user_id") == self.self_id
+            or getattr(self, "user_id") == self.self_tiny_id
+        )
 
 
 class MessageEvent(CQHTTPEvent):
     """消息事件"""
 
     __event__ = "message"
     post_type: Literal["message"]
     message_type: Literal["private", "group", "guild"]
-    sub_type: Union[Literal["channel"],str]
-    message_id: Union[str,int]
-    user_id: Union[str,int]
+    sub_type: Union[Literal["channel"], str]
+    message_id: Union[str, int]
+    user_id: Union[str, int]
     message: CQHTTPMessage
     raw_message: Optional[str]
     font: Optional[int]
     sender: Sender
     guild_id: Optional[str]
     channel_id: Optional[str]
 
@@ -499,14 +502,15 @@
     """心跳包"""
 
     __event__ = "meta_event.heartbeat"
     meta_event_type: Literal["heartbeat"]
     status: Status
     interval: int
 
+
 class GuildMessageEvent(MessageEvent):
     """收到频道消息"""
 
     __event__ = "message.guild"
     message_type: Literal["guild"]
     sub_type: Literal["channel"]
     guild_id: str
@@ -514,17 +518,20 @@
     user_id: str
     message_id: str
     sender: Sender
     message: CQHTTPMessage
 
     async def reply(self, msg: "T_CQMSG") -> Dict[str, Any]:
         return await self.adapter.send_guild_channel_msg(
-            guild_id=self.guild_id,channel_id=self.channel_id, message=CQHTTPMessage(msg)
+            guild_id=self.guild_id,
+            channel_id=self.channel_id,
+            message=CQHTTPMessage(msg),
         )
 
+
 class GuildMessageReactionUpdated(NoticeEvent):
     """频道消息表情贴更新"""
 
     __event__ = "notice.message_reactions_updated"
     notice_type: Literal["message_reactions_updated"]
     guild_id: str
     channel_id: str
@@ -546,27 +553,27 @@
     new_info: ChannelInfo
 
 
 class GuildChannelCreated(NoticeEvent):
     """子频道创建"""
 
     __event__ = "notice.channel_created"
-    notice_type: Literal['channel_created']
+    notice_type: Literal["channel_created"]
     guild_id: str
     channel_id: str
     user_id: str
     operator_id: str
     channel_info: ChannelInfo
 
 
 class GuildChannelDestoryed(NoticeEvent):
     """子频道删除"""
 
     __event__ = "notice.channel_destroyed"
-    notice_type: Literal['channel_destroyed']
+    notice_type: Literal["channel_destroyed"]
     guild_id: str
     channel_id: str
     user_id: str
     operator_id: str
     channel_info: ChannelInfo
```

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/exceptions.py` & `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/iamai/adapter/cqhttp/message.py` & `iamai_adapter_cqhttp-0.6.1/iamai/adapter/cqhttp/message.py`

 * *Files identical despite different names*

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/pyproject.toml` & `iamai_adapter_cqhttp-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iamai-adapter-cqhttp"
-version = "0.6.0.post1"
+version = "0.6.1"
 description = "OneBot(CQHTTP) adapter for iamai."
 authors = ["简律纯 <admin@jyunko.cn>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://retrofor.space/"
 repository = "https://github.com/retrofor/iamai"
 documentation = "https://iamai.retrofor.space/"
```

### Comparing `iamai_adapter_cqhttp-0.6.0.post1/PKG-INFO` & `iamai_adapter_cqhttp-0.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai-adapter-cqhttp
-Version: 0.6.0.post1
+Version: 0.6.1
 Summary: OneBot(CQHTTP) adapter for iamai.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,chatbot,qq,qqbot,cqhttp,coolq
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
```

