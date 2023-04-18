# Comparing `tmp/nonebot_plugin_tts_gal-0.3.8.tar.gz` & `tmp/nonebot_plugin_tts_gal-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tts_gal-0.3.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_tts_gal-0.3.9.tar", max compression
```

## Comparing `nonebot_plugin_tts_gal-0.3.8.tar` & `nonebot_plugin_tts_gal-0.3.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1081 2022-09-20 04:49:48.895524 nonebot_plugin_tts_gal-0.3.8/LICENSE
--rw-r--r--   0        0        0     7917 2023-01-12 10:41:17.971827 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/__init__.py
--rw-r--r--   0        0        0    11979 2023-01-12 09:38:22.473816 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/attentions.py
--rw-r--r--   0        0        0  5018988 2023-01-12 09:38:22.514597 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/cc_cedict_local.py
--rw-r--r--   0        0        0     2540 2023-01-12 09:38:22.514597 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/commons.py
--rw-r--r--   0        0        0     1012 2023-01-12 09:38:22.515593 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/config.py
--rw-r--r--   0        0        0     1394 2023-01-12 09:38:22.515593 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/depends.py
--rw-r--r--   0        0        0    10671 2023-01-12 10:25:47.114290 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/function.py
--rw-r--r--   0        0        0     2510 2023-01-12 09:38:22.557448 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/initial.py
--rw-r--r--   0        0        0   171271 2023-01-12 09:38:22.558453 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/kmandarin_8105_local.py
--rw-r--r--   0        0        0     3666 2023-01-12 09:38:22.559452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/mel_processing.py
--rw-r--r--   0        0        0    19715 2023-01-12 09:38:22.559452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/models.py
--rw-r--r--   0        0        0    13427 2023-01-12 09:38:22.559452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/modules.py
--rw-r--r--   0        0        0      634 2023-01-12 09:38:22.559452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/monotonic_align/__init__.py
--rw-r--r--   0        0        0      978 2023-01-12 09:38:22.560452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/monotonic_align/core.py
--rw-r--r--   0        0        0     1723 2023-01-12 09:38:22.560452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/__init__.py
--rw-r--r--   0        0        0     8578 2023-01-12 09:38:22.560452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/cleaners.py
--rw-r--r--   0        0        0     1072 2023-01-12 09:38:22.560452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/LICENSE
--rw-r--r--   0        0        0     2115 2023-01-12 09:38:22.561452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/symbols.py
--rw-r--r--   0        0        0     8683 2023-01-12 09:38:22.561452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/transforms.py
--rw-r--r--   0        0        0     1692 2023-01-12 09:38:22.561452 nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/utils.py
--rw-r--r--   0        0        0      811 2023-01-12 09:38:22.562452 nonebot_plugin_tts_gal-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     9648 2023-01-12 09:38:22.466816 nonebot_plugin_tts_gal-0.3.8/README.md
--rw-r--r--   0        0        0    10836 1970-01-01 00:00:00.000000 nonebot_plugin_tts_gal-0.3.8/setup.py
--rw-r--r--   0        0        0    10650 1970-01-01 00:00:00.000000 nonebot_plugin_tts_gal-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-09-20 04:49:48.895524 nonebot_plugin_tts_gal-0.3.9/LICENSE
+-rw-r--r--   0        0        0     7858 2023-04-09 14:20:55.069098 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/__init__.py
+-rw-r--r--   0        0        0    11979 2023-04-09 14:20:55.069098 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/attentions.py
+-rw-r--r--   0        0        0  5018988 2023-04-09 14:20:55.092022 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/cc_cedict_local.py
+-rw-r--r--   0        0        0     2540 2023-04-09 14:20:55.092022 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/commons.py
+-rw-r--r--   0        0        0     1012 2023-04-09 14:20:55.092022 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/config.py
+-rw-r--r--   0        0        0     1394 2023-04-09 14:20:55.092022 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/depends.py
+-rw-r--r--   0        0        0    11017 2023-04-09 14:20:55.093017 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/function.py
+-rw-r--r--   0        0        0     2510 2023-04-09 14:20:55.093017 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/initial.py
+-rw-r--r--   0        0        0   171271 2023-04-09 14:20:55.094010 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/kmandarin_8105_local.py
+-rw-r--r--   0        0        0     3666 2023-04-09 14:20:55.094010 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/mel_processing.py
+-rw-r--r--   0        0        0    19715 2023-04-09 14:20:55.095011 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/models.py
+-rw-r--r--   0        0        0    13427 2023-04-09 14:20:55.095011 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/modules.py
+-rw-r--r--   0        0        0      634 2023-04-09 14:20:55.095011 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/monotonic_align/__init__.py
+-rw-r--r--   0        0        0      978 2023-04-09 14:20:55.095011 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/monotonic_align/core.py
+-rw-r--r--   0        0        0     1723 2023-04-09 14:20:55.096007 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/__init__.py
+-rw-r--r--   0        0        0     8578 2023-04-09 14:20:55.096007 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/cleaners.py
+-rw-r--r--   0        0        0     1072 2023-04-09 14:20:55.095011 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/LICENSE
+-rw-r--r--   0        0        0     2115 2023-04-09 14:20:55.096007 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/symbols.py
+-rw-r--r--   0        0        0     8683 2023-04-09 14:20:55.096007 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/transforms.py
+-rw-r--r--   0        0        0     1794 2023-04-09 14:20:55.096007 nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/utils.py
+-rw-r--r--   0        0        0      811 2023-04-09 14:20:55.097004 nonebot_plugin_tts_gal-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     9862 2023-04-09 14:20:55.062121 nonebot_plugin_tts_gal-0.3.9/README.md
+-rw-r--r--   0        0        0    11050 1970-01-01 00:00:00.000000 nonebot_plugin_tts_gal-0.3.9/setup.py
+-rw-r--r--   0        0        0    10858 1970-01-01 00:00:00.000000 nonebot_plugin_tts_gal-0.3.9/PKG-INFO
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/LICENSE` & `nonebot_plugin_tts_gal-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/__init__.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,37 +21,33 @@
 
 from .depends import *
 from .initial import *
 from .config import *
 from .utils import *
 from .models import SynthesizerTrn
 from .function import *
-from .text.symbols import symbols_ja, symbols_zh_CHS
 
 
 __plugin_meta__ = PluginMetadata(
     name="vits角色语音合成本地化",
     description="基于nonebot2和vits的本地化角色语音合成插件",
     usage=f"触发方式：{trigger_rule}[角色名][发送|说][文本内容]\n"+
         "※超级用户管理(若设置前缀，以下均加上前缀)\n"+
         f"   {trigger_rule}[禁用翻译 xxx]   禁用xxx翻译项\n"+
         f"   {trigger_rule}[启用翻译 xxx]   启用xxx翻译项\n"+
         f"   {trigger_rule}[查看翻译]         查看目前可用的翻译项\n"+
         f"   {trigger_rule}[查看禁用翻译]  查看已被禁用的翻译项",
     extra={
         "example": f"{trigger_rule} 宁宁说おはようございます.",
         "author": "dpm12345 <1006975692@qq.com>",
-        "version": "0.3.8",
+        "version": "0.3.9",
     },
 )
 
-symbols_dict = {
-    "zh-CHS": symbols_zh_CHS,
-    "ja": symbols_ja
-}
+
 
 
 auto_delete_voice = tts_gal_config.auto_delete_voice
 tts_gal = eval(tts_gal_config.tts_gal)
 tran_type = tts_gal_config.tts_gal_tran_type
 prefix = tts_gal_config.tts_gal_prefix
 priority = tts_gal_config.tts_gal_priority
