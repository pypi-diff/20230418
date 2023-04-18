# Comparing `tmp/iamai-3.14.2.tar.gz` & `tmp/iamai-3.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamai-3.14.2.tar", max compression
+gzip compressed data, was "iamai-3.14.4.tar", max compression
```

## Comparing `iamai-3.14.2.tar` & `iamai-3.14.4.tar`

### file list

```diff
@@ -1,43 +1,25 @@
--rw-r--r--   0        0        0     1071 2023-04-03 22:27:00.721005 iamai-3.14.2/LICENSE
--rw-r--r--   0        0        0     9121 2023-04-03 22:27:00.721005 iamai-3.14.2/README.md
--rw-r--r--   0        0        0      543 2023-04-03 22:27:00.721005 iamai-3.14.2/iamai/__init__.py
--rw-r--r--   0        0        0     4432 2023-04-03 22:27:00.721005 iamai-3.14.2/iamai/adapter/__init__.py
--rw-r--r--   0        0        0     5157 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9165 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0        0        0     4675 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/apscheduler/__init__.py
--rw-r--r--   0        0        0      377 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/apscheduler/config.py
--rw-r--r--   0        0        0      932 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/apscheduler/event.py
--rw-r--r--   0        0        0     7977 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__init__.py
--rw-r--r--   0        0        0     7174 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1290 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0    17516 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__pycache__/event.cpython-310.pyc
--rw-r--r--   0        0        0     1334 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0        0        0     7812 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/__pycache__/message.cpython-310.pyc
--rw-r--r--   0        0        0      896 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/config.py
--rw-r--r--   0        0        0    13989 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/event.py
--rw-r--r--   0        0        0      656 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/exceptions.py
--rw-r--r--   0        0        0     7475 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/cqhttp/message.py
--rw-r--r--   0        0        0     5440 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/dingtalk/__init__.py
--rw-r--r--   0        0        0      590 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/dingtalk/config.py
--rw-r--r--   0        0        0     2363 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/dingtalk/event.py
--rw-r--r--   0        0        0      387 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/dingtalk/exceptions.py
--rw-r--r--   0        0        0     3200 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/dingtalk/message.py
--rw-r--r--   0        0        0       44 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/github/__init.py
--rw-r--r--   0        0        0      924 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/github/config.py
--rw-r--r--   0        0        0        0 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/github/event.py
--rw-r--r--   0        0        0        0 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/github/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/github/message.py
--rw-r--r--   0        0        0     1211 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/http_server_test_adapter.py
--rw-r--r--   0        0        0     1059 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/test.py
--rw-r--r--   0        0        0     7955 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/adapter/utils.py
--rw-r--r--   0        0        0    34529 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/bot.py
--rw-r--r--   0        0        0     1968 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/config.py
--rw-r--r--   0        0        0     1907 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/event.py
--rw-r--r--   0        0        0     1088 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/exceptions.py
--rw-r--r--   0        0        0      426 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/log.py
--rw-r--r--   0        0        0    13843 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/message.py
--rw-r--r--   0        0        0     3503 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/plugin.py
--rw-r--r--   0        0        0     1052 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/typing.py
--rw-r--r--   0        0        0     5529 2023-04-03 22:27:00.725005 iamai-3.14.2/iamai/utils.py
--rw-r--r--   0        0        0     2221 2023-04-03 22:27:00.725005 iamai-3.14.2/pyproject.toml
--rw-r--r--   0        0        0    10702 1970-01-01 00:00:00.000000 iamai-3.14.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-05 06:03:03.797478 iamai-3.14.4/LICENSE
+-rw-r--r--   0        0        0     9133 2023-04-05 06:03:03.797478 iamai-3.14.4/README.md
+-rw-r--r--   0        0        0      543 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/__init__.py
+-rw-r--r--   0        0        0     4432 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__init__.py
+-rw-r--r--   0        0        0     5157 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9165 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0       44 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/__init.py
+-rw-r--r--   0        0        0      924 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/config.py
+-rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/event.py
+-rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/github/message.py
+-rw-r--r--   0        0        0     1210 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/http_server_test_adapter.py
+-rw-r--r--   0        0        0     1059 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/test.py
+-rw-r--r--   0        0        0     7954 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/adapter/utils.py
+-rw-r--r--   0        0        0    34568 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/bot.py
+-rw-r--r--   0        0        0     1968 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/config.py
+-rw-r--r--   0        0        0     1906 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/event.py
+-rw-r--r--   0        0        0     1088 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/exceptions.py
+-rw-r--r--   0        0        0      429 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/log.py
+-rw-r--r--   0        0        0    13843 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/message.py
+-rw-r--r--   0        0        0     3503 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/plugin.py
+-rw-r--r--   0        0        0     1052 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/typing.py
+-rw-r--r--   0        0        0     5529 2023-04-05 06:03:03.805478 iamai-3.14.4/iamai/utils.py
+-rw-r--r--   0        0        0     2311 2023-04-05 06:03:03.809478 iamai-3.14.4/pyproject.toml
+-rw-r--r--   0        0        0    10428 1970-01-01 00:00:00.000000 iamai-3.14.4/PKG-INFO
```

### Comparing `iamai-3.14.2/LICENSE` & `iamai-3.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/README.md` & `iamai-3.14.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 - 🎪 **Interactive [docs](https://iamai.retrofor.space) &amp; [demos](https://iamai.retrofor.space/demos)**
 - 🕶 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more...
 - ⚡ **Fully tree shakeable**: Only take what you want, [bundle size](https://iamai.retrofor.space/export-size)
 - 🔩 **Flexible**: Configurable event filters and targets
 - 🔌 **Optional [Add-ons](https://iamai.retrofor.space/add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler), etc.
 - 👍 **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter](https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/adapters/github), etc.
 
-<p align="center"><img width="512" src="https://iamai.retrofor.space/logo.png"></p>
+<p align="center"><img width="512" src="https://iamai.retrofor.space/icons/retro_plus.png"></p>
 
 ## ⬇️ Install
 
 - STABLE VERSION
 
   ```sh
   pip install iamai
```

#### html2text {}

```diff
@@ -37,15 +37,15 @@
 filters and targets - ð **Optional [Add-ons](https://iamai.retrofor.space/
 add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler),
 etc. - ð **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/
 onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter]
 (https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://
 iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/
 adapters/github), etc.
-                    [https://iamai.retrofor.space/logo.png]
+              [https://iamai.retrofor.space/icons/retro_plus.png]
 ## â¬ï¸ Install - STABLE VERSION ```sh pip install iamai ``` or you can also
 install for TEST. - TEST VERSION ```sh pip install -i https://test.pypi.org/
 simple/ iamai ``` ## â Usage firstly, you need to load an adapter. ```python
 from iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp")
 bot.run() ``` then, you need load the transformer and use your models.
 **transformer(Use from the ð¤/transformers library)** ```python from
 transformers import AutoModelWithLMHead, AutoTokenizer # load models model =
```

### Comparing `iamai-3.14.2/iamai/__init__.py` & `iamai-3.14.4/iamai/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/__init__.py` & `iamai-3.14.4/iamai/adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/__pycache__/__init__.cpython-310.pyc` & `iamai-3.14.4/iamai/adapter/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/__pycache__/utils.cpython-310.pyc` & `iamai-3.14.4/iamai/adapter/__pycache__/utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/github/config.py` & `iamai-3.14.4/iamai/adapter/github/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/http_server_test_adapter.py` & `iamai-3.14.4/iamai/adapter/http_server_test_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """HTTP 服务端适配器示例。
 
 这里是一个最简单可以直接使用的 HTTP 服务端适配器示例。
 """
 from typing import TYPE_CHECKING, Union
 
 from aiohttp import web
-
 from iamai.event import Event
 from iamai.adapter.utils import HttpServerAdapter
 from iamai.message import Message, MessageSegment
 
 if TYPE_CHECKING:
     from iamai.message import T_Message, T_MessageSegment
```

### Comparing `iamai-3.14.2/iamai/adapter/test.py` & `iamai-3.14.4/iamai/adapter/test.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/adapter/utils.py` & `iamai-3.14.4/iamai/adapter/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 """
 import asyncio
 from typing import Union, Literal
 from abc import ABCMeta, abstractmethod
 
 import aiohttp
 from aiohttp import web
-
 from iamai.adapter import Adapter
 from iamai.typing import T_Event, T_Config
 from iamai.log import logger, error_or_exception
 
 
 class PollingAdapter(Adapter[T_Event, T_Config], metaclass=ABCMeta):
     """轮询式适配器示例。"""
```

### Comparing `iamai-3.14.2/iamai/bot.py` & `iamai-3.14.4/iamai/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 import asyncio
 import threading
 from pathlib import Path
 from itertools import chain
 from collections import defaultdict
 from typing import Any, Dict, List, Type, Union, Callable, Optional, Awaitable
 
-from pydantic import ValidationError, create_model
-
 from iamai.adapter import Adapter
 from iamai.plugin import Plugin, PluginLoadType
 from iamai.log import logger, error_or_exception
+from pydantic import ValidationError, create_model
 from iamai.typing import T_Event, T_BotHook, T_EventHook, T_AdapterHook
 from iamai.config import MainConfig, ConfigModel, PluginConfig, AdapterConfig
 from iamai.exceptions import (
     SkipException,
     StopException,
     GetEventTimeout,
     LoadModuleError,
@@ -152,15 +151,15 @@
             if self._restart_flag:
                 self._load_plugins_from_dirs(*self._extend_plugin_dirs)
                 self._load_plugins(*self._extend_plugins)
                 self._load_adapters(*self._extend_adapters)
 
     def restart(self):
         """退出并重新运行 iamai。"""
-        logger.info("Restarting iamai...")
+        logger.warning("Restarting iamai...")
         self._restart_flag = True
         self.should_exit.set()
 
     async def _run(self):
         """运行 iamai。"""
         self.should_exit = asyncio.Event()
         self._condition = asyncio.Condition()
@@ -183,15 +182,15 @@
         # 加载插件和适配器
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self.config.bot.plugins)
         self._load_adapters(*self.config.bot.adapters)
         self._update_config()
 
         # 启动 iamai
-        logger.info("Running iamai...")
+        logger.warning("Running iamai...")
 
         hot_reload_task = None
         if self._hot_reload:
             hot_reload_task = asyncio.create_task(self._run_hot_reload())
 
         for _hook_func in self._bot_run_hooks:
             await _hook_func(self)
@@ -241,15 +240,15 @@
                     and samefile(x.__plugin_file_path__, file),
                     plugins,
                 )
             )
             removed_plugins.extend(_removed_plugins)
             for plugin_ in _removed_plugins:
                 plugins.remove(plugin_)
-                logger.info(
+                logger.success(
                     "Succeeded to remove plugin "
                     f'"{plugin_.__name__}" from file "{file}"'
                 )
         return removed_plugins
 
     async def _run_hot_reload(self):
         """热重载。"""
@@ -258,15 +257,15 @@
         except ImportError:
             logger.warning(
                 'Hot reload needs to install "watchfiles", '
                 'try "pip install watchfiles"'
             )
             return
 
-        logger.info("Hot reload is working!")
+        logger.success("Hot reload is working!")
         async for changes in awatch(
             *map(
                 lambda x: x.resolve(),
                 set(self._extend_plugin_dirs)
                 .union(self.config.bot.plugin_dirs)
                 .union(
                     {Path(self._config_file)}
@@ -280,15 +279,15 @@
             # 以确保发生重命名时先处理删除再处理新增
             for change_type, file in sorted(changes, key=lambda x: x[0], reverse=True):
                 # 更改配置文件
                 if (
                     samefile(self._config_file, file)
                     and change_type == change_type.modified
                 ):
-                    logger.info(f'Reload config file "{self._config_file}"')
+                    logger.warning(f'Reload config file "{self._config_file}"')
                     old_config = self.config
                     self._reload_config_dict()
                     if (
                         self.config.bot != old_config.bot
                         or self.config.adapter != old_config.adapter
                     ):
                         self.restart()
@@ -397,17 +396,17 @@
         self._load_plugins_from_dirs(*self.config.bot.plugin_dirs)
         self._load_plugins(*self._extend_plugins)
         self._load_plugins_from_dirs(*self._extend_plugin_dirs)
         self._update_config()
 
     def _handle_exit(self, *args):  # noqa
         """当机器人收到退出信号时，根据情况进行处理。"""
-        logger.info("Stopping iamai...")
+        logger.warning("Stopping iamai...")
         if self.should_exit.is_set():
-            logger.warning("Force Exit iamai...")
+            logger.critical("Force Exit iamai...")
             sys.exit()
         else:
             self.should_exit.set()
 
     async def handle_event(
         self, current_event: T_Event, *, handle_get: bool = True, show_log: bool = True
     ):
@@ -451,15 +450,15 @@
                     f"Checking for matching plugins with priority {plugin_priority!r}"
                 )
                 stop = False
                 for _plugin in self.plugins_priority_dict[plugin_priority]:
                     try:
                         _plugin = _plugin(current_event)
                         if await _plugin.rule():
-                            logger.info(f"Event will be handled by {_plugin!r}")
+                            logger.warning(f"Event will be handled by {_plugin!r}")
                             try:
                                 await _plugin.handle()
                             finally:
                                 if _plugin.block:
                                     stop = True
                     except SkipException:
                         # 插件要求跳过自身继续当前事件传播
@@ -481,15 +480,15 @@
                     e,
                     self.config.bot.log.verbose_exception,
                 )
 
         for _hook_func in self._event_postprocessor_hooks:
             await _hook_func(current_event)
 
-        logger.info("Event Finished")
+        logger.warning("Event Finished")
 
     async def get(
         self,
         func: Optional[Callable[[T_Event], Union[bool, Awaitable[bool]]]] = None,
         *,
         max_try_times: Optional[int] = None,
         timeout: Optional[Union[int, float]] = None,
@@ -557,15 +556,15 @@
                 if _plugin.__name__ == plugin_class.__name__:
                     logger.warning(
                         f'Already have a same name plugin "{_plugin.__name__}"'
                     )
             plugin_class.__plugin_load_type__ = plugin_load_type
             plugin_class.__plugin_file_path__ = plugin_file_path
             self.plugins_priority_dict[priority].append(plugin_class)
-            logger.info(
+            logger.success(
                 f'Succeeded to load plugin "{plugin_class.__name__}" '
                 f'from class "{plugin_class!r}"'
             )
         else:
             error_or_exception(
                 f'Load plugin from class "{plugin_class!r}" failed:',
                 LoadModuleError(
@@ -617,20 +616,20 @@
                         plugin_, plugin_load_type or PluginLoadType.CLASS, None
                     )
                 else:
                     logger.error(
                         f'The plugin class "{plugin_!r}" must be a subclass of Plugin'
                     )
             elif isinstance(plugin_, str):
-                logger.info(f'Loading plugins from module "{plugin_}"')
+                logger.warning(f'Loading plugins from module "{plugin_}"')
                 self._load_plugins_from_module_name(
                     plugin_, plugin_load_type or PluginLoadType.NAME
                 )
             elif isinstance(plugin_, Path):
-                logger.info(f'Loading plugins from path "{plugin_}"')
+                logger.warning(f'Loading plugins from path "{plugin_}"')
                 if plugin_.is_file():
                     if plugin_.suffix != ".py":
                         logger.error(f'The path "{plugin_}" must endswith ".py"')
                         return
 
                     plugin_module_name = None
                     for path in self._module_path_finder.path:
@@ -679,15 +678,15 @@
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
         Args:
             *dirs: 储存包含插件的模块的模块路径。
                 例如：`pathlib.Path("path/of/plugins/")` 。
         """
         dirs = list(map(lambda x: str(x.resolve()), dirs)) # type: ignore
-        logger.info(f'Loading plugins from dirs "{", ".join(map(str, dirs))}"')
+        logger.warning(f'Loading plugins from dirs "{", ".join(map(str, dirs))}"')
         self._module_path_finder.path.extend(dirs) # type: ignore
         for plugin_class, module in get_classes_from_dir(dirs, Plugin): # type: ignore
             self._load_plugin_class(plugin_class, PluginLoadType.DIR, module.__file__)
 
     def load_plugins_from_dirs(self, *dirs: Path):
         """从目录中加载插件，以 `_` 开头的模块中的插件不会被导入。路径可以是相对路径或绝对路径。
 
@@ -736,15 +735,15 @@
                 error_or_exception(
                     f'Load adapter "{adapter_}" failed:',
                     e,
                     self.config.bot.log.verbose_exception,
                 )
             else:
                 self.adapters.append(adapter_object)
-                logger.info(
+                logger.success(
                     f'Succeeded to load adapter "{adapter_object.__class__.__name__}" '
                     f'from "{adapter_}"'
                 )
 
     def load_adapters(self, *adapters: Union[Type[Adapter], str]):
         """加载适配器。
```

### Comparing `iamai-3.14.2/iamai/config.py` & `iamai-3.14.4/iamai/config.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/event.py` & `iamai-3.14.4/iamai/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 """iamai 事件。
 
 事件类的基类。适配器开发者应实现此事件类基类的子类。
 """
 from abc import ABC
 from typing import Any, Generic, Optional
 
-from pydantic import BaseModel, PrivateAttr
-
 from iamai.message import Message
 from iamai.typing import T_Adapter
 from iamai.utils import DataclassEncoder
+from pydantic import BaseModel, PrivateAttr
 
 __all__ = ["Event"]
 
 
 class Event(ABC, BaseModel, Generic[T_Adapter]):
     """事件类的基类。
```

### Comparing `iamai-3.14.2/iamai/exceptions.py` & `iamai-3.14.4/iamai/exceptions.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/message.py` & `iamai-3.14.4/iamai/message.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/plugin.py` & `iamai-3.14.4/iamai/plugin.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/typing.py` & `iamai-3.14.4/iamai/typing.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/iamai/utils.py` & `iamai-3.14.4/iamai/utils.py`

 * *Files identical despite different names*

### Comparing `iamai-3.14.2/PKG-INFO` & `iamai-3.14.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamai
-Version: 3.14.2
+Version: 3.14.4
 Summary: bot framework.
 Home-page: https://retrofor.space/
 License: MIT
 Keywords: bot,qq,qqbot,mirai,coolq
 Author: 简律纯
 Author-email: admin@jyunko.cn
 Requires-Python: >=3.8,<4.0
@@ -15,30 +15,24 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: aiohttp
 Provides-Extra: all
-Provides-Extra: fastapi
-Provides-Extra: httpx
-Provides-Extra: quart
-Provides-Extra: websockets
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "aiohttp" or extra == "all"
-Requires-Dist: apscheduler (>=3.10.0,<4.0.0)
-Requires-Dist: fastapi (>=0.87.0,!=0.89.0,<1.0.0) ; extra == "fastapi" or extra == "all"
-Requires-Dist: flask (>=2.2.2,<3.0.0)
+Provides-Extra: apscheduler
+Provides-Extra: cqhttp
+Provides-Extra: dingtalk
+Provides-Extra: hot-reload
+Requires-Dist: aiohttp (>=3.8.0,<4.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: onedice (>=1.0.5,<2.0.0)
-Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: watchfiles (>=0.18.1,<0.19.0)
+Requires-Dist: pydantic (>=1.10.0,<2.0.0)
+Requires-Dist: tomli (>=2.0.0,<3.0.0) ; python_version < "3.11"
+Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
 Project-URL: Documentation, https://iamai.retrofor.space/
 Project-URL: Repository, https://github.com/retrofor/iamai
 Description-Content-Type: text/markdown
 
 <p align="center"><img width="128" src="https://iamai.retrofor.space/retro.png"></p>
 <h1 align="center">
   iamai
@@ -124,15 +118,15 @@
 - 🎪 **Interactive [docs](https://iamai.retrofor.space) &amp; [demos](https://iamai.retrofor.space/demos)**
 - 🕶 **Seamless migration**: Works for **both** [Rasa]() and [GPT]() and more...
 - ⚡ **Fully tree shakeable**: Only take what you want, [bundle size](https://iamai.retrofor.space/export-size)
 - 🔩 **Flexible**: Configurable event filters and targets
 - 🔌 **Optional [Add-ons](https://iamai.retrofor.space/add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler), etc.
 - 👍 **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter](https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/adapters/github), etc.
 
-<p align="center"><img width="512" src="https://iamai.retrofor.space/logo.png"></p>
+<p align="center"><img width="512" src="https://iamai.retrofor.space/icons/retro_plus.png"></p>
 
 ## ⬇️ Install
 
 - STABLE VERSION
 
   ```sh
   pip install iamai
```

#### html2text {}

```diff
@@ -1,28 +1,25 @@
-Metadata-Version: 2.1 Name: iamai Version: 3.14.2 Summary: bot framework. Home-
+Metadata-Version: 2.1 Name: iamai Version: 3.14.4 Summary: bot framework. Home-
 page: https://retrofor.space/ License: MIT Keywords: bot,qq,qqbot,mirai,coolq
 Author: ç®å¾çº¯ Author-email: admin@jyunko.cn Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable Classifier: Framework
 :: Robot Framework Classifier: Framework :: Robot Framework :: Library
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Provides-Extra: aiohttp Provides-Extra: all Provides-Extra: fastapi
-Provides-Extra: httpx Provides-Extra: quart Provides-Extra: websockets
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "aiohttp" or extra == "all"
-Requires-Dist: apscheduler (>=3.10.0,<4.0.0) Requires-Dist: fastapi
-(>=0.87.0,!=0.89.0,<1.0.0) ; extra == "fastapi" or extra == "all" Requires-
-Dist: flask (>=2.2.2,<3.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-
-Dist: onedice (>=1.0.5,<2.0.0) Requires-Dist: pydantic (>=1.10.4,<2.0.0)
-Requires-Dist: tomli (>=2.0.1,<3.0.0) Requires-Dist: typing-extensions
-(>=4.5.0,<5.0.0) Requires-Dist: watchfiles (>=0.18.1,<0.19.0) Project-URL:
-Documentation, https://iamai.retrofor.space/ Project-URL: Repository, https://
-github.com/retrofor/iamai Description-Content-Type: text/markdown
+Python :: 3 Provides-Extra: all Provides-Extra: apscheduler Provides-Extra:
+cqhttp Provides-Extra: dingtalk Provides-Extra: hot-reload Requires-Dist:
+aiohttp (>=3.8.0,<4.0.0) Requires-Dist: loguru (>=0.6.0,<0.7.0) Requires-Dist:
+pydantic (>=1.10.0,<2.0.0) Requires-Dist: tomli (>=2.0.0,<3.0.0) ;
+python_version < "3.11" Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
+Project-URL: Documentation, https://iamai.retrofor.space/ Project-URL:
+Repository, https://github.com/retrofor/iamai Description-Content-Type: text/
+markdown
                    [https://iamai.retrofor.space/retro.png]
                               ****** iamai ******
                                [Discord] [QQç¾¤]
                       ç®ä½ä¸­æ ã«ã»ãã íêµ­ì´
             Cross-platform robot framework, mainly used for ML/DL.
                              [Website] [Website]
                                [pypi] [python]
@@ -58,15 +55,15 @@
 filters and targets - ð **Optional [Add-ons](https://iamai.retrofor.space/
 add-ons)**: [Apscheduler](https://iamai.retrofor.space/add-ons/apscheduler),
 etc. - ð **Cross-platform**: [Onebot](https://iamai.retrofor.space/adapters/
 onebot), [Wechat](https://iamai.retrofor.space/adapters/wechat), [Twitter]
 (https://iamai.retrofor.space/adapters/twitter), [Bilibili](https://
 iamai.retrofor.space/adapters/bilibili), [Github](https://iamai.retrofor.space/
 adapters/github), etc.
-                    [https://iamai.retrofor.space/logo.png]
+              [https://iamai.retrofor.space/icons/retro_plus.png]
 ## â¬ï¸ Install - STABLE VERSION ```sh pip install iamai ``` or you can also
 install for TEST. - TEST VERSION ```sh pip install -i https://test.pypi.org/
 simple/ iamai ``` ## â Usage firstly, you need to load an adapter. ```python
 from iamai import Bot bot = Bot() bot.load_adapters("iamai.adapter.cqhttp")
 bot.run() ``` then, you need load the transformer and use your models.
 **transformer(Use from the ð¤/transformers library)** ```python from
 transformers import AutoModelWithLMHead, AutoTokenizer # load models model =
```

