# Comparing `tmp/mmguero-1.0.9.tar.gz` & `tmp/mmguero-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmguero-1.0.9.tar", last modified: Tue Apr 12 14:06:10 2022, max compression
+gzip compressed data, was "mmguero-1.1.0.tar", last modified: Tue Apr 18 18:37:48 2023, max compression
```

## Comparing `mmguero-1.0.9.tar` & `mmguero-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:06:09.995629 mmguero-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-04-12 14:06:00.000000 mmguero-1.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-04-12 14:06:09.995629 mmguero-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-04-12 14:06:00.000000 mmguero-1.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-12 14:06:00.000000 mmguero-1.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      686 2022-04-12 14:06:09.995629 mmguero-1.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:06:09.995629 mmguero-1.0.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:06:09.995629 mmguero-1.0.9/src/mmguero/
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-04-12 14:06:00.000000 mmguero-1.0.9/src/mmguero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2146 2022-04-12 14:06:00.000000 mmguero-1.0.9/src/mmguero/caselessdictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)    24195 2022-04-12 14:06:00.000000 mmguero-1.0.9/src/mmguero/mmguero.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-12 14:06:09.995629 mmguero-1.0.9/src/mmguero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2853 2022-04-12 14:06:09.000000 mmguero-1.0.9/src/mmguero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-04-12 14:06:09.000000 mmguero-1.0.9/src/mmguero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 14:06:09.000000 mmguero-1.0.9/src/mmguero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-12 14:06:08.000000 mmguero-1.0.9/src/mmguero.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-12 14:06:09.000000 mmguero-1.0.9/src/mmguero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-18 18:37:40.000000 mmguero-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-18 18:37:48.947974 mmguero-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-18 18:37:40.000000 mmguero-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 18:37:40.000000 mmguero-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-04-18 18:37:48.947974 mmguero-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.943974 mmguero-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.943974 mmguero-1.1.0/src/mmguero/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/caselessdictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34925 2023-04-18 18:37:40.000000 mmguero-1.1.0/src/mmguero/mmguero.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/src/mmguero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 18:37:48.000000 mmguero-1.1.0/src/mmguero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:37:48.947974 mmguero-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-18 18:37:40.000000 mmguero-1.1.0/tests/test_sample.py
```

### Comparing `mmguero-1.0.9/LICENSE` & `mmguero-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmguero-1.0.9/setup.cfg` & `mmguero-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mmguero
-version = 1.0.9
+version = 1.1.0
 author = Seth Grover
 author_email = mero.mero.guero@gmail.com
 description = Useful helpers by me, for me.
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mmguero/python-mmguero
```

### Comparing `mmguero-1.0.9/src/mmguero/caselessdictionary.py` & `mmguero-1.1.0/src/mmguero/caselessdictionary.py`

 * *Files identical despite different names*

### Comparing `mmguero-1.0.9/src/mmguero/mmguero.py` & `mmguero-1.1.0/src/mmguero/mmguero.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import contextlib
 import getpass
+import hashlib
 import importlib
 import json
 import os
 import platform
 import re
 import socket
 import string
 import sys
+import tempfile
 import time
 
 from base64 import b64decode
 from collections import defaultdict
 from collections.abc import Iterable
+from datetime import datetime
 from enum import IntFlag, auto
 from multiprocessing import RawValue
-from subprocess import PIPE, STDOUT, Popen, CalledProcessError
+from subprocess import PIPE, Popen, CalledProcessError
 from threading import Lock
 
 try:
     from pwd import getpwuid
 except ImportError:
     getpwuid = None
 
@@ -47,14 +50,15 @@
 PLATFORM_LINUX = "Linux"
 PLATFORM_LINUX_CENTOS = "centos"
 PLATFORM_LINUX_DEBIAN = "debian"
 PLATFORM_LINUX_FEDORA = "fedora"
 PLATFORM_LINUX_UBUNTU = "ubuntu"
 PLATFORM_LINUX_RASPBIAN = "raspbian"
 
+
 ###################################################################################################
 class UserInputDefaultsBehavior(IntFlag):
     DefaultsPrompt = auto()
     DefaultsAccept = auto()
     DefaultsNonInteractive = auto()
 
 
@@ -88,30 +92,95 @@
         return self.increment()
 
     def __exit__(self, type, value, traceback):
         return self.decrement()
 
 
 ###################################################################################################