@@ -60,15 +56,15 @@
 lock_tran_list = {
     "auto":[],
     "manual":[]
 }
 
 
 @driver.on_startup
-def _():
+async def _():
     logger.info("正在检查目录是否存在...")
     asyncio.ensure_future(checkDir(data_path, base_path, voice_path, model_path, config_path))
     filenames = []
     [filenames.append(model[0])
      for model in tts_gal.values() if not model[0] in filenames]
     logger.info("正在检查配置文件是否存在...")
     asyncio.ensure_future(checkFile(model_path, config_path, filenames, tts_gal, __plugin_meta__, __valid_names__))
@@ -97,15 +93,17 @@
     first_name = "".join(random.sample([x for x in string.ascii_letters + string.digits], 8))
     filename = hashlib.md5(first_name.encode()).hexdigest() + ".mp3"
     # 加载配置文件
     hps_ms = get_hparams_from_file(config_path / config_file)
 
     # 翻译的目标语言
     lang = load_language(hps_ms)
-    symbols = load_symbols(hps_ms, lang, symbols_dict)
+    symbols = load_symbols(hps_ms, lang)
+    if not symbols:
+        await voice.finish("symbols项配置错误")
 
     # 文本处理
     text = changeE2C(text) if lang == "zh-CHS" else changeC2E(text)
     text = await translate(tran_type, lock_tran_list, text, lang)
     if not text:
         await voice.finish("翻译文本时出错,请查看日志获取细节")
     text = get_text(text, hps_ms, symbols, lang, False)
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/attentions.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/attentions.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/cc_cedict_local.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/cc_cedict_local.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/commons.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/commons.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/config.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/depends.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/depends.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/function.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/function.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,18 +11,25 @@
 import os
 from .text import text_to_sequence
 from .commons import intersperse
 from torch import no_grad, LongTensor
 from .utils import *
 from nonebot.log import logger
 from .config import tts_gal_config
-from typing import List, Tuple, Dict
+from typing import List, Tuple, Dict, Union
+from pathlib import Path
 from sys import maxsize
+from .text.symbols import *
 
 
+symbols_dict = {
+    "zh-CHS": symbols_zh_CHS,
+    "ja": symbols_ja
+}
+
 def check_character(name, valid_names, tts_gal):
     index = None
     config_file = ""
     model_file = ""
     for names, model in tts_gal.items():
         if names in valid_names and \
                 ((isinstance(names, str) and names == name) or
@@ -40,25 +47,30 @@
     except:
         logger.info("配置文件中缺少language项,请手动添加(新版本内容),具体填写内容请查看github主页\
             https://github.com/dpm12345/nonebot_plugin_tts_gal/")
         logger.info("将默认使用日语配置项")
         return "ja"
 
 
-def load_symbols(hps_ms, lang, symbols_dict):
+def load_symbols(hps_ms, lang):
     try:
         symbols = hps_ms.symbols
-    except:
+        if isinstance(symbols,str):
+            symbols = eval(symbols)
+    except AttributeError:
         logger.info("配置文件中缺失symbols项,建议手动添加")
         if lang in symbols_dict.keys():
             logger.info("采用language指定的symbols项")
             symbols = symbols_dict[lang]
         else:
             logger.info("该语言未有默认symbols项，将采用日语symbols")
             symbols = symbols_dict["ja"]
+    except NameError:
+        logger.error(f"不存在{symbols}项")
+        symbols = None
     return symbols
 
 
 def get_text(text, hps, symbols, lang, cleaned=False):
     if cleaned:
         text_norm = text_to_sequence(text, symbols, [], lang)
     else:
@@ -266,25 +278,26 @@
     "youdao": translate_youdao,
     "baidu": translate_baidu,
     "tencent": translate_tencent
 }
 
 
 async def translate(tran_type: List[str], lock_tran_list: Dict[str, List[str]], text: str, lang: str) -> str:
+    res = ""
     for tran in tran_type:
         if tran not in lock_tran_list["manual"] and tran not in lock_tran_list["auto"]:
             res, flag = await support_tran[tran](text, lang)
             if flag:
                 lock_tran_list["auto"].append(tran)
             if res:
                 break
     return res
 
 
-def change_by_decibel(audio_path: str, output_dir: str, decibel):
+def change_by_decibel(audio_path: Union[str,Path], output_dir: Union[str,Path], decibel):
     ext = os.path.basename(audio_path).strip().split('.')[-1]
     if ext not in ['wav', 'mp3']:
         raise Exception('format error')
     new_name = uuid.uuid4()
     ff = FFmpeg(inputs={'{}'.format(audio_path): None},
                 outputs={os.path.join(output_dir, '{}.{}'.format(new_name, ext)): '-filter:a "volume={}dB" -loglevel quiet'.format(decibel)})
     ff.run()
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/initial.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/initial.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/kmandarin_8105_local.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/kmandarin_8105_local.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/mel_processing.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/mel_processing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/models.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/modules.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/modules.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/monotonic_align/__init__.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/monotonic_align/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/monotonic_align/core.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/monotonic_align/core.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/__init__.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/cleaners.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/cleaners.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/LICENSE` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/text/symbols.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/text/symbols.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/transforms.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/transforms.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tts_gal-0.3.8/nonebot_plugin_tts_gal/utils.py` & `nonebot_plugin_tts_gal-0.3.9/nonebot_plugin_tts_gal/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,13 +57,17 @@
     model.load_state_dict(new_state_dict)
   logging.info("Loaded checkpoint '{}' (iteration {})" .format(
     checkpoint_path, iteration))
   return
 
 
 def get_hparams_from_file(config_path):
-  with open(config_path, "r") as f:
-    data = f.read()
+  try:
+    with open(config_path, "r") as f:
+      data = f.read()
+  except:
+    with open(config_path, "r",encoding="utf-8") as f:
+      data = f.read()
   config = loads(data)
 
   hparams = HParams(**config)
   return hparams
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/pyproject.toml` & `nonebot_plugin_tts_gal-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_tts_gal"
-version = "0.3.8"
+version = "0.3.9"
 description = "基于nonebot2和vits的本地化角色语音合成插件"
 authors = ["dpm12345 <1006975692@qq.com>"]
 readme = "README.md"
 homepage = "https://github.com/dpm12345/nonebot_plugin_tts_gal"
 repository = "https://github.com/dpm12345/nonebot_plugin_tts_gal"
 license = "MIT"
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/README.md` & `nonebot_plugin_tts_gal-0.3.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -83,17 +83,17 @@
 </details>
 
 ## ⚙️ 配置
 
 | 配置项  | 必填 | 类型 | 默认值 |  说明  |
 | :-----: | :--: | :----: | :----: | :-----: |
 | tts_gal |  是  | Dict[Tuble[str],List[str]] | {():[""]} | 生成指定角色语音的关键配置，具体可见[tts_gal的配置要求](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82) |
-| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否<br>(配置文件中请填`true`或`false`) |
+| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否 |
 | decibel | 否 | int | -10 | 发送语音相对生成的分贝数<br>(原生成的音频音量可能比较大，因此通过此项来降低，负数为降，整数位升) |
-| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人，<br>(若填写，填`true`或`false`) |
+| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人 |
 | tts_gal_prefix | 否 | str | ""(空) | 使用该插件时的触发匹配前缀，减少冲突 |
 | tts_gal_priority | 否 | int | 3 | 该插件的优先级大小 |
 | tts_gal_tran_type | 否 | List[str] | ["youdao"] | 文本翻译使用项，默认为有道翻译("youdao")，可支持百度翻译("baidu")和腾讯翻译("tencent")，填写顺序为翻译调用优先级，若填写百度和腾讯翻译后需填写对应的配置项 |
 | baidu_tran_appid | 否 | str | ""(空) | 百度翻译接口对应的appid，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |
 | baidu_tran_apikey | 否 | str | ""(空) | 百度翻译接口对应的apikey，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |
 | tencent_tran_region | 否 | str | "ap-shanghai" | 腾讯翻译接口对应的地域，可在[地域列表](https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8)获取 |
 | tencent_tran_secretid | 否 | str | ""(空) | 腾讯翻译接口对应secretid，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |
@@ -199,14 +199,20 @@
 
 + 部分代码参考自[nonebot-plugin-petpet](https://github.com/noneplugin/nonebot-plugin-petpet)
 + **[CjangCjengh](https://github.com/CjangCjengh/)**：g2p转换，适用于日语调形标注的符号文件及分享的[柚子社多人模型](https://github.com/CjangCjengh/TTSModels)
 + **[luoyily](https://github.com/luoyily)**：分享的[ATRI模型](https://pan.baidu.com/s/1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4)
 
 ## 📝 更新日志
 
+**2023.4.9 version 0.3.9：**
+
+支持添加生成symbols的代码，以便添加更多的symbols,详见[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E5%85%B3%E4%BA%8Esymbols)
+
+fix bug [#39](https://github.com/dpm12345/nonebot_plugin_tts_gal/issues/39)
+
 **2023.1.12 version 0.3.8：**
 
 修复regex的匹配问题
 
 **2023.1.11 version 0.3.7：**
 
 支持百度翻译和腾讯翻译的api使用，增加是否需要@机器人、自定义前缀、自定义插件priority等配置
```

