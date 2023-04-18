# Comparing `tmp/stable-ts-2.4.0.tar.gz` & `tmp/stable-ts-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.4.0.tar", last modified: Sun Apr 16 00:44:47 2023, max compression
+gzip compressed data, was "stable-ts-2.4.1.tar", last modified: Tue Apr 18 21:35:58 2023, max compression
```

## Comparing `stable-ts-2.4.0.tar` & `stable-ts-2.4.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.079108 stable-ts-2.4.0/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.4.0/LICENSE
--rw-rw-rw-   0        0        0     6890 2023-04-16 00:44:47.078110 stable-ts-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.4.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-16 00:44:47.079108 stable-ts-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.026117 stable-ts-2.4.0/stable_ts.egg-info/
--rw-rw-rw-   0        0        0     6890 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      567 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-16 00:44:46.000000 stable-ts-2.4.0/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-16 00:44:47.076108 stable-ts-2.4.0/stable_whisper/
--rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.4.0/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.4.0/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-04-16 00:28:38.000000 stable-ts-2.4.0/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     6525 2023-04-16 00:09:42.000000 stable-ts-2.4.0/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.4.0/stable_whisper/decode.py
--rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.4.0/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    28381 2023-04-15 17:10:33.000000 stable-ts-2.4.0/stable_whisper/result.py
--rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.4.0/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    12598 2023-04-05 01:42:52.000000 stable-ts-2.4.0/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.4.0/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.4.0/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    48728 2023-04-16 00:31:11.000000 stable-ts-2.4.0/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.178899 stable-ts-2.4.1/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.4.1/LICENSE
+-rw-rw-rw-   0        0        0     6890 2023-04-18 21:35:58.177899 stable-ts-2.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6594 2023-04-04 01:04:16.000000 stable-ts-2.4.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 21:35:58.179901 stable-ts-2.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.126898 stable-ts-2.4.1/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0     6890 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 21:35:57.000000 stable-ts-2.4.1/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 21:35:58.175899 stable-ts-2.4.1/stable_whisper/
+-rw-rw-rw-   0        0        0      200 2023-03-17 04:40:26.000000 stable-ts-2.4.1/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.4.1/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-04-18 21:09:40.000000 stable-ts-2.4.1/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     6525 2023-04-16 00:09:42.000000 stable-ts-2.4.1/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4328 2023-03-22 02:57:30.000000 stable-ts-2.4.1/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0     1645 2023-03-10 21:20:52.000000 stable-ts-2.4.1/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    28584 2023-04-18 21:10:38.000000 stable-ts-2.4.1/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    13168 2023-04-04 00:54:46.000000 stable-ts-2.4.1/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    14331 2023-04-18 21:08:14.000000 stable-ts-2.4.1/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0     9744 2023-04-08 16:34:45.000000 stable-ts-2.4.1/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.4.1/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    48816 2023-04-18 21:05:11.000000 stable-ts-2.4.1/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.4.0/LICENSE` & `stable-ts-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/PKG-INFO` & `stable-ts-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.4.0
+Version: 2.4.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.4.0/README.md` & `stable-ts-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/setup.py` & `stable-ts-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.4.1/stable_ts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.4.0
+Version: 2.4.1
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `stable-ts-2.4.0/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.4.1/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/audio.py` & `stable-ts-2.4.1/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/decode.py` & `stable-ts-2.4.1/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/quantization.py` & `stable-ts-2.4.1/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/result.py` & `stable-ts-2.4.1/stable_whisper/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,24 +185,24 @@
                     if segment.words[i-1].duration < segment.words[i-1].duration:
                         segment.add_words(i-1, i, inplace=True)
                     else:
                         segment.add_words(i, i+1, inplace=True)
                 max_i -= 1
         return segment
 
-    def _to_rtl(
+    def _to_reverse_text(
             self,
             prepend_punctuations: str = None,
             append_punctuations: str = None
     ):
         """
 
         Returns
         -------
-        A copy in RTL format
+        A copy with words reversed order per segment
 
         """
         if prepend_punctuations is None:
             prepend_punctuations = "\"'“¿([{-"
         if prepend_punctuations and ' ' not in prepend_punctuations:
             prepend_punctuations += ' '
         if append_punctuations is None:
@@ -236,30 +236,34 @@
                         else:
                             break
                 word.word = f'{new_prepend}{word.word}{new_append[::-1]}'
             self_copy.text = ''.join(w.word for w in reversed(word_objs))
 
         return self_copy
 
-    def to_dict(self, rtl: Union[bool, tuple] = False):
-        if rtl:
-            seg_dict = (self._to_rtl(*rtl) if isinstance(rtl, tuple) else self._to_rtl()).__dict__
+    def to_dict(self, reverse_text: Union[bool, tuple] = False):
+        if reverse_text:
+            seg_dict = (
+                (self._to_reverse_text(*reverse_text)
+                 if isinstance(reverse_text, tuple) else
+                 self._to_reverse_text()).__dict__
+            )
         else:
             seg_dict = deepcopy(self.__dict__)
         seg_dict.pop('ori_has_words')
         if self.has_words:
             seg_dict['words'] = [w.to_dict() for w in seg_dict['words']]
         elif self.ori_has_words:
             seg_dict['words'] = []
         else:
             seg_dict.pop('words')
         if self.id is None:
             seg_dict.pop('id')
-        if rtl:
-            seg_dict['rtl'] = True
+        if reverse_text:
+            seg_dict['reversed_text'] = True
         return seg_dict
 
     @property
     def left_locked(self):
         if self.has_words:
             return self.words[0].left_locked
         return False
@@ -541,16 +545,16 @@
 
     def to_dict(self):
         return dict(text=self.text,
                     segments=self.segments_to_dicts(),
                     language=self.language,
                     ori_dict=self.ori_dict)
 
-    def segments_to_dicts(self, rtl: Union[bool, tuple] = False):
-        return [s.to_dict(rtl=rtl) for s in self.segments]
+    def segments_to_dicts(self, reverse_text: Union[bool, tuple] = False):
+        return [s.to_dict(reverse_text=reverse_text) for s in self.segments]
 
     def _split_segments(self, get_indices, args: list = None, *, lock: bool = False):
         if args is None:
             args = []
         no_words = False
         for i in reversed(range(0, len(self.segments))):
             no_words = not self.segments[i].has_words
```