-# chdir to directory as context manager, returning automatically
+# a context manager for entering a directory and leaving it upon leaving the context
 @contextlib.contextmanager
 def pushd(directory):
     prevDir = os.getcwd()
     os.chdir(directory)
     try:
         yield
     finally:
         os.chdir(prevDir)
 
 
 ###################################################################################################
+# a context manager returning a temporary filename which is deleted upon leaving the context
+@contextlib.contextmanager
+def TemporaryFilename(suffix=None):
+    try:
+        f = tempfile.NamedTemporaryFile(suffix=suffix, delete=False)
+        tmp_name = f.name
+        f.close()
+        yield tmp_name
+    finally:
+        os.unlink(tmp_name)
+
+
+###################################################################################################
+# open a file and close it, updating its access time
+def Touch(filename):
+    open(filename, 'a').close()
+    os.utime(filename, None)
+
+
+###################################################################################################
+# read the contents of a file, first assuming text (with encoding), optionally falling back to binary
+def FileContents(filename, encoding='utf-8', binary_fallback=False):
+    if os.path.isfile(filename):
+        decodeErr = False
+
+        try:
+            with open(filename, 'r', encoding=encoding) as f:
+                return f.read()
+        except (UnicodeDecodeError, AttributeError):
+            if binary_fallback:
+                decodeErr = True
+            else:
+                raise
+
+        if decodeErr and binary_fallback:
+            with open(filename, 'rb') as f:
+                return f.read()
+
+    else:
+        return None
+
+
+###################################################################################################
 # print to stderr
 def eprint(*args, **kwargs):
-    print(*args, file=sys.stderr, **kwargs)
-    sys.stderr.flush()
+    filteredArgs = (
+        {k: v for (k, v) in kwargs.items() if k not in ('timestamp', 'flush')} if isinstance(kwargs, dict) else {}
+    )
+    if "timestamp" in kwargs and kwargs["timestamp"]:
+        print(
+            datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            *args,
+            file=sys.stderr,
+            **filteredArgs,
+        )
+    else:
+        print(*args, file=sys.stderr, **filteredArgs)
+    if "flush" in kwargs and kwargs["flush"]:
+        sys.stderr.flush()
+
+
+###################################################################################################
+# print a list of lists into a nice table
+def Tablify(matrix, file=sys.stdout):
+    colMaxLen = {i: max(map(len, inner)) for i, inner in enumerate(zip(*matrix))}
+    for row in matrix:
+        for col, data in enumerate(row):
+            print(f"{data:{colMaxLen[col]}}", end=" | ", file=file)
+        print(file=file)
 
 
 ###################################################################################################
 # convenient boolean argument parsing
 def str2bool(v):
     if isinstance(v, bool):
         return v
@@ -123,28 +192,148 @@
         else:
             raise ValueError("Boolean value expected")
     else:
         raise ValueError("Boolean value expected")
 
 
 ###################################################################################################
