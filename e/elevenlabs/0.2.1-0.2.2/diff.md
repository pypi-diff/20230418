# Comparing `tmp/elevenlabs-0.2.1.tar.gz` & `tmp/elevenlabs-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabs-0.2.1.tar", last modified: Tue Apr 18 17:02:49 2023, max compression
+gzip compressed data, was "elevenlabs-0.2.2.tar", last modified: Tue Apr 18 20:35:23 2023, max compression
```

## Comparing `elevenlabs-0.2.1.tar` & `elevenlabs-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.743512 elevenlabs-0.2.1/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/elevenlabs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/history.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/tts.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/api/voice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/elevenlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:02:49.743512 elevenlabs-0.2.1/elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 17:02:49.000000 elevenlabs-0.2.1/elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 17:02:49.747512 elevenlabs-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-18 17:02:35.000000 elevenlabs-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/tts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/api/voice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/elevenlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 20:35:23.000000 elevenlabs-0.2.2/elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:35:23.065561 elevenlabs-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 20:35:09.000000 elevenlabs-0.2.2/setup.py
```

### Comparing `elevenlabs-0.2.1/PKG-INFO` & `elevenlabs-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.1
+Version: 0.2.2
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.1/README.md` & `elevenlabs-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 ```bash
 pip install elevenlabs
 ```
 
 ## 🗣️ Usage
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/gist/flavioschneider/49468d728a816c6538fd2f56b3b50b96/elevenlabs-python.ipynb)
+
 ```py
 from elevenlabs import generate, play
 
-text = """ Hi! I'm the world's most advanced text-to-speech system, made by elevenlabs. """
-audio = generate(text)
+audio = generate("Hi! I'm the world's most advanced text-to-speech system, made by elevenlabs.")
+
 play(audio)
 ```
 
 <details> <summary> Play </summary>
 
 <i> Don't forget to unmute the player! </i>
 
@@ -32,17 +33,20 @@
 </details>
 
 ### 👥 Voices
 
 ```py
 from elevenlabs import generate, play
 
-voice = "Adam"
-text = f""" Hi! My name is {voice}, nice to meet you! """
-audio = generate(text, voice=voice)
+voice = "Bella"
+audio = generate(
+  text=f"Hi! My name is {voice}, nice to meet you!",
+  voice=voice
+)
+
 play(audio)
 ```
 
 <details> <summary> Play </summary>
 
 <i> Don't forget to unmute the player! </i>
 
@@ -85,16 +89,19 @@
 </details>
 
 ### 🚿 Streaming
 
 ```py
 from elevenlabs import generate, stream
 
-text = """ This is a... streaming voice!! """
-audio_stream = generate(text, stream=True)
+audio_stream = generate(
+  text="This is a... streaming voice!!",
+  stream=True
+)
+
 stream(audio_stream)
 ```
 
 ### 🔑 API Key
 
 The basic API has a limited number of characters. To increase this limit, you can get a free API key from [Elevenlabs](https://elevenlabs.io/) and set is as environment variable `ELEVEN_API_KEY`. Alternatively pass the `api_key` string argument to the `generate` function, or set it programmatically as:
 ```py
```

### Comparing `elevenlabs-0.2.1/elevenlabs/__init__.py` & `elevenlabs-0.2.2/elevenlabs/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.1/elevenlabs/api/base.py` & `elevenlabs-0.2.2/elevenlabs/api/base.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.1/elevenlabs/api/history.py` & `elevenlabs-0.2.2/elevenlabs/api/history.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.1/elevenlabs/api/tts.py` & `elevenlabs-0.2.2/elevenlabs/api/tts.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.1/elevenlabs/api/voice.py` & `elevenlabs-0.2.2/elevenlabs/api/voice.py`

 * *Files identical despite different names*

### Comparing `elevenlabs-0.2.1/elevenlabs/utils.py` & `elevenlabs-0.2.2/elevenlabs/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,41 +4,59 @@
 import wave
 from collections.abc import Iterator
 from pathlib import Path
 
 from IPython.display import Audio, display
 
 
-def play(audio: bytes, autoplay: bool = True) -> None:
-    display(Audio(audio, rate=44100, autoplay=autoplay))
+def play(audio: bytes, notebook: bool = False) -> None:
+    if notebook:
+        display(Audio(audio, rate=44100, autoplay=True))
+    else:
+        if not is_installed("ffplay"):
+            raise ValueError("ffplay from ffmpeg not found, necessary to play audio.")
+        args = ["ffplay", "-autoexit", "-", "-nodisp"]
+        proc = subprocess.Popen(
+            args=args,
+            stdout=subprocess.PIPE,
+            stdin=subprocess.PIPE,
+            stderr=subprocess.PIPE,
+        )
+        out, err = proc.communicate(input=audio)
+        proc.poll()
 
 
 def save(audio: bytes, filename: str) -> None:
     with wave.open(filename, "w") as f:
         f.setnchannels(2)
         f.setsampwidth(2)
         f.setframerate(44100)
         f.writeframes(audio)
 
 
-def is_mpv_installed() -> bool:
-    mpv = shutil.which("mpv")
-    if mpv is None:
+def is_installed(lib_name: str) -> bool:
+    lib = shutil.which(lib_name)
+    if lib is None:
         return False
-    global_path = Path(mpv)
+    global_path = Path(lib)
     # else check if path is valid and has the correct access rights
     return global_path.exists() and os.access(global_path, os.X_OK)
 
 
 def stream(audio_stream: Iterator[bytes]) -> None:
-    if not is_mpv_installed():
+    if not is_installed("mpv"):
         raise ValueError("mpv not found, necessary to stream audio.")
 
     mpv_command = ["mpv", "--no-cache", "--no-terminal", "--", "fd://0"]
-    mpv_process = subprocess.Popen(mpv_command, stdin=subprocess.PIPE, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    mpv_process = subprocess.Popen(
+        mpv_command,
+        stdin=subprocess.PIPE,
+        stdout=subprocess.DEVNULL,
+        stderr=subprocess.DEVNULL,
+    )
 
     for chunk in audio_stream:
         if chunk is not None:
             mpv_process.stdin.write(chunk)  # type: ignore
             mpv_process.stdin.flush()  # type: ignore
 
     if mpv_process.stdin:
```

### Comparing `elevenlabs-0.2.1/elevenlabs.egg-info/PKG-INFO` & `elevenlabs-0.2.2/elevenlabs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabs
-Version: 0.2.1
+Version: 0.2.2
 Summary: The official elevenlabs python package.
 Home-page: https://github.com/elevenlabs/elevenlabs-python
 Author: Elevenlabs
 Keywords: artificial intelligence,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `elevenlabs-0.2.1/setup.py` & `elevenlabs-0.2.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elevenlabs",
     packages=find_packages(exclude=[]),
-    version="0.2.1",
+    version="0.2.2",
     description="The official elevenlabs python package.",
     long_description_content_type="text/markdown",
     author="Elevenlabs",
     url="https://github.com/elevenlabs/elevenlabs-python",
     keywords=["artificial intelligence", "deep learning"],
-    install_requires=[
-        "pydantic>=1.10",
-    ],
+    install_requires=["pydantic>=1.10", "ipython>=8.0"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
     ],
```