### Comparing `stable-ts-2.4.0/stable_whisper/stabilization.py` & `stable-ts-2.4.1/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/text_output.py` & `stable-ts-2.4.1/stable_whisper/text_output.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import json
 import os
 import warnings
-from typing import List, Tuple, Union
+from typing import List, Tuple, Union, Callable
 from itertools import chain
 from .stabilization import valid_ts
 
 __all__ = ['result_to_srt_vtt', 'result_to_ass', 'save_as_json', 'load_result']
 
 
 def _save_as_file(content: str, path: str):
     with open(path, 'w', encoding='utf-8') as f:
         f.write(content)
     print(f'Saved: {os.path.abspath(path)}')
 
 
-def _get_segments(result: (dict, list), min_dur: float, rtl: Union[bool, tuple] = False):
+def _get_segments(result: (dict, list), min_dur: float, reverse_text: Union[bool, tuple] = False):
     if isinstance(result, dict):
-        if rtl:
-            warnings.warn(f'[rtl]=True only applies to WhisperResult but result is {type(result)}')
+        if reverse_text:
+            warnings.warn(f'[reverse_text]=True only applies to WhisperResult but result is {type(result)}')
         return result.get('segments')
     elif not isinstance(result, list) and callable(getattr(result, 'segments_to_dicts', None)):