+# convenient boolean argument parsing
+def val2bool(v):
+    try:
+        if v is None:
+            return False
+        elif isinstance(v, bool):
+            return v
+        elif isinstance(v, str):
+            if v.lower() in ("yes", "true", "t", "y"):
+                return True
+            elif v.lower() in ("no", "false", "f", "n"):
+                return False
+            else:
+                raise ValueError(f'Boolean value expected (got {v})')
+        else:
+            raise ValueError(f'Boolean value expected (got {v})')
+    except Exception:
+        # just pitch it back and let the caller worry about it
+        return v
+
+
+###################################################################################################
+# urlencode each character of a string
+def AggressiveUrlEncode(val):
+    return "".join("%{0:0>2}".format(format(ord(char), "x")) for char in val)
+
+
+###################################################################################################
+# any character in the string is in string.whitespace
+def ContainsWhitespace(s):
+    return True in [c in s for c in string.whitespace]
+
+
+###################################################################################################
+def CustomMakeTranslation(text, translation):
+    regex = re.compile('|'.join(map(re.escape, translation)))
+    return regex.sub(lambda match: translation[match.group(0)], text)
+
+
+###################################################################################################
+# remove ANSI escape sequences
+def EscapeAnsi(line):
+    ansiEscape = re.compile(r'(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]')
+    return ansiEscape.sub('', line)
+
+
+###################################################################################################
+# EVP_BytesToKey - create key compatible with openssl enc
+# reference: https://github.com/openssl/openssl/blob/6f0ac0e2f27d9240516edb9a23b7863e7ad02898/crypto/evp/evp_key.c#L74
+#            https://gist.github.com/chrono-meter/d122cbefc6f6248a0af554995f072460
+EVP_KEY_SIZE = 32
+OPENSSL_ENC_MAGIC = b'Salted__'
+PKCS5_SALT_LEN = 8
+
+
+def EVP_BytesToKey(key_length: int, iv_length: int, md, salt: bytes, data: bytes, count: int = 1) -> (bytes, bytes):
+    assert data
+    assert salt == b'' or len(salt) == PKCS5_SALT_LEN
+
+    md_buf = b''
+    key = b''
+    iv = b''
+    addmd = 0
+
+    while key_length > len(key) or iv_length > len(iv):
+        c = md()
+        if addmd:
+            c.update(md_buf)
+        addmd += 1
+        c.update(data)
+        c.update(salt)
+        md_buf = c.digest()
+        for i in range(1, count):
+            md_buf = md(md_buf)
+
+        md_buf2 = md_buf
+
+        if key_length > len(key):
+            key, md_buf2 = key + md_buf2[: key_length - len(key)], md_buf2[key_length - len(key) :]
+
+        if iv_length > len(iv):
+            iv = iv + md_buf2[: iv_length - len(iv)]
+
+    return key, iv
+
+
+###################################################################################################
 # safe deep get for a dictionary
 #
 # Example:
 #   d = {'meta': {'status': 'OK', 'status_code': 200}}
 #   DeepGet(d, ['meta', 'status_code'])          # => 200
 #   DeepGet(d, ['garbage', 'status_code'])       # => None
 #   DeepGet(d, ['meta', 'garbage'], default='-') # => '-'
 def DeepGet(d, keys, default=None):
-    assert type(keys) is list
+    k = GetIterable(keys)
     if d is None:
         return default
     if not keys:
         return d
-    return DeepGet(d.get(keys[0]), keys[1:], default)
+    return DeepGet(d.get(k[0]), k[1:], default)
+
+
+###################################################################################################
+# convenience routine for setting-getting a value into a dictionary
+def DeepSet(d, keys, value, deleteIfNone=False):
+    k = GetIterable(keys)
+    for key in k[:-1]:
+        if (key not in d) or (not isinstance(d[key], dict)):
+            d[key] = dict()
+        d = d[key]
+    d[k[-1]] = value
+    if deleteIfNone and (value is None):
+        d.pop(k[-1], None)
+
+
+###################################################################################################
+# recursive dictionary key search
+def DictSearch(d, target):
+    val = filter(
+        None, [[b] if a == target else DictSearch(b, target) if isinstance(b, dict) else None for a, b in d.items()]
+    )
+    return [i for b in val for i in b]
+
+
+###################################################################################################
+# flatten a collection, but don't split strings
+def Flatten(coll):
+    for i in coll:
+        if isinstance(i, Iterable) and not isinstance(i, str):
+            for subc in Flatten(i):
+                yield subc
+        else:
+            yield i
 
 
 ###################################################################################################
 # if the object is an iterable, return it, otherwise return a tuple with it as a single element.
 # useful if you want to user either a scalar or an array in a loop, etc.
 def GetIterable(x):
     if isinstance(x, Iterable) and not isinstance(x, str):
@@ -154,28 +343,27 @@
 
 
 ###################################################################################################
 # attempt to clear the screen
 def ClearScreen():
     try:
         os.system("clear" if platform.system() != PLATFORM_WINDOWS else "cls")
-    except Exception as e:
+    except Exception:
         pass
 
 
 ###################################################################################################
 # get interactive user response to Y/N question
 def YesOrNo(
     question,
     default=None,
     defaultBehavior=UserInputDefaultsBehavior.DefaultsPrompt,
     uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
     clearScreen=False,
 ):
-
     if (default is not None) and (
         (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept)
         and (defaultBehavior & UserInputDefaultsBehavior.DefaultsNonInteractive)
     ):
         reply = ""
 
     elif (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
@@ -185,46 +373,45 @@
         )
         if defaultYes:
             reply = 'y' if (reply == Dialog.OK) else 'n'
         else:
             reply = 'n' if (reply == Dialog.OK) else 'y'
 
     elif uiMode & UserInterfaceMode.InteractionInput:
-
         if (default is not None) and defaultBehavior & UserInputDefaultsBehavior.DefaultsPrompt:
             if str2bool(default):
-                questionStr = f"{question} (Y/n): "
+                questionStr = f"\n{question} (Y/n): "
             else:
-                questionStr = f"{question} (y/N): "
+                questionStr = f"\n{question} (y/N): "
         else:
-            questionStr = f"{question}: "
+            questionStr = f"\n{question}: "
 
         while True:
             reply = str(input(questionStr)).lower().strip()
             if len(reply) > 0:
                 try:
                     str2bool(reply)
                     break
-                except ValueError as e:
+                except ValueError:
                     pass
             elif (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept) and (default is not None):
                 break
 
     else:
         raise RuntimeError("No user interfaces available")
 
     if (len(reply) == 0) and (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept):
         reply = "y" if (default is not None) and str2bool(default) else "n"
 
-    if clearScreen == True:
+    if clearScreen is True:
         ClearScreen()
 
     try:
         return str2bool(reply)
-    except ValueError as e:
+    except ValueError:
         return YesOrNo(
             question,
             default=default,
             uiMode=uiMode,
             defaultBehavior=defaultBehavior - UserInputDefaultsBehavior.DefaultsAccept,
             clearScreen=clearScreen,
         )
@@ -235,15 +422,14 @@
 def AskForString(
     question,
     default=None,
     defaultBehavior=UserInputDefaultsBehavior.DefaultsPrompt,
     uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
     clearScreen=False,
 ):
