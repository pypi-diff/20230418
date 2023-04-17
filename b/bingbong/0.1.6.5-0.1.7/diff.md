# Comparing `tmp/bingbong-0.1.6.5-py3-none-any.whl.zip` & `tmp/bingbong-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11055 bytes, number of entries: 15
--rw-rw-rw-  2.0 unx       55 b- defN 23-Apr-17 13:08 pingpong/__init__.py
--rw-rw-rw-  2.0 unx     1446 b- defN 23-Apr-17 12:46 pingpong/alpaca.py
--rw-rw-rw-  2.0 unx     1215 b- defN 23-Apr-14 12:55 pingpong/dolly.py
+Zip file size: 11082 bytes, number of entries: 15
+-rw-rw-rw-  2.0 unx       53 b- defN 23-Apr-17 23:09 pingpong/__init__.py
+-rw-rw-rw-  2.0 unx     1547 b- defN 23-Apr-17 23:05 pingpong/alpaca.py
+-rw-rw-rw-  2.0 unx     1287 b- defN 23-Apr-17 22:59 pingpong/dolly.py
 -rw-rw-rw-  2.0 unx      987 b- defN 23-Apr-14 05:26 pingpong/gradio.py
--rw-rw-rw-  2.0 unx     1192 b- defN 23-Apr-14 12:50 pingpong/pingpong.py
+-rw-rw-rw-  2.0 unx     1212 b- defN 23-Apr-17 22:55 pingpong/pingpong.py
 -rw-rw-rw-  2.0 unx      173 b- defN 23-Apr-12 04:36 pingpong/context/__init__.py
 -rw-rw-rw-  2.0 unx      589 b- defN 23-Apr-12 00:59 pingpong/context/auto_summary_strategy.py
--rw-rw-rw-  2.0 unx      773 b- defN 23-Apr-17 13:08 pingpong/context/last_window_strategy.py
+-rw-rw-rw-  2.0 unx      789 b- defN 23-Apr-17 22:54 pingpong/context/last_window_strategy.py
 -rw-rw-rw-  2.0 unx      840 b- defN 23-Apr-12 04:54 pingpong/context/search_window_strategy.py
 -rw-rw-rw-  2.0 unx      119 b- defN 23-Apr-11 14:54 pingpong/context/strategy.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 13:09 bingbong-0.1.6.5.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     3348 b- defN 23-Apr-17 13:09 bingbong-0.1.6.5.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 13:09 bingbong-0.1.6.5.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 13:09 bingbong-0.1.6.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-17 13:09 bingbong-0.1.6.5.dist-info/RECORD
-15 files, 23430 bytes uncompressed, 9001 bytes compressed:  61.6%
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 unx     3346 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        9 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1225 b- defN 23-Apr-17 23:10 bingbong-0.1.7.dist-info/RECORD
+15 files, 23625 bytes uncompressed, 9048 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.6.5.dist-info/LICENSE
+Filename: bingbong-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.6.5.dist-info/METADATA
+Filename: bingbong-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.6.5.dist-info/WHEEL
+Filename: bingbong-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.6.5.dist-info/top_level.txt
+Filename: bingbong-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.6.5.dist-info/RECORD
+Filename: bingbong-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.6.5'
+__version__ = '0.1.7'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -9,18 +9,20 @@
     else:
       return f"""### Input:
 {context}
 
 """
 
   @classmethod
-  def prompt(cls, pingpong):
-    return f"""### Instruction: {pingpong.ping}
+  def prompt(cls, pingpong, truncate_size):
+    return f"""### Instruction:
+{pingpong.ping[:truncate_size]}
 
-### Response: {"" if pingpong.pong is None else pingpong.pong}"""
+### Response:
+{"" if pingpong.pong is None else pingpong.pong[:truncate_size]}"""
 
 class AlpacaChatPPManager(PPManager):
   def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
     allowed = super().add_ping(ping, fmt)
 
     if allowed:
       if self.ctx == "":
@@ -36,22 +38,22 @@
 ### Response:
 """
       return prompts
 
     return None
 
 
-  def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt):
+  def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt, truncate_size: int=None):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
       to_idx = len(self.pingpongs)
 
     results = ""
 
     for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
-      results += fmt.prompt(pingpong)
+      results += fmt.prompt(pingpong, truncate_size=truncate_size)
 
       if from_idx+idx != to_idx-1:
         results += """
 
 """
 
     return results
```

## pingpong/dolly.py

```diff
@@ -9,20 +9,20 @@
     else:
       return f"""
 ### Input:
 {context}
 """
 
   @classmethod
-  def prompt(cls, pingpong):
+  def prompt(cls, pingpong, truncate_size):
     return f"""### Instruction:
-{pingpong.ping}
+{pingpong.ping[:truncate_size]}
 
 ### Response:
-{"" if pingpong.pong is None else pingpong.pong}"""
+{"" if pingpong.pong is None else pingpong.pong[:truncate_size]}"""
 
 class DollyChatPPManager(PPManager):
   def add_ping(self, ping, fmt: PromptFmt=DollyPromptFmt):
     allowed = super().add_ping(ping, fmt)
 
     if allowed:
       prompts = f"""Below is an instruction that describes a task. Write a response that appropriately completes the request.