-        return result.apply_min_dur(min_dur, inplace=False).segments_to_dicts(rtl=rtl)
+        return result.apply_min_dur(min_dur, inplace=False).segments_to_dicts(reverse_text=reverse_text)
     return result
 
 
 def sec2hhmmss(seconds: (float, int)):
     mm, ss = divmod(seconds, 60)
     hh, mm = divmod(mm, 60)
     return hh, mm, ss
@@ -55,15 +55,15 @@
 
 
 def segment2assblock(segment: dict, idx: int, strip=True) -> str:
     return f'Dialogue: {idx},{sec2ass(segment["start"])},{sec2ass(segment["end"])},Default,,0,0,0,,' \
            f'{segment["text"].strip() if strip else segment["text"]}'
 
 
-def words2segments(words: List[dict], tag: Tuple[str, str], rtl: bool = False) -> List[dict]:
+def words2segments(words: List[dict], tag: Tuple[str, str], reverse_text: bool = False) -> List[dict]:
     def add_tag(idx: int):
         return ''.join(
             (
                 f" {tag[0]}{w['word'][1:]}{tag[1]}"
                 if w['word'].startswith(' ') else
                 f"{tag[0]}{w['word']}{tag[1]}"
             )
@@ -77,24 +77,29 @@
         curr_end = round(word['end'], 3)
         filled_words.append(dict(word=word['word'], start=round(word['start'], 3), end=curr_end))
         if word != words[-1]:
             next_start = round(words[i + 1]['start'], 3)
             if next_start - curr_end != 0:
                 filled_words.append(dict(word='', start=curr_end, end=next_start))
     idx_filled_words = list(enumerate(filled_words))
-    if rtl:
+    if reverse_text:
         idx_filled_words = list(reversed(idx_filled_words))
 
     segments = [dict(text=add_tag(i), start=filled_words[i]['start'], end=filled_words[i]['end'])
                 for i in range(len(filled_words))]
     return segments
 
 
 def to_word_level_segments(segments: List[dict], tag: Tuple[str, str]) -> List[dict]:
-    return list(chain.from_iterable(words2segments(s['words'], tag, rtl=s.get('rtl')) for s in segments))
+    return list(
+        chain.from_iterable(
+            words2segments(s['words'], tag, reverse_text=s.get('reversed_text'))
+            for s in segments
+        )
+    )
 
 
 def to_word_level(segments: List[dict]) -> List[dict]:
     return [dict(text=w['word'], start=w['start'], end=w['end']) for s in segments for w in s['words']]
 
 
 def _confirm_word_level(segments: List[dict]) -> bool:
@@ -105,31 +110,86 @@
     return True
 
 
 def _preprocess_args(result: (dict, list),
                      segment_level: bool,
                      word_level: bool,
                      min_dur: float,
-                     rtl: Union[bool, tuple] = False):
+                     reverse_text: Union[bool, tuple] = False):
     assert segment_level or word_level, '`segment_level` or `word_level` must be True'
-    segments = _get_segments(result, min_dur, rtl=rtl)
+    segments = _get_segments(result, min_dur, reverse_text=reverse_text)
     if word_level:
         word_level = _confirm_word_level(segments)
     return segments, segment_level, word_level
 
 