-
     if (default is not None) and (
         (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept)
         and (defaultBehavior & UserInputDefaultsBehavior.DefaultsNonInteractive)
     ):
         reply = default
 
     elif (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
@@ -257,49 +443,48 @@
             raise RuntimeError("Operation cancelled")
         else:
             reply = reply.strip()
 
     elif uiMode & UserInterfaceMode.InteractionInput:
         reply = str(
             input(
-                f"{question}{f' ({default})' if (default is not None) and (defaultBehavior & UserInputDefaultsBehavior.DefaultsPrompt) else ''}: "
+                f"\n{question}{f' ({default})' if (default is not None) and (defaultBehavior & UserInputDefaultsBehavior.DefaultsPrompt) else ''}: "
             )
         ).strip()
         if (len(reply) == 0) and (default is not None) and (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept):
             reply = default
 
     else:
         raise RuntimeError("No user interfaces available")
 
-    if clearScreen == True:
+    if clearScreen is True:
         ClearScreen()
 
     return reply
 
 
 ###################################################################################################
 # get interactive password (without echoing)
 def AskForPassword(
     prompt,
     uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
     clearScreen=False,
 ):
-
     if (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
         code, reply = MainDialog.passwordbox(prompt, insecure=True)
         if (code == Dialog.CANCEL) or (code == Dialog.ESC):
             raise RuntimeError("Operation cancelled")
 
     elif uiMode & UserInterfaceMode.InteractionInput:
         reply = getpass.getpass(prompt=f"{prompt}: ")
 
     else:
         raise RuntimeError("No user interfaces available")
 
-    if clearScreen == True:
+    if clearScreen is True:
         ClearScreen()
 
     return reply
 
 
 ###################################################################################################
 # Choose one of many.
@@ -310,17 +495,16 @@
 def ChooseOne(
     prompt,
     choices=[],
     defaultBehavior=UserInputDefaultsBehavior.DefaultsPrompt,
     uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
     clearScreen=False,
 ):
-
     validChoices = [x for x in choices if len(x) == 3 and isinstance(x[0], str) and isinstance(x[2], bool)]
-    defaulted = next(iter([x for x in validChoices if x[2] == True]), None)
+    defaulted = next(iter([x for x in validChoices if x[2] is True]), None)
 
     if (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept) and (
         defaultBehavior & UserInputDefaultsBehavior.DefaultsNonInteractive
     ):
         reply = defaulted[0] if defaulted is not None else ""
 
     elif (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
@@ -354,15 +538,15 @@
                 if inputIndex > -1 and inputIndex < len(validChoices):
                     reply = validChoices[inputIndex][0]
                     break
 
     else:
         raise RuntimeError("No user interfaces available")
 
-    if clearScreen == True:
+    if clearScreen is True:
         ClearScreen()
 
     return reply
 
 
 ###################################################################################################
 # Choose multiple of many
@@ -372,17 +556,16 @@
 def ChooseMultiple(
     prompt,
     choices=[],
     defaultBehavior=UserInputDefaultsBehavior.DefaultsPrompt,
     uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
     clearScreen=False,
 ):
-
     validChoices = [x for x in choices if len(x) == 3 and isinstance(x[0], str) and isinstance(x[2], bool)]
-    defaulted = [x[0] for x in validChoices if x[2] == True]
+    defaulted = [x[0] for x in validChoices if x[2] is True]
 
     if (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept) and (
         defaultBehavior & UserInputDefaultsBehavior.DefaultsNonInteractive
     ):
         reply = defaulted
 
     elif (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
@@ -392,15 +575,15 @@
         )
         if code == Dialog.CANCEL or code == Dialog.ESC:
             raise RuntimeError("Operation cancelled")
 
     elif uiMode & UserInterfaceMode.InteractionInput:
         allowedChars = set(string.digits + ',' + ' ')
         defaultValListStr = ",".join(defaulted)
-        print(f"0: NONE")
+        print("0: NONE")
         index = 0
         for choice in validChoices:
             index = index + 1
             print(
                 f"{index}: {choice[0]}{f' - {choice[1]}' if isinstance(choice[1], str) and len(choice[1]) > 0 else ''}"
             )
         while True:
@@ -425,102 +608,224 @@
                         reply.append(validChoices[idx][0])
                 if len(reply) > 0:
                     break
 
     else:
         raise RuntimeError("No user interfaces available")
 
-    if clearScreen == True:
+    if clearScreen is True:
         ClearScreen()
 
     return reply
 
 
 ###################################################################################################
+# display a message to the user without feedback
+def DisplayMessage(
+    message,
+    defaultBehavior=UserInputDefaultsBehavior.DefaultsPrompt,
+    uiMode=UserInterfaceMode.InteractionDialog | UserInterfaceMode.InteractionInput,
+    clearScreen=False,
+):
+    reply = False
+
+    if (defaultBehavior & UserInputDefaultsBehavior.DefaultsAccept) and (
+        defaultBehavior & UserInputDefaultsBehavior.DefaultsNonInteractive
+    ):
+        reply = True
+
+    elif (uiMode & UserInterfaceMode.InteractionDialog) and (MainDialog is not None):
+        code = MainDialog.msgbox(
+            message,
+        )
+        if (code == Dialog.CANCEL) or (code == Dialog.ESC):
+            raise RuntimeError("Operation cancelled")
+        else:
+            reply = True
+
+    else:
+        print(f"\n{message}")
+        reply = True
+
+    if clearScreen is True:
+        ClearScreen()
+
+    return reply
+
+
+###################################################################################################
+# display streaming content via Dialog.programbox
+def DisplayProgramBox(
+    filePath=None,
+    fileFlags=0,
+    fileDescriptor=None,
+    text=None,
+    clearScreen=False,
+):
+    reply = False
+
+    if MainDialog is not None:
+        code = MainDialog.programbox(
+            file_path=filePath,
+            file_flags=fileFlags,
+            fd=fileDescriptor,
+            text=text,
+            width=78,
+            height=20,
+        )
+        if (code == Dialog.CANCEL) or (code == Dialog.ESC):
+            raise RuntimeError("Operation cancelled")
+        else:
+            reply = True
+
+            if clearScreen is True:
+                ClearScreen()
+
+    return reply
+
+
+###################################################################################################
 # decode a string as base64 only if it starts with base64:, otherwise just return
 def Base64DecodeIfPrefixed(s: str):
     if s.startswith('base64:'):
         return b64decode(s[7:]).decode('utf-8')
     else:
         return s
 
 
 ###################################################################################################
+# strip a prefix from the beginning of a string if needed
+def RemovePrefix(text, prefix):
+    if (len(prefix) > 0) and text.startswith(prefix):
+        return text[len(prefix) :]
+    else:
+        return text
+
+
+###################################################################################################
+# strip a suffix from the end of a string if needed
+def RemoveSuffix(text, suffix):
+    if (len(suffix) > 0) and text.endswith(suffix):
+        return text[: len(text) - len(suffix)]
+    else:
+        return text
+
+
+###################################################################################################
+# return true if os.path.samefile, also False on exception
+def SameFileOrDir(path1, path2):
+    try:
+        return os.path.samefile(path1, path2)
+    except Exception:
+        return False
+
+
+###################################################################################################
 # determine if a program/script exists and is executable in the system path
 def Which(cmd, debug=False):
     global HasWhich
     if HasWhich:
         result = which(cmd) is not None
     else:
         result = any(os.access(os.path.join(path, cmd), os.X_OK) for path in os.environ["PATH"].split(os.pathsep))
     if debug:
         eprint(f"Which({HasWhich}) {cmd} returned {result}")
     return result
 
 
 ###################################################################################################
+# calculate a sha256 hash of a file
+def sha256sum(filename):
+    h = hashlib.sha256()
+    b = bytearray(64 * 1024)
+    mv = memoryview(b)
+    with open(filename, 'rb', buffering=0) as f:
+        for n in iter(lambda: f.readinto(mv), 0):
+            h.update(mv[:n])
+    return h.hexdigest()
+
+
+###################################################################################################
 # nice human-readable file sizes
 def SizeHumanFormat(num, suffix="B"):
     for unit in ["", "Ki", "Mi", "Gi", "Ti", "Pi", "Ei", "Zi"]:
         if abs(num) < 1024.0:
             return f"{num:3.1f}{unit}{suffix}"
         num /= 1024.0
     return f"{num:.1f}{'Yi'}{suffix}"
 
 
 ###################################################################################################
 # test if a remote port is open
 def TestSocket(host, port):
-    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
+    with contextlib.closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as sock:
         sock.settimeout(10)
         if sock.connect_ex((host, port)) == 0:
             return True
         else:
             return False
 
 
 ###################################################################################################
-# is this valid json? if so, load and return it
+# return the primary IP (the one with a default route) on the local box
+def GetPrimaryIP():
+    s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+    s.settimeout(0)
+    try:
+        # this IP doesn't have to be reachable
+        s.connect(('10.254.254.254', 1))
+        ip = s.getsockname()[0]
+    except Exception:
+        ip = '127.0.0.1'
+    finally:
+        s.close()
+    return ip
+
+
+###################################################################################################
+# attempt to decode a string as JSON, returning the object if it decodes and None otherwise
 def LoadStrIfJson(jsonStr):
     try:
         return json.loads(jsonStr)
-    except ValueError as e:
+    except ValueError:
         return None
 
 
+###################################################################################################
+# attempt to decode a file (given by handle) as JSON, returning the object if it decodes and
+# None otherwise
 def LoadFileIfJson(fileHandle):
     try:
         return json.load(fileHandle)
-    except ValueError as e:
+    except ValueError:
         return None
 
 
 ###################################################################################################
 # run command with arguments and return its exit code, stdout, and stderr
 def CheckOutputInput(*popenargs, **kwargs):
+    if 'stdout' in kwargs:
+        raise ValueError('stdout argument not allowed, it will be overridden')
 
-    if "stdout" in kwargs:
-        raise ValueError("stdout argument not allowed, it will be overridden")
-
-    if "stderr" in kwargs:
-        raise ValueError("stderr argument not allowed, it will be overridden")
+    if 'stderr' in kwargs:
+        raise ValueError('stderr argument not allowed, it will be overridden')
 
-    if "input" in kwargs and kwargs["input"]:
-        if "stdin" in kwargs:
-            raise ValueError("stdin and input arguments may not both be used")
-        inputdata = kwargs["input"]
-        kwargs["stdin"] = PIPE
+    if 'input' in kwargs and kwargs['input']:
+        if 'stdin' in kwargs:
+            raise ValueError('stdin and input arguments may not both be used')
+        inputdata = kwargs['input']
+        kwargs['stdin'] = PIPE
     else:
         inputdata = None
-    kwargs.pop("input", None)
+    kwargs.pop('input', None)
 
     process = Popen(*popenargs, stdout=PIPE, stderr=PIPE, **kwargs)
     try:
         output, errput = process.communicate(inputdata)
-    except:
+    except Exception:
         process.kill()
         process.wait()
         raise
 
     retcode = process.poll()
 
     return retcode, output, errput
@@ -534,62 +839,84 @@
     stderr=True,
     stdin=None,
     retry=0,
     retrySleepSec=5,
     cwd=None,
     env=None,
     debug=False,
+    logger=None,
 ):
-
     retcode = -1
     output = []
+    flat_command = list(Flatten(GetIterable(command)))
 
     try:
         # run the command
-        retcode, cmdout, cmderr = CheckOutputInput(command, input=stdin.encode() if stdin else stdin, cwd=cwd, env=env)
+        retcode, cmdout, cmderr = CheckOutputInput(
+            flat_command,
+            input=stdin.encode() if stdin else None,
+            cwd=cwd,
+            env=env,
+        )
 
         # split the output on newlines to return a list
         if stderr and (len(cmderr) > 0):
-            output.extend(cmderr.decode(sys.getdefaultencoding()).split("\n"))
+            output.extend(cmderr.decode(sys.getdefaultencoding()).split('\n'))
         if stdout and (len(cmdout) > 0):
-            output.extend(cmdout.decode(sys.getdefaultencoding()).split("\n"))
+            output.extend(cmdout.decode(sys.getdefaultencoding()).split('\n'))
 
-    except (FileNotFoundError, OSError, IOError) as e:
+    except (FileNotFoundError, OSError, IOError):
         if stderr:
-            output.append(f"Command {command} not found or unable to execute")
+            output.append(f"Command {flat_command} not found or unable to execute")
 
     if debug:
-        eprint(f"{command}({stdin[:80] + bool(stdin[80:]) * '...' if stdin else ''}) returned {retcode}: {output}")
+        dbgStr = (
+            f"{flat_command} ({stdin[:80] + bool(stdin[80:]) * '...' if stdin else ''}) returned {retcode}: {output}"
+        )
+        if logger is not None:
+            logger.debug(dbgStr)
+        else:
+            eprint(dbgStr)
 
     if (retcode != 0) and retry and (retry > 0):
         # sleep then retry
         time.sleep(retrySleepSec)
-        return RunProcess(command, stdout, stderr, stdin, retry - 1, retrySleepSec, cwd, env, debug)
+        return RunProcess(
+            flat_command,
+            stdout,
+            stderr,
+            stdin,
+            retry - 1,
+            retrySleepSec,
+            cwd,
+            env,
+            debug,
+            logger,
+        )
     else:
         return retcode, output
 
 
 ###################################################################################################
 # attempt dynamic imports, prompting for install via pip if possible
 DynImports = defaultdict(lambda: None)
 
 
 def DoDynamicImport(importName, pipPkgName, interactive=False, debug=False):
     global DynImports
 
     # see if we've already imported it
     if not DynImports[importName]:
-
         # if not, attempt the import
         try:
             tmpImport = importlib.import_module(importName)
             if tmpImport:
                 DynImports[importName] = tmpImport
                 return DynImports[importName]
-        except ImportError as e:
+        except ImportError:
             pass
 
         # see if we can help out by installing the module
 
         pyPlatform = platform.system()
         pyExec = sys.executable
         pipCmd = "pip3"
@@ -632,20 +959,20 @@
         )
 
     return DynImports[importName]
 
 
 ###################################################################################################
 # download to file
-def DownloadToFile(url, local_filename, chunk_bytes=4096, interactive=False, debug=False):
+def DownloadToFile(url, local_filename, chunk_size=4096, interactive=False, debug=False):
     requests = DoDynamicImport("requests", "requests", interactive=interactive, debug=debug)
 
     r = requests.get(url, stream=True, allow_redirects=True)
     with open(local_filename, "wb") as f:
-        for chunk in r.iter_content(chunk_bytes=chunk_size):
+        for chunk in r.iter_content(chunk_size=chunk_size):
             if chunk:
                 f.write(chunk)
     fExists = os.path.isfile(local_filename)
     fSize = os.path.getsize(local_filename)
     if debug:
         eprint(
             f"Download of {url} to {local_filename} {'succeeded' if fExists else 'failed'} ({SizeHumanFormat(fSize)})"
@@ -695,14 +1022,14 @@
             if os.path.isdir(fullpath):
                 RemoveEmptyFolders(fullpath)
 
     files = os.listdir(path)
     if len(files) == 0 and removeRoot:
         try:
             os.rmdir(path)
-        except:
+        except Exception:
             pass
 
 
 ###################################################################################################
 if __name__ == "__main__":
     eprint("H̵e̷l̷l̵o̸,̸ ̵w̶o̵r̸l̴d̷!̸")
```

