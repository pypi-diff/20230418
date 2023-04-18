# Comparing `tmp/haystack_memory-0.6.tar.gz` & `tmp/haystack_memory-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haystack_memory-0.6.tar", last modified: Mon Apr 17 19:52:56 2023, max compression
+gzip compressed data, was "haystack_memory-0.7.tar", last modified: Tue Apr 18 16:35:33 2023, max compression
```

## Comparing `haystack_memory-0.6.tar` & `haystack_memory-0.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-04-06 20:01:18.510222 haystack_memory-0.6/LICENSE
--rw-r--r--   0        0        0     5014 2023-04-17 19:43:07.695713 haystack_memory-0.6/README.md
--rw-r--r--   0        0        0        0 2023-04-06 20:01:18.510922 haystack_memory-0.6/haystack_memory/__init__.py
--rw-r--r--   0        0        0     2083 2023-04-06 20:01:18.511075 haystack_memory-0.6/haystack_memory/memory.py
--rw-r--r--   0        0        0     1985 2023-04-16 19:46:09.913105 haystack_memory-0.6/haystack_memory/prompt_templates.py
--rw-r--r--   0        0        0     3544 2023-04-17 17:06:45.888849 haystack_memory-0.6/haystack_memory/utils.py
--rw-r--r--   0        0        0      761 2023-04-17 19:52:56.732312 haystack_memory-0.6/pyproject.toml
--rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 haystack_memory-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-18 16:33:59.537382 haystack_memory-0.7/LICENSE
+-rw-r--r--   0        0        0     4996 2023-04-18 16:33:59.537486 haystack_memory-0.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:33:59.537903 haystack_memory-0.7/haystack_memory/__init__.py
+-rw-r--r--   0        0        0     2083 2023-04-18 16:33:59.537992 haystack_memory-0.7/haystack_memory/memory.py
+-rw-r--r--   0        0        0     1985 2023-04-18 16:33:59.538068 haystack_memory-0.7/haystack_memory/prompt_templates.py
+-rw-r--r--   0        0        0     3550 2023-04-18 16:33:59.538144 haystack_memory-0.7/haystack_memory/utils.py
+-rw-r--r--   0        0        0      761 2023-04-18 16:35:33.109370 haystack_memory-0.7/pyproject.toml
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 haystack_memory-0.7/PKG-INFO
```

### Comparing `haystack_memory-0.6/LICENSE` & `haystack_memory-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `haystack_memory-0.6/README.md` & `haystack_memory-0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Redis implementation featuring a sliding window. On the other hand, the sensory memory is an in-memory implementation that mimics 
 a human's brief sensory memory, lasting only for the duration of one interaction.. 
 
 ## Installation
 
 - Python pip: ```pip install --upgrade haystack-memory``` . This method will attempt to install the dependencies (farm-haystack>=1.15.0, redis)
 - Python pip (skip dependency installation): Use  ```pip install --upgrade haystack-memory --no-deps```
-- Using git: ```pip install git+https://github.com/rolandtannous/HaystackAgentBasicMemory.git@main#egg=HaystackAgentBasicMemory```
+- Using git: ```pip install git+https://github.com/rolandtannous/haystack-memory.git@main#egg=haystack-memory```
 
 
 ## Usage
 
 To use memory in your agent, you need three components:
 - `MemoryRecallNode`: This node is added to the agent as a tool. It will allow the agent to remember the conversation and make query-memory associations.
 - `MemoryUtils`: This class should be used to save the queries and the final agent answers to the conversation memory.
```

### Comparing `haystack_memory-0.6/haystack_memory/memory.py` & `haystack_memory-0.7/haystack_memory/memory.py`

 * *Files identical despite different names*

### Comparing `haystack_memory-0.6/haystack_memory/prompt_templates.py` & `haystack_memory-0.7/haystack_memory/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `haystack_memory-0.6/haystack_memory/utils.py` & `haystack_memory-0.7/haystack_memory/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         Internal function to store the initial query and the answer of the agent to the memory
         :param result: Transcript of the agent
         """
         if not self.__expiration_is_set:
             self.redis.expire(self.memory_id, self.expiration)
             self.__expiration_is_set = True
         self.redis.rpush(self.memory_id, result["query"])
-        self.__transfer_sensory_memory()
+        self.__transfer_sensory_memory(result)
         self.redis.rpush(self.memory_id, result["answers"][0].answer)
 
     def chat(self,
              query: str):
         """
         Function to run a query with the given agent. Stores the results in the memory
         :param query: Query to run with the agent
```

### Comparing `haystack_memory-0.6/pyproject.toml` & `haystack_memory-0.7/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm.build]
 
 [project]
 name = "haystack_memory"
-version = "0.6"
+version = "0.7"
 description = "Memory library for Haystack NLP agents."
 authors = [
     { name = "Florian Brand <github@florianbrand.de>, Roland Tannous, Tuana Celik, recrudesce" },
 ]
 dependencies = [
     "farm-haystack>=1.15.0",
     "redis",
```

### Comparing `haystack_memory-0.6/PKG-INFO` & `haystack_memory-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haystack-memory
-Version: 0.6
+Version: 0.7
 Summary: Memory library for Haystack NLP agents.
 Author: Florian Brand <github@florianbrand.de>, Roland Tannous, Tuana Celik, recrudesce
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/rolandtannous/haystack-memory
@@ -21,15 +21,15 @@
 Redis implementation featuring a sliding window. On the other hand, the sensory memory is an in-memory implementation that mimics 
 a human's brief sensory memory, lasting only for the duration of one interaction.. 
 
 ## Installation
 
 - Python pip: ```pip install --upgrade haystack-memory``` . This method will attempt to install the dependencies (farm-haystack>=1.15.0, redis)
 - Python pip (skip dependency installation): Use  ```pip install --upgrade haystack-memory --no-deps```
-- Using git: ```pip install git+https://github.com/rolandtannous/HaystackAgentBasicMemory.git@main#egg=HaystackAgentBasicMemory```
+- Using git: ```pip install git+https://github.com/rolandtannous/haystack-memory.git@main#egg=haystack-memory```
 
 
 ## Usage
 
 To use memory in your agent, you need three components:
 - `MemoryRecallNode`: This node is added to the agent as a tool. It will allow the agent to remember the conversation and make query-memory associations.
 - `MemoryUtils`: This class should be used to save the queries and the final agent answers to the conversation memory.
```

