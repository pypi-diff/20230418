# Comparing `tmp/megabots-0.0.8.tar.gz` & `tmp/megabots-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "megabots-0.0.8.tar", last modified: Sat Apr 15 15:18:22 2023, max compression
+gzip compressed data, was "megabots-0.0.9.tar", last modified: Tue Apr 18 19:49:17 2023, max compression
```

## Comparing `megabots-0.0.8.tar` & `megabots-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.451927 megabots-0.0.8/
--rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.8/LICENCE
--rw-r--r--   0 momegas    (501) staff       (20)     4784 2023-04-15 15:18:22.451791 megabots-0.0.8/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)     4311 2023-04-15 12:28:59.000000 megabots-0.0.8/README.md
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.449851 megabots-0.0.8/megabots/
--rw-r--r--   0 momegas    (501) staff       (20)     7219 2023-04-15 15:17:29.000000 megabots-0.0.8/megabots/__init__.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.450607 megabots-0.0.8/megabots.egg-info/
--rw-r--r--   0 momegas    (501) staff       (20)     4784 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/PKG-INFO
--rw-r--r--   0 momegas    (501) staff       (20)      278 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/SOURCES.txt
--rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/dependency_links.txt
--rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/requires.txt
--rw-r--r--   0 momegas    (501) staff       (20)       15 2023-04-15 15:18:22.000000 megabots-0.0.8/megabots.egg-info/top_level.txt
--rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-15 15:18:22.451969 megabots-0.0.8/setup.cfg
--rw-r--r--   0 momegas    (501) staff       (20)      854 2023-04-15 15:18:13.000000 megabots-0.0.8/setup.py
-drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-15 15:18:22.451399 megabots-0.0.8/tests/
--rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.8/tests/__init__.py
--rw-r--r--   0 momegas    (501) staff       (20)      593 2023-04-15 11:10:48.000000 megabots-0.0.8/tests/test_api.py
--rw-r--r--   0 momegas    (501) staff       (20)     1423 2023-04-15 14:44:20.000000 megabots-0.0.8/tests/test_bots.py
--rw-r--r--   0 momegas    (501) staff       (20)      596 2023-04-15 11:12:44.000000 megabots-0.0.8/tests/test_ui.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-18 19:49:17.512524 megabots-0.0.9/
+-rw-r--r--   0 momegas    (501) staff       (20)     1075 2023-04-14 20:57:02.000000 megabots-0.0.9/LICENCE
+-rw-r--r--   0 momegas    (501) staff       (20)     7967 2023-04-18 19:49:17.512361 megabots-0.0.9/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)     7498 2023-04-18 19:39:22.000000 megabots-0.0.9/README.md
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-18 19:49:17.510482 megabots-0.0.9/megabots/
+-rw-r--r--   0 momegas    (501) staff       (20)     7958 2023-04-18 19:46:07.000000 megabots-0.0.9/megabots/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1043 2023-04-18 19:46:39.000000 megabots-0.0.9/megabots/vectorstores.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-18 19:49:17.511197 megabots-0.0.9/megabots.egg-info/
+-rw-r--r--   0 momegas    (501) staff       (20)     7967 2023-04-18 19:49:17.000000 megabots-0.0.9/megabots.egg-info/PKG-INFO
+-rw-r--r--   0 momegas    (501) staff       (20)      303 2023-04-18 19:49:17.000000 megabots-0.0.9/megabots.egg-info/SOURCES.txt
+-rw-r--r--   0 momegas    (501) staff       (20)        1 2023-04-18 19:49:17.000000 megabots-0.0.9/megabots.egg-info/dependency_links.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       63 2023-04-18 19:49:17.000000 megabots-0.0.9/megabots.egg-info/requires.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       15 2023-04-18 19:49:17.000000 megabots-0.0.9/megabots.egg-info/top_level.txt
+-rw-r--r--   0 momegas    (501) staff       (20)       38 2023-04-18 19:49:17.512572 megabots-0.0.9/setup.cfg
+-rw-r--r--   0 momegas    (501) staff       (20)      873 2023-04-18 19:49:07.000000 megabots-0.0.9/setup.py
+drwxr-xr-x   0 momegas    (501) staff       (20)        0 2023-04-18 19:49:17.511958 megabots-0.0.9/tests/
+-rw-r--r--   0 momegas    (501) staff       (20)        0 2023-04-12 18:37:58.000000 megabots-0.0.9/tests/__init__.py
+-rw-r--r--   0 momegas    (501) staff       (20)      593 2023-04-15 11:10:48.000000 megabots-0.0.9/tests/test_api.py
+-rw-r--r--   0 momegas    (501) staff       (20)     1423 2023-04-15 14:44:20.000000 megabots-0.0.9/tests/test_bots.py
+-rw-r--r--   0 momegas    (501) staff       (20)      512 2023-04-16 18:23:41.000000 megabots-0.0.9/tests/test_ui.py
```

### Comparing `megabots-0.0.8/LICENCE` & `megabots-0.0.9/LICENCE`

 * *Files identical despite different names*

### Comparing `megabots-0.0.8/megabots/__init__.py` & `megabots-0.0.9/megabots/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,67 @@
+from typing import Any
 from langchain.llms import OpenAI
 from langchain.chat_models import ChatOpenAI
 from langchain.embeddings import OpenAIEmbeddings