#### html2text {}

```diff
@@ -26,21 +26,19 @@
 éç½® | éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | :-----: | :--: |
 :----: | :----: | :-----: | | tts_gal | æ¯ | Dict[Tuble[str],List[str]] | {():
 [""]} | çææå®è§è²è¯­é³çå³é®éç½®ï¼å·ä½å¯è§
 [tts_galçéç½®è¦æ±](https://github.com/dpm12345/nonebot_plugin_tts_gal/
 blob/master/
 Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82)
 | | auto_delete_voice | å¦ | Bool | True |
-æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦
-(éç½®æä»¶ä¸­è¯·å¡«`true`æ`false`) | | decibel | å¦ | int | -10 |
-åéè¯­é³ç¸å¯¹çæçåè´æ°
+æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦ | | decibel | å¦
+| int | -10 | åéè¯­é³ç¸å¯¹çæçåè´æ°
 (åçæçé³é¢é³éå¯è½æ¯è¾å¤§ï¼å æ­¤éè¿æ­¤é¡¹æ¥éä½ï¼è´æ°ä¸ºéï¼æ´æ°ä½å)
-| | tts_gal_is_at | å¦ | Bool | True |
-ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äººï¼
-(è¥å¡«åï¼å¡«`true`æ`false`) | | tts_gal_prefix | å¦ | str | ""(ç©º) |
+| | tts_gal_is_at | å¦ | Bool | True | ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äºº |
+| tts_gal_prefix | å¦ | str | ""(ç©º) |
 ä½¿ç¨è¯¥æä»¶æ¶çè§¦åå¹éåç¼ï¼åå°å²çª | | tts_gal_priority |
 å¦ | int | 3 | è¯¥æä»¶çä¼åçº§å¤§å° | | tts_gal_tran_type | å¦ | List
 [str] | ["youdao"] | ææ¬ç¿»è¯ä½¿ç¨é¡¹ï¼é»è®¤ä¸ºæéç¿»è¯
 ("youdao")ï¼å¯æ¯æç¾åº¦ç¿»è¯("baidu")åè¾è®¯ç¿»è¯
 ("tencent")ï¼å¡«åé¡ºåºä¸ºç¿»è¯è°ç¨ä¼åçº§ï¼è¥å¡«åç¾åº¦åè¾è®¯ç¿»è¯åéå¡«åå¯¹åºçéç½®é¡¹
 | | baidu_tran_appid | å¦ | str | ""(ç©º) |
 ç¾åº¦ç¿»è¯æ¥å£å¯¹åºçappidï¼å¯å¨[ç¾åº¦ç¿»è¯æ§å¶å°](https://fanyi-
@@ -100,16 +98,21 @@
 å¦æåºç°ä¸è½½open_jtalkçéè¯¯ä¿¡æ¯ï¼å¯ä»¥åæ¬¡å°è¯ï¼å¦æå®å¨ä¸è¡ï¼å¯ä»¥ä½¿ç¨`pip
 install openjtalk`  ## ð¡ é¸£è°¢ + é¨åä»£ç åèèª[nonebot-plugin-
 petpet](https://github.com/noneplugin/nonebot-plugin-petpet) + **[CjangCjengh]
 (https://github.com/CjangCjengh/
 )**ï¼g2pè½¬æ¢ï¼éç¨äºæ¥è¯­è°å½¢æ æ³¨çç¬¦å·æä»¶ååäº«ç
 [æå­ç¤¾å¤äººæ¨¡å](https://github.com/CjangCjengh/TTSModels) + **[luoyily]
 (https://github.com/luoyily)**ï¼åäº«ç[ATRIæ¨¡å](https://pan.baidu.com/s/
-1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4) ## ð æ´æ°æ¥å¿ **2023.1.12 version
-0.3.8ï¼** ä¿®å¤regexçå¹éé®é¢ **2023.1.11 version 0.3.7ï¼**
+1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4) ## ð æ´æ°æ¥å¿ **2023.4.9 version
+0.3.9ï¼**
+æ¯ææ·»å çæsymbolsçä»£ç ï¼ä»¥ä¾¿æ·»å æ´å¤çsymbols,è¯¦è§
+[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/
+Usage.md#%E5%85%B3%E4%BA%8Esymbols) fix bug [#39](https://github.com/dpm12345/
+nonebot_plugin_tts_gal/issues/39) **2023.1.12 version 0.3.8ï¼**
+ä¿®å¤regexçå¹éé®é¢ **2023.1.11 version 0.3.7ï¼**
 æ¯æç¾åº¦ç¿»è¯åè¾è®¯ç¿»è¯çapiä½¿ç¨ï¼å¢å æ¯å¦éè¦@æºå¨äººãèªå®ä¹åç¼ãèªå®ä¹æä»¶priorityç­éç½®
 **2022.12.9 version 0.3.3ï¼** èªå¨è¯»åå·²å è½½çè§è²æ¨¡åï¼å¯éè¿
 [PicMenuæä»¶](https://github.com/hamo-reid/
 nonebot_plugin_PicMenu)è¿è¡æ¾ç¤ºå¯ä½¿ç¨çè§è²;å¯¹ä»£ç è¿è¡ç¸å³ä¼å
 **2022.10.27 version 0.3.2ï¼** ä¿®æ¹æ­£åè¡¨è¾¾å¼ï¼é¿åææ¬åºç°"è¯´/
 åé"èé ænameçå¹ééè¯¯ **2022.10.21 version 0.3.1ï¼**
 ä¿®å¤å¯¹éç½®é¡¹auto_delete_voiceçå¤æ­bug **2022.10.19 version 0.3.0ï¼**
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/setup.py` & `nonebot_plugin_tts_gal-0.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,17 +23,17 @@
  'pypinyin>=0.47.0,<0.48.0',
  'scipy>=1.5.2,<2.0.0',
  'torch>=1.6.0,<2.0.0',
  'unidecode>=1.1.1,<2.0.0']
 
 setup_kwargs = {
     'name': 'nonebot-plugin-tts-gal',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '基于nonebot2和vits的本地化角色语音合成插件',
-    'long_description': '\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-tts-gal\n\n_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 基于nonebot2和vits的本地化角色语音合成插件 ✨_\n\n<p align="center">\n  <a href="https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/LICENSE">\n    <img src="https://img.shields.io/github/license/dpm12345/nonebot_plugin_tts_gal.svg" alt="license">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">\n  <img src="https://img.shields.io/badge/nonebot-2.0.0b4+-red.svg" alt="NoneBot">\n  <a href="https://pypi.org/project/nonebot-plugin-tts-gal">\n    <img src="https://badgen.net/pypi/v/nonebot-plugin-tts-gal" alt="pypi">\n  </a>\n</p>\n\n</div>\n\n## 💬 前言\n\n平时因为学业问题，有时可能会回复得比较慢，请见谅。\n\n## 📖 介绍\n\nvits的nonebot的本地化插件，使用已训练好的模型，按照配置要求，使机器人发送文本对应的语音\n\n(**PS: 语音生成比较吃配置，生成过程花费时间可能会比较长，且大文本量会占用较大内存，过大会导致机器人进程 killed ，请留意**)\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n\n    nb plugin install nonebot-plugin-tts-gal\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n\n    pip install nonebot_plugin_tts_gal\n\n</details>\n\n## 🍰 资源文件\n\n`data`文件夹中的`nonebot_plugin_tts_gal`会存储与插件有关的文件\n\n可以安装完插件后运行一次自动建立再退出\n\n也可以按照该页面的`data`文件夹进行手动建立\n\n具体的资源下载示例请查看[例子示例](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E4%BE%8B%E5%AD%90%E7%A4%BA%E4%BE%8B)\n\n## 💻 相关依赖\n\n<details>\n<summary>ffmpeg的安装</summary> \n\n**Windows**\n\n在ffmpeg官网[下载](https://github.com/BtbN/FFmpeg-Builds/releases),选择对应的版本，下载后解压，并将位于`bin`目录添加到环境变量中\n\n其他具体细节可自行搜索\n\n**Linux**\n\nUbuntu下\n\n```\napt-get install ffmpeg\n```\n\n或者下载源码安装(具体可搜索相关教程)\n\n</details>\n\n## ⚙️ 配置\n\n| 配置项  | 必填 | 类型 | 默认值 |  说明  |\n| :-----: | :--: | :----: | :----: | :-----: |\n| tts_gal |  是  | Dict[Tuble[str],List[str]] | {():[""]} | 生成指定角色语音的关键配置，具体可见[tts_gal的配置要求](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82) |\n| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否<br>(配置文件中请填`true`或`false`) |\n| decibel | 否 | int | -10 | 发送语音相对生成的分贝数<br>(原生成的音频音量可能比较大，因此通过此项来降低，负数为降，整数位升) |\n| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人，<br>(若填写，填`true`或`false`) |\n| tts_gal_prefix | 否 | str | ""(空) | 使用该插件时的触发匹配前缀，减少冲突 |\n| tts_gal_priority | 否 | int | 3 | 该插件的优先级大小 |\n| tts_gal_tran_type | 否 | List[str] | ["youdao"] | 文本翻译使用项，默认为有道翻译("youdao")，可支持百度翻译("baidu")和腾讯翻译("tencent")，填写顺序为翻译调用优先级，若填写百度和腾讯翻译后需填写对应的配置项 |\n| baidu_tran_appid | 否 | str | ""(空) | 百度翻译接口对应的appid，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |\n| baidu_tran_apikey | 否 | str | ""(空) | 百度翻译接口对应的apikey，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |\n| tencent_tran_region | 否 | str | "ap-shanghai" | 腾讯翻译接口对应的地域，可在[地域列表](https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8)获取 |\n| tencent_tran_secretid | 否 | str | ""(空) | 腾讯翻译接口对应secretid，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |\n| tencent_tran_secretkey | 否 | str | ""(空) | 腾讯翻译接口对应secretkey，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |\n| tencent_tran_projectid | 否 | int | 0 | 腾讯翻译接口对应projectid，该项可以根据控制台-账号中心-项目管理中的配置填写，如无配置请填写默认项目ID:0或不填 |\n\n\n## 🎉 使用\n\n群聊和私聊仅有细微差别，其中下面语句中，`name`为合成语音的角色，`text`为转语音的文本内容(根据模型配置文件中的`language`会自动翻译为对应语言)，具体的相关功能解释可查看[这里](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E5%8A%9F%E8%83%BD%E8%A7%A3%E9%87%8A)\n\n| 指令 | 可使用者 |  说明   |\n| :---: | :----: | :-----: |\n| [name]说[text]<br>或<br>[name]发送[text] | 所有人 | 生成语音，<br>若配置了`tts_gal_is_at`为`true`和`tts_gal_prefix`不为空，<br>那么分别要@机器人和在`name`前添加配置的前缀，<br>如设置前缀`tts`，那么使用时为 tts[name]说[text] |\n| 禁用翻译 xxx | 超级用户(SUPERUSER) | 禁用名为xxx的翻译项，在启用前都不会使用xxx的翻译 |\n| 启用翻译 xxx | 超级用户(SUPERUSER) | 启用名为xxx的翻译项，将会使用xxx的翻译(按原来配置设置的优先级) |\n| 查看翻译 | 超级用户(SUPERUSER) | 查看插件目前调用的翻译项 |\n| 查看禁用翻译 | 超级用户(SUPERUSER) | 查看插件目前禁用的翻译项 |\n\n例如：\n+ 宁宁说おはようございます.\n+ 禁用翻译 baidu\n+ 启用翻译 baidu\n+ 查看翻译\n+ 查看禁用翻译\n\n## ✏️ 今后\n\n添加更多的模型\n\n添加更多的翻译选项\n\n\n## ❔ Q&A\n\n<details>\n<summary>安装pyopenjtalk</summary> \n\n如果出现如下错误\n\n<img src="./images/nonebot_plugin_tts_gal_3.jpg" alt="图3" style="zoom:80%;" />\n\n可能由于缺少cmake和MSVC造成的，需要在本机安装\n\n## Windows\n\n### 第一步 安装Visual Studio\n\n在Visual Studio的官网下载安装器,[VS2022点击此处下载](https://visualstudio.microsoft.com/zh-hans/free-developer-offers/)\n\n下载社区版，即`Visual Studio Community`\n\n### 第二步 下载相关工具\n\n下载后点击，进入如图所示先点击修改，然后选择如图所示的项目\n\n<img src="./images/nonebot_plugin_tts_gal_1.jpg" alt="图1" style="zoom:50%;" />\n\n<img src="./images/nonebot_plugin_tts_gal_2.jpg" alt="图2" style="zoom:50%;" />\n\n### 第三步 设置环境变量\n\n下载好后，在安装目录中找到cmake和MSVC的bin目录\n\n下面是参考目录,前面的目录即为之前强调的路径\n\n```\nE:\\Program Files (x86)\\Microsoft Visual Studio\\2022\\Community\\Common7\\IDE\\CommonExtensions\\Microsoft\\CMake\\CMake\\bin\n\nE:\\Program Files (x86)\\Microsoft Visual Studio\\2022\\Community\\VC\\Tools\\MSVC\\14.32.31326\\bin\\Hostx86\\x64\n\n```\n\n将这两个目录添加到环境变量中\n\n这样，windows安装pyopenjtalk的前置依赖便解决了\n\n## Linux\n\nLinux如出现以下情况\n\n<img src="./images/nonebot_plugin_tts_gal_4.jpg" alt="图4" style="zoom:50%;" />\n\n原因为缺少cmake工具，可以使用apt命令下载安装\n\n```\nsudo apt install cmake\n```\n\n安装好后便可安装pyopenjtalk\n</details>\n\n</details>\n\n<details>\n<summary>无法生成语音</summary> \n\n如果出现下载open_jtalk的错误信息，可以再次尝试，如果实在不行，可以使用`pip install openjtalk`\n\n</details>\n\n## 💡 鸣谢\n\n+ 部分代码参考自[nonebot-plugin-petpet](https://github.com/noneplugin/nonebot-plugin-petpet)\n+ **[CjangCjengh](https://github.com/CjangCjengh/)**：g2p转换，适用于日语调形标注的符号文件及分享的[柚子社多人模型](https://github.com/CjangCjengh/TTSModels)\n+ **[luoyily](https://github.com/luoyily)**：分享的[ATRI模型](https://pan.baidu.com/s/1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4)\n\n## 📝 更新日志\n\n**2023.1.12 version 0.3.8：**\n\n修复regex的匹配问题\n\n**2023.1.11 version 0.3.7：**\n\n支持百度翻译和腾讯翻译的api使用，增加是否需要@机器人、自定义前缀、自定义插件priority等配置\n\n**2022.12.9 version 0.3.3：**\n\n自动读取已加载的角色模型，可通过[PicMenu插件](https://github.com/hamo-reid/nonebot_plugin_PicMenu)进行显示可使用的角色;对代码进行相关优化\n\n**2022.10.27 version 0.3.2：**\n\n修改正则表达式，避免文本出现"说/发送"而造成name的匹配错误\n\n**2022.10.21 version 0.3.1：**\n\n修复对配置项auto_delete_voice的判断bug\n\n**2022.10.19 version 0.3.0：**\n\n支持添加中文模型，优化相关代码，增添更多提示\n\n**2022.10.7 version 0.2.3:**\n\n适配nonebot2-rc1版本，并添加部分报错信息提醒\n\n**2022.9.28 version 0.2.2:**\n\n添加中文逗号替换成英文逗号\n\n**version 0.2.1:**\n\n将pyopenjtalk依赖更新为0.3.0，使python3.10也能使用\n\n**2022.9.25 version 0.2.0:**\n\n优化修改代码逻辑，支持自行添加vits模型，简单修复了一下有道翻译的翻译问题，启动时自动检测所需文件是否缺失\n\n**2022.9.21 version 0.1.1:**\n\n修改依赖\n\n',
+    'long_description': '\n<p align="center">\n  <a href="https://v2.nonebot.dev/"><img src="https://v2.nonebot.dev/logo.png" width="200" height="200" alt="nonebot"></a>\n</p>\n\n<div align="center">\n\n# nonebot-plugin-tts-gal\n\n_✨ [Nonebot2](https://github.com/nonebot/nonebot2) 基于nonebot2和vits的本地化角色语音合成插件 ✨_\n\n<p align="center">\n  <a href="https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/LICENSE">\n    <img src="https://img.shields.io/github/license/dpm12345/nonebot_plugin_tts_gal.svg" alt="license">\n  </a>\n  <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="Python">\n  <img src="https://img.shields.io/badge/nonebot-2.0.0b4+-red.svg" alt="NoneBot">\n  <a href="https://pypi.org/project/nonebot-plugin-tts-gal">\n    <img src="https://badgen.net/pypi/v/nonebot-plugin-tts-gal" alt="pypi">\n  </a>\n</p>\n\n</div>\n\n## 💬 前言\n\n平时因为学业问题，有时可能会回复得比较慢，请见谅。\n\n## 📖 介绍\n\nvits的nonebot的本地化插件，使用已训练好的模型，按照配置要求，使机器人发送文本对应的语音\n\n(**PS: 语音生成比较吃配置，生成过程花费时间可能会比较长，且大文本量会占用较大内存，过大会导致机器人进程 killed ，请留意**)\n\n## 💿 安装\n\n<details>\n<summary>nb-cli安装</summary>\n在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装\n\n    nb plugin install nonebot-plugin-tts-gal\n\n</details>\n\n<details>\n<summary>pip安装</summary>\n\n    pip install nonebot_plugin_tts_gal\n\n</details>\n\n## 🍰 资源文件\n\n`data`文件夹中的`nonebot_plugin_tts_gal`会存储与插件有关的文件\n\n可以安装完插件后运行一次自动建立再退出\n\n也可以按照该页面的`data`文件夹进行手动建立\n\n具体的资源下载示例请查看[例子示例](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E4%BE%8B%E5%AD%90%E7%A4%BA%E4%BE%8B)\n\n## 💻 相关依赖\n\n<details>\n<summary>ffmpeg的安装</summary> \n\n**Windows**\n\n在ffmpeg官网[下载](https://github.com/BtbN/FFmpeg-Builds/releases),选择对应的版本，下载后解压，并将位于`bin`目录添加到环境变量中\n\n其他具体细节可自行搜索\n\n**Linux**\n\nUbuntu下\n\n```\napt-get install ffmpeg\n```\n\n或者下载源码安装(具体可搜索相关教程)\n\n</details>\n\n## ⚙️ 配置\n\n| 配置项  | 必填 | 类型 | 默认值 |  说明  |\n| :-----: | :--: | :----: | :----: | :-----: |\n| tts_gal |  是  | Dict[Tuble[str],List[str]] | {():[""]} | 生成指定角色语音的关键配置，具体可见[tts_gal的配置要求](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82) |\n| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否 |\n| decibel | 否 | int | -10 | 发送语音相对生成的分贝数<br>(原生成的音频音量可能比较大，因此通过此项来降低，负数为降，整数位升) |\n| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人 |\n| tts_gal_prefix | 否 | str | ""(空) | 使用该插件时的触发匹配前缀，减少冲突 |\n| tts_gal_priority | 否 | int | 3 | 该插件的优先级大小 |\n| tts_gal_tran_type | 否 | List[str] | ["youdao"] | 文本翻译使用项，默认为有道翻译("youdao")，可支持百度翻译("baidu")和腾讯翻译("tencent")，填写顺序为翻译调用优先级，若填写百度和腾讯翻译后需填写对应的配置项 |\n| baidu_tran_appid | 否 | str | ""(空) | 百度翻译接口对应的appid，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |\n| baidu_tran_apikey | 否 | str | ""(空) | 百度翻译接口对应的apikey，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |\n| tencent_tran_region | 否 | str | "ap-shanghai" | 腾讯翻译接口对应的地域，可在[地域列表](https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8)获取 |\n| tencent_tran_secretid | 否 | str | ""(空) | 腾讯翻译接口对应secretid，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |\n| tencent_tran_secretkey | 否 | str | ""(空) | 腾讯翻译接口对应secretkey，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |\n| tencent_tran_projectid | 否 | int | 0 | 腾讯翻译接口对应projectid，该项可以根据控制台-账号中心-项目管理中的配置填写，如无配置请填写默认项目ID:0或不填 |\n\n\n## 🎉 使用\n\n群聊和私聊仅有细微差别，其中下面语句中，`name`为合成语音的角色，`text`为转语音的文本内容(根据模型配置文件中的`language`会自动翻译为对应语言)，具体的相关功能解释可查看[这里](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E5%8A%9F%E8%83%BD%E8%A7%A3%E9%87%8A)\n\n| 指令 | 可使用者 |  说明   |\n| :---: | :----: | :-----: |\n| [name]说[text]<br>或<br>[name]发送[text] | 所有人 | 生成语音，<br>若配置了`tts_gal_is_at`为`true`和`tts_gal_prefix`不为空，<br>那么分别要@机器人和在`name`前添加配置的前缀，<br>如设置前缀`tts`，那么使用时为 tts[name]说[text] |\n| 禁用翻译 xxx | 超级用户(SUPERUSER) | 禁用名为xxx的翻译项，在启用前都不会使用xxx的翻译 |\n| 启用翻译 xxx | 超级用户(SUPERUSER) | 启用名为xxx的翻译项，将会使用xxx的翻译(按原来配置设置的优先级) |\n| 查看翻译 | 超级用户(SUPERUSER) | 查看插件目前调用的翻译项 |\n| 查看禁用翻译 | 超级用户(SUPERUSER) | 查看插件目前禁用的翻译项 |\n\n例如：\n+ 宁宁说おはようございます.\n+ 禁用翻译 baidu\n+ 启用翻译 baidu\n+ 查看翻译\n+ 查看禁用翻译\n\n## ✏️ 今后\n\n添加更多的模型\n\n添加更多的翻译选项\n\n\n## ❔ Q&A\n\n<details>\n<summary>安装pyopenjtalk</summary> \n\n如果出现如下错误\n\n<img src="./images/nonebot_plugin_tts_gal_3.jpg" alt="图3" style="zoom:80%;" />\n\n可能由于缺少cmake和MSVC造成的，需要在本机安装\n\n## Windows\n\n### 第一步 安装Visual Studio\n\n在Visual Studio的官网下载安装器,[VS2022点击此处下载](https://visualstudio.microsoft.com/zh-hans/free-developer-offers/)\n\n下载社区版，即`Visual Studio Community`\n\n### 第二步 下载相关工具\n\n下载后点击，进入如图所示先点击修改，然后选择如图所示的项目\n\n<img src="./images/nonebot_plugin_tts_gal_1.jpg" alt="图1" style="zoom:50%;" />\n\n<img src="./images/nonebot_plugin_tts_gal_2.jpg" alt="图2" style="zoom:50%;" />\n\n### 第三步 设置环境变量\n\n下载好后，在安装目录中找到cmake和MSVC的bin目录\n\n下面是参考目录,前面的目录即为之前强调的路径\n\n```\nE:\\Program Files (x86)\\Microsoft Visual Studio\\2022\\Community\\Common7\\IDE\\CommonExtensions\\Microsoft\\CMake\\CMake\\bin\n\nE:\\Program Files (x86)\\Microsoft Visual Studio\\2022\\Community\\VC\\Tools\\MSVC\\14.32.31326\\bin\\Hostx86\\x64\n\n```\n\n将这两个目录添加到环境变量中\n\n这样，windows安装pyopenjtalk的前置依赖便解决了\n\n## Linux\n\nLinux如出现以下情况\n\n<img src="./images/nonebot_plugin_tts_gal_4.jpg" alt="图4" style="zoom:50%;" />\n\n原因为缺少cmake工具，可以使用apt命令下载安装\n\n```\nsudo apt install cmake\n```\n\n安装好后便可安装pyopenjtalk\n</details>\n\n</details>\n\n<details>\n<summary>无法生成语音</summary> \n\n如果出现下载open_jtalk的错误信息，可以再次尝试，如果实在不行，可以使用`pip install openjtalk`\n\n</details>\n\n## 💡 鸣谢\n\n+ 部分代码参考自[nonebot-plugin-petpet](https://github.com/noneplugin/nonebot-plugin-petpet)\n+ **[CjangCjengh](https://github.com/CjangCjengh/)**：g2p转换，适用于日语调形标注的符号文件及分享的[柚子社多人模型](https://github.com/CjangCjengh/TTSModels)\n+ **[luoyily](https://github.com/luoyily)**：分享的[ATRI模型](https://pan.baidu.com/s/1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4)\n\n## 📝 更新日志\n\n**2023.4.9 version 0.3.9：**\n\n支持添加生成symbols的代码，以便添加更多的symbols,详见[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E5%85%B3%E4%BA%8Esymbols)\n\nfix bug [#39](https://github.com/dpm12345/nonebot_plugin_tts_gal/issues/39)\n\n**2023.1.12 version 0.3.8：**\n\n修复regex的匹配问题\n\n**2023.1.11 version 0.3.7：**\n\n支持百度翻译和腾讯翻译的api使用，增加是否需要@机器人、自定义前缀、自定义插件priority等配置\n\n**2022.12.9 version 0.3.3：**\n\n自动读取已加载的角色模型，可通过[PicMenu插件](https://github.com/hamo-reid/nonebot_plugin_PicMenu)进行显示可使用的角色;对代码进行相关优化\n\n**2022.10.27 version 0.3.2：**\n\n修改正则表达式，避免文本出现"说/发送"而造成name的匹配错误\n\n**2022.10.21 version 0.3.1：**\n\n修复对配置项auto_delete_voice的判断bug\n\n**2022.10.19 version 0.3.0：**\n\n支持添加中文模型，优化相关代码，增添更多提示\n\n**2022.10.7 version 0.2.3:**\n\n适配nonebot2-rc1版本，并添加部分报错信息提醒\n\n**2022.9.28 version 0.2.2:**\n\n添加中文逗号替换成英文逗号\n\n**version 0.2.1:**\n\n将pyopenjtalk依赖更新为0.3.0，使python3.10也能使用\n\n**2022.9.25 version 0.2.0:**\n\n优化修改代码逻辑，支持自行添加vits模型，简单修复了一下有道翻译的翻译问题，启动时自动检测所需文件是否缺失\n\n**2022.9.21 version 0.1.1:**\n\n修改依赖\n\n',
     'author': 'dpm12345',
     'author_email': '1006975692@qq.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/dpm12345/nonebot_plugin_tts_gal',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 'nonebot_plugin_tts_gal.text'] package_data = \ {'': ['*']} install_requires =
 \ ['ffmpy>=0.3.0,<0.4.0', 'httpx>=0.23.1,<0.24.0', 'janome>=0.4.2,<0.5.0',
 'jieba>=0.42.1,<0.43.0', 'nonebot-adapter-onebot>=2.1.1,<3.0.0', 'nonebot-
 plugin-apscheduler>=0.2.0,<0.3.0', 'nonebot2>=2.0.0b4,<3.0.0',
 'numba>=0.56.2,<0.57.0', 'numpy>=1.20.0,<2.0.0', 'pyopenjtalk>=0.3.0,<0.4.0',
 'pypinyin>=0.47.0,<0.48.0', 'scipy>=1.5.2,<2.0.0', 'torch>=1.6.0,<2.0.0',
 'unidecode>=1.1.1,<2.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-tts-gal',
-'version': '0.3.8', 'description':
+'version': '0.3.9', 'description':
 'åºäºnonebot2åvitsçæ¬å°åè§è²è¯­é³åææä»¶',
 'long_description': '\n
                                 \n [nonebot]\n
 \n\n
   \n\n# nonebot-plugin-tts-gal\n\n_â¨ [Nonebot2](https://github.com/nonebot/
  nonebot2) åºäºnonebot2åvitsçæ¬å°åè§è²è¯­é³åææä»¶ â¨_\n\n
            \n \n_[license]\n\n [Python]\n [NoneBot]\n \n_[pypi]\n\n
@@ -36,21 +36,19 @@
 (å·ä½å¯æç´¢ç¸å³æç¨)\n\n\n\n## âï¸ éç½®\n\n| éç½®é¡¹ | å¿å¡« |
 ç±»å | é»è®¤å¼ | è¯´æ |\n| :-----: | :--: | :----: | :----: | :-----:
 |\n| tts_gal | æ¯ | Dict[Tuble[str],List[str]] | {():[""]} |
 çææå®è§è²è¯­é³çå³é®éç½®ï¼å·ä½å¯è§[tts_galçéç½®è¦æ±]
 (https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/
 Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82)
 |\n| auto_delete_voice | å¦ | Bool | True |
-æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦
-(éç½®æä»¶ä¸­è¯·å¡«`true`æ`false`) |\n| decibel | å¦ | int | -10 |
-åéè¯­é³ç¸å¯¹çæçåè´æ°
+æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦ |\n| decibel |
+å¦ | int | -10 | åéè¯­é³ç¸å¯¹çæçåè´æ°
 (åçæçé³é¢é³éå¯è½æ¯è¾å¤§ï¼å æ­¤éè¿æ­¤é¡¹æ¥éä½ï¼è´æ°ä¸ºéï¼æ´æ°ä½å)
-|\n| tts_gal_is_at | å¦ | Bool | True |
-ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äººï¼
-(è¥å¡«åï¼å¡«`true`æ`false`) |\n| tts_gal_prefix | å¦ | str | ""(ç©º) |
+|\n| tts_gal_is_at | å¦ | Bool | True | ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äºº
+|\n| tts_gal_prefix | å¦ | str | ""(ç©º) |
 ä½¿ç¨è¯¥æä»¶æ¶çè§¦åå¹éåç¼ï¼åå°å²çª |\n| tts_gal_priority |
 å¦ | int | 3 | è¯¥æä»¶çä¼åçº§å¤§å° |\n| tts_gal_tran_type | å¦ | List
 [str] | ["youdao"] | ææ¬ç¿»è¯ä½¿ç¨é¡¹ï¼é»è®¤ä¸ºæéç¿»è¯
 ("youdao")ï¼å¯æ¯æç¾åº¦ç¿»è¯("baidu")åè¾è®¯ç¿»è¯
 ("tencent")ï¼å¡«åé¡ºåºä¸ºç¿»è¯è°ç¨ä¼åçº§ï¼è¥å¡«åç¾åº¦åè¾è®¯ç¿»è¯åéå¡«åå¯¹åºçéç½®é¡¹
 |\n| baidu_tran_appid | å¦ | str | ""(ç©º) |
 ç¾åº¦ç¿»è¯æ¥å£å¯¹åºçappidï¼å¯å¨[ç¾åº¦ç¿»è¯æ§å¶å°](https://fanyi-
@@ -109,15 +107,19 @@
 install openjtalk`\n\n\n\n## ð¡ é¸£è°¢\n\n+ é¨åä»£ç åèèª[nonebot-
 plugin-petpet](https://github.com/noneplugin/nonebot-plugin-petpet)\n+ **
 [CjangCjengh](https://github.com/CjangCjengh/
 )**ï¼g2pè½¬æ¢ï¼éç¨äºæ¥è¯­è°å½¢æ æ³¨çç¬¦å·æä»¶ååäº«ç
 [æå­ç¤¾å¤äººæ¨¡å](https://github.com/CjangCjengh/TTSModels)\n+ **
 [luoyily](https://github.com/luoyily)**ï¼åäº«ç[ATRIæ¨¡å](https://
 pan.baidu.com/s/1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4)\n\n## ð
-æ´æ°æ¥å¿\n\n**2023.1.12 version
+æ´æ°æ¥å¿\n\n**2023.4.9 version
+0.3.9ï¼**\n\næ¯ææ·»å çæsymbolsçä»£ç ï¼ä»¥ä¾¿æ·»å æ´å¤çsymbols,è¯¦è§
+[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/
+Usage.md#%E5%85%B3%E4%BA%8Esymbols)\n\nfix bug [#39](https://github.com/
+dpm12345/nonebot_plugin_tts_gal/issues/39)\n\n**2023.1.12 version
 0.3.8ï¼**\n\nä¿®å¤regexçå¹éé®é¢\n\n**2023.1.11 version
 0.3.7ï¼**\n\næ¯æç¾åº¦ç¿»è¯åè¾è®¯ç¿»è¯çapiä½¿ç¨ï¼å¢å æ¯å¦éè¦@æºå¨äººãèªå®ä¹åç¼ãèªå®ä¹æä»¶priorityç­éç½®\n\n**2022.12.9
 version 0.3.3ï¼**\n\nèªå¨è¯»åå·²å è½½çè§è²æ¨¡åï¼å¯éè¿
 [PicMenuæä»¶](https://github.com/hamo-reid/
 nonebot_plugin_PicMenu)è¿è¡æ¾ç¤ºå¯ä½¿ç¨çè§è²;å¯¹ä»£ç è¿è¡ç¸å³ä¼å\n\n**2022.10.27
 version 0.3.2ï¼**\n\nä¿®æ¹æ­£åè¡¨è¾¾å¼ï¼é¿åææ¬åºç°"è¯´/
 åé"èé ænameçå¹ééè¯¯\n\n**2022.10.21 version
```

### Comparing `nonebot_plugin_tts_gal-0.3.8/PKG-INFO` & `nonebot_plugin_tts_gal-0.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tts-gal
-Version: 0.3.8
+Version: 0.3.9
 Summary: 基于nonebot2和vits的本地化角色语音合成插件
 Home-page: https://github.com/dpm12345/nonebot_plugin_tts_gal
 License: MIT
 Author: dpm12345
 Author-email: 1006975692@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -114,17 +114,17 @@
 </details>
 
 ## ⚙️ 配置
 
 | 配置项  | 必填 | 类型 | 默认值 |  说明  |
 | :-----: | :--: | :----: | :----: | :-----: |
 | tts_gal |  是  | Dict[Tuble[str],List[str]] | {():[""]} | 生成指定角色语音的关键配置，具体可见[tts_gal的配置要求](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82) |
-| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否<br>(配置文件中请填`true`或`false`) |
+| auto_delete_voice | 否 | Bool | True | 是否自动删除生成语音，`True`为是，`False`为否 |
 | decibel | 否 | int | -10 | 发送语音相对生成的分贝数<br>(原生成的音频音量可能比较大，因此通过此项来降低，负数为降，整数位升) |
-| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人，<br>(若填写，填`true`或`false`) |
+| tts_gal_is_at | 否 | Bool | True | 使用该功能是否需要@机器人 |
 | tts_gal_prefix | 否 | str | ""(空) | 使用该插件时的触发匹配前缀，减少冲突 |
 | tts_gal_priority | 否 | int | 3 | 该插件的优先级大小 |
 | tts_gal_tran_type | 否 | List[str] | ["youdao"] | 文本翻译使用项，默认为有道翻译("youdao")，可支持百度翻译("baidu")和腾讯翻译("tencent")，填写顺序为翻译调用优先级，若填写百度和腾讯翻译后需填写对应的配置项 |
 | baidu_tran_appid | 否 | str | ""(空) | 百度翻译接口对应的appid，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |
 | baidu_tran_apikey | 否 | str | ""(空) | 百度翻译接口对应的apikey，可在[百度翻译控制台](https://fanyi-api.baidu.com/manage/developer)获取 |
 | tencent_tran_region | 否 | str | "ap-shanghai" | 腾讯翻译接口对应的地域，可在[地域列表](https://cloud.tencent.com/document/api/551/15615#.E5.9C.B0.E5.9F.9F.E5.88.97.E8.A1.A8)获取 |
 | tencent_tran_secretid | 否 | str | ""(空) | 腾讯翻译接口对应secretid，可在[云API密钥](https://console.cloud.tencent.com/capi)获取 |
@@ -230,14 +230,20 @@
 
 + 部分代码参考自[nonebot-plugin-petpet](https://github.com/noneplugin/nonebot-plugin-petpet)
 + **[CjangCjengh](https://github.com/CjangCjengh/)**：g2p转换，适用于日语调形标注的符号文件及分享的[柚子社多人模型](https://github.com/CjangCjengh/TTSModels)
 + **[luoyily](https://github.com/luoyily)**：分享的[ATRI模型](https://pan.baidu.com/s/1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4)
 
 ## 📝 更新日志
 
+**2023.4.9 version 0.3.9：**
+
+支持添加生成symbols的代码，以便添加更多的symbols,详见[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/Usage.md#%E5%85%B3%E4%BA%8Esymbols)
+
+fix bug [#39](https://github.com/dpm12345/nonebot_plugin_tts_gal/issues/39)
+
 **2023.1.12 version 0.3.8：**
 
 修复regex的匹配问题
 
 **2023.1.11 version 0.3.7：**
 
 支持百度翻译和腾讯翻译的api使用，增加是否需要@机器人、自定义前缀、自定义插件priority等配置
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tts-gal Version: 0.3.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tts-gal Version: 0.3.9 Summary:
 åºäºnonebot2åvitsçæ¬å°åè§è²è¯­é³åææä»¶ Home-page: https://
 github.com/dpm12345/nonebot_plugin_tts_gal License: MIT Author: dpm12345
 Author-email: 1006975692@qq.com Requires-Python: >=3.8,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: ffmpy (>=0.3.0,<0.4.0) Requires-Dist: httpx (>=0.23.1,<0.24.0)
@@ -43,21 +43,19 @@
 éç½® | éç½®é¡¹ | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | | :-----: | :--: |
 :----: | :----: | :-----: | | tts_gal | æ¯ | Dict[Tuble[str],List[str]] | {():
 [""]} | çææå®è§è²è¯­é³çå³é®éç½®ï¼å·ä½å¯è§
 [tts_galçéç½®è¦æ±](https://github.com/dpm12345/nonebot_plugin_tts_gal/
 blob/master/
 Usage.md#%E6%9C%BA%E5%99%A8%E4%BA%BA%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6%E8%A6%81%E6%B1%82)
 | | auto_delete_voice | å¦ | Bool | True |
-æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦
-(éç½®æä»¶ä¸­è¯·å¡«`true`æ`false`) | | decibel | å¦ | int | -10 |
-åéè¯­é³ç¸å¯¹çæçåè´æ°
+æ¯å¦èªå¨å é¤çæè¯­é³ï¼`True`ä¸ºæ¯ï¼`False`ä¸ºå¦ | | decibel | å¦
+| int | -10 | åéè¯­é³ç¸å¯¹çæçåè´æ°
 (åçæçé³é¢é³éå¯è½æ¯è¾å¤§ï¼å æ­¤éè¿æ­¤é¡¹æ¥éä½ï¼è´æ°ä¸ºéï¼æ´æ°ä½å)
-| | tts_gal_is_at | å¦ | Bool | True |
-ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äººï¼
-(è¥å¡«åï¼å¡«`true`æ`false`) | | tts_gal_prefix | å¦ | str | ""(ç©º) |
+| | tts_gal_is_at | å¦ | Bool | True | ä½¿ç¨è¯¥åè½æ¯å¦éè¦@æºå¨äºº |
+| tts_gal_prefix | å¦ | str | ""(ç©º) |
 ä½¿ç¨è¯¥æä»¶æ¶çè§¦åå¹éåç¼ï¼åå°å²çª | | tts_gal_priority |
 å¦ | int | 3 | è¯¥æä»¶çä¼åçº§å¤§å° | | tts_gal_tran_type | å¦ | List
 [str] | ["youdao"] | ææ¬ç¿»è¯ä½¿ç¨é¡¹ï¼é»è®¤ä¸ºæéç¿»è¯
 ("youdao")ï¼å¯æ¯æç¾åº¦ç¿»è¯("baidu")åè¾è®¯ç¿»è¯
 ("tencent")ï¼å¡«åé¡ºåºä¸ºç¿»è¯è°ç¨ä¼åçº§ï¼è¥å¡«åç¾åº¦åè¾è®¯ç¿»è¯åéå¡«åå¯¹åºçéç½®é¡¹
 | | baidu_tran_appid | å¦ | str | ""(ç©º) |
 ç¾åº¦ç¿»è¯æ¥å£å¯¹åºçappidï¼å¯å¨[ç¾åº¦ç¿»è¯æ§å¶å°](https://fanyi-
@@ -117,16 +115,21 @@
 å¦æåºç°ä¸è½½open_jtalkçéè¯¯ä¿¡æ¯ï¼å¯ä»¥åæ¬¡å°è¯ï¼å¦æå®å¨ä¸è¡ï¼å¯ä»¥ä½¿ç¨`pip
 install openjtalk`  ## ð¡ é¸£è°¢ + é¨åä»£ç åèèª[nonebot-plugin-
 petpet](https://github.com/noneplugin/nonebot-plugin-petpet) + **[CjangCjengh]
 (https://github.com/CjangCjengh/
 )**ï¼g2pè½¬æ¢ï¼éç¨äºæ¥è¯­è°å½¢æ æ³¨çç¬¦å·æä»¶ååäº«ç
 [æå­ç¤¾å¤äººæ¨¡å](https://github.com/CjangCjengh/TTSModels) + **[luoyily]
 (https://github.com/luoyily)**ï¼åäº«ç[ATRIæ¨¡å](https://pan.baidu.com/s/
-1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4) ## ð æ´æ°æ¥å¿ **2023.1.12 version
-0.3.8ï¼** ä¿®å¤regexçå¹éé®é¢ **2023.1.11 version 0.3.7ï¼**
+1_vhOx50OE5R4bE02ZMe9GA?pwd=9jo4) ## ð æ´æ°æ¥å¿ **2023.4.9 version
+0.3.9ï¼**
+æ¯ææ·»å çæsymbolsçä»£ç ï¼ä»¥ä¾¿æ·»å æ´å¤çsymbols,è¯¦è§
+[Usage.md](https://github.com/dpm12345/nonebot_plugin_tts_gal/blob/master/
+Usage.md#%E5%85%B3%E4%BA%8Esymbols) fix bug [#39](https://github.com/dpm12345/
+nonebot_plugin_tts_gal/issues/39) **2023.1.12 version 0.3.8ï¼**
+ä¿®å¤regexçå¹éé®é¢ **2023.1.11 version 0.3.7ï¼**
 æ¯æç¾åº¦ç¿»è¯åè¾è®¯ç¿»è¯çapiä½¿ç¨ï¼å¢å æ¯å¦éè¦@æºå¨äººãèªå®ä¹åç¼ãèªå®ä¹æä»¶priorityç­éç½®
 **2022.12.9 version 0.3.3ï¼** èªå¨è¯»åå·²å è½½çè§è²æ¨¡åï¼å¯éè¿
 [PicMenuæä»¶](https://github.com/hamo-reid/
 nonebot_plugin_PicMenu)è¿è¡æ¾ç¤ºå¯ä½¿ç¨çè§è²;å¯¹ä»£ç è¿è¡ç¸å³ä¼å
 **2022.10.27 version 0.3.2ï¼** ä¿®æ¹æ­£åè¡¨è¾¾å¼ï¼é¿åææ¬åºç°"è¯´/
 åé"èé ænameçå¹ééè¯¯ **2022.10.21 version 0.3.1ï¼**
 ä¿®å¤å¯¹éç½®é¡¹auto_delete_voiceçå¤æ­bug **2022.10.19 version 0.3.0ï¼**
```

