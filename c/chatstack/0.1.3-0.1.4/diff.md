# Comparing `tmp/chatstack-0.1.3.tar.gz` & `tmp/chatstack-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatstack-0.1.3.tar", last modified: Fri Mar 31 14:12:47 2023, max compression
+gzip compressed data, was "chatstack-0.1.4.tar", last modified: Tue Apr 18 20:17:12 2023, max compression
```

## Comparing `chatstack-0.1.3.tar` & `chatstack-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-03-31 14:12:47.411468 chatstack-0.1.3/
--rw-r--r--   0 wsk        (501) staff       (20)    11349 2023-03-15 04:39:00.000000 chatstack-0.1.3/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     4275 2023-03-31 14:12:47.411201 chatstack-0.1.3/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     3774 2023-03-31 01:37:45.000000 chatstack-0.1.3/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-03-31 14:12:47.409366 chatstack-0.1.3/chatstack/
--rw-r--r--   0 wsk        (501) staff       (20)      115 2023-03-20 15:51:51.000000 chatstack-0.1.3/chatstack/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)    11423 2023-03-31 14:12:10.000000 chatstack-0.1.3/chatstack/chatstack.py
--rw-r--r--   0 wsk        (501) staff       (20)      393 2023-03-20 19:07:12.000000 chatstack-0.1.3/chatstack/pricing.py
--rw-r--r--   0 wsk        (501) staff       (20)     1786 2023-03-15 04:41:41.000000 chatstack-0.1.3/chatstack/retry.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-03-31 14:12:47.410843 chatstack-0.1.3/chatstack.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     4275 2023-03-31 14:12:47.000000 chatstack-0.1.3/chatstack.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      281 2023-03-31 14:12:47.000000 chatstack-0.1.3/chatstack.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-03-31 14:12:47.000000 chatstack-0.1.3/chatstack.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-03-31 14:12:47.000000 chatstack-0.1.3/chatstack.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-03-31 14:12:47.000000 chatstack-0.1.3/chatstack.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      632 2023-03-31 14:12:22.000000 chatstack-0.1.3/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-03-31 14:12:47.411554 chatstack-0.1.3/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-18 20:17:12.075284 chatstack-0.1.4/
+-rw-r--r--   0 wsk        (501) staff       (20)    11349 2023-03-15 04:39:00.000000 chatstack-0.1.4/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     4275 2023-04-18 20:17:12.075013 chatstack-0.1.4/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     3774 2023-03-31 01:37:45.000000 chatstack-0.1.4/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-18 20:17:12.073317 chatstack-0.1.4/chatstack/
+-rw-r--r--   0 wsk        (501) staff       (20)      115 2023-03-20 15:51:51.000000 chatstack-0.1.4/chatstack/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)    11424 2023-04-17 23:05:00.000000 chatstack-0.1.4/chatstack/chatstack.py
+-rw-r--r--   0 wsk        (501) staff       (20)      393 2023-03-20 19:07:12.000000 chatstack-0.1.4/chatstack/pricing.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1786 2023-03-15 04:41:41.000000 chatstack-0.1.4/chatstack/retry.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-04-18 20:17:12.074679 chatstack-0.1.4/chatstack.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     4275 2023-04-18 20:17:12.000000 chatstack-0.1.4/chatstack.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      281 2023-04-18 20:17:12.000000 chatstack-0.1.4/chatstack.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-04-18 20:17:12.000000 chatstack-0.1.4/chatstack.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-04-18 20:17:12.000000 chatstack-0.1.4/chatstack.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-04-18 20:17:12.000000 chatstack-0.1.4/chatstack.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      632 2023-04-18 20:16:31.000000 chatstack-0.1.4/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-04-18 20:17:12.075375 chatstack-0.1.4/setup.cfg
```

### Comparing `chatstack-0.1.3/LICENSE` & `chatstack-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chatstack-0.1.3/PKG-INFO` & `chatstack-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstack
-Version: 0.1.3
+Version: 0.1.4
 Summary: Message-based LLM tools.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/chatstack
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/chatstack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chatstack-0.1.3/README.md` & `chatstack-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `chatstack-0.1.3/chatstack/chatstack.py` & `chatstack-0.1.4/chatstack/chatstack.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
             chat_messages.append(msg)
             chat_tokens += msg.tokens
         chat_messages.reverse()   # put chat messages back in chronological order
         #logger.info(f'chat messages: {chat_tokens} tokens')
         
         # compute the maximum number of tokens to use for dynamic context
         max_dynamic_context = max_input_context - chat_tokens - self.base_system_msg.tokens
-        logger.info(f'maximum dynamic context: {max_dynamic_context} tokens')
+        #logger.info(f'maximum dynamic context: {max_dynamic_context} tokens')
                 
         # assemble dynamic context up to the token limit
         dynamic_context_messages = []
         dynamic_context = dynamic_context if dynamic_context else []        
         for msg in dynamic_context:
             if msg.tokens > max_dynamic_context:
                 break
```

### Comparing `chatstack-0.1.3/chatstack/retry.py` & `chatstack-0.1.4/chatstack/retry.py`

 * *Files identical despite different names*

### Comparing `chatstack-0.1.3/chatstack.egg-info/PKG-INFO` & `chatstack-0.1.4/chatstack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatstack
-Version: 0.1.3
+Version: 0.1.4
 Summary: Message-based LLM tools.
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/chatstack
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/chatstack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `chatstack-0.1.3/pyproject.toml` & `chatstack-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chatstack"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['pydantic', 'openai', 'tiktoken', 'loguru']
 description = "Message-based LLM tools."
 readme = "README.md"
 requires-python = ">=3.7"
```