-from langchain.document_loaders import DirectoryLoader, S3DirectoryLoader
 from langchain.chains.qa_with_sources import load_qa_with_sources_chain
 from langchain.vectorstores.faiss import FAISS
 import gradio as gr
 from fastapi import FastAPI
 import pickle
 import os
 from dotenv import load_dotenv
 from langchain.prompts import PromptTemplate
 from langchain.chains.question_answering import load_qa_chain
-from langchain.chains.conversational_retrieval.prompts import (
-    CONDENSE_QUESTION_PROMPT,
-    QA_PROMPT,
-)
+from langchain.chains.conversational_retrieval.prompts import QA_PROMPT
+from langchain.document_loaders import DirectoryLoader
+from megabots.vectorstores import VectorStore, vectorstore
 
 load_dotenv()
 
 
 class Bot:
     def __init__(
         self,
         model: str | None = None,
         prompt_template: str | None = None,
         prompt_variables: list[str] | None = None,
-        memory: str | None = None,
         index: str | None = None,
         sources: bool | None = False,
+        vectorstore: VectorStore | None = None,
+        memory: str | None = None,
         verbose: bool = False,
         temperature: int = 0,
     ):
         self.select_model(model, temperature)
         self.create_loader(index)
-        self.load_or_create_index(index)
+        self.load_or_create_index(index, vectorstore)
 
         # Load the question-answering chain for the selected model
         self.chain = self.create_chain(
-            prompt_template, prompt_variables, verbose=verbose
+            prompt_template, prompt_variables, sources=sources, verbose=verbose
         )
 
     def create_chain(
         self,
         prompt_template: str | None = None,
         prompt_variables: list[str] | None = None,
+        sources: bool | None = False,
         verbose: bool = False,
     ):
         prompt = (
             PromptTemplate(template=prompt_template, input_variables=prompt_variables)
             if prompt_template is not None and prompt_variables is not None
             else QA_PROMPT
         )
+        # TODO: Changing the prompt here is not working. Leave it as is for now.
+        # Reference: https://github.com/hwchase17/langchain/issues/2858
+        if sources:
+            return load_qa_with_sources_chain(
+                self.llm, chain_type="stuff", verbose=verbose
+            )
         return load_qa_chain(
             self.llm, chain_type="stuff", verbose=verbose, prompt=prompt
         )
 
     def select_model(self, model: str | None, temperature: float):
         # Select and set the appropriate model based on the provided input
         if model is None or model == "gpt-3.5-turbo":
@@ -72,26 +79,33 @@
                 """
             Impossible to find a valid index. 
             Either provide a valid path to a pickle file or a directory.               
             """
             )
         self.loader = DirectoryLoader(index, recursive=True)
 
-    def load_or_create_index(self, index_path: str):
+    def load_or_create_index(self, index: str, vectorstore: VectorStore | None = None):
         # Load an existing index from disk or create a new one if not available
+        if vectorstore is not None:
+            self.search_index = vectorstore.client.from_documents(
+                self.loader.load_and_split(),
+                OpenAIEmbeddings(),
+                connection_args={"host": vectorstore.host, "port": vectorstore.port},
+            )
+            return
 
         # Is pickle
-        if index_path is not None and "pkl" in index_path or "pickle" in index_path:
-            print("Loading path from disk...")
-            with open(index_path, "rb") as f:
+        if index is not None and "pkl" in index or "pickle" in index:
+            print("Loading path from pickle file: ", index, "...")
+            with open(index, "rb") as f:
                 self.search_index = pickle.load(f)
             return
 
         # Is directory
-        if index_path is not None and os.path.isdir(index_path):
+        if index is not None and os.path.isdir(index):
             print("Creating index...")
             self.search_index = FAISS.from_documents(
                 self.loader.load_and_split(), OpenAIEmbeddings()
             )
             return
 
         raise RuntimeError(
@@ -114,17 +128,16 @@
 
 
 SUPPORTED_TASKS = {
     "qna-over-docs": {
         "impl": Bot,
         "default": {
             "model": "gpt-3.5-turbo",
-            "prompt": "",
             "temperature": 0,
-            "index": "./files",
+            "index": "./index",
         },
     }
 }
 
 SUPPORTED_MODELS = {}
```

### Comparing `megabots-0.0.8/setup.py` & `megabots-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 setup(
     name="megabots",
     version=VERSION,
     packages=find_packages(),
     install_requires=[
         "langchain",
@@ -16,13 +16,14 @@
     ],
     author="Megaklis Vasilakis",
     author_email="megaklis.vasilakis@gmail.com",
     description="🤖 Megabots provides State-of-the-art, production ready bots made mega-easy, so you don't have to build them from scratch 🤯 Create a bot, now 🫵",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/momegas/megabots",
+    license="MIT",
     classifiers=[
         # Choose appropriate classifiers from
         # https://pypi.org/classifiers/
         "Development Status :: 4 - Beta"
     ],
 )
```

### Comparing `megabots-0.0.8/tests/test_api.py` & `megabots-0.0.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `megabots-0.0.8/tests/test_bots.py` & `megabots-0.0.9/tests/test_bots.py`

 * *Files identical despite different names*