@@ -31,15 +31,15 @@
 {ping}
 {fmt.ctx(self.ctx)}
 """
       return prompts
 
     return None
 
-  def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=DollyPromptFmt):
+  def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=DollyPromptFmt, truncate_size: int=None):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
       to_idx = len(self.pingpongs)
 
     results = fmt.ctx(self.ctx)
 
     for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
       print(idx)
```

## pingpong/pingpong.py

```diff
@@ -43,13 +43,13 @@
 
   def add_pingpong(self, pingpong):
     self.pingpongs.append(pingpong)
 
   def pop_pingpong(self):
     return self.pingpongs.pop()
 
-  def build_prompts(self, from_idx: int, to_idx: int, fmt: PromptFmt):
+  def build_prompts(self, from_idx: int, to_idx: int, fmt: PromptFmt, truncate_size: int):
     pass
 
   def build_uis(self, from_idx: int, to_idx: int, fmt: UIFmt):
     pass
```

## pingpong/context/last_window_strategy.py

```diff
@@ -1,23 +1,22 @@
 from pingpong.pingpong import PPManager
 from pingpong.context.strategy import CtxStrategy
 
 class CtxLastWindowStrategy(CtxStrategy):
     def __init__(self, max_pingpongs: int):
         self.max_pingpongs = max_pingpongs
     
-    def __call__(self, ppmanager: PPManager, build_uis=False, remove_last=False):
+    def __call__(self, ppmanager: PPManager, build_uis=False, truncate_size=None):
         pps = ppmanager.pingpongs
 
         if len(pps) <= self.max_pingpongs:
             start_idx = 0
         else:
             start_idx = len(pps) - self.max_pingpongs
-            if remove_last: start_idx += 1
 
         if build_uis:
             return (
-                ppmanager.build_prompts(from_idx=start_idx),
+                ppmanager.build_prompts(from_idx=start_idx, truncate_size=truncate_size),
                 ppmanager.build_uis(from_idx=start_idx)
             )
         else:
-            return ppmanager.build_prompts(from_idx=start_idx)
+            return ppmanager.build_prompts(from_idx=start_idx, truncate_size=truncate_size)
```

## Comparing `bingbong-0.1.6.5.dist-info/LICENSE` & `bingbong-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.6.5.dist-info/METADATA` & `bingbong-0.1.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.6.5
+Version: 0.1.7
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.6.5.dist-info/RECORD` & `bingbong-0.1.7.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pingpong/__init__.py,sha256=8pL5QUrViBgfsTAwdhJAqaXS702U3y0zg_pcqKPlY6w,55
-pingpong/alpaca.py,sha256=WIo2FX8PAUDmLdq2FeN4_8fuuxmEnWStRpmNG1dTxUM,1446
-pingpong/dolly.py,sha256=jAWnieNLTPFzGNBI5hBaSIhx7XW0c7xGyO1PVGaBy9g,1215
+pingpong/__init__.py,sha256=bqXv93dQwN97gVcKA93Gg5dZ4nWBtg7yx8nTyRCQXrg,53
+pingpong/alpaca.py,sha256=ahlbjhzrosNq6nIbDi2VAR4cC2s-GL1S2ItziNnPc1A,1547
+pingpong/dolly.py,sha256=vMbHiwgeewzRAsruuMVnQc2w3KEKhWJUdOmaBbyazQo,1287
 pingpong/gradio.py,sha256=IchvS_gOuPk3TCATVKDWMaLEaIRqjPpi3MFnYwa0JwU,987
-pingpong/pingpong.py,sha256=yQcXkdWc9aWem0vdbqtwMMvJXsqmLnwlSuGBkM4ZHk8,1192
+pingpong/pingpong.py,sha256=XfCYe-OdNkyrKOhAEaL4Q-HhZx829_i-ohDlY2GF7gM,1212
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
-pingpong/context/last_window_strategy.py,sha256=7Hy1YJLCNumoRERzbOD8MABi7K6yXSxMRHx_cbGwjT4,773
+pingpong/context/last_window_strategy.py,sha256=JN7pFDD2C8nGMUx-H3aHNQrXCT0E0S-FlBunOrQGX-w,789
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.6.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.6.5.dist-info/METADATA,sha256=D2FboboYu0hA_yiIEszw9TGlh071HJ4u3uAY8MnJtNo,3348
-bingbong-0.1.6.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.6.5.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.6.5.dist-info/RECORD,,
+bingbong-0.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.7.dist-info/METADATA,sha256=rBg_oUA3-x1uuHkOznDbB7_Zbix4F16HKrnPWMqNK00,3346
+bingbong-0.1.7.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+bingbong-0.1.7.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.7.dist-info/RECORD,,
```