+def result_to_any(result: (dict, list),
+                  filepath: str = None,
+                  filetype: str = None,
+                  segments2blocks: Callable = None,
+                  segment_level=True,
+                  word_level=True,
+                  min_dur: float = 0.02,
+                  tag: Tuple[str, str] = None,
+                  default_tag: Tuple[str, str] = None,
+                  strip=True,
+                  reverse_text: Union[bool, tuple] = False):
+    """
+
+    Generate file from result to display segment-level and/or word-level timestamp.
+
+    Returns
+    -------
+    string of content if no [filepath] is provided, else None
+
+    """
+    segments, segment_level, word_level = _preprocess_args(
+        result, segment_level, word_level, min_dur, reverse_text=reverse_text
+    )
+
+    if filetype is None:
+        filetype = os.path.splitext(filepath)[-1][1:] or 'srt'
+    if filetype.lower() not in ('srt', 'vtt', 'ass', 'tsv'):
+        raise NotImplementedError(f'{filetype} not supported')
+
+    if filepath and not filepath.lower().endswith(f'.{filetype}'):
+        filepath += f'.{filetype}'
+
+    if word_level and segment_level:
+        if tag is None:
+            if default_tag is None:
+                tag = ('<font color="#00ff00">', '</font>') if filetype == 'srt' else ('<u>', '</u>')
+            else:
+                tag = default_tag
+        segments = to_word_level_segments(segments, tag)
+    elif word_level:
+        segments = to_word_level(segments)
+
+    valid_ts(segments)
+
+    if segments2blocks is None:
+        sub_str = '\n\n'.join(segment2srtblock(s, i, strip=strip) for i, s in enumerate(segments))
+    else:
+        sub_str = segments2blocks(segments)
+
+    if filepath:
+        _save_as_file(sub_str, filepath)
+    else:
+        return sub_str
+
+
 def result_to_srt_vtt(result: (dict, list),
                       filepath: str = None,
                       segment_level=True,
                       word_level=True,
                       min_dur: float = 0.02,
                       tag: Tuple[str, str] = None,
                       vtt: bool = None,
                       strip=True,
-                      rtl: Union[bool, tuple] = False):
+                      reverse_text: Union[bool, tuple] = False):
     """
 
     Generate SRT/VTT from result to display segment-level and/or word-level timestamp.
 
     Parameters
     ----------
     result: (dict, list)
@@ -147,68 +207,56 @@
         tag used to change the properties a word at its timestamp
         SRT Default: '<font color="#00ff00">', '</font>'
         VTT Default: '<u>', '</u>'
     vtt: bool
         whether to output VTT (default: False if no [filepath] is specified, else determined by [filepath] extension)
     strip: bool
         whether to remove spaces before and after text on each segment for output (default: True)
-    rtl: Union[bool, tuple]
-        whether to reverse Left-To-Right text into Right-To-Left format (default: False)
+    reverse_text: Union[bool, tuple]
+        whether to reverse the order of words for each segment (default: False)
         or provide the [prepend_punctuations] and [append_punctuations] as tuple pair instead of True
         to match transcription settings (if True, the default punctuations will be used)
         Note: This will not fix RTL text not displaying tags properly which is an issue with video player.
                 VLC seems to not suffer from this issue.
 
     Returns
     -------
     string of content if no [filepath] is provided, else None
 
     """
-    segments, segment_level, word_level = _preprocess_args(result, segment_level, word_level, min_dur, rtl=rtl)
-
-    is_srt = (filepath is None or not filepath.endswith('.vtt')) if vtt is None else vtt
-    if filepath:
-        if is_srt:
-            if not filepath.endswith('.srt'):
-                filepath += '.srt'
-        elif not filepath.endswith('.vtt'):
-            filepath += '.vtt'
-
-    sub_str = '' if is_srt else 'WEBVTT\n\n'
-
-    if word_level and segment_level:
-        if tag is None:
-            tag = ('<font color="#00ff00">', '</font>') if is_srt else ('<u>', '</u>')
-        segments = to_word_level_segments(segments, tag)
-    elif word_level:
-        segments = to_word_level(segments)
-
-    valid_ts(segments)
-
+    is_srt = (filepath is None or not filepath.lower().endswith('.vtt')) if vtt is None else not vtt
     if is_srt:
-        sub_str += '\n\n'.join(segment2srtblock(s, i, strip=strip) for i, s in enumerate(segments))
-    else:
-        sub_str += '\n\n'.join(segment2vttblock(s, strip=strip) for i, s in enumerate(segments))
-
-    if filepath:
-        _save_as_file(sub_str, filepath)
+        segments2blocks = None
     else:
-        return sub_str
+        def segments2blocks(segments):
+            return 'WEBVTT\n\n' + '\n\n'.join(segment2vttblock(s, strip=strip) for i, s in enumerate(segments))
+    return result_to_any(
+        result=result,
+        filepath=filepath,
+        filetype=('vtt', 'srt')[is_srt],
+        segments2blocks=segments2blocks,
+        segment_level=segment_level,
+        word_level=word_level,
+        min_dur=min_dur,
+        tag=tag,
+        strip=strip,
+        reverse_text=reverse_text
+    )
 
 
 def result_to_ass(result: (dict, list),
                   filepath: str = None,
                   segment_level=True,
                   word_level=True,
                   min_dur: float = 0.02,
                   tag: Tuple[str, str] = None,
                   font: str = None,
                   font_size: int = 24,
                   strip=True,
-                  rtl: Union[bool, tuple] = False,
+                  reverse_text: Union[bool, tuple] = False,
                   **kwargs):
     """
 
     Generate Advanced SubStation Alpha (ASS) file from result to display segment-level and/or word-level timestamp.
 
     Note: ass file is used in the same way as srt, vtt, etc.
 
@@ -229,75 +277,75 @@
         tag used to change the properties a word at its timestamp (default: '{\\1c&HFF00&}', '{\\r}')
     font: str
         word font (default: Arial)
     font_size: int
         word font size (default: 48)
     strip: bool
         whether to remove spaces before and after text on each segment for output (default: True)
-    rtl: Union[bool, tuple]
-        whether to use Right-To-Left format (default: False)
+    reverse_text: Union[bool, tuple]
+        whether to reverse the order of words for each segment (default: False)
         or provide the [prepend_punctuations] and [append_punctuations] as tuple pair instead of True
         to match transcription settings (if True, the default punctuations will be used)
+        Note: This will not fix RTL text not displaying tags properly which is an issue with video player.
+                VLC seems to not suffer from this issue.
     kwargs:
         used for format styles:
         'Name', 'Fontname', 'Fontsize', 'PrimaryColour', 'SecondaryColour', 'OutlineColour', 'BackColour', 'Bold',
         'Italic', 'Underline', 'StrikeOut', 'ScaleX', 'ScaleY', 'Spacing', 'Angle', 'BorderStyle', 'Outline',
         'Shadow', 'Alignment', 'MarginL', 'MarginR', 'MarginV', 'Encoding'
 
     Returns
     -------
     string of content if no [filepath] is provided, else None
 
     """
-    segments, segment_level, word_level = _preprocess_args(result, segment_level, word_level, min_dur, rtl=rtl)
-
-    fmt_style_dict = {'Name': 'Default', 'Fontname': 'Arial', 'Fontsize': '48', 'PrimaryColour': '&Hffffff',
-                      'SecondaryColour': '&Hffffff', 'OutlineColour': '&H0', 'BackColour': '&H0', 'Bold': '0',
-                      'Italic': '0', 'Underline': '0', 'StrikeOut': '0', 'ScaleX': '100', 'ScaleY': '100',
-                      'Spacing': '0', 'Angle': '0', 'BorderStyle': '1', 'Outline': '1', 'Shadow': '0',
-                      'Alignment': '2', 'MarginL': '10', 'MarginR': '10', 'MarginV': '10', 'Encoding': '0'}
 
-    for k, v in filter(lambda x: 'colour' in x[0].lower() and not str(x[1]).startswith('&H'), kwargs.items()):
-        kwargs[k] = f'&H{kwargs[k]}'
+    def segments2blocks(segments):
+        fmt_style_dict = {'Name': 'Default', 'Fontname': 'Arial', 'Fontsize': '48', 'PrimaryColour': '&Hffffff',
+                          'SecondaryColour': '&Hffffff', 'OutlineColour': '&H0', 'BackColour': '&H0', 'Bold': '0',
+                          'Italic': '0', 'Underline': '0', 'StrikeOut': '0', 'ScaleX': '100', 'ScaleY': '100',
+                          'Spacing': '0', 'Angle': '0', 'BorderStyle': '1', 'Outline': '1', 'Shadow': '0',
+                          'Alignment': '2', 'MarginL': '10', 'MarginR': '10', 'MarginV': '10', 'Encoding': '0'}
 
-    fmt_style_dict.update((k, v) for k, v in kwargs.items() if k in fmt_style_dict)
+        for k, v in filter(lambda x: 'colour' in x[0].lower() and not str(x[1]).startswith('&H'), kwargs.items()):
+            kwargs[k] = f'&H{kwargs[k]}'
 
-    if font:
-        fmt_style_dict.update(Fontname=font)
-    if font_size:
-        fmt_style_dict.update(Fontsize=font_size)
+        fmt_style_dict.update((k, v) for k, v in kwargs.items() if k in fmt_style_dict)
 
-    fmts = f'Format: {", ".join(map(str, fmt_style_dict.keys()))}'
+        if font:
+            fmt_style_dict.update(Fontname=font)
+        if font_size:
+            fmt_style_dict.update(Fontsize=font_size)
 
-    styles = f'Style: {",".join(map(str, fmt_style_dict.values()))}'
-
-    sub_str = f'[Script Info]\nScriptType: v4.00+\nPlayResX: 384\nPlayResY: 288\nScaledBorderAndShadow: yes\n\n' \
-              f'[V4+ Styles]\n{fmts}\n{styles}\n\n' \
-              f'[Events]\nFormat: Layer, Start, End, Style, Name, MarginL, MarginR, MarginV, Effect, Text\n\n'
-
-    if word_level and segment_level:
-        if tag is None:
-            color = 'HFF00'
-            tag = (r'{\1c&' + f'{color.upper()}&' + '}', r'{\r}')
-        segments = to_word_level_segments(segments, tag)
-    elif word_level:
-        segments = to_word_level(segments)
+        fmts = f'Format: {", ".join(map(str, fmt_style_dict.keys()))}'
 
-    valid_ts(segments)
+        styles = f'Style: {",".join(map(str, fmt_style_dict.values()))}'
 
-    sub_str += '\n'.join(segment2assblock(s, i, strip=strip) for i, s in enumerate(segments))
+        sub_str = f'[Script Info]\nScriptType: v4.00+\nPlayResX: 384\nPlayResY: 288\nScaledBorderAndShadow: yes\n\n' \
+                  f'[V4+ Styles]\n{fmts}\n{styles}\n\n' \
+                  f'[Events]\nFormat: Layer, Start, End, Style, Name, MarginL, MarginR, MarginV, Effect, Text\n\n'
 
-    if filepath:
-        if not filepath.lower().endswith('.ass'):
-            filepath += '.ass'
+        sub_str += '\n'.join(segment2assblock(s, i, strip=strip) for i, s in enumerate(segments))
 
-        _save_as_file(sub_str, filepath)
-    else:
         return sub_str
 
+    return result_to_any(
+        result=result,
+        filepath=filepath,
+        filetype='ass',
+        segments2blocks=segments2blocks,
+        segment_level=segment_level,
+        word_level=word_level,
+        min_dur=min_dur,
+        tag=tag,
+        default_tag=(r'{\1c&' + 'HFF00&' + '}', r'{\r}'),
+        strip=strip,
+        reverse_text=reverse_text
+    )
+
 
 def save_as_json(result: dict, path: str):
     """
     Save result as json.
     """
     if not isinstance(result, dict) and callable(getattr(result, 'to_dict')):
         result = result.to_dict()
```

### Comparing `stable-ts-2.4.0/stable_whisper/timing.py` & `stable-ts-2.4.1/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/video_output.py` & `stable-ts-2.4.1/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.4.0/stable_whisper/whisper_word_level.py` & `stable-ts-2.4.1/stable_whisper/whisper_word_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -758,16 +758,16 @@
                              "VTT Default: '<u>', '</u>'"
                              "ASS Default: '{\\1c&HFF00&}', '{\\r}'")
     parser.add_argument('--segment_level', type=str2bool, default=True,
                         help="whether to use segment-level timestamps in output")
     parser.add_argument('--word_level', type=str2bool, default=True,
                         help="whether to use word-level timestamps in output")
 
-    parser.add_argument('--rtl', type=str2bool, default=False,
-                        help="whether to reverse Left-To-Right text into Right-To-Left format for text outputs")
+    parser.add_argument('--reverse_text', type=str2bool, default=False,
+                        help="whether to reverse the order of words for each segment of text output")
 
     # ass output
     parser.add_argument('--font', type=str, default='Arial',
                         help="word font for ASS output(s)")
     parser.add_argument('--font_size', type=int, default=48,
                         help="word font size for ASS output(s)")
 
@@ -829,15 +829,15 @@
     output_format: str = args.pop("output_format")
     overwrite: bool = args.pop("overwrite")
     use_demucs = args.pop('demucs')
     demucs_outputs: List[Optional[str]] = args.pop("demucs_output")
     regroup = args.pop('regroup')
     max_chars = args.pop('max_chars')
     max_words = args.pop('max_words')
-    rtl = args.pop('rtl')
+    reverse_text = args.pop('reverse_text')
 
     if outputs:
         unsupported_formats = set(splitext(o)[-1].lower().strip('.') for o in outputs) - output_formats
         if len(unsupported_formats) != 0:
             raise NotImplementedError(f'{unsupported_formats} are not supported. Supported formats: {outputs}.')
 
     has_demucs_output = bool(demucs_outputs)
@@ -939,15 +939,15 @@
               f'segment_level: {segment_level}\n'
               f'word_level: {word_level}\n'
               f'tag: {tag}\n'
               f'strip: {strip}\n'
               f'regroup: {regroup}\n'
               f'max_chars: {max_chars}\n'
               f'max_words: {max_words}\n'
-              f'rtl: {rtl}\n'
+              f'reverse_text: {reverse_text}\n'
               f'\nArguments for ASS Output',
               f'\nfont: {font}\n'
               f'font_size: {font_size}\n')
 
         print('Input(s)  ->  Outputs(s)')
         for i, (input_audio, output_path) in enumerate(zip(inputs, outputs)):
             dm_output = f' {demucs_outputs[i]} ->' if demucs_outputs else ''
@@ -1007,36 +1007,36 @@
 
         if args.get('word_timestamps'):
             if regroup:
                 result.regroup()
             if max_chars or max_words:
                 result.split_by_length(max_chars=max_chars, max_words=max_words)
 
-        if rtl:
-            rtl = (args.get('prepend_punctuations'), args.get('append_punctuations'))
+        if reverse_text:
+            reverse_text = (args.get('prepend_punctuations'), args.get('append_punctuations'))
         make_parent(output_path)
         if is_json(output_path):
             result.save_as_json(output_path)
         elif output_path.endswith('.srt') or output_path.endswith('.vtt'):
             result.to_srt_vtt(
                 filepath=output_path,
                 segment_level=segment_level,
                 word_level=word_level,
                 tag=tag,
                 strip=strip,
-                rtl=rtl
+                reverse_text=reverse_text
             )
         else:
             result.to_ass(
                 filepath=output_path,
                 segment_level=segment_level,
                 word_level=word_level,
                 tag=tag,
                 font=font,
                 font_size=font_size,
                 strip=strip,
-                rtl=rtl
+                reverse_text=reverse_text
             )
 
 
 if __name__ == '__main__':
     cli()
```

